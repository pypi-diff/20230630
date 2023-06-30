# Comparing `tmp/django-axes-6.0.4.tar.gz` & `tmp/django-axes-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-axes-6.0.4.tar", last modified: Thu Jun 22 08:47:47 2023, max compression
+gzip compressed data, was "django-axes-6.0.5.tar", last modified: Fri Jun 30 21:07:57 2023, max compression
```

## Comparing `django-axes-6.0.4.tar` & `django-axes-6.0.5.tar`

### file list

```diff
@@ -1,136 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.769328 django-axes-6.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.753328 django-axes-6.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.753328 django-axes-6.0.4/.github/ISSUE_TEMPLATES/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/ISSUE_TEMPLATES/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/ISSUE_TEMPLATES/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.753328 django-axes-6.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-22 08:47:27.000000 django-axes-6.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 08:47:27.000000 django-axes-6.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 08:47:27.000000 django-axes-6.0.4/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-06-22 08:47:27.000000 django-axes-6.0.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-22 08:47:27.000000 django-axes-6.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-22 08:47:27.000000 django-axes-6.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-22 08:47:27.000000 django-axes-6.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36853 2023-06-22 08:47:47.769328 django-axes-6.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-22 08:47:27.000000 django-axes-6.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.757328 django-axes-6.0.4/axes/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.757328 django-axes-6.0.4/axes/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.757328 django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.757328 django-axes-6.0.4/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset_failure_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0007_alter_accessattempt_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0008_accessfailurelog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-22 08:47:27.000000 django-axes-6.0.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.765329 django-axes-6.0.4/django_axes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36853 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.765329 django-axes-6.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/10_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/1_requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/2_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/3_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/4_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/5_customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/6_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/7_architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/8_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/9_contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.765329 django-axes-6.0.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/images/flow.png
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-22 08:47:27.000000 django-axes-6.0.4/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-22 08:47:27.000000 django-axes-6.0.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-22 08:47:27.000000 django-axes-6.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 08:47:27.000000 django-axes-6.0.4/requirements-qa.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-22 08:47:27.000000 django-axes-6.0.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 08:47:27.000000 django-axes-6.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 08:47:47.769328 django-axes-6.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-22 08:47:27.000000 django-axes-6.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.769328 django-axes-6.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    38226 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/urls_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.525846 django-axes-6.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/.github/ISSUE_TEMPLATES/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/ISSUE_TEMPLATES/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/ISSUE_TEMPLATES/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-30 21:07:43.000000 django-axes-6.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 21:07:43.000000 django-axes-6.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 21:07:43.000000 django-axes-6.0.5/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    32723 2023-06-30 21:07:43.000000 django-axes-6.0.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-30 21:07:43.000000 django-axes-6.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-30 21:07:43.000000 django-axes-6.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-30 21:07:43.000000 django-axes-6.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36937 2023-06-30 21:07:57.521846 django-axes-6.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-30 21:07:43.000000 django-axes-6.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset_failure_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0008_accessfailurelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-30 21:07:43.000000 django-axes-6.0.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36937 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.521846 django-axes-6.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/9_contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-30 21:07:44.000000 django-axes-6.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-30 21:07:44.000000 django-axes-6.0.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.521846 django-axes-6.0.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-06-30 21:07:44.000000 django-axes-6.0.5/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-30 21:07:44.000000 django-axes-6.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-30 21:07:44.000000 django-axes-6.0.5/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-30 21:07:44.000000 django-axes-6.0.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-30 21:07:44.000000 django-axes-6.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 21:07:44.000000 django-axes-6.0.5/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 21:07:44.000000 django-axes-6.0.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 21:07:44.000000 django-axes-6.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:07:57.525846 django-axes-6.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-30 21:07:44.000000 django-axes-6.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.521846 django-axes-6.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38226 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/urls_empty.py
```

### Comparing `django-axes-6.0.4/.github/ISSUE_TEMPLATES/bug_report.md` & `django-axes-6.0.5/.github/ISSUE_TEMPLATES/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/.github/ISSUE_TEMPLATES/feature_request.md` & `django-axes-6.0.5/.github/ISSUE_TEMPLATES/feature_request.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/.github/PULL_REQUEST_TEMPLATE.md` & `django-axes-6.0.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/.github/workflows/codeql.yml` & `django-axes-6.0.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/.github/workflows/release.yml` & `django-axes-6.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/.github/workflows/test.yml` & `django-axes-6.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/CHANGES.rst` & `django-axes-6.0.5/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 
 Changes
 =======
 
 
+6.0.5 (2023-07-01)
+------------------
+
+- Add Indonesion translation.
+  [kiraware]
+
+
 6.0.4 (2023-06-22)
 ------------------
 
 - Remove unused methods from AxesStandaloneBackend.
   [314eter]
```

### Comparing `django-axes-6.0.4/CODE_OF_CONDUCT.md` & `django-axes-6.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/CONTRIBUTING.rst` & `django-axes-6.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/LICENSE` & `django-axes-6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/PKG-INFO` & `django-axes-6.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.4
+Version: 6.0.5
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -123,14 +123,21 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.5 (2023-07-01)
+------------------
+
+- Add Indonesion translation.
+  [kiraware]
+
+
 6.0.4 (2023-06-22)
 ------------------
 
 - Remove unused methods from AxesStandaloneBackend.
   [314eter]
```

### Comparing `django-axes-6.0.4/README.rst` & `django-axes-6.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/admin.py` & `django-axes-6.0.5/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/apps.py` & `django-axes-6.0.5/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/attempts.py` & `django-axes-6.0.5/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/backends.py` & `django-axes-6.0.5/axes/backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/checks.py` & `django-axes-6.0.5/axes/checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/conf.py` & `django-axes-6.0.5/axes/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/decorators.py` & `django-axes-6.0.5/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/handlers/base.py` & `django-axes-6.0.5/axes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/handlers/cache.py` & `django-axes-6.0.5/axes/handlers/cache.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/handlers/database.py` & `django-axes-6.0.5/axes/handlers/database.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/handlers/dummy.py` & `django-axes-6.0.5/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/handlers/proxy.py` & `django-axes-6.0.5/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/handlers/test.py` & `django-axes-6.0.5/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/helpers.py` & `django-axes-6.0.5/axes/helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/django.mo` & `django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/django.po` & `django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-6.0.5/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-6.0.5/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/django.mo` & `django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/django.po` & `django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/management/commands/axes_reset_failure_logs.py` & `django-axes-6.0.5/axes/management/commands/axes_reset_failure_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/management/commands/axes_reset_ip.py` & `django-axes-6.0.5/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/management/commands/axes_reset_logs.py` & `django-axes-6.0.5/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/management/commands/axes_reset_username.py` & `django-axes-6.0.5/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/middleware.py` & `django-axes-6.0.5/axes/middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/migrations/0001_initial.py` & `django-axes-6.0.5/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-6.0.5/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-6.0.5/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-6.0.5/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/migrations/0007_alter_accessattempt_unique_together.py` & `django-axes-6.0.5/axes/migrations/0007_alter_accessattempt_unique_together.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/migrations/0008_accessfailurelog.py` & `django-axes-6.0.5/axes/migrations/0008_accessfailurelog.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/models.py` & `django-axes-6.0.5/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/signals.py` & `django-axes-6.0.5/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/axes/utils.py` & `django-axes-6.0.5/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/django_axes.egg-info/PKG-INFO` & `django-axes-6.0.5/django_axes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.4
+Version: 6.0.5
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -123,14 +123,21 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.5 (2023-07-01)
+------------------
+
+- Add Indonesion translation.
+  [kiraware]
+
+
 6.0.4 (2023-06-22)
 ------------------
 
 - Remove unused methods from AxesStandaloneBackend.
   [314eter]
```

### Comparing `django-axes-6.0.4/django_axes.egg-info/SOURCES.txt` & `django-axes-6.0.5/django_axes.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 axes/handlers/dummy.py
 axes/handlers/proxy.py
 axes/handlers/test.py
 axes/locale/ar/LC_MESSAGES/django.mo
 axes/locale/ar/LC_MESSAGES/django.po
 axes/locale/de/LC_MESSAGES/django.mo
 axes/locale/de/LC_MESSAGES/django.po
+axes/locale/id/LC_MESSAGES/django.mo
+axes/locale/id/LC_MESSAGES/django.po
 axes/locale/pl/LC_MESSAGES/django.mo
 axes/locale/pl/LC_MESSAGES/django.po
 axes/locale/ru/LC_MESSAGES/django.mo
 axes/locale/ru/LC_MESSAGES/django.po
 axes/locale/tr/LC_MESSAGES/django.mo
 axes/locale/tr/LC_MESSAGES/django.po
 axes/management/__init__.py
```

### Comparing `django-axes-6.0.4/docs/1_requirements.rst` & `django-axes-6.0.5/docs/1_requirements.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/docs/2_installation.rst` & `django-axes-6.0.5/docs/2_installation.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/docs/3_usage.rst` & `django-axes-6.0.5/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/docs/4_configuration.rst` & `django-axes-6.0.5/docs/4_configuration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/docs/5_customization.rst` & `django-axes-6.0.5/docs/5_customization.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/docs/6_integration.rst` & `django-axes-6.0.5/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/docs/7_architecture.rst` & `django-axes-6.0.5/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/docs/Makefile` & `django-axes-6.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/docs/conf.py` & `django-axes-6.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/docs/images/flow.png` & `django-axes-6.0.5/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/pyproject.toml` & `django-axes-6.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/setup.py` & `django-axes-6.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/base.py` & `django-axes-6.0.5/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/settings.py` & `django-axes-6.0.5/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_admin.py` & `django-axes-6.0.5/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_attempts.py` & `django-axes-6.0.5/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_backends.py` & `django-axes-6.0.5/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_checks.py` & `django-axes-6.0.5/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_decorators.py` & `django-axes-6.0.5/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_failures.py` & `django-axes-6.0.5/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_handlers.py` & `django-axes-6.0.5/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_helpers.py` & `django-axes-6.0.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_logging.py` & `django-axes-6.0.5/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_login.py` & `django-axes-6.0.5/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_management.py` & `django-axes-6.0.5/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_middleware.py` & `django-axes-6.0.5/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.4/tests/test_models.py` & `django-axes-6.0.5/tests/test_models.py`

 * *Files identical despite different names*

