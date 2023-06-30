# Comparing `tmp/design.plone.ioprenoto-1.0.9.tar.gz` & `tmp/design.plone.ioprenoto-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.ioprenoto-1.0.9.tar", last modified: Mon Jun 19 15:40:45 2023, max compression
+gzip compressed data, was "design.plone.ioprenoto-1.1.0.tar", last modified: Fri Jun 30 06:48:24 2023, max compression
```

## Comparing `design.plone.ioprenoto-1.0.9.tar` & `design.plone.ioprenoto-1.1.0.tar`

### file list

```diff
@@ -1,109 +1,111 @@
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.629567 design.plone.ioprenoto-1.0.9/
--rw-r--r--   0 roman      (502) staff       (20)     1059 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/CHANGES.rst
--rw-r--r--   0 roman      (502) staff       (20)       58 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/CONTRIBUTORS.rst
--rw-r--r--   0 roman      (502) staff       (20)     1338 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/DEVELOP.rst
--rw-r--r--   0 roman      (502) staff       (20)    18092 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/LICENSE.GPL
--rw-r--r--   0 roman      (502) staff       (20)      662 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/LICENSE.rst
--rw-r--r--   0 roman      (502) staff       (20)      116 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/MANIFEST.in
--rw-r--r--   0 roman      (502) staff       (20)     8527 2023-06-19 15:40:45.629737 design.plone.ioprenoto-1.0.9/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     4344 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/README.rst
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.611973 design.plone.ioprenoto-1.0.9/docs/
--rw-r--r--   0 roman      (502) staff       (20)     7986 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/docs/conf.py
--rw-r--r--   0 roman      (502) staff       (20)       89 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/docs/index.rst
--rw-r--r--   0 roman      (502) staff       (20)      340 2023-06-19 15:40:45.630244 design.plone.ioprenoto-1.0.9/setup.cfg
--rw-r--r--   0 roman      (502) staff       (20)     2774 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/setup.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.605752 design.plone.ioprenoto-1.0.9/src/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.612227 design.plone.ioprenoto-1.0.9/src/design/
--rw-r--r--   0 roman      (502) staff       (20)       80 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.614570 design.plone.ioprenoto-1.0.9/src/design/plone/
--rw-r--r--   0 roman      (502) staff       (20)       80 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.616091 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/
--rw-r--r--   0 roman      (502) staff       (20)      139 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.616979 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/adapters/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/adapters/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      562 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/adapters/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1015 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/adapters/stringinterp.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.617791 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/behaviors/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/behaviors/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1392 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/behaviors/additional_fields.py
--rw-r--r--   0 roman      (502) staff       (20)      591 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/behaviors/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.618194 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/browser/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/browser/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      628 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/browser/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.618414 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/browser/overrides/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/browser/overrides/.gitkeep
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.618717 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/browser/static/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/browser/static/.gitkeep
--rw-r--r--   0 roman      (502) staff       (20)     1530 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.619401 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/events/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/events/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      724 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/events/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1649 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/events/on_create.py
--rw-r--r--   0 roman      (502) staff       (20)      270 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.620623 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/
--rw-r--r--   0 roman      (502) staff       (20)      611 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/README.rst
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1520 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.607054 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/en/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.620855 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)     1395 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.607310 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/it/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.621188 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)     1395 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
--rw-r--r--   0 roman      (502) staff       (20)     1754 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/update.py
--rwxr-xr-x   0 roman      (502) staff       (20)      503 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/update.sh
--rw-r--r--   0 roman      (502) staff       (20)      273 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/permissions.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.607915 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.622228 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/default/
--rw-r--r--   0 roman      (502) staff       (20)      191 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      105 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/default/catalog.xml
--rw-r--r--   0 roman      (502) staff       (20)      191 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/default/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.622536 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/default/registry/
--rw-r--r--   0 roman      (502) staff       (20)      180 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/default/registry/main.xml
--rw-r--r--   0 roman      (502) staff       (20)      340 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/default/rolemap.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.622760 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/default/types/
--rw-r--r--   0 roman      (502) staff       (20)      325 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.622987 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/uninstall/
--rw-r--r--   0 roman      (502) staff       (20)      132 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.623561 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      280 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.623989 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      166 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.625042 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      414 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1685 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
--rw-r--r--   0 roman      (502) staff       (20)     2773 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.625344 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.625923 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/bookable_list/
--rw-r--r--   0 roman      (502) staff       (20)      478 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     6155 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.626783 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/bookings/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      354 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      653 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/bookings/search.py
--rw-r--r--   0 roman      (502) staff       (20)      201 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      794 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/setuphandlers.py
--rw-r--r--   0 roman      (502) staff       (20)     2326 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/testing.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.628986 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.629371 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/robot/
--rw-r--r--   0 roman      (502) staff       (20)     2019 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/robot/test_example.robot
--rw-r--r--   0 roman      (502) staff       (20)     1231 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
--rw-r--r--   0 roman      (502) staff       (20)     2873 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py
--rw-r--r--   0 roman      (502) staff       (20)     2221 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
--rw-r--r--   0 roman      (502) staff       (20)     2800 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
--rw-r--r--   0 roman      (502) staff       (20)     7008 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
--rw-r--r--   0 roman      (502) staff       (20)     2459 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_setup.py
--rw-r--r--   0 roman      (502) staff       (20)     4095 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-06-19 15:40:45.614353 design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/
--rw-r--r--   0 roman      (502) staff       (20)     8527 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     3812 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (502) staff       (20)      147 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/entry_points.txt
--rw-r--r--   0 roman      (502) staff       (20)       20 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/not-zip-safe
--rw-r--r--   0 roman      (502) staff       (20)      293 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/requires.txt
--rw-r--r--   0 roman      (502) staff       (20)        7 2023-06-19 15:40:45.000000 design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.918298 design.plone.ioprenoto-1.1.0/
+-rw-r--r--   0 cekk       (501) staff       (20)     1414 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       58 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1338 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      662 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      136 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     9034 2023-06-30 06:48:24.918498 design.plone.ioprenoto-1.1.0/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     4344 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/README.rst
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.900755 design.plone.ioprenoto-1.1.0/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7986 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       89 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      340 2023-06-30 06:48:24.919011 design.plone.ioprenoto-1.1.0/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2774 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.894194 design.plone.ioprenoto-1.1.0/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.900994 design.plone.ioprenoto-1.1.0/src/design/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.903342 design.plone.ioprenoto-1.1.0/src/design/plone/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.904911 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/
+-rw-r--r--   0 cekk       (501) staff       (20)      139 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.905626 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      562 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1471 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/stringinterp.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.906360 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1392 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/additional_fields.py
+-rw-r--r--   0 cekk       (501) staff       (20)      591 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.906794 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      628 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.907113 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/overrides/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.907305 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/static/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)     1530 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.908067 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/events/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/events/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      481 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/events/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      136 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/events/on_create.py
+-rw-r--r--   0 cekk       (501) staff       (20)      270 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.909299 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1520 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.895723 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.909810 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1395 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.896002 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.910367 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1395 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1754 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      503 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      273 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.896662 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.911354 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      191 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      191 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.911640 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)      180 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/registry/main.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      340 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.911900 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/types/
+-rw-r--r--   0 cekk       (501) staff       (20)      325 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.912143 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      132 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.912659 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      280 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.913089 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      166 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.914059 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      414 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1742 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2773 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.914306 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.915011 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookable_list/
+-rw-r--r--   0 cekk       (501) staff       (20)      478 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     6155 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.915730 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      354 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      744 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/search.py
+-rw-r--r--   0 cekk       (501) staff       (20)      201 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      794 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2248 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.917776 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.918021 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/robot/
+-rw-r--r--   0 cekk       (501) staff       (20)     2019 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/robot/test_example.robot
+-rw-r--r--   0 cekk       (501) staff       (20)     1231 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2873 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3941 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2800 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
+-rw-r--r--   0 cekk       (501) staff       (20)     7008 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2459 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4844 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.903104 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     9034 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3964 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      147 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       20 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      293 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        7 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/top_level.txt
```

### Comparing `design.plone.ioprenoto-1.0.9/DEVELOP.rst` & `design.plone.ioprenoto-1.1.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/LICENSE.GPL` & `design.plone.ioprenoto-1.1.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/LICENSE.rst` & `design.plone.ioprenoto-1.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/PKG-INFO` & `design.plone.ioprenoto-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ioprenoto
-Version: 1.0.9
+Version: 1.1.0
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/design.plone.ioprenoto
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ioprenoto/
 Project-URL: Source, https://github.com/RedTurtle/design.plone.ioprenoto
@@ -177,14 +177,33 @@
         - RedTurtle, info@redturtle.it
         
         
         Changelog
         =========
         
         
+        1.1.0 (2023-06-30)
+        ------------------
+        
+        - Move message to contentrule in iocittadino
+          [mamico]
+        
+        - Handle custom frontend_domain in notification urls (to fix the /admin problem).
+          [cekk]
+        
+        - Fix permission management in PrenotazioniFolder serializer.
+          [cekk]
+        
+        1.0.10 (2023-06-20)
+        -------------------
+        
+        - Fix the prentazione created message.
+          [folix-01]
+        
+        
         1.0.9 (2023-06-19)
         ------------------
         
         - Fix the prentazione link in the message.
           [folix-01]
```

### Comparing `design.plone.ioprenoto-1.0.9/README.rst` & `design.plone.ioprenoto-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/docs/conf.py` & `design.plone.ioprenoto-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/setup.py` & `design.plone.ioprenoto-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.ioprenoto",
-    version="1.0.9",
+    version="1.1.0",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/adapters/configure.zcml` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/behaviors/additional_fields.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/behaviors/configure.zcml` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/browser/configure.zcml` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/configure.zcml` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/README.rst` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/locales/update.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,39 +5,43 @@
 from plone.restapi.serializer.dxcontent import SerializeFolderToJson
 from plone.restapi.serializer.summary import DefaultJSONSummarySerializer
 from redturtle.prenotazioni.content.prenotazioni_folder import IPrenotazioniFolder
 from zope.component import adapter
 from zope.interface import implementer
 
 
-PRENOTAZIONI_MANAGE_PERMISSION = "redturtle.prenotazioni.ManagePrenotazioni"
+PRENOTAZIONI_MANAGE_PERMISSION = "redturtle.prenotazioni: Manage Prenotazioni"
 PRENOTAZIONE_APPUNTAMENTO_ADDRESS = "prenotazione-appuntamento"
 
 
 @implementer(ISerializeToJsonSummary)
 @adapter(IPrenotazioniFolder, IDesignPloneIoprenotoLayer)
 class SerializePrenotazioniFolderToJsonSummary(DefaultJSONSummarySerializer):
     def __call__(self, *args, **kwargs):
         if not api.user.has_permission(
-            PRENOTAZIONI_MANAGE_PERMISSION, user=api.user.get_current()
+            PRENOTAZIONI_MANAGE_PERMISSION,
+            obj=self.context,
         ):
             self.request.response.redirect(
                 self.context.portal_url() + "/" + PRENOTAZIONE_APPUNTAMENTO_ADDRESS
             )
 
             return
 
         return super().__call__(*args, **kwargs)
 
 
 @implementer(ISerializeToJson)
 @adapter(IPrenotazioniFolder, IDesignPloneIoprenotoLayer)
 class SerializePrenotazioniFolderToJson(SerializeFolderToJson):
     def __call__(self, *args, **kwargs):
-        if not api.user.has_permission(PRENOTAZIONI_MANAGE_PERMISSION):
+        if not api.user.has_permission(
+            PRENOTAZIONI_MANAGE_PERMISSION,
+            obj=self.context,
+        ):
             self.request.response.redirect(
                 self.context.portal_url() + "/" + PRENOTAZIONE_APPUNTAMENTO_ADDRESS
             )
 
             return
 
         return super().__call__(*args, **kwargs)
```

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/restapi/services/bookings/search.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,11 +7,14 @@
 from plone import api
 
 
 @implementer(IPublishTraverse)
 class BookingsSearch(BookingsSearchBase):
     def reply(self):
         response = super(BookingsSearch, self).reply()
-        base_url = f"{api.portal.get().absolute_url()}/prenotazione-appuntamenti-uffici"
+        base_url = api.portal.get_registry_record(
+            name="volto.frontend_domain", default=""
+        )
+        base_url = f"{base_url}/prenotazione-appuntamenti-uffici"
         for item in response.get("items") or []:
             item["url"] = f"{base_url}?booking_id={item['booking_id']}"
         return response
```

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/setuphandlers.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/testing.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/testing.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,18 +31,18 @@
         if iocittadino_installed:
             self.loadZCML(package=design.plone.iocittadino)
 
     def setUpPloneSite(self, portal):
         super().setUpPloneSite(portal)
 
         applyProfile(portal, "design.plone.ioprenoto:default")
-        applyProfile(portal, "redturtle.prenotazioni:default")
 
-        # if iocittadino_installed:
-        #     applyProfile(portal, "design.plone.iocittadino:default")
+
+# if iocittadino_installed:
+#     applyProfile(portal, "design.plone.iocittadino:default")
 
 
 DESIGN_PLONE_IOPRENOTO_FIXTURE = DesignPloneIoprenotoLayer()
 
 
 DESIGN_PLONE_IOPRENOTO_INTEGRATION_TESTING = IntegrationTesting(
     bases=(DESIGN_PLONE_IOPRENOTO_FIXTURE,),
```

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/robot/test_example.robot` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_setup.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.9/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py` & `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 from plone import api
 from plone.app.testing import (
     TEST_USER_ID,
     setRoles,
 )
 from design.plone.ioprenoto.testing import DESIGN_PLONE_IOPRENOTO_FUNCTIONAL_TESTING
 from datetime import datetime
+from plone.registry.interfaces import IRegistry
+from plone.stringinterp.interfaces import IStringSubstitution
+from plone.volto.interfaces import IVoltoSettings
 from redturtle.prenotazioni.adapters.booker import IBooker
 from zope.component import getAdapter
-from plone.stringinterp.interfaces import IStringSubstitution
+from zope.component import getUtility
 
 import unittest
 import transaction
 
 
 class TestStringinterpOverrides(unittest.TestCase):
     layer = DESIGN_PLONE_IOPRENOTO_FUNCTIONAL_TESTING
@@ -105,23 +108,35 @@
         )
 
         transaction.commit()
 
     def test_booking_print_url_override(
         self,
     ):
-        self.assertIn(
-            "prenotazione-appuntamenti-uffici",
+        self.assertEqual(
             getAdapter(self.prenotazione, IStringSubstitution, "booking_print_url")(),
+            f"{self.portal_url}/prenotazione-appuntamenti-uffici?booking_id={self.prenotazione.UID()}",
         )
 
     def test_booking_print_url_with_delete_token_override(
         self,
     ):
-        self.assertIn(
-            "prenotazione-appuntamenti-uffici",
+        self.assertEqual(
             getAdapter(
                 self.prenotazione,
                 IStringSubstitution,
                 "booking_print_url_with_delete_token",
             )(),
+            f"{self.portal_url}/prenotazione-appuntamenti-uffici?booking_id={self.prenotazione.UID()}",
+        )
+
+    def test_booking_print_url_override_with_custom_frontend_domain(
+        self,
+    ):
+        registry = getUtility(IRegistry)
+        settings = registry.forInterface(IVoltoSettings, prefix="volto", check=False)
+        settings.frontend_domain = "http://foo.bar"
+
+        self.assertEqual(
+            getAdapter(self.prenotazione, IStringSubstitution, "booking_print_url")(),
+            f"http://foo.bar/prenotazione-appuntamenti-uffici?booking_id={self.prenotazione.UID()}",
         )
```

### Comparing `design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/PKG-INFO` & `design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ioprenoto
-Version: 1.0.9
+Version: 1.1.0
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/design.plone.ioprenoto
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ioprenoto/
 Project-URL: Source, https://github.com/RedTurtle/design.plone.ioprenoto
@@ -177,14 +177,33 @@
         - RedTurtle, info@redturtle.it
         
         
         Changelog
         =========
         
         
+        1.1.0 (2023-06-30)
+        ------------------
+        
+        - Move message to contentrule in iocittadino
+          [mamico]
+        
+        - Handle custom frontend_domain in notification urls (to fix the /admin problem).
+          [cekk]
+        
+        - Fix permission management in PrenotazioniFolder serializer.
+          [cekk]
+        
+        1.0.10 (2023-06-20)
+        -------------------
+        
+        - Fix the prentazione created message.
+          [folix-01]
+        
+        
         1.0.9 (2023-06-19)
         ------------------
         
         - Fix the prentazione link in the message.
           [folix-01]
```

### Comparing `design.plone.ioprenoto-1.0.9/src/design.plone.ioprenoto.egg-info/SOURCES.txt` & `design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 src/design/plone/ioprenoto/events/configure.zcml
 src/design/plone/ioprenoto/events/on_create.py
 src/design/plone/ioprenoto/locales/README.rst
 src/design/plone/ioprenoto/locales/__init__.py
 src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
 src/design/plone/ioprenoto/locales/update.py
 src/design/plone/ioprenoto/locales/update.sh
+src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.mo
 src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
+src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.mo
 src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
 src/design/plone/ioprenoto/profiles/default/browserlayer.xml
 src/design/plone/ioprenoto/profiles/default/catalog.xml
 src/design/plone/ioprenoto/profiles/default/metadata.xml
 src/design/plone/ioprenoto/profiles/default/rolemap.xml
 src/design/plone/ioprenoto/profiles/default/registry/main.xml
 src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
```

