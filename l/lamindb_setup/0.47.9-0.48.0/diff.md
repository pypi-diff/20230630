# Comparing `tmp/lamindb_setup-0.47.9.tar.gz` & `tmp/lamindb_setup-0.48.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.47.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.48.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.47.9.tar` & `lamindb_setup-0.48.0.tar`

### file list

```diff
@@ -1,86 +1,98 @@
--rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.47.9/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.47.9/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.47.9/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.47.9/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.47.9/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.47.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.47.9/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.47.9/README.md
--rw-r--r--   0        0        0    55000 2023-06-16 00:45:51.189658 lamindb_setup-0.47.9/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.47.9/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.47.9/docs/faq/index.md
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.47.9/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.47.9/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.47.9/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4362 2023-06-08 11:34:59.766951 lamindb_setup-0.47.9/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5750 2023-06-08 11:34:59.767059 lamindb_setup-0.47.9/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.47.9/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.47.9/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.47.9/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.47.9/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.47.9/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.47.9/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.47.9/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.47.9/lamin-project.yaml
--rw-r--r--   0        0        0     2715 2023-06-16 00:45:42.214821 lamindb_setup-0.47.9/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.47.9/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.47.9/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.47.9/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.47.9/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.47.9/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.47.9/lamindb_setup/_info.py
--rw-r--r--   0        0        0     6662 2023-06-14 07:51:53.730520 lamindb_setup-0.47.9/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     5670 2023-06-11 19:14:24.008895 lamindb_setup-0.47.9/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0     1118 2023-06-15 00:10:45.075143 lamindb_setup-0.47.9/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.47.9/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.47.9/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.47.9/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1891 2023-06-08 07:33:18.805466 lamindb_setup-0.47.9/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.47.9/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.47.9/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.47.9/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.47.9/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.47.9/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.47.9/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.47.9/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.47.9/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0    10751 2023-06-15 12:55:29.507946 lamindb_setup-0.47.9/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.47.9/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     9359 2023-06-14 07:52:21.048065 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.47.9/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.47.9/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     4812 2023-06-15 12:55:29.508183 lamindb_setup-0.47.9/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.47.9/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      815 2023-06-15 00:10:32.815663 lamindb_setup-0.47.9/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.47.9/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.47.9/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.47.9/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.47.9/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    27342 2023-06-12 19:29:46.148924 lamindb_setup-0.47.9/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.47.9/lnschema-core/LICENSE
--rw-r--r--   0        0        0      308 2023-06-12 10:24:01.839064 lamindb_setup-0.47.9/lnschema-core/README.md
--rw-r--r--   0        0        0      608 2023-06-12 19:29:46.149107 lamindb_setup-0.47.9/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-07 12:14:30.488867 lamindb_setup-0.47.9/lnschema-core/lnschema_core/_lookup.py
--rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.47.9/lnschema-core/lnschema_core/_queryset.py
--rw-r--r--   0        0        0     1644 2023-06-12 19:29:46.149255 lamindb_setup-0.47.9/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    12754 2023-06-12 19:29:46.149559 lamindb_setup-0.47.9/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.47.9/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    20627 2023-06-15 15:27:51.637812 lamindb_setup-0.47.9/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      591 2023-06-12 10:24:01.840710 lamindb_setup-0.47.9/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.47.9/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      184 2023-06-15 00:10:32.816080 lamindb_setup-0.47.9/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      850 2023-06-07 12:14:30.490216 lamindb_setup-0.47.9/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0     1911 2023-06-07 16:31:43.467939 lamindb_setup-0.47.9/noxfile.py
--rw-r--r--   0        0        0     1337 2023-06-15 18:22:44.771393 lamindb_setup-0.47.9/pyproject.toml
--rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.47.9/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.47.9/tests/test_init_instance.py
--rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.47.9/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.47.9/tests/test_login.py
--rw-r--r--   0        0        0      420 2023-06-15 00:10:45.075855 lamindb_setup-0.47.9/tests/test_migrate.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.47.9/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.47.9/tests/test_signup.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.9/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-21 19:39:29.494297 lamindb_setup-0.48.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.48.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.48.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.48.0/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.48.0/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.48.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.48.0/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.48.0/README.md
+-rw-r--r--   0        0        0    56567 2023-06-30 11:13:13.187677 lamindb_setup-0.48.0/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.48.0/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.48.0/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.48.0/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.48.0/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.48.0/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4418 2023-06-20 11:14:24.334197 lamindb_setup-0.48.0/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.48.0/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.48.0/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.48.0/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.48.0/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.48.0/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.48.0/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.48.0/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.48.0/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.48.0/lamin-project.yaml
+-rw-r--r--   0        0        0     2757 2023-06-30 11:13:03.703842 lamindb_setup-0.48.0/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.48.0/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1396 2023-06-29 14:23:25.509218 lamindb_setup-0.48.0/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.48.0/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.48.0/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.48.0/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.48.0/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     6734 2023-06-28 12:29:31.054038 lamindb_setup-0.48.0/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     5946 2023-06-29 14:23:25.509432 lamindb_setup-0.48.0/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0     1118 2023-06-15 00:10:45.075143 lamindb_setup-0.48.0/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.48.0/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.48.0/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.48.0/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.48.0/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.48.0/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.48.0/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.48.0/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.48.0/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.48.0/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.48.0/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.48.0/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.48.0/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0    10748 2023-06-29 15:11:20.989570 lamindb_setup-0.48.0/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.48.0/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     3456 2023-06-18 07:46:49.405332 lamindb_setup-0.48.0/lamindb_setup/dev/_hub_client.py
+-rw-r--r--   0        0        0     9074 2023-06-20 11:14:24.335109 lamindb_setup-0.48.0/lamindb_setup/dev/_hub_core.py
+-rw-r--r--   0        0        0     3310 2023-06-18 07:46:49.405673 lamindb_setup-0.48.0/lamindb_setup/dev/_hub_crud.py
+-rw-r--r--   0        0        0     4129 2023-06-27 14:15:46.405828 lamindb_setup-0.48.0/lamindb_setup/dev/_hub_utils.py
+-rw-r--r--   0        0        0     9365 2023-06-28 12:32:26.045930 lamindb_setup-0.48.0/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.48.0/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.48.0/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.48.0/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.48.0/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.48.0/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.48.0/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4812 2023-06-15 12:55:29.508183 lamindb_setup-0.48.0/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.48.0/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.48.0/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.48.0/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.48.0/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.48.0/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.48.0/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    29416 2023-06-29 19:17:30.194449 lamindb_setup-0.48.0/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.48.0/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.48.0/lnschema-core/README.md
+-rw-r--r--   0        0        0      617 2023-06-29 19:17:30.195331 lamindb_setup-0.48.0/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.48.0/lnschema-core/lnschema_core/_queryset.py
+-rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.48.0/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.48.0/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.48.0/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
+-rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.48.0/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
+-rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.48.0/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
+-rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.48.0/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
+-rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.48.0/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.48.0/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    23909 2023-06-29 19:17:30.196117 lamindb_setup-0.48.0/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      951 2023-06-29 19:17:30.196374 lamindb_setup-0.48.0/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.48.0/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.48.0/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.48.0/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.48.0/lnschema-core/tests/test_integrity.py
+-rw-r--r--   0        0        0     1821 2023-06-27 14:15:46.405994 lamindb_setup-0.48.0/noxfile.py
+-rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.48.0/pyproject.toml
+-rw-r--r--   0        0        0     1169 2023-06-27 14:15:46.406331 lamindb_setup-0.48.0/tests/hub/test_instance.py
+-rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.48.0/tests/hub/test_signup_signin.py
+-rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.48.0/tests/hub/test_storage.py
+-rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.48.0/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-19 15:23:54.026893 lamindb_setup-0.48.0/tests/test_init_instance.py
+-rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.48.0/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.48.0/tests/test_login.py
+-rw-r--r--   0        0        0      420 2023-06-15 00:10:45.075855 lamindb_setup-0.48.0/tests/test_migrate.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.48.0/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.48.0/tests/test_signup.py
+-rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.48.0/PKG-INFO
```

### Comparing `lamindb_setup-0.47.9/.github/workflows/build.yml` & `lamindb_setup-0.48.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/.github/workflows/latest-changes.yml` & `lamindb_setup-0.48.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/.gitignore` & `lamindb_setup-0.48.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/.pre-commit-config.yaml` & `lamindb_setup-0.48.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/LICENSE` & `lamindb_setup-0.48.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/docs/changelog.md` & `lamindb_setup-0.48.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Fix sqlite file not existing in the bucket error | [432](https://github.com/laminlabs/lamindb-setup/pull/432) | [Koncopd](https://github.com/Koncopd) | 2023-06-28 | 0.48.0
+🩹 Do not register storage through `set.storage` on the hub | [430](https://github.com/laminlabs/lamindb-setup/pull/430) | [falexwolf](https://github.com/falexwolf) | 2023-06-28 |
+🐛 Lock cloud sqlite instances on init | [429](https://github.com/laminlabs/lamindb-setup/pull/429) | [Koncopd](https://github.com/Koncopd) | 2023-06-27 |
+👷 Add local hub tests | [427](https://github.com/laminlabs/lamindb-setup/pull/427) | [falexwolf](https://github.com/falexwolf) | 2023-06-26 |
+✨ Set s3 region in set.storage | [428](https://github.com/laminlabs/lamindb-setup/pull/428) | [Koncopd](https://github.com/Koncopd) | 2023-06-26 |
+➖ Simplify deps | [426](https://github.com/laminlabs/lamindb-setup/pull/426) | [falexwolf](https://github.com/falexwolf) | 2023-06-21 |
+✅ Try to trigger error | [424](https://github.com/laminlabs/lamindb-setup/pull/424) | [falexwolf](https://github.com/falexwolf) | 2023-06-20 | 0.47.11
+🔧 Back to UTC | [423](https://github.com/laminlabs/lamindb-setup/pull/423) | [falexwolf](https://github.com/falexwolf) | 2023-06-20 |
+♻️ Simplify schema validation | [422](https://github.com/laminlabs/lamindb-setup/pull/422) | [falexwolf](https://github.com/falexwolf) | 2023-06-18 | 0.47.10
+🎨  Remove `lnhub_rest` from `lamindb_setup` | [421](https://github.com/laminlabs/lamindb-setup/pull/421) | [bpenteado](https://github.com/bpenteado) | 2023-06-16 |
 🍱 Fix legacy data migration | [420](https://github.com/laminlabs/lamindb-setup/pull/420) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.47.9
 ✨ Add ability to check for migrations | [419](https://github.com/laminlabs/lamindb-setup/pull/419) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.47.8
 🎨 Updated bionty function imports | [418](https://github.com/laminlabs/lamindb-setup/pull/418) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-14 |
 ♻️ Different migr strategy | [417](https://github.com/laminlabs/lamindb-setup/pull/417) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.7
 🍱 Added migration script from legacy instances | [416](https://github.com/laminlabs/lamindb-setup/pull/416) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.5
 🔥 Adapt locker to lock entire lamindb session | [415](https://github.com/laminlabs/lamindb-setup/pull/415) | [Koncopd](https://github.com/Koncopd) | 2023-06-11 |
 🚑 Only delete bionty sources when bionty is installed | [414](https://github.com/laminlabs/lamindb-setup/pull/414) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.4
```

### Comparing `lamindb_setup-0.47.9/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.48.0/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.48.0/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.48.0/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.48.0/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.48.0/docs/guide/02-load-instance.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984722222222222%*

 * *Differences: {"'cells'": "{10: {'source': ['If there is a typo, or you get the account wrong, an error will be "*

 * *            "raised:']}, 11: {'source': ['import pytest\\n', '\\n', 'with "*

 * *            'pytest.raises(RuntimeError):\\n\', \'    ln_setup.load("testuser2/mydata")\']}}'}*

```diff
@@ -131,25 +131,28 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "0986a5f3",
             "metadata": {},
             "source": [
-                "If there is a typo, or you get the account wrong, you'll see:"
+                "If there is a typo, or you get the account wrong, an error will be raised:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bc3568ae",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln_setup.load(\"testuser2/mydata\") == \"instance-not-reachable\""
+                "import pytest\n",
+                "\n",
+                "with pytest.raises(RuntimeError):\n",
+                "    ln_setup.load(\"testuser2/mydata\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "e3701120",
             "metadata": {},
```

### Comparing `lamindb_setup-0.47.9/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.48.0/docs/guide/03-set-storage.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9889172335600906%*

 * *Differences: {"'cells'": "{0: {delete: ['attachments']}, 3: {delete: ['attachments']}, 7: {delete: "*

 * *            "['attachments']}, 11: {delete: ['attachments']}, 14: {delete: ['attachments']}, 15: "*

 * *            "{'source': {insert: [(2, 'assert ln_setup.settings.storage.region == "*

 * *            '"us-east-1"\\n\')]}}, 16: {delete: [\'attachments\']}, 19: {delete: '*

 * *            "['attachments']}, 20: {delete: ['attachments']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.12'}}"}*

```diff
@@ -1,11 +1,10 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "# Set storage"
@@ -33,15 +32,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import lamindb_setup as ln_setup"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "a7cf42fb",
             "metadata": {},
             "source": [
                 "## Set storage"
             ]
         },
@@ -79,15 +77,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln_setup.settings.storage.root"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "e6638f44",
             "metadata": {},
             "source": [
                 "Local storage:"
             ]
         },
@@ -124,15 +121,14 @@
             "source": [
                 "from pathlib import Path\n",
                 "\n",
                 "assert ln_setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_2\""
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "de1c12b8",
             "metadata": {},
             "source": [
                 "Cloud storage:"
             ]
         },
@@ -153,15 +149,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln_setup.settings.storage.root"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "859a972e",
             "metadata": {},
             "source": [
                 "See an overview:"
             ]
         },
@@ -174,22 +169,22 @@
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "assert ln_setup.settings.storage.is_cloud\n",
                 "assert ln_setup.settings.storage.root_as_str == \"s3://lndb-setup-ci\"\n",
+                "assert ln_setup.settings.storage.region == \"us-east-1\"\n",
                 "# root.fs contains the underlying fsspec filesystem\n",
                 "assert (\n",
                 "    ln_setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by default\n",
                 ")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "ae953b6a",
             "metadata": {},
             "source": [
                 "You can set any additional `fsspec` filesystem arguments for cloud storage, such as `profile` or `cache_regions` (for s3 only), for example:"
             ]
         },
@@ -222,26 +217,24 @@
                 ")\n",
                 "ln_setup.set.storage(\"./storage_3\")\n",
                 "assert ln_setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_3\"\n",
                 "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "3fb6a223",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "### Currently not possible: setting storage for SQLite instance"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "6ccb6573",
             "metadata": {},
             "source": [
                 "If you try to set the storage for an sqlite instance, an error message is returned:\n",
                 "```\n",
                 "assert ln_setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\"\n",
@@ -261,15 +254,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.12"
         },
         "vscode": {
             "interpreter": {
                 "hash": "61b4062b24dfb1010f420dad5aa3bd73a4d2af47d0ec44eafec465a35a9d7239"
             }
         }
     },
```

### Comparing `lamindb_setup-0.47.9/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.48.0/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/docs/guide/setup-user.md` & `lamindb_setup-0.48.0/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/__init__.py` & `lamindb_setup-0.48.0/lamindb_setup/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.47.9"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.48.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
@@ -68,14 +68,15 @@
 from ._migrate import migrate
 from ._register_instance import register  # noqa
 from ._schema import schema  # noqa
 from ._set import set, set_storage  # noqa
 from ._settings import settings  # noqa
 from ._setup_user import login, signup  # noqa
 
+_TESTING = False  # used in lamindb tests
 
 # unlock and clear on uncaught exception
 def _clear_on_exception():
     from .dev._cloud_sqlite_locker import _locker
 
     if _locker is not None:
         try:
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/__main__.py` & `lamindb_setup-0.48.0/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.48.0/lamindb_setup/_check_instance_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,11 +30,11 @@
                 "Current instance cannot be reached, close it: `lamin close`\n"
                 "Alternatively, init or load a connectable instance on the"
                 " command line: `lamin load <instance>` or `lamin init <...>`"
             )
     else:
         if from_lamindb:
             logger.warning(
-                "You haven't yet setup an instance using the CLI: Please call"
+                "You haven't yet setup an instance: Please call"
                 " `ln.setup.init()` or `ln.setup.load()`"
             )
         return False
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_close.py` & `lamindb_setup-0.48.0/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_delete.py` & `lamindb_setup-0.48.0/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_docstrings.py` & `lamindb_setup-0.48.0/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_init_instance.py` & `lamindb_setup-0.48.0/lamindb_setup/_init_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from lamindb_setup.dev.upath import UPath
 
 from ._docstrings import instance_description as description
 from ._settings import settings
 from .dev import InstanceSettings
 from .dev._docs import doc_args
-from .dev._setup_schema import load_schema
+from .dev._setup_schema import get_schema_module_name, load_schema
 from .dev._storage import Storage
 
 
 def register_user_and_storage(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
     from django.db.utils import OperationalError
     from lnschema_core.models import Storage, User
@@ -44,16 +44,14 @@
         if created:
             logger.success(f"Saved: {storage}")
     except OperationalError as error:
         logger.warning(f"Instance seems not set up ({error})")
 
 
 def reload_schema_modules(isettings: InstanceSettings):
-    from lnhub_rest._assets._schemas import get_schema_module_name
-
     schema_names = ["core"] + list(isettings.schema)
     schema_module_names = [get_schema_module_name(n) for n in schema_names]
 
     for schema_module_name in schema_module_names:
         if schema_module_name in sys.modules:
             schema_module = importlib.import_module(schema_module_name)
             importlib.reload(schema_module)
@@ -97,29 +95,24 @@
     Args:
         storage: {}
         name: {}
         db: {}
         schema: {}
     """
     # clean up in next refactor
-    from lnhub_rest.core.instance._init_instance import (
-        init_instance as init_instance_hub,
-    )
-    from lnhub_rest.core.instance._init_instance import (
+    # avoid circular import
+    from ._load_instance import load
+    from .dev._hub_core import init_instance as init_instance_hub
+    from .dev._hub_utils import (
+        get_storage_region,
         validate_db_arg,
         validate_schema_arg,
-    )
-    from lnhub_rest.core.storage._add_storage import (
-        get_storage_region,
         validate_storage_root_arg,
     )
 
-    # avoid circular import
-    from ._load_instance import load
-
     assert settings.user.id  # check user is logged in
     owner = settings.user.handle
 
     schema = validate_schema_arg(schema)
     validate_storage_root_arg(str(storage))
     validate_db_arg(db)
 
@@ -129,15 +122,15 @@
     if response is None:
         return None  # successful load!
 
     isettings = InstanceSettings(
         owner=owner,
         name=name_str,
         storage_root=storage,
-        storage_region=get_storage_region(storage),
+        storage_region=get_storage_region(storage),  # type: ignore
         db=db,
         schema=schema,
     )
 
     if isettings._is_cloud_sqlite:
         if (
             not isettings._sqlite_file.exists()
@@ -172,20 +165,27 @@
     if isettings._is_db_setup(mute=True)[0]:
         raise RuntimeError(
             "Your instance DB is already set up but couldn't be loaded, something"
             " is off"
         )
     load_from_isettings(isettings, init=True)
     if isettings._is_cloud_sqlite:
-        logger.hint("To push changes to the cloud SQLite file, call: lamin close")
+        isettings._cloud_sqlite_locker.lock()
+        logger.warning(
+            "Locked the instance. To unlock and push changes to the cloud SQLite file,"
+            " call: lamin close"
+        )
     if not isettings.is_remote:
+        verbosity = logger._verbosity
+        logger.set_verbosity(3)
         logger.hint(
             "Did not register local instance on hub (if you want to, call `lamin"
             " register`)"
         )
+        logger.set_verbosity(verbosity)
     return None
 
 
 def load_from_isettings(
     isettings: InstanceSettings,
     *,
     init: bool = False,
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_load_instance.py` & `lamindb_setup-0.48.0/lamindb_setup/_load_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,56 +27,60 @@
         identifier: `str` - The instance identifier can the instance name (owner is
             current user), handle/name, or the URL: https://lamin.ai/handle/name.
         storage: `Optional[PathLike] = None` - Load the instance with an
             updated default storage.
     """
     owner, name = get_owner_name_from_identifier(identifier)
 
-    from lnhub_rest.core.instance._load_instance import (
-        load_instance as load_instance_from_hub,
-    )
+    from .dev._hub_core import load_instance as load_instance_from_hub
 
     hub_result = load_instance_from_hub(
         owner=owner, name=name, _access_token=_access_token
     )
     # if hub_result is not a string, it means it made a request
     # that successfully returned metadata
     if not isinstance(hub_result, str):
         instance_result, storage_result = hub_result
         isettings = InstanceSettings(
             owner=owner,
             name=name,
-            storage_root=storage_result.root,
-            storage_region=storage_result.region,
-            db=instance_result.db,
-            schema=instance_result.schema_str,
+            storage_root=storage_result["root"],
+            storage_region=storage_result["region"],
+            db=instance_result["db"],
+            schema=instance_result["schema_str"],
         )
     else:
         settings_file = instance_settings_file(name, owner)
         if settings_file.exists():
             logger.info(f"Found cached instance metadata: {settings_file}")
             isettings = load_instance_settings(settings_file)
         else:
             if _log_error_message:
-                logger.error(
+                raise RuntimeError(
                     f"Instance {owner}/{name} neither loadable from hub nor local"
                     " cache. Check whether instance exists and you have access:"
                     f" https://lamin.ai/{owner}/{name}?tab=collaborators"
                 )
             return "instance-not-reachable"
 
     if storage is not None:
         update_isettings_with_storage(isettings, storage)
     if _test:
         isettings._persist()  # this is to test the settings
         return None
 
     check, msg = isettings._is_db_setup()  # this also updates local SQLite
     if not check:
-        if _log_error_message:
+        local_db = isettings._is_cloud_sqlite and isettings._sqlite_file_local.exists()
+        if local_db:
+            logger.warning(
+                "SQLite file does not exist in the cloud, but exists locally. To push"
+                " the file to the cloud, call: lamin close"
+            )
+        elif _log_error_message:
             raise RuntimeError(msg)
         else:
             logger.warning(
                 "Instance metadata exists, but DB might have been corrupted or deleted."
                 " Re-initializing the DB."
             )
             return "instance-not-reachable"
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_migrate.py` & `lamindb_setup-0.48.0/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_notebook.py` & `lamindb_setup-0.48.0/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_register_instance.py` & `lamindb_setup-0.48.0/lamindb_setup/_register_instance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from lamin_logger import logger
 
 from ._settings import settings
 
 
 def register():
     """Register an instance on the hub."""
-    from lnhub_rest.core.instance._init_instance import (
-        init_instance as init_instance_hub,
-    )
+    from .dev._hub_core import init_instance as init_instance_hub
 
     isettings = settings.instance
     result = init_instance_hub(
         owner=isettings.owner,
         name=isettings.name,
         storage=isettings.storage.root_as_str,
         db=isettings.db if isettings.dialect != "sqlite" else None,
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_schema.py` & `lamindb_setup-0.48.0/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_set.py` & `lamindb_setup-0.48.0/lamindb_setup/_set.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,32 +26,37 @@
 
         >>> ln.setup.set.storage(
         >>>    "s3://some-bucket",
         >>>     profile="some_profile", # fsspec arg
         >>>     cache_regions=True # fsspec arg for s3
         >>> )
         """
-        from lnhub_rest.core.storage._add_storage import add_storage as add_storage_hub
+        from .dev._hub_utils import get_storage_region
 
         if settings.instance.dialect == "sqlite":
             logger.error("Can't set storage for sqlite instances.")
             return "set-storage-failed"
 
         new_isettings = InstanceSettings(
             owner=settings.instance.owner,
             name=settings.instance.name,
             storage_root=root,
+            storage_region=get_storage_region(root),
             db=settings.instance.db,
             schema=settings.instance._schema_str,
         )
 
         new_isettings._persist()  # this also updates the settings object
         register_user_and_storage(new_isettings, settings.user)
-        if settings.instance.is_remote:
-            add_storage_hub(root, account_handle=settings.instance.owner)
+        # we are not doing this for now because of difficulties to define the right RLS policy  # noqa
+        # https://laminlabs.slack.com/archives/C04FPE8V01W/p1687948324601929?thread_ts=1687531921.394119&cid=C04FPE8V01W
+        # if settings.instance.is_remote:
+        #     add_storage_hub(
+        #         root, account_handle=settings.instance.owner  # type: ignore
+        #     )
 
         settings.storage._set_fs_kwargs(**fs_kwargs)
 
         logger.success(f"Set storage {root}")
 
 
 @deprecated("lamindb_setup.set.storage()")
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_settings.py` & `lamindb_setup-0.48.0/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_setup_user.py` & `lamindb_setup-0.48.0/lamindb_setup/_setup_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .dev._settings_load import load_or_create_user_settings, load_user_settings
 from .dev._settings_save import save_user_settings
 from .dev._settings_store import user_settings_file_email, user_settings_file_handle
 
 
 def signup(email: str) -> Union[str, None]:
     """Sign up user."""
-    from lnhub_rest.core.account._signup_signin import sign_up_hub
+    from .dev._hub_core import sign_up_hub
 
     response = sign_up_hub(email)
     if response == "handle-exists":  # handle already exists
         logger.error("The handle already exists. Please choose a different one.")
         return "handle-exists"
     if response == "user-exists":  # user already exists
         logger.error("User already exists! Please login instead: `lamin login`.")
@@ -76,15 +76,15 @@
 
     if user_settings.password is None:
         raise RuntimeError(
             "No stored user password, please call: lamin login <your-email>"
             " --password <your-password>"
         )
 
-    from lnhub_rest.core.account._signup_signin import sign_in_hub
+    from .dev._hub_core import sign_in_hub
 
     response = sign_in_hub(
         user_settings.email, user_settings.password, user_settings.handle
     )
     if response == "could-not-login":
         return response
     elif response == "complete-signup":
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.48.0/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_django.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_django.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,24 +164,26 @@
         default=isettings.db,
         conn_max_age=600,
         conn_health_checks=True,
     )
     DATABASES = {
         "default": default_db,
     }
-    from lnhub_rest._assets._schemas import get_schema_module_name
+    from ._setup_schema import get_schema_module_name
 
     schema_names = ["core"] + list(isettings.schema)
     schema_module_names = [get_schema_module_name(n) for n in schema_names]
 
     if not settings.configured:
         settings.configure(
             INSTALLED_APPS=schema_module_names,
             DATABASES=DATABASES,
             DEFAULT_AUTO_FIELD="django.db.models.BigAutoField",
+            TIME_ZONE="UTC",
+            USE_TZ=True,
         )
         django.setup(set_prefix=False)
 
         if create_migrations:
             call_command("makemigrations")
             return None
 
@@ -198,19 +200,18 @@
                     # no need to update the remote sqlite
                     isettings._update_cloud_sqlite_file()
             else:
                 logger.warning(
                     "\n\nYour database is not up to date with your installed"
                     " schemas!\n\nIt misses the following"
                     f" migrations:\n{planned_migrations}\n\nIf you are an admin and"
-                    " know what you're doing, deploy the migration:\nlamin migrate"
-                    " deploy\n\nOtherwise, please install previouses release of the"
-                    " above-mentioned schemas\n\nIn case you haven't yet migrated to"
-                    " Django, please upgrade to lamindb 0.41.2 before deploying this"
-                    " migration - you'll need a manual step then, please reach out to"
-                    " Lamin\n"
+                    " know what you're doing, deploy the migration: lamin migrate"
+                    " deploy\n\nOtherwise, please install an earlier version of  your"
+                    " custom schema module\n\nIn case you haven't yet migrated to"
+                    " Django, please FIRST upgrade to lamindb 0.41.2 before deploying"
+                    " this migration and consider reaching out to Lamin\n"
                 )
         else:
             if deploy_migrations:
                 logger.info("Database already up-to-date with migrations!")
         global IS_SETUP
         IS_SETUP = True
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_settings_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,28 +96,28 @@
     def _sqlite_file_local(self) -> Path:
         """Local SQLite file."""
         return self.storage.cloud_to_local_no_update(self._sqlite_file)
 
     def _update_cloud_sqlite_file(self) -> None:
         """Upload the local sqlite file to the cloud file."""
         if self._is_cloud_sqlite:
-            logger.info("Updating & unlocking cloud SQLite")
+            logger.warning("Updating & unlocking cloud SQLite")
             sqlite_file = self._sqlite_file
             cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
             sqlite_file.upload_from(cache_file)  # type: ignore
             cloud_mtime = sqlite_file.modified.timestamp()  # type: ignore
             # this seems to work even if there is an open connection
             # to the cache file
             os.utime(cache_file, times=(cloud_mtime, cloud_mtime))
             self._cloud_sqlite_locker.unlock()
 
     def _update_local_sqlite_file(self) -> None:
         """Download the cloud sqlite file if it is newer than local."""
         if self._is_cloud_sqlite:
-            logger.info(
+            logger.warning(
                 "Updating local SQLite & locking cloud SQLite (sync back & unlock:"
                 " lamin close)"
             )
             sqlite_file = self._sqlite_file
             cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
             sqlite_file.synchronize(cache_file)  # type: ignore
             self._cloud_sqlite_locker.lock()
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_setup_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import importlib
 from types import ModuleType
 
 from importlib_metadata import requires as importlib_requires
 from importlib_metadata import version as get_pip_version
 from lamin_logger import logger
-from lnhub_rest._assets._schemas import get_schema_module_name
 from packaging.requirements import Requirement
 
 from ._django import setup_django
 from ._settings_instance import InstanceSettings
 
 
+def get_schema_module_name(schema_name):
+    return f"lnschema_{schema_name.replace('-', '_')}"
+
+
 def check_schema_version_and_import(schema_name) -> ModuleType:
     lamindb_installed = True
     try:
         get_pip_version("lamindb")  # noqa
     except Exception:
         lamindb_installed = False
```

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lamindb_setup/dev/upath.py` & `lamindb_setup-0.48.0/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.48.0/lnschema-core/.github/workflows/build.yml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
 jobs:
-  lint:
+  build:
     runs-on: ubuntu-latest
     env:
       GITHUB_EVENT_NAME: ${{ github.event_name }}
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9"]
@@ -27,7 +27,8 @@
       - name: cache pre-commit
         uses: actions/cache@v3
         with:
           path: ~/.cache/pre-commit
           key: pre-commit-${{ runner.os }}-${{ hashFiles('.pre-commit-config.yaml') }}
       - run: pip install -U laminci
       - run: nox -s lint
+      - run: nox -s test
```

### Comparing `lamindb_setup-0.47.9/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.48.0/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lnschema-core/.gitignore` & `lamindb_setup-0.48.0/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.48.0/lnschema-core/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
       - id: flake8
         additional_dependencies:
           - flake8-black==0.3.3
           - flake8-typing-imports==1.10.0
         language_version: python3
         args:
           - --max-line-length=176
-          - --ignore=E203,BLK100,W503
+          - --ignore=E203,BLK100,W503,TYP001
         exclude: |
           (?x)(
               __init__.py
           )
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v2.6.2
     hooks:
```

### Comparing `lamindb_setup-0.47.9/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.48.0/lnschema-core/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚚 Rename `BaseORM` to `ORM`, move `ORM` signatures here | [213](https://github.com/laminlabs/lnschema-core/pull/213) | [falexwolf](https://github.com/falexwolf) | 2023-06-29 |
+✨ Add `Dataset` & `Feature` ORMs | [212](https://github.com/laminlabs/lnschema-core/pull/212) | [falexwolf](https://github.com/falexwolf) | 2023-06-29 | 0.37a1
+💄 Denoise display of timestamps | [211](https://github.com/laminlabs/lnschema-core/pull/211) | [falexwolf](https://github.com/falexwolf) | 2023-06-26 |
+🎨 Auto-manage `RunInput` relationship | [210](https://github.com/laminlabs/lnschema-core/pull/210) | [falexwolf](https://github.com/falexwolf) | 2023-06-26 | 0.36.1
+🚚 Repurpose `Folder` to `Tag` | [209](https://github.com/laminlabs/lnschema-core/pull/209) | [falexwolf](https://github.com/falexwolf) | 2023-06-22 | 0.36.0
+🚚 Move `BaseORM.__init__` to lamindb | [208](https://github.com/laminlabs/lnschema-core/pull/208) | [falexwolf](https://github.com/falexwolf) | 2023-06-19 | 0.35.10
+🚚 Expand field length `short_name` in transform | [207](https://github.com/laminlabs/lnschema-core/pull/207) | [falexwolf](https://github.com/falexwolf) | 2023-06-19 |
+🔥 Remove `Lookup` | [206](https://github.com/laminlabs/lnschema-core/pull/206) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.35.9
+🚚 Move methods to lamindb | [205](https://github.com/laminlabs/lnschema-core/pull/205) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.35.8
+🚚 Make `User.name` nullable | [204](https://github.com/laminlabs/lnschema-core/pull/204) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 |
+🔥 Remove unnecessary file | [203](https://github.com/laminlabs/lnschema-core/pull/203) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 |
+✅ Add migrations check | [202](https://github.com/laminlabs/lnschema-core/pull/202) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 |
+♻️ Alter SA migration strategy | [200](https://github.com/laminlabs/lnschema-core/pull/200) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.35.7
 🍱 Add migration process for legacy SA instances | [199](https://github.com/laminlabs/lnschema-core/pull/199) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.35.5
 ♻️ Less customized IDs | [198](https://github.com/laminlabs/lnschema-core/pull/198) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 |
 ♻️ Move logic to lamindb | [197](https://github.com/laminlabs/lnschema-core/pull/197) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 |
 ✨ Delete storage in File.delete | [196](https://github.com/laminlabs/lnschema-core/pull/196) | [Koncopd](https://github.com/Koncopd) | 2023-06-12 |
 🚚 Rename Featureset to FeatureSet | [194](https://github.com/laminlabs/lnschema-core/pull/194) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.35.4
 ♻️ Move save logic here | [193](https://github.com/laminlabs/lnschema-core/pull/193) | [falexwolf](https://github.com/falexwolf) | 2023-06-10 | 0.35.3
 🔥 Remove unnecessary files | [192](https://github.com/laminlabs/lnschema-core/pull/192) | [falexwolf](https://github.com/falexwolf) | 2023-06-09 | 0.35.2
```

### Comparing `lamindb_setup-0.47.9/lnschema-core/LICENSE` & `lamindb_setup-0.48.0/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.48.0/lnschema-core/lnschema_core/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Data objects & lineage (`yvzi`)."""
 _schema_id = "yvzi"
 _name = "core"
-__version__ = "0.35.5"
+__version__ = "0.37a1"
 
 # can directly import from lamindb_setup going forward
 from lamindb_setup._check_instance_setup import (
     check_instance_setup as _check_instance_setup,
 )
 
 _INSTANCE_SETUP = _check_instance_setup()
 
 if _INSTANCE_SETUP:
     from . import ids, types
     from .models import (  # type: ignore
-        BaseORM,
+        ORM,
+        Dataset,
+        Feature,
         FeatureSet,
         File,
-        Folder,
         Project,
         Run,
-        RunInput,
         Storage,
+        Tag,
         Transform,
         User,
     )
 
     Features = FeatureSet  # backward compat
```

### Comparing `lamindb_setup-0.47.9/lnschema-core/lnschema_core/_queryset.py` & `lamindb_setup-0.48.0/lnschema-core/lnschema_core/_queryset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.48.0/lnschema-core/lnschema_core/ids.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 """IDs.
 
-See: https://github.com/laminlabs/lamin-notes/blob/main/docs/2022/ids.ipynb
-
 Base generators:
 
 .. autosummary::
    :toctree: .
 
    base26
    base62
-   Base62
    base64
 
-For example, 8 base62 characters:
+8 base62 characters:
 
 ======= ===========
-n_rows  p_collision
+n       p_collision
 ======= ===========
 100k    2e-05
 1M      2e-03
 ======= ===========
 
-20 base62 characters (62**20=7e+35) roughly matches UUID (2*122=5e+36).
+12 base62 characters:
+
+======= ===========
+n       p_collision
+======= ===========
+100M    2e-06
+1B      2e-04
+======= ===========
+
+20 base62 characters (62**20=7e+35) roughly matches UUID (2*122=5e+36):
+
+======= ===========
+n       p_collision
+======= ===========
+3e15    1e-6
+======= ===========
+
 """
-# Some IDs got updated on 2023-02-14 to be multiples of 4
-# for matching byte representation, should we ever go there.
 import secrets
 import string
 
 
 def base64(n_char: int) -> str:
-    """Like nanoid."""
+    """Random Base64 string."""
     alphabet = string.digits + string.ascii_letters.swapcase() + "_" + "-"
     id = "".join(secrets.choice(alphabet) for i in range(n_char))
     return id
 
 
 def base62(n_char: int) -> str:
-    """Like nanoid without hyphen and underscore."""
+    """Random Base62 string."""
     alphabet = string.digits + string.ascii_letters.swapcase()
     id = "".join(secrets.choice(alphabet) for i in range(n_char))
     return id
 
 
-# this cannot be serialized by Django,
-# hence, see below
-class Base62:
-    def __init__(self, n_char: int):
-        self.n_char = n_char
+# the following cannot be serialized by Django
+# class Base62:
+#     def __init__(self, n_char: int):
+#         self.n_char = n_char
 
-    def __call__(self):
-        return base62(self.n_char)
+#     def __call__(self):
+#         return base62(self.n_char)
 
 
 def base26(n_char: int):
     """ASCII lowercase."""
     alphabet = string.ascii_lowercase
     id = "".join(secrets.choice(alphabet) for i in range(n_char))
     return id
```

### Comparing `lamindb_setup-0.47.9/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.48.0/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 import lnschema_core.ids
 import lnschema_core.types
 import lnschema_core.users
 
-MANAGED = True
-
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies: List[str] = []
 
     operations = [
@@ -26,57 +24,45 @@
                 ("suffix", models.CharField(db_index=True, default=None, max_length=30, null=True)),
                 ("size", models.BigIntegerField(db_index=True, null=True)),
                 ("hash", models.CharField(db_index=True, default=None, max_length=86, null=True)),
                 ("key", models.CharField(db_index=True, default=None, max_length=255, null=True)),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
             ],
-            options={
-                "managed": MANAGED,
-            },
         ),
         migrations.CreateModel(
             name="Folder",
             fields=[
                 ("id", models.CharField(max_length=20, primary_key=True, serialize=False)),
                 ("name", models.CharField(db_index=True, default=None, max_length=255)),
                 ("key", models.CharField(db_index=True, default=None, max_length=255, null=True)),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
             ],
-            options={
-                "managed": MANAGED,
-            },
         ),
         migrations.CreateModel(
             name="Run",
             fields=[
                 ("id", models.CharField(default=lnschema_core.ids.base62_20, max_length=20, primary_key=True, serialize=False)),
                 ("name", models.CharField(db_index=True, default=None, max_length=255, null=True)),
                 ("external_id", models.CharField(db_index=True, default=None, max_length=255, null=True)),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("run_at", models.DateTimeField(auto_now_add=True, db_index=True)),
             ],
-            options={
-                "managed": MANAGED,
-            },
         ),
         migrations.CreateModel(
             name="User",
             fields=[
                 ("id", models.CharField(default=None, max_length=8, primary_key=True, serialize=False)),
                 ("handle", models.CharField(db_index=True, default=None, max_length=30, unique=True)),
                 ("email", models.CharField(db_index=True, default=None, max_length=255, unique=True)),
                 ("name", models.CharField(db_index=True, max_length=255)),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
             ],
-            options={
-                "managed": MANAGED,
-            },
         ),
         migrations.CreateModel(
             name="Transform",
             fields=[
                 ("id", models.CharField(db_index=True, default=None, max_length=14, primary_key=True, serialize=False)),
                 ("name", models.CharField(db_index=True, default=None, max_length=255, null=True)),
                 ("short_name", models.CharField(db_index=True, default=None, max_length=30, null=True)),
@@ -98,15 +84,14 @@
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id, on_delete=django.db.models.deletion.PROTECT, related_name="created_transforms", to="lnschema_core.user"
                     ),
                 ),
             ],
             options={
-                "managed": MANAGED,
                 "unique_together": {("stem_id", "version")},
             },
         ),
         migrations.CreateModel(
             name="Storage",
             fields=[
                 ("id", models.CharField(db_index=True, default=lnschema_core.ids.base62_8, max_length=8, primary_key=True, serialize=False)),
@@ -118,27 +103,23 @@
                 (
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id, on_delete=django.db.models.deletion.PROTECT, related_name="created_storages", to="lnschema_core.user"
                     ),
                 ),
             ],
-            options={
-                "managed": MANAGED,
-            },
         ),
         migrations.CreateModel(
             name="RunInput",
             fields=[
                 ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
                 ("file", models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to="lnschema_core.file")),
                 ("run", models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to="lnschema_core.run")),
             ],
             options={
-                "managed": MANAGED,
                 "unique_together": {("run", "file")},
             },
         ),
         migrations.AddField(
             model_name="run",
             name="created_by",
             field=models.ForeignKey(
@@ -168,17 +149,14 @@
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id, on_delete=django.db.models.deletion.PROTECT, related_name="created_projects", to="lnschema_core.user"
                     ),
                 ),
                 ("files", models.ManyToManyField(related_name="projects", to="lnschema_core.file")),
                 ("folders", models.ManyToManyField(related_name="projects", to="lnschema_core.folder")),
             ],
-            options={
-                "managed": MANAGED,
-            },
         ),
         migrations.AddField(
             model_name="folder",
             name="created_by",
             field=models.ForeignKey(
                 default=lnschema_core.users.current_user_id, on_delete=django.db.models.deletion.PROTECT, related_name="created_folders", to="lnschema_core.user"
             ),
@@ -226,61 +204,17 @@
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id, on_delete=django.db.models.deletion.PROTECT, related_name="created_featuresets", to="lnschema_core.user"
                     ),
                 ),
                 ("files", models.ManyToManyField(related_name="featuresets", to="lnschema_core.file")),
             ],
-            options={
-                "managed": MANAGED,
-            },
         ),
         migrations.AlterUniqueTogether(
             name="folder",
             unique_together={("storage", "key")},
         ),
         migrations.AlterUniqueTogether(
             name="file",
             unique_together={("storage", "key")},
         ),
     ]
-
-
-if not MANAGED:
-    Migration.operations += [
-        migrations.AlterModelOptions(
-            name="featureset",
-            options={"managed": True},
-        ),
-        migrations.AlterModelOptions(
-            name="file",
-            options={"managed": True},
-        ),
-        migrations.AlterModelOptions(
-            name="folder",
-            options={"managed": True},
-        ),
-        migrations.AlterModelOptions(
-            name="project",
-            options={"managed": True},
-        ),
-        migrations.AlterModelOptions(
-            name="run",
-            options={"managed": True},
-        ),
-        migrations.AlterModelOptions(
-            name="runinput",
-            options={"managed": True},
-        ),
-        migrations.AlterModelOptions(
-            name="storage",
-            options={"managed": True},
-        ),
-        migrations.AlterModelOptions(
-            name="transform",
-            options={"managed": True},
-        ),
-        migrations.AlterModelOptions(
-            name="user",
-            options={"managed": True},
-        ),
-    ]
```

### Comparing `lamindb_setup-0.47.9/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.48.0/lnschema-core/lnschema_core/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,196 +1,371 @@
 import builtins
-import traceback
-from pathlib import Path
-from typing import Dict, Iterable, NamedTuple, Optional, Union, overload  # noqa
+from typing import (  # noqa
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Iterable,
+    List,
+    Literal,
+    NamedTuple,
+    Optional,
+    Union,
+    overload,
+)
 
 from django.db import models
-from django.db.models import PROTECT, Manager
-from lamin_logger import colors, logger
-from upath import UPath
+from django.db.models import PROTECT, CharField, Manager, TextField
+
+from lnschema_core.types import ListLike, StrField
 
-from ._lookup import lookup as _lookup
 from ._queryset import QuerySet
-from .ids import base62, base62_8, base62_12, base62_20
-from .types import DataLike, PathLike, TransformType
+from .ids import base62_8, base62_12, base62_20
+from .types import TransformType
 from .users import current_user_id
 
+if TYPE_CHECKING:
+    import pandas as pd
+
 is_run_from_ipython = getattr(builtins, "__IPYTHON__", False)
 TRANSFORM_TYPE_DEFAULT = TransformType.notebook if is_run_from_ipython else TransformType.pipeline
 
 
-def validate_required_fields(orm, kwargs):
-    required_fields = {k.name for k in orm._meta.fields if not k.null and k.default is None}
-    required_fields_not_passed = {k: None for k in required_fields if k not in kwargs}
-    kwargs.update(required_fields_not_passed)
-    missing_fields = [k for k, v in kwargs.items() if v is None and k in required_fields]
-    if missing_fields:
-        raise TypeError(f"{missing_fields} are required.")
-
-
-# todo, make a CreatedUpdated Mixin, but need to figure out docs
-class BaseORM(models.Model):
-    """Base data model.
-
-    Is essentially equal to the Django Model base class, but adds the following
-    methods.
-    """
-
-    def __repr__(self) -> str:
-        fields = [field.name for field in self._meta.fields if not isinstance(field, models.ForeignKey)]
-        fields += [f"{field.name}_id" for field in self._meta.fields if isinstance(field, models.ForeignKey)]
-        fields_str = ", ".join([f"{k}={getattr(self, k)}" for k in fields if hasattr(self, k)])
-        return f"{self.__class__.__name__}({fields_str})"
-
-    def __str__(self) -> str:
-        return self.__repr__()
-
-    def __init__(self, *args, **kwargs):
-        if not args:  # object is loaded from DB
-            validate_required_fields(self, kwargs)
-        super().__init__(*args, **kwargs)
+class ORM(models.Model):
+    """LaminDB's base ORM.
+
+    Is based on `django.db.models.Model`.
+    """
+
+    def add_synonym(self, synonym: Union[str, ListLike], force: bool = False):
+        """Add synonyms to a record."""
+        pass
+
+    def remove_synonym(self, synonym: Union[str, ListLike]):
+        """Remove synonyms from a record."""
+        pass
 
     @classmethod
-    def lookup(cls, field: Optional[str] = None) -> NamedTuple:
-        """Lookup object for auto-completing field values."""
-        return _lookup(cls, field)
+    def from_values(cls, identifiers: ListLike, field: StrField, **kwargs):
+        """Parse values for an identifier (a name, an id, etc.) and create records.
+
+        This method helps avoid problems around duplication of entries,
+        violation of idempotency, and performance when creating records in bulk.
+
+        Guide: :doc:`/biology/registries`.
+
+        Args:
+            identifiers: `ListLike` A list of values for an identifier, e.g.
+                `["name1", "name2"]`.
+            field: `StrField` If `iterable` is `ListLike`, an `ORM` field to look
+                up, e.g. `lb.CellMarker.name`.
+            **kwargs: Can contain `species`. Either `"human"`, `"mouse"`, or any other
+                `name` of `Bionty.Species`. If `None`, will use default species in
+                bionty for each entity.
+
+        Returns:
+            A list of records.
+
+        For every `value` in an iterable of identifiers and a given `ORM.field`,
+        this function performs:
+
+        1. It checks whether the value already exists in the database
+        (`ORM.select(field=value)`). If so, it adds the queried record to
+        the returned list and skips step 2. Otherwise, proceed with 2.
+        2. If the `ORM` is from `lnschema_bionty`, it checks whether there is an
+        exact match in the underlying ontology (`Bionty.inspect(value, field)`).
+        If so, it creates a record from Bionty and adds it to the returned list.
+        Otherwise, it creates a record that populates a single field using `value`
+        and adds the record to the returned list.
+        """
+        pass
+
+    @classmethod
+    def inspect(
+        cls,
+        identifiers: ListLike,
+        field: StrField,
+        *,
+        case_sensitive: bool = False,
+        inspect_synonyms: bool = True,
+        return_df: bool = False,
+        logging: bool = True,
+        **kwargs,
+    ) -> Union["pd.DataFrame", Dict[str, List[str]]]:
+        """Inspect if a list of identifiers are mappable to existing values of a field.
+
+        Args:
+            identifiers: `ListLike` Identifiers that will be checked against the
+                field.
+            field: `StrField` The field of identifiers.
+                    Examples are 'ontology_id' to map against the source ID
+                    or 'name' to map against the ontologies field names.
+            case_sensitive: Whether the identifier inspection is case sensitive.
+            inspect_synonyms: Whether to inspect synonyms.
+            return_df: Whether to return a Pandas DataFrame.
+
+        Returns:
+            - A Dictionary of "mapped" and "unmapped" identifiers
+            - If `return_df`: A DataFrame indexed by identifiers with a boolean `__mapped__`
+                column that indicates compliance with the identifiers.
+
+        Examples:
+            >>> import lnschema_bionty as lb
+            >>> gene_symbols = ["A1CF", "A1BG", "FANCD1", "FANCD20"]
+            >>> lb.Gene.inspect(gene_symbols, field=lb.Gene.symbol)
+        """
+        pass
+
+    @classmethod
+    def lookup(cls, field: Optional[StrField] = None) -> NamedTuple:
+        """Return an auto-complete object for a field.
+
+        Args:
+            field: `Optional[StrField] = None` The field to
+                look up the values for. Defaults to first string field.
+
+        Returns:
+            A `NamedTuple` of lookup information of the field values with a
+            dictionary converter.
+
+        Examples:
+            >>> import lnschema_bionty as lb
+            >>> lookup = lb.Gene.lookup()
+            >>> lookup.adgb_dt
+            >>> lookup_dict = lookup.dict()
+            >>> lookup['ADGB-DT']
+        """
+        pass
+
+    @classmethod
+    def map_synonyms(
+        cls,
+        synonyms: Iterable,
+        *,
+        return_mapper: bool = False,
+        case_sensitive: bool = False,
+        keep: Literal["first", "last", False] = "first",
+        synonyms_field: str = "synonyms",
+        synonyms_sep: str = "|",
+        field: Optional[str] = None,
+        **kwargs,
+    ) -> Union[List[str], Dict[str, str]]:
+        """Maps input synonyms to standardized names.
+
+        Args:
+            synonyms: `Iterable` Synonyms that will be standardized.
+            return_mapper: `bool = False` If `True`, returns `{input_synonym1:
+                standardized_name1}`.
+            case_sensitive: `bool = False` Whether the mapping is case sensitive.
+            species: `Optional[str]` Map only against this species related entries.
+            keep: `Literal["first", "last", False] = "first"` When a synonym maps to
+                multiple names, determines which duplicates to mark as
+                `pd.DataFrame.duplicated`
+
+                    - "first": returns the first mapped standardized name
+                    - "last": returns the last mapped standardized name
+                    - `False`: returns all mapped standardized name
+            synonyms_field: `str = "synonyms"` A field containing the concatenated synonyms.
+            synonyms_sep: `str = "|"` Which separator is used to separate synonyms.
+            field: `Optional[str]` The field representing the standardized names.
+
+        Returns:
+            If `return_mapper` is `False`: a list of standardized names. Otherwise,
+            a dictionary of mapped values with mappable synonyms as keys and
+            standardized names as values.
+
+        Examples:
+            >>> import lnschema_bionty as lb
+            >>> gene_synonyms = ["A1CF", "A1BG", "FANCD1", "FANCD20"]
+            >>> standardized_names = lb.Gene.map_synonyms(gene_synonyms, species="human")
+        """
 
     @classmethod
     def select(cls, **expressions) -> Union[QuerySet, Manager]:
-        """Query the ORM."""
+        """Query records.
+
+        Guide: :doc:`/guide/select`.
+
+        Args:
+            ORM: An ORM class.
+            expressions: Fields and values passed as Django query expressions.
+
+        Returns:
+            A `QuerySet` or Django `Manager`.
+        """
         from lamindb._select import select
 
         return select(cls, **expressions)
 
+    @classmethod
+    def search(
+        cls,
+        string: str,
+        *,
+        field: Optional[StrField] = None,
+        top_hit: bool = False,
+        case_sensitive: bool = True,
+        synonyms_field: Optional[Union[str, TextField, CharField]] = "synonyms",
+        synonyms_sep: str = "|",
+    ) -> Union["pd.DataFrame", "ORM"]:
+        """Search the table.
+
+        Args:
+            string: `str` The input string to match against the field ontology values.
+            field: `Optional[StrField] = None` The field
+                against which the input string is matching.
+            top_hit: `bool = False` If `True`, return only the top hit or hits (in
+                case of equal scores).
+            case_sensitive: `bool = False` Whether the match is case sensitive.
+            synonyms_field: `bool = True` Also search synonyms. If `None`, is ignored.
+
+        Returns:
+            A sorted `DataFrame` of search results with a score in column
+            `__ratio__`. If `top_hit` is `True`, the best match.
+        """
+        pass
+
     class Meta:
         abstract = True
 
 
 # A note on required fields at the ORM level
 #
 # As Django does most of its validation on the Form-level, it doesn't offer functionality
 # for validating the integrity of an ORM object upon instantation (similar to pydantic)
 #
 # For required fields, we define them as commonly done on the SQL level together
-# with a validator in BaseORM (validate_required_fields)
+# with a validator in ORM (validate_required_fields)
 #
 # This goes against the Django convention, but goes with the SQLModel convention
 # (Optional fields can be null on the SQL level, non-optional fields cannot)
 #
 # Due to Django's convention where CharField has pre-configured (null=False, default=""), marking
 # a required field necessitates passing `default=None`. Without the validator it would trigger
 # an error at the SQL-level, with it, it triggers it at instantiation
 
+# A note on class and instance methods of core ORM
+#
+# All of these are defined and tested within lamindb, in files starting with _{orm_name}.py
 
-class User(BaseORM):
-    """User accounts.
+
+class User(ORM):
+    """Users.
 
     All data in this table is synched from the cloud user account to ensure a
     universal user identity, valid across DB instances, email & handle changes.
     """
 
     id = models.CharField(max_length=8, primary_key=True, default=None)
     """Universal id, valid across DB instances."""
     handle = models.CharField(max_length=30, unique=True, db_index=True, default=None)
-    """Universal handle, valid across DB instances."""
+    """Universal handle, valid across DB instances (required)."""
     email = models.CharField(max_length=255, unique=True, db_index=True, default=None)
-    """Latest email address."""
-    name = models.CharField(max_length=255, db_index=True)
-    """Name."""
+    """Email address (required)."""
+    name = models.CharField(max_length=255, db_index=True, null=True, default=None)
+    """Name (optional)."""  # has to match hub specification, where it's also optional
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
 
-    class Meta:
-        managed = True
-
 
-class Storage(BaseORM):
-    """Storage locations, typically cloud storage buckets.
+class Storage(ORM):
+    """Storage locations.
 
-    A file can be stored in S3 and GCP buckets or local storage locations.
-
-    This ORM tracks these locations along with metadata.
+    Either S3 or GCP buckets or local storage locations.
     """
 
     id = models.CharField(max_length=8, default=base62_8, db_index=True, primary_key=True)
     """Universal id, valid across DB instances."""
     root = models.CharField(max_length=255, db_index=True, default=None)
-    """Path to the root of the storage location (an s3 path, a local path, etc.)."""
+    """Root path of storage, an s3 path, a local path, etc. (required)."""
     type = models.CharField(max_length=30, db_index=True)
     """Local vs. s3 vs. gcp etc."""
-    region = models.CharField(max_length=63, db_index=True, null=True, default=None)
+    region = models.CharField(max_length=64, db_index=True, null=True, default=None)
     """Cloud storage region, if applicable."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_storages")
     """Creator of record, a :class:`~lamindb.User`."""
 
-    class Meta:
-        managed = True
+
+class Tag(ORM):
+    """Tags."""
+
+    id = models.CharField(max_length=8, default=base62_8, primary_key=True)
+    """A universal random id, valid across DB instances."""
+    name = models.CharField(max_length=255, db_index=True, unique=True, default=None)
+    """Name or title of tag."""
+    files = models.ManyToManyField("File", related_name="tags")
+    """:class:`~lamindb.File` records in tag."""
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_tags")
+    """Creator of record, a :class:`~lamindb.User`."""
 
 
-class Project(BaseORM):
+class Project(ORM):
     """Projects."""
 
     id = models.CharField(max_length=8, default=base62_8, primary_key=True)
     """Universal id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, unique=True, default=None)
     """Project name or title."""
     external_id = models.CharField(max_length=40, db_index=True, null=True, default=None)
     """External id (such as from a project management tool)."""
-    folders = models.ManyToManyField("Folder", related_name="projects")
-    """Project folders."""
+    tags = models.ManyToManyField("Tag", related_name="projects")
+    """Project tags."""
     files = models.ManyToManyField("File", related_name="projects")
     """Project files."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_projects")
     """Creator of record, a :class:`~lamindb.User`."""
 
-    class Meta:
-        managed = True
-
 
-class Transform(BaseORM):
-    """Data transformations.
+class Transform(ORM):
+    """Transformations of files (:class:`~lamindb.File`).
 
-    Pipelines, workflows, notebooks, app-based transforms.
+    Pipelines, workflows, notebooks, app-based transformations.
 
     A pipeline is versioned software that transforms data.
     This can be anything from typical workflow tools (Nextflow, Snakemake,
     Prefect, Apache Airflow, etc.) to simple (versioned) scripts.
-
-    Creating a file is a transform, too.
     """
 
     id = models.CharField(max_length=14, db_index=True, primary_key=True, default=None)
     """Universal id, composed of stem_id and version suffix."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Transform name or title, a pipeline name, notebook title, etc..
     """
-    short_name = models.CharField(max_length=30, db_index=True, null=True, default=None)
+    short_name = models.CharField(max_length=128, db_index=True, null=True, default=None)
     """A short name.
     """
     stem_id = models.CharField(max_length=12, default=base62_12, db_index=True)
     """Stem of id, identifying transform up to version."""
     version = models.CharField(max_length=10, default="0", db_index=True)
     """Version, defaults to `"0"`.
 
     Use this to label different versions of the same pipeline, notebook, etc.
 
     Consider using `semantic versioning <https://semver.org>`__
     with `Python versioning <https://peps.python.org/pep-0440/>`__.
     """
-    type = models.CharField(max_length=20, choices=TransformType.choices(), db_index=True, default=TRANSFORM_TYPE_DEFAULT)
+    type = models.CharField(
+        max_length=20,
+        choices=TransformType.choices(),
+        db_index=True,
+        default=TRANSFORM_TYPE_DEFAULT,
+    )
     """Transform type.
 
     Defaults to `notebook` if run from ipython and to `pipeline` if run from python.
 
     If run from the app, it defaults to `app`.
     """
     reference = models.CharField(max_length=255, db_index=True, null=True, default=None)
@@ -200,334 +375,197 @@
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_transforms")
     """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
-        managed = True
         unique_together = (("stem_id", "version"),)
 
-    def __init__(self, *args, **kwargs):
-        if len(args) > 0:  # initialize with all fields from db as args
-            super().__init__(*args, **kwargs)
-            return None
-        else:  # user-facing calling signature
-            # set default ids
-            if "id" not in kwargs and "stem_id" not in kwargs:
-                kwargs["id"] = base62(14)
-                kwargs["stem_id"] = kwargs["id"][:12]
-            elif "stem_id" in kwargs:
-                assert isinstance(kwargs["stem_id"], str) and len(kwargs["stem_id"]) == 12
-                kwargs["id"] = kwargs["stem_id"] + base62(2)
-            elif "id" in kwargs:
-                assert isinstance(kwargs["id"], str) and len(kwargs["id"]) == 14
-                kwargs["stem_id"] = kwargs["id"][:12]
-            super().__init__(**kwargs)
-
 
-class Run(BaseORM):
-    """Runs of data transformations.
+class Run(ORM):
+    """Runs of transformations (:class:`~lamindb.Transform`).
 
     Typically, a run has inputs and outputs:
 
-    - References to outputs are stored in the `File` ORM in the `run` field.
+    - References to outputs are stored in :class:`~lamindb.File` in the `run` field.
       This is possible as every given file has a unique run that created it. Any
       given `Run` can output multiple `files`: `run.outputs`.
-    - References to inputs are stored in the `RunInput` ORM, a many-to-many link
-      ORM between `File` and `Run`. Any `file` might serve as an input for
-      multiple `runs`: `file.input_of`. Similarly, any `run` might have many
-      `files` as inputs: `run.inputs`.
+    - References to inputs are stored in the :class:`~lamindb.File` in the
+      `input_of` field. Any `file` might serve as an input for multiple `runs`.
+      Similarly, any `run` might have many `files` as inputs: `run.inputs`.
     """
 
     id = models.CharField(max_length=20, default=base62_20, primary_key=True)
     """Universal id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Name or title of run."""
     external_id = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """External id (such as from a workflow tool)."""
     transform = models.ForeignKey(Transform, PROTECT, related_name="runs")
     """The transform :class:`~lamindb.Transform` that is being run."""
-    inputs = models.ManyToManyField("File", through="RunInput", related_name="input_of")
+    inputs = models.ManyToManyField("File", related_name="input_of")
     """The input files for the run."""
     # outputs on File
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     run_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of run execution."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_runs")
     """Creator of record, a :class:`~lamindb.User`."""
 
-    class Meta:
-        managed = True
 
+class Dataset(ORM):
+    """Datasets: measurements of features.
+
+    Datasets are measurements of features (aka observations of variables).
+
+    1. A feature can be a “high-level” feature, i.e., it has meaning, can label
+       a column in a DataFrame, and can be modeled as a Feature or another ORM.
+       Examples: gene id, protein id, phenotype name, temperature,
+       concentration, treatment label, treatment id, etc.
+    2. In other cases, a feature might be a “low-level” feature without semantic
+       meaning. Examples: pixels, single letters in sequences, etc.
+
+    LaminDB typically stores datasets as files (`.files`), either as
+
+    1. serialized `DataFrame` or `AnnData` objects (for high-level features)
+    2. a set of files of any type (for low-level features, e.g., a folder of
+       images or fastqs)
+
+    In simple cases, a single serialized DataFrame or AnnData object (`.file`)
+    is enough.
+
+    One might also store a dataset in a SQL table or view, but this is not yet
+    supported by LaminDB.
+    """
+
+    id = models.CharField(max_length=20, default=base62_20, primary_key=True)
+    """Universal id, valid across DB instances."""
+    name = models.CharField(max_length=255, db_index=True, default=None)
+    """Name or title of dataset (required)."""
+    description = models.TextField(null=True, default=None)
+    """A description."""
+    hash = models.CharField(max_length=86, db_index=True, null=True, default=None)
+    """Hash of dataset content. 86 base64 chars allow to store 64 bytes, 512 bits."""
+    feature_sets = models.ManyToManyField("FeatureSet", related_name="datasets")
+    """The feature sets measured in this dataset."""
+    file = models.ForeignKey("File", on_delete=PROTECT, null=True, unique=True, related_name="datasets")
+    """Storage of dataset as a one file."""
+    files = models.ManyToManyField("File", related_name="datasets")
+    """Storage of dataset as multiple file."""
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of run execution."""
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_datasets")
+    """Creator of record, a :class:`~lamindb.User`."""
+
+
+class Feature(ORM):
+    """Features: column names of DataFrames.
 
-class FeatureSet(BaseORM):
-    """Feature sets.
+    Note that you can use Bionty ORMs to manage common features like genes,
+    pathways, proteins & cell markers.
 
-    A feature set is represented by the hash of the set of primary keys and the feature type.
+    Similarly, you can define custom ORMs to manage features like gene sets, nodes, etc.
+
+    This ORM is a way of getting started without using Bionty or a custom schema.
+    """
+
+    id = models.CharField(max_length=12, default=base62_12, primary_key=True)
+    """Universal id, valid across DB instances."""
+    name = models.CharField(max_length=255, db_index=True, default=None)
+    """Name or title of feature (required)."""
+    type = models.CharField(max_length=96, null=True, default=None)
+    """A way of grouping features of same type."""
+    description = models.TextField(null=True, default=None)
+    """A description."""
+    feature_sets = models.ManyToManyField("FeatureSet", related_name="features")
+    """Feature sets linked to this gene."""
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of run execution."""
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_features")
+    """Creator of record, a :class:`~lamindb.User`."""
+
+
+class FeatureSet(ORM):
+    """Feature sets: sets of features.
+
+    A feature set is represented by the hash of the id set for the feature type.
 
     The current supported feature types are `lnschema_bionty.Gene`,
     `lnschema_bionty.Protein`, and `lnschema_bionty.CellMarker`.
 
     Guides:
 
     - :doc:`/biology/scrna`
     - :doc:`/biology/flow`
 
     Examples:
 
     >>> import lnschema_bionty as bt
     >>> reference = bt.Gene(species="mouse")
-    >>> features = ln.Features.from_iterable(adata.var["ensemble_id"], Gene.ensembl_gene_id)
-    >>> features.save()
+    >>> feature_set = ln.FeatureSet.from_values(adata.var["ensemble_id"], Gene.ensembl_gene_id)
+    >>> feature_set.save()
     >>> file = ln.File(adata, name="Mouse Lymph Node scRNA-seq")
     >>> file.save()
     >>> file.featuresets.add(featureset)
 
     """
 
     id = models.CharField(max_length=64, primary_key=True, default=None)
     """A universal id, valid across DB instances, a hash of the linked set of features."""
     type = models.CharField(max_length=64)
     """A feature entity type."""
-    files = models.ManyToManyField("File", related_name="featuresets")
-    """Files linked to the featureset."""
+    files = models.ManyToManyField("File", related_name="feature_sets")
+    """Files linked to the feature set."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_featuresets")
     """Creator of record, a :class:`~lamindb.User`."""
 
-    class Meta:
-        managed = True
-
-    @classmethod
-    def from_iterable(
-        cls,
-        iterable: Iterable,
-        field: models.CharField,
-        species: str = None,
-    ):
-        """Parse iterable & return featureset & records."""
-        from lamindb._features import parse_features_from_iterable
-
-        features = parse_features_from_iterable(
-            iterable=iterable,
-            field=field,
-            species=species,
-        )
-        return features
-
-    def __init__(self, *args, **kwargs):  # type: ignore
-        related_names = [i.related_name for i in self.__class__._meta.related_objects]
-
-        relationships: Dict = {}
-        for related_name in related_names:
-            if related_name in kwargs:
-                relationships[related_name] = kwargs.pop(related_name)
-        self._relationships = relationships
-
-        super().__init__(*args, **kwargs)
-
-    def save(self, *args, **kwargs):
-        super().save(*args, **kwargs)
-        for key, records in self._relationships.items():
-            [r.save() for r in records]
-            getattr(self, key).set(records)
 
+class File(ORM):
+    """Test."""
 
-class Folder(BaseORM):
-    id = models.CharField(max_length=20, primary_key=True)
-    """A universal random id, valid across DB instances."""
-    name = models.CharField(max_length=255, db_index=True, default=None)
-    """Name or title of folder."""
-    # below is one of the few cases with null=True, default=None
-    key = models.CharField(max_length=255, db_index=True, null=True, default=None)
-    """Storage key of folder."""
-    storage = models.ForeignKey(Storage, PROTECT, related_name="folders", null=True)
-    """:class:`~lamindb.Storage` location of folder, see `.path()` for full path."""
-    files = models.ManyToManyField("File", related_name="folders")
-    """:class:`~lamindb.File` records in folder."""
-    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
-    """Time of creation of record."""
-    updated_at = models.DateTimeField(auto_now=True, db_index=True)
-    """Time of last update to record."""
-    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_folders")
-    """Creator of record, a :class:`~lamindb.User`."""
-
-    class Meta:
-        managed = True
-        unique_together = (("storage", "key"),)
-
-    @property
-    def __name__(cls) -> str:
-        return "Folder"
-
-    def path(self) -> Union[Path, UPath]:
-        """Path on storage."""
-        from lamindb._file_access import filepath_from_file_or_folder
-
-        return filepath_from_file_or_folder(self)
-
-    def tree(
-        self,
-        level: int = -1,
-        limit_to_directories: bool = False,
-        length_limit: int = 1000,
-    ) -> None:
-        """Print a visual tree structure."""
-        from lamindb._folder import tree
-
-        return tree(
-            self,
-            level=level,
-            limit_to_directories=limit_to_directories,
-            length_limit=length_limit,
-        )
-
-    def __init__(self, *args, **kwargs):
-        from lamindb._folder import init_folder
-
-        init_folder(self, *args, **kwargs)
-
-    def save(self, *args, **kwargs) -> None:
-        """Save the folder."""
-        # only has attr _files if freshly initialized
-        if hasattr(self, "_files"):
-            for file in self._files:
-                file.save()
-        super().save(*args, **kwargs)
-        if hasattr(self, "_files"):
-            self.files.set(self._files)
-
-
-class File(BaseORM):
     id = models.CharField(max_length=20, primary_key=True)
     """A universal random id (20-char base62), valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
-    """A universal random id, valid across DB instances."""
+    """A name or title for the file, mostly useful if no key is provided."""
+    key = models.CharField(max_length=255, db_index=True, null=True, default=None)
+    """Storage key, the relative path within the storage location."""
     suffix = models.CharField(max_length=30, db_index=True, null=True, default=None)
     """File suffix.
 
     This is a file extension if the `file` is stored in a file format.
     It's `None` if the storage format doesn't have a canonical extension.
     """
     size = models.BigIntegerField(null=True, db_index=True)
     """Size in bytes.
 
     Examples: 1KB is 1e3 bytes, 1MB is 1e6, 1GB is 1e9, 1TB is 1e12 etc.
     """
     hash = models.CharField(max_length=86, db_index=True, null=True, default=None)
     """Hash of file content. 86 base64 chars allow to store 64 bytes, 512 bits."""
-    # below is one of the few cases with null=True, default=None
-    key = models.CharField(max_length=255, db_index=True, null=True, default=None)
-    """Storage key, the relative path within the storage location."""
     run = models.ForeignKey(Run, PROTECT, related_name="outputs", null=True)
     """:class:`~lamindb.Run` that created the `file`."""
     transform = models.ForeignKey(Transform, PROTECT, related_name="files", null=True)
     """:class:`~lamindb.Transform` whose run created the `file`."""
     storage: "Storage" = models.ForeignKey(Storage, PROTECT, related_name="files")
     """:class:`~lamindb.Storage` location of `file`, see `.path()` for full path."""
-    # folders from Folders.files
+    # tags from Tags.files
     # features from Features.files
     # input_of from Run.inputs
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_files")
     """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
-        managed = True
         unique_together = (("storage", "key"),)
-
-    def path(self) -> Union[Path, UPath]:
-        """Path on storage."""
-        from lamindb._file_access import filepath_from_file_or_folder
-
-        return filepath_from_file_or_folder(self)
-
-    # likely needs an arg `key`
-    def replace(
-        self,
-        data: Union[PathLike, DataLike],
-        run: Optional[Run] = None,
-        format: Optional[str] = None,
-    ) -> None:
-        """Replace file content."""
-        from lamindb._file import replace_file
-
-        replace_file(self, data, run, format)
-
-    @overload
-    def __init__(
-        data: Union[PathLike, DataLike],
-        key: Optional[str] = None,
-        name: Optional[str] = None,
-        run: Optional[Run] = None,
-    ):
-        ...
-
-    @overload
-    def __init__(
-        *args,
-        **kwargs,
-    ):
-        ...
-
-    def __init__(  # type: ignore
-        self,
-        *args,
-        **kwargs,
-    ):
-        from lamindb._file import init_file
-
-        init_file(self, *args, **kwargs)
-
-    def save(self, *args, **kwargs) -> None:
-        """Save the file to database & storage."""
-        self._save_skip_storage(*args, **kwargs)
-        from lamindb._save import check_and_attempt_clearing, check_and_attempt_upload
-
-        exception = check_and_attempt_upload(self)
-        if exception is not None:
-            self._delete_skip_storage()
-            raise RuntimeError(exception)
-        exception = check_and_attempt_clearing(self)
-        if exception is not None:
-            raise RuntimeError(exception)
-
-    def _save_skip_storage(self, *args, **kwargs) -> None:
-        if self.transform is not None:
-            self.transform.save()
-        if self.run is not None:
-            self.run.save()
-        super().save(*args, **kwargs)
-
-    def delete(self, *args, **kwargs) -> None:
-        from lamindb._file_access import storage_key_from_file
-        from lamindb.dev.storage import delete_storage
-
-        storage_key = storage_key_from_file(self)
-
-        self._delete_skip_storage(*args, **kwargs)
-
-        try:
-            delete_storage(storage_key)
-            logger.success(f"Deleted {colors.yellow(f'object {storage_key}')} from storage.")
-        except Exception:
-            traceback.print_exc()
-
-    def _delete_skip_storage(self, *args, **kwargs) -> None:
-        super().delete(*args, **kwargs)
-
-
-class RunInput(BaseORM):
-    run = models.ForeignKey("Run", on_delete=models.CASCADE)
-    file = models.ForeignKey("File", on_delete=models.CASCADE)
-
-    class Meta:
-        managed = True
-        unique_together = ("run", "file")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lamindb_setup-0.47.9/lnschema-core/pyproject.toml` & `lamindb_setup-0.48.0/lnschema-core/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "lamindb_setup",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lnschema-core"
 
 [project.optional-dependencies]
-test = [
+dev = [
+    "lamindb_setup>=0.47.8",  # not possible on PyPI:  @ git+https://github.com/laminlabs/lamindb-setup
     "pre-commit",
     "nox",
     "laminci",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject-test",
 ]
```

### Comparing `lamindb_setup-0.47.9/noxfile.py` & `lamindb_setup-0.48.0/noxfile.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,35 +31,33 @@
 )
 def install(session: nox.Session, group: str) -> None:
     session.run(*"pip install git+https://github.com/laminlabs/bionty".split())
     session.run(
         *"pip install --no-deps git+https://github.com/laminlabs/lnschema-bionty"
         .split()
     )
-    # session.run(
-    #     *"pip install --no-deps git+https://github.com/laminlabs/lnschema-lamin1"
-    #     .split()
-    # )
     # install lnschema-core from sub-module
     session.run(*"pip install --no-deps ./lnschema-core".split())
     # install lamindb-setup without deps
-    session.run(*"pip install .[aws,test]".split())
+    session.run(*"pip install .[aws,dev]".split())
 
 
 @nox.session
 @nox.parametrize(
     "group",
     ["unit", "docs"],
 )
 def build(session: nox.Session, group: str):
     login_testuser1(session, env=env)
     login_testuser2(session, env=env)
     coverage_args = "--cov=lamindb_setup --cov-append --cov-report=term-missing"  # noqa
     if group.startswith("unit"):
-        session.run(*f"pytest -s {coverage_args} ./tests".split(), env=env)
+        session.run(
+            *f"pytest -s {coverage_args} ./tests --ignore tests/hub".split(), env=env
+        )
     elif group.startswith("docs"):
         session.run(*f"pytest -s {coverage_args} ./docs".split(), env=env)
 
 
 @nox.session
 def docs(session: nox.Session):
     session.run(*"lamin init --storage ./docsbuild".split())
```

### Comparing `lamindb_setup-0.47.9/pyproject.toml` & `lamindb_setup-0.48.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,50 +4,48 @@
 
 [project]
 name = "lamindb_setup"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
-    # PINNED internal LAMIN dependency
-    # !!! lnhub_rest cannot be pinned in LaminDB !!!
-    # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.9.10",
-    "sqlmodel",  # this here just for lnhub_rest
-    # NO other Lamin packages should be pinned or even be a dependency
     "lnschema_core>=0.35.4",
     "lamin_logger>=0.3.3",
     # External dependencies
     "django",
     "dj_database_url",
     "pydantic[dotenv]",
-    "ipython",
-    "sqlalchemy",  # just temporarily
+    "sqlalchemy<2.0.0",  # just temporarily
     "appdirs",
-    "pandas",  # remove!!!
     "python-dateutil",
-    "universal_pathlib"
+    "universal_pathlib",
+    "botocore",
+    "supabase==1.0.3",
+    "pyjwt",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lamindb-setup"
 
 [project.optional-dependencies]
 aws = [
     "s3fs",
 ]
-test = [
+dev = [
     "psycopg2-binary",
     "python-dotenv",
     "erdiagram",
     "pre-commit",
     "nox",
     "pytest>=6.0",
     "pytest-cov",
+    "pytest-xdist",
     "nbproject-test>=0.4.3",
+    "faker",
+    "moto[s3]",
 ]
 
 [project.scripts]
 lamin = "lamindb_setup.__main__:main"
 
 [tool.black]
 preview = true
```

### Comparing `lamindb_setup-0.47.9/tests/test_init_instance.py` & `lamindb_setup-0.48.0/tests/test_init_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from pathlib import Path
 
-import pytest
-
 import lamindb_setup as ln_setup
 
 pgurl = "postgresql://postgres:pwd@0.0.0.0:5432/pgtest"
 
 
 def test_init_instance_postgres_default_name():
     ln_setup.init(storage="./mydatapg", db=pgurl, _test=True)
@@ -79,10 +77,10 @@
 # # this fails because there is already an sqlite with the same name in that bucket
 # # hence, the sqlite file would clash
 
 # # with pytest.raises(RuntimeError):
 # #     ln_setup.init(storage="s3://lamindb-ci")
 
 
-def test_value_error_schema():
-    with pytest.raises(ValueError):
-        ln_setup.init(storage="tmpstorage1", schema="bionty, xyz1")
+# def test_value_error_schema():
+#     with pytest.raises(ModuleNotFoundError):
+#         ln_setup.init(storage="tmpstorage1", schema="bionty, xyz1")
```

### Comparing `lamindb_setup-0.47.9/tests/test_load_instance.py` & `lamindb_setup-0.48.0/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.9/PKG-INFO` & `lamindb_setup-0.48.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.47.9
+Version: 0.48.0
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnhub_rest==0.9.10
-Requires-Dist: sqlmodel
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
 Requires-Dist: django
 Requires-Dist: dj_database_url
 Requires-Dist: pydantic[dotenv]
-Requires-Dist: ipython
-Requires-Dist: sqlalchemy
+Requires-Dist: sqlalchemy<2.0.0
 Requires-Dist: appdirs
-Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: universal_pathlib
+Requires-Dist: botocore
+Requires-Dist: supabase==1.0.3
+Requires-Dist: pyjwt
 Requires-Dist: s3fs ; extra == "aws"
-Requires-Dist: psycopg2-binary ; extra == "test"
-Requires-Dist: python-dotenv ; extra == "test"
-Requires-Dist: erdiagram ; extra == "test"
-Requires-Dist: pre-commit ; extra == "test"
-Requires-Dist: nox ; extra == "test"
-Requires-Dist: pytest>=6.0 ; extra == "test"
-Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: nbproject-test>=0.4.3 ; extra == "test"
+Requires-Dist: psycopg2-binary ; extra == "dev"
+Requires-Dist: python-dotenv ; extra == "dev"
+Requires-Dist: erdiagram ; extra == "dev"
+Requires-Dist: pre-commit ; extra == "dev"
+Requires-Dist: nox ; extra == "dev"
+Requires-Dist: pytest>=6.0 ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: pytest-xdist ; extra == "dev"
+Requires-Dist: nbproject-test>=0.4.3 ; extra == "dev"
+Requires-Dist: faker ; extra == "dev"
+Requires-Dist: moto[s3] ; extra == "dev"
 Project-URL: Home, https://github.com/laminlabs/lamindb-setup
 Provides-Extra: aws
-Provides-Extra: test
+Provides-Extra: dev
 
 [![codecov](https://codecov.io/gh/laminlabs/lamindb-setup/branch/main/graph/badge.svg)](https://codecov.io/gh/laminlabs/lamindb-setup)
 
 # lamindb-setup: Setup LaminDB
 
 - Stable user docs: [lamin.ai/docs/setup/](https://lamin.ai/docs/setup/)
 - Latest developer docs: [netlify](https://lndb-htry.netlify.app/docs/lndb/)
```

