# Comparing `tmp/redturtle.prenotazioni-2.0.0.dev1.tar.gz` & `tmp/redturtle.prenotazioni-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.prenotazioni-2.0.0.dev1.tar", last modified: Mon Jun 12 13:12:19 2023, max compression
+gzip compressed data, was "redturtle.prenotazioni-2.0.0.dev2.tar", last modified: Fri Jun 30 10:39:22 2023, max compression
```

## Comparing `redturtle.prenotazioni-2.0.0.dev1.tar` & `redturtle.prenotazioni-2.0.0.dev2.tar`

### file list

```diff
@@ -1,283 +1,284 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      748 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/APP_IO.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6585 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       79 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      110 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    24194 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16268 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      164 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/TODO.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/constraints-5.2.x.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       27 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/constraints.txt
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7921 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      476 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/requirements-6.0.x.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       48 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/requirements.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      344 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3275 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2297 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2132 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/mail.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5157 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/booker.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4573 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4440 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/conflict.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/slot.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6903 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/stringinterp.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1779 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/add_edit_view.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1816 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/base.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7801 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      541 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/custom_radio_input.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4782 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/delete_reservation.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      674 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/folderfactories.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      155 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/overrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/overrides/.gitkeep
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3168 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    14679 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_add.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6920 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_move.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2038 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_print.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    30483 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1736 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11366 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_search.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/.gitkeep
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      364 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/calendar-add.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      503 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/calendar-icon.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      266 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/cross-icon.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9794 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1600 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      922 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/times-solid.png
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2108 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2377 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
--rw-rw-r--   0 mauro     (1000) mauro     (1000)   342590 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      148 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4616 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4486 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1059 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2718 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1555 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      103 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1507 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1261 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/index.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/utils/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      941 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      298 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      614 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3862 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/booking_stats.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      575 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2809 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5466 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2300 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       42 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/nofollow.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8165 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    10429 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    15258 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2266 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5916 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4895 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1892 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/week.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      333 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9540 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/vacations.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1524 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/viewlets.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    10867 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/week.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1193 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/widget.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6310 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      383 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/config.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2327 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1785 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/pause.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7355 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_day.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16926 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_folder.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_week.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_year.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8119 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/validators.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2080 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      214 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/handlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6160 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1567 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/events_logger.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      835 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1189 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/prenotazioni_folder.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      211 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      832 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/searchable_text.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1191 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexes.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    35726 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/it/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    45854 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      830 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/manual.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    35854 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1618 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/update.sh
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/monkeypatcher/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/monkeypatcher/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      499 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1282 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/permissions.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/prenotazione_event.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2345 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/actions.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      192 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6189 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/contentrules.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/metadata.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5093 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1980 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      914 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1645 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3551 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3811 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3094 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3795 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3796 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      564 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7373 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7623 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1402/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1381 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1500/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      196 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1500/types.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      412 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      123 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      199 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      309 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3328 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      559 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      162 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4469 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/add.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1152 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/delete.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1166 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      409 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4198 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      279 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1926 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/search.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      308 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      395 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1848 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2998 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6955 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/app_io.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5302 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/README.md
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      246 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8614 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1034 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/cli.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16384 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/io.db
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       45 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/io_tools.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1945 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/monkey.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2825 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    27521 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/storage.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1062 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3197 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6283 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_booking_info.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_booking_schema.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8293 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_delete_booking.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9673 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9236 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_month_slots.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5762 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5913 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8811 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3536 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    12116 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6301 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/upgrades.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2798 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/upgrades.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/dateutils.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1119 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/urls.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      472 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/app_io.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/templates/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      957 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/templates/app_io.pt
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1096 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      607 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/gates.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1010 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      598 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/review_states.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1696 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/tipologies.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1054 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2549 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_months.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1367 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    24194 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    12223 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      179 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      748 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/APP_IO.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6889 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       79 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      110 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    24498 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16268 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      164 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/TODO.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/constraints-5.2.x.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       27 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/constraints.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.401210 redturtle.prenotazioni-2.0.0.dev2/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7921 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      476 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/requirements-6.0.x.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       48 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/requirements.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      344 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3282 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.401210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.405210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2297 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.405210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      226 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3325 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/mail.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.405210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5157 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/booker.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4924 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4440 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/conflict.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3979 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/ical.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/slot.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6903 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/stringinterp.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1816 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/base.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7260 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      541 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/custom_radio_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4782 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/delete_reservation.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      674 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/folderfactories.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      155 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/overrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/overrides/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3168 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    14679 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_add.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6919 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_move.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2038 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_print.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    30638 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1736 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    11366 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_search.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      364 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/calendar-add.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      503 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/calendar-icon.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      266 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/cross-icon.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9794 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1600 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      922 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/times-solid.png
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2108 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2377 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)   342590 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      148 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4616 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4486 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1059 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2718 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1555 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      103 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1507 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1261 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/index.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/utils/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      941 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      298 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      614 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3862 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/booking_stats.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      575 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2809 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5466 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2300 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       42 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/nofollow.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8165 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10429 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    15258 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2266 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5916 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4895 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1892 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/week.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      333 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9540 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/vacations.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1524 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/viewlets.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10867 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/week.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1193 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/widget.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6310 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      383 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/config.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2327 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1785 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/pause.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7355 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_day.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    17762 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_folder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_week.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_year.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8119 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/validators.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2080 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      214 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/handlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6160 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1567 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/events_logger.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      835 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1189 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/prenotazioni_folder.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      211 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      832 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/searchable_text.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1191 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexes.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    35726 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/it/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    45854 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      830 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/manual.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    35854 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1618 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/update.sh
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/monkeypatcher/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/monkeypatcher/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      499 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1282 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/permissions.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/prenotazione_event.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2345 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/actions.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      192 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6288 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/contentrules.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/metadata.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5093 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1980 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      914 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1645 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3551 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3811 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3094 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3795 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3796 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      564 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7373 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7623 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1402/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1381 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1500/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      196 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1500/types.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      412 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      123 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      199 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      309 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3380 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      559 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      162 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4469 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/add.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1152 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/delete.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1166 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      409 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4198 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      279 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1926 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      308 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      395 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2209 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2998 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6955 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/app_io.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5302 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/README.md
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      246 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8614 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1034 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/cli.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16384 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/io.db
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       45 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/io_tools.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1945 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/monkey.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2825 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    27521 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/storage.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1062 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3271 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6283 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_booking_info.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_booking_schema.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8293 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_delete_booking.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9673 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10405 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_month_slots.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5762 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5913 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8811 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9432 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_send_ical.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3536 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12116 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6301 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/upgrades.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2798 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/upgrades.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/dateutils.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1119 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/urls.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      472 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/app_io.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/templates/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      957 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/templates/app_io.pt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1096 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      607 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/gates.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1010 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      598 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/review_states.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1696 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/tipologies.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1054 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2549 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_months.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1367 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.401210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    24498 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12266 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      179 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      399 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/top_level.txt
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/APP_IO.txt` & `redturtle.prenotazioni-2.0.0.dev2/APP_IO.txt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/CHANGES.rst` & `redturtle.prenotazioni-2.0.0.dev2/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 Changelog
 =========
 
 
+2.0.0.dev2 (2023-06-30)
+-----------------------
+
+- reorganize backend form
+  [mamico]
+
+- booking_type filter in @months-slots
+  [mamico]
+
+- Register adapters for IMailFromFieldAction for both Site root and dx containers.
+  [cekk]
+
 2.0.0.dev1 (2023-06-12)
 -----------------------
 
 - Add Booking restapi
   [mamico]
 
 - Fix Plone6 compatibility.
@@ -34,17 +46,22 @@
 - Added field "cosa_serve" (#40445).
   [daniele]
 
 - Refactor booking delete machinery and remove unused token.
   [cekk]
 
 - Add DELETE endpoint for booking.
+  [cekk]
+
 - Add new field that allows to override week schedule for a certain date range.
   [cekk]
 
+- Send iCal attachment on approved or moved booking.
+  [cekk]
+
 1.7.1 (2023-03-28)
 ------------------
 
 - Add plone5 profile to setup.
   [foxtrot-dfm1]
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/DEVELOP.rst` & `redturtle.prenotazioni-2.0.0.dev2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/LICENSE.GPL` & `redturtle.prenotazioni-2.0.0.dev2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/LICENSE.rst` & `redturtle.prenotazioni-2.0.0.dev2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/PKG-INFO` & `redturtle.prenotazioni-2.0.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -633,14 +633,26 @@
 - Daniele Andreotti, daniele.andreotti@redturtle.it
 
 
 Changelog
 =========
 
 
+2.0.0.dev2 (2023-06-30)
+-----------------------
+
+- reorganize backend form
+  [mamico]
+
+- booking_type filter in @months-slots
+  [mamico]
+
+- Register adapters for IMailFromFieldAction for both Site root and dx containers.
+  [cekk]
+
 2.0.0.dev1 (2023-06-12)
 -----------------------
 
 - Add Booking restapi
   [mamico]
 
 - Fix Plone6 compatibility.
@@ -669,17 +681,22 @@
 - Added field "cosa_serve" (#40445).
   [daniele]
 
 - Refactor booking delete machinery and remove unused token.
   [cekk]
 
 - Add DELETE endpoint for booking.
+  [cekk]
+
 - Add new field that allows to override week schedule for a certain date range.
   [cekk]
 
+- Send iCal attachment on approved or moved booking.
+  [cekk]
+
 1.7.1 (2023-03-28)
 ------------------
 
 - Add plone5 profile to setup.
   [foxtrot-dfm1]
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/README.rst` & `redturtle.prenotazioni-2.0.0.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/docs/conf.py` & `redturtle.prenotazioni-2.0.0.dev2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/setup.py` & `redturtle.prenotazioni-2.0.0.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.prenotazioni",
-    version="2.0.0.dev1",
+    version="2.0.0.dev2",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -54,15 +54,15 @@
     python_requires=">=3.8",
     install_requires=[
         "setuptools",
         # -*- Extra requirements: -*-
         "z3c.jbot",
         "plone.api>=1.8.4",
         "plone.restapi",
-        "collective.contentrules.mailfromfield",
+        "collective.contentrules.mailfromfield>=1.2.0",
         "pyinter",
         "collective.honeypot",
         "collective.z3cform.datagridfield>=2.0",
         "pyexcel_ods3",
         "click",
         # FIXME: se si rimuove il profilo di caching da qui (perchè c'è?), si può togliere anche questo pin
         # 3.0.0a14 e successive richiedono plone.base che è solo su plone 6
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/__init__.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/mail.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/mail.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,49 +3,56 @@
 from Acquisition import aq_inner
 from collective.contentrules.mailfromfield import logger
 from collective.contentrules.mailfromfield.actions.mail import IMailFromFieldAction
 from collective.contentrules.mailfromfield.actions.mail import (
     MailActionExecutor as BaseExecutor,
 )
 from plone.contentrules.rule.interfaces import IExecutable
+from plone.dexterity.interfaces import IDexterityContainer
+from plone.event.interfaces import IICalendar
 from Products.CMFPlone.interfaces.siteroot import IPloneSiteRoot
+from redturtle.prenotazioni.prenotazione_event import IMovedPrenotazione
 from six.moves import filter
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 import six
 
 
-@implementer(IExecutable)
-@adapter(IPloneSiteRoot, IMailFromFieldAction, Interface)
 class MailActionExecutor(BaseExecutor):
     """The executor for this action."""
 
     def get_target_obj(self):
         """Get's the target object, i.e. the object that will provide the field
         with the email address
         """
+        event_obj = self.event.object
+        if event_obj.portal_type != "Prenotazione":
+            return super().get_target_obj()
         target = self.element.target
         if target == "object":
             obj = self.context
         elif target == "parent":
-            obj = self.event.object.aq_parent
-            # NEEDED JUST FOR PRENOTAZIONI...
-            return obj
+            # this is the patch
+            return event_obj.aq_parent
         elif target == "target":
-            obj = self.event.object
+            obj = event_obj
         else:
             raise ValueError(target)
         return aq_base(aq_inner(obj))
 
     def get_recipients(self):
         """
         The recipients of this mail
         """
+
+        if self.event.object.portal_type != "Prenotazione":
+            return super().get_recipients()
+
         # Try to load data from the target object
         fieldName = str(self.element.fieldName)
         obj = self.get_target_obj()
 
         attr = getattr(obj, fieldName)
         if hasattr(attr, "__call__"):
             recipients = attr()
@@ -56,7 +63,38 @@
 
         # now transform recipients in a iterator, if needed
         if type(recipients) == str or type(recipients) == six.text_type:
             recipients = [str(recipients)]
         if not recipients:
             return []
         return list(filter(bool, recipients))
+
+    def manage_attachments(self, msg):
+        booking = self.event.object
+        action = getattr(self.event, "action", "")
+        if (
+            not (action == "confirm" or IMovedPrenotazione.providedBy(self.event))
+            or booking.portal_type != "Prenotazione"
+        ):
+            return
+        cal = IICalendar(booking)
+        ical = cal.to_ical()
+        name = f"{booking.getId()}.ics"
+
+        msg.add_attachment(
+            ical,
+            maintype="text",
+            subtype="calendar",
+            filename=name,
+        )
+
+
+@implementer(IExecutable)
+@adapter(IPloneSiteRoot, IMailFromFieldAction, Interface)
+class MailActionExecutorRoot(MailActionExecutor):
+    """Registered for site root"""
+
+
+@implementer(IExecutable)
+@adapter(IDexterityContainer, IMailFromFieldAction, Interface)
+class MailActionExecutorFolder(MailActionExecutor):
+    """Registered for folderish content"""
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/booker.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -144,8 +144,21 @@
   <adapter
       factory=".stringinterp.BookingUrlWithDeleteToken"
       provides="plone.stringinterp.interfaces.IStringSubstitution"
       for="*"
       name="booking_url_with_delete_token"
       />
 
+
+  <!-- ical adapters -->
+  <adapter
+      factory=".ical.ICalendarBookingComponent"
+      for="redturtle.prenotazioni.content.prenotazione.IPrenotazione"
+      />
+
+  <adapter
+      factory=".ical.calendar_from_booking"
+      provides="plone.event.interfaces.IICalendar"
+      for="redturtle.prenotazioni.content.prenotazione.IPrenotazione"
+      />
+
 </configure>
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/conflict.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/conflict.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/slot.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/stringinterp.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/base.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/base.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/configure.zcml`

 * *Files 5% similar despite different names*

```diff
@@ -21,31 +21,14 @@
       directory="static"
       name="redturtle.prenotazioni"
       type="plone"
       />
 
   <include package=".stats" />
 
-
-  <browser:page
-      name="edit"
-      for="..content.prenotazioni_folder.IPrenotazioniFolder"
-      class=".add_edit_view.DefaultEditView"
-      permission="cmf.ModifyPortalContent"
-      />
-
-  <adapter
-      factory=".add_edit_view.DefaultAddView"
-      provides="zope.publisher.interfaces.browser.IBrowserPage"
-      for="Products.CMFPlone.interfaces.siteroot.IPloneSiteRoot
-           zope.publisher.interfaces.browser.IDefaultBrowserLayer
-           plone.dexterity.interfaces.IDexterityFTI"
-      name="PrenotazioniFolder"
-      />
-
   <include package="plone.app.contentmenu" />
 
 
   <!-- macros to be used in a prenotazione -->
   <browser:page
       name="prenotazione_macros"
       for="..content.prenotazioni_folder.IPrenotazioniFolder"
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/custom_radio_input.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/custom_radio_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/delete_reservation.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/delete_reservation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/folderfactories.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_add.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_move.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_move.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,17 +128,17 @@
             "form.buttons.action_move": "Move",
             "data": self.request.form.get("data", ""),
             "form.widgets.gate": gate,
         }
         times = slot.get_values_hr_every(300)
         urls = []
         base_url = "/".join((self.context.absolute_url(), "prenotazione_move"))
-        now_str = tznow().strftime("%Y-%m-%d %H:%M")
+        now_str = tznow().strftime("%Y-%m-%dT%H:%M")
         for t in times:
-            form_booking_date = " ".join((date, t))
+            form_booking_date = "T".join((date, t))
             params["form.widgets.booking_date"] = form_booking_date
             urls.append(
                 {
                     "title": t,
                     "url": addTokenToUrl(urlify(base_url, params=params)),
                     "class": t.endswith(":00") and "oclock" or None,
                     "future": (now_str <= form_booking_date),
@@ -155,15 +155,14 @@
         data["booking_type"] = self.context.getBooking_type()
         conflict_manager = self.prenotazioni_view.conflict_manager
         current_data = self.context.getBooking_date()
         current = {"booking_date": current_data, "booking_type": data["booking_type"]}
         current_slot = conflict_manager.get_choosen_slot(current)
         current_gate = getattr(self.context, "gate", "")
         exclude = {current_gate: [current_slot]}
-
         if conflict_manager.conflicts(data, exclude=exclude):
             msg = _(
                 "Sorry, this slot is not available or does not fit your " "booking."
             )
             api.portal.show_message(msg, self.request, type="error")
             raise ActionExecutionError(Invalid(msg))
         if self.exceedes_date_limit(data):
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_print.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_print.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,18 @@
     @property
     @memoize
     def base_booking_url(self):
         """Return the base booking url (no parameters) for this context"""
         return "%s/%s" % (self.context.absolute_url(), self.add_view)
 
     def get_booking_urls(self, day, slot, slot_min_size=0, gate=None):
-        """Returns, if possible, the booking urls"""
+        """Returns, if possible, the booking urls
+
+        slot_min_size: seconds
+        """
         # we have some conditions to check
         if not self.is_valid_day(day):
             return []
         if self.maximum_bookable_date:
             if day > self.maximum_bookable_date.date():
                 return []
         date = day.strftime("%Y-%m-%d")
@@ -330,15 +333,18 @@
                     "booking_date": booking_date,
                     "future": (now_str <= form_booking_date),
                 }
             )
         return urls
 
     def get_all_booking_urls_by_gate(self, day, slot_min_size=0):
-        """Get all the booking urls divided by gate"""
+        """Get all the booking urls divided by gate
+
+        slot_min_size: seconds
+        """
         slots_by_gate = self.get_free_slots(day)
         urls = {}
         for gate in slots_by_gate:
             slots = slots_by_gate[gate]
             for slot in slots:
                 slot_urls = self.get_booking_urls(
                     day, slot, slot_min_size=slot_min_size
@@ -346,14 +352,16 @@
                 urls.setdefault(gate, []).extend(slot_urls)
         return urls
 
     def get_all_booking_urls(self, day, slot_min_size=0):
         """Get all the booking urls
 
         Not divided by gate
+
+        slot_min_size: seconds
         """
         urls_by_gate = self.get_all_booking_urls_by_gate(day, slot_min_size)
         urls = {}
         for gate in urls_by_gate:
             for url in urls_by_gate[gate]:
                 urls[url["title"]] = url
         return sorted(six.itervalues(urls), key=lambda x: x["title"])
@@ -367,15 +375,18 @@
                 if intersection:
                     if intersection.lower_value != intersection.upper_value:
                         return False
         return True
 
     @memoize
     def get_anonymous_booking_url(self, day, slot, slot_min_size=0):
-        """Returns, the the booking url for an anonymous user"""
+        """Returns, the the booking url for an anonymous user
+
+        slot_min_size: seconds
+        """
         # First we check if we have booking urls
         all_booking_urls = self.get_all_booking_urls(day, slot_min_size)
         if not all_booking_urls:
             # If not the slot can be unavailable or busy
             if self.is_slot_busy(day, slot):
                 return self.busy_slot_booking_url
             else:
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_search.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/times-solid.png` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/times-solid.png`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/index.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/booking_stats.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/booking_stats.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/booking_stats.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/week.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/week.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/vacations.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/vacations.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/viewlets.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/week.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/week.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/widget.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/z3c_custom_widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/pause.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/pause.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_folder.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     return data
 
 
 class IWeekTableRow(model.Schema):
     day = schema.TextLine(
         title=_("day_label", default="Day of week"), required=True, default=""
     )
+    form.mode(day="display")
     morning_start = schema.Choice(
         title=_("morning_start_label", default="Start time in the morning"),
         vocabulary="redturtle.prenotazioni.VocOreInizio",
         required=False,
     )
     morning_end = schema.Choice(
         title=_("morning_end_label", default="End time in the morning"),
@@ -134,14 +135,16 @@
     textindexer.searchable("descriptionAgenda")
     descriptionAgenda = RichText(
         required=False,
         title=_("Descrizione Agenda", default="Descrizione Agenda"),
         description=_("Inserire il testo di presentazione dell'agenda corrente"),
     )
 
+    form.mode(descriptionAgenda="display")
+
     cosa_serve = schema.Text(
         required=False,
         title=_("Cosa serve", default="Cosa serve"),
         description=_(
             "Elencare le informazioni utili per il giorno della prenotazione, come ad esempio i documenti da presentare."
         ),
     )
@@ -273,15 +276,21 @@
                 "afternoon_start": None,
                 "morning_end": None,
                 "afternoon_end": None,
             },
         ],
     )
     form.widget(
-        "week_table", DataGridFieldFactory, frontendOptions={"widget": "data_grid"}
+        "week_table",
+        DataGridFieldFactory,
+        allow_insert=False,
+        allow_delete=False,
+        allow_reorder=False,
+        auto_append=False,
+        frontendOptions={"widget": "data_grid"},
     )
 
     week_table_overrides = schema.SourceText(
         title=_("week_table_overrides_label", default="Week table overrides"),
         description=_(
             "week_table_overrides_help",
             default="Insert here week schema for some custom date intervals.",
@@ -437,21 +446,50 @@
                 if interval["morning_start"] > interval["morning_end"]:
                     raise Invalid(_("Morning start should not be greater than end."))
             if interval["afternoon_start"] and interval["afternoon_end"]:
                 if interval["afternoon_start"] > interval["afternoon_end"]:
                     raise Invalid(_("Afternoon start should not be greater than end."))
 
     # TODO: definire o descrivere quando avviee la notifica
+    # TODO: inserire qui la chiave IO ? o su un config in zope.conf/environment ?
     app_io_enabled = schema.Bool(
         title=_("App IO notification"),
         default=False,
         required=False,
     )
 
-    # TODO: inserire qui la chiave IO ? o su un config in zope.conf/environment ?
+    model.fieldset(
+        "dates",
+        label=_("Date validità"),
+        fields=[
+            "daData",
+            "aData",
+            "same_day_booking_disallowed",
+            "holidays",
+            "futureDays",
+            "notBeforeDays",
+            "pause_table",
+        ],
+    )
+
+    model.fieldset(
+        "week_table",
+        label=_("Week table"),
+        fields=[
+            "week_table",
+        ],
+    )
+
+    model.fieldset(
+        "week_table_overrides",
+        label=_("week_table_overrides_label", default="Week table overrides"),
+        fields=[
+            "week_table_overrides",
+        ],
+    )
 
     model.fieldset(
         "contacts",
         label=_("contacts_label", default="Contacts"),
         description=_(
             "contacts_help",
             default="Show here contacts information that will be used by authomatic mail system",  # noqa
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/validators.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/validators.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/events_logger.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/events_logger.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/prenotazioni_folder.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/searchable_text.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/searchable_text.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexes.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexes.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/interfaces.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/manual.pot` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/update.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/permissions.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/permissions.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/actions.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/contentrules.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/contentrules.xml`

 * *Files 14% similar despite different names*

#### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/contentrules.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/contentrules.xml`

```diff
@@ -12,40 +12,41 @@
           <element>confirm</element>
         </property>
       </condition>
     </conditions>
     <actions>
       <action type="plone.actions.MailFromField">
         <property name="source"/>
-        <property name="message">La prenotazione per ${title} è stata accettata. Il codice di prenotazione è ${booking_code}</property>
-        <property name="message">La prenotazione per ${title} e' stata accettata.
+        <property name="message">La prenotazione ${booking_type} è stata accettata.
 
-Se desideri visualizzare, stampare o cancellare questa prenotazione puoi utilizzare il seguente link: ${booking_print_url}</property>
+Se desideri visualizzare, stampare o cancellare questa prenotazione puoi utilizzare il [seguente link](${booking_print_url})</property>
+        <property name="is_markdown">True</property>
         <property name="fieldName">email</property>
         <property name="target">target</property>
-        <property name="subject">Prenotazione del ${booking_date} alle ${booking_time} accettata</property>
+        <property name="subject">Prenotazione ${booking_type} del ${booking_date} alle ${booking_time} accettata</property>
       </action>
     </actions>
   </rule>
   <rule name="booking-moved" title="Invia un'email all'utente quando la data della prenotazione viene cambiata" description="Viene inviata una mail al richiedente per avvertire dello spostamento della prenotazione" enabled="True" event="redturtle.prenotazioni.prenotazione_event.IMovedPrenotazione" stop-after="False">
     <conditions>
       <condition type="plone.conditions.PortalType">
         <property name="check_types">
           <element>Prenotazione</element>
         </property>
       </condition>
     </conditions>
     <actions>
       <action type="plone.actions.MailFromField">
         <property name="source"/>
-        <property name="message">L'orario della sua prenotazione &quot;${title}&quot; e' stata modificato.
+        <property name="message">L'orario della sua prenotazione ${booking_type} è stata modificato.
 
 La nuova data è ${booking_date} alle ore ${booking_time}.
 
-Controlla o stampa il nuovo promemoria a questo link: ${booking_print_url}</property>
+Controlla o stampa il nuovo promemoria su [questo link](${booking_print_url}).</property>
+        <property name="is_markdown">True</property>
         <property name="fieldName">email</property>
         <property name="target">target</property>
         <property name="subject">Modifica data di prenotazione per ${title}</property>
       </action>
     </actions>
   </rule>
   <rule name="booking-created-user" title="Invia un'email all'utente quando la prenotazione è stata creata" description="Viene inviata una mail all'utente per avvertirlo della creazione della prenotazione" enabled="True" event="Products.CMFCore.interfaces.IActionSucceededEvent" stop-after="False">
@@ -60,19 +61,20 @@
           <element>submit</element>
         </property>
       </condition>
     </conditions>
     <actions>
       <action type="plone.actions.MailFromField">
         <property name="source"/>
-        <property name="message">La prenotazione per il ${booking_date} alle ${booking_time} è stata creata.
+        <property name="message">La prenotazione ${booking_type} per il ${booking_date} alle ${booking_time} è stata creata.
 
 Riceverete una mail di conferma quando la prenotazione verrà confermata definitivamente.
 
-Se non hai salvato o stampato il promemoria, puoi visualizzarlo a questo link: ${booking_print_url}</property>
+Se non hai salvato o stampato il promemoria, puoi visualizzarlo su [questo link](${booking_print_url})</property>
+        <property name="is_markdown">True</property>
         <property name="fieldName">email</property>
         <property name="target">target</property>
         <property name="subject">Prenotazione creata correttamente per ${title}</property>
       </action>
     </actions>
   </rule>
   <rule name="booking-refuse" title="Invia un'email all'utente quando la prenotazione è stata rifiutata" description="Viene inviata una mail all'utente per avvisarlo della prenotazione rifiutata" enabled="True" event="Products.CMFCore.interfaces.IActionSucceededEvent" stop-after="False">
@@ -87,15 +89,15 @@
           <element>refuse</element>
         </property>
       </condition>
     </conditions>
     <actions>
       <action type="plone.actions.MailFromField">
         <property name="source"/>
-        <property name="message">La prenotazione del ${booking_date} delle ore ${booking_time} è stata rifiutata.</property>
+        <property name="message">La prenotazione ${booking_type} del ${booking_date} delle ore ${booking_time} è stata rifiutata.</property>
         <property name="fieldName">email</property>
         <property name="target">target</property>
         <property name="subject">Prenotazione rifiutata per ${title}</property>
       </action>
     </actions>
   </rule>
   <rule name="booking-confirm" title="Conferma automatica prenotazioni" cascading="False" description="Conferma automatica degli appuntamenti" enabled="True" event="Products.CMFCore.interfaces.IActionSucceededEvent" stop-after="False">
@@ -113,17 +115,20 @@
     </conditions>
     <actions>
       <action type="plone.actions.Mail">
         <property name="subject">Prenotazione del ${booking_date} alle ${booking_time} accettata</property>
         <property name="source"/>
         <property name="recipients">${booking_user_email}</property>
         <property name="exclude_actor">False</property>
-        <property name="message">La prenotazione per ${title} e' stata confermata!
-     Se non hai salvato o stampato il promemoria, puoi visualizzarlo a questo link: ${booking_print_url}
-     Se desideri cancellare la prenotazione, accedi all'indirizzo ${booking_print_url}</property>
+        <property name="message">La prenotazione ${booking_type} per ${title} è stata confermata!
+
+Se non hai salvato o stampato il promemoria, puoi visualizzarlo su [questo link](${booking_print_url})
+     
+Se desideri cancellare la prenotazione, accedi all'[indirizzo](${booking_print_url})</property>
+        <property name="is_markdown">True</property>
       </action>
       <action type="plone.actions.Workflow">
         <property name="transition">confirm</property>
       </action>
     </actions>
   </rule>
 </contentrules>
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/resources.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self.reqeuest = request
 
     def __call__(self, *args, **kwargs):
         booking_folder = self.prenotazione.getPrenotazioniFolder()
         useful_docs = getattr(booking_folder, "cosa_serve", "")
         return {
             "UID": self.prenotazione.UID(),
+            "@type": self.prenotazione.portal_type,
             "title": self.prenotazione.title,
             "description": self.prenotazione.description,
             "gate": self.prenotazione.gate,
             "id": self.prenotazione.id,
             "phone": self.prenotazione.phone,
             "email": self.prenotazione.email,
             "fiscalcode": self.prenotazione.fiscalcode,
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/add.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/delete.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/delete.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/get.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/search.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/get.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/get.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,24 @@
             "prenotazioni_week_view", context=self.context, request=self.request
         )
         now = self.request.form.get("date", "")
         if now:
             now = date.fromisoformat(now)
         else:
             now = date.today()
-
+        booking_type = self.request.form.get("booking_type")
+        if booking_type:
+            slot_min_size = (
+                prenotazioni_week_view.prenotazioni.get_booking_type_duration(
+                    booking_type
+                )
+                * 60
+            )  # noqa
+        else:
+            slot_min_size = 0
         start_year = now.year
         start_month = now.month
         start_day = now.day
 
         response = {"@id": f"{self.context.absolute_url()}/@month_slots", "items": []}
         for week in calendar.monthcalendar(start_year, start_month):
             for day in week:
@@ -37,15 +46,15 @@
                 booking_date = date(start_year, start_month, day)
                 slots = prenotazioni_week_view.prenotazioni.get_anonymous_slots(
                     booking_date=booking_date
                 )
                 for slot in slots.get("anonymous_gate", []):
                     info = (
                         prenotazioni_week_view.prenotazioni.get_anonymous_booking_url(
-                            booking_date, slot
+                            booking_date, slot, slot_min_size=slot_min_size
                         )
                     )
                     if not info.get("url", ""):
                         continue
                     response["items"].append(
                         json_compatible(info.get("booking_date", ""))
                     )
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/get.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/app_io.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/app_io.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/README.md` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/api.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/cli.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/cli.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/io.db` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/io.db`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/monkey.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/storage.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/storage.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/setuphandlers.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/testing.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
+from plone.app.testing import MOCK_MAILHOST_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.restapi.testing import PloneRestApiDXLayer
 from plone.testing import z2
 
 import collective.contentrules.mailfromfield
 import collective.z3cform.datagridfield
 import plone.app.caching
@@ -18,15 +19,15 @@
 
     HAS_DX_TEXTINDEXER = True
 except ImportError:
     HAS_DX_TEXTINDEXER = False
 
 
 class RedturtlePrenotazioniLayer(PloneSandboxLayer):
-    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
+    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE, MOCK_MAILHOST_FIXTURE)
 
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
         # layer.
         self.loadZCML(package=plone.app.caching)
         self.loadZCML(package=plone.restapi)
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_booking_info.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_booking_info.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_booking_schema.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_booking_schema.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_delete_booking.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_delete_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_delete_booking_api.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_delete_booking_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_month_slots.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_month_slots.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                     "morning_end": None,
                     "afternoon_start": None,
                     "afternoon_end": None,
                 },
             ],
             booking_types=[
                 {"name": "Type A", "duration": "30"},
+                {"name": "Type B", "duration": "90"},
             ],
             gates=["Gate A"],
         )
 
         year = api.content.create(
             container=self.folder_prenotazioni, type="PrenotazioniYear", title="Year"
         )
@@ -101,14 +102,15 @@
             container=week, type="PrenotazioniDay", title="Day"
         )
         transaction.commit()
 
     def tearDown(self):
         self.api_session.close()
 
+    @unittest.skip("issue testing in the last days of a month")
     def test_month_slots_called_without_params_return_all_available_slots_of_current_month(
         self,
     ):
         response = self.api_session.get(
             "{}/@month-slots".format(self.folder_prenotazioni.absolute_url())
         )
         # get next mondays in current month
@@ -122,15 +124,14 @@
             if week[0] > current_day:
                 for hour in [7, 8, 9]:
                     expected.append(
                         json_compatible(
                             datetime(current_year, current_month, week[0], hour, 0)
                         )
                     )
-
         self.assertEqual(expected, response.json()["items"])
 
     def test_month_slots_called_without_params_return_available_slots_of_current_month_when_some_are_full(
         self,
     ):
         now = date.today()
         current_year = now.year
@@ -215,14 +216,15 @@
                     expected.append(
                         json_compatible(
                             datetime(current_year, next_month, monday, hour, 0)
                         )
                     )
         self.assertEqual(expected, response.json()["items"])
 
+    @unittest.skipIf(date.today().day > 20, "issue testing in the last days of a month")
     def test_month_slots_notBeforeDays_honored(
         self,
     ):
         now = date.today()
         week_table = []
         for i in range(0, 7):
             data = {
@@ -261,7 +263,30 @@
         self.assertNotIn(tomorrow, response.json()["items"])
 
         folder.notBeforeDays = 0
         transaction.commit()
 
         response = self.api_session.get("{}/@month-slots".format(folder.absolute_url()))
         self.assertIn(tomorrow, response.json()["items"])
+
+    @unittest.skipIf(date.today().day > 20, "issue testing in the last days of a month")
+    def test_month_slots_filtered_by_booking_type(self):
+        # Type A 30 minutes
+        response = self.api_session.get(
+            f"{self.folder_prenotazioni.absolute_url()}/@month-slots?booking_type=Type A"
+        )  # noqa
+        self.assertEqual(response.status_code, 200)
+
+        # crappy test .... TODO: rethink
+        # self.assertEqual(len(response.json()["items"]), 6)
+        type_a_len = len(response.json()["items"])
+
+        # Type B 90 minutes
+        response = self.api_session.get(
+            f"{self.folder_prenotazioni.absolute_url()}/@month-slots?booking_type=Type B"
+        )  # noqa
+        self.assertEqual(response.status_code, 200)
+
+        # crappy test .... TODO: rethink
+        # self.assertEqual(len(response.json()["items"]), 4)
+        type_b_len = len(response.json()["items"])
+        self.assertTrue(type_a_len > type_b_len)
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_setup.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_week_table_overrides.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_week_table_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/upgrades.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/upgrades.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/upgrades.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/dateutils.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/dateutils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/urls.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/urls.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/templates/app_io.pt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/templates/app_io.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/gates.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/review_states.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/review_states.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/tipologies.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/tipologies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_months.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_months.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/PKG-INFO` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -633,14 +633,26 @@
 - Daniele Andreotti, daniele.andreotti@redturtle.it
 
 
 Changelog
 =========
 
 
+2.0.0.dev2 (2023-06-30)
+-----------------------
+
+- reorganize backend form
+  [mamico]
+
+- booking_type filter in @months-slots
+  [mamico]
+
+- Register adapters for IMailFromFieldAction for both Site root and dx containers.
+  [cekk]
+
 2.0.0.dev1 (2023-06-12)
 -----------------------
 
 - Add Booking restapi
   [mamico]
 
 - Fix Plone6 compatibility.
@@ -669,17 +681,22 @@
 - Added field "cosa_serve" (#40445).
   [daniele]
 
 - Refactor booking delete machinery and remove unused token.
   [cekk]
 
 - Add DELETE endpoint for booking.
+  [cekk]
+
 - Add new field that allows to override week schedule for a certain date range.
   [cekk]
 
+- Send iCal attachment on approved or moved booking.
+  [cekk]
+
 1.7.1 (2023-03-28)
 ------------------
 
 - Add plone5 profile to setup.
   [foxtrot-dfm1]
```

### Comparing `redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/SOURCES.txt` & `redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 src/redturtle/prenotazioni/actions/__init__.py
 src/redturtle/prenotazioni/actions/configure.zcml
 src/redturtle/prenotazioni/actions/mail.py
 src/redturtle/prenotazioni/adapters/__init__.py
 src/redturtle/prenotazioni/adapters/booker.py
 src/redturtle/prenotazioni/adapters/configure.zcml
 src/redturtle/prenotazioni/adapters/conflict.py
+src/redturtle/prenotazioni/adapters/ical.py
 src/redturtle/prenotazioni/adapters/prenotazione_menu.py
 src/redturtle/prenotazioni/adapters/slot.py
 src/redturtle/prenotazioni/adapters/stringinterp.py
 src/redturtle/prenotazioni/browser/__init__.py
-src/redturtle/prenotazioni/browser/add_edit_view.py
 src/redturtle/prenotazioni/browser/base.py
 src/redturtle/prenotazioni/browser/configure.zcml
 src/redturtle/prenotazioni/browser/custom_radio_input.pt
 src/redturtle/prenotazioni/browser/delete_reservation.py
 src/redturtle/prenotazioni/browser/folderfactories.py
 src/redturtle/prenotazioni/browser/interfaces.py
 src/redturtle/prenotazioni/browser/prenotazione.py
@@ -200,14 +200,15 @@
 src/redturtle/prenotazioni/tests/test_booking_schema.py
 src/redturtle/prenotazioni/tests/test_delete_booking.py
 src/redturtle/prenotazioni/tests/test_delete_booking_api.py
 src/redturtle/prenotazioni/tests/test_month_slots.py
 src/redturtle/prenotazioni/tests/test_prenotazione.py
 src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
 src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
+src/redturtle/prenotazioni/tests/test_send_ical.py
 src/redturtle/prenotazioni/tests/test_setup.py
 src/redturtle/prenotazioni/tests/test_week_table_overrides.py
 src/redturtle/prenotazioni/utilities/__init__.py
 src/redturtle/prenotazioni/utilities/dateutils.py
 src/redturtle/prenotazioni/utilities/urls.py
 src/redturtle/prenotazioni/viewlets/__init__.py
 src/redturtle/prenotazioni/viewlets/app_io.py
```

