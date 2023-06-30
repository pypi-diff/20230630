# Comparing `tmp/cryton_core-2022.2.2.tar.gz` & `tmp/cryton_core-2023.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryton_core-2022.2.2.tar", max compression
+gzip compressed data, was "cryton_core-2023.1.2.tar", max compression
```

## Comparing `cryton_core-2022.2.2.tar` & `cryton_core-2023.1.2.tar`

### file list

```diff
@@ -1,242 +1,243 @@
--rw-r--r--   0        0        0     1075 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/LICENSE
--rw-r--r--   0        0        0    22489 2023-02-09 07:57:11.886519 cryton_core-2022.2.2/README.md
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/__init__.py
--rw-r--r--   0        0        0      399 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/asgi.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/__init__.py
--rw-r--r--   0        0        0       63 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/admin.py
--rw-r--r--   0        0        0      167 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/apps.py
--rw-r--r--   0        0        0      526 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/management/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/management/commands/__init__.py
--rw-r--r--   0        0        0      730 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/management/commands/runserver.py
--rw-r--r--   0        0        0     1710 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/management/commands/startgunicorn.py
--rw-r--r--   0        0        0      234 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/management/commands/startlistener.py
--rw-r--r--   0        0        0     1352 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/management/commands/startmonitoring.py
--rw-r--r--   0        0        0    12212 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/cryton_app/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/migrations/__init__.py
--rw-r--r--   0        0        0     4428 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/cryton_app/models.py
--rw-r--r--   0        0        0     6244 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/serializers.py
--rw-r--r--   0        0        0     1628 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/cryton_app/urls.py
--rw-r--r--   0        0        0     5988 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/cryton_app/util.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/__init__.py
--rw-r--r--   0        0        0     1230 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/cryton_app/views/dynamic_run_views.py
--rw-r--r--   0        0        0     3390 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/execution_variable_views.py
--rw-r--r--   0        0        0     2094 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/log_views.py
--rw-r--r--   0        0        0     5626 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/plan_execution_views.py
--rw-r--r--   0        0        0     2451 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/plan_template_views.py
--rw-r--r--   0        0        0     7231 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/plan_views.py
--rw-r--r--   0        0        0    14167 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/run_views.py
--rw-r--r--   0        0        0     4288 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/stage_execution_views.py
--rw-r--r--   0        0        0     6652 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/stage_views.py
--rw-r--r--   0        0        0     3958 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/step_execution_views.py
--rw-r--r--   0        0        0     7075 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/step_views.py
--rw-r--r--   0        0        0     2829 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/cryton_app/views/worker_views.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/etc/__init__.py
--rw-r--r--   0        0        0     2274 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/etc/config.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.852105 cryton_core-2022.2.2/cryton_core/lib/models/__init__.py
--rw-r--r--   0        0        0    23361 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/models/plan.py
--rw-r--r--   0        0        0    13298 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/models/run.py
--rw-r--r--   0        0        0     3522 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/models/session.py
--rw-r--r--   0        0        0    21296 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/models/stage.py
--rw-r--r--   0        0        0    46568 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/models/step.py
--rw-r--r--   0        0        0     3397 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/models/worker.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/services/__init__.py
--rw-r--r--   0        0        0    14970 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/services/listener.py
--rw-r--r--   0        0        0     3861 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/services/scheduler.py
--rw-r--r--   0        0        0     1022 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/triggers/__init__.py
--rw-r--r--   0        0        0     8987 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_base.py
--rw-r--r--   0        0        0     1673 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_datetime.py
--rw-r--r--   0        0        0     1453 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_delta.py
--rw-r--r--   0        0        0     1092 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_http.py
--rw-r--r--   0        0        0     1930 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_msf.py
--rw-r--r--   0        0        0        0 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/util/__init__.py
--rw-r--r--   0        0        0     3317 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/util/constants.py
--rw-r--r--   0        0        0     6559 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/util/creator.py
--rw-r--r--   0        0        0     4754 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/util/event.py
--rw-r--r--   0        0        0    17943 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/util/exceptions.py
--rw-r--r--   0        0        0     4976 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/util/logger.py
--rw-r--r--   0        0        0     8002 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/util/rabbit_client.py
--rw-r--r--   0        0        0     3061 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/util/scheduler_client.py
--rw-r--r--   0        0        0    13190 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/lib/util/states.py
--rw-r--r--   0        0        0    15103 2023-02-09 07:45:58.971248 cryton_core-2022.2.2/cryton_core/lib/util/util.py
--rwxr-xr-x   0        0        0      667 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/manage.py
--rw-r--r--   0        0        0     4370 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/settings.py
--rw-r--r--   0        0        0     9114 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/autocomplete.css
--rw-r--r--   0        0        0    19513 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/base.css
--rw-r--r--   0        0        0     6932 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/changelists.css
--rw-r--r--   0        0        0      380 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/dashboard.css
--rw-r--r--   0        0        0      423 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/fonts.css
--rw-r--r--   0        0        0     8878 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/forms.css
--rw-r--r--   0        0        0      954 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/login.css
--rw-r--r--   0        0        0     2616 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/nav_sidebar.css
--rw-r--r--   0        0        0    18575 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/responsive.css
--rw-r--r--   0        0        0     1741 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/responsive_rtl.css
--rw-r--r--   0        0        0     3234 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/rtl.css
--rw-r--r--   0        0        0     1124 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/vendor/select2/LICENSE-SELECT2.md
--rw-r--r--   0        0        0    17358 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/vendor/select2/select2.css
--rw-r--r--   0        0        0    14966 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/vendor/select2/select2.min.css
--rw-r--r--   0        0        0    11097 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/css/widgets.css
--rw-r--r--   0        0        0    11560 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/fonts/LICENSE.txt
--rw-r--r--   0        0        0      214 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/fonts/README.txt
--rw-r--r--   0        0        0    86184 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/fonts/Roboto-Bold-webfont.woff
--rw-r--r--   0        0        0    85692 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/fonts/Roboto-Light-webfont.woff
--rw-r--r--   0        0        0    85876 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/fonts/Roboto-Regular-webfont.woff
--rw-r--r--   0        0        0     1081 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/img/LICENSE
--rw-r--r--   0        0        0      319 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/img/README.txt
--rw-r--r--   0        0        0     1094 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/img/calendar-icons.svg
--rw-r--r--   0        0        0     1129 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/img/gis/move_vertex_off.svg
--rw-r--r--   0        0        0     1129 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/img/gis/move_vertex_on.svg
--rw-r--r--   0        0        0      331 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-addlink.svg
--rw-r--r--   0        0        0      504 2023-02-08 20:28:30.856105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-alert.svg
--rw-r--r--   0        0        0     1086 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-calendar.svg
--rw-r--r--   0        0        0      380 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-changelink.svg
--rw-r--r--   0        0        0      677 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-clock.svg
--rw-r--r--   0        0        0      392 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-deletelink.svg
--rw-r--r--   0        0        0      560 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-no.svg
--rw-r--r--   0        0        0      655 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-unknown-alt.svg
--rw-r--r--   0        0        0      655 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-unknown.svg
--rw-r--r--   0        0        0      581 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-viewlink.svg
--rw-r--r--   0        0        0      436 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/icon-yes.svg
--rw-r--r--   0        0        0      560 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/inline-delete.svg
--rw-r--r--   0        0        0      458 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/search.svg
--rw-r--r--   0        0        0     3291 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/selector-icons.svg
--rw-r--r--   0        0        0     1097 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/sorting-icons.svg
--rw-r--r--   0        0        0      331 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/tooltag-add.svg
--rw-r--r--   0        0        0      280 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/img/tooltag-arrowright.svg
--rw-r--r--   0        0        0     4360 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/SelectBox.js
--rw-r--r--   0        0        0    12350 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/SelectFilter2.js
--rw-r--r--   0        0        0     7872 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/actions.js
--rw-r--r--   0        0        0    19634 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/admin/DateTimeShortcuts.js
--rw-r--r--   0        0        0     5984 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--   0        0        0     1121 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/autocomplete.js
--rw-r--r--   0        0        0     8466 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/calendar.js
--rw-r--r--   0        0        0      884 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/cancel.js
--rw-r--r--   0        0        0      606 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/change_form.js
--rw-r--r--   0        0        0     1803 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/collapse.js
--rw-r--r--   0        0        0     5698 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/core.js
--rw-r--r--   0        0        0    14969 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/inlines.js
--rw-r--r--   0        0        0      347 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/jquery.init.js
--rw-r--r--   0        0        0     3401 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/nav_sidebar.js
--rw-r--r--   0        0        0      551 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/popup_response.js
--rw-r--r--   0        0        0     1531 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/prepopulate.js
--rw-r--r--   0        0        0      492 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/prepopulate_init.js
--rw-r--r--   0        0        0     7902 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/urlify.js
--rw-r--r--   0        0        0     1097 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/jquery/LICENSE.txt
--rw-r--r--   0        0        0   288580 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/jquery/jquery.js
--rw-r--r--   0        0        0    89501 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/jquery/jquery.min.js
--rw-r--r--   0        0        0     1124 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/LICENSE.md
--rw-r--r--   0        0        0      866 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/af.js
--rw-r--r--   0        0        0      905 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ar.js
--rw-r--r--   0        0        0      721 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/az.js
--rw-r--r--   0        0        0      968 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/bg.js
--rw-r--r--   0        0        0     1291 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/bn.js
--rw-r--r--   0        0        0      965 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/bs.js
--rw-r--r--   0        0        0      900 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ca.js
--rw-r--r--   0        0        0     1292 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/cs.js
--rw-r--r--   0        0        0      828 2023-02-08 20:28:30.860105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/da.js
--rw-r--r--   0        0        0      866 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/de.js
--rw-r--r--   0        0        0     1017 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/dsb.js
--rw-r--r--   0        0        0     1182 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/el.js
--rw-r--r--   0        0        0      844 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/en.js
--rw-r--r--   0        0        0      922 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/es.js
--rw-r--r--   0        0        0      801 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/et.js
--rw-r--r--   0        0        0      868 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/eu.js
--rw-r--r--   0        0        0     1023 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/fa.js
--rw-r--r--   0        0        0      803 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/fi.js
--rw-r--r--   0        0        0      924 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/fr.js
--rw-r--r--   0        0        0      924 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/gl.js
--rw-r--r--   0        0        0      984 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/he.js
--rw-r--r--   0        0        0     1175 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hi.js
--rw-r--r--   0        0        0      852 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hr.js
--rw-r--r--   0        0        0     1018 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hsb.js
--rw-r--r--   0        0        0      831 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hu.js
--rw-r--r--   0        0        0     1028 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hy.js
--rw-r--r--   0        0        0      768 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/id.js
--rw-r--r--   0        0        0      807 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/is.js
--rw-r--r--   0        0        0      897 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/it.js
--rw-r--r--   0        0        0      862 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ja.js
--rw-r--r--   0        0        0     1195 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ka.js
--rw-r--r--   0        0        0     1088 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/km.js
--rw-r--r--   0        0        0      855 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ko.js
--rw-r--r--   0        0        0      944 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/lt.js
--rw-r--r--   0        0        0      900 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/lv.js
--rw-r--r--   0        0        0     1038 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/mk.js
--rw-r--r--   0        0        0      811 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ms.js
--rw-r--r--   0        0        0      778 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/nb.js
--rw-r--r--   0        0        0     1357 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ne.js
--rw-r--r--   0        0        0      904 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/nl.js
--rw-r--r--   0        0        0      947 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/pl.js
--rw-r--r--   0        0        0     1049 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ps.js
--rw-r--r--   0        0        0      876 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/pt-BR.js
--rw-r--r--   0        0        0      878 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/pt.js
--rw-r--r--   0        0        0      938 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ro.js
--rw-r--r--   0        0        0     1171 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ru.js
--rw-r--r--   0        0        0     1306 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sk.js
--rw-r--r--   0        0        0      925 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sl.js
--rw-r--r--   0        0        0      903 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sq.js
--rw-r--r--   0        0        0     1109 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
--rw-r--r--   0        0        0      980 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sr.js
--rw-r--r--   0        0        0      786 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sv.js
--rw-r--r--   0        0        0     1074 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/th.js
--rw-r--r--   0        0        0      771 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/tk.js
--rw-r--r--   0        0        0      775 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/tr.js
--rw-r--r--   0        0        0     1156 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/uk.js
--rw-r--r--   0        0        0      796 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/vi.js
--rw-r--r--   0        0        0      768 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/zh-CN.js
--rw-r--r--   0        0        0      707 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/zh-TW.js
--rw-r--r--   0        0        0   173566 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/select2.full.js
--rw-r--r--   0        0        0    79212 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/select2.full.min.js
--rw-r--r--   0        0        0     1103 2023-02-08 20:28:30.864105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/xregexp/LICENSE.txt
--rw-r--r--   0        0        0   232381 2023-02-08 20:28:30.868105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/xregexp/xregexp.js
--rw-r--r--   0        0        0   125266 2023-02-08 20:28:30.868105 cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/xregexp/xregexp.min.js
--rw-r--r--   0        0        0   866343 2023-02-08 20:28:30.872105 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js
--rw-r--r--   0        0        0     3625 2023-02-08 20:28:30.872105 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js.LICENSE.txt
--rw-r--r--   0        0        0  3061752 2023-02-08 20:28:30.888105 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js.map
--rw-r--r--   0        0        0      628 2023-02-08 20:28:30.888105 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/favicon-32x32.png
--rw-r--r--   0        0        0     2595 2023-02-08 20:28:30.888105 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/oauth2-redirect.html
--rw-r--r--   0        0        0  1080049 2023-02-08 20:28:30.892105 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js
--rw-r--r--   0        0        0    11358 2023-02-08 20:28:30.892105 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0  4281500 2023-02-08 20:28:30.912106 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js.map
--rw-r--r--   0        0        0   319759 2023-02-08 20:28:30.916106 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-standalone-preset.js
--rw-r--r--   0        0        0  1424676 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-standalone-preset.js.map
--rw-r--r--   0        0        0   143858 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui.css
--rw-r--r--   0        0        0   275373 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui.css.map
--rw-r--r--   0        0        0    23411 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/css/bootstrap-theme.min.css
--rw-r--r--   0        0        0     3385 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/css/bootstrap-tweaks.css
--rw-r--r--   0        0        0   121457 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/css/bootstrap.min.css
--rw-r--r--   0        0        0     1152 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/css/default.css
--rw-r--r--   0        0        0    21658 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/css/font-awesome-4.0.3.css
--rw-r--r--   0        0        0      817 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/css/prettify.css
--rw-r--r--   0        0        0     6156 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/css/base.css
--rw-r--r--   0        0        0     1682 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/css/highlight.css
--rw-r--r--   0        0        0     1307 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/css/jquery.json-view.min.css
--rw-r--r--   0        0        0     5430 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/img/favicon.ico
--rw-r--r--   0        0        0     1458 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/img/grid.png
--rw-r--r--   0        0        0    10539 2023-02-08 20:28:30.924106 cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/js/api.js
--rw-r--r--   0        0        0   300764 2023-02-08 20:28:30.928106 cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/js/highlight.pack.js
--rw-r--r--   0        0        0     2700 2023-02-08 20:28:30.928106 cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/js/jquery.json-view.min.js
--rw-r--r--   0        0        0    38205 2023-02-08 20:28:30.928106 cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   202148 2023-02-08 20:28:30.928106 cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0    80652 2023-02-08 20:28:30.928106 cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    44432 2023-02-08 20:28:30.928106 cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    20127 2023-02-08 20:28:30.928106 cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0   108738 2023-02-08 20:28:30.928106 cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    45404 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23424 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0    18028 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0        0        0     8777 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/img/glyphicons-halflings-white.png
--rw-r--r--   0        0        0    12762 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/img/glyphicons-halflings.png
--rw-r--r--   0        0        0     1458 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/img/grid.png
--rw-r--r--   0        0        0     3597 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/js/ajax-form.js
--rw-r--r--   0        0        0    39680 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/js/bootstrap.min.js
--rw-r--r--   0        0        0   157600 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/js/coreapi-0.1.1.js
--rw-r--r--   0        0        0     1719 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/js/csrf.js
--rw-r--r--   0        0        0     1268 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/js/default.js
--rw-r--r--   0        0        0    89476 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/js/jquery-3.5.1.min.js
--rw-r--r--   0        0        0    13632 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/static/rest_framework/js/prettify-min.js
--rw-r--r--   0        0        0     1111 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/urls.py
--rw-r--r--   0        0        0      399 2023-02-08 20:28:30.932106 cryton_core-2022.2.2/cryton_core/wsgi.py
--rw-r--r--   0        0        0     1592 2023-02-09 07:57:11.886519 cryton_core-2022.2.2/pyproject.toml
--rw-r--r--   0        0        0    25642 1970-01-01 00:00:00.000000 cryton_core-2022.2.2/setup.py
--rw-r--r--   0        0        0    24261 1970-01-01 00:00:00.000000 cryton_core-2022.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/LICENSE
+-rw-r--r--   0        0        0     2515 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.166018 cryton_core-2023.1.2/cryton_core/__init__.py
+-rw-r--r--   0        0        0      399 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/asgi.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/cryton_app/__init__.py
+-rw-r--r--   0        0        0       63 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/admin.py
+-rw-r--r--   0        0        0      167 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/apps.py
+-rw-r--r--   0        0        0      526 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/cryton_app/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/cryton_app/management/commands/__init__.py
+-rw-r--r--   0        0        0      730 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/management/commands/runserver.py
+-rw-r--r--   0        0        0     1947 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/management/commands/start.py
+-rw-r--r--   0        0        0     1186 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/management/commands/startgunicorn.py
+-rw-r--r--   0        0        0      234 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/management/commands/startlistener.py
+-rw-r--r--   0        0        0     1352 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/management/commands/startmonitoring.py
+-rw-r--r--   0        0        0    12274 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/cryton_app/migrations/__init__.py
+-rw-r--r--   0        0        0     4474 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/models.py
+-rw-r--r--   0        0        0     6244 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/serializers.py
+-rw-r--r--   0        0        0     1541 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/urls.py
+-rw-r--r--   0        0        0     7343 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/util.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/cryton_app/views/__init__.py
+-rw-r--r--   0        0        0     3390 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/execution_variable_views.py
+-rw-r--r--   0        0        0     2094 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/log_views.py
+-rw-r--r--   0        0        0     5626 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/plan_execution_views.py
+-rw-r--r--   0        0        0     2451 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/plan_template_views.py
+-rw-r--r--   0        0        0     7231 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/plan_views.py
+-rw-r--r--   0        0        0    14167 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/run_views.py
+-rw-r--r--   0        0        0     4288 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/stage_execution_views.py
+-rw-r--r--   0        0        0     6652 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/stage_views.py
+-rw-r--r--   0        0        0     3958 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/step_execution_views.py
+-rw-r--r--   0        0        0     7075 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/step_views.py
+-rw-r--r--   0        0        0     2829 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/cryton_app/views/worker_views.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/etc/__init__.py
+-rw-r--r--   0        0        0     2446 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/etc/config.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/lib/models/__init__.py
+-rw-r--r--   0        0        0    22271 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/lib/models/plan.py
+-rw-r--r--   0        0        0    13298 2023-03-27 14:39:48.113649 cryton_core-2023.1.2/cryton_core/lib/models/run.py
+-rw-r--r--   0        0        0     2698 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/models/session.py
+-rw-r--r--   0        0        0    21642 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/models/stage.py
+-rw-r--r--   0        0        0    47544 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/models/step.py
+-rw-r--r--   0        0        0     3293 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/models/worker.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/lib/services/__init__.py
+-rw-r--r--   0        0        0      590 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/services/gunicorn.py
+-rw-r--r--   0        0        0    14863 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/services/listener.py
+-rw-r--r--   0        0        0     3815 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/services/scheduler.py
+-rw-r--r--   0        0        0     1022 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/triggers/__init__.py
+-rw-r--r--   0        0        0     8987 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_base.py
+-rw-r--r--   0        0        0     1673 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_datetime.py
+-rw-r--r--   0        0        0     1453 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_delta.py
+-rw-r--r--   0        0        0     1092 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_http.py
+-rw-r--r--   0        0        0     1930 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_msf.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:33.170018 cryton_core-2023.1.2/cryton_core/lib/util/__init__.py
+-rw-r--r--   0        0        0     3362 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/util/constants.py
+-rw-r--r--   0        0        0     6559 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/util/creator.py
+-rw-r--r--   0        0        0     4632 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/util/event.py
+-rw-r--r--   0        0        0    17642 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/util/exceptions.py
+-rw-r--r--   0        0        0     4956 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/util/logger.py
+-rw-r--r--   0        0        0     8002 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/util/rabbit_client.py
+-rw-r--r--   0        0        0     2597 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/util/scheduler_client.py
+-rw-r--r--   0        0        0    13190 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/util/states.py
+-rw-r--r--   0        0        0    11839 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/lib/util/util.py
+-rwxr-xr-x   0        0        0      667 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/manage.py
+-rw-r--r--   0        0        0     4370 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/settings.py
+-rw-r--r--   0        0        0     9114 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/static/admin/css/autocomplete.css
+-rw-r--r--   0        0        0    19513 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/static/admin/css/base.css
+-rw-r--r--   0        0        0     6932 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/static/admin/css/changelists.css
+-rw-r--r--   0        0        0      380 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/static/admin/css/dashboard.css
+-rw-r--r--   0        0        0      423 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/static/admin/css/fonts.css
+-rw-r--r--   0        0        0     8878 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/static/admin/css/forms.css
+-rw-r--r--   0        0        0      954 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/static/admin/css/login.css
+-rw-r--r--   0        0        0     2616 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/static/admin/css/nav_sidebar.css
+-rw-r--r--   0        0        0    18575 2023-03-27 14:39:48.117649 cryton_core-2023.1.2/cryton_core/static/admin/css/responsive.css
+-rw-r--r--   0        0        0     1741 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/css/responsive_rtl.css
+-rw-r--r--   0        0        0     3234 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/css/rtl.css
+-rw-r--r--   0        0        0     1124 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/css/vendor/select2/LICENSE-SELECT2.md
+-rw-r--r--   0        0        0    17358 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/css/vendor/select2/select2.css
+-rw-r--r--   0        0        0    14966 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/css/vendor/select2/select2.min.css
+-rw-r--r--   0        0        0    11097 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/css/widgets.css
+-rw-r--r--   0        0        0    11560 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/fonts/LICENSE.txt
+-rw-r--r--   0        0        0      214 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/fonts/README.txt
+-rw-r--r--   0        0        0    86184 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/fonts/Roboto-Bold-webfont.woff
+-rw-r--r--   0        0        0    85692 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/fonts/Roboto-Light-webfont.woff
+-rw-r--r--   0        0        0    85876 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/fonts/Roboto-Regular-webfont.woff
+-rw-r--r--   0        0        0     1081 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/LICENSE
+-rw-r--r--   0        0        0      319 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/README.txt
+-rw-r--r--   0        0        0     1094 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/calendar-icons.svg
+-rw-r--r--   0        0        0     1129 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/gis/move_vertex_off.svg
+-rw-r--r--   0        0        0     1129 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/gis/move_vertex_on.svg
+-rw-r--r--   0        0        0      331 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-addlink.svg
+-rw-r--r--   0        0        0      504 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-alert.svg
+-rw-r--r--   0        0        0     1086 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-calendar.svg
+-rw-r--r--   0        0        0      380 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-changelink.svg
+-rw-r--r--   0        0        0      677 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-clock.svg
+-rw-r--r--   0        0        0      392 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-deletelink.svg
+-rw-r--r--   0        0        0      560 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-no.svg
+-rw-r--r--   0        0        0      655 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-unknown-alt.svg
+-rw-r--r--   0        0        0      655 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-unknown.svg
+-rw-r--r--   0        0        0      581 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-viewlink.svg
+-rw-r--r--   0        0        0      436 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/icon-yes.svg
+-rw-r--r--   0        0        0      560 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/inline-delete.svg
+-rw-r--r--   0        0        0      458 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/search.svg
+-rw-r--r--   0        0        0     3291 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/selector-icons.svg
+-rw-r--r--   0        0        0     1097 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/sorting-icons.svg
+-rw-r--r--   0        0        0      331 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/tooltag-add.svg
+-rw-r--r--   0        0        0      280 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/img/tooltag-arrowright.svg
+-rw-r--r--   0        0        0     4360 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/js/SelectBox.js
+-rw-r--r--   0        0        0    12350 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/js/SelectFilter2.js
+-rw-r--r--   0        0        0     7872 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/js/actions.js
+-rw-r--r--   0        0        0    19634 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/js/admin/DateTimeShortcuts.js
+-rw-r--r--   0        0        0     5984 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0        0        0     1121 2023-03-27 14:39:48.121650 cryton_core-2023.1.2/cryton_core/static/admin/js/autocomplete.js
+-rw-r--r--   0        0        0     8466 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/calendar.js
+-rw-r--r--   0        0        0      884 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/cancel.js
+-rw-r--r--   0        0        0      606 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/change_form.js
+-rw-r--r--   0        0        0     1803 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/collapse.js
+-rw-r--r--   0        0        0     5698 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/core.js
+-rw-r--r--   0        0        0    14969 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/inlines.js
+-rw-r--r--   0        0        0      347 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/jquery.init.js
+-rw-r--r--   0        0        0     3401 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/nav_sidebar.js
+-rw-r--r--   0        0        0      551 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/popup_response.js
+-rw-r--r--   0        0        0     1531 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/prepopulate.js
+-rw-r--r--   0        0        0      492 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/prepopulate_init.js
+-rw-r--r--   0        0        0     7902 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/urlify.js
+-rw-r--r--   0        0        0     1097 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/jquery/LICENSE.txt
+-rw-r--r--   0        0        0   288580 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/jquery/jquery.js
+-rw-r--r--   0        0        0    89501 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/jquery/jquery.min.js
+-rw-r--r--   0        0        0     1124 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/LICENSE.md
+-rw-r--r--   0        0        0      866 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/af.js
+-rw-r--r--   0        0        0      905 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ar.js
+-rw-r--r--   0        0        0      721 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/az.js
+-rw-r--r--   0        0        0      968 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/bg.js
+-rw-r--r--   0        0        0     1291 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/bn.js
+-rw-r--r--   0        0        0      965 2023-03-27 14:39:48.125650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/bs.js
+-rw-r--r--   0        0        0      900 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ca.js
+-rw-r--r--   0        0        0     1292 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/cs.js
+-rw-r--r--   0        0        0      828 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/da.js
+-rw-r--r--   0        0        0      866 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/de.js
+-rw-r--r--   0        0        0     1017 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/dsb.js
+-rw-r--r--   0        0        0     1182 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/el.js
+-rw-r--r--   0        0        0      844 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/en.js
+-rw-r--r--   0        0        0      922 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/es.js
+-rw-r--r--   0        0        0      801 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/et.js
+-rw-r--r--   0        0        0      868 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/eu.js
+-rw-r--r--   0        0        0     1023 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/fa.js
+-rw-r--r--   0        0        0      803 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/fi.js
+-rw-r--r--   0        0        0      924 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/fr.js
+-rw-r--r--   0        0        0      924 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/gl.js
+-rw-r--r--   0        0        0      984 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/he.js
+-rw-r--r--   0        0        0     1175 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hi.js
+-rw-r--r--   0        0        0      852 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hr.js
+-rw-r--r--   0        0        0     1018 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hsb.js
+-rw-r--r--   0        0        0      831 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hu.js
+-rw-r--r--   0        0        0     1028 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hy.js
+-rw-r--r--   0        0        0      768 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/id.js
+-rw-r--r--   0        0        0      807 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/is.js
+-rw-r--r--   0        0        0      897 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/it.js
+-rw-r--r--   0        0        0      862 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ja.js
+-rw-r--r--   0        0        0     1195 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ka.js
+-rw-r--r--   0        0        0     1088 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/km.js
+-rw-r--r--   0        0        0      855 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ko.js
+-rw-r--r--   0        0        0      944 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/lt.js
+-rw-r--r--   0        0        0      900 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/lv.js
+-rw-r--r--   0        0        0     1038 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/mk.js
+-rw-r--r--   0        0        0      811 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ms.js
+-rw-r--r--   0        0        0      778 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/nb.js
+-rw-r--r--   0        0        0     1357 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ne.js
+-rw-r--r--   0        0        0      904 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/nl.js
+-rw-r--r--   0        0        0      947 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/pl.js
+-rw-r--r--   0        0        0     1049 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ps.js
+-rw-r--r--   0        0        0      876 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/pt-BR.js
+-rw-r--r--   0        0        0      878 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/pt.js
+-rw-r--r--   0        0        0      938 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ro.js
+-rw-r--r--   0        0        0     1171 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ru.js
+-rw-r--r--   0        0        0     1306 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sk.js
+-rw-r--r--   0        0        0      925 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sl.js
+-rw-r--r--   0        0        0      903 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sq.js
+-rw-r--r--   0        0        0     1109 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
+-rw-r--r--   0        0        0      980 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sr.js
+-rw-r--r--   0        0        0      786 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sv.js
+-rw-r--r--   0        0        0     1074 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/th.js
+-rw-r--r--   0        0        0      771 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/tk.js
+-rw-r--r--   0        0        0      775 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/tr.js
+-rw-r--r--   0        0        0     1156 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/uk.js
+-rw-r--r--   0        0        0      796 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/vi.js
+-rw-r--r--   0        0        0      768 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/zh-CN.js
+-rw-r--r--   0        0        0      707 2023-03-27 14:39:48.129650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/zh-TW.js
+-rw-r--r--   0        0        0   173566 2023-03-27 14:39:48.133650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/select2.full.js
+-rw-r--r--   0        0        0    79212 2023-03-27 14:39:48.133650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/select2.full.min.js
+-rw-r--r--   0        0        0     1103 2023-03-27 14:39:48.133650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/xregexp/LICENSE.txt
+-rw-r--r--   0        0        0   232381 2023-03-27 14:39:48.133650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/xregexp/xregexp.js
+-rw-r--r--   0        0        0   125266 2023-03-27 14:39:48.133650 cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/xregexp/xregexp.min.js
+-rw-r--r--   0        0        0   866343 2023-03-27 14:39:48.141650 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js
+-rw-r--r--   0        0        0     3625 2023-03-27 14:39:48.141650 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js.LICENSE.txt
+-rw-r--r--   0        0        0  3061752 2023-03-27 14:39:48.153650 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js.map
+-rw-r--r--   0        0        0      628 2023-03-27 14:39:48.153650 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/favicon-32x32.png
+-rw-r--r--   0        0        0     2595 2023-03-27 14:39:48.153650 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/oauth2-redirect.html
+-rw-r--r--   0        0        0  1080049 2023-03-27 14:39:48.161651 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js
+-rw-r--r--   0        0        0    11358 2023-03-27 14:39:48.161651 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0  4281500 2023-03-27 14:39:48.181651 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js.map
+-rw-r--r--   0        0        0   319759 2023-03-27 14:39:48.185651 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-standalone-preset.js
+-rw-r--r--   0        0        0  1424676 2023-03-27 14:39:48.193651 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0        0        0   143858 2023-03-27 14:39:48.193651 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui.css
+-rw-r--r--   0        0        0   275373 2023-03-27 14:39:48.193651 cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui.css.map
+-rw-r--r--   0        0        0    23411 2023-03-27 14:39:48.193651 cryton_core-2023.1.2/cryton_core/static/rest_framework/css/bootstrap-theme.min.css
+-rw-r--r--   0        0        0     3385 2023-03-27 14:39:48.193651 cryton_core-2023.1.2/cryton_core/static/rest_framework/css/bootstrap-tweaks.css
+-rw-r--r--   0        0        0   121457 2023-03-27 14:39:48.193651 cryton_core-2023.1.2/cryton_core/static/rest_framework/css/bootstrap.min.css
+-rw-r--r--   0        0        0     1152 2023-03-27 14:39:48.193651 cryton_core-2023.1.2/cryton_core/static/rest_framework/css/default.css
+-rw-r--r--   0        0        0    21658 2023-03-27 14:39:48.193651 cryton_core-2023.1.2/cryton_core/static/rest_framework/css/font-awesome-4.0.3.css
+-rw-r--r--   0        0        0      817 2023-03-27 14:39:48.193651 cryton_core-2023.1.2/cryton_core/static/rest_framework/css/prettify.css
+-rw-r--r--   0        0        0     6156 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/css/base.css
+-rw-r--r--   0        0        0     1682 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/css/highlight.css
+-rw-r--r--   0        0        0     1307 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/css/jquery.json-view.min.css
+-rw-r--r--   0        0        0     5430 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/img/favicon.ico
+-rw-r--r--   0        0        0     1458 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/img/grid.png
+-rw-r--r--   0        0        0    10539 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/js/api.js
+-rw-r--r--   0        0        0   300764 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/js/highlight.pack.js
+-rw-r--r--   0        0        0     2700 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/js/jquery.json-view.min.js
+-rw-r--r--   0        0        0    38205 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   202148 2023-03-27 14:39:48.197651 cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0    80652 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    44432 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    20127 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0   108738 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    45404 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23424 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    18028 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0        0        0     8777 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/img/glyphicons-halflings-white.png
+-rw-r--r--   0        0        0    12762 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/img/glyphicons-halflings.png
+-rw-r--r--   0        0        0     1458 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/img/grid.png
+-rw-r--r--   0        0        0     3597 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/js/ajax-form.js
+-rw-r--r--   0        0        0    39680 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/js/bootstrap.min.js
+-rw-r--r--   0        0        0   157600 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/js/coreapi-0.1.1.js
+-rw-r--r--   0        0        0     1719 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/js/csrf.js
+-rw-r--r--   0        0        0     1268 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/js/default.js
+-rw-r--r--   0        0        0    89476 2023-03-27 14:39:48.201651 cryton_core-2023.1.2/cryton_core/static/rest_framework/js/jquery-3.5.1.min.js
+-rw-r--r--   0        0        0    13632 2023-03-27 14:39:48.205651 cryton_core-2023.1.2/cryton_core/static/rest_framework/js/prettify-min.js
+-rw-r--r--   0        0        0     1111 2023-03-27 14:39:48.205651 cryton_core-2023.1.2/cryton_core/urls.py
+-rw-r--r--   0        0        0      399 2023-03-27 14:39:48.205651 cryton_core-2023.1.2/cryton_core/wsgi.py
+-rw-r--r--   0        0        0     1628 2023-03-27 15:00:51.957267 cryton_core-2023.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cryton_core-2023.1.2/setup.py
+-rw-r--r--   0        0        0     4273 1970-01-01 00:00:00.000000 cryton_core-2023.1.2/PKG-INFO
```

### Comparing `cryton_core-2022.2.2/LICENSE` & `cryton_core-2023.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/exceptions.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/exceptions.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/management/commands/runserver.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/management/commands/startgunicorn.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/management/commands/start.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 from threading import Thread
 from django.core.management.base import BaseCommand
-from gunicorn.app.base import BaseApplication
+from click import echo
 
 from cryton_core.asgi import application
+from cryton_core.lib.services.gunicorn import GunicornApplication
+from cryton_core.lib.services.listener import Listener
 from cryton_core.lib.util.logger import logger_object
 
 
-class GunicornApplication(BaseApplication):
-
-    def __init__(self, app, options=None):
-        self.options = options or {}
-        self.application = app
-        super().__init__()
-
-    def init(self, parser, opts, args):
-        pass
-
-    def load_config(self):
-        config = {key: value for key, value in self.options.items()
-                  if key in self.cfg.settings and value is not None}
-        for key, value in config.items():
-            self.cfg.set(key.lower(), value)
-
-    def load(self):
-        return self.application
-
-
 class Command(BaseCommand):
 
     def add_arguments(self, parser):
         parser.add_argument("--bind", type=str, help="ADDRESS:PORT to serve the server at.")
         parser.add_argument("--workers", type=int, help="The NUMBER of worker processes for handling requests.")
 
     def handle(self, *args, **options):
+        """
+        Starts logger processor, listener, and gunicorn app.
+        :param args: Arguments passed to the handle
+        :param options: Options passed to the handle
+        :return: None
+        """
         hard_options = {
             "bind": options.get("bind", "0.0.0.0:8000"),
             "worker_class": "uvicorn.workers.UvicornWorker",
             "workers": options.get("workers", 2)
         }
 
+        echo("Set up... ", nl=False)
         gunicorn_app = GunicornApplication(application, hard_options)
+        listener = Listener()
 
         # Start log_handler in a thread to ensure the logs from multiprocessing aren't missing
         logger_processor_thread = Thread(target=logger_object.log_handler)
         logger_processor_thread.start()
+        echo("OK")
 
         try:
+            echo("Starting RabbitMQ listener... ", nl=False)
+            listener.begin()
+            echo("OK")
             gunicorn_app.run()
-        finally:  # Ensure the log_handler will stop
-            logger_object.log_queue.put(None)
+        finally:
+            echo("Stopping REST API... OK")  # Gunicorn doesn't have user-friendly output
+            echo("Stopping RabbitMQ listener... ", nl=False)
+            listener.stop()
+            echo("OK")
+
+            echo("Cleaning up... ", nl=False)
+            logger_object.log_queue.put(None)  # Ensure the log_handler will stop
+            echo("OK")
```

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/management/commands/startmonitoring.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/management/commands/startmonitoring.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/migrations/0001_initial.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.0.6 on 2022-07-21 12:12
+# Generated by Django 4.0.7 on 2023-01-31 19:41
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
@@ -34,14 +34,15 @@
             name='PlanModel',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('updated_at', models.DateTimeField(auto_now=True)),
                 ('name', models.TextField()),
                 ('owner', models.TextField()),
+                ('settings', models.JSONField(default=dict)),
                 ('dynamic', models.BooleanField(default=False)),
             ],
             options={
                 'abstract': False,
             },
         ),
         migrations.CreateModel(
@@ -134,16 +135,16 @@
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('updated_at', models.DateTimeField(auto_now=True)),
                 ('state', models.TextField(default='PENDING')),
                 ('start_time', models.DateTimeField(null=True)),
                 ('pause_time', models.DateTimeField(null=True)),
                 ('finish_time', models.DateTimeField(null=True)),
                 ('result', models.TextField(default='')),
-                ('output', models.TextField(default='')),
                 ('serialized_output', models.JSONField(default=dict)),
+                ('output', models.TextField(default='')),
                 ('valid', models.BooleanField(default=False)),
                 ('parent_id', models.IntegerField(null=True)),
                 ('stage_execution', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='step_executions', to='cryton_app.stageexecutionmodel')),
                 ('step_model', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='step_executions', to='cryton_app.stepmodel')),
             ],
             options={
                 'abstract': False,
```

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/models.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
     class Meta:
         abstract = True
 
 
 class PlanModel(InstanceModel):
     owner = models.TextField()
+    settings = models.JSONField(default=dict)
     dynamic = models.BooleanField(default=False)
 
 
 class StageModel(InstanceModel):
     plan_model = models.ForeignKey(PlanModel, on_delete=models.CASCADE, related_name='stages')
     trigger_type = models.TextField()
     trigger_args = models.JSONField()
```

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/serializers.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/serializers.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/urls.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 router.register(r'stage_executions', stage_execution_views.StageExecutionViewSet)
 router.register(r'steps', step_views.StepViewSet)
 router.register(r'step_executions', step_execution_views.StepExecutionViewSet)
 router.register(r'workers', worker_views.WorkerViewSet)
 router.register(r'templates', plan_template_views.PlanTemplateViewSet)
 router.register(r'execution_variables', execution_variable_views.ExecutionVariableViewSet)
 router.register(r'logs', log_views.LogViewSet, "log")
-# router.register(r'dynamic_runs', dynamic_run_views.DynamicRunViewSet, "dynamic_run")
 
 
 urlpatterns = [
     path('', router.get_api_root_view()),
     path('', include(router.urls)),
     path('schema/', SpectacularAPIView.as_view(), name='schema'),
     path('schema/swagger-ui/', SpectacularSwaggerView.as_view(url_name='schema'), name='swagger-ui'),
```

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/util.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from datetime import datetime
 import yaml
+import configparser
+import json
 import pytz
+from jinja2 import nativetypes, DebugUndefined, ChainableUndefined, UndefinedError
 
 from rest_framework.viewsets import GenericViewSet, mixins
 from django.db.models.query import QuerySet
 from django.utils.datastructures import MultiValueDict
 
 from cryton_core.cryton_app import exceptions
-from cryton_core.lib.util import util as core_util, constants, exceptions as core_exceptions
+from cryton_core.lib.util import util as core_util, constants
 
 
 def filter_decorator(func):
     """
     Decorator for filtering of serializer results.
     :param func:
     :return: Filtered queryset
@@ -81,51 +84,95 @@
         start_time = core_util.convert_to_utc(start_time, time_zone)
     except pytz.UnknownTimeZoneError:
         raise exceptions.ValidationError("Defined 'time_zone' is not supported!")
 
     return start_time
 
 
+def parse_inventory(inventory: str) -> dict:
+    """
+    Reads inventory file (JSON, YAML, INI) and returns it as a dictionary
+    :param inventory: Inventory file content
+    :return: Inventory variables
+    """
+    # JSON
+    try:
+        return json.loads(inventory)
+    except json.decoder.JSONDecodeError:
+        pass
+
+    # YAML
+    try:
+        return yaml.safe_load(inventory)
+    except yaml.YAMLError:
+        pass
+
+    # INI
+    try:
+        config_parser = configparser.ConfigParser()
+        config_parser.read_string(inventory)
+        return {section: dict(config_parser.items(section)) for section in config_parser.sections()}
+    except configparser.Error:
+        pass
+
+    raise ValueError(f"Inventory file must contain data and be of type JSON, YAML, or INI. File: {inventory}")
+
+
 def get_inventory_variables_from_files(files: MultiValueDict) -> dict:
     """
     Get all inventory variables from input.
     :param files: Files to parse
     :return: All inventory variables
     """
     # Get inventory files from request and load them
     inventory_variables = {}
     for inventory_file in files.values():
         file_content = inventory_file.read()
         if isinstance(file_content, bytes):
             file_content = file_content.decode("utf-8")
 
         try:
-            inventory_variables.update(core_util.parse_inventory(file_content))
+            inventory_variables.update(parse_inventory(file_content))
         except ValueError as ex:
             raise exceptions.ValidationError(f"Cannot read inventory file. Original exception: {ex}. "
                                              f"Inventory file: {inventory_file}.")
 
     return inventory_variables
 
 
+class IgnoreNestedUndefined(ChainableUndefined, DebugUndefined):
+    def __getattr__(self, attr: str) -> "IgnoreNestedUndefined":
+        self._undefined_name += f'.{attr}'
+
+        return self
+
+    def __getitem__(self, item: str) -> "IgnoreNestedUndefined":
+        self._undefined_name += f'[{item}]'
+
+        return self
+
+
 def fill_template(inventory_variables: dict, template: str) -> str:
     """
-    Fill template (if there are any inventory variables).
+    Fill Jinja variables in the template (if there are any inventory variables).
     :param inventory_variables: Template variables to fill the template with
     :param template: Template to fill
     :return: Filled template
     """
     # Either fill the Plan template or consider the template already filled
     if inventory_variables == {}:
         return template
 
+    env = nativetypes.NativeEnvironment(undefined=IgnoreNestedUndefined)
+
     try:
-        return core_util.fill_template(template, inventory_variables)
-    except core_exceptions.ValidationError as ex:
-        raise exceptions.ValidationError(f"File is not a template, original exception: {ex}")
+        plan_template_obj = env.from_string(template)
+        return plan_template_obj.render(**inventory_variables)
+    except (TypeError, UndefinedError) as ex:
+        raise exceptions.ValidationError(f"File is not a valid Jinja template, original exception: {ex}")
 
 
 def parse_object_from_files(files: MultiValueDict) -> dict:
     """
     Get serialized object from input - parse template and fill it with inventory variables.
     :param files: Input files
     :return: Serialized object
```

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/execution_variable_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/execution_variable_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/log_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/log_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/plan_execution_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/plan_execution_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/plan_template_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/plan_template_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/plan_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/plan_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/run_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/run_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/stage_execution_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/stage_execution_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/stage_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/stage_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/step_execution_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/step_execution_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/step_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/step_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/cryton_app/views/worker_views.py` & `cryton_core-2023.1.2/cryton_core/cryton_app/views/worker_views.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/models/plan.py` & `cryton_core-2023.1.2/cryton_core/lib/models/plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from schema import Schema, Optional as SchemaOptional, SchemaError
 from multiprocessing import Process
 
 from cryton_core.cryton_app.models import PlanModel, PlanExecutionModel, StageExecutionModel
 from cryton_core.etc import config
 
-from cryton_core.lib.util import constants as co, exceptions, logger, scheduler_client, states as st, util
+from cryton_core.lib.util import constants, exceptions, logger, scheduler_client, states as st
 from cryton_core.lib.models import worker
 from cryton_core.lib.models.stage import StageExecution, Stage
 from django.utils import timezone
 
 
 class Plan:
     def __init__(self, **kwargs):
@@ -68,14 +68,24 @@
 
     @dynamic.setter
     def dynamic(self, value: bool):
         model = self.model
         model.dynamic = value
         model.save()
 
+    @property
+    def settings(self) -> dict:
+        return self.model.settings
+
+    @settings.setter
+    def settings(self, value: dict):
+        model = self.model
+        model.settings = value
+        model.save()
+        
     @staticmethod
     def filter(**kwargs) -> QuerySet:
         """
         List PlanModel objects fulfilling fields specified in kwargs.
         If no such fields are specified all objects are returned.
         :param kwargs: dict of field-value pairs to filter by
         :raises WrongParameterError: invalid field is specified
@@ -105,52 +115,56 @@
         for stage_dict in plan_dict.get('stages'):
             # validate unique stage names in plan
             if (stage_name := stage_dict['name']) in stage_names:
                 raise exceptions.DuplicateNameInPlan(unique_argument="Stage", duplicate_name=stage_name,
                                                      plan_name=plan_dict.get("name"))
             stage_names.append(stage_name)
 
-            if stage_dict.get(co.TRIGGER_TYPE) == co.MSF_LISTENER:
+            if stage_dict.get(constants.TRIGGER_TYPE) == constants.MSF_LISTENER:
                 session_names.append(f"{stage_name}_session")
 
             for step in stage_dict.get('steps'):
                 # validate unique step names in plan
                 if (step_name := step['name']) in step_names:
                     raise exceptions.DuplicateNameInPlan(unique_argument="Step", duplicate_name=step_name,
                                                          plan_name=plan_dict.get("name"))
                 step_names.append(step_name)
 
                 # validate unique empire agent names in plan
-                if step[co.STEP_TYPE] == co.STEP_TYPE_DEPLOY_AGENT:
-                    if (agent_name := step[co.ARGUMENTS][co.AGENT_NAME]) in agent_names:
+                if step[constants.STEP_TYPE] == constants.STEP_TYPE_DEPLOY_AGENT:
+                    if (agent_name := step[constants.ARGUMENTS][constants.AGENT_NAME]) in agent_names:
                         raise exceptions.DuplicateNameInPlan(unique_argument="Empire Agent", duplicate_name=agent_name,
                                                              plan_name=plan_dict.get("name"))
                     agent_names.append(agent_name)
 
-                if co.CREATE_NAMED_SESSION in step[co.ARGUMENTS]:
-                    if (session_name := step[co.ARGUMENTS][co.CREATE_NAMED_SESSION]) in session_names:
+                if constants.CREATE_NAMED_SESSION in step[constants.ARGUMENTS]:
+                    if (session_name := step[constants.ARGUMENTS][constants.CREATE_NAMED_SESSION]) in session_names:
                         raise exceptions.DuplicateNameInPlan(unique_argument="Session", duplicate_name=session_name,
                                                              plan_name=plan_dict.get("name"))
                     session_names.append(session_name)
 
     @staticmethod
     def validate(plan_dict, dynamic: bool = False) -> None:
         """
-        Check if plan's dictionary is valid:param plan_dict: Plan information
+        Check if plan's dictionary is valid
+        :param plan_dict: Plan information
         :param dynamic: If the Plan is static or dynamic
         :raises
             exceptions.PlanValidationError:
             exceptions.StageValidationError
             exceptions.StepValidationError
         :return: True if dictionary is valid
         """
         conf_schema = Schema({
             "name": str,
             SchemaOptional("owner"): str,
             SchemaOptional("dynamic"): bool,
+            SchemaOptional('settings'): {
+                SchemaOptional(constants.SEPARATOR): str
+            },
             "stages": list
         })
 
         try:
             logger.logger.debug("Validating plan", plan_name=plan_dict.get('name'))
             conf_schema.validate(plan_dict)
         except SchemaError as ex:
@@ -401,34 +415,14 @@
         if new_time < timezone.now():
             raise exceptions.UserInputError("Time argument must be greater or equal than current time.", str(new_time))
 
         self.unschedule()
         self.schedule(new_time)
         logger.logger.info("Plan execution rescheduled", plan_execution_id=self.model.id, status='success')
 
-    # TODO: never used; deprecated?
-    def postpone(self, delta: str):
-        """
-        Postpone plan execution.
-        :param delta: Time to postpone by, in [int]h[int]m[int]s format
-        :raises UserInputError: when provided delta is in incorrect format
-        :return: None
-        """
-        logger.logger.debug("Postponing Plan", plan_execution_id=self.model.id)
-        st.PlanStateMachine(self.model.id).validate_state(self.state, st.PLAN_POSTPONE_STATES)
-
-        original_schedule_time = self.schedule_time
-        delta = util.parse_delta_to_datetime(delta)
-
-        schedule_time = original_schedule_time + delta
-
-        self.unschedule()
-        self.schedule(schedule_time)
-        logger.logger.info("Plan execution postponed", plan_execution_id=self.model.id, status='success')
-
     def pause(self) -> None:
         """
         Pause plan execution.
         :return: None
         """
         logger.logger.debug("Pausing Plan", plan_execution_id=self.model.id)
         st.PlanStateMachine(self.model.id).validate_state(self.state, st.PLAN_PAUSE_STATES)
@@ -449,15 +443,15 @@
         st.PlanStateMachine(self.model.id).validate_state(self.state, st.PLAN_UNPAUSE_STATES)
 
         self.pause_time = None
         self.state = st.RUNNING
 
         for stage_execution_model in self.model.stage_executions.all():
             stage_ex = StageExecution(stage_execution_id=stage_execution_model.id)
-            if stage_ex.model.stage_model.trigger_type == co.DELTA and stage_ex.state in st.STAGE_SCHEDULE_STATES:
+            if stage_ex.model.stage_model.trigger_type == constants.DELTA and stage_ex.state in st.STAGE_SCHEDULE_STATES:
                 stage_ex.trigger.schedule()
             else:
                 try:
                     stage_ex.trigger.unpause()
                 except exceptions.StageInvalidStateError:
                     pass
 
@@ -485,27 +479,14 @@
         for stage_execution_model in self.model.stage_executions.all():
             stage_execution = StageExecution(stage_execution_id=stage_execution_model.id)
             stage_execution.trigger.start()
             logger.logger.debug("Trigger started", plan_execution_id=self.model.id,
                                 trigger=str(stage_execution.trigger))
         logger.logger.info("Triggers started", plan_execution_id=self.model.id, status='success')
 
-    def stop_triggers(self) -> None:
-        """
-        Stop triggers for all execution stages. Also unschedules delta types.
-        :return: None
-        """
-        logger.logger.debug("Stopping triggers", plan_execution_id=self.model.id)
-        for stage_execution_model in self.model.stage_executions.all():
-            stage_execution = StageExecution(stage_execution_id=stage_execution_model.id)
-            stage_execution.trigger.stop()
-            logger.logger.debug("Trigger stopped", plan_execution_id=self.model.id,
-                                trigger=str(stage_execution.trigger))
-        logger.logger.info("Triggers stopped", plan_execution_id=self.model.id, status='success')
-
     @staticmethod
     def filter(**kwargs) -> QuerySet:
         """
         List PlanExecutionModel objects fulfilling fields specified in kwargs.
         If no such fields are specified all objects are returned.
         :param kwargs: dict of field-value pairs to filter by
         :return: Queryset of PlanExecutionModel objects
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/models/run.py` & `cryton_core-2023.1.2/cryton_core/lib/models/run.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/models/session.py` & `cryton_core-2023.1.2/cryton_core/lib/models/session.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,37 +40,14 @@
     logger.logger.debug("Getting session id", session_name=session_name)
     try:
         return SessionModel.objects.get(name=session_name, plan_execution_id=plan_execution_id).msf_id
     except ObjectDoesNotExist as ex:
         raise exceptions.SessionObjectDoesNotExist(ex, session_name=session_name, plan_execution_id=plan_execution_id)
 
 
-def set_msf_session_id(session_name: str,
-                       msf_session_id: str,
-                       plan_execution_id: Union[Type[int], int]) -> int:
-    """
-    Update metasploit session ID
-
-    :param int plan_execution_id: ID of the desired plan execution
-    :param msf_session_id: Metasploit session ID
-    :param str session_name: Session name
-    :return: ID of the named session
-    """
-
-    try:
-        named_session = SessionModel.objects.get(name=session_name, plan_execution_id=plan_execution_id)
-    except ObjectDoesNotExist as ex:
-        raise exceptions.SessionObjectDoesNotExist(ex, session_name=session_name,
-                                                   plan_execution_id=plan_execution_id)
-    named_session.msf_id = msf_session_id
-    named_session.save()
-
-    return named_session.id
-
-
 # TODO: has to be fixed, since there is no `target_ip` argument in sessions details
 def get_session_ids(target_ip: str, plan_execution_id: Union[Type[int], int]) -> list:
     """
     Get list of session IDs to specified IP
 
     :param str target_ip: Target IP
     :param int plan_execution_id: ID of the desired Plan execution
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/models/stage.py` & `cryton_core-2023.1.2/cryton_core/lib/models/stage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Type, Optional
+from typing import Union, Type, Optional, List
 from datetime import datetime
 from django.utils import timezone
 from schema import Schema, SchemaError, Or, Optional as SchemaOptional
 import copy
 from threading import Thread
 
 from django.db.models.query import QuerySet
@@ -394,14 +394,34 @@
         :return: None
         """
         step_execution_kwargs = {'stage_execution': self.model}
         for step_obj in self.model.stage_model.steps.all():
             step_execution_kwargs.update({'step_model': step_obj})
             StepExecution(**step_execution_kwargs)
 
+    @staticmethod
+    def _run_step_executions(step_executions: List[StepExecution]):
+        """
+        Evenly distribute Step executions and run each batch in a Process.
+        :param step_executions: Step executions to be distributed into Processes
+        :return: None
+        """
+        # Evenly distribute StepExecutions into processes.
+        step_exec_lists = list(util.split_into_lists(step_executions, config.CPU_CORES))
+        processes = []
+        for step_executions in step_exec_lists:
+            if step_executions:
+                processes.append(logger.LoggedProcess(logg_queue=logger.logger_object.log_queue,
+                                                      target=util.run_executions_in_threads, args=(step_executions,)))
+
+        # Close django db connections and run processes
+        connections.close_all()
+        for process in processes:
+            process.start()
+
     def execute(self) -> None:
         """
         Check if all requirements for execution are met, get init steps and execute them.
         :return: None
         """
         logger.logger.debug("Executing Stage", stage_execution_id=self.model.id)
         st.StageStateMachine(self.model.id).validate_state(self.state, st.STAGE_EXECUTE_STATES)
@@ -426,26 +446,15 @@
             return
 
         # Update state and time
         if self.start_time is None:
             self.start_time = timezone.now()
         self.state = st.RUNNING
 
-        # Evenly distribute StepExecutions into processes.
-        step_exec_lists = list(util.split_into_lists(step_executions, config.CPU_CORES))
-        processes = []
-        for step_executions in step_exec_lists:
-            if step_executions:
-                processes.append(logger.LoggedProcess(logg_queue=logger.logger_object.log_queue,
-                                                      target=util.run_executions_in_threads, args=(step_executions,)))
-
-        # Close django db connections and run processes
-        connections.close_all()
-        for process in processes:
-            process.start()
+        self._run_step_executions(step_executions)
 
         logger.logger.info("Stage execution executed", stage_execution_id=self.model.id,
                            stage_name=self.model.stage_model.name, status='success')
 
     def validate_modules(self) -> None:
         """
         Check if module is present and module args are correct for each Step
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/models/step.py` & `cryton_core-2023.1.2/cryton_core/lib/models/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from datetime import datetime
 from typing import Union, Type, Optional
 import re
 import copy
+import yaml
+import amqpstorm
+from schema import Schema, Optional as SchemaOptional, SchemaError, Or, And
+from jinja2 import nativetypes, StrictUndefined, UndefinedError
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import transaction
 from django.db.models.query import QuerySet
 from django.core import exceptions as django_exc
 from django.utils import timezone
-import amqpstorm
-from schema import Schema, Optional as SchemaOptional, SchemaError, Or, And
 
 from cryton_core.cryton_app.models import StepModel, StepExecutionModel, SuccessorModel, ExecutionVariableModel, \
     OutputMappingModel, CorrelationEventModel
 
 from cryton_core.etc import config
 from cryton_core.lib.util import constants, exceptions, logger, states, util, rabbit_client
 from cryton_core.lib.models import worker, session
@@ -55,15 +57,15 @@
                 self.model = StepModel.objects.get(id=step_model_id)
             except django_exc.ObjectDoesNotExist:
                 raise exceptions.StepObjectDoesNotExist("PlanModel with id {} does not exist."
                                                         .format(step_model_id))
 
         else:
             step_obj_arguments = copy.deepcopy(kwargs)
-            step_obj_arguments.pop('next', None)
+            step_obj_arguments.pop(constants.NEXT, None)
             step_obj_arguments.pop('output_mapping', None)
             # Set default prefix as step name
             if step_obj_arguments.get('output_prefix') is None:
                 step_obj_arguments.update({'output_prefix': step_obj_arguments.get('name')})
             self.model = StepModel.objects.create(**step_obj_arguments)
 
     def delete(self):
@@ -595,16 +597,19 @@
         """
         logger.logger.debug("Updating step arguments with dynamic variables", step_execution_id=self.model.id,
                             step_arguments=arguments)
 
         # Get list of dynamic variables
         vars_list = util.get_dynamic_variables(arguments)
 
+        dynamic_variable_separator = self.model.step_model.stage_model.plan_model. \
+            settings.get(constants.SEPARATOR,
+                         constants.SEPARATOR_DEFAULT_VALUE)
         # Get their prefixes
-        prefixes = util.get_prefixes(vars_list)
+        prefixes = util.get_prefixes(vars_list, dynamic_variable_separator)
         vars_dict = dict()
         is_parent = False
 
         for prefix in prefixes:
             # If prefix is parent, get parents prefix
             if prefix == 'parent':
                 if parent_step_ex_id is None:
@@ -622,30 +627,39 @@
                     tmp_dict.update(step_ex.serialized_output)
             # Change parents prefix back to 'parent' for updating dictionary to substitute
             if is_parent:
                 prefix = 'parent'
                 is_parent = False
             vars_dict.update({prefix: tmp_dict})
 
-        updated_arguments = util.fill_dynamic_variables(arguments, vars_dict)
+        updated_arguments = util.fill_dynamic_variables(copy.deepcopy(arguments), vars_dict, dynamic_variable_separator)
         return updated_arguments
 
     @staticmethod
-    def _update_arguments_with_execution_variables(arguments: dict, execution_vars: list) -> dict:
+    def _update_arguments_with_execution_variables(arguments: dict, execution_variables: list) -> dict:
         """
-        Update passed arguments with execution variables.
-        :param arguments: Arguments to be updated with execution variables
-        :param execution_vars: Execution variables to be passed to arguments
-        :return: Updated arguments with execution variables
-        """
-        execution_vars_dict = dict()
-        for execution_var in execution_vars:
-            execution_vars_dict.update({execution_var.get('name'): execution_var.get('value')})
+        Fill Jinja variables in the arguments with execution variables.
+        :param arguments: Arguments to fill
+        :param execution_variables: Execution variables to fill the template (arguments) with
+        :return: Filled arguments
+        """
+        parsed_execution_variables = {variable.get('name'): variable.get('value') for variable in execution_variables}
+
+        env = nativetypes.NativeEnvironment(
+            undefined=StrictUndefined, block_start_string=constants.BLOCK_START_STRING,
+            block_end_string=constants.BLOCK_END_STRING, variable_start_string=constants.VARIABLE_START_STRING,
+            variable_end_string=constants.VARIABLE_END_STRING, comment_start_string=constants.COMMENT_START_STRING,
+            comment_end_string=constants.COMMENT_END_STRING
+        )
+        arguments_template = env.from_string(yaml.safe_dump(arguments))
 
-        return util.fill_execution_variables(arguments, execution_vars_dict)
+        try:
+            return yaml.safe_load(arguments_template.render(**parsed_execution_variables))
+        except (yaml.YAMLError, UndefinedError, TypeError) as ex:
+            raise exceptions.StepValidationError(f"An error occurred while updating execution variables. {ex}.")
 
     def update_step_arguments(self, arguments: dict, plan_execution_id: Type[int]) -> dict:
         """
         Update Step arguments with execution and dynamic variables.
         :param arguments: Arguments to be updated
         :param plan_execution_id: ID of the parent step of the current step execution
         :return: Updated arguments with execution and dynamic variables
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/models/worker.py` & `cryton_core-2023.1.2/cryton_core/lib/models/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,15 @@
             state: str
         """
         worker_model_id = kwargs.get('worker_model_id')
         if worker_model_id:
             try:
                 self.model = WorkerModel.objects.get(id=worker_model_id)
             except django_exc.ObjectDoesNotExist:
-                raise exceptions.WorkerObjectDoesNotExist(
-                    "WorkerModel with id {} does not exist.".format(worker_model_id), worker_model_id
-                )
+                raise exceptions.WorkerObjectDoesNotExist(worker_model_id)
 
         else:
             self.model = WorkerModel.objects.create(**kwargs)
 
     def delete(self):
         self.model.delete()
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/services/listener.py` & `cryton_core-2023.1.2/cryton_core/lib/services/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,18 @@
             return
 
         logger.logger.debug("Stopping Consumer.", id=self._id)
         self._stopped.set()
 
         if self._connection is not None and self._connection.is_open:  # Close connection and its channels.
             logger.logger.debug("Closing channels.")
-            print("Closing connection and it's channels..")
+
             for channel in list(self._connection.channels.values()):
                 channel.close()
+
             logger.logger.debug("Closing connection.")
             self._connection.close()
 
         logger.logger.debug("Consumer stopped.", id=self._id)
 
     def _update_connection(self) -> bool:
         """
@@ -155,49 +156,54 @@
         self.queues = {
             config.Q_ATTACK_RESPONSE_NAME: self.step_response_callback,
             config.Q_AGENT_RESPONSE_NAME: self.step_response_callback,
             config.Q_EVENT_RESPONSE_NAME: self.event_callback,
             config.Q_CONTROL_REQUEST_NAME: self.control_request_callback
         }
 
-    def start(self) -> None:
+    def begin(self) -> None:
         """
-        Start consumers and keep self alive.
+        Create and start consumers.
         :return: None
         """
-        print("Starting RabbitMQ listener")
         self._create_consumers()
         self._start_consumers()
-        print("Started RabbitMQ listener")
+
         logger.logger.info("Started RabbitMQ listener")
+
+    def start(self) -> None:
+        """
+        Start and keep self alive.
+        :return: None
+        """
+        self.begin()
+
         try:
             while not self._stopped.is_set():
                 time.sleep(5)
         except KeyboardInterrupt:
             pass
 
         self.stop()
 
     def stop(self) -> None:
         """
         Stop Listener and it's Consumers.
         :return: None
         """
-        print("Stopping RabbitMQ listener")
         for consumer, consumer_process in self._consumers.items():
             try:
                 consumer.stop()
             except Exception as ex:
                 logger.logger.warning("Unable to stop Consumer", error=str(ex))
                 consumer_process.kill()
 
         self.scheduler.scheduler.shutdown()
-
         self._stopped.set()
-        print("Stopped RabbitMQ listener")
+
         logger.logger.info("Stopped RabbitMQ listener")
 
     def _create_consumers(self) -> None:
         """
         Create consumers and their processes.
         :return: None
         """
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/services/scheduler.py` & `cryton_core-2023.1.2/cryton_core/lib/services/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,10 +93,7 @@
     def exposed_pause_scheduler(self):
         logger.logger.debug("Pausing scheduler service")
         return self.scheduler.pause()
 
     def exposed_resume_scheduler(self):
         logger.logger.debug("Resuming scheduler service")
         return self.scheduler.resume()
-
-    def health_check(self):
-        return 0
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/triggers/__init__.py` & `cryton_core-2023.1.2/cryton_core/lib/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_base.py` & `cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_base.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_datetime.py` & `cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_datetime.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_delta.py` & `cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_delta.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_http.py` & `cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_http.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/triggers/trigger_msf.py` & `cryton_core-2023.1.2/cryton_core/lib/triggers/trigger_msf.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/util/constants.py` & `cryton_core-2023.1.2/cryton_core/lib/util/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,20 +75,22 @@
 # RabbitMQ message keywords
 EVENT_T = "event_t"
 EVENT_V = "event_v"
 ACK_QUEUE = "ack_queue"
 REPLY_TO = "reply_to"
 
 # Other constants
-PAUSE = 'PAUSE'
-STATUS_OK = 'success'
 EVENT_ACTION = 'action'
 TRIGGER_TYPE = "trigger_type"
 TRIGGER_ID = "trigger_id"
 
+# Plan settings constatnts
+SEPARATOR = 'separator'
+SEPARATOR_DEFAULT_VALUE = '.'
+
 # Event types
 EVENT_VALIDATE_MODULE = "VALIDATE_MODULE"
 EVENT_LIST_MODULES = "LIST_MODULES"
 EVENT_LIST_SESSIONS = "LIST_SESSIONS"
 EVENT_KILL_STEP_EXECUTION = "KILL_STEP_EXECUTION"
 EVENT_HEALTH_CHECK = "HEALTH_CHECK"
 EVENT_ADD_TRIGGER = "ADD_TRIGGER"
@@ -121,7 +123,8 @@
 # Jinja regex values
 BLOCK_START_STRING = "'{%"
 BLOCK_END_STRING = "%}'"
 VARIABLE_START_STRING = "'{{"
 VARIABLE_END_STRING = "}}'"
 COMMENT_START_STRING = "'{#"
 COMMENT_END_STRING = "#}'"
+
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/util/creator.py` & `cryton_core-2023.1.2/cryton_core/lib/util/creator.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/util/event.py` & `cryton_core-2023.1.2/cryton_core/lib/util/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,14 @@
                 ret_val = scheduler_obj.exposed_remove_job(**scheduler_args)
             elif scheduler_action == constants.GET_JOBS:
                 ret_val = scheduler_obj.exposed_get_jobs()
             elif scheduler_action == constants.PAUSE_SCHEDULER:
                 ret_val = scheduler_obj.exposed_pause_scheduler()
             elif scheduler_action == constants.RESUME_SCHEDULER:
                 ret_val = scheduler_obj.exposed_resume_scheduler()
-            elif scheduler_action == constants.EVENT_HEALTH_CHECK:
-                ret_val = scheduler_obj.health_check()
         except Exception as ex:
             logger.logger.error("Scheduler could not process the request", error=str(ex))
 
         return ret_val if ret_val is not None else 0
 
     def handle_finished_step(self) -> None:
         """
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/util/exceptions.py` & `cryton_core-2023.1.2/cryton_core/lib/util/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,397 +1,351 @@
 from typing import Union, Type, List
 from cryton_core.lib.util import logger
 
 
 class Error(Exception):
     """Base class for exceptions in this module."""
-    pass
 
 
 class ValidationError(Error):
     """Exception raised for errors in the validation process."""
-
     def __init__(self, message: Union[dict, Exception, str]):
         if type(message) != dict:
             self.message = {"message": message}
         else:
             self.message = message
 
         super().__init__(self.message)
 
 
 class PlanValidationError(ValidationError):
     """Exception raised for errors in the Plan validation process."""
-
     def __init__(self, message: Union[Exception, str], plan_name: str = None):
         self.message = {"message": message, "plan_name": plan_name}
         super().__init__(self.message)
 
 
 class DuplicateNameInPlan(PlanValidationError):
+    """Exception raised when multiple instances have the same name in one Plan."""
     def __init__(self, unique_argument: str, duplicate_name: str, plan_name: str):
         self.message = f"{unique_argument} name '{duplicate_name}' is not unique in the plan"
         super().__init__(self.message, plan_name)
 
 
 class StageValidationError(ValidationError):
     """Exception raised for errors in the Stage validation process."""
-
     def __init__(self, message: Union[Exception, str], stage_name: str = None):
         self.message = {"message": message, "stage_name": stage_name}
         logger.logger.error(message, stage_name=stage_name, state='fail')
         super().__init__(self.message)
 
 
 class StepValidationError(ValidationError):
     """Exception raised for errors in the Step validation process."""
-
     def __init__(self, message: Union[Exception, str], step_name: str = None):
         self.message = {"message": message, "step_name": step_name}
         super().__init__(self.message)
 
 
 class UserInputError(Error):
     """Exception raised for errors when user inputs an invalid input."""
-
     def __init__(self, message: Union[Exception, str], user_input: Union[str, int] = None):
         self.message = {"message": message, "user_input": user_input}
         super().__init__(self.message)
 
 
 class ObjectDoesNotExist(Error):
     """Exception raised if trying to use an object that doesn't exist."""
-    pass
 
 
 class RunObjectDoesNotExist(ObjectDoesNotExist):
     """Exception raised if trying to use a Run object that doesn't exist."""
-
     def __init__(self, run_id: int = None, plan_id: int = None, stage_id: int = None,
                  step_id: int = None, worker_id: int = None):
         self.message = {
-            "message": 'RunModel does not exist.', "run_id": run_id, "plan_id": plan_id,
-            "stage_id": stage_id, "step_id": step_id,
-            "worker_id": worker_id
+            "message": 'RunModel does not exist.', "run_id": run_id, "plan_id": plan_id, "stage_id": stage_id,
+            "step_id": step_id, "worker_id": worker_id
         }
         super().__init__(self.message)
 
 
 class PlanObjectDoesNotExist(ObjectDoesNotExist):
     """Exception raised if trying to use a Plan object that doesn't exist."""
-
     def __init__(self, plan_id: int = None):
         self.message = {"message": 'Plan model does not exist.', "plan_id": plan_id}
         super().__init__(self.message)
 
 
 class StageObjectDoesNotExist(ObjectDoesNotExist):
     """Exception raised if trying to use a Stage object that doesn't exist."""
-
     def __init__(self, message: Union[Exception, str], stage_id: int = None, plan_id: int = None):
         self.message = {"message": message, "stage_id": stage_id, "plan_id": plan_id}
         super().__init__(self.message)
 
 
 class StageExecutionObjectDoesNotExist(ObjectDoesNotExist):
     """Exception raised if trying to use a StageExecution object that doesn't exist."""
-
     def __init__(self, message: Union[Exception, str], stage_id: int = None, plan_id: int = None):
         self.message = {"message": message, "stage_id": stage_id, "plan_id": plan_id}
         super().__init__(self.message)
 
 
 class StepObjectDoesNotExist(ObjectDoesNotExist):
     """Exception raised if trying to use a Step object that doesn't exist."""
-
     def __init__(self, message: Union[Exception, str], step_id: int = None, step_name: str = None,
                  stage_id: Union[int, Type[int]] = None, plan_id: int = None):
         self.message = {
             "message": message, "step_id": step_id, "step_name": step_name, "stage_id": stage_id, "plan_id": plan_id
         }
         super().__init__(self.message)
 
 
 class StepExecutionObjectDoesNotExist(Error):
     """Exception raised if trying to set invalid type of successor."""
-
     def __init__(self, message: Union[Exception, str] = 'StepExecution not found', step_execution_id: str = None):
         self.message = {"message": message, "step_execution_id": step_execution_id}
         super().__init__(self.message)
 
 
 class SuccessorObjectDoesNotExist(ObjectDoesNotExist):
     """Exception raised if trying to use a Successor object that doesn't exist."""
-
     def __init__(self, message: Union[Exception, str], step_id: int = None):
         self.message = {"message": message, "step_id": step_id}
         super().__init__(self.message)
 
 
 class WorkerObjectDoesNotExist(ObjectDoesNotExist):
     """Exception raised if trying to use a Worker object that doesn't exist."""
-
-    def __init__(self, message: Union[Exception, str], worker_id: int = None, worker_name: str = None,
-                 plan_id: int = None, stage_id: int = None):
-        self.message = {
-            "message": 'WorkerModel does not exist.', "worker_id": worker_id, "worker_name": worker_name,
-            "plan_id": plan_id, "stage_id": stage_id
-        }
+    def __init__(self, worker_id: int):
+        self.message = {"message": 'WorkerModel does not exist.', "worker_id": worker_id}
         super().__init__(self.message)
 
 
 class SessionObjectDoesNotExist(ObjectDoesNotExist):
     """Exception raised if trying to use a Session object that doesn't exist."""
-
     def __init__(self, message: Union[Exception, str], session_name: str = None, session_id: int = None,
                  plan_execution_id: Union[Type[int], int] = None, step_id: int = None, plan_id: int = None,
                  target=None, target_id=None):
         self.message = {
             "message": message, "session_name": session_name, "session_id": session_id, "plan_execution_id":
                 plan_execution_id,
             "step_id": step_id, "plan_id": plan_id, "target": target, "target_id": target_id
         }
         super().__init__(self.message)
 
 
 class SessionIsNotOpen(Error):
+    """Exception raised if the desired session isn't open."""
     def __init__(self, message: Union[Exception, str], session_name: str,
                  plan_execution_id: Union[Type[int], int], step_id: int):
         self.message = {
-            "message": message, "session_name": session_name, "plan_execution_id":
-                plan_execution_id,
+            "message": message, "session_name": session_name, "plan_execution_id": plan_execution_id,
             "step_id": step_id
         }
         super().__init__(self.message)
 
 
 class ArgumentsObjectDoesNotExist(ObjectDoesNotExist):
     """Exception raised if trying to use an Arguments object that doesn't exist."""
-
     def __init__(self, message: Union[Exception, str], step_id: int = None):
         self.message = {"message": message, "step_id": step_id}
         super().__init__(self.message)
 
 
 class InvalidStateError(Error):
     """Exception raised if an invalid state is detected."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state: str, allowed_states: list):
         self.message = {
             "message": message, "execution_id": execution_id, "state": state, "allowed_states": allowed_states
         }
         super().__init__(self.message)
 
 
 class RunInvalidStateError(InvalidStateError):
     """Exception raised if Run's invalid state is detected."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state: str, allowed_states: list):
         super().__init__(message, execution_id, state, allowed_states)
         logger.logger.error(message, execution_id=execution_id, state=state, allowed_states=allowed_states)
 
 
 class PlanInvalidStateError(InvalidStateError):
     """Exception raised if PlanExecution's invalid state is detected."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state: str, allowed_states: list):
         super().__init__(message, execution_id, state, allowed_states)
         logger.logger.error(message, execution_id=execution_id, state=state, allowed_states=allowed_states)
 
 
 class StageInvalidStateError(InvalidStateError):
     """Exception raised if StageExecution's invalid state is detected."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state: str, allowed_states: list):
         super().__init__(message, execution_id, state, allowed_states)
         logger.logger.error(message, execution_id=execution_id, state=state, allowed_states=allowed_states)
 
 
 class StepInvalidStateError(InvalidStateError):
     """Exception raised if StepExecution's invalid state is detected."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state: str, allowed_states: list):
         super().__init__(message, execution_id, state, allowed_states)
         logger.logger.error(message, execution_id=execution_id, state=state, allowed_states=allowed_states)
 
 
 class StateTransitionError(Error):
     """Exception raised if an invalid state transition is made."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state_from: str, state_to: str,
                  allowed_transitions: list):
         self.message = {
             "message": message, "execution_id": execution_id, "state_from": state_from, "state_to": state_to,
             "allowed_transitions": allowed_transitions
         }
         super().__init__(self.message)
 
 
 class RunStateTransitionError(StateTransitionError):
     """Raised if an invalid Run's state transition is made."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state_from: str, state_to: str,
                  allowed_transitions: list):
         super().__init__(message, execution_id, state_from, state_to, allowed_transitions)
         logger.logger.warning("Invalid transition detected in Run", execution_id=execution_id,
                               state_from=state_from, state_to=state_to)
 
 
 class PlanStateTransitionError(StateTransitionError):
     """Raised if an invalid PlanExecution's state transition is made."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state_from: str, state_to: str,
                  allowed_transitions: list):
         super().__init__(message, execution_id, state_from, state_to, allowed_transitions)
         logger.logger.warning("Invalid transition detected in Plan", execution_id=execution_id,
                               state_from=state_from, state_to=state_to)
 
 
 class StageStateTransitionError(StateTransitionError):
     """Raised if an invalid StageExecution's state transition is made."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state_from: str, state_to: str,
                  allowed_transitions: list):
         super().__init__(message, execution_id, state_from, state_to, allowed_transitions)
         logger.logger.warning("Invalid transition detected in Stage", execution_id=execution_id,
                               state_from=state_from, state_to=state_to)
 
 
 class StepStateTransitionError(StateTransitionError):
     """Raised if an invalid StepExecution's state transition is made."""
-
     def __init__(self, message: Union[Exception, str], execution_id: int, state_from: str, state_to: str,
                  allowed_transitions: list):
         super().__init__(message, execution_id, state_from, state_to, allowed_transitions)
         logger.logger.warning("Invalid transition detected in Step", execution_id=execution_id,
                               state_from=state_from, state_to=state_to)
 
 
 class UnexpectedValue(Error):
     """Raised if an invalid value is used."""
-
     def __init__(self, message: Union[Exception, str], wrong_value: Union[str, int] = None):
         self.message = {"message": message, "wrong_value": wrong_value}
         super().__init__(self.message)
 
 
 class WrongParameterError(Error):
     """Exception raised if trying to filter in model by wrong parameter."""
-
     def __init__(self, message: Union[Exception, str] = 'Wrong parameter name', param_name: str = None):
         self.message = {"message": message, "param_name": param_name}
         super().__init__(self.message)
 
 
 class ParameterMissingError(Error):
     """Exception raised if compulsory parameter is missing."""
-
     def __init__(self, message: Union[Exception, str] = 'Missing parameter', param_name: str = None):
         self.message = {"message": message, "param_name": param_name}
         super().__init__(self.message)
 
 
 class DependencyDoesNotExist(Error):
     """Exception raised if could not create dependency between Stages."""
     def __init__(self, message: Union[Exception, str], stage_name: str = None):
         self.message = {"message": message, "stage_name": stage_name}
-        logger.logger.error("stage dependency does not exist", stage_name=stage_name, status='fail')
+        logger.logger.error("stage dependency does not exist", stage_name=stage_name)
         super().__init__(self.message)
 
 
 class InvalidSuccessorType(Error):
     """Exception raised if trying to set invalid type of successor."""
-
     def __init__(self, message: Union[Exception, str] = 'Wrong successor type', successor_type: str = None):
         self.message = {"message": message, "successor_type": successor_type}
         super().__init__(self.message)
 
 
 class InvalidSuccessorValue(Error):
     """Exception raised if trying to set invalid value for successor."""
-
     def __init__(self, message: Union[Exception, str] = 'Wrong successor value', successor_value: str = None):
         self.message = {"message": message, "successor_value": successor_value}
         super().__init__(self.message)
 
 
 class PlanExecutionDoesNotExist(Error):
     """Exception raised if Execution does not exist."""
-
     def __init__(self, message: Union[Exception, str] = 'PlanExecution not found', plan_execution_id: str = None):
         self.message = {"message": message, "plan_execution_id": plan_execution_id}
         super().__init__(self.message)
 
 
 class CreationFailedError(Error):
     """Exception raised if object creation failed."""
-
     def __init__(self, message: dict):
         self.message = message
         super().__init__(self.message)
 
 
 class PlanCreationFailedError(CreationFailedError):
     """Exception raised if Plan creation failed."""
-
     def __init__(self, message: Union[Exception, str], plan_name: str = None):
         self.message = {"message": message, "plan_name": plan_name}
-        logger.logger.error("plan creation failed", plan_name=plan_name, status='fail')
+        logger.logger.error("plan creation failed", plan_name=plan_name)
         super().__init__(self.message)
 
 
 class StageCreationFailedError(CreationFailedError):
     """Exception raised if Stage creation failed."""
-
     def __init__(self, message: Union[Exception, str], stage_name: str = None):
         self.message = {"message": message, "stage_name": stage_name}
-        logger.logger.error("stage creation failed", stage_name=stage_name, status='fail')
+        logger.logger.error("stage creation failed", stage_name=stage_name)
         super().__init__(self.message)
 
 
 class StepCreationFailedError(CreationFailedError):
     """Exception raised if Step creation failed."""
-
     def __init__(self, message: Union[Exception, str], step_name: str = None):
         self.message = {"message": message, "step_name": step_name}
-        logger.logger.error("step creation failed", step_name=step_name, status='fail')
+        logger.logger.error("step creation failed", step_name=step_name)
         super().__init__(self.message)
 
 
 class SuccessorCreationFailedError(CreationFailedError):
     """Exception raised if Successor creation failed."""
-
     def __init__(self, message: Union[Exception, str], successor_name: str = None):
         self.message = {"message": message, "successor_name": successor_name}
-        logger.logger.error("Successor creation failed", successor_name=successor_name, status='fail')
+        logger.logger.error("Successor creation failed", successor_name=successor_name)
         super().__init__(self.message)
 
 
 class PlanExecutionCreationFailedError(CreationFailedError):
     """Exception raised if PlanExecution creation failed."""
-
     def __init__(self, message: Union[Exception, str] = 'Bad argument', param_name: str = None, param_type: str = None):
         self.message = {"message": message, "param_type": param_type, "param_name": param_name}
-        logger.logger.error("PlanExecution creation failed", param_name=param_name,
-                            param_type=param_type, status='fail')
+        logger.logger.error("PlanExecution creation failed", param_name=param_name, param_type=param_type)
         super().__init__(self.message)
 
 
 class RunCreationFailedError(CreationFailedError):
     """Exception raised if Run creation failed."""
-
     def __init__(self, message: Union[Exception, str]):
         self.message = {"message": message}
-        logger.logger.error("run creation failed", status='fail')
+        logger.logger.error("run creation failed")
         super().__init__(self.message)
 
 
 class RabbitError(Error):
     """Exception raised when there is some problem with RabbitMQ"""
-
     def __init__(self, message: Union[Exception, str]):
         self.message = {"message": message}
         super().__init__(self.message)
 
 
 class RpcTimeoutError(RabbitError):
     """Exception raised if the RPC request timeouts"""
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/util/logger.py` & `cryton_core-2023.1.2/cryton_core/lib/util/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 import logging.config
 import logging.handlers
 from multiprocessing import Process, Queue
 
 from . import constants
 from cryton_core.etc import config
 
-"""
-Default Cryton logger setup and configuration
-"""
-
 
 class Logger:
+    """
+    Default logger
+    """
     def __init__(self, logger_config):
         self.logger_config = logger_config
         self.logger_type = constants.LOGGER_CRYTON_PRODUCTION
         self.logger = None
         self.log_queue = Queue()
 
         if config.DEBUG:
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/util/rabbit_client.py` & `cryton_core-2023.1.2/cryton_core/lib/util/rabbit_client.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/util/scheduler_client.py` & `cryton_core-2023.1.2/cryton_core/lib/util/scheduler_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -68,24 +68,7 @@
             'job_id': job_id
         }
         message = {constants.EVENT_T: constants.EVENT_UPDATE_SCHEDULER,
                    constants.EVENT_V: {constants.EVENT_ACTION: constants.REMOVE_JOB, 'args': args}}
         rpc.call(config.Q_CONTROL_REQUEST_NAME, message)
 
     return 0
-
-
-# TODO: remove, deprecated
-def health_check() -> bool:
-    """
-
-    :return: True or False
-    """
-    rpc = RpcClient()
-    args = {}
-    message = {constants.EVENT_T: constants.EVENT_UPDATE_SCHEDULER,
-               constants.EVENT_V: {constants.EVENT_ACTION: constants.EVENT_HEALTH_CHECK, 'args': args}}
-    resp = rpc.call(config.Q_CONTROL_REQUEST_NAME, message)
-    health = resp.get('return_value')
-    if health != 0:
-        return False
-    return True
```

### Comparing `cryton_core-2022.2.2/cryton_core/lib/util/states.py` & `cryton_core-2023.1.2/cryton_core/lib/util/states.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/lib/util/util.py` & `cryton_core-2023.1.2/cryton_core/lib/util/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-import json
 from threading import Thread
 from functools import reduce
 import copy
 from typing import List, Union, Dict
 from datetime import datetime, timedelta
-import configparser
 import pytz
 import amqpstorm
-from jinja2 import nativetypes, DebugUndefined, StrictUndefined, ChainableUndefined, UndefinedError
 import re
-import yaml
 
 from cryton_core.etc import config
-from cryton_core.lib.util import exceptions, logger, constants
+from cryton_core.lib.util import exceptions, logger
 
 from django.utils import timezone
 
 
 def convert_to_utc(original_datetime: datetime, time_zone: str = 'utc', offset_aware: bool = False) -> datetime:
     """
     Convert datetime in specified timezone to UTC timezone
@@ -69,106 +65,22 @@
         seconds = int(seconds)
     except Exception:
         raise exceptions.UserInputError("Invalid delta provided. Correct format is [int]h[int]m[int]s", time_str)
 
     return timedelta(hours=hours, minutes=minutes, seconds=seconds)
 
 
-# TODO: move to the cryton_app/util.py
-class IgnoreNestedUndefined(ChainableUndefined, DebugUndefined):
-    def __getattr__(self, attr: str) -> "IgnoreNestedUndefined":
-        self._undefined_name += f'.{attr}'
-
-        return self
-
-    def __getitem__(self, item: str) -> "IgnoreNestedUndefined":
-        self._undefined_name += f'[{item}]'
-
-        return self
-
-
-# TODO: move to StepEx class
-def fill_execution_variables(arguments: dict, execution_variables: dict) -> dict:
-    """
-    Fill Jinja variables in the Step arguments with execution variables.
-    :param arguments: Arguments to fill
-    :param execution_variables: Execution variables to fill the template with
-    :return: Filled arguments
-    """
-    env = nativetypes.NativeEnvironment(
-        undefined=StrictUndefined, block_start_string=constants.BLOCK_START_STRING,
-        block_end_string=constants.BLOCK_END_STRING, variable_start_string=constants.VARIABLE_START_STRING,
-        variable_end_string=constants.VARIABLE_END_STRING, comment_start_string=constants.COMMENT_START_STRING,
-        comment_end_string=constants.COMMENT_END_STRING)
-
-    arguments_template = env.from_string(yaml.safe_dump(arguments))
-    try:
-        return yaml.safe_load(arguments_template.render(**execution_variables))
-    except (yaml.YAMLError, UndefinedError, TypeError) as ex:
-        raise exceptions.StepValidationError(f"An error occurred while updating execution variables. {ex}.")
-
-
-# TODO: move to the cryton_app/util.py
-def fill_template(template: str, inventory_variables: dict) -> str:
-    """
-    Fill Jinja variables in the template with inventory variables.
-    :param inventory_variables: Template variables to fill the template with
-    :param template: Template to fill
-    :return: Filled template
-    """
-    env = nativetypes.NativeEnvironment(undefined=IgnoreNestedUndefined)
-
-    try:
-        plan_template_obj = env.from_string(template)
-        filled_template = plan_template_obj.render(**inventory_variables)
-    except (TypeError, UndefinedError):
-        raise exceptions.ValidationError(f"Template is not a valid jinja template: {template}")
-
-    return filled_template
-
-
-# TODO: move to the cryton_app/util.py
-def parse_inventory(inventory: str) -> dict:
-    """
-    Reads inventory file (JSON, YAML, INI) and returns it as a dictionary
-    :param inventory: Inventory file content
-    :return: Inventory variables
-    """
-    # JSON
-    try:
-        return json.loads(inventory)
-    except json.decoder.JSONDecodeError:
-        pass
-
-    # YAML
-    try:
-        return yaml.safe_load(inventory)
-    except yaml.YAMLError:
-        pass
-
-    # INI
-    try:
-        config_parser = configparser.ConfigParser()
-        config_parser.read_string(inventory)
-        return {section: dict(config_parser.items(section)) for section in config_parser.sections()}
-    except configparser.Error:
-        pass
-
-    raise ValueError(f"Inventory file must contain data and be of type JSON, YAML, or INI. File: {inventory}")
-
-
 def split_into_lists(input_list: List, target_number_of_lists: int) -> List[List]:
     """
     Evenly splits list into n lists.
     E.g. split_into_lists([1,2,3,4], 4) returns [[1], [2], [3], [4]].
     :param input_list: object to split
     :param target_number_of_lists: how many lists to split into
     :returns: list of lists containing original items
     """
-
     quotient, reminder = divmod(len(input_list), target_number_of_lists)
     return [input_list[i * quotient + min(i, reminder):(i + 1) * quotient + min(i + 1, reminder)] for i in
             range(target_number_of_lists)]
 
 
 def run_executions_in_threads(step_executions: List) -> None:
     """
@@ -242,29 +154,30 @@
     if list_indexes is not None:  # Get each List index in '[index]' format and get index only.
         parsed_list_indexes = re.findall(r"(\[[0-9]+])", list_indexes.group())
         parsed_list_indexes = [index for index in parsed_list_indexes]
         return [dot_argument[0:list_indexes.start()]] + parsed_list_indexes
     return [dot_argument]  # If no List Indexes are present.
 
 
-def get_from_dict(dict_in: dict, value: str):
+def get_from_dict(dict_in: dict, value: str, separator: str):
     """
     Get value from dict_in dict
     eg:
       dict_in: {'output': {'username': 'admin'}}
       value: '$dict_in.output.username'
       return: 'admin'
     :param value: value defined in template
     :param dict_in: dict_in for this step
+    :param separator: separator for dynamic variable
     :return: value from dict_in
     """
-    dot_args = value.lstrip('$').split('.')  # Get keys using '.' separator.
+    dynamic_var_arguments = value.lstrip('$').split(separator)  # Get keys using '.' separator.
     all_args = []  # Dict keys and List indexes.
-    for dot_arg in dot_args:  # Go through dot_args and separate all args.
-        all_args.extend(parse_dot_argument(dot_arg))
+    for argument in dynamic_var_arguments:  # Go through dot_args and separate all args.
+        all_args.extend(parse_dot_argument(argument))
 
     try:
         res = reduce(getitem, all_args, dict_in)
     except KeyError:
         res = None
 
     return res
@@ -282,71 +195,41 @@
     for k, v in obj.items():
         if isinstance(v, dict):
             item = _finditem(v, key)
             if item is not None:
                 return item
 
 
-def update_inner(obj: dict, dict_in: dict, startswith: str):
+def fill_dynamic_variables(dict_to_update: dict, dynamic_variables_dict: dict, separator: str,
+                           startswith: str = '$'):
     """
 
-    Update value inside the object with one specified by prefix and path from dict_in
-    eg.: $dict_in.test replaces with dict_in.get('test')
+    Fill variables in dict_to_update with dynamic_variables_dict.
 
-    :param obj: Object
-    :param dict_in: dict_in dictioanry
+    :param dict_to_update: Module arguments that should be filled with dynamic variables
+    :param dynamic_variables_dict: Output from another module that will be used to update 'dict_to_update'
     :param startswith: prefix, eg. $
+    :param separator: separator for dynamic variable
     :return:
     """
-    if isinstance(obj, dict):
-        for k, v in obj.items():
-            if isinstance(v, str):
-                if v.startswith(startswith):
-                    new_val = get_from_dict(dict_in, v)
-                    if new_val is not None:
-                        obj.update({k: new_val})
-            elif isinstance(v, dict):
-                update_inner(v, dict_in, startswith)
-            elif isinstance(v, list):
-                for value in v:
-                    update_inner(value, dict_in, startswith)
-
-
-def replace_value_in_dict(dict_to_repl: dict,
-                          dict_in: dict,
-                          startswith: str = '$'):
-    """
-    Replace value in dictionary
-    :param dict_to_repl:
-    :param dict_in: dict_in
-    :param startswith: prefix
-    :return:
-    """
-
-    if startswith not in str(dict_to_repl):
-        raise ValueError("No value starting with {} in dictionary".format(startswith))
-    if dict_in is None:
-        # Nothing to replace
-        return None
-    update_inner(dict_to_repl, dict_in, startswith)
-
-
-def fill_dynamic_variables(in_dict, var_dict):
-    """
 
-    Fill variables in in_dict with var_dict.
-
-    :param in_dict:
-    :param var_dict:
-    :return:
-    """
-    in_dict_copy = copy.deepcopy(in_dict)
-    update_inner(in_dict_copy, var_dict, '$')
+    if isinstance(dict_to_update, dict):
+        for argument_key, argument_value in dict_to_update.items():
+            if isinstance(argument_value, str):
+                if argument_value.startswith(startswith):
+                    new_val = get_from_dict(dynamic_variables_dict, argument_value, separator)
+                    if new_val is not None:
+                        dict_to_update.update({argument_key: new_val})
+            elif isinstance(argument_value, dict):
+                fill_dynamic_variables(argument_value, dynamic_variables_dict, separator, startswith)
+            elif isinstance(argument_value, list):
+                for list_value in argument_value:
+                    fill_dynamic_variables(list_value, dynamic_variables_dict, separator, startswith)
 
-    return in_dict_copy
+    return dict_to_update
 
 
 def get_all_values(input_container):
     """
     Get all values (recursively) from a dict
     :param input_container: input dict or list
     :return: yields elements, use as list(get_all_values(d))
@@ -371,22 +254,23 @@
     vars_list = list(get_all_values(in_dict))
 
     for i in vars_list:
         if isinstance(i, str) and i.startswith(prefix):
             yield i
 
 
-def get_prefixes(vars_list):
+def get_prefixes(vars_list: list, separator: str):
     """
     Get list of prefixes from list of dynamic variables
-    :param vars_list:
+    :param vars_list: Individual pieces of a dynamic variable
+    :param separator: Dynamic variable separator
     :return:
     """
     for i in vars_list:
-        yield i.split('.')[0].lstrip('$')
+        yield i.split(separator)[0].lstrip('$')
 
 
 def pop_key(in_dict, val):
     """
     Pop key at specified position (eg. 'k1.k2.k3')
     :param in_dict:
     :param val:
```

### Comparing `cryton_core-2022.2.2/cryton_core/manage.py` & `cryton_core-2023.1.2/cryton_core/manage.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/settings.py` & `cryton_core-2023.1.2/cryton_core/settings.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/autocomplete.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/base.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/changelists.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/forms.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/login.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/nav_sidebar.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/responsive.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/responsive_rtl.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/responsive_rtl.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/rtl.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/vendor/select2/LICENSE-SELECT2.md` & `cryton_core-2023.1.2/cryton_core/static/admin/css/vendor/select2/LICENSE-SELECT2.md`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/vendor/select2/select2.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/vendor/select2/select2.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/vendor/select2/select2.min.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/vendor/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/css/widgets.css` & `cryton_core-2023.1.2/cryton_core/static/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/fonts/LICENSE.txt` & `cryton_core-2023.1.2/cryton_core/static/admin/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/fonts/Roboto-Bold-webfont.woff` & `cryton_core-2023.1.2/cryton_core/static/admin/fonts/Roboto-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/fonts/Roboto-Light-webfont.woff` & `cryton_core-2023.1.2/cryton_core/static/admin/fonts/Roboto-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/fonts/Roboto-Regular-webfont.woff` & `cryton_core-2023.1.2/cryton_core/static/admin/fonts/Roboto-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/LICENSE` & `cryton_core-2023.1.2/cryton_core/static/admin/img/LICENSE`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/calendar-icons.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/gis/move_vertex_off.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/gis/move_vertex_off.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/gis/move_vertex_on.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/gis/move_vertex_on.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/icon-calendar.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/icon-clock.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/icon-clock.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/icon-no.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/icon-no.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/icon-unknown-alt.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/icon-unknown-alt.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/icon-unknown.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/icon-unknown.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/icon-viewlink.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/icon-viewlink.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/inline-delete.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/inline-delete.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/selector-icons.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/img/sorting-icons.svg` & `cryton_core-2023.1.2/cryton_core/static/admin/img/sorting-icons.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/SelectBox.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/SelectBox.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/SelectFilter2.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/SelectFilter2.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/actions.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/actions.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/admin/DateTimeShortcuts.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/admin/DateTimeShortcuts.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/admin/RelatedObjectLookups.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/admin/RelatedObjectLookups.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/autocomplete.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/calendar.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/calendar.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/cancel.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/cancel.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/change_form.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/change_form.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/collapse.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/collapse.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/core.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/core.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/inlines.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/inlines.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/nav_sidebar.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/nav_sidebar.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/popup_response.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/popup_response.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/prepopulate.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/prepopulate.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/urlify.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/urlify.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/jquery/LICENSE.txt` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/jquery/jquery.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/jquery/jquery.min.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/LICENSE.md` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/af.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/af.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ar.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/az.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/bg.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/bn.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/bs.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ca.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/cs.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/da.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/de.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/dsb.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/el.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/el.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/en.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/es.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/et.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/eu.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/fa.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/fi.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/fr.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/gl.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/he.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hi.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hr.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hsb.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hu.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/hy.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/id.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/is.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/it.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ja.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ka.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/km.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/km.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ko.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/lt.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/lv.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/mk.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ms.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/nb.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ne.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/nl.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/pl.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ps.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/pt-BR.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/pt.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ro.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/ru.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sk.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sl.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sq.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sr-Cyrl.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sr.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/sv.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/th.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/tk.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/tr.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/uk.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/vi.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/zh-CN.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/i18n/zh-TW.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/select2.full.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/select2.full.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/select2/select2.full.min.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/select2/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/xregexp/LICENSE.txt` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/xregexp/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/xregexp/xregexp.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/xregexp/xregexp.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/admin/js/vendor/xregexp/xregexp.min.js` & `cryton_core-2023.1.2/cryton_core/static/admin/js/vendor/xregexp/xregexp.min.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js.LICENSE.txt` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js.map` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/redoc/bundles/redoc.standalone.js.map`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/favicon-32x32.png` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/oauth2-redirect.html` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js.LICENSE.txt` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js.map` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-standalone-preset.js` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-standalone-preset.js.map` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui.css` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui.css.map` & `cryton_core-2023.1.2/cryton_core/static/drf_spectacular_sidecar/swagger-ui-dist/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/css/bootstrap-theme.min.css` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/css/bootstrap-tweaks.css` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/css/bootstrap-tweaks.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/css/bootstrap.min.css` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/css/default.css` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/css/default.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/css/font-awesome-4.0.3.css` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/css/font-awesome-4.0.3.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/css/prettify.css` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/css/prettify.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/css/base.css` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/css/base.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/css/highlight.css` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/css/highlight.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/css/jquery.json-view.min.css` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/css/jquery.json-view.min.css`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/img/favicon.ico` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/img/grid.png` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/img/grid.png`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/js/api.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/js/api.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/js/highlight.pack.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/docs/js/jquery.json-view.min.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/docs/js/jquery.json-view.min.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.eot` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.svg` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.ttf` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.woff` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.eot` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.svg` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.ttf` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.woff` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.woff2` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/img/glyphicons-halflings-white.png` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/img/glyphicons-halflings.png` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/img/grid.png` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/img/grid.png`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/js/ajax-form.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/js/ajax-form.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/js/bootstrap.min.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/js/coreapi-0.1.1.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/js/coreapi-0.1.1.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/js/csrf.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/js/csrf.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/js/default.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/js/default.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/js/jquery-3.5.1.min.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/js/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/static/rest_framework/js/prettify-min.js` & `cryton_core-2023.1.2/cryton_core/static/rest_framework/js/prettify-min.js`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/cryton_core/urls.py` & `cryton_core-2023.1.2/cryton_core/urls.py`

 * *Files identical despite different names*

### Comparing `cryton_core-2022.2.2/pyproject.toml` & `cryton_core-2023.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cryton-core"
-version = "2022.2.2"
+version = "2023.1.2"
 description = "Advanced scheduler for attack scenarios"
 authors = [
     "Ivo Nutár <nutar@ics.muni.cz>",
     "Milan Boháček <bohacek@ics.muni.cz>",
     "Jiří Rája <raja@ics.muni.cz>",
     "Andrej Tomči <tomci@ics.muni.cz>"
 ]
@@ -18,45 +18,47 @@
 documentation = "https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/"
 keywords = [
     "cryton", "core", "advanced", "scheduler"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-APScheduler = "~3.8.1"
-Django = "~4.0.1"
-django-cors-headers = "~3.11.0"
-djangorestframework = "~3.13.1"
-drf-spectacular = "~0.21.2"
-drf-spectacular-sidecar = "~2022.2.21"
-Jinja2 = "~3.0.3"
-model-bakery = "~1.4.0"
-psycopg2-binary = "~2.9.5"
-PyYAML = "~6.0"
-rpyc = "~5.0.1"
-schema = "~0.7.5"
-structlog = "~21.5.0"
-pytz = "~2021.3"
-AMQPStorm = "~2.10.4"
-uuid = "~1.30"
-SQLAlchemy = "~1.4.29"
-gunicorn = "~20.1.0"
-uvicorn = "~0.17.5"
-tzlocal = "~4.1"
-python-dotenv = "~0.20.0"
+python = ">=3.8,<3.12"
+APScheduler = "^3.8.1"
+Django = "^4.0.1"
+django-cors-headers = "^3.13.0"
+djangorestframework = "^3.14.0"
+drf-spectacular = "^0.26.0"
+drf-spectacular-sidecar = "^2023.3.1"
+Jinja2 = "^3.0.3"
+psycopg2-binary = "^2.9.5"
+PyYAML = "^6.0"
+rpyc = "^5.3.0"
+schema = "^0.7.5"
+structlog = "^22.3.0"
+pytz = "^2022.7"
+AMQPStorm = "^2.10.4"
+uuid = "^1.30"
+SQLAlchemy = "^1.4.29"
+gunicorn = "^20.1.0"
+uvicorn = "^0.20.0"
+tzlocal = "^4.1"
+python-dotenv = "^1.0.0"
+click = "^8.1.3"
 
-[tool.poetry.dev-dependencies]
-pytest = "~6.2.5"
-pytest-cov = "~3.0.0"
-pytest-django = "~4.5.2"
-pytest-mock = "~3.6.1"
+[tool.poetry.group.dev.dependencies]
+pytest = "^6.2.5"
+pytest-cov = "^3.0.0"
+pytest-django = "^4.5.2"
+pytest-mock = "^3.6.1"
+model-bakery = "^1.4.0"
+tox = "^4.4.4"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 cryton-core = 'cryton_core.manage:main'
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.settings"
```

