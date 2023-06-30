# Comparing `tmp/UnleashClient-5.6.0.tar.gz` & `tmp/UnleashClient-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/UnleashClient-5.6.0.tar", last modified: Fri Apr  7 08:04:50 2023, max compression
+gzip compressed data, was "/home/runner/work/unleash-client-python/unleash-client-python/dist/.tmp-vk9kzf1p/UnleashClient-5.7.0.tar", last modified: Fri Jun 30 11:56:36 2023, max compression
```

## Comparing `UnleashClient-5.6.0.tar` & `UnleashClient-5.7.0.tar`

### file list

```diff
@@ -1,150 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.devcontainer/post_install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/workflows/add-to-project.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/workflows/release-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient/
--rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient/api/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/api/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/api/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/deprecation_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient/features/
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/features/Feature.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient/periodic_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/periodic_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/periodic_tasks/fetch_and_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/periodic_tasks/send_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/ApplicationHostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/Default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/FlexibleRolloutStrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/GradualRolloutRandom.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/GradualRolloutSessionId.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/GradualRolloutUserId.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/RemoteAddress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/Strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/UserWithId.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient/variants/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/variants/Variants.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/UnleashClient/variants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 08:04:48.000000 UnleashClient-5.6.0/UnleashClient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/UnleashClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/basecache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/customcache.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/customstrategies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/eventcallbacks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/filecache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/strategy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/unleashclient.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/docs/wsgi.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/get-spec.sh
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/integration_tests/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/integration_tests/integration_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/integration_tests/integration_unleashheroku.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/integration_tests/integration_unleashhosted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/specification_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/specification_tests/test_client_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/unit_tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/api/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/api/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/api/test_register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/unit_tests/periodic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/periodic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/periodic/test_fetch_and_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/unit_tests/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/strategies/test_applicationhostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/strategies/test_defaultstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/strategies/test_flexiblerollout.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/strategies/test_gradualrolloutrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/strategies/test_gradualrolloutwithsessionid.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/strategies/test_gradualrolloutwithuserid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/strategies/test_remoteaddress.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/strategies/test_userwithids.py
--rw-r--r--   0 runner    (1001) docker     (123)    22320 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/test_custom_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/unit_tests/test_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/utilities/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/mocks/mock_all_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/mocks/mock_bootstrap.json
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/mocks/mock_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/mocks/mock_custom_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/mocks/mock_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/mocks/mock_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/mocks/mock_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:04:50.000000 UnleashClient-5.6.0/tests/utilities/old_code/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/old_code/StrategyV2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/old_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tests/utilities/testing_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 08:03:59.000000 UnleashClient-5.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.devcontainer/post_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/add-to-project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/release-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.lift.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/api/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/deprecation_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/features/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/periodic_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/periodic_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/periodic_tasks/fetch_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/periodic_tasks/send_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/ApplicationHostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/Default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/FlexibleRolloutStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutRandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutSessionId.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutUserId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/RemoteAddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/Strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/UserWithId.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/variants/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/variants/Variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/variants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/basecache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/customcache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/customstrategies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/eventcallbacks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/filecache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/strategy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/unleashclient.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/wsgi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/scripts/get-spec.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/integration_tests/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/integration_tests/integration_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/integration_tests/integration_unleashheroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/integration_tests/integration_unleashhosted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/specification_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/specification_tests/test_client_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/unit_tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/api/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/api/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/api/test_register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/unit_tests/periodic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/periodic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/periodic/test_fetch_and_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_applicationhostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_defaultstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_flexiblerollout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_gradualrolloutrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_gradualrolloutwithsessionid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_gradualrolloutwithuserid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_remoteaddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_userwithids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23845 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_custom_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/utilities/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_all_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_bootstrap.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_custom_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/utilities/old_code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/old_code/StrategyV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/old_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/testing_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tox.ini
```

### Comparing `UnleashClient-5.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/.github/PULL_REQUEST_TEMPLATE.md` & `UnleashClient-5.7.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 - [ ] My code follows the style guidelines of this project
 - [ ] I have performed a self-review of my own code
 - [ ] I have commented my code, particularly in hard-to-understand areas
 - [ ] I have made corresponding changes to the documentation
 - [ ] My changes generate no new warnings
 - [ ] I have added tests that prove my fix is effective or that my feature works
 - [ ] New and existing unit tests pass locally with my changes
-- [ ] Any dependent changes have been merged and published in downstream modules
+- [ ] Any dependent changes have been merged and published in downstream modules
```

### Comparing `UnleashClient-5.6.0/.github/workflows/codeql-analysis.yml` & `UnleashClient-5.7.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/.github/workflows/release-docs.yml` & `UnleashClient-5.7.0/.github/workflows/release-package.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,42 @@
-name: Release docs
+name: Release package
 
 on:
-  push:
-    branches: ["main"]
+  release:
+    types: [published]
 
 jobs:
-  Build:
+  main:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v1
-      - name: Set up Python 3.9
-        uses: actions/setup-python@v2
+      - name: Set up Python 3.7
+        uses: actions/setup-python@v1
         with:
-          python-version: 3.9
+          python-version: 3.7
       - name: Install dependencies
         run: |
-          python -m pip install --upgrade pip
-          pip install -r requirements.txt
-          pip install wheel
-          python setup.py install
+          make install
+      - name: Build package
+        run: |
+          make build
+        env:
+          TWINE_USERNAME: ${{ secrets.pypi_username }}
+          TWINE_PASSWORD: ${{ secrets.pypi_password }}
       - name: Build docs
         run: |
           cd docs
           make html
       - name: Deploy docs
         uses: peaceiris/actions-gh-pages@v3
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
-          publish_dir: ./docs/_build/html
+          publish_dir: ./docs/_build/html
+      - name: Notify Slack of pipeline completion
+        uses: 8398a7/action-slack@v2
+        with:
+          status: ${{ job.status }}
+          author_name: Github Action
+        env:
+          GITHUB_TOKEN: ${{ secrets.github_slack_token }}
+          SLACK_WEBHOOK_URL: ${{ secrets.slack_webhook }}
+        if: always()
```

### Comparing `UnleashClient-5.6.0/.github/workflows/release-package.yml` & `UnleashClient-5.7.0/.github/workflows/pull_request.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-name: Release package
+name: CI
 
 on:
-  release:
-    types: [published]
+  push:
+  pull_request:
 
 jobs:
   main:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v1
       - name: Set up Python 3.7
-        uses: actions/setup-python@v1
+        uses: actions/setup-python@v2
         with:
-          python-version: 3.7
-      - name: Install dependencies
+          python-version: "3.7"
+      - name: Install packages
         run: |
-          python -m pip install --upgrade pip
-          pip install -r requirements.txt
-          pip install wheel
-          python setup.py install
-      - name: Build package
+          make install
+      - name: Linting
         run: |
-          python setup.py sdist bdist_wheel
-      - name: Upload package to pypi
+          make lint
+      - name: Run tests
         run: |
-          twine upload dist/*
+          make test
+      - name: Send coverage to Coveralls
         env:
-          TWINE_USERNAME: ${{ secrets.pypi_username }}
-          TWINE_PASSWORD: ${{ secrets.pypi_password }}
-      - name: Build docs
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
-          cd docs
-          make html
-      - name: Deploy docs
-        uses: peaceiris/actions-gh-pages@v3
-        with:
-          github_token: ${{ secrets.GITHUB_TOKEN }}
-          publish_dir: ./docs/_build/html
-      - name: Notify Slack of pipeline completion
-        uses: 8398a7/action-slack@v2
+          coveralls --service=github
+
+  tox:
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        os: [ubuntu-latest, macos-latest, windows-latest]
+        python: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+    steps:
+      - uses: actions/checkout@v1
+      - name: Setup Python
+        uses: actions/setup-python@v2
         with:
-          status: ${{ job.status }}
-          author_name: Github Action
-        env:
-          GITHUB_TOKEN: ${{ secrets.github_slack_token }}
-          SLACK_WEBHOOK_URL: ${{ secrets.slack_webhook }}
-        if: always() 
+          python-version: ${{ matrix.python }}
+      - name: Install Tox and any other packages
+        run:  |
+          python -m pip install --upgrade pip
+          pip install tox
+      - name: Run Tox
+        run: tox -e py
```

### Comparing `UnleashClient-5.6.0/.gitignore` & `UnleashClient-5.7.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -93,17 +93,26 @@
 
 # Spyder project settings
 .spyderproject
 
 # Rope project settings
 .ropeproject
 
-#Custom
+# Custom
+
+# - IDEs
 .idea
 .vscode
-assets
+
+# - Linting
+.ruff_cache
+
+# - Testing
 results*
+tests/specification_tests/client-specification
+
+# - Docs
+assets
 site
 test_results
 _static
 _templates
-tests/specification_tests/client-specification
```

### Comparing `UnleashClient-5.6.0/CHANGELOG.md` & `UnleashClient-5.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+## Next
+* (Minor) Switch to ruff for linting and black for formatting.
+
 ## v5.6.0
 * (Major) Add support for event callbacks.
 
 ## v5.5.0
 * (Minor) SDK now warns when multiple instances are created
 * (Bugfix) Fix an issue where the NOT_IN operator behaves incorrectly when inverted and no context is passed
```

### Comparing `UnleashClient-5.6.0/CODE_OF_CONDUCT.md` & `UnleashClient-5.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/CONTRIBUTING.md` & `UnleashClient-5.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/LICENSE.md` & `UnleashClient-5.7.0/LICENSE.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### Comparing `UnleashClient-5.6.0/PKG-INFO` & `UnleashClient-5.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,127 @@
 Metadata-Version: 2.1
 Name: UnleashClient
-Version: 5.6.0
+Version: 5.7.0
 Summary: Python client for the Unleash feature toggle system!
-Home-page: https://github.com/Unleash/unleash-client-python
-Author: Ivan Lee
-Author-email: ivanklee86@gmail.com
-License: UNKNOWN
-Description: # unleash-client-python
-        
-        ![](https://github.com/unleash/unleash-client-python/workflows/CI/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/Unleash/unleash-client-python/badge.svg?branch=main)](https://coveralls.io/github/Unleash/unleash-client-python?branch=main) [![PyPI version](https://badge.fury.io/py/UnleashClient.svg)](https://badge.fury.io/py/UnleashClient) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/UnleashClient.svg) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        
-        This is the Python client for [Unleash](https://github.com/unleash/unleash).  It implements [Client Specifications 1.0](https://github.com/Unleash/unleash/blob/main/docs/client-specification.md) and checks compliance based on spec in [unleash/client-specifications](https://github.com/Unleash/client-specification)
-        
-        What it supports:
-        * Default activation strategies using 32-bit [Murmurhash3](https://en.wikipedia.org/wiki/MurmurHash)
-        * Custom strategies
-        * Full client lifecycle:
-            * Client registers with Unleash server
-            * Client periodically fetches feature toggles and stores to on-disk cache
-            * Client periodically sends metrics to Unleash Server
-        * Tested on Linux (Ubuntu), OSX, and Windows
-        
-        Check out the [project documentation](https://unleash.github.io/unleash-client-python/) and the [changelog](https://docs.getunleash.io/unleash-client-python/changelog.html).
-        
-        ## Installation
-        
-        Check out the package on [Pypi](https://pypi.org/project/UnleashClient/)!
-        
-        ```bash
-        pip install UnleashClient
-        ```
-        
-        ## For Flask Users
-        
-        If you're looking into running Unleash from Flask, you might want to take a look at [_Flask-Unleash_, the Unleash Flask extension](https://github.com/Unleash/Flask-Unleash). The extension builds upon this SDK to reduce the amount of boilerplate code you need to write to integrate with Flask. Of course, if you'd rather use this package directly, that will work too.
-        
-        ## Usage
-        
-        ### Initialization
-        
-        ```python
-        from UnleashClient import UnleashClient
-        
-        client = UnleashClient(
-            url="https://unleash.herokuapp.com",
-            app_name="my-python-app",
-            custom_headers={'Authorization': '<API token>'})
-        
-        client.initialize_client()
-        ```
-        
-        For more information about configuring `UnleashClient`, check out the [project reference docs](https://docs.getunleash.io/unleash-client-python/unleashclient.html)!
-        
-        ### Checking if a feature is enabled
-        
-        A check of a simple toggle:
-        ```python
-        client.is_enabled("my_toggle")
-        ```
-        
-        To supply application context, use the second positional argument:
-        
-        ```python
-        app_context = {"userId": "test@email.com"}
-        client.is_enabled("user_id_toggle", app_context)
-        ```
-        
-        #### Fallback function and default values
-        
-        You can specify a fallback function for cases where the client doesn't recognize the toggle by using the `fallback_function` keyword argument:
-        
-        ```python
-        def custom_fallback(feature_name: str, context: dict) -> bool:
-            return True
-        
-        client.is_enabled("my_toggle", fallback_function=custom_fallback)
-        ```
-        
-        You can also use the `fallback_function` argument to replace the obsolete `default_value` keyword argument by using a lambda that ignores its inputs. Whatever the lambda returns will be used as the default value.
-        
-        ```python
-        client.is_enabled("my_toggle", fallback_function=lambda feature_name, context: True)
-        ```
-        
-        The fallback function **must** accept the feature name and context as positional arguments in that order.
-        
-        The client will evaluate the fallback function only if an exception occurs when calling the `is_enabled()` method. This happens when the client can't find the feature flag. The client _may_ also throw other, general exceptions.
-        
-        For more information about usage, see the [Usage documentation](https://docs.getunleash.io/unleash-client-python/usage.html).
-        
-        ### Getting a variant
-        
-        Checking for a variant:
-        ```python
-        context = {'userId': '2'}  # Context must have userId, sessionId, or remoteAddr.  If none are present, distribution will be random.
-        
-        variant = client.get_variant("variant_toggle", context)
-        
-        print(variant)
-        > {
-        >    "name": "variant1",
-        >    "payload": {
-        >        "type": "string",
-        >        "value": "val1"
-        >        },
-        >    "enabled": True
-        > }
-        ```
-        
-        For more information about variants, see the [Variant documentation](https://docs.getunleash.io/advanced/toggle_variants).
-        
-Platform: UNKNOWN
+Author-email: Ivan Lee <ivanklee86@gmail.com>
+Project-URL: Homepage, https://github.com/Unleash/unleash-client-python
+Project-URL: Documentation, https://docs.getunleash.io/unleash-client-python
+Project-URL: Changelog, https://github.com/Unleash/unleash-client-python/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/Unleash/unleash-client-python
+Project-URL: Issues, https://github.com/Unleash/unleash-client-python/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# unleash-client-python
+
+![](https://github.com/unleash/unleash-client-python/workflows/CI/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/Unleash/unleash-client-python/badge.svg?branch=main)](https://coveralls.io/github/Unleash/unleash-client-python?branch=main) [![PyPI version](https://badge.fury.io/py/UnleashClient.svg)](https://badge.fury.io/py/UnleashClient) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/UnleashClient.svg) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+
+This is the Python client for [Unleash](https://github.com/unleash/unleash).  It implements [Client Specifications 1.0](https://github.com/Unleash/unleash/blob/main/docs/client-specification.md) and checks compliance based on spec in [unleash/client-specifications](https://github.com/Unleash/client-specification)
+
+What it supports:
+* Default activation strategies using 32-bit [Murmurhash3](https://en.wikipedia.org/wiki/MurmurHash)
+* Custom strategies
+* Full client lifecycle:
+    * Client registers with Unleash server
+    * Client periodically fetches feature toggles and stores to on-disk cache
+    * Client periodically sends metrics to Unleash Server
+* Tested on Linux (Ubuntu), OSX, and Windows
+
+Check out the [project documentation](https://unleash.github.io/unleash-client-python/) and the [changelog](https://docs.getunleash.io/unleash-client-python/changelog.html).
+
+## Installation
+
+Check out the package on [Pypi](https://pypi.org/project/UnleashClient/)!
+
+```bash
+pip install UnleashClient
+```
+
+## For Flask Users
+
+If you're looking into running Unleash from Flask, you might want to take a look at [_Flask-Unleash_, the Unleash Flask extension](https://github.com/Unleash/Flask-Unleash). The extension builds upon this SDK to reduce the amount of boilerplate code you need to write to integrate with Flask. Of course, if you'd rather use this package directly, that will work too.
+
+## Usage
+
+### Initialization
+
+```python
+from UnleashClient import UnleashClient
+
+client = UnleashClient(
+    url="https://unleash.herokuapp.com",
+    app_name="my-python-app",
+    custom_headers={'Authorization': '<API token>'})
+
+client.initialize_client()
+```
+
+For more information about configuring `UnleashClient`, check out the [project reference docs](https://docs.getunleash.io/unleash-client-python/unleashclient.html)!
+
+### Checking if a feature is enabled
+
+A check of a simple toggle:
+```python
+client.is_enabled("my_toggle")
+```
+
+To supply application context, use the second positional argument:
+
+```python
+app_context = {"userId": "test@email.com"}
+client.is_enabled("user_id_toggle", app_context)
+```
+
+#### Fallback function and default values
+
+You can specify a fallback function for cases where the client doesn't recognize the toggle by using the `fallback_function` keyword argument:
+
+```python
+def custom_fallback(feature_name: str, context: dict) -> bool:
+    return True
+
+client.is_enabled("my_toggle", fallback_function=custom_fallback)
+```
+
+You can also use the `fallback_function` argument to replace the obsolete `default_value` keyword argument by using a lambda that ignores its inputs. Whatever the lambda returns will be used as the default value.
+
+```python
+client.is_enabled("my_toggle", fallback_function=lambda feature_name, context: True)
+```
+
+The fallback function **must** accept the feature name and context as positional arguments in that order.
+
+The client will evaluate the fallback function only if an exception occurs when calling the `is_enabled()` method. This happens when the client can't find the feature flag. The client _may_ also throw other, general exceptions.
+
+For more information about usage, see the [Usage documentation](https://docs.getunleash.io/unleash-client-python/usage.html).
+
+### Getting a variant
+
+Checking for a variant:
+```python
+context = {'userId': '2'}  # Context must have userId, sessionId, or remoteAddr.  If none are present, distribution will be random.
+
+variant = client.get_variant("variant_toggle", context)
+
+print(variant)
+> {
+>    "name": "variant1",
+>    "payload": {
+>        "type": "string",
+>        "value": "val1"
+>        },
+>    "enabled": True
+> }
+```
+
+For more information about variants, see the [Variant documentation](https://docs.getunleash.io/advanced/toggle_variants).
```

### Comparing `UnleashClient-5.6.0/README.md` & `UnleashClient-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/UnleashClient/__init__.py` & `UnleashClient-5.7.0/UnleashClient/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,163 +1,193 @@
 # pylint: disable=invalid-name
-import warnings
 import random
 import string
 import uuid
+import warnings
 from datetime import datetime, timezone
 from typing import Callable, Optional
+
+from apscheduler.executors.pool import ThreadPoolExecutor
 from apscheduler.job import Job
-from apscheduler.schedulers.base import BaseScheduler
 from apscheduler.schedulers.background import BackgroundScheduler
+from apscheduler.schedulers.base import BaseScheduler
 from apscheduler.triggers.interval import IntervalTrigger
-from apscheduler.executors.pool import ThreadPoolExecutor
+
 from UnleashClient.api import register_client
-from UnleashClient.periodic_tasks import fetch_and_load_features, aggregate_and_send_metrics
-from UnleashClient.strategies import ApplicationHostname, Default, GradualRolloutRandom, \
-    GradualRolloutSessionId, GradualRolloutUserId, UserWithId, RemoteAddress, FlexibleRollout
-from UnleashClient.constants import METRIC_LAST_SENT_TIME, DISABLED_VARIATION, ETAG
-from UnleashClient.loader import load_features
+from UnleashClient.constants import DISABLED_VARIATION, ETAG, METRIC_LAST_SENT_TIME
 from UnleashClient.events import UnleashEvent, UnleashEventType
-from .utils import LOGGER, InstanceCounter, InstanceAllowType
-from .deprecation_warnings import strategy_v2xx_deprecation_check
-from .cache import BaseCache, FileCache
+from UnleashClient.features import Feature
+from UnleashClient.loader import load_features
+from UnleashClient.periodic_tasks import (
+    aggregate_and_send_metrics,
+    fetch_and_load_features,
+)
+from UnleashClient.strategies import (
+    ApplicationHostname,
+    Default,
+    FlexibleRollout,
+    GradualRolloutRandom,
+    GradualRolloutSessionId,
+    GradualRolloutUserId,
+    RemoteAddress,
+    UserWithId,
+)
 
+from .cache import BaseCache, FileCache
+from .deprecation_warnings import strategy_v2xx_deprecation_check
+from .utils import LOGGER, InstanceAllowType, InstanceCounter
 
 INSTANCES = InstanceCounter()
 
+
 # pylint: disable=dangerous-default-value
 class UnleashClient:
     """
     A client for the Unleash feature toggle system.
 
     :param url: URL of the unleash server, required.
     :param app_name: Name of the application using the unleash client, required.
-    :param  environment: Name of the environment using the unleash client, optional & defaults to "default".
+    :param environment: Name of the environment using the unleash client, optional & defaults to "default".
     :param instance_id: Unique identifier for unleash client instance, optional & defaults to "unleash-client-python"
     :param refresh_interval: Provisioning refresh interval in seconds, optional & defaults to 15 seconds
     :param refresh_jitter: Provisioning refresh interval jitter in seconds, optional & defaults to None
     :param metrics_interval: Metrics refresh interval in seconds, optional & defaults to 60 seconds
     :param metrics_jitter: Metrics refresh interval jitter in seconds, optional & defaults to None
     :param disable_metrics: Disables sending metrics to unleash server, optional & defaults to false.
+    :param disable_registration: Disables registration with unleash server, optional & defaults to false.
     :param custom_headers: Default headers to send to unleash server, optional & defaults to empty.
     :param custom_options: Default requests parameters, optional & defaults to empty.  Can be used to skip SSL verification.
     :param custom_strategies: Dictionary of custom strategy names : custom strategy objects.
     :param cache_directory: Location of the cache directory. When unset, FCache will determine the location.
     :param verbose_log_level: Numerical log level (https://docs.python.org/3/library/logging.html#logging-levels) for cases where checking a feature flag fails.
     :param cache: Custom cache implementation that extends UnleashClient.cache.BaseCache.  When unset, UnleashClient will use Fcache.
     :param scheduler: Custom APScheduler object.  Use this if you want to customize jobstore or executors.  When unset, UnleashClient will create it's own scheduler.
     :param scheduler_executor: Name of APSCheduler executor to use if using a custom scheduler.
     :param multiple_instance_mode: Determines how multiple instances being instantiated is handled by the SDK, when set to InstanceAllowType.BLOCK, the client constructor will fail when more than one instance is detected, when set to InstanceAllowType.WARN, multiple instances will be allowed but log a warning, when set to InstanceAllowType.SILENTLY_ALLOW, no warning or failure will be raised when instantiating multiple instances of the client. Defaults to InstanceAllowType.WARN
     :param event_callback: Function to call if impression events are enabled.  WARNING: Depending on your event library, this may have performance implications!
     """
-    def __init__(self,
-                 url: str,
-                 app_name: str,
-                 environment: str = "default",
-                 instance_id: str = "unleash-client-python",
-                 refresh_interval: int = 15,
-                 refresh_jitter: Optional[int] = None,
-                 metrics_interval: int = 60,
-                 metrics_jitter: Optional[int] = None,
-                 disable_metrics: bool = False,
-                 disable_registration: bool = False,
-                 custom_headers: Optional[dict] = None,
-                 custom_options: Optional[dict] = None,
-                 custom_strategies: Optional[dict] = None,
-                 cache_directory: Optional[str] = None,
-                 project_name: str = None,
-                 verbose_log_level: int = 30,
-                 cache: Optional[BaseCache] = None,
-                 scheduler: Optional[BaseScheduler] = None,
-                 scheduler_executor: Optional[str] = None,
-                 multiple_instance_mode: InstanceAllowType = InstanceAllowType.WARN,
-                 event_callback: Optional[Callable[[UnleashEvent], None]] = None) -> None:
+
+    def __init__(
+        self,
+        url: str,
+        app_name: str,
+        environment: str = "default",
+        instance_id: str = "unleash-client-python",
+        refresh_interval: int = 15,
+        refresh_jitter: Optional[int] = None,
+        metrics_interval: int = 60,
+        metrics_jitter: Optional[int] = None,
+        disable_metrics: bool = False,
+        disable_registration: bool = False,
+        custom_headers: Optional[dict] = None,
+        custom_options: Optional[dict] = None,
+        custom_strategies: Optional[dict] = None,
+        cache_directory: Optional[str] = None,
+        project_name: Optional[str] = None,
+        verbose_log_level: int = 30,
+        cache: Optional[BaseCache] = None,
+        scheduler: Optional[BaseScheduler] = None,
+        scheduler_executor: Optional[str] = None,
+        multiple_instance_mode: InstanceAllowType = InstanceAllowType.WARN,
+        event_callback: Optional[Callable[[UnleashEvent], None]] = None,
+    ) -> None:
         custom_headers = custom_headers or {}
         custom_options = custom_options or {}
         custom_strategies = custom_strategies or {}
 
         # Configuration
-        self.unleash_url = url.rstrip('/')
+        self.unleash_url = url.rstrip("/")
         self.unleash_app_name = app_name
         self.unleash_environment = environment
         self.unleash_instance_id = instance_id
         self.unleash_refresh_interval = refresh_interval
-        self.unleash_refresh_jitter = int(refresh_jitter) if refresh_jitter is not None else None
+        self.unleash_refresh_jitter = (
+            int(refresh_jitter) if refresh_jitter is not None else None
+        )
         self.unleash_metrics_interval = metrics_interval
-        self.unleash_metrics_jitter = int(metrics_jitter) if metrics_jitter is not None else None
+        self.unleash_metrics_jitter = (
+            int(metrics_jitter) if metrics_jitter is not None else None
+        )
         self.unleash_disable_metrics = disable_metrics
         self.unleash_disable_registration = disable_registration
         self.unleash_custom_headers = custom_headers
         self.unleash_custom_options = custom_options
         self.unleash_static_context = {
             "appName": self.unleash_app_name,
-            "environment": self.unleash_environment
+            "environment": self.unleash_environment,
         }
         self.unleash_project_name = project_name
         self.unleash_verbose_log_level = verbose_log_level
         self.unleash_event_callback = event_callback
 
         self._do_instance_check(multiple_instance_mode)
 
         # Class objects
         self.features: dict = {}
         self.fl_job: Job = None
         self.metric_job: Job = None
 
-        self.cache = cache or FileCache(self.unleash_app_name, directory=cache_directory)
-        self.cache.mset({
-            METRIC_LAST_SENT_TIME: datetime.now(timezone.utc),
-            ETAG: ''
-        })
+        self.cache = cache or FileCache(
+            self.unleash_app_name, directory=cache_directory
+        )
+        self.cache.mset({METRIC_LAST_SENT_TIME: datetime.now(timezone.utc), ETAG: ""})
         self.unleash_bootstrapped = self.cache.bootstrapped
 
         # Scheduler bootstrapping
         # - Figure out the Unleash executor name.
         if scheduler and scheduler_executor:
             self.unleash_executor_name = scheduler_executor
         elif scheduler and not scheduler_executor:
-            raise ValueError("If using a custom scheduler, you must specify a executor.")
+            raise ValueError(
+                "If using a custom scheduler, you must specify a executor."
+            )
         else:
-            if not scheduler:
-                LOGGER.warning("scheduler_executor should only be used with a custom scheduler.")
+            if not scheduler and scheduler_executor:
+                LOGGER.warning(
+                    "scheduler_executor should only be used with a custom scheduler."
+                )
 
             self.unleash_executor_name = f"unleash_executor_{''.join(random.choices(string.ascii_uppercase + string.digits, k=6))}"
 
         # Set up the scheduler.
         if scheduler:
             self.unleash_scheduler = scheduler
         else:
-            executors = {
-                self.unleash_executor_name: ThreadPoolExecutor()
-            }
+            executors = {self.unleash_executor_name: ThreadPoolExecutor()}
             self.unleash_scheduler = BackgroundScheduler(executors=executors)
 
         # Mappings
         default_strategy_mapping = {
             "applicationHostname": ApplicationHostname,
             "default": Default,
             "gradualRolloutRandom": GradualRolloutRandom,
             "gradualRolloutSessionId": GradualRolloutSessionId,
             "gradualRolloutUserId": GradualRolloutUserId,
             "remoteAddress": RemoteAddress,
             "userWithId": UserWithId,
-            "flexibleRollout": FlexibleRollout
+            "flexibleRollout": FlexibleRollout,
         }
 
         if custom_strategies:
-            strategy_v2xx_deprecation_check([x for x in custom_strategies.values()])  # pylint: disable=R1721
+            strategy_v2xx_deprecation_check(
+                [x for x in custom_strategies.values()]
+            )  # pylint: disable=R1721
 
         self.strategy_mapping = {**custom_strategies, **default_strategy_mapping}
 
         # Client status
         self.is_initialized = False
 
         # Bootstrapping
         if self.unleash_bootstrapped:
-            load_features(cache=self.cache, feature_toggles=self.features, strategy_mapping=self.strategy_mapping)
+            load_features(
+                cache=self.cache,
+                feature_toggles=self.features,
+                strategy_mapping=self.strategy_mapping,
+            )
 
     def initialize_client(self, fetch_toggles: bool = True) -> None:
         """
         Initializes client and starts communication with central unleash server(s).
 
         This kicks off:
 
@@ -189,22 +219,28 @@
                 metrics_args = {
                     "url": self.unleash_url,
                     "app_name": self.unleash_app_name,
                     "instance_id": self.unleash_instance_id,
                     "custom_headers": self.unleash_custom_headers,
                     "custom_options": self.unleash_custom_options,
                     "features": self.features,
-                    "cache": self.cache
+                    "cache": self.cache,
                 }
 
                 # Register app
                 if not self.unleash_disable_registration:
-                    register_client(self.unleash_url, self.unleash_app_name, self.unleash_instance_id,
-                                    self.unleash_metrics_interval, self.unleash_custom_headers,
-                                    self.unleash_custom_options, self.strategy_mapping)
+                    register_client(
+                        self.unleash_url,
+                        self.unleash_app_name,
+                        self.unleash_instance_id,
+                        self.unleash_metrics_interval,
+                        self.unleash_custom_headers,
+                        self.unleash_custom_options,
+                        self.strategy_mapping,
+                    )
 
                 if fetch_toggles:
                     job_args = {
                         "url": self.unleash_url,
                         "app_name": self.unleash_app_name,
                         "instance_id": self.unleash_instance_id,
                         "custom_headers": self.unleash_custom_headers,
@@ -222,66 +258,78 @@
                         "strategy_mapping": self.strategy_mapping,
                     }
                     job_func = load_features
 
                 job_func(**job_args)  # type: ignore
                 # Start periodic jobs
                 self.unleash_scheduler.start()
-                self.fl_job = self.unleash_scheduler.add_job(job_func,
-                                                     trigger=IntervalTrigger(
-                                                         seconds=int(self.unleash_refresh_interval),
-                                                         jitter=self.unleash_refresh_jitter,
-                                                     ),
-                                                     executor=self.unleash_executor_name,
-                                                     kwargs=job_args)
+                self.fl_job = self.unleash_scheduler.add_job(
+                    job_func,
+                    trigger=IntervalTrigger(
+                        seconds=int(self.unleash_refresh_interval),
+                        jitter=self.unleash_refresh_jitter,
+                    ),
+                    executor=self.unleash_executor_name,
+                    kwargs=job_args,
+                )
 
                 if not self.unleash_disable_metrics:
-                    self.metric_job = self.unleash_scheduler.add_job(aggregate_and_send_metrics,
-                                                             trigger=IntervalTrigger(
-                                                                 seconds=int(self.unleash_metrics_interval),
-                                                                 jitter=self.unleash_metrics_jitter,
-                                                             ),
-                                                             executor=self.unleash_executor_name,
-                                                             kwargs=metrics_args)
+                    self.metric_job = self.unleash_scheduler.add_job(
+                        aggregate_and_send_metrics,
+                        trigger=IntervalTrigger(
+                            seconds=int(self.unleash_metrics_interval),
+                            jitter=self.unleash_metrics_jitter,
+                        ),
+                        executor=self.unleash_executor_name,
+                        kwargs=metrics_args,
+                    )
             except Exception as excep:
                 # Log exceptions during initialization.  is_initialized will remain false.
-                LOGGER.warning("Exception during UnleashClient initialization: %s", excep)
+                LOGGER.warning(
+                    "Exception during UnleashClient initialization: %s", excep
+                )
                 raise excep
             else:
-                # Set is_iniialized to true if no exception is encountered.
+                # Set is_initialized to true if no exception is encountered.
                 self.is_initialized = True
         else:
-            warnings.warn("Attempted to initialize an Unleash Client instance that has already been initialized.")
+            warnings.warn(
+                "Attempted to initialize an Unleash Client instance that has already been initialized."
+            )
 
     def destroy(self) -> None:
         """
         Gracefully shuts down the Unleash client by stopping jobs, stopping the scheduler, and deleting the cache.
 
         You shouldn't need this too much!
         """
         self.fl_job.remove()
         if self.metric_job:
             self.metric_job.remove()
         self.unleash_scheduler.shutdown()
         self.cache.destroy()
 
     @staticmethod
-    def _get_fallback_value(fallback_function: Callable, feature_name: str, context: dict) -> bool:
+    def _get_fallback_value(
+        fallback_function: Callable, feature_name: str, context: dict
+    ) -> bool:
         if fallback_function:
             fallback_value = fallback_function(feature_name, context)
         else:
             fallback_value = False
 
         return fallback_value
 
     # pylint: disable=broad-except
-    def is_enabled(self,
-                   feature_name: str,
-                   context: Optional[dict] = None,
-                   fallback_function: Callable = None) -> bool:
+    def is_enabled(
+        self,
+        feature_name: str,
+        context: Optional[dict] = None,
+        fallback_function: Callable = None,
+    ) -> bool:
         """
         Checks if a feature toggle is enabled.
 
         Notes:
 
         * If client hasn't been initialized yet or an error occurs, flat will default to false.
 
@@ -298,43 +346,76 @@
         context = base_context
 
         if self.unleash_bootstrapped or self.is_initialized:
             try:
                 feature = self.features[feature_name]
                 feature_check = feature.is_enabled(context)
 
+                if feature.only_for_metrics:
+                    return self._get_fallback_value(
+                        fallback_function, feature_name, context
+                    )
+
                 try:
                     if self.unleash_event_callback and feature.impression_data:
                         event = UnleashEvent(
                             event_type=UnleashEventType.FEATURE_FLAG,
                             event_id=uuid.uuid4(),
                             context=context,
                             enabled=feature_check,
-                            feature_name=feature_name
+                            feature_name=feature_name,
                         )
 
                         self.unleash_event_callback(event)
                 except Exception as excep:
-                    LOGGER.log(self.unleash_verbose_log_level, "Error in event callback: %s", excep)
+                    LOGGER.log(
+                        self.unleash_verbose_log_level,
+                        "Error in event callback: %s",
+                        excep,
+                    )
                     return feature_check
 
                 return feature_check
             except Exception as excep:
-                LOGGER.log(self.unleash_verbose_log_level, "Returning default value for feature: %s", feature_name)
-                LOGGER.log(self.unleash_verbose_log_level, "Error checking feature flag: %s", excep)
-                return self._get_fallback_value(fallback_function, feature_name, context)
+                LOGGER.log(
+                    self.unleash_verbose_log_level,
+                    "Returning default value for feature: %s",
+                    feature_name,
+                )
+                LOGGER.log(
+                    self.unleash_verbose_log_level,
+                    "Error checking feature flag: %s",
+                    excep,
+                )
+                # The feature doesn't exist, so create it to track metrics
+                new_feature = Feature.metrics_only_feature(feature_name)
+                self.features[feature_name] = new_feature
+
+                # Use the feature's is_enabled method to count the call
+                new_feature.is_enabled(context)
+
+                return self._get_fallback_value(
+                    fallback_function, feature_name, context
+                )
+
         else:
-            LOGGER.log(self.unleash_verbose_log_level, "Returning default value for feature: %s", feature_name)
-            LOGGER.log(self.unleash_verbose_log_level, "Attempted to get feature_flag %s, but client wasn't initialized!", feature_name)
+            LOGGER.log(
+                self.unleash_verbose_log_level,
+                "Returning default value for feature: %s",
+                feature_name,
+            )
+            LOGGER.log(
+                self.unleash_verbose_log_level,
+                "Attempted to get feature_flag %s, but client wasn't initialized!",
+                feature_name,
+            )
             return self._get_fallback_value(fallback_function, feature_name, context)
 
     # pylint: disable=broad-except
-    def get_variant(self,
-                    feature_name: str,
-                    context: Optional[dict] = None) -> dict:
+    def get_variant(self, feature_name: str, context: Optional[dict] = None) -> dict:
         """
         Checks if a feature toggle is enabled.  If so, return variant.
 
         Notes:
 
         * If client hasn't been initialized yet or an error occurs, flat will default to false.
 
@@ -352,46 +433,76 @@
 
                 if self.unleash_event_callback and feature.impression_data:
                     try:
                         event = UnleashEvent(
                             event_type=UnleashEventType.VARIANT,
                             event_id=uuid.uuid4(),
                             context=context,
-                            enabled=variant_check['enabled'],
+                            enabled=variant_check["enabled"],
                             feature_name=feature_name,
-                            variant=variant_check['name']
+                            variant=variant_check["name"],
                         )
 
                         self.unleash_event_callback(event)
                     except Exception as excep:
-                        LOGGER.log(self.unleash_verbose_log_level, "Error in event callback: %s", excep)
+                        LOGGER.log(
+                            self.unleash_verbose_log_level,
+                            "Error in event callback: %s",
+                            excep,
+                        )
                         return variant_check
 
                 return variant_check
             except Exception as excep:
-                LOGGER.log(self.unleash_verbose_log_level, "Returning default flag/variation for feature: %s", feature_name)
-                LOGGER.log(self.unleash_verbose_log_level, "Error checking feature flag variant: %s", excep)
-                return DISABLED_VARIATION
+                LOGGER.log(
+                    self.unleash_verbose_log_level,
+                    "Returning default flag/variation for feature: %s",
+                    feature_name,
+                )
+                LOGGER.log(
+                    self.unleash_verbose_log_level,
+                    "Error checking feature flag variant: %s",
+                    excep,
+                )
+
+                # The feature doesn't exist, so create it to track metrics
+                new_feature = Feature.metrics_only_feature(feature_name)
+                self.features[feature_name] = new_feature
+
+                # Use the feature's get_variant method to count the call
+                return new_feature.get_variant(context)
         else:
-            LOGGER.log(self.unleash_verbose_log_level, "Returning default flag/variation for feature: %s", feature_name)
-            LOGGER.log(self.unleash_verbose_log_level, "Attempted to get feature flag/variation %s, but client wasn't initialized!", feature_name)
+            LOGGER.log(
+                self.unleash_verbose_log_level,
+                "Returning default flag/variation for feature: %s",
+                feature_name,
+            )
+            LOGGER.log(
+                self.unleash_verbose_log_level,
+                "Attempted to get feature flag/variation %s, but client wasn't initialized!",
+                feature_name,
+            )
             return DISABLED_VARIATION
 
     def _do_instance_check(self, multiple_instance_mode):
         identifier = self.__get_identifier()
         if identifier in INSTANCES:
             msg = f"You already have {INSTANCES.count(identifier)} instance(s) configured for this config: {identifier}, please double check the code where this client is being instantiated."
             if multiple_instance_mode == InstanceAllowType.BLOCK:
                 raise Exception(msg)  # pylint: disable=broad-exception-raised
             if multiple_instance_mode == InstanceAllowType.WARN:
                 LOGGER.error(msg)
         INSTANCES.increment(identifier)
 
     def __get_identifier(self):
-        api_key = self.unleash_custom_headers.get("Authorization") if self.unleash_custom_headers is not None else None
+        api_key = (
+            self.unleash_custom_headers.get("Authorization")
+            if self.unleash_custom_headers is not None
+            else None
+        )
         return f"apiKey:{api_key} appName:{self.unleash_app_name} instanceId:{self.unleash_instance_id}"
 
     def __enter__(self) -> "UnleashClient":
         self.initialize_client()
         return self
 
     def __exit__(self, *args, **kwargs):
```

### Comparing `UnleashClient-5.6.0/UnleashClient/api/features.py` & `UnleashClient-5.7.0/UnleashClient/api/features.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from typing import Tuple
+from typing import Optional, Tuple
+
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
-from UnleashClient.constants import REQUEST_TIMEOUT, FEATURES_URL, \
-    REQUEST_RETRIES
+from UnleashClient.constants import FEATURES_URL, REQUEST_RETRIES, REQUEST_TIMEOUT
 from UnleashClient.utils import LOGGER, log_resp_info
 
 
 # pylint: disable=broad-except
-def get_feature_toggles(url: str,
-                        app_name: str,
-                        instance_id: str,
-                        custom_headers: dict,
-                        custom_options: dict,
-                        project: str = None,
-                        cached_etag: str = '') -> Tuple[dict, str]:
+def get_feature_toggles(
+    url: str,
+    app_name: str,
+    instance_id: str,
+    custom_headers: dict,
+    custom_options: dict,
+    project: Optional[str] = None,
+    cached_etag: str = "",
+) -> Tuple[dict, str]:
     """
     Retrieves feature flags from unleash central server.
 
     Notes:
     * If unsuccessful (i.e. not HTTP status code 200), exception will be caught and logged.
       This is to allow "safe" error handling if unleash server goes down.
 
@@ -31,47 +33,55 @@
     :param project:
     :param cached_etag:
     :return: (Feature flags, etag) if successful, ({},'') if not
     """
     try:
         LOGGER.info("Getting feature flag.")
 
-        headers = {
-            "UNLEASH-APPNAME": app_name,
-            "UNLEASH-INSTANCEID": instance_id
-        }
+        headers = {"UNLEASH-APPNAME": app_name, "UNLEASH-INSTANCEID": instance_id}
 
         if cached_etag:
-            headers['If-None-Match'] = cached_etag
+            headers["If-None-Match"] = cached_etag
 
         base_url = f"{url}{FEATURES_URL}"
         base_params = {}
 
         if project:
-            base_params = {'project': project}
+            base_params = {"project": project}
 
-        adapter = HTTPAdapter(max_retries=Retry(total=REQUEST_RETRIES, status_forcelist=[500, 502, 504]))
+        adapter = HTTPAdapter(
+            max_retries=Retry(total=REQUEST_RETRIES, status_forcelist=[500, 502, 504])
+        )
         with requests.Session() as session:
             session.mount("https://", adapter)
             session.mount("http://", adapter)
-            resp = session.get(base_url,
-                               headers={**custom_headers, **headers},
-                               params=base_params,
-                               timeout=REQUEST_TIMEOUT, **custom_options)
+            resp = session.get(
+                base_url,
+                headers={**custom_headers, **headers},
+                params=base_params,
+                timeout=REQUEST_TIMEOUT,
+                **custom_options,
+            )
 
         if resp.status_code not in [200, 304]:
             log_resp_info(resp)
-            LOGGER.warning("Unleash Client feature fetch failed due to unexpected HTTP status code.")
-            raise Exception("Unleash Client feature fetch failed!")  # pylint: disable=broad-exception-raised
-
-        etag = ''
-        if 'etag' in resp.headers.keys():
-            etag = resp.headers['etag']
+            LOGGER.warning(
+                "Unleash Client feature fetch failed due to unexpected HTTP status code."
+            )
+            raise Exception(
+                "Unleash Client feature fetch failed!"
+            )  # pylint: disable=broad-exception-raised
+
+        etag = ""
+        if "etag" in resp.headers.keys():
+            etag = resp.headers["etag"]
 
         if resp.status_code == 304:
             return None, etag
 
         return resp.json(), etag
     except Exception as exc:
-        LOGGER.exception("Unleash Client feature fetch failed due to exception: %s", exc)
+        LOGGER.exception(
+            "Unleash Client feature fetch failed due to exception: %s", exc
+        )
 
-    return {}, ''
+    return {}, ""
```

### Comparing `UnleashClient-5.6.0/UnleashClient/api/metrics.py` & `UnleashClient-5.7.0/UnleashClient/api/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
+
 import requests
-from UnleashClient.constants import REQUEST_TIMEOUT, APPLICATION_HEADERS, METRICS_URL
+
+from UnleashClient.constants import APPLICATION_HEADERS, METRICS_URL, REQUEST_TIMEOUT
 from UnleashClient.utils import LOGGER, log_resp_info
 
 
 # pylint: disable=broad-except
-def send_metrics(url: str,
-                 request_body: dict,
-                 custom_headers: dict,
-                 custom_options: dict) -> bool:
+def send_metrics(
+    url: str, request_body: dict, custom_headers: dict, custom_options: dict
+) -> bool:
     """
     Attempts to send metrics to Unleash server
 
     Notes:
     * If unsuccessful (i.e. not HTTP status code 200), message will be logged
 
     :param url:
@@ -21,24 +22,29 @@
     :param custom_options:
     :return: true if registration successful, false if registration unsuccessful or exception.
     """
     try:
         LOGGER.info("Sending messages to with unleash @ %s", url)
         LOGGER.info("unleash metrics information: %s", request_body)
 
-        resp = requests.post(url + METRICS_URL,
-                             data=json.dumps(request_body),
-                             headers={**custom_headers, **APPLICATION_HEADERS},
-                             timeout=REQUEST_TIMEOUT, **custom_options)
+        resp = requests.post(
+            url + METRICS_URL,
+            data=json.dumps(request_body),
+            headers={**custom_headers, **APPLICATION_HEADERS},
+            timeout=REQUEST_TIMEOUT,
+            **custom_options,
+        )
 
         if resp.status_code != 202:
             log_resp_info(resp)
             LOGGER.warning("Unleash CLient metrics submission failed.")
             return False
 
         LOGGER.info("Unleash Client metrics successfully sent!")
 
         return True
     except requests.RequestException as exc:
-        LOGGER.warning("Unleash Client metrics submission failed due to exception: %s", exc)
+        LOGGER.warning(
+            "Unleash Client metrics submission failed due to exception: %s", exc
+        )
 
     return False
```

### Comparing `UnleashClient-5.6.0/UnleashClient/api/register.py` & `UnleashClient-5.7.0/UnleashClient/api/register.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 import json
 from datetime import datetime, timezone
+
 import requests
-from requests.exceptions import MissingSchema, InvalidSchema, InvalidURL, InvalidHeader
-from UnleashClient.constants import SDK_NAME, SDK_VERSION, REQUEST_TIMEOUT, APPLICATION_HEADERS, REGISTER_URL
+from requests.exceptions import InvalidHeader, InvalidSchema, InvalidURL, MissingSchema
+
+from UnleashClient.constants import (
+    APPLICATION_HEADERS,
+    REGISTER_URL,
+    REQUEST_TIMEOUT,
+    SDK_NAME,
+    SDK_VERSION,
+)
 from UnleashClient.utils import LOGGER, log_resp_info
 
 
 # pylint: disable=broad-except
-def register_client(url: str,
-                    app_name: str,
-                    instance_id: str,
-                    metrics_interval: int,
-                    custom_headers: dict,
-                    custom_options: dict,
-                    supported_strategies: dict) -> bool:
+def register_client(
+    url: str,
+    app_name: str,
+    instance_id: str,
+    metrics_interval: int,
+    custom_headers: dict,
+    custom_options: dict,
+    supported_strategies: dict,
+) -> bool:
     """
     Attempts to register client with unleash server.
 
     Notes:
     * If unsuccessful (i.e. not HTTP status code 202), exception will be caught and logged.
       This is to allow "safe" error handling if unleash server goes down.
 
@@ -32,34 +42,41 @@
     """
     registation_request = {
         "appName": app_name,
         "instanceId": instance_id,
         "sdkVersion": f"{SDK_NAME}:{SDK_VERSION}",
         "strategies": [*supported_strategies],
         "started": datetime.now(timezone.utc).isoformat(),
-        "interval": metrics_interval
+        "interval": metrics_interval,
     }
 
     try:
         LOGGER.info("Registering unleash client with unleash @ %s", url)
         LOGGER.info("Registration request information: %s", registation_request)
 
-        resp = requests.post(url + REGISTER_URL,
-                             data=json.dumps(registation_request),
-                             headers={**custom_headers, **APPLICATION_HEADERS},
-                             timeout=REQUEST_TIMEOUT, **custom_options)
+        resp = requests.post(
+            url + REGISTER_URL,
+            data=json.dumps(registation_request),
+            headers={**custom_headers, **APPLICATION_HEADERS},
+            timeout=REQUEST_TIMEOUT,
+            **custom_options,
+        )
 
         if resp.status_code != 202:
             log_resp_info(resp)
-            LOGGER.warning("Unleash Client registration failed due to unexpected HTTP status code.")
+            LOGGER.warning(
+                "Unleash Client registration failed due to unexpected HTTP status code."
+            )
             return False
 
         LOGGER.info("Unleash Client successfully registered!")
 
         return True
     except (MissingSchema, InvalidSchema, InvalidHeader, InvalidURL) as exc:
-        LOGGER.exception("Unleash Client registration failed fatally due to exception: %s", exc)
+        LOGGER.exception(
+            "Unleash Client registration failed fatally due to exception: %s", exc
+        )
         raise exc
     except requests.RequestException as exc:
         LOGGER.exception("Unleash Client registration failed due to exception: %s", exc)
 
     return False
```

### Comparing `UnleashClient-5.6.0/UnleashClient/cache.py` & `UnleashClient-5.7.0/UnleashClient/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import abc
 import json
 from pathlib import Path
 from typing import Any, Optional
 
 import requests
 from fcache.cache import FileCache as _FileCache
+
 from UnleashClient.constants import FEATURES_URL, REQUEST_TIMEOUT
 
 
 class BaseCache(abc.ABC):
     """
     Abstract base class for caches used for UnleashClient.
 
     If implementing your own bootstrapping methods:
 
     - Add your custom bootstrap method.
     - You must set the `bootstrapped` attribute to True after configuration is set.
     """
+
     bootstrapped = False
 
     @abc.abstractmethod
     def set(self, key: str, value: Any):
         pass
 
     @abc.abstractmethod
@@ -61,20 +63,21 @@
         from UnleashClient import UnleashClient
 
         my_cache = FileCache("HAMSTER_API")
         my_cache.bootstrap_from_file(Path("/path/to/boostrap.json"))
         unleash_client = UnleashClient(
             "https://my.unleash.server.com",
             "HAMSTER_API",
-            cache=cache
+            cache=my_cache
         )
 
     :param name: Name of cache.
     :param directory: Location to create cache.  If empty, will use filecache default.
     """
+
     def __init__(self, name: str, directory: Optional[str] = None):
         self._cache = _FileCache(name, app_cache_dir=directory)
 
     def bootstrap_from_dict(self, initial_config: dict) -> None:
         """
         Loads initial Unleash configuration from a dictionary.
 
@@ -89,28 +92,32 @@
         """
         Loads initial Unleash configuration from a file.
 
         Note: Pre-seeded configuration will only be used if UnleashClient is initialized with `bootstrap=true`.
 
         :param initial_configuration_file: Path to document containing initial configuration.  Must be JSON.
         """
-        with open(initial_config_file, "r",  encoding="utf8") as bootstrap_file:
+        with open(initial_config_file, "r", encoding="utf8") as bootstrap_file:
             self.set(FEATURES_URL, json.loads(bootstrap_file.read()))
             self.bootstrapped = True
 
-    def bootstrap_from_url(self, initial_config_url: str, headers: Optional[dict] = None) -> None:
+    def bootstrap_from_url(
+        self, initial_config_url: str, headers: Optional[dict] = None
+    ) -> None:
         """
         Loads initial Unleash configuration from a url.
 
         Note: Pre-seeded configuration will only be used if UnleashClient is initialized with `bootstrap=true`.
 
         :param initial_configuration_url: Url that returns document containing initial configuration.  Must return JSON.
         :param headers: Headers to use when GETing the initial configuration URL.
         """
-        response = requests.get(initial_config_url, headers=headers, timeout=REQUEST_TIMEOUT)
+        response = requests.get(
+            initial_config_url, headers=headers, timeout=REQUEST_TIMEOUT
+        )
         self.set(FEATURES_URL, response.json())
         self.bootstrapped = True
 
     def set(self, key: str, value: Any):
         self._cache[key] = value
         self._cache.sync()
```

### Comparing `UnleashClient-5.6.0/UnleashClient/constants.py` & `UnleashClient-5.7.0/UnleashClient/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 SDK_VERSION = version("UnleashClient")
 REQUEST_TIMEOUT = 30
 REQUEST_RETRIES = 3
 METRIC_LAST_SENT_TIME = "mlst"
 CLIENT_SPEC_VERSION = "4.2.2"
 
 # =Unleash=
-APPLICATION_HEADERS = {"Content-Type": "application/json", "Unleash-Client-Spec": CLIENT_SPEC_VERSION}
-DISABLED_VARIATION = {
-    'name': 'disabled',
-    'enabled': False
+APPLICATION_HEADERS = {
+    "Content-Type": "application/json",
+    "Unleash-Client-Spec": CLIENT_SPEC_VERSION,
 }
+DISABLED_VARIATION = {"name": "disabled", "enabled": False}
 
 # Paths
 REGISTER_URL = "/client/register"
 FEATURES_URL = "/client/features"
 METRICS_URL = "/client/metrics"
 
 # Cache keys
-FAILED_STRATEGIES = 'failed_strategies'
-ETAG = 'etag'
+FAILED_STRATEGIES = "failed_strategies"
+ETAG = "etag"
```

### Comparing `UnleashClient-5.6.0/UnleashClient/constraints/Constraint.py` & `UnleashClient-5.7.0/UnleashClient/constraints/Constraint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # pylint: disable=invalid-name, too-few-public-methods, use-a-generator
-from typing import Optional, Union
 from datetime import datetime
 from enum import Enum
-from dateutil.parser import parse, ParserError
+from typing import Optional, Union
+
 import semver
+from dateutil.parser import ParserError, parse
+
 from UnleashClient.utils import LOGGER, get_identifier
 
 
 class ConstraintOperators(Enum):
     # Logical operators
     IN = "IN"
     NOT_IN = "NOT_IN"
@@ -37,22 +39,35 @@
 class Constraint:
     def __init__(self, constraint_dict: dict) -> None:
         """
         Represents a constraint on a strategy
 
         :param constraint_dict: From the strategy document.
         """
-        self.context_name: str = constraint_dict['contextName']
-        self.operator: ConstraintOperators = ConstraintOperators(constraint_dict['operator'].upper())
-        self.values = constraint_dict['values'] if 'values' in constraint_dict.keys() else []
-        self.value = constraint_dict['value'] if 'value' in constraint_dict.keys() else None
-
-        self.case_insensitive = constraint_dict['caseInsensitive'] if 'caseInsensitive' in constraint_dict.keys() else False
-        self.inverted = constraint_dict['inverted'] if 'inverted' in constraint_dict.keys() else False
-
+        self.context_name: str = constraint_dict["contextName"]
+        self.operator: ConstraintOperators = ConstraintOperators(
+            constraint_dict["operator"].upper()
+        )
+        self.values = (
+            constraint_dict["values"] if "values" in constraint_dict.keys() else []
+        )
+        self.value = (
+            constraint_dict["value"] if "value" in constraint_dict.keys() else None
+        )
+
+        self.case_insensitive = (
+            constraint_dict["caseInsensitive"]
+            if "caseInsensitive" in constraint_dict.keys()
+            else False
+        )
+        self.inverted = (
+            constraint_dict["inverted"]
+            if "inverted" in constraint_dict.keys()
+            else False
+        )
 
     # Methods to handle each operator type.
     def check_list_operators(self, context_value: str) -> bool:
         return_value = False
 
         if self.operator == ConstraintOperators.IN:
             return_value = context_value in self.values
@@ -68,19 +83,25 @@
         else:
             normalized_values = self.values
             normalized_context_value = context_value
 
         return_value = False
 
         if self.operator == ConstraintOperators.STR_CONTAINS:
-            return_value = any([x in normalized_context_value for x in normalized_values])
+            return_value = any(
+                [x in normalized_context_value for x in normalized_values]
+            )
         elif self.operator == ConstraintOperators.STR_ENDS_WITH:
-            return_value = any([normalized_context_value.endswith(x) for x in normalized_values])
+            return_value = any(
+                [normalized_context_value.endswith(x) for x in normalized_values]
+            )
         elif self.operator == ConstraintOperators.STR_STARTS_WITH:
-            return_value = any([normalized_context_value.startswith(x) for x in normalized_values])
+            return_value = any(
+                [normalized_context_value.startswith(x) for x in normalized_values]
+            )
 
         return return_value
 
     def check_numeric_operators(self, context_value: Union[float, int]) -> bool:
         return_value = False
 
         parsed_value = float(self.value)
@@ -94,15 +115,14 @@
             return_value = parsed_context >= parsed_value
         elif self.operator == ConstraintOperators.NUM_LT:
             return_value = parsed_context < parsed_value
         elif self.operator == ConstraintOperators.NUM_LTE:
             return_value = parsed_context <= parsed_value
         return return_value
 
-
     def check_date_operators(self, context_value: Union[datetime, str]) -> bool:
         return_value = False
         parsing_exception = False
 
         try:
             parsed_date = parse(self.value)
             if isinstance(context_value, str):
@@ -117,15 +137,14 @@
             if self.operator == ConstraintOperators.DATE_AFTER:
                 return_value = context_date > parsed_date
             elif self.operator == ConstraintOperators.DATE_BEFORE:
                 return_value = context_date < parsed_date
 
         return return_value
 
-
     def check_semver_operators(self, context_value: str) -> bool:
         return_value = False
         parsing_exception = False
         target_version: Optional[semver.VersionInfo] = None
         context_version: Optional[semver.VersionInfo] = None
 
         try:
@@ -146,15 +165,14 @@
             elif self.operator == ConstraintOperators.SEMVER_GT:
                 return_value = context_version > target_version
             elif self.operator == ConstraintOperators.SEMVER_LT:
                 return_value = context_version < target_version
 
         return return_value
 
-
     def apply(self, context: dict = None) -> bool:
         """
         Returns true/false depending on constraint provisioning and context.
 
         :param context: Context information
         :return:
         """
@@ -164,26 +182,58 @@
             context_value = get_identifier(self.context_name, context)
 
             # Set currentTime if not specified
             if self.context_name == "currentTime" and not context_value:
                 context_value = datetime.now()
 
             if context_value is not None:
-                if self.operator in [ConstraintOperators.IN, ConstraintOperators.NOT_IN]:
-                    constraint_check = self.check_list_operators(context_value=context_value)
-                elif self.operator in [ConstraintOperators.STR_CONTAINS, ConstraintOperators.STR_ENDS_WITH, ConstraintOperators.STR_STARTS_WITH]:
-                    constraint_check = self.check_string_operators(context_value=context_value)
-                elif self.operator in [ConstraintOperators.NUM_EQ, ConstraintOperators.NUM_GT, ConstraintOperators.NUM_GTE, ConstraintOperators.NUM_LT, ConstraintOperators.NUM_LTE]:
-                    constraint_check = self.check_numeric_operators(context_value=context_value)
-                elif self.operator in [ConstraintOperators.DATE_AFTER, ConstraintOperators.DATE_BEFORE]:
-                    constraint_check = self.check_date_operators(context_value=context_value)
-                elif self.operator in [ConstraintOperators.SEMVER_EQ, ConstraintOperators.SEMVER_GT, ConstraintOperators.SEMVER_LT]:
-                    constraint_check = self.check_semver_operators(context_value=context_value)
+                if self.operator in [
+                    ConstraintOperators.IN,
+                    ConstraintOperators.NOT_IN,
+                ]:
+                    constraint_check = self.check_list_operators(
+                        context_value=context_value
+                    )
+                elif self.operator in [
+                    ConstraintOperators.STR_CONTAINS,
+                    ConstraintOperators.STR_ENDS_WITH,
+                    ConstraintOperators.STR_STARTS_WITH,
+                ]:
+                    constraint_check = self.check_string_operators(
+                        context_value=context_value
+                    )
+                elif self.operator in [
+                    ConstraintOperators.NUM_EQ,
+                    ConstraintOperators.NUM_GT,
+                    ConstraintOperators.NUM_GTE,
+                    ConstraintOperators.NUM_LT,
+                    ConstraintOperators.NUM_LTE,
+                ]:
+                    constraint_check = self.check_numeric_operators(
+                        context_value=context_value
+                    )
+                elif self.operator in [
+                    ConstraintOperators.DATE_AFTER,
+                    ConstraintOperators.DATE_BEFORE,
+                ]:
+                    constraint_check = self.check_date_operators(
+                        context_value=context_value
+                    )
+                elif self.operator in [
+                    ConstraintOperators.SEMVER_EQ,
+                    ConstraintOperators.SEMVER_GT,
+                    ConstraintOperators.SEMVER_LT,
+                ]:
+                    constraint_check = self.check_semver_operators(
+                        context_value=context_value
+                    )
             else:
                 # This is a special case in the client spec - so it's getting it's own handler here
-                if self.operator is ConstraintOperators.NOT_IN:
+                if self.operator is ConstraintOperators.NOT_IN:  # noqa: PLR5501
                     constraint_check = True
 
         except Exception as excep:  # pylint: disable=broad-except
-            LOGGER.info("Could not evaluate context %s!  Error: %s", self.context_name, excep)
+            LOGGER.info(
+                "Could not evaluate context %s!  Error: %s", self.context_name, excep
+            )
 
         return not constraint_check if self.inverted else constraint_check
```

### Comparing `UnleashClient-5.6.0/UnleashClient/deprecation_warnings.py` & `UnleashClient-5.7.0/UnleashClient/deprecation_warnings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import warnings
+
 from UnleashClient.strategies import Strategy
 
 
 def strategy_v2xx_deprecation_check(strategies: list) -> None:
     """
     Notify users of backwards incompatible changes in v3 for custom strategies.
     """
     for strategy in strategies:
         try:
             # Check if the __call__() method is overwritten (should only be true for custom strategies in v1.x or v2.x.
             if strategy.__call__ != Strategy.__call__:
                 warnings.warn(
                     f"unleash-client-python v3.x.x requires overriding the execute() method instead of the __call__() method. Error in: {strategy.__name__}",
-                    DeprecationWarning
+                    DeprecationWarning,
                 )
         except AttributeError:
             # Ignore if not.
             pass
```

### Comparing `UnleashClient-5.6.0/UnleashClient/events.py` & `UnleashClient-5.7.0/UnleashClient/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from typing import Optional
 from dataclasses import dataclass
 from enum import Enum
+from typing import Optional
 from uuid import UUID
 
 
 class UnleashEventType(Enum):
     """
     Indicates what kind of event was triggered.
     """
+
     FEATURE_FLAG = "feature_flag"
     VARIANT = "variant"
 
 
 @dataclass
 class UnleashEvent:
     """
     Dataclass capturing information from an Unleash feature flag or variant check.
     """
+
     event_type: UnleashEventType
     event_id: UUID
     context: dict
     enabled: bool
     feature_name: str
-    variant: Optional[str] = ''
+    variant: Optional[str] = ""
```

### Comparing `UnleashClient-5.6.0/UnleashClient/features/Feature.py` & `UnleashClient-5.7.0/UnleashClient/features/Feature.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # pylint: disable=invalid-name
-from typing import Optional
+from typing import Dict, Optional, cast
 
-from UnleashClient.variants import Variants
-from UnleashClient.utils import LOGGER
 from UnleashClient.constants import DISABLED_VARIATION
+from UnleashClient.utils import LOGGER
+from UnleashClient.variants import Variants
 
 
 # pylint: disable=dangerous-default-value, broad-except
 class Feature:
-    def __init__(self,
-                 name: str,
-                 enabled: bool,
-                 strategies: list,
-                 variants: Optional[Variants] = None,
-                 impression_data: bool = False) -> None:
+    def __init__(
+        self,
+        name: str,
+        enabled: bool,
+        strategies: list,
+        variants: Optional[Variants] = None,
+        impression_data: bool = False,
+    ) -> None:
         """
         A representation of a feature object
 
         :param name: Name of the feature.
         :param enabled: Whether feature is enabled.
         :param strategies: List of sub-classed Strategy objects representing feature strategies.
         :param impression_data: Whether impression data is enabled.
@@ -30,39 +32,54 @@
 
         # Additional information
         self.impression_data = impression_data
 
         # Stats tracking
         self.yes_count = 0
         self.no_count = 0
+        ## { [ variant name ]: number }
+        self.variant_counts: Dict[str, int] = {}
+
+        # Whether the feature exists only for tracking metrics or not.
+        self.only_for_metrics = False
 
     def reset_stats(self) -> None:
         """
         Resets stats after metrics reporting
 
         :return:
         """
         self.yes_count = 0
         self.no_count = 0
+        self.variant_counts = {}
 
     def increment_stats(self, result: bool) -> None:
         """
         Increments stats.
 
         :param result:
         :return:
         """
         if result:
             self.yes_count += 1
         else:
             self.no_count += 1
 
-    def is_enabled(self,
-                   context: dict = None,
-                   default_value: bool = False) -> bool:  # pylint: disable=unused-argument
+    def _count_variant(self, variant_name: str) -> None:
+        """
+        Count a specific variant.
+
+        :param variant_name: The name of the variant to count.
+        :return:
+        """
+        self.variant_counts[variant_name] = self.variant_counts.get(variant_name, 0) + 1
+
+    def is_enabled(
+        self, context: dict = None, default_value: bool = False
+    ) -> bool:  # pylint: disable=unused-argument
         """
         Checks if feature is enabled.
 
         :param context: Context information
         :param default_value: Deprecated!  Users should use the fallback_function on the main is_enabled() method.
         :return:
         """
@@ -82,26 +99,32 @@
 
         self.increment_stats(flag_value)
 
         LOGGER.info("Feature toggle status for feature %s: %s", self.name, flag_value)
 
         return flag_value
 
-    def get_variant(self,
-                    context: dict = None) -> dict:
+    def get_variant(self, context: dict = None) -> dict:
         """
         Checks if feature is enabled and, if so, get the variant.
 
         :param context: Context information
         :return:
         """
         variant = DISABLED_VARIATION
         is_feature_enabled = self.is_enabled(context)
 
         if is_feature_enabled and self.variants is not None:
             try:
                 variant = self.variants.get_variant(context)
-                variant['enabled'] = is_feature_enabled
+                variant["enabled"] = is_feature_enabled
             except Exception as variant_exception:
                 LOGGER.warning("Error selecting variant: %s", variant_exception)
 
+        self._count_variant(cast(str, variant["name"]))
         return variant
+
+    @staticmethod
+    def metrics_only_feature(feature_name: str):
+        feature = Feature(feature_name, False, [])
+        feature.only_for_metrics = True
+        return feature
```

### Comparing `UnleashClient-5.6.0/UnleashClient/loader.py` & `UnleashClient-5.7.0/UnleashClient/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,94 +1,113 @@
 from typing import Optional
+
+from UnleashClient.cache import BaseCache
+from UnleashClient.constants import FAILED_STRATEGIES, FEATURES_URL
 from UnleashClient.features.Feature import Feature
-from UnleashClient.variants.Variants import Variants
-from UnleashClient.constants import FEATURES_URL, FAILED_STRATEGIES
 from UnleashClient.utils import LOGGER
-from UnleashClient.cache import BaseCache
+from UnleashClient.variants.Variants import Variants
 
 
 # pylint: disable=broad-except
-def _create_strategies(provisioning: dict,
-                       strategy_mapping: dict,
-                       cache: BaseCache,
-                       global_segments: Optional[dict]) -> list:
+def _create_strategies(
+    provisioning: dict,
+    strategy_mapping: dict,
+    cache: BaseCache,
+    global_segments: Optional[dict],
+) -> list:
     feature_strategies = []
 
     for strategy in provisioning["strategies"]:
         try:
             if "parameters" in strategy.keys():
-                strategy_provisioning = strategy['parameters']
+                strategy_provisioning = strategy["parameters"]
             else:
                 strategy_provisioning = {}
 
             if "constraints" in strategy.keys():
-                constraint_provisioning = strategy['constraints']
+                constraint_provisioning = strategy["constraints"]
             else:
                 constraint_provisioning = {}
 
             if "segments" in strategy.keys():
-                segment_provisioning = strategy['segments']
+                segment_provisioning = strategy["segments"]
             else:
                 segment_provisioning = []
 
-            feature_strategies.append(strategy_mapping[strategy['name']](
-                constraints=constraint_provisioning, parameters=strategy_provisioning, global_segments=global_segments, segment_ids=segment_provisioning
-            ))
+            feature_strategies.append(
+                strategy_mapping[strategy["name"]](
+                    constraints=constraint_provisioning,
+                    parameters=strategy_provisioning,
+                    global_segments=global_segments,
+                    segment_ids=segment_provisioning,
+                )
+            )
         except Exception as excep:
             strategies = cache.get(FAILED_STRATEGIES, [])
 
-            if strategy['name'] not in strategies:
-                LOGGER.warning("Failed to load strategy. This may be a problem with a custom strategy. Exception: %s", excep)
-                strategies.append(strategy['name'])
+            if strategy["name"] not in strategies:
+                LOGGER.warning(
+                    "Failed to load strategy. This may be a problem with a custom strategy. Exception: %s",
+                    excep,
+                )
+                strategies.append(strategy["name"])
 
             cache.set(FAILED_STRATEGIES, strategies)
 
     return feature_strategies
 
 
-def _create_feature(provisioning: dict,
-                    strategy_mapping: dict,
-                    cache: BaseCache,
-                    global_segments: Optional[dict]) -> Feature:
+def _create_feature(
+    provisioning: dict,
+    strategy_mapping: dict,
+    cache: BaseCache,
+    global_segments: Optional[dict],
+) -> Feature:
     if "strategies" in provisioning.keys():
-        parsed_strategies = _create_strategies(provisioning, strategy_mapping, cache, global_segments)
+        parsed_strategies = _create_strategies(
+            provisioning, strategy_mapping, cache, global_segments
+        )
     else:
         parsed_strategies = []
 
     if "variants" in provisioning:
-        variant = Variants(provisioning['variants'], provisioning['name'])
+        variant = Variants(provisioning["variants"], provisioning["name"])
     else:
         variant = None
 
     return Feature(
         name=provisioning["name"],
         enabled=provisioning["enabled"],
         strategies=parsed_strategies,
         variants=variant,
         impression_data=provisioning.get("impressionData", False),
     )
 
 
-def load_features(cache: BaseCache,
-                  feature_toggles: dict,
-                  strategy_mapping: dict,
-                  global_segments: Optional[dict] = None) -> None:
+def load_features(
+    cache: BaseCache,
+    feature_toggles: dict,
+    strategy_mapping: dict,
+    global_segments: Optional[dict] = None,
+) -> None:
     """
     Caching
 
     :param cache: Should be the cache class variable from UnleashClient
     :param feature_toggles: Should be the features class variable from UnleashClient
     :param strategy_mapping:
     :return:
     """
     # Pull raw provisioning from cache.
     feature_provisioning = cache.get(FEATURES_URL)
     if not feature_provisioning:
-        LOGGER.warning("Unleash client does not have cached features. "
-                       "Please make sure client can communicate with Unleash server!")
+        LOGGER.warning(
+            "Unleash client does not have cached features. "
+            "Please make sure client can communicate with Unleash server!"
+        )
         return
 
     # Parse provisioning
     parsed_features = {}
     feature_names = [d["name"] for d in feature_provisioning["features"]]
 
     if "segments" in feature_provisioning.keys():
@@ -108,23 +127,33 @@
     # Update existing objects
     for feature in feature_toggles.keys():
         feature_for_update = feature_toggles[feature]
         strategies = parsed_features[feature]["strategies"]
 
         feature_for_update.enabled = parsed_features[feature]["enabled"]
         if strategies:
-            parsed_strategies = _create_strategies(parsed_features[feature], strategy_mapping, cache, global_segments)
+            parsed_strategies = _create_strategies(
+                parsed_features[feature], strategy_mapping, cache, global_segments
+            )
             feature_for_update.strategies = parsed_strategies
 
-        if 'variants' in parsed_features[feature]:
+        if "variants" in parsed_features[feature]:
             feature_for_update.variants = Variants(
-                parsed_features[feature]['variants'],
-                parsed_features[feature]['name']
+                parsed_features[feature]["variants"], parsed_features[feature]["name"]
             )
 
-        feature_for_update.impression_data = parsed_features[feature].get("impressionData", False)
+        feature_for_update.impression_data = parsed_features[feature].get(
+            "impressionData", False
+        )
+
+        # If the feature had previously been added to the features list only for
+        # tracking, indicate that it is now a real feature that should be
+        # evaluated properly.
+        feature_for_update.only_for_metrics = False
 
     # Handle creation or deletions
     new_features = list(set(feature_names) - set(feature_toggles.keys()))
 
     for feature in new_features:
-        feature_toggles[feature] = _create_feature(parsed_features[feature], strategy_mapping, cache, global_segments)
+        feature_toggles[feature] = _create_feature(
+            parsed_features[feature], strategy_mapping, cache, global_segments
+        )
```

### Comparing `UnleashClient-5.6.0/UnleashClient/periodic_tasks/fetch_and_load.py` & `UnleashClient-5.7.0/UnleashClient/periodic_tasks/fetch_and_load.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+from typing import Optional
+
 from UnleashClient.api import get_feature_toggles
+from UnleashClient.cache import BaseCache
+from UnleashClient.constants import ETAG, FEATURES_URL
 from UnleashClient.loader import load_features
-from UnleashClient.constants import FEATURES_URL, ETAG
 from UnleashClient.utils import LOGGER
-from UnleashClient.cache import BaseCache
 
 
-def fetch_and_load_features(url: str,
-                            app_name: str,
-                            instance_id: str,
-                            custom_headers: dict,
-                            custom_options: dict,
-                            cache: BaseCache,
-                            features: dict,
-                            strategy_mapping: dict,
-                            project: str = None) -> None:
+def fetch_and_load_features(
+    url: str,
+    app_name: str,
+    instance_id: str,
+    custom_headers: dict,
+    custom_options: dict,
+    cache: BaseCache,
+    features: dict,
+    strategy_mapping: dict,
+    project: Optional[str] = None,
+) -> None:
     (feature_provisioning, etag) = get_feature_toggles(
         url,
         app_name,
         instance_id,
         custom_headers,
         custom_options,
         project,
-        cache.get(ETAG)
+        cache.get(ETAG),
     )
 
     if feature_provisioning:
         cache.set(FEATURES_URL, feature_provisioning)
     else:
-        LOGGER.debug("No feature provisioning returned from server, using cached provisioning.")
+        LOGGER.debug(
+            "No feature provisioning returned from server, using cached provisioning."
+        )
 
     if etag:
         cache.set(ETAG, etag)
 
     load_features(cache, features, strategy_mapping)
```

### Comparing `UnleashClient-5.6.0/UnleashClient/periodic_tasks/send_metrics.py` & `UnleashClient-5.7.0/UnleashClient/periodic_tasks/send_metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 from collections import ChainMap
 from datetime import datetime, timezone
+
 from UnleashClient.api import send_metrics
+from UnleashClient.cache import BaseCache
 from UnleashClient.constants import METRIC_LAST_SENT_TIME
 from UnleashClient.utils import LOGGER
-from UnleashClient.cache import BaseCache
 
 
-def aggregate_and_send_metrics(url: str,
-                               app_name: str,
-                               instance_id: str,
-                               custom_headers: dict,
-                               custom_options: dict,
-                               features: dict,
-                               cache: BaseCache
-                               ) -> None:
+def aggregate_and_send_metrics(
+    url: str,
+    app_name: str,
+    instance_id: str,
+    custom_headers: dict,
+    custom_options: dict,
+    features: dict,
+    cache: BaseCache,
+) -> None:
     feature_stats_list = []
 
     for feature_name in features.keys():
         if not (features[feature_name].yes_count or features[feature_name].no_count):
             continue
 
         feature_stats = {
             features[feature_name].name: {
                 "yes": features[feature_name].yes_count,
-                "no": features[feature_name].no_count
+                "no": features[feature_name].no_count,
+                "variants": features[feature_name].variant_counts,
             }
         }
 
         features[feature_name].reset_stats()
         feature_stats_list.append(feature_stats)
 
     metrics_request = {
         "appName": app_name,
         "instanceId": instance_id,
         "bucket": {
             "start": cache.get(METRIC_LAST_SENT_TIME).isoformat(),
             "stop": datetime.now(timezone.utc).isoformat(),
-            "toggles": dict(ChainMap(*feature_stats_list))
-        }
+            "toggles": dict(ChainMap(*feature_stats_list)),
+        },
     }
 
     if feature_stats_list:
         send_metrics(url, metrics_request, custom_headers, custom_options)
         cache.set(METRIC_LAST_SENT_TIME, datetime.now(timezone.utc))
     else:
         LOGGER.debug("No feature flags with metrics, skipping metrics submission.")
```

### Comparing `UnleashClient-5.6.0/UnleashClient/strategies/FlexibleRolloutStrategy.py` & `UnleashClient-5.7.0/UnleashClient/strategies/FlexibleRolloutStrategy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # pylint: disable=invalid-name
 import random
+
 from UnleashClient.strategies.Strategy import Strategy
 from UnleashClient.utils import normalized_hash
 
 
 class FlexibleRollout(Strategy):
     @staticmethod
     def random_hash() -> int:
@@ -11,25 +12,35 @@
 
     def apply(self, context: dict = None) -> bool:
         """
         If constraints are satisfied, return a percentage rollout on provisioned.
 
         :return:
         """
-        percentage = int(self.parameters['rollout'])
-        activation_group = self.parameters['groupId']
-        stickiness = self.parameters['stickiness'] if "stickiness" in self.parameters else "default"
-
-        if stickiness == 'default':
-            if 'userId' in context.keys():
-                calculated_percentage = normalized_hash(context['userId'], activation_group)
-            elif 'sessionId' in context.keys():
-                calculated_percentage = normalized_hash(context['sessionId'], activation_group)
+        percentage = int(self.parameters["rollout"])
+        activation_group = self.parameters["groupId"]
+        stickiness = (
+            self.parameters["stickiness"]
+            if "stickiness" in self.parameters
+            else "default"
+        )
+
+        if stickiness == "default":
+            if "userId" in context.keys():
+                calculated_percentage = normalized_hash(
+                    context["userId"], activation_group
+                )
+            elif "sessionId" in context.keys():
+                calculated_percentage = normalized_hash(
+                    context["sessionId"], activation_group
+                )
             else:
                 calculated_percentage = self.random_hash()
         elif stickiness == "random":
             calculated_percentage = self.random_hash()
         else:
-            custom_stickiness = context.get(stickiness) or context.get("properties")[stickiness]
+            custom_stickiness = (
+                context.get(stickiness) or context.get("properties")[stickiness]
+            )
             calculated_percentage = normalized_hash(custom_stickiness, activation_group)
 
         return percentage > 0 and calculated_percentage <= percentage
```

### Comparing `UnleashClient-5.6.0/UnleashClient/strategies/GradualRolloutSessionId.py` & `UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutSessionId.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable=invalid-name
-from UnleashClient.utils import normalized_hash
 from UnleashClient.strategies.Strategy import Strategy
+from UnleashClient.utils import normalized_hash
 
 
 class GradualRolloutSessionId(Strategy):
     def apply(self, context: dict = None) -> bool:
         """
         Returns true if userId is a member of id list.
 
         :return:
         """
         percentage = int(self.parameters["percentage"])
         activation_group = self.parameters["groupId"]
 
-        return percentage > 0 and normalized_hash(context["sessionId"], activation_group) <= percentage
+        return (
+            percentage > 0
+            and normalized_hash(context["sessionId"], activation_group) <= percentage
+        )
```

### Comparing `UnleashClient-5.6.0/UnleashClient/strategies/GradualRolloutUserId.py` & `UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutUserId.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable=invalid-name
-from UnleashClient.utils import normalized_hash
 from UnleashClient.strategies.Strategy import Strategy
+from UnleashClient.utils import normalized_hash
 
 
 class GradualRolloutUserId(Strategy):
     def apply(self, context: dict = None) -> bool:
         """
         Returns true if userId is a member of id list.
 
         :return:
         """
         percentage = int(self.parameters["percentage"])
         activation_group = self.parameters["groupId"]
 
-        return percentage > 0 and normalized_hash(context["userId"], activation_group) <= percentage
+        return (
+            percentage > 0
+            and normalized_hash(context["userId"], activation_group) <= percentage
+        )
```

### Comparing `UnleashClient-5.6.0/UnleashClient/strategies/RemoteAddress.py` & `UnleashClient-5.7.0/UnleashClient/strategies/RemoteAddress.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 # pylint: disable=invalid-name
 import ipaddress
+
 from UnleashClient.strategies.Strategy import Strategy
 from UnleashClient.utils import LOGGER
 
 
 class RemoteAddress(Strategy):
     def load_provisioning(self) -> list:
         parsed_ips = []
 
-        for address in self.parameters["IPs"].split(','):
-
+        for address in self.parameters["IPs"].split(","):
             if "/" in address:
                 try:
                     parsed_ips.append(ipaddress.ip_network(address.strip(), strict=True))  # type: ignore
-                except (ipaddress.AddressValueError, ipaddress.NetmaskValueError, ValueError) as parsing_error:
+                except (
+                    ipaddress.AddressValueError,
+                    ipaddress.NetmaskValueError,
+                    ValueError,
+                ) as parsing_error:
                     LOGGER.warning("Error parsing IP range: %s", parsing_error)
             else:
                 try:
                     parsed_ips.append(ipaddress.ip_address(address.strip()))  # type: ignore
-                except (ipaddress.AddressValueError, ipaddress.NetmaskValueError, ValueError) as parsing_error:
+                except (
+                    ipaddress.AddressValueError,
+                    ipaddress.NetmaskValueError,
+                    ValueError,
+                ) as parsing_error:
                     LOGGER.warning("Error parsing IP : %s", parsing_error)
 
         return parsed_ips
 
     def apply(self, context: dict = None) -> bool:
         """
         Returns true if IP is in list of IPs
 
         :return:
         """
         return_value = False
 
         try:
             context_ip = ipaddress.ip_address(context["remoteAddress"])
-        except (ipaddress.AddressValueError, ipaddress.NetmaskValueError, ValueError) as parsing_error:
+        except (
+            ipaddress.AddressValueError,
+            ipaddress.NetmaskValueError,
+            ValueError,
+        ) as parsing_error:
             LOGGER.warning("Error parsing IP : %s", parsing_error)
             context_ip = None
 
         if context_ip:
-            for addr_or_range in [value for value in self.parsed_provisioning if value.version == context_ip.version]:
-                if isinstance(addr_or_range, (ipaddress.IPv4Address, ipaddress.IPv6Address)):
+            for addr_or_range in [
+                value
+                for value in self.parsed_provisioning
+                if value.version == context_ip.version
+            ]:
+                if isinstance(
+                    addr_or_range, (ipaddress.IPv4Address, ipaddress.IPv6Address)
+                ):
                     if context_ip == addr_or_range:
                         return_value = True
                         break
                 else:
-                    if context_ip in addr_or_range:
+                    if context_ip in addr_or_range:  # noqa: PLR5501
                         return_value = True
                         break
 
         return return_value
```

### Comparing `UnleashClient-5.6.0/UnleashClient/strategies/Strategy.py` & `UnleashClient-5.7.0/UnleashClient/strategies/Strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=invalid-name,dangerous-default-value
-from typing import Iterator
 import warnings
+from typing import Iterator
+
 from UnleashClient.constraints import Constraint
 
 
 class Strategy:
     """
     The parent class for default and custom strategies.
 
@@ -13,30 +14,31 @@
     - ``__init__()`` - Depending on the parameters your feature needs
     - ``apply()`` - Your feature provisioning
 
     :param constraints: List of 'constraints' objects derived from strategy section (...from feature section) of `/api/clients/features` Unleash server response.
     :param parameters: The 'parameter' objects from the strategy section (...from feature section) of `/api/clients/features` Unleash server response.
     """
 
-    def __init__(self,
-                 constraints: list = [],
-                 parameters: dict = {},
-                 segment_ids: list = None,
-                 global_segments: dict = None
-                 ) -> None:
+    def __init__(
+        self,
+        constraints: list = [],
+        parameters: dict = {},
+        segment_ids: list = None,
+        global_segments: dict = None,
+    ) -> None:
         self.parameters = parameters
         self.constraints = constraints
         self.segment_ids = segment_ids or []
         self.global_segments = global_segments or {}
         self.parsed_provisioning = self.load_provisioning()
 
     def __call__(self, context: dict = None):
         warnings.warn(
             "unleash-client-python v3.x.x requires overriding the execute() method instead of the __call__() method.",
-            DeprecationWarning
+            DeprecationWarning,
         )
 
     def execute(self, context: dict = None) -> bool:
         """
         Executes the strategies by:
 
         - Checking constraints
@@ -68,15 +70,17 @@
         """
         Loads strategy provisioning from Unleash feature flag configuration.
 
         This should parse the raw values in ``self.parameters`` into format Python can comprehend.
         """
         return []
 
-    def apply(self, context: dict = None) -> bool:  # pylint: disable=unused-argument,no-self-use
+    def apply(
+        self, context: dict = None
+    ) -> bool:  # pylint: disable=unused-argument,no-self-use
         """
         Strategy implementation.
 
         :param context: Feature flag context
         :return: Feature flag result
         """
         return False
```

### Comparing `UnleashClient-5.6.0/UnleashClient/strategies/UserWithId.py` & `UnleashClient-5.7.0/UnleashClient/strategies/UserWithId.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable=invalid-name
 from UnleashClient.strategies.Strategy import Strategy
 
 
 class UserWithId(Strategy):
     def load_provisioning(self) -> list:
-        return [x.strip() for x in self.parameters["userIds"].split(',')]
+        return [x.strip() for x in self.parameters["userIds"].split(",")]
 
     def apply(self, context: dict = None) -> bool:
         """
         Returns true if userId is a member of id list.
 
         :return:
         """
```

### Comparing `UnleashClient-5.6.0/UnleashClient/utils.py` & `UnleashClient-5.7.0/UnleashClient/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from enum import Enum
 from threading import RLock
 from typing import Any
+
 import mmh3  # pylint: disable=import-error
 from requests import Response
 
-LOGGER = logging.getLogger('UnleashClient')
+LOGGER = logging.getLogger("UnleashClient")
 
 
 class InstanceAllowType(Enum):
     BLOCK = 1
     WARN = 2
     SILENTLY_ALLOW = 3
 
@@ -34,25 +35,28 @@
         with self.lock:
             if key in self:
                 self.instances[key] += 1
             else:
                 self.instances[key] = 1
 
 
-def normalized_hash(identifier: str,
-                    activation_group: str,
-                    normalizer: int = 100) -> int:
+def normalized_hash(
+    identifier: str, activation_group: str, normalizer: int = 100
+) -> int:
     return mmh3.hash(f"{activation_group}:{identifier}", signed=False) % normalizer + 1
 
 
 def get_identifier(context_key_name: str, context: dict) -> Any:
     if context_key_name in context.keys():
         value = context[context_key_name]
-    elif 'properties' in context.keys() and context_key_name in context['properties'].keys():
-        value = context['properties'][context_key_name]
+    elif (
+        "properties" in context.keys()
+        and context_key_name in context["properties"].keys()
+    ):
+        value = context["properties"][context_key_name]
     else:
         value = None
 
     return value
 
 
 def log_resp_info(resp: Response) -> None:
```

### Comparing `UnleashClient-5.6.0/UnleashClient/variants/Variants.py` & `UnleashClient-5.7.0/UnleashClient/variants/Variants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=invalid-name, too-few-public-methods
-import random
 import copy
-from typing import Dict
+import random
+from typing import Dict  # noqa: F401
+
 from UnleashClient import utils
 from UnleashClient.constants import DISABLED_VARIATION
 
 
 class Variants:
     def __init__(self, variants_list: list, feature_name: str) -> None:
         """
@@ -19,54 +20,57 @@
     def _apply_overrides(self, context: dict) -> dict:
         """
         Figures out if an override should be applied based on a context.
 
         Notes:
             - This matches only the first variant found.
         """
-        variants_with_overrides = [x for x in self.variants if 'overrides' in x.keys()]
+        variants_with_overrides = [x for x in self.variants if "overrides" in x.keys()]
         override_variant = {}  # type: Dict
 
         for variant in variants_with_overrides:
-            for override in variant['overrides']:
-                identifier = utils.get_identifier(override['contextName'], context)
+            for override in variant["overrides"]:
+                identifier = utils.get_identifier(override["contextName"], context)
                 if identifier in override["values"]:
                     override_variant = variant
 
         return override_variant
 
     @staticmethod
     def _get_seed(context: dict, stickiness_selector: str = "default") -> str:
         """Grabs seed value from context."""
         seed = ""
 
         if stickiness_selector == "default":
-            if 'userId' in context:
-                seed = context['userId']
-            elif 'sessionId' in context:
-                seed = context['sessionId']
-            elif 'remoteAddress' in context:
-                seed = context['remoteAddress']
+            if "userId" in context:
+                seed = context["userId"]
+            elif "sessionId" in context:
+                seed = context["sessionId"]
+            elif "remoteAddress" in context:
+                seed = context["remoteAddress"]
             else:
                 seed = str(random.random() * 10000)
-        elif stickiness_selector == 'random':
+        elif stickiness_selector == "random":
             seed = str(random.random() * 10000)
         else:
-            seed = context.get(stickiness_selector) or context.get("properties")[stickiness_selector]
+            seed = (
+                context.get(stickiness_selector)
+                or context.get("properties")[stickiness_selector]
+            )
 
         return seed
 
     @staticmethod
     def _format_variation(variation: dict) -> dict:
         formatted_variation = copy.deepcopy(variation)
-        del formatted_variation['weight']
-        if 'overrides' in formatted_variation:
-            del formatted_variation['overrides']
-        if 'stickiness' in formatted_variation:
-            del formatted_variation['stickiness']
+        del formatted_variation["weight"]
+        if "overrides" in formatted_variation:
+            del formatted_variation["overrides"]
+        if "stickiness" in formatted_variation:
+            del formatted_variation["stickiness"]
         return formatted_variation
 
     def get_variant(self, context: dict) -> dict:
         """
         Determines what variation a user is in.
 
         :param context:
@@ -75,22 +79,30 @@
         fallback_variant = copy.deepcopy(DISABLED_VARIATION)
 
         if self.variants:
             override_variant = self._apply_overrides(context)
             if override_variant:
                 return self._format_variation(override_variant)
 
-            total_weight = sum(x['weight'] for x in self.variants)
+            total_weight = sum(x["weight"] for x in self.variants)
             if total_weight <= 0:
                 return fallback_variant
 
-            stickiness_selector = self.variants[0]['stickiness'] if 'stickiness' in self.variants[0].keys() else "default"
-            target = utils.normalized_hash(self._get_seed(context, stickiness_selector), self.feature_name, total_weight)
+            stickiness_selector = (
+                self.variants[0]["stickiness"]
+                if "stickiness" in self.variants[0].keys()
+                else "default"
+            )
+            target = utils.normalized_hash(
+                self._get_seed(context, stickiness_selector),
+                self.feature_name,
+                total_weight,
+            )
             counter = 0
             for variation in self.variants:
-                counter += variation['weight']
+                counter += variation["weight"]
 
                 if counter >= target:
                     return self._format_variation(variation)
 
         # Catch all return.
         return fallback_variant
```

### Comparing `UnleashClient-5.6.0/UnleashClient.egg-info/PKG-INFO` & `UnleashClient-5.7.0/UnleashClient.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,127 @@
 Metadata-Version: 2.1
 Name: UnleashClient
-Version: 5.6.0
+Version: 5.7.0
 Summary: Python client for the Unleash feature toggle system!
-Home-page: https://github.com/Unleash/unleash-client-python
-Author: Ivan Lee
-Author-email: ivanklee86@gmail.com
-License: UNKNOWN
-Description: # unleash-client-python
-        
-        ![](https://github.com/unleash/unleash-client-python/workflows/CI/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/Unleash/unleash-client-python/badge.svg?branch=main)](https://coveralls.io/github/Unleash/unleash-client-python?branch=main) [![PyPI version](https://badge.fury.io/py/UnleashClient.svg)](https://badge.fury.io/py/UnleashClient) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/UnleashClient.svg) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        
-        This is the Python client for [Unleash](https://github.com/unleash/unleash).  It implements [Client Specifications 1.0](https://github.com/Unleash/unleash/blob/main/docs/client-specification.md) and checks compliance based on spec in [unleash/client-specifications](https://github.com/Unleash/client-specification)
-        
-        What it supports:
-        * Default activation strategies using 32-bit [Murmurhash3](https://en.wikipedia.org/wiki/MurmurHash)
-        * Custom strategies
-        * Full client lifecycle:
-            * Client registers with Unleash server
-            * Client periodically fetches feature toggles and stores to on-disk cache
-            * Client periodically sends metrics to Unleash Server
-        * Tested on Linux (Ubuntu), OSX, and Windows
-        
-        Check out the [project documentation](https://unleash.github.io/unleash-client-python/) and the [changelog](https://docs.getunleash.io/unleash-client-python/changelog.html).
-        
-        ## Installation
-        
-        Check out the package on [Pypi](https://pypi.org/project/UnleashClient/)!
-        
-        ```bash
-        pip install UnleashClient
-        ```
-        
-        ## For Flask Users
-        
-        If you're looking into running Unleash from Flask, you might want to take a look at [_Flask-Unleash_, the Unleash Flask extension](https://github.com/Unleash/Flask-Unleash). The extension builds upon this SDK to reduce the amount of boilerplate code you need to write to integrate with Flask. Of course, if you'd rather use this package directly, that will work too.
-        
-        ## Usage
-        
-        ### Initialization
-        
-        ```python
-        from UnleashClient import UnleashClient
-        
-        client = UnleashClient(
-            url="https://unleash.herokuapp.com",
-            app_name="my-python-app",
-            custom_headers={'Authorization': '<API token>'})
-        
-        client.initialize_client()
-        ```
-        
-        For more information about configuring `UnleashClient`, check out the [project reference docs](https://docs.getunleash.io/unleash-client-python/unleashclient.html)!
-        
-        ### Checking if a feature is enabled
-        
-        A check of a simple toggle:
-        ```python
-        client.is_enabled("my_toggle")
-        ```
-        
-        To supply application context, use the second positional argument:
-        
-        ```python
-        app_context = {"userId": "test@email.com"}
-        client.is_enabled("user_id_toggle", app_context)
-        ```
-        
-        #### Fallback function and default values
-        
-        You can specify a fallback function for cases where the client doesn't recognize the toggle by using the `fallback_function` keyword argument:
-        
-        ```python
-        def custom_fallback(feature_name: str, context: dict) -> bool:
-            return True
-        
-        client.is_enabled("my_toggle", fallback_function=custom_fallback)
-        ```
-        
-        You can also use the `fallback_function` argument to replace the obsolete `default_value` keyword argument by using a lambda that ignores its inputs. Whatever the lambda returns will be used as the default value.
-        
-        ```python
-        client.is_enabled("my_toggle", fallback_function=lambda feature_name, context: True)
-        ```
-        
-        The fallback function **must** accept the feature name and context as positional arguments in that order.
-        
-        The client will evaluate the fallback function only if an exception occurs when calling the `is_enabled()` method. This happens when the client can't find the feature flag. The client _may_ also throw other, general exceptions.
-        
-        For more information about usage, see the [Usage documentation](https://docs.getunleash.io/unleash-client-python/usage.html).
-        
-        ### Getting a variant
-        
-        Checking for a variant:
-        ```python
-        context = {'userId': '2'}  # Context must have userId, sessionId, or remoteAddr.  If none are present, distribution will be random.
-        
-        variant = client.get_variant("variant_toggle", context)
-        
-        print(variant)
-        > {
-        >    "name": "variant1",
-        >    "payload": {
-        >        "type": "string",
-        >        "value": "val1"
-        >        },
-        >    "enabled": True
-        > }
-        ```
-        
-        For more information about variants, see the [Variant documentation](https://docs.getunleash.io/advanced/toggle_variants).
-        
-Platform: UNKNOWN
+Author-email: Ivan Lee <ivanklee86@gmail.com>
+Project-URL: Homepage, https://github.com/Unleash/unleash-client-python
+Project-URL: Documentation, https://docs.getunleash.io/unleash-client-python
+Project-URL: Changelog, https://github.com/Unleash/unleash-client-python/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/Unleash/unleash-client-python
+Project-URL: Issues, https://github.com/Unleash/unleash-client-python/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# unleash-client-python
+
+![](https://github.com/unleash/unleash-client-python/workflows/CI/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/Unleash/unleash-client-python/badge.svg?branch=main)](https://coveralls.io/github/Unleash/unleash-client-python?branch=main) [![PyPI version](https://badge.fury.io/py/UnleashClient.svg)](https://badge.fury.io/py/UnleashClient) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/UnleashClient.svg) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+
+This is the Python client for [Unleash](https://github.com/unleash/unleash).  It implements [Client Specifications 1.0](https://github.com/Unleash/unleash/blob/main/docs/client-specification.md) and checks compliance based on spec in [unleash/client-specifications](https://github.com/Unleash/client-specification)
+
+What it supports:
+* Default activation strategies using 32-bit [Murmurhash3](https://en.wikipedia.org/wiki/MurmurHash)
+* Custom strategies
+* Full client lifecycle:
+    * Client registers with Unleash server
+    * Client periodically fetches feature toggles and stores to on-disk cache
+    * Client periodically sends metrics to Unleash Server
+* Tested on Linux (Ubuntu), OSX, and Windows
+
+Check out the [project documentation](https://unleash.github.io/unleash-client-python/) and the [changelog](https://docs.getunleash.io/unleash-client-python/changelog.html).
+
+## Installation
+
+Check out the package on [Pypi](https://pypi.org/project/UnleashClient/)!
+
+```bash
+pip install UnleashClient
+```
+
+## For Flask Users
+
+If you're looking into running Unleash from Flask, you might want to take a look at [_Flask-Unleash_, the Unleash Flask extension](https://github.com/Unleash/Flask-Unleash). The extension builds upon this SDK to reduce the amount of boilerplate code you need to write to integrate with Flask. Of course, if you'd rather use this package directly, that will work too.
+
+## Usage
+
+### Initialization
+
+```python
+from UnleashClient import UnleashClient
+
+client = UnleashClient(
+    url="https://unleash.herokuapp.com",
+    app_name="my-python-app",
+    custom_headers={'Authorization': '<API token>'})
+
+client.initialize_client()
+```
+
+For more information about configuring `UnleashClient`, check out the [project reference docs](https://docs.getunleash.io/unleash-client-python/unleashclient.html)!
+
+### Checking if a feature is enabled
+
+A check of a simple toggle:
+```python
+client.is_enabled("my_toggle")
+```
+
+To supply application context, use the second positional argument:
+
+```python
+app_context = {"userId": "test@email.com"}
+client.is_enabled("user_id_toggle", app_context)
+```
+
+#### Fallback function and default values
+
+You can specify a fallback function for cases where the client doesn't recognize the toggle by using the `fallback_function` keyword argument:
+
+```python
+def custom_fallback(feature_name: str, context: dict) -> bool:
+    return True
+
+client.is_enabled("my_toggle", fallback_function=custom_fallback)
+```
+
+You can also use the `fallback_function` argument to replace the obsolete `default_value` keyword argument by using a lambda that ignores its inputs. Whatever the lambda returns will be used as the default value.
+
+```python
+client.is_enabled("my_toggle", fallback_function=lambda feature_name, context: True)
+```
+
+The fallback function **must** accept the feature name and context as positional arguments in that order.
+
+The client will evaluate the fallback function only if an exception occurs when calling the `is_enabled()` method. This happens when the client can't find the feature flag. The client _may_ also throw other, general exceptions.
+
+For more information about usage, see the [Usage documentation](https://docs.getunleash.io/unleash-client-python/usage.html).
+
+### Getting a variant
+
+Checking for a variant:
+```python
+context = {'userId': '2'}  # Context must have userId, sessionId, or remoteAddr.  If none are present, distribution will be random.
+
+variant = client.get_variant("variant_toggle", context)
+
+print(variant)
+> {
+>    "name": "variant1",
+>    "payload": {
+>        "type": "string",
+>        "value": "val1"
+>        },
+>    "enabled": True
+> }
+```
+
+For more information about variants, see the [Variant documentation](https://docs.getunleash.io/advanced/toggle_variants).
```

### Comparing `UnleashClient-5.6.0/UnleashClient.egg-info/SOURCES.txt` & `UnleashClient-5.7.0/UnleashClient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-.flake8
 .gitignore
+.lift.toml
+.pre-commit-config.yaml
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE.md
 Makefile
 README.md
-get-spec.sh
 pyproject.toml
 requirements.txt
-setup.py
 tox.ini
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .devcontainer/post_install.sh
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 .github/stale.yml
@@ -31,16 +30,14 @@
 UnleashClient/events.py
 UnleashClient/loader.py
 UnleashClient/py.typed
 UnleashClient/utils.py
 UnleashClient.egg-info/PKG-INFO
 UnleashClient.egg-info/SOURCES.txt
 UnleashClient.egg-info/dependency_links.txt
-UnleashClient.egg-info/not-zip-safe
-UnleashClient.egg-info/requires.txt
 UnleashClient.egg-info/top_level.txt
 UnleashClient/api/__init__.py
 UnleashClient/api/features.py
 UnleashClient/api/metrics.py
 UnleashClient/api/register.py
 UnleashClient/constraints/Constraint.py
 UnleashClient/constraints/__init__.py
@@ -75,14 +72,15 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/strategy.rst
 docs/unleashclient.rst
 docs/usage.rst
 docs/wsgi.rst
+scripts/get-spec.sh
 tests/__init__.py
 tests/conftest.py
 tests/integration_tests/integration.py
 tests/integration_tests/integration_gitlab.py
 tests/integration_tests/integration_unleashheroku.py
 tests/integration_tests/integration_unleashhosted.py
 tests/specification_tests/__init__.py
```

### Comparing `UnleashClient-5.6.0/docs/Makefile` & `UnleashClient-5.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/docs/celery.rst` & `UnleashClient-5.7.0/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/docs/conf.py` & `UnleashClient-5.7.0/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,62 +6,65 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
-import UnleashClient
 from importlib_metadata import version
 
+import UnleashClient  # noqa: F401
+
 # -- Project information -----------------------------------------------------
 
-project = 'unleash-client-python'
-copyright = '2022 Unleash'
-author = 'Ivan Lee'
+project = "unleash-client-python"
+copyright = "2022 Unleash"
+author = "Ivan Lee"
 version = version("UnleashClient")
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.autosummary",
     "sphinx.ext.githubpages",
     "m2r2",
-    "enum_tools.autoenum"
+    "enum_tools.autoenum",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
-source_suffix = ['.rst', '.md']
+source_suffix = [".rst", ".md"]
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 
-html_sidebars = { '**': ['globaltoc.html', 'relations.html', 'sourcelink.html', 'searchbox.html'] }
+html_sidebars = {
+    "**": ["globaltoc.html", "relations.html", "sourcelink.html", "searchbox.html"]
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 html_context = {
-  'display_github': True,
-  'github_user': 'unleash',
-  'github_repo': 'unleash-client-python',
-  'github_version': 'main/docs/',
+    "display_github": True,
+    "github_user": "unleash",
+    "github_repo": "unleash-client-python",
+    "github_version": "main/docs/",
 }
```

### Comparing `UnleashClient-5.6.0/docs/customcache.rst` & `UnleashClient-5.7.0/docs/customcache.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/docs/customstrategies.rst` & `UnleashClient-5.7.0/docs/customstrategies.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/docs/development.rst` & `UnleashClient-5.7.0/docs/development.rst`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 Here are some notes about common tools and tasks you'll run into when working on `unleash-client-python`.
 
 Tooling
 #######################################
 
 - `Pyenv <https://github.com/pyenv/pyenv>`_ for managing Python versions.
+- `ruff <https://github.com/charliermarsh/ruff>`_ for linting.
+- `black <https://github.com/psf/black>`_ for formatting.
 
 Testing
 #######################################
 
 1. Activate your virtualenv solution (e.g. `source activate YOUR_VIRTUALENV`).
 2. Run linting & tests: ``make test``
```

### Comparing `UnleashClient-5.6.0/docs/eventcallbacks.rst` & `UnleashClient-5.7.0/docs/eventcallbacks.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ****************************************
 Event Callbacks
 ****************************************
 
-The Unleash Python client support event callbacks!  
+The Unleash Python client support event callbacks!
 
 1. Create a function with the type `Callable[[UnleashEvent]]` and pass it to the Unleash client at initialization.
 2. Enable `impression data <https://docs.getunleash.io/reference/impression-data#enabling-impression-data>`_ on feature flag configuration.
 
-Example code using `blinker <https://github.com/pallets-eco/blinker>`_: 
+Example code using `blinker <https://github.com/pallets-eco/blinker>`_:
 
 .. code-block:: python
 
-    from blinker import ignal
+    from blinker import signal
     from UnleashClient import UnleashClient
     from UnleashClient.events import UnleashEvent
-    
+
     send_data = signal('send-data')
 
     @send_data.connect
     def receive_data(sender, **kw):
         print("Caught signal from %r, data %r" % (sender, kw))
         return kw
```

### Comparing `UnleashClient-5.6.0/docs/index.rst` & `UnleashClient-5.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/docs/make.bat` & `UnleashClient-5.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/docs/usage.rst` & `UnleashClient-5.7.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/docs/wsgi.rst` & `UnleashClient-5.7.0/docs/wsgi.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.6.0/tests/integration_tests/integration.py` & `UnleashClient-5.7.0/tests/integration_tests/integration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-import time
-from UnleashClient import UnleashClient
-
 # ---
 import logging
 import sys
+import time
+
+from UnleashClient import UnleashClient
 
 root = logging.getLogger()
 root.setLevel(logging.DEBUG)
 
 handler = logging.StreamHandler(sys.stdout)
 handler.setLevel(logging.DEBUG)
-formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 handler.setFormatter(formatter)
 root.addHandler(handler)
 # ---
 
-my_client = UnleashClient(
-    url="http://localhost:4242/api",
-    app_name="pyIvan"
-)
+my_client = UnleashClient(url="http://localhost:4242/api", app_name="pyIvan")
 
 my_client.initialize_client()
 
 while True:
     time.sleep(10)
     print(my_client.is_enabled("Demo"))
```

### Comparing `UnleashClient-5.6.0/tests/integration_tests/integration_gitlab.py` & `UnleashClient-5.7.0/tests/integration_tests/integration_gitlab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import time
-from UnleashClient import UnleashClient
-
 # ---
 import logging
 import sys
+import time
+
+from UnleashClient import UnleashClient
 
 root = logging.getLogger()
 root.setLevel(logging.DEBUG)
 
 handler = logging.StreamHandler(sys.stdout)
 handler.setLevel(logging.DEBUG)
-formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 handler.setFormatter(formatter)
 root.addHandler(handler)
 # ---
 
 
 my_client = UnleashClient(
     url="https://gitlab.com/api/v4/feature_flags/unleash/32635317",
     app_name="pyIvan",
     instance_id="Sc5fv9aCyFPB4XcEFk-E",
     disable_metrics=True,
-    disable_registration=True
+    disable_registration=True,
 )
 
 my_client.initialize_client()
 
 while True:
     time.sleep(10)
     print(my_client.is_enabled("test"))
```

### Comparing `UnleashClient-5.6.0/tests/integration_tests/integration_unleashheroku.py` & `UnleashClient-5.7.0/tests/integration_tests/integration_unleashheroku.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-import time
-from UnleashClient import UnleashClient
-
-
 # ---
 import logging
 import sys
+import time
+
+from UnleashClient import UnleashClient
 
 root = logging.getLogger()
 root.setLevel(logging.DEBUG)
 
 handler = logging.StreamHandler(sys.stdout)
 handler.setLevel(logging.DEBUG)
-formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 handler.setFormatter(formatter)
 root.addHandler(handler)
 # ---
 
 my_client = UnleashClient(
     url="https://unleash.herokuapp.com/api",
     environment="staging",
     app_name="pyIvan",
 )
 
 my_client.initialize_client()
 
 while True:
     time.sleep(10)
-    context = {
-        'userId': "1",
-        'sound': 'woof'
-    }
+    context = {"userId": "1", "sound": "woof"}
     print(f"ivantest: {my_client.is_enabled('ivantest', context)}")
```

### Comparing `UnleashClient-5.6.0/tests/integration_tests/integration_unleashhosted.py` & `UnleashClient-5.7.0/tests/integration_tests/integration_unleashhosted.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from UnleashClient import UnleashClient
 from UnleashClient.strategies import Strategy
 
 
 # ---
 class DogTest(Strategy):
     def load_provisioning(self) -> list:
-        return [x.strip() for x in self.parameters["sound"].split(',')]
+        return [x.strip() for x in self.parameters["sound"].split(",")]
 
     def apply(self, context: dict = None) -> bool:
         """
         Turn on if I'm a dog.
 
         :return:
         """
@@ -28,36 +28,37 @@
 # ---
 
 root = logging.getLogger()
 root.setLevel(logging.DEBUG)
 
 handler = logging.StreamHandler(sys.stdout)
 handler.setLevel(logging.DEBUG)
-formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 handler.setFormatter(formatter)
 root.addHandler(handler)
 # ---
 
 custom_strategies_dict = {
     "amIADog": DogTest,
 }
 
 my_client = UnleashClient(
     url="https://app.unleash-hosted.com/demo/api",
     environment="staging",
     app_name="pyIvan",
-    custom_headers={'Authorization': '56907a2fa53c1d16101d509a10b78e36190b0f918d9f122d'},
+    custom_headers={
+        "Authorization": "56907a2fa53c1d16101d509a10b78e36190b0f918d9f122d"
+    },
     custom_strategies=custom_strategies_dict,
-    verbose_log_level=10
+    verbose_log_level=10,
 )
 
 my_client.initialize_client()
 
 while True:
     time.sleep(10)
-    context = {
-        'userId': "1",
-        'sound': 'woof'
-    }
+    context = {"userId": "1", "sound": "woof"}
     print(f"ivantest: {my_client.is_enabled('ivantest', context)}")
     print(f"ivan-variations: {my_client.get_variant('ivan-variations', context)}")
-    print(f"ivan-customstrategyx: {my_client.is_enabled('ivan-customstrategy', context)}")
+    print(
+        f"ivan-customstrategyx: {my_client.is_enabled('ivan-customstrategy', context)}"
+    )
```

### Comparing `UnleashClient-5.6.0/tests/specification_tests/test_client_specs.py` & `UnleashClient-5.7.0/tests/specification_tests/test_client_specs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import uuid
 from os import path
-from UnleashClient import UnleashClient
-from tests.utilities.testing_constants import URL, APP_NAME
-from UnleashClient.cache import FileCache
+
 import pytest
 
+from tests.utilities.testing_constants import APP_NAME, URL
+from UnleashClient import UnleashClient
+from UnleashClient.cache import FileCache
 
 CLIENT_SPEC_PATH = "tests/specification_tests/client-specification/specifications"
 
 
 def load_spec(spec):
     with open(path.join(CLIENT_SPEC_PATH, spec)) as _f:
         data = json.load(_f)
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/api/test_feature.py` & `UnleashClient-5.7.0/tests/unit_tests/api/test_feature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,141 @@
+from datetime import date
+
+import pytest
 import responses
 from pytest import mark, param
 
-from tests.utilities.mocks.mock_features import MOCK_FEATURE_RESPONSE, MOCK_FEATURE_RESPONSE_PROJECT
-from tests.utilities.testing_constants import URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS, PROJECT_URL, PROJECT_NAME, ETAG_VALUE
-from UnleashClient.constants import FEATURES_URL
+from tests.utilities.mocks.mock_features import (
+    MOCK_FEATURE_RESPONSE,
+    MOCK_FEATURE_RESPONSE_PROJECT,
+)
+from tests.utilities.testing_constants import (
+    APP_NAME,
+    CUSTOM_HEADERS,
+    CUSTOM_OPTIONS,
+    ETAG_VALUE,
+    INSTANCE_ID,
+    PROJECT_NAME,
+    PROJECT_URL,
+    URL,
+)
 from UnleashClient.api import get_feature_toggles
-
+from UnleashClient.constants import FEATURES_URL
 
 FULL_FEATURE_URL = URL + FEATURES_URL
 
 
 @responses.activate
-@mark.parametrize("response,status,calls,expected", (
-    param(MOCK_FEATURE_RESPONSE, 200, 1, lambda result: result["version"] == 1, id="success"),
-    param(MOCK_FEATURE_RESPONSE, 202, 1, lambda result: not result, id="failure"),
-    param({}, 500, 4, lambda result: not result, id="failure"),
-))
+@mark.parametrize(
+    "response,status,calls,expected",
+    (
+        param(
+            MOCK_FEATURE_RESPONSE,
+            200,
+            1,
+            lambda result: result["version"] == 1,
+            id="success",
+        ),
+        param(MOCK_FEATURE_RESPONSE, 202, 1, lambda result: not result, id="failure"),
+        param({}, 500, 4, lambda result: not result, id="failure"),
+    ),
+)
 def test_get_feature_toggle(response, status, calls, expected):
-    responses.add(responses.GET, FULL_FEATURE_URL, json=response, status=status, headers={'etag': ETAG_VALUE})
-
-    (result, etag) = get_feature_toggles(URL,
-                                         APP_NAME,
-                                         INSTANCE_ID,
-                                         CUSTOM_HEADERS,
-                                         CUSTOM_OPTIONS)
+    responses.add(
+        responses.GET,
+        FULL_FEATURE_URL,
+        json=response,
+        status=status,
+        headers={"etag": ETAG_VALUE},
+    )
+
+    (result, etag) = get_feature_toggles(
+        URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS
+    )
 
     assert len(responses.calls) == calls
     assert expected(result)
 
 
 @responses.activate
 def test_get_feature_toggle_project():
-    responses.add(responses.GET, PROJECT_URL, json=MOCK_FEATURE_RESPONSE_PROJECT, status=200, headers={'etag': ETAG_VALUE})
-
-    (result, etag) = get_feature_toggles(URL,
-                                         APP_NAME,
-                                         INSTANCE_ID,
-                                         CUSTOM_HEADERS,
-                                         CUSTOM_OPTIONS,
-                                         PROJECT_NAME)
+    responses.add(
+        responses.GET,
+        PROJECT_URL,
+        json=MOCK_FEATURE_RESPONSE_PROJECT,
+        status=200,
+        headers={"etag": ETAG_VALUE},
+    )
+
+    (result, etag) = get_feature_toggles(
+        URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS, PROJECT_NAME
+    )
 
     assert len(responses.calls) == 1
     assert len(result["features"]) == 1
     assert etag == ETAG_VALUE
 
 
 @responses.activate
 def test_get_feature_toggle_failed_etag():
-    responses.add(responses.GET, PROJECT_URL, json={}, status=500, headers={'etag': ETAG_VALUE})
-
-    (result, etag) = get_feature_toggles(URL,
-                                         APP_NAME,
-                                         INSTANCE_ID,
-                                         CUSTOM_HEADERS,
-                                         CUSTOM_OPTIONS,
-                                         PROJECT_NAME)
+    responses.add(
+        responses.GET, PROJECT_URL, json={}, status=500, headers={"etag": ETAG_VALUE}
+    )
+
+    (result, etag) = get_feature_toggles(
+        URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS, PROJECT_NAME
+    )
 
     assert len(responses.calls) == 4
-    assert etag == ''
+    assert not etag
 
 
+@pytest.mark.skipif(
+    date.today() < date(2023, 7, 1),
+    reason="This is currently breaking due to a dependency or the test setup. Skipping this allows us to run tests in CI without this popping up as an error all the time.",
+)
 @responses.activate
 def test_get_feature_toggle_etag_present():
-    responses.add(responses.GET, PROJECT_URL, json={}, status=304, headers={'etag': ETAG_VALUE})
-
-    (result, etag) = get_feature_toggles(URL,
-                                         APP_NAME,
-                                         INSTANCE_ID,
-                                         CUSTOM_HEADERS,
-                                         CUSTOM_OPTIONS,
-                                         PROJECT_NAME,
-                                         ETAG_VALUE)
+    responses.add(
+        responses.GET, PROJECT_URL, json={}, status=304, headers={"etag": ETAG_VALUE}
+    )
+
+    (result, etag) = get_feature_toggles(
+        URL,
+        APP_NAME,
+        INSTANCE_ID,
+        CUSTOM_HEADERS,
+        CUSTOM_OPTIONS,
+        PROJECT_NAME,
+        ETAG_VALUE,
+    )
 
     assert len(responses.calls) == 1
     assert not result
-    assert responses.calls[0].request.headers['If-None-Match'] == ETAG_VALUE
+    assert responses.calls[0].request.headers["If-None-Match"] == ETAG_VALUE
     assert etag == ETAG_VALUE
 
 
 @responses.activate
 def test_get_feature_toggle_retries():
     responses.add(responses.GET, PROJECT_URL, json={}, status=500)
-    responses.add(responses.GET, PROJECT_URL, json=MOCK_FEATURE_RESPONSE_PROJECT, status=200, headers={'etag': ETAG_VALUE})
-
-    (result, etag) = get_feature_toggles(URL,
-                                     APP_NAME,
-                                     INSTANCE_ID,
-                                     CUSTOM_HEADERS,
-                                     CUSTOM_OPTIONS,
-                                     PROJECT_NAME,
-                                     ETAG_VALUE)
+    responses.add(
+        responses.GET,
+        PROJECT_URL,
+        json=MOCK_FEATURE_RESPONSE_PROJECT,
+        status=200,
+        headers={"etag": ETAG_VALUE},
+    )
+
+    (result, etag) = get_feature_toggles(
+        URL,
+        APP_NAME,
+        INSTANCE_ID,
+        CUSTOM_HEADERS,
+        CUSTOM_OPTIONS,
+        PROJECT_NAME,
+        ETAG_VALUE,
+    )
 
     assert len(responses.calls) == 2
     assert len(result["features"]) == 1
     assert etag == ETAG_VALUE
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/api/test_metrics.py` & `UnleashClient-5.7.0/tests/unit_tests/api/test_metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import responses
 from pytest import mark, param
 from requests import ConnectionError
-from tests.utilities.testing_constants import URL, CUSTOM_HEADERS, CUSTOM_OPTIONS
+
 from tests.utilities.mocks.mock_metrics import MOCK_METRICS_REQUEST
-from UnleashClient.constants import METRICS_URL
+from tests.utilities.testing_constants import CUSTOM_HEADERS, CUSTOM_OPTIONS, URL
 from UnleashClient.api import send_metrics
-
+from UnleashClient.constants import METRICS_URL
 
 FULL_METRICS_URL = URL + METRICS_URL
 
 
 @responses.activate
-@mark.parametrize("payload,status,expected", (
-    param({"json": {}}, 202, lambda result: result, id="success"),
-    param({"json": {}}, 500, lambda result: not result, id="failure"),
-    param({"body": ConnectionError("Test connection error.")}, 200, lambda result: not result, id="exception"),
-))
+@mark.parametrize(
+    "payload,status,expected",
+    (
+        param({"json": {}}, 202, lambda result: result, id="success"),
+        param({"json": {}}, 500, lambda result: not result, id="failure"),
+        param(
+            {"body": ConnectionError("Test connection error.")},
+            200,
+            lambda result: not result,
+            id="exception",
+        ),
+    ),
+)
 def test_send_metrics(payload, status, expected):
     responses.add(responses.POST, FULL_METRICS_URL, **payload, status=status)
 
     result = send_metrics(URL, MOCK_METRICS_REQUEST, CUSTOM_HEADERS, CUSTOM_OPTIONS)
 
     assert len(responses.calls) == 1
     assert expected(result)
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py` & `UnleashClient-5.7.0/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 import json
-from datetime import datetime, timezone, timedelta
+from datetime import datetime, timedelta, timezone
+
 import responses
-from tests.utilities.testing_constants import URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS, IP_LIST
-from UnleashClient.constants import METRICS_URL, METRIC_LAST_SENT_TIME
-from UnleashClient.periodic_tasks import aggregate_and_send_metrics
-from UnleashClient.features import Feature
-from UnleashClient.strategies import RemoteAddress, Default
-from UnleashClient.cache import FileCache
 
+from tests.utilities.mocks.mock_variants import VARIANTS
+from tests.utilities.testing_constants import (
+    APP_NAME,
+    CUSTOM_HEADERS,
+    CUSTOM_OPTIONS,
+    INSTANCE_ID,
+    IP_LIST,
+    URL,
+)
+from UnleashClient.cache import FileCache
+from UnleashClient.constants import METRIC_LAST_SENT_TIME, METRICS_URL
+from UnleashClient.features import Feature
+from UnleashClient.periodic_tasks import aggregate_and_send_metrics
+from UnleashClient.strategies import Default, RemoteAddress
+from UnleashClient.variants import Variants
 
 FULL_METRICS_URL = URL + METRICS_URL
 print(FULL_METRICS_URL)
 
 
 @responses.activate
 def test_aggregate_and_send_metrics():
@@ -21,33 +31,48 @@
     cache = FileCache("TestCache")
     cache.set(METRIC_LAST_SENT_TIME, start_time)
     strategies = [RemoteAddress(parameters={"IPs": IP_LIST}), Default()]
     my_feature1 = Feature("My Feature1", True, strategies)
     my_feature1.yes_count = 1
     my_feature1.no_count = 1
 
-    my_feature2 = Feature("My Feature2", True, strategies)
+    my_feature2 = Feature(
+        "My Feature2", True, strategies, variants=Variants(VARIANTS, "My Feature2")
+    )
     my_feature2.yes_count = 2
     my_feature2.no_count = 2
 
+    feature2_variant_counts = {
+        "VarA": 56,
+        "VarB": 0,
+        "VarC": 4,
+    }
+    my_feature2.variant_counts = feature2_variant_counts
+
     my_feature3 = Feature("My Feature3", True, strategies)
     my_feature3.yes_count = 0
     my_feature3.no_count = 0
 
     features = {"My Feature1": my_feature1, "My Feature 2": my_feature2}
 
-    aggregate_and_send_metrics(URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS, features, cache)
+    aggregate_and_send_metrics(
+        URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS, features, cache
+    )
 
     assert len(responses.calls) == 1
     request = json.loads(responses.calls[0].request.body)
 
-    assert len(request['bucket']["toggles"].keys()) == 2
-    assert request['bucket']["toggles"]["My Feature1"]["yes"] == 1
-    assert request['bucket']["toggles"]["My Feature1"]["no"] == 1
-    assert "My Feature3" not in request['bucket']["toggles"].keys()
+    assert len(request["bucket"]["toggles"].keys()) == 2
+    assert request["bucket"]["toggles"]["My Feature1"]["yes"] == 1
+    assert request["bucket"]["toggles"]["My Feature1"]["no"] == 1
+    assert (
+        request["bucket"]["toggles"]["My Feature2"]["variants"]
+        == feature2_variant_counts
+    )
+    assert "My Feature3" not in request["bucket"]["toggles"].keys()
     assert cache.get(METRIC_LAST_SENT_TIME) > start_time
 
 
 @responses.activate
 def test_no_metrics():
     responses.add(responses.POST, FULL_METRICS_URL, json={}, status=200)
 
@@ -58,10 +83,12 @@
 
     my_feature1 = Feature("My Feature1", True, strategies)
     my_feature1.yes_count = 0
     my_feature1.no_count = 0
 
     features = {"My Feature1": my_feature1}
 
-    aggregate_and_send_metrics(URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS, features, cache)
+    aggregate_and_send_metrics(
+        URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS, features, cache
+    )
 
     assert len(responses.calls) == 0
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/periodic/test_fetch_and_load.py` & `UnleashClient-5.7.0/tests/unit_tests/periodic/test_fetch_and_load.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,113 @@
 import responses
-from UnleashClient.constants import FEATURES_URL, ETAG
-from UnleashClient.periodic_tasks import fetch_and_load_features
-from UnleashClient.features import Feature
-from tests.utilities.mocks.mock_features import MOCK_FEATURE_RESPONSE, MOCK_FEATURE_RESPONSE_PROJECT
-from tests.utilities.testing_constants import URL, APP_NAME, INSTANCE_ID, CUSTOM_HEADERS, CUSTOM_OPTIONS, DEFAULT_STRATEGY_MAPPING, PROJECT_URL, PROJECT_NAME, ETAG_VALUE
 
+from tests.utilities.mocks.mock_features import (
+    MOCK_FEATURE_RESPONSE,
+    MOCK_FEATURE_RESPONSE_PROJECT,
+)
+from tests.utilities.testing_constants import (
+    APP_NAME,
+    CUSTOM_HEADERS,
+    CUSTOM_OPTIONS,
+    DEFAULT_STRATEGY_MAPPING,
+    ETAG_VALUE,
+    INSTANCE_ID,
+    PROJECT_NAME,
+    PROJECT_URL,
+    URL,
+)
+from UnleashClient.constants import ETAG, FEATURES_URL
+from UnleashClient.features import Feature
+from UnleashClient.periodic_tasks import fetch_and_load_features
 
 FULL_FEATURE_URL = URL + FEATURES_URL
 
 
 @responses.activate
 def test_fetch_and_load(cache_empty):  # noqa: F811
     # Set up for tests
     in_memory_features = {}
-    responses.add(responses.GET, FULL_FEATURE_URL, json=MOCK_FEATURE_RESPONSE, status=200, headers={'etag': ETAG_VALUE})
+    responses.add(
+        responses.GET,
+        FULL_FEATURE_URL,
+        json=MOCK_FEATURE_RESPONSE,
+        status=200,
+        headers={"etag": ETAG_VALUE},
+    )
     temp_cache = cache_empty
 
-    fetch_and_load_features(URL,
-                            APP_NAME,
-                            INSTANCE_ID,
-                            CUSTOM_HEADERS,
-                            CUSTOM_OPTIONS,
-                            temp_cache,
-                            in_memory_features,
-                            DEFAULT_STRATEGY_MAPPING)
+    fetch_and_load_features(
+        URL,
+        APP_NAME,
+        INSTANCE_ID,
+        CUSTOM_HEADERS,
+        CUSTOM_OPTIONS,
+        temp_cache,
+        in_memory_features,
+        DEFAULT_STRATEGY_MAPPING,
+    )
 
     assert isinstance(in_memory_features["testFlag"], Feature)
     assert temp_cache.get(ETAG) == ETAG_VALUE
 
 
 @responses.activate
 def test_fetch_and_load_project(cache_empty):  # noqa: F811
     # Set up for tests
     in_memory_features = {}
-    responses.add(responses.GET, PROJECT_URL, json=MOCK_FEATURE_RESPONSE_PROJECT, status=200)
+    responses.add(
+        responses.GET, PROJECT_URL, json=MOCK_FEATURE_RESPONSE_PROJECT, status=200
+    )
     temp_cache = cache_empty
 
-    fetch_and_load_features(URL,
-                            APP_NAME,
-                            INSTANCE_ID,
-                            CUSTOM_HEADERS,
-                            CUSTOM_OPTIONS,
-                            temp_cache,
-                            in_memory_features,
-                            DEFAULT_STRATEGY_MAPPING,
-                            PROJECT_NAME)
+    fetch_and_load_features(
+        URL,
+        APP_NAME,
+        INSTANCE_ID,
+        CUSTOM_HEADERS,
+        CUSTOM_OPTIONS,
+        temp_cache,
+        in_memory_features,
+        DEFAULT_STRATEGY_MAPPING,
+        PROJECT_NAME,
+    )
 
     assert len(in_memory_features.keys()) == 1
     assert isinstance(in_memory_features["ivan-project"], Feature)
 
 
 @responses.activate
 def test_fetch_and_load_failure(cache_empty):  # noqa: F811
     # Set up for tests
     in_memory_features = {}
-    responses.add(responses.GET, FULL_FEATURE_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, FULL_FEATURE_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     temp_cache = cache_empty
 
-    fetch_and_load_features(URL,
-                            APP_NAME,
-                            INSTANCE_ID,
-                            CUSTOM_HEADERS,
-                            CUSTOM_OPTIONS,
-                            temp_cache,
-                            in_memory_features,
-                            DEFAULT_STRATEGY_MAPPING)
+    fetch_and_load_features(
+        URL,
+        APP_NAME,
+        INSTANCE_ID,
+        CUSTOM_HEADERS,
+        CUSTOM_OPTIONS,
+        temp_cache,
+        in_memory_features,
+        DEFAULT_STRATEGY_MAPPING,
+    )
 
     # Fail next request
     responses.reset()
     responses.add(responses.GET, FULL_FEATURE_URL, json={}, status=500)
 
-    fetch_and_load_features(URL,
-                            APP_NAME,
-                            INSTANCE_ID,
-                            CUSTOM_HEADERS,
-                            CUSTOM_OPTIONS,
-                            temp_cache,
-                            in_memory_features,
-                            DEFAULT_STRATEGY_MAPPING)
+    fetch_and_load_features(
+        URL,
+        APP_NAME,
+        INSTANCE_ID,
+        CUSTOM_HEADERS,
+        CUSTOM_OPTIONS,
+        temp_cache,
+        in_memory_features,
+        DEFAULT_STRATEGY_MAPPING,
+    )
 
     assert isinstance(in_memory_features["testFlag"], Feature)
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/strategies/test_remoteaddress.py` & `UnleashClient-5.7.0/tests/unit_tests/strategies/test_remoteaddress.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
-from UnleashClient.strategies import RemoteAddress
+
 from tests.utilities.testing_constants import IP_LIST
+from UnleashClient.strategies import RemoteAddress
 
 
 @pytest.fixture()
 def strategy():
     yield RemoteAddress(parameters={"IPs": IP_LIST})
 
 
@@ -25,16 +26,20 @@
 
 
 def test_ipv4_value(strategy):
     assert strategy.execute(context={"remoteAddress": "70.208.1.1"})
 
 
 def test_ipv6_rangee(strategy):
-    assert strategy.execute(context={"remoteAddress": "2001:db8:1234:0000:0000:0000:0000:0001"})
+    assert strategy.execute(
+        context={"remoteAddress": "2001:db8:1234:0000:0000:0000:0000:0001"}
+    )
 
 
 def test_ipv6_value(strategy):
-    assert strategy.execute(context={"remoteAddress": "2002:db8:1234:0000:0000:0000:0000:0001"})
+    assert strategy.execute(
+        context={"remoteAddress": "2002:db8:1234:0000:0000:0000:0000:0001"}
+    )
 
 
 def test_garbage_value(strategy):
     assert not strategy.execute(context={"remoteAddress": "WTFISTHISURCRAZY"})
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/test_client.py` & `UnleashClient-5.7.0/tests/unit_tests/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,51 @@
-import time
 import json
+import time
 import warnings
 from pathlib import Path
 
 import pytest
 import responses
-from apscheduler.schedulers.background import BackgroundScheduler
 from apscheduler.executors.pool import ThreadPoolExecutor
+from apscheduler.schedulers.background import BackgroundScheduler
 from blinker import signal
 
-from UnleashClient import UnleashClient, INSTANCES
-from UnleashClient.strategies import Strategy
-from UnleashClient.utils import InstanceAllowType
-from tests.utilities.testing_constants import URL, ENVIRONMENT, APP_NAME, INSTANCE_ID, REFRESH_INTERVAL, REFRESH_JITTER, \
-    METRICS_INTERVAL, METRICS_JITTER, DISABLE_METRICS, DISABLE_REGISTRATION, CUSTOM_HEADERS, CUSTOM_OPTIONS, PROJECT_NAME, PROJECT_URL, \
-    ETAG_VALUE
-from tests.utilities.mocks.mock_features import MOCK_FEATURE_RESPONSE, MOCK_FEATURE_RESPONSE_PROJECT
 from tests.utilities.mocks.mock_all_features import MOCK_ALL_FEATURES
-from UnleashClient.constants import REGISTER_URL, FEATURES_URL, METRICS_URL
+from tests.utilities.mocks.mock_features import (
+    MOCK_FEATURE_RESPONSE,
+    MOCK_FEATURE_RESPONSE_PROJECT,
+)
+from tests.utilities.testing_constants import (
+    APP_NAME,
+    CUSTOM_HEADERS,
+    CUSTOM_OPTIONS,
+    DISABLE_METRICS,
+    DISABLE_REGISTRATION,
+    ENVIRONMENT,
+    ETAG_VALUE,
+    INSTANCE_ID,
+    METRICS_INTERVAL,
+    METRICS_JITTER,
+    PROJECT_NAME,
+    PROJECT_URL,
+    REFRESH_INTERVAL,
+    REFRESH_JITTER,
+    URL,
+)
+from UnleashClient import INSTANCES, UnleashClient
 from UnleashClient.cache import FileCache
+from UnleashClient.constants import FEATURES_URL, METRICS_URL, REGISTER_URL
 from UnleashClient.events import UnleashEvent, UnleashEventType
+from UnleashClient.strategies import Strategy
+from UnleashClient.utils import InstanceAllowType
 
 
 class EnvironmentStrategy(Strategy):
     def load_provisioning(self) -> list:
-        return [x.strip() for x in self.parameters["environments"].split(',')]
+        return [x.strip() for x in self.parameters["environments"].split(",")]
 
     def apply(self, context: dict = None) -> bool:
         """
         Turn on if environemnt is a match.
 
         :return:
         """
@@ -53,81 +70,83 @@
 @pytest.fixture()
 def unleash_client(cache):
     unleash_client = UnleashClient(
         URL,
         APP_NAME,
         refresh_interval=REFRESH_INTERVAL,
         metrics_interval=METRICS_INTERVAL,
-        cache=cache
+        cache=cache,
     )
     yield unleash_client
     unleash_client.destroy()
 
 
 @pytest.fixture()
 def unleash_client_project(cache):
     unleash_client = UnleashClient(
         URL,
         APP_NAME,
         refresh_interval=REFRESH_INTERVAL,
         metrics_interval=METRICS_INTERVAL,
         cache=cache,
-        project_name=PROJECT_NAME
+        project_name=PROJECT_NAME,
     )
     yield unleash_client
     unleash_client.destroy()
 
 
 @pytest.fixture()
 def unleash_client_nodestroy(cache):
     unleash_client = UnleashClient(
         URL,
         APP_NAME,
         refresh_interval=REFRESH_INTERVAL,
         metrics_interval=METRICS_INTERVAL,
-        cache=cache
+        cache=cache,
     )
     yield unleash_client
 
 
 @pytest.fixture()
 def unleash_client_toggle_only(cache):
     unleash_client = UnleashClient(
         URL,
         APP_NAME,
         refresh_interval=REFRESH_INTERVAL,
         metrics_interval=METRICS_INTERVAL,
         disable_registration=True,
         disable_metrics=True,
-        cache=cache
+        cache=cache,
     )
     yield unleash_client
     unleash_client.destroy()
 
 
 def test_UC_initialize_default():
     client = UnleashClient(URL, APP_NAME)
     assert client.unleash_url == URL
     assert client.unleash_app_name == APP_NAME
     assert client.unleash_metrics_interval == 60
 
 
 def test_UC_initialize_full():
-    client = UnleashClient(URL,
-                           APP_NAME,
-                           ENVIRONMENT,
-                           INSTANCE_ID,
-                           REFRESH_INTERVAL,
-                           REFRESH_JITTER,
-                           METRICS_INTERVAL,
-                           METRICS_JITTER,
-                           DISABLE_METRICS,
-                           DISABLE_REGISTRATION,
-                           CUSTOM_HEADERS,
-                           CUSTOM_OPTIONS)
+    client = UnleashClient(
+        URL,
+        APP_NAME,
+        ENVIRONMENT,
+        INSTANCE_ID,
+        REFRESH_INTERVAL,
+        REFRESH_JITTER,
+        METRICS_INTERVAL,
+        METRICS_JITTER,
+        DISABLE_METRICS,
+        DISABLE_REGISTRATION,
+        CUSTOM_HEADERS,
+        CUSTOM_OPTIONS,
+    )
     assert client.unleash_instance_id == INSTANCE_ID
     assert client.unleash_refresh_interval == REFRESH_INTERVAL
     assert client.unleash_refresh_jitter == REFRESH_JITTER
     assert client.unleash_metrics_interval == METRICS_INTERVAL
     assert client.unleash_metrics_jitter == METRICS_JITTER
     assert client.unleash_disable_metrics == DISABLE_METRICS
     assert client.unleash_disable_registration == DISABLE_REGISTRATION
@@ -142,53 +161,75 @@
     assert client.unleash_refresh_interval == "60"
 
 
 @responses.activate
 def test_uc_lifecycle(unleash_client):
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200, headers={'etag': ETAG_VALUE})
+    responses.add(
+        responses.GET,
+        URL + FEATURES_URL,
+        json=MOCK_FEATURE_RESPONSE,
+        status=200,
+        headers={"etag": ETAG_VALUE},
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
     assert unleash_client.is_initialized
     assert len(unleash_client.features) >= 4
 
     # Simulate caching
-    responses.add(responses.GET, URL + FEATURES_URL, json={}, status=304, headers={'etag': ETAG_VALUE})
+    responses.add(
+        responses.GET,
+        URL + FEATURES_URL,
+        json={},
+        status=304,
+        headers={"etag": ETAG_VALUE},
+    )
     time.sleep(16)
 
     # Simulate server provisioning change
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_ALL_FEATURES, status=200, headers={'etag': 'W/somethingelse'})
+    responses.add(
+        responses.GET,
+        URL + FEATURES_URL,
+        json=MOCK_ALL_FEATURES,
+        status=200,
+        headers={"etag": "W/somethingelse"},
+    )
     time.sleep(30)
     assert len(unleash_client.features) >= 9
 
 
 @responses.activate
 def test_uc_is_enabled(unleash_client):
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
     assert unleash_client.is_enabled("testFlag")
 
 
 @responses.activate
 def test_uc_project(unleash_client_project):
     unleash_client = unleash_client_project
 
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, PROJECT_URL, json=MOCK_FEATURE_RESPONSE_PROJECT, status=200)
+    responses.add(
+        responses.GET, PROJECT_URL, json=MOCK_FEATURE_RESPONSE_PROJECT, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
     assert unleash_client.is_enabled("ivan-project")
 
@@ -198,45 +239,51 @@
     def good_fallback(feature_name: str, context: dict) -> bool:
         return True
 
     def bad_fallback(feature_name: str, context: dict) -> bool:
         return False
 
     def context_fallback(feature_name: str, context: dict) -> bool:
-        return context['wat']
+        return context["wat"]
 
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
     fallback_spy = mocker.Mock(wraps=good_fallback)
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
     # Non-existent feature flag, fallback_function
     assert unleash_client.is_enabled("notFoundTestFlag", fallback_function=fallback_spy)
     assert fallback_spy.call_count == 1
     fallback_spy.reset_mock()
 
     # Non-existent feature flag, default value, fallback_function
-    assert not unleash_client.is_enabled("notFoundTestFlag", fallback_function=bad_fallback)
+    assert not unleash_client.is_enabled(
+        "notFoundTestFlag", fallback_function=bad_fallback
+    )
     assert fallback_spy.call_count == 0
 
     # Existent feature flag, fallback_function
     assert unleash_client.is_enabled("testFlag", fallback_function=good_fallback)
     assert fallback_spy.call_count == 0
 
 
 @responses.activate
 def test_uc_dirty_cache(unleash_client_nodestroy):
     unleash_client = unleash_client_nodestroy
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(5)
     assert unleash_client.is_enabled("testFlag")
     unleash_client.unleash_scheduler.shutdown()
@@ -247,162 +294,206 @@
     assert unleash_client.is_enabled("testFlag")
 
 
 @responses.activate
 def test_uc_is_enabled_with_context():
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
-    custom_strategies_dict = {
-        "custom-context": EnvironmentStrategy
-    }
+    custom_strategies_dict = {"custom-context": EnvironmentStrategy}
 
-    unleash_client = UnleashClient(URL, APP_NAME, environment='prod', custom_strategies=custom_strategies_dict)
+    unleash_client = UnleashClient(
+        URL, APP_NAME, environment="prod", custom_strategies=custom_strategies_dict
+    )
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
 
     time.sleep(1)
     assert unleash_client.is_enabled("testContextFlag")
     unleash_client.destroy()
 
 
 @responses.activate
 def test_uc_is_enabled_error_states(unleash_client):
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
     assert not unleash_client.is_enabled("ThisFlagDoesn'tExist")
-    assert unleash_client.is_enabled("ThisFlagDoesn'tExist", fallback_function=lambda x, y: True)
+    assert unleash_client.is_enabled(
+        "ThisFlagDoesn'tExist", fallback_function=lambda x, y: True
+    )
 
 
 @responses.activate
 def test_uc_context_manager(unleash_client_nodestroy):
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     with unleash_client_nodestroy as unleash_client:
         assert unleash_client.is_initialized
 
 
 @responses.activate
 def test_uc_not_initialized_isenabled():
     unleash_client = UnleashClient(URL, APP_NAME)
     assert not unleash_client.is_enabled("ThisFlagDoesn'tExist")
-    assert unleash_client.is_enabled("ThisFlagDoesn'tExist", fallback_function=lambda x, y: True)
+    assert unleash_client.is_enabled(
+        "ThisFlagDoesn'tExist", fallback_function=lambda x, y: True
+    )
 
 
 @responses.activate
 def test_uc_get_variant():
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     unleash_client = UnleashClient(URL, APP_NAME)
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
 
     time.sleep(1)
     # If feature flag is on.
-    variant = unleash_client.get_variant("testVariations", context={'userId': '2'})
-    assert variant['name'] == 'VarA'
-    assert variant['enabled']
+    variant = unleash_client.get_variant("testVariations", context={"userId": "2"})
+    assert variant["name"] == "VarA"
+    assert variant["enabled"]
 
     # If feature flag is not.
-    variant = unleash_client.get_variant("testVariations", context={'userId': '3'})
-    assert variant['name'] == 'disabled'
-    assert not variant['enabled']
+    variant = unleash_client.get_variant("testVariations", context={"userId": "3"})
+    assert variant["name"] == "disabled"
+    assert not variant["enabled"]
 
     unleash_client.destroy()
 
 
 @responses.activate
 def test_uc_not_initialized_getvariant():
     unleash_client = UnleashClient(URL, APP_NAME)
     variant = unleash_client.get_variant("ThisFlagDoesn'tExist")
-    assert not variant['enabled']
-    assert variant['name'] == 'disabled'
+    assert not variant["enabled"]
+    assert variant["name"] == "disabled"
 
 
 @responses.activate
 def test_uc_metrics(unleash_client):
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
     assert unleash_client.is_enabled("testFlag")
 
     time.sleep(12)
     request = json.loads(responses.calls[-1].request.body)
-    assert request['bucket']["toggles"]["testFlag"]["yes"] == 1
+    assert request["bucket"]["toggles"]["testFlag"]["yes"] == 1
 
 
 @responses.activate
-def test_uc_disabled_registration(unleash_client_toggle_only):
-    unleash_client = unleash_client_toggle_only
-    # Set up APIs
-    responses.add(responses.POST, URL + REGISTER_URL, json={}, status=401)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
-    responses.add(responses.POST, URL + METRICS_URL, json={}, status=401)
+def test_uc_registers_metrics_for_nonexistent_features(unleash_client):
+    # Set up API
+    responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
+    responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
+    # Create Unleash client and check initial load
     unleash_client.initialize_client()
-    unleash_client.is_enabled("testFlag")
-    time.sleep(20)
-    assert unleash_client.is_enabled("testFlag")
+    time.sleep(1)
 
-    for api_call in responses.calls:
-        assert '/api/client/features' in api_call.request.url
+    # Check a flag that doesn't exist
+    unleash_client.is_enabled("nonexistent-flag")
+
+    # Verify that the metrics are serialized
+    time.sleep(12)
+    request = json.loads(responses.calls[-1].request.body)
+    assert request["bucket"]["toggles"]["nonexistent-flag"]["no"] == 1
 
 
 @responses.activate
-def test_uc_server_error(unleash_client):
-    # Verify that Unleash Client will still fall back gracefully if SERVER ANGRY RAWR, and then recover gracefully.
+def test_uc_registers_variant_metrics_for_nonexistent_features(unleash_client):
+    # Set up API
+    responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
+    responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
-    unleash_client = unleash_client
+    # Create Unleash client and check initial load
+    unleash_client.initialize_client()
+    time.sleep(1)
+
+    # Check a flag that doesn't exist
+    unleash_client.get_variant("nonexistent-flag")
+
+    # Verify that the metrics are serialized
+    time.sleep(12)
+    request = json.loads(responses.calls[-1].request.body)
+    assert request["bucket"]["toggles"]["nonexistent-flag"]["no"] == 1
+    assert request["bucket"]["toggles"]["nonexistent-flag"]["variants"]["disabled"] == 1
+
+
+@responses.activate
+def test_uc_disabled_registration(unleash_client_toggle_only):
+    unleash_client = unleash_client_toggle_only
     # Set up APIs
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=401)
-    responses.add(responses.GET, URL + FEATURES_URL, status=500)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=401)
 
     unleash_client.initialize_client()
-    assert not unleash_client.is_enabled("testFlag")
-
-    responses.remove(responses.GET, URL + FEATURES_URL)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    unleash_client.is_enabled("testFlag")
     time.sleep(20)
     assert unleash_client.is_enabled("testFlag")
 
+    for api_call in responses.calls:
+        assert "/api/client/features" in api_call.request.url
+
 
 @responses.activate
-def test_uc_server_error_recovery(unleash_client):
+def test_uc_server_error(unleash_client):
     # Verify that Unleash Client will still fall back gracefully if SERVER ANGRY RAWR, and then recover gracefully.
 
     unleash_client = unleash_client
     # Set up APIs
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=401)
     responses.add(responses.GET, URL + FEATURES_URL, status=500)
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=401)
 
     unleash_client.initialize_client()
     assert not unleash_client.is_enabled("testFlag")
 
     responses.remove(responses.GET, URL + FEATURES_URL)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     time.sleep(20)
     assert unleash_client.is_enabled("testFlag")
 
 
 def test_uc_with_invalid_url():
     unleash_client = UnleashClient("thisisnotavalidurl", APP_NAME)
 
@@ -417,15 +508,21 @@
     assert unleash_client.is_enabled
 
 
 @responses.activate
 def test_uc_multiple_initializations(unleash_client):
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200, headers={'etag': ETAG_VALUE})
+    responses.add(
+        responses.GET,
+        URL + FEATURES_URL,
+        json=MOCK_FEATURE_RESPONSE,
+        status=200,
+        headers={"etag": ETAG_VALUE},
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
     assert unleash_client.is_initialized
     assert len(unleash_client.features) >= 4
@@ -438,27 +535,33 @@
     assert "initialize" in str(w[0].message)
 
 
 @responses.activate
 def test_uc_cache_bootstrap_dict(cache):
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200, headers={'etag': ETAG_VALUE})
+    responses.add(
+        responses.GET,
+        URL + FEATURES_URL,
+        json=MOCK_FEATURE_RESPONSE,
+        status=200,
+        headers={"etag": ETAG_VALUE},
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Set up cache
     cache.bootstrap_from_dict(initial_config=MOCK_FEATURE_RESPONSE_PROJECT)
 
     # Check bootstrapping
     unleash_client = UnleashClient(
         URL,
         APP_NAME,
         refresh_interval=REFRESH_INTERVAL,
         metrics_interval=METRICS_INTERVAL,
-        cache=cache
+        cache=cache,
     )
     assert len(unleash_client.features) == 1
     assert unleash_client.is_enabled("ivan-project")
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
@@ -466,86 +569,112 @@
     assert len(unleash_client.features) >= 4
     assert unleash_client.is_enabled("testFlag")
 
 
 @responses.activate
 def test_uc_cache_bootstrap_file(cache):
     # Set up cache
-    test_file = Path(Path(__file__).parent.resolve(), '..', 'utilities', 'mocks', 'mock_bootstrap.json')
+    test_file = Path(
+        Path(__file__).parent.resolve(),
+        "..",
+        "utilities",
+        "mocks",
+        "mock_bootstrap.json",
+    )
     cache.bootstrap_from_file(initial_config_file=test_file)
 
     # Check bootstrapping
     unleash_client = UnleashClient(
         URL,
         APP_NAME,
         refresh_interval=REFRESH_INTERVAL,
         metrics_interval=METRICS_INTERVAL,
-        cache=cache
+        cache=cache,
     )
     assert len(unleash_client.features) >= 1
     assert unleash_client.is_enabled("ivan-project")
 
 
 @responses.activate
 def test_uc_cache_bootstrap_url(cache):
     # Set up API
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200, headers={'etag': ETAG_VALUE})
+    responses.add(
+        responses.GET,
+        URL + FEATURES_URL,
+        json=MOCK_FEATURE_RESPONSE,
+        status=200,
+        headers={"etag": ETAG_VALUE},
+    )
 
     # Set up cache
     cache.bootstrap_from_url(initial_config_url=URL + FEATURES_URL)
 
     # Check bootstrapping
     unleash_client = UnleashClient(
         URL,
         APP_NAME,
         refresh_interval=REFRESH_INTERVAL,
         metrics_interval=METRICS_INTERVAL,
-        cache=cache
+        cache=cache,
     )
     assert len(unleash_client.features) >= 4
     assert unleash_client.is_enabled("testFlag")
 
 
 @responses.activate
 def test_uc_custom_scheduler():
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200, headers={'etag': ETAG_VALUE})
+    responses.add(
+        responses.GET,
+        URL + FEATURES_URL,
+        json=MOCK_FEATURE_RESPONSE,
+        status=200,
+        headers={"etag": ETAG_VALUE},
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Set up UnleashClient
-    custom_executors = {
-        'hamster_executor': ThreadPoolExecutor()
-    }
+    custom_executors = {"hamster_executor": ThreadPoolExecutor()}
 
-    custom_scheduler = BackgroundScheduler(
-        executors=custom_executors
-    )
+    custom_scheduler = BackgroundScheduler(executors=custom_executors)
 
     unleash_client = UnleashClient(
         URL,
         APP_NAME,
         refresh_interval=5,
         metrics_interval=10,
         scheduler=custom_scheduler,
-        scheduler_executor='hamster_executor'
+        scheduler_executor="hamster_executor",
     )
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
     assert unleash_client.is_initialized
     assert len(unleash_client.features) >= 4
 
     # Simulate caching
-    responses.add(responses.GET, URL + FEATURES_URL, json={}, status=304, headers={'etag': ETAG_VALUE})
+    responses.add(
+        responses.GET,
+        URL + FEATURES_URL,
+        json={},
+        status=304,
+        headers={"etag": ETAG_VALUE},
+    )
     time.sleep(6)
 
     # Simulate server provisioning change
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_ALL_FEATURES, status=200, headers={'etag': 'W/somethingelse'})
+    responses.add(
+        responses.GET,
+        URL + FEATURES_URL,
+        json=MOCK_ALL_FEATURES,
+        status=200,
+        headers={"etag": "W/somethingelse"},
+    )
     time.sleep(6)
     assert len(unleash_client.features) >= 9
 
 
 def test_multiple_instances_blocks_client_instantiation():
     with pytest.raises(Exception):
         UnleashClient(URL, APP_NAME, multiple_instance_mode=InstanceAllowType.BLOCK)
@@ -564,62 +693,83 @@
     UnleashClient(URL, APP_NAME, multiple_instance_mode=InstanceAllowType.WARN)
     assert any(["You already have 1 instance" in r.msg for r in caplog.records])
     assert any(["You already have 2 instance(s)" in r.msg for r in caplog.records])
 
 
 def test_multiple_instances_no_warnings_or_errors_with_different_client_configs(caplog):
     UnleashClient(URL, "some-probably-unique-app-name")
-    UnleashClient(URL, "some-probably-unique-app-name", instance_id="some-unique-instance-id", refresh_interval="60")
-    UnleashClient(URL, "some-probably-unique-but-different-app-name", refresh_interval="60")
-    assert not all(["Multiple instances has been disabled" in r.msg for r in caplog.records])
+    UnleashClient(
+        URL,
+        "some-probably-unique-app-name",
+        instance_id="some-unique-instance-id",
+        refresh_interval="60",
+    )
+    UnleashClient(
+        URL, "some-probably-unique-but-different-app-name", refresh_interval="60"
+    )
+    assert not any(
+        ["Multiple instances has been disabled" in r.msg for r in caplog.records]
+    )
 
 
 def test_multiple_instances_are_unique_on_api_key(caplog):
-    UnleashClient(URL, "some-probably-unique-app-name", custom_headers={"Authorization": "penguins"})
-    UnleashClient(URL, "some-probably-unique-app-name", custom_headers={"Authorization": "hamsters"})
-    assert not all(["Multiple instances has been disabled" in r.msg for r in caplog.records])
+    UnleashClient(
+        URL,
+        "some-probably-unique-app-name",
+        custom_headers={"Authorization": "penguins"},
+    )
+    UnleashClient(
+        URL,
+        "some-probably-unique-app-name",
+        custom_headers={"Authorization": "hamsters"},
+    )
+    assert not any(
+        ["Multiple instances has been disabled" in r.msg for r in caplog.records]
+    )
 
 
 @responses.activate
 def test_signals_feature_flag(cache):
     # Set up API
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_FEATURE_RESPONSE, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
     # Set up signals
-    send_data = signal('send-data')
+    send_data = signal("send-data")
 
     @send_data.connect
     def receive_data(sender, **kw):
         print("Caught signal from %r, data %r" % (sender, kw))
 
-        if kw['data'].event_type == UnleashEventType.FEATURE_FLAG:
-            assert kw['data'].feature_name == 'testFlag'
-            assert kw['data'].enabled
-        elif kw['data'].event_type == UnleashEventType.VARIANT:
-            assert kw['data'].feature_name == 'testVariations'
-            assert kw['data'].enabled
-            assert kw['data'].variant == 'VarA'
+        if kw["data"].event_type == UnleashEventType.FEATURE_FLAG:
+            assert kw["data"].feature_name == "testFlag"
+            assert kw["data"].enabled
+        elif kw["data"].event_type == UnleashEventType.VARIANT:
+            assert kw["data"].feature_name == "testVariations"
+            assert kw["data"].enabled
+            assert kw["data"].variant == "VarA"
 
         raise Exception("Random!")
 
     def example_callback(event: UnleashEvent):
-        send_data.send('anonymous', data=event)
+        send_data.send("anonymous", data=event)
 
     # Set up Unleash
     unleash_client = UnleashClient(
         URL,
         APP_NAME,
         refresh_interval=REFRESH_INTERVAL,
         metrics_interval=METRICS_INTERVAL,
         cache=cache,
-        event_callback=example_callback
+        event_callback=example_callback,
     )
 
     # Create Unleash client and check initial load
     unleash_client.initialize_client()
     time.sleep(1)
 
     assert unleash_client.is_enabled("testFlag")
-    variant = unleash_client.get_variant("testVariations", context={'userId': '2'})
-    assert variant['name'] == 'VarA'
+    variant = unleash_client.get_variant("testVariations", context={"userId": "2"})
+    assert variant["name"] == "VarA"
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/test_constraints.py` & `UnleashClient-5.7.0/tests/unit_tests/test_constraints.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from datetime import datetime
-import pytz
+
 import pytest
-from UnleashClient.constraints import Constraint
+import pytz
+
 from tests.utilities.mocks import mock_constraints
+from UnleashClient.constraints import Constraint
 
 
 @pytest.fixture()
 def constraint_IN():
     yield Constraint(mock_constraints.CONSTRAINT_DICT_IN)
 
 
 @pytest.fixture()
 def constraint_NOTIN():
     yield Constraint(mock_constraints.CONSTRAINT_DICT_NOTIN)
 
 
 def test_constraint_IN_match(constraint_IN):
     constraint = constraint_IN
-    context = {
-        'appName': 'test'
-    }
+    context = {"appName": "test"}
 
     assert constraint.apply(context)
 
 
 def test_constraint_IN_not_match(constraint_IN):
     constraint = constraint_IN
-    context = {
-        'appName': 'test3'
-    }
+    context = {"appName": "test3"}
 
     assert not constraint.apply(context)
 
 
 def test_constraint_IN_missingcontext(constraint_IN):
     constraint = constraint_IN
     assert not constraint.apply({})
@@ -46,171 +44,181 @@
 def test_constraint_NOTIN_missingcontext_inversion():
     constraint = Constraint(mock_constraints.CONSTRAINT_DICT_NOTIN_INVERT)
     assert not constraint.apply({})
 
 
 def test_constraint_NOTIN_match(constraint_NOTIN):
     constraint = constraint_NOTIN
-    context = {
-        'appName': 'test'
-    }
+    context = {"appName": "test"}
 
     assert not constraint.apply(context)
 
 
 def test_constraint_NOTIN_not_match(constraint_NOTIN):
     constraint = constraint_NOTIN
-    context = {
-        'appName': 'test3'
-    }
+    context = {"appName": "test3"}
 
     assert constraint.apply(context)
 
 
 def test_constraint_inversion():
-    constraint_ci = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_INVERT)
+    constraint_ci = Constraint(
+        constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_INVERT
+    )
 
-    assert not constraint_ci.apply({'customField': "adogb"})
+    assert not constraint_ci.apply({"customField": "adogb"})
 
 
 def test_constraint_STR_CONTAINS():
-    constraint_not_ci = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_CONTAINS_NOT_CI)
-    constraint_ci = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_CONTAINS_CI)
-
-    assert constraint_ci.apply({'customField': "adogb"})
-    assert not constraint_ci.apply({'customField': "aparrotb"})
-    assert constraint_ci.apply({'customField': "ahamsterb"})
-
-    assert constraint_not_ci.apply({'customField': "adogb"})
-    assert not constraint_ci.apply({'customField': "aparrotb"})
-    assert not constraint_not_ci.apply({'customField': "ahamsterb"})
+    constraint_not_ci = Constraint(
+        constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_CONTAINS_NOT_CI
+    )
+    constraint_ci = Constraint(
+        constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_CONTAINS_CI
+    )
+
+    assert constraint_ci.apply({"customField": "adogb"})
+    assert not constraint_ci.apply({"customField": "aparrotb"})
+    assert constraint_ci.apply({"customField": "ahamsterb"})
+
+    assert constraint_not_ci.apply({"customField": "adogb"})
+    assert not constraint_ci.apply({"customField": "aparrotb"})
+    assert not constraint_not_ci.apply({"customField": "ahamsterb"})
 
 
 def test_constraint_STR_ENDS_WITH():
-    constraint_not_ci = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_ENDS_WITH_NOT_CI)
-    constraint_ci = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_ENDS_WITH_CI)
-
-    assert constraint_ci.apply({'customField': "adog"})
-    assert not constraint_ci.apply({'customField': "aparrot"})
-    assert constraint_ci.apply({'customField': "ahamster"})
-
-    assert constraint_not_ci.apply({'customField': "adog"})
-    assert not constraint_not_ci.apply({'customField': "aparrot"})
-    assert not constraint_not_ci.apply({'customField': "ahamster"})
+    constraint_not_ci = Constraint(
+        constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_ENDS_WITH_NOT_CI
+    )
+    constraint_ci = Constraint(
+        constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_ENDS_WITH_CI
+    )
+
+    assert constraint_ci.apply({"customField": "adog"})
+    assert not constraint_ci.apply({"customField": "aparrot"})
+    assert constraint_ci.apply({"customField": "ahamster"})
+
+    assert constraint_not_ci.apply({"customField": "adog"})
+    assert not constraint_not_ci.apply({"customField": "aparrot"})
+    assert not constraint_not_ci.apply({"customField": "ahamster"})
 
 
 def test_constraint_STR_STARTS_WITH():
-    constraint_not_ci = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_STARTS_WITH_NOT_CI)
-    constraint_ci = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_STARTS_WITH_CI)
-
-    assert constraint_ci.apply({'customField': "dogb"})
-    assert not constraint_ci.apply({'customField': "parrotb"})
-    assert constraint_ci.apply({'customField': "hamsterb"})
-
-    assert constraint_not_ci.apply({'customField': "dogb"})
-    assert not constraint_not_ci.apply({'customField': "parrotb"})
-    assert not constraint_not_ci.apply({'customField': "hamsterb"})
+    constraint_not_ci = Constraint(
+        constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_STARTS_WITH_NOT_CI
+    )
+    constraint_ci = Constraint(
+        constraint_dict=mock_constraints.CONSTRAINT_DICT_STR_STARTS_WITH_CI
+    )
+
+    assert constraint_ci.apply({"customField": "dogb"})
+    assert not constraint_ci.apply({"customField": "parrotb"})
+    assert constraint_ci.apply({"customField": "hamsterb"})
+
+    assert constraint_not_ci.apply({"customField": "dogb"})
+    assert not constraint_not_ci.apply({"customField": "parrotb"})
+    assert not constraint_not_ci.apply({"customField": "hamsterb"})
 
 
 def test_constraints_NUM_EQ():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_NUM_EQ)
 
-    assert not constraint.apply({'customField': 4})
-    assert constraint.apply({'customField': 5})
-    assert not constraint.apply({'customField': 6})
+    assert not constraint.apply({"customField": 4})
+    assert constraint.apply({"customField": 5})
+    assert not constraint.apply({"customField": 6})
 
 
 def test_constraints_NUM_GT():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_NUM_GT)
 
-    assert not constraint.apply({'customField': 4})
-    assert not constraint.apply({'customField': 5})
-    assert constraint.apply({'customField': 6})
+    assert not constraint.apply({"customField": 4})
+    assert not constraint.apply({"customField": 5})
+    assert constraint.apply({"customField": 6})
 
 
 def test_constraints_NUM_GTE():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_NUM_GTE)
 
-    assert not constraint.apply({'customField': 4})
-    assert constraint.apply({'customField': 5})
-    assert constraint.apply({'customField': 6})
+    assert not constraint.apply({"customField": 4})
+    assert constraint.apply({"customField": 5})
+    assert constraint.apply({"customField": 6})
 
 
 def test_constraints_NUM_LT():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_NUM_LT)
 
-    assert constraint.apply({'customField': 4})
-    assert not constraint.apply({'customField': 5})
-    assert not constraint.apply({'customField': 6})
+    assert constraint.apply({"customField": 4})
+    assert not constraint.apply({"customField": 5})
+    assert not constraint.apply({"customField": 6})
 
 
 def test_constraints_NUM_LTE():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_NUM_LTE)
 
-    assert constraint.apply({'customField': 4})
-    assert constraint.apply({'customField': 5})
-    assert not constraint.apply({'customField': 6})
+    assert constraint.apply({"customField": 4})
+    assert constraint.apply({"customField": 5})
+    assert not constraint.apply({"customField": 6})
 
 
 def test_constraints_NUM_FLOAT():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_NUM_FLOAT)
 
-    assert constraint.apply({'customField': 5})
-    assert constraint.apply({'customField': 5.1})
-    assert not constraint.apply({'customField': 5.2})
+    assert constraint.apply({"customField": 5})
+    assert constraint.apply({"customField": 5.1})
+    assert not constraint.apply({"customField": 5.2})
 
 
 def test_constraints_DATE_AFTER():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DATE_AFTER)
 
-    assert constraint.apply({'currentTime': datetime(2022, 1, 23, tzinfo=pytz.UTC)})
-    assert not constraint.apply({'currentTime': datetime(2022, 1, 22, tzinfo=pytz.UTC)})
-    assert not constraint.apply({'currentTime': datetime(2022, 1, 21, tzinfo=pytz.UTC)})
+    assert constraint.apply({"currentTime": datetime(2022, 1, 23, tzinfo=pytz.UTC)})
+    assert not constraint.apply({"currentTime": datetime(2022, 1, 22, tzinfo=pytz.UTC)})
+    assert not constraint.apply({"currentTime": datetime(2022, 1, 21, tzinfo=pytz.UTC)})
 
 
 def test_constraints_DATE_BEFORE():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DATE_BEFORE)
 
-    assert not constraint.apply({'currentTime': datetime(2022, 1, 23, tzinfo=pytz.UTC)})
-    assert not constraint.apply({'currentTime': datetime(2022, 1, 22, tzinfo=pytz.UTC)})
-    assert constraint.apply({'currentTime': datetime(2022, 1, 21, tzinfo=pytz.UTC)})
+    assert not constraint.apply({"currentTime": datetime(2022, 1, 23, tzinfo=pytz.UTC)})
+    assert not constraint.apply({"currentTime": datetime(2022, 1, 22, tzinfo=pytz.UTC)})
+    assert constraint.apply({"currentTime": datetime(2022, 1, 21, tzinfo=pytz.UTC)})
 
 
 def test_constraints_default():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DATE_BEFORE)
 
     assert not constraint.apply({})
 
 
 def test_constraints_date_error():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_DATE_ERROR)
-    assert not constraint.apply({'currentTime': datetime(2022, 1, 23)})
+    assert not constraint.apply({"currentTime": datetime(2022, 1, 23)})
 
 
 def test_constraints_SEMVER_EQ():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_SEMVER_EQ)
 
-    assert not constraint.apply({'customField': '1.2.1'})
-    assert constraint.apply({'customField': '1.2.2'})
-    assert not constraint.apply({'customField': '1.2.3'})
+    assert not constraint.apply({"customField": "1.2.1"})
+    assert constraint.apply({"customField": "1.2.2"})
+    assert not constraint.apply({"customField": "1.2.3"})
 
 
 def test_constraints_SEMVER_GT():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_SEMVER_GT)
 
-    assert not constraint.apply({'customField': '1.2.1'})
-    assert not constraint.apply({'customField': '1.2.2'})
-    assert constraint.apply({'customField': '1.2.3'})
+    assert not constraint.apply({"customField": "1.2.1"})
+    assert not constraint.apply({"customField": "1.2.2"})
+    assert constraint.apply({"customField": "1.2.3"})
 
 
 def test_constraints_SEMVER_LT():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_SEMVER_LT)
 
-    assert constraint.apply({'customField': '1.2.1'})
-    assert not constraint.apply({'customField': '1.2.2'})
-    assert not constraint.apply({'customField': '1.2.3'})
+    assert constraint.apply({"customField": "1.2.1"})
+    assert not constraint.apply({"customField": "1.2.2"})
+    assert not constraint.apply({"customField": "1.2.3"})
 
 
 def test_constraints_semverexception():
     constraint = Constraint(constraint_dict=mock_constraints.CONSTRAINT_SEMVER_EQ)
 
-    assert not constraint.apply({'customField': 'hamstershamsterhamsters'})
+    assert not constraint.apply({"customField": "hamstershamsterhamsters"})
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/test_custom_strategy.py` & `UnleashClient-5.7.0/tests/unit_tests/test_custom_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import responses
-from UnleashClient import UnleashClient
-from UnleashClient.strategies import Strategy
-from tests.utilities.testing_constants import URL, APP_NAME
+
 from tests.utilities.mocks import MOCK_CUSTOM_STRATEGY
 from tests.utilities.old_code.StrategyV2 import StrategyOldV2
-from UnleashClient.constants import REGISTER_URL, FEATURES_URL, METRICS_URL
+from tests.utilities.testing_constants import APP_NAME, URL
+from UnleashClient import UnleashClient
+from UnleashClient.constants import FEATURES_URL, METRICS_URL, REGISTER_URL
+from UnleashClient.strategies import Strategy
 
 
 class CatTest(Strategy):
     def load_provisioning(self) -> list:
-        return [x.strip() for x in self.parameters["sound"].split(',')]
+        return [x.strip() for x in self.parameters["sound"].split(",")]
 
     def apply(self, context: dict = None) -> bool:
         """
         Turn on if I'm a cat.
 
         :return:
         """
@@ -23,15 +24,15 @@
             default_value = context["sound"] in self.parsed_provisioning
 
         return default_value
 
 
 class DogTest(StrategyOldV2):
     def load_provisioning(self) -> list:
-        return [x.strip() for x in self.parameters["sound"].split(',')]
+        return [x.strip() for x in self.parameters["sound"].split(",")]
 
     def _call_(self, context: dict = None) -> bool:
         """
         Turn on if I'm a dog.
 
         :return:
         """
@@ -42,27 +43,24 @@
 
         return default_value
 
 
 @responses.activate
 def test_uc_customstrategy_happypath(recwarn):
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_CUSTOM_STRATEGY, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_CUSTOM_STRATEGY, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
-    custom_strategies_dict = {
-        "amIACat": CatTest,
-        "amIADog": DogTest
-    }
+    custom_strategies_dict = {"amIACat": CatTest, "amIADog": DogTest}
 
     unleash_client = UnleashClient(
-        URL,
-        APP_NAME,
-        environment="prod",
-        custom_strategies=custom_strategies_dict)
+        URL, APP_NAME, environment="prod", custom_strategies=custom_strategies_dict
+    )
 
     unleash_client.initialize_client()
 
     # Check custom strategy.
     assert unleash_client.is_enabled("CustomToggle", {"sound": "meow"})
     assert not unleash_client.is_enabled("CustomToggle", {"sound": "bark"})
 
@@ -70,48 +68,42 @@
     assert len(recwarn) >= 1
     assert any([x.category == DeprecationWarning for x in recwarn])
 
 
 @responses.activate
 def test_uc_customstrategy_depredationwarning():
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_CUSTOM_STRATEGY, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_CUSTOM_STRATEGY, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
-    custom_strategies_dict = {
-        "amIACat": CatTest,
-        "amIADog": DogTest
-    }
+    custom_strategies_dict = {"amIACat": CatTest, "amIADog": DogTest}
 
     unleash_client = UnleashClient(
-        URL,
-        APP_NAME,
-        environment="prod",
-        custom_strategies=custom_strategies_dict)
+        URL, APP_NAME, environment="prod", custom_strategies=custom_strategies_dict
+    )
 
     unleash_client.initialize_client()
 
     # Check a toggle that contains an outdated custom strategy
     assert unleash_client.is_enabled("CustomToggleWarning", {"sound": "meow"})
 
 
 @responses.activate
 def test_uc_customstrategy_safemulti():
     responses.add(responses.POST, URL + REGISTER_URL, json={}, status=202)
-    responses.add(responses.GET, URL + FEATURES_URL, json=MOCK_CUSTOM_STRATEGY, status=200)
+    responses.add(
+        responses.GET, URL + FEATURES_URL, json=MOCK_CUSTOM_STRATEGY, status=200
+    )
     responses.add(responses.POST, URL + METRICS_URL, json={}, status=202)
 
-    custom_strategies_dict = {
-        "amIACat": CatTest,
-        "amIADog": DogTest
-    }
+    custom_strategies_dict = {"amIACat": CatTest, "amIADog": DogTest}
 
     unleash_client = UnleashClient(
-        URL,
-        APP_NAME,
-        environment="prod",
-        custom_strategies=custom_strategies_dict)
+        URL, APP_NAME, environment="prod", custom_strategies=custom_strategies_dict
+    )
 
     unleash_client.initialize_client()
 
     # Check a toggle that contains an outdated custom strategy and a default strategy.
     assert unleash_client.is_enabled("CustomToggleWarningMultiStrat", {"sound": "meow"})
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/test_loader.py` & `UnleashClient-5.7.0/tests/unit_tests/test_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import copy
-from UnleashClient.loader import load_features
-from UnleashClient.features import Feature
-from UnleashClient.strategies import GradualRolloutUserId, FlexibleRollout, UserWithId
-from UnleashClient.variants import Variants
-from UnleashClient.constants import FEATURES_URL, FAILED_STRATEGIES
+
 from tests.utilities.mocks import MOCK_ALL_FEATURES
 from tests.utilities.testing_constants import DEFAULT_STRATEGY_MAPPING
+from UnleashClient.constants import FAILED_STRATEGIES, FEATURES_URL
+from UnleashClient.features import Feature
+from UnleashClient.loader import load_features
+from UnleashClient.strategies import FlexibleRollout, GradualRolloutUserId, UserWithId
+from UnleashClient.variants import Variants
 
 
 def test_loader_initialization(cache_full):  # noqa: F811
     # Set up variables
     in_memory_features = {}
     temp_cache = cache_full
 
     # Tests
     load_features(temp_cache, in_memory_features, DEFAULT_STRATEGY_MAPPING)
     assert isinstance(in_memory_features["GradualRolloutUserID"], Feature)
-    assert isinstance(in_memory_features["GradualRolloutUserID"].strategies[0], GradualRolloutUserId)
+    assert isinstance(
+        in_memory_features["GradualRolloutUserID"].strategies[0], GradualRolloutUserId
+    )
 
     for feature_name in in_memory_features.keys():
-        if feature_name == 'Garbage':  # Don't check purposely invalid strategy.
+        if feature_name == "Garbage":  # Don't check purposely invalid strategy.
             break
 
         feature = in_memory_features[feature_name]
         assert len(feature.strategies) > 0
         strategy = feature.strategies[0]
 
         if isinstance(strategy, UserWithId):
@@ -49,15 +52,20 @@
     # Simulate update mutation
     mock_updated = copy.deepcopy(MOCK_ALL_FEATURES)
     mock_updated["features"][4]["strategies"][0]["parameters"]["percentage"] = 60
     temp_cache.set(FEATURES_URL, mock_updated)
 
     load_features(temp_cache, in_memory_features, DEFAULT_STRATEGY_MAPPING)
 
-    assert in_memory_features["GradualRolloutUserID"].strategies[0].parameters["percentage"] == 60
+    assert (
+        in_memory_features["GradualRolloutUserID"]
+        .strategies[0]
+        .parameters["percentage"]
+        == 60
+    )
     assert len(temp_cache.get(FAILED_STRATEGIES)) == 1
 
 
 def test_loader_refresh_variants(cache_full):  # noqa: F811
     # Set up variables
     in_memory_features = {}
     temp_cache = cache_full
@@ -88,8 +96,8 @@
     # Set up variables
     in_memory_features = {}
     temp_cache = cache_segments
 
     load_features(temp_cache, in_memory_features, DEFAULT_STRATEGY_MAPPING)
     feature = in_memory_features["Test"]
     loaded_constraints = list(feature.strategies[0].parsed_constraints)
-    assert(len(loaded_constraints) == 2)
+    assert len(loaded_constraints) == 2
```

### Comparing `UnleashClient-5.6.0/tests/unit_tests/test_variants.py` & `UnleashClient-5.7.0/tests/unit_tests/test_variants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,94 @@
 import pytest
-from UnleashClient.variants import Variants
+
 from tests.utilities.mocks.mock_variants import VARIANTS, VARIANTS_WITH_STICKINESS
+from UnleashClient.variants import Variants
 
 
 @pytest.fixture()
 def variations():
     yield Variants(VARIANTS, "TestFeature")
 
 
 @pytest.fixture()
 def variations_with_stickiness():
     yield Variants(VARIANTS_WITH_STICKINESS, "TestFeature")
 
 
 def test_variations_override_match(variations):
-    override_variant = variations._apply_overrides({'userId': '1'})
-    assert override_variant['name'] == 'VarA'
+    override_variant = variations._apply_overrides({"userId": "1"})
+    assert override_variant["name"] == "VarA"
 
 
 def test_variations_overrid_nomatch(variations):
-    assert not variations._apply_overrides({'userId': '2'})
+    assert not variations._apply_overrides({"userId": "2"})
 
 
 def test_variations_seed(variations):
     # Random seed generation
     context = {}
     seed = variations._get_seed(context)
     assert float(seed) > 0
 
     # UserId, SessionId, and remoteAddress
-    context = {
-        'userId': '1',
-        'sessionId': '1',
-        'remoteAddress': '1.1.1.1'
-    }
+    context = {"userId": "1", "sessionId": "1", "remoteAddress": "1.1.1.1"}
 
-    assert context['userId'] == variations._get_seed(context)
-    del context['userId']
-    assert context['sessionId'] == variations._get_seed(context)
-    del context['sessionId']
-    assert context['remoteAddress'] == variations._get_seed(context)
+    assert context["userId"] == variations._get_seed(context)
+    del context["userId"]
+    assert context["sessionId"] == variations._get_seed(context)
+    del context["sessionId"]
+    assert context["remoteAddress"] == variations._get_seed(context)
 
 
 def test_variations_seed_override(variations):
     # UserId, SessionId, and remoteAddress
     context = {
-        'userId': '1',
-        'sessionId': '1',
-        'remoteAddress': '1.1.1.1',
-        'customField': "ActuallyAmAHamster"
+        "userId": "1",
+        "sessionId": "1",
+        "remoteAddress": "1.1.1.1",
+        "customField": "ActuallyAmAHamster",
     }
 
-    assert context['customField'] == variations._get_seed(context, 'customField')
+    assert context["customField"] == variations._get_seed(context, "customField")
 
 
 def test_variation_selectvariation_happypath(variations):
-    variant = variations.get_variant({'userId': '2'})
+    variant = variations.get_variant({"userId": "2"})
     assert variant
-    assert 'payload' in variant
-    assert variant['name'] == 'VarC'
+    assert "payload" in variant
+    assert variant["name"] == "VarC"
 
 
 def test_variation_customvariation(variations_with_stickiness):
     variations = variations_with_stickiness
-    variant = variations.get_variant({'customField': 'ActuallyAmAHamster1234'})
+    variant = variations.get_variant({"customField": "ActuallyAmAHamster1234"})
     assert variant
-    assert 'payload' in variant
-    assert variant['name'] == 'VarC'
+    assert "payload" in variant
+    assert variant["name"] == "VarC"
 
 
 def test_variation_selectvariation_multi(variations):
     tracker = {}
     for x in range(100):
         variant = variations.get_variant({})
-        name = variant['name']
+        name = variant["name"]
         if name in tracker:
             tracker[name] += 1
         else:
             tracker[name] = 1
 
     assert len(tracker) == 3
     assert sum([tracker[x] for x in tracker.keys()]) == 100
 
 
 def test_variation_override(variations):
-    variant = variations.get_variant({'userId': '1'})
+    variant = variations.get_variant({"userId": "1"})
     assert variant
-    assert 'payload' in variant
-    assert variant['name'] == 'VarA'
+    assert "payload" in variant
+    assert variant["name"] == "VarA"
 
 
 def test_variation_novariants():
     variations = Variants([], "TestFeature")
     variant = variations.get_variant({})
     assert variant
-    assert variant['name'] == 'disabled'
+    assert variant["name"] == "disabled"
```

### Comparing `UnleashClient-5.6.0/tests/utilities/mocks/mock_all_features.py` & `UnleashClient-5.7.0/tests/utilities/mocks/mock_all_features.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,220 +4,171 @@
         {
             "name": "ApplicationHostname",
             "description": "Application Hostname strategy",
             "enabled": True,
             "strategies": [
                 {
                     "name": "applicationHostname",
-                    "parameters": {
-                        "hostNames": "iMacPro.local,test1,test2"
-                    }
+                    "parameters": {"hostNames": "iMacPro.local,test1,test2"},
                 }
             ],
             "createdAt": "2018-10-09T06:05:14.757Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "Default",
             "description": "Default feature toggle",
             "enabled": True,
-            "strategies": [
-                {
-                    "name": "default",
-                    "parameters": {}
-                }
-            ],
+            "strategies": [{"name": "default", "parameters": {}}],
             "createdAt": "2018-10-09T06:04:05.667Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "GradualRolloutRandom",
             "description": "Gradual Rollout Random example",
             "enabled": True,
             "strategies": [
-                {
-                    "name": "gradualRolloutRandom",
-                    "parameters": {
-                        "percentage": 50
-                    }
-                }
+                {"name": "gradualRolloutRandom", "parameters": {"percentage": 50}}
             ],
             "createdAt": "2018-10-09T06:05:37.637Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "GradualRolloutSessionId",
             "description": "SessionID check!",
             "enabled": True,
             "strategies": [
                 {
                     "name": "gradualRolloutSessionId",
                     "parameters": {
                         "percentage": 50,
-                        "groupId": "GradualRolloutSessionId"
-                    }
+                        "groupId": "GradualRolloutSessionId",
+                    },
                 }
             ],
             "createdAt": "2018-10-09T06:06:51.057Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "GradualRolloutUserID",
             "description": "GradualRolloutUserID strategy",
             "enabled": True,
             "strategies": [
                 {
                     "name": "gradualRolloutUserId",
-                    "parameters": {
-                        "percentage": 50,
-                        "groupId": "GradualRolloutUserID"
-                    }
+                    "parameters": {"percentage": 50, "groupId": "GradualRolloutUserID"},
                 }
             ],
             "createdAt": "2018-10-09T06:07:17.520Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "RemoteAddress",
             "description": "RemoteAddress strategies",
             "enabled": True,
             "strategies": [
                 {
                     "name": "remoteAddress",
                     "parameters": {
                         "IPs": "69.208.0.0/29,70.208.1.1,2001:db8:1234::/48,2002:db8:1234:0000:0000:0000:0000:0001"
-                    }
+                    },
                 }
             ],
             "createdAt": "2018-10-09T06:08:42.398Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "UserWithId",
             "description": "UserWithId strategies",
             "enabled": True,
             "strategies": [
                 {
                     "name": "userWithId",
                     "parameters": {
                         "userIds": "meep@meep.com,test@test.com,wat@wat.com"
-                    }
+                    },
                 }
             ],
             "createdAt": "2018-10-09T06:09:19.203Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "FlexibleRollout",
             "description": "FlexibleRollout strategies",
             "enabled": True,
             "strategies": [
                 {
                     "name": "flexibleRollout",
                     "parameters": {
                         "rollout": "21",
                         "stickiness": "userId",
-                        "groupId": "ivantest"
+                        "groupId": "ivantest",
                     },
                     "constraints": [
                         {
                             "contextName": "environment",
                             "operator": "IN",
-                            "values": [
-                                "staging",
-                                "prod"
-                            ]
+                            "values": ["staging", "prod"],
                         },
                         {
                             "contextName": "userId",
                             "operator": "NOT_IN",
-                            "values": [
-                                "1",
-                                "2",
-                                "3"
-                            ]
+                            "values": ["1", "2", "3"],
                         },
                         {
                             "contextName": "userId",
                             "operator": "IN",
-                            "values": [
-                                "4",
-                                "5",
-                                "6"
-                            ]
+                            "values": ["4", "5", "6"],
                         },
                         {
                             "contextName": "appName",
                             "operator": "IN",
-                            "values": [
-                                "test"
-                            ]
-                        }
-                    ]
+                            "values": ["test"],
+                        },
+                    ],
                 }
             ],
             "variants": None,
             "createdAt": "2019-10-05T07:30:29.896Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "Variations",
             "description": "Test variation",
             "enabled": True,
-            "strategies": [
-                {
-                    "name": "default"
-                }
-            ],
+            "strategies": [{"name": "default"}],
             "variants": [
                 {
                     "name": "VarA",
                     "weight": 34,
-                    "payload": {
-                        "type": "string",
-                        "value": "Test1"
-                    },
+                    "payload": {"type": "string", "value": "Test1"},
                     "overrides": [
                         {
                             "contextName": "userId",
-                            "values": [
-                                "ivanklee86@gmail.com",
-                                "ivan@aaptiv.com"
-                            ]
+                            "values": ["ivanklee86@gmail.com", "ivan@aaptiv.com"],
                         }
-                    ]
+                    ],
                 },
                 {
                     "name": "VarB",
                     "weight": 33,
-                    "payload": {
-                        "type": "string",
-                        "value": "Test 2"
-                    }
+                    "payload": {"type": "string", "value": "Test 2"},
                 },
                 {
                     "name": "VarC",
                     "weight": 33,
-                    "payload": {
-                        "type": "string",
-                        "value": "Test 3"
-                    }
-                }
+                    "payload": {"type": "string", "value": "Test 3"},
+                },
             ],
             "createdAt": "2019-10-25T13:22:02.035Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "Garbage",
             "description": "Invalid strategy",
             "enabled": True,
-            "strategies": [
-                {
-                    "name": "blargwatisdis",
-                    "parameters": {}
-                }
-            ],
+            "strategies": [{"name": "blargwatisdis", "parameters": {}}],
             "createdAt": "2018-10-09T06:04:05.667Z",
-            "impressionData": False
+            "impressionData": False,
         },
-    ]
+    ],
 }
```

### Comparing `UnleashClient-5.6.0/tests/utilities/mocks/mock_constraints.py` & `UnleashClient-5.7.0/tests/utilities/mocks/mock_constraints.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,209 +1,178 @@
-CONSTRAINT_DICT_IN = \
-    {
-        "contextName": "appName",
-        "operator": "IN",
-        "values": [
-            "test",
-            "test2"
-        ]
-    }
-
-
-CONSTRAINT_DICT_NOTIN = \
-    {
-        "contextName": "appName",
-        "operator": "NOT_IN",
-        "values": [
-            "test",
-            "test2"
-        ]
-    }
-
-
-CONSTRAINT_DICT_NOTIN_INVERT = \
-    {
-        "contextName": "appName",
-        "operator": "NOT_IN",
-        "values": [
-            "test",
-            "test2"
-        ],
-        "inverted": True
-    }
-
-
-CONSTRAINT_DICT_STR_INVERT = \
-    {
-        "contextName": "customField",
-        "operator": "STR_CONTAINS",
-        "values": ["dog", "cat", "hAmStEr"],
-        "caseInsensitive": True,
-        "inverted": True
-    }
-
-
-CONSTRAINT_DICT_STR_CONTAINS_CI = \
-    {
-        "contextName": "customField",
-        "operator": "STR_CONTAINS",
-        "values": ["dog", "cat", "hAmStEr"],
-        "caseInsensitive": True,
-        "inverted": False
-    }
-
-
-CONSTRAINT_DICT_STR_CONTAINS_NOT_CI = \
-    {
-        "contextName": "customField",
-        "operator": "STR_CONTAINS",
-        "values": ["dog", "cat", "hAmStEr"],
-        "caseInsensitive": False,
-        "inverted": False
-    }
-
-
-CONSTRAINT_DICT_STR_ENDS_WITH_CI = \
-    {
-        "contextName": "customField",
-        "operator": "STR_ENDS_WITH",
-        "values": ["dog", "cat", "hAmStEr"],
-        "caseInsensitive": True,
-        "inverted": False
-    }
-
-CONSTRAINT_DICT_STR_ENDS_WITH_NOT_CI = \
-    {
-        "contextName": "customField",
-        "operator": "STR_ENDS_WITH",
-        "values": ["dog", "cat", "hAmStEr"],
-        "caseInsensitive": False,
-        "inverted": False
-    }
-
-
-CONSTRAINT_DICT_STR_STARTS_WITH_CI = \
-    {
-        "contextName": "customField",
-        "operator": "STR_STARTS_WITH",
-        "values": ["dog", "cat", "hAmStEr"],
-        "caseInsensitive": True,
-        "inverted": False
-    }
-
-
-CONSTRAINT_DICT_STR_STARTS_WITH_NOT_CI = \
-    {
-        "contextName": "customField",
-        "operator": "STR_STARTS_WITH",
-        "values": ["dog", "cat", "hAmStEr"],
-        "caseInsensitive": False,
-        "inverted": False
-    }
-
-
-CONSTRAINT_NUM_EQ = \
-    {
-        "contextName": "customField",
-        "operator": "NUM_EQ",
-        "value": "5",
-        "inverted": False
-    }
-
-
-CONSTRAINT_NUM_GT = \
-    {
-        "contextName": "customField",
-        "operator": "NUM_GT",
-        "value": "5",
-        "inverted": False
-    }
-
-
-CONSTRAINT_NUM_GTE = \
-    {
-        "contextName": "customField",
-        "operator": "NUM_GTE",
-        "value": 5,
-        "inverted": False
-    }
-
-
-CONSTRAINT_NUM_LT = \
-    {
-        "contextName": "customField",
-        "operator": "NUM_LT",
-        "value": "5",
-        "inverted": False
-    }
-
-
-CONSTRAINT_NUM_LTE = \
-    {
-        "contextName": "customField",
-        "operator": "NUM_LTE",
-        "value": "5",
-        "inverted": False
-    }
-
-
-CONSTRAINT_NUM_FLOAT = \
-    {
-        "contextName": "customField",
-        "operator": "NUM_LTE",
-        "value": "5.1",
-        "inverted": False
-    }
-
-
-CONSTRAINT_DATE_AFTER = \
-    {
-        "contextName": "currentTime",
-        "operator": "DATE_AFTER",
-        "value": "2022-01-22T00:00:00.000Z",
-        "inverted": False
-    }
-
-
-CONSTRAINT_DATE_BEFORE = \
-    {
-        "contextName": "currentTime",
-        "operator": "DATE_BEFORE",
-        "value": "2022-01-22T00:00:00.000Z",
-        "inverted": False
-    }
-
-
-CONSTRAINT_DATE_ERROR = \
-    {
-        "contextName": "currentTime",
-        "operator": "DATE_AFTER",
-        "value": "abcd",
-        "inverted": False
-    }
-
-
-CONSTRAINT_SEMVER_EQ = \
-    {
-        "contextName": "customField",
-        "operator": "SEMVER_EQ",
-        "value": "1.2.2",
-        "inverted": False
-    }
-
-
-CONSTRAINT_SEMVER_GT = \
-    {
-        "contextName": "customField",
-        "operator": "SEMVER_GT",
-        "value": "1.2.2",
-        "inverted": False
-    }
-
-
-CONSTRAINT_SEMVER_LT = \
-    {
-        "contextName": "customField",
-        "operator": "SEMVER_LT",
-        "value": "1.2.2",
-        "inverted": False
-    }
+CONSTRAINT_DICT_IN = {
+    "contextName": "appName",
+    "operator": "IN",
+    "values": ["test", "test2"],
+}
+
+
+CONSTRAINT_DICT_NOTIN = {
+    "contextName": "appName",
+    "operator": "NOT_IN",
+    "values": ["test", "test2"],
+}
+
+
+CONSTRAINT_DICT_NOTIN_INVERT = {
+    "contextName": "appName",
+    "operator": "NOT_IN",
+    "values": ["test", "test2"],
+    "inverted": True,
+}
+
+
+CONSTRAINT_DICT_STR_INVERT = {
+    "contextName": "customField",
+    "operator": "STR_CONTAINS",
+    "values": ["dog", "cat", "hAmStEr"],
+    "caseInsensitive": True,
+    "inverted": True,
+}
+
+
+CONSTRAINT_DICT_STR_CONTAINS_CI = {
+    "contextName": "customField",
+    "operator": "STR_CONTAINS",
+    "values": ["dog", "cat", "hAmStEr"],
+    "caseInsensitive": True,
+    "inverted": False,
+}
+
+
+CONSTRAINT_DICT_STR_CONTAINS_NOT_CI = {
+    "contextName": "customField",
+    "operator": "STR_CONTAINS",
+    "values": ["dog", "cat", "hAmStEr"],
+    "caseInsensitive": False,
+    "inverted": False,
+}
+
+
+CONSTRAINT_DICT_STR_ENDS_WITH_CI = {
+    "contextName": "customField",
+    "operator": "STR_ENDS_WITH",
+    "values": ["dog", "cat", "hAmStEr"],
+    "caseInsensitive": True,
+    "inverted": False,
+}
+
+CONSTRAINT_DICT_STR_ENDS_WITH_NOT_CI = {
+    "contextName": "customField",
+    "operator": "STR_ENDS_WITH",
+    "values": ["dog", "cat", "hAmStEr"],
+    "caseInsensitive": False,
+    "inverted": False,
+}
+
+
+CONSTRAINT_DICT_STR_STARTS_WITH_CI = {
+    "contextName": "customField",
+    "operator": "STR_STARTS_WITH",
+    "values": ["dog", "cat", "hAmStEr"],
+    "caseInsensitive": True,
+    "inverted": False,
+}
+
+
+CONSTRAINT_DICT_STR_STARTS_WITH_NOT_CI = {
+    "contextName": "customField",
+    "operator": "STR_STARTS_WITH",
+    "values": ["dog", "cat", "hAmStEr"],
+    "caseInsensitive": False,
+    "inverted": False,
+}
+
+
+CONSTRAINT_NUM_EQ = {
+    "contextName": "customField",
+    "operator": "NUM_EQ",
+    "value": "5",
+    "inverted": False,
+}
+
+
+CONSTRAINT_NUM_GT = {
+    "contextName": "customField",
+    "operator": "NUM_GT",
+    "value": "5",
+    "inverted": False,
+}
+
+
+CONSTRAINT_NUM_GTE = {
+    "contextName": "customField",
+    "operator": "NUM_GTE",
+    "value": 5,
+    "inverted": False,
+}
+
+
+CONSTRAINT_NUM_LT = {
+    "contextName": "customField",
+    "operator": "NUM_LT",
+    "value": "5",
+    "inverted": False,
+}
+
+
+CONSTRAINT_NUM_LTE = {
+    "contextName": "customField",
+    "operator": "NUM_LTE",
+    "value": "5",
+    "inverted": False,
+}
+
+
+CONSTRAINT_NUM_FLOAT = {
+    "contextName": "customField",
+    "operator": "NUM_LTE",
+    "value": "5.1",
+    "inverted": False,
+}
+
+
+CONSTRAINT_DATE_AFTER = {
+    "contextName": "currentTime",
+    "operator": "DATE_AFTER",
+    "value": "2022-01-22T00:00:00.000Z",
+    "inverted": False,
+}
+
+
+CONSTRAINT_DATE_BEFORE = {
+    "contextName": "currentTime",
+    "operator": "DATE_BEFORE",
+    "value": "2022-01-22T00:00:00.000Z",
+    "inverted": False,
+}
+
+
+CONSTRAINT_DATE_ERROR = {
+    "contextName": "currentTime",
+    "operator": "DATE_AFTER",
+    "value": "abcd",
+    "inverted": False,
+}
+
+
+CONSTRAINT_SEMVER_EQ = {
+    "contextName": "customField",
+    "operator": "SEMVER_EQ",
+    "value": "1.2.2",
+    "inverted": False,
+}
+
+
+CONSTRAINT_SEMVER_GT = {
+    "contextName": "customField",
+    "operator": "SEMVER_GT",
+    "value": "1.2.2",
+    "inverted": False,
+}
+
+
+CONSTRAINT_SEMVER_LT = {
+    "contextName": "customField",
+    "operator": "SEMVER_LT",
+    "value": "1.2.2",
+    "inverted": False,
+}
```

### Comparing `UnleashClient-5.6.0/tests/utilities/mocks/mock_features.py` & `UnleashClient-5.7.0/tests/utilities/mocks/mock_features.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,208 +1,160 @@
 MOCK_FEATURE_RESPONSE = {
     "version": 1,
     "features": [
         {
             "name": "testFlag",
             "description": "This is a test!",
             "enabled": True,
-            "strategies": [
-                {
-                    "name": "default",
-                    "parameters": {}
-                }
-            ],
+            "strategies": [{"name": "default", "parameters": {}}],
             "createdAt": "2018-10-04T01:27:28.477Z",
-            "impressionData": True
+            "impressionData": True,
         },
         {
             "name": "testFlag2",
             "description": "Test flag 2",
             "enabled": True,
             "strategies": [
-                {
-                    "name": "gradualRolloutRandom",
-                    "parameters": {
-                        "percentage": 50
-                    }
-                }
+                {"name": "gradualRolloutRandom", "parameters": {"percentage": 50}}
             ],
             "createdAt": "2018-10-04T11:03:56.062Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "testContextFlag",
             "description": "This is a test for static context fileds!",
             "enabled": True,
             "strategies": [
-                {
-                    "name": "custom-context",
-                    "parameters": {
-                        "environments": "prod"
-                    }
-                }
+                {"name": "custom-context", "parameters": {"environments": "prod"}}
             ],
             "createdAt": "2018-10-04T01:27:28.477Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "testConstraintFlag",
             "description": "This is a flag with a constraint!",
             "enabled": True,
             "strategies": [
                 {
                     "name": "default",
                     "parameters": {},
                     "constraints": [
                         {
                             "contextName": "currentTime",
                             "operator": "DATE_BEFORE",
                             "value": "2022-01-22T00:00:00.000Z",
-                            "inverted": False
+                            "inverted": False,
                         }
                     ],
                 },
             ],
             "createdAt": "2018-10-04T01:27:28.477Z",
-            "impressionData": False
+            "impressionData": False,
         },
         {
             "name": "testVariations",
             "description": "Test variation",
             "enabled": True,
-            "strategies": [
-                {
-                    "name": "userWithId",
-                    "parameters": {
-                        "userIds": "2"
-                    }
-                }
-            ],
+            "strategies": [{"name": "userWithId", "parameters": {"userIds": "2"}}],
             "variants": [
                 {
                     "name": "VarA",
                     "weight": 34,
-                    "payload": {
-                        "type": "string",
-                        "value": "Test1"
-                    },
+                    "payload": {"type": "string", "value": "Test1"},
                     "overrides": [
                         {
                             "contextName": "userId",
-                            "values": [
-                                "ivanklee86@gmail.com",
-                                "ivan@aaptiv.com"
-                            ]
+                            "values": ["ivanklee86@gmail.com", "ivan@aaptiv.com"],
                         }
-                    ]
+                    ],
                 },
                 {
                     "name": "VarB",
                     "weight": 33,
-                    "payload": {
-                        "type": "string",
-                        "value": "Test 2"
-                    }
+                    "payload": {"type": "string", "value": "Test 2"},
                 },
                 {
                     "name": "VarC",
                     "weight": 33,
-                    "payload": {
-                        "type": "string",
-                        "value": "Test 3"
-                    }
-                }
+                    "payload": {"type": "string", "value": "Test 3"},
+                },
             ],
             "createdAt": "2019-10-25T13:22:02.035Z",
-            "impressionData": True
-        }
-    ]
+            "impressionData": True,
+        },
+    ],
 }
 
 MOCK_FEATURES_WITH_SEGMENTS_RESPONSE = {
     "version": 2,
     "features": [
         {
             "strategies": [
                 {
                     "name": "default",
                     "constraints": [],
                     "parameters": {},
-                    "segments": [
-                        1, 2
-                    ]
+                    "segments": [1, 2],
                 }
             ],
             "impressionData": False,
             "enabled": True,
             "name": "Test",
             "description": "",
             "project": "default",
             "type": "release",
-            "variants": []
+            "variants": [],
         }
     ],
-    "query": {
-        "environment": "development",
-        "inlineSegmentConstraints": False
-    },
+    "query": {"environment": "development", "inlineSegmentConstraints": False},
     "segments": [
         {
             "id": 1,
             "name": "TestSegment1",
             "description": "test",
             "constraints": [
                 {
                     "value": "2022-06-14T06:40:17.766Z",
                     "values": [],
                     "inverted": False,
                     "operator": "DATE_BEFORE",
                     "contextName": "currentTime",
-                    "caseInsensitive": False
+                    "caseInsensitive": False,
                 }
             ],
             "createdBy": "admin",
-            "createdAt": "2022-06-14T06:40:25.331Z"
+            "createdAt": "2022-06-14T06:40:25.331Z",
         },
         {
             "id": 2,
             "name": "TestSegment2",
             "description": "test",
             "constraints": [
                 {
                     "value": "2022-06-14T06:40:17.766Z",
                     "values": [],
                     "inverted": False,
                     "operator": "DATE_AFTER",
                     "contextName": "currentTime",
-                    "caseInsensitive": False
+                    "caseInsensitive": False,
                 }
             ],
             "createdBy": "admin",
-            "createdAt": "2022-06-14T06:40:25.331Z"
-        }
-    ]
+            "createdAt": "2022-06-14T06:40:25.331Z",
+        },
+    ],
 }
 
 MOCK_FEATURE_RESPONSE_PROJECT = {
     "version": 1,
     "features": [
         {
             "name": "ivan-project",
             "type": "release",
             "enabled": True,
-            "strategies": [
-                {
-                    "name": "default",
-                    "parameters": {
-
-                    }
-                }
-            ],
-            "variants": [
-
-            ],
+            "strategies": [{"name": "default", "parameters": {}}],
+            "variants": [],
             "createdAt": "2023-01-24T06:40:25.331Z",
-            "impressionData": False
+            "impressionData": False,
         }
-    ]
+    ],
 }
```

### Comparing `UnleashClient-5.6.0/tests/utilities/old_code/StrategyV2.py` & `UnleashClient-5.7.0/tests/utilities/old_code/StrategyV2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Old Strategy object from unleash-client-python version 1.x.x and 2.x.x
 
+
 # pylint: disable=dangerous-default-value
-class StrategyOldV2():
+class StrategyOldV2:
     """
     In general, default & custom classes should only need to override:
     * __call__() - Implementation of the strategy.
     * load_provisioning - Loads strategy provisioning
     """
-    def __init__(self,
-                 parameters: dict = {}) -> None:
+
+    def __init__(self, parameters: dict = {}) -> None:
         """
         A generic strategy objects.
         :param parameters: 'parameters' key from strategy section (...from feature section) of
         /api/clients/features response
         """
         # Experiment information
         self.parameters = parameters
```

### Comparing `UnleashClient-5.6.0/tests/utilities/testing_constants.py` & `UnleashClient-5.7.0/tests/utilities/testing_constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,18 @@
-from UnleashClient.strategies import ApplicationHostname, Default, GradualRolloutRandom, \
-    GradualRolloutSessionId, GradualRolloutUserId, UserWithId, RemoteAddress, FlexibleRollout
 from UnleashClient.constants import FEATURES_URL
+from UnleashClient.strategies import (
+    ApplicationHostname,
+    Default,
+    FlexibleRollout,
+    GradualRolloutRandom,
+    GradualRolloutSessionId,
+    GradualRolloutUserId,
+    RemoteAddress,
+    UserWithId,
+)
 
 # General configs
 APP_NAME = "pytest"
 ENVIRONMENT = "unit"
 INSTANCE_ID = "123"
 REFRESH_INTERVAL = 15
 REFRESH_JITTER = None
@@ -17,22 +25,24 @@
 
 # URLs
 URL = "http://localhost:4242/api"
 INTEGRATION_URL = "http://localhost:4242/api"
 PROJECT_URL = f"{URL}{FEATURES_URL}?project=ivan"
 
 # Constants
-IP_LIST = "69.208.0.0/29,70.208.1.1,2001:db8:1234::/48,2002:db8:1234:0000:0000:0000:0000:0001"
-PROJECT_NAME = 'ivan'
+IP_LIST = (
+    "69.208.0.0/29,70.208.1.1,2001:db8:1234::/48,2002:db8:1234:0000:0000:0000:0000:0001"
+)
+PROJECT_NAME = "ivan"
 ETAG_VALUE = 'W/"730-v0ozrE11zfZK13j7rQ5PxkXfjYQ"'
 
 # Mapping
 DEFAULT_STRATEGY_MAPPING = {
     "applicationHostname": ApplicationHostname,
     "default": Default,
     "gradualRolloutRandom": GradualRolloutRandom,
     "gradualRolloutSessionId": GradualRolloutSessionId,
     "gradualRolloutUserId": GradualRolloutUserId,
     "remoteAddress": RemoteAddress,
     "userWithId": UserWithId,
-    "flexibleRollout": FlexibleRollout
+    "flexibleRollout": FlexibleRollout,
 }
```

