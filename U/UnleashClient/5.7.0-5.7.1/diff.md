# Comparing `tmp/UnleashClient-5.7.0.tar.gz` & `tmp/UnleashClient-5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/unleash-client-python/unleash-client-python/dist/.tmp-vk9kzf1p/UnleashClient-5.7.0.tar", last modified: Fri Jun 30 11:56:36 2023, max compression
+gzip compressed data, was "/home/runner/work/unleash-client-python/unleash-client-python/dist/.tmp-oxpjksgk/UnleashClient-5.7.1.tar", last modified: Fri Jun 30 16:11:07 2023, max compression
```

## Comparing `UnleashClient-5.7.0.tar` & `UnleashClient-5.7.1.tar`

### file list

```diff
@@ -1,149 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.devcontainer/post_install.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/add-to-project.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/release-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.lift.toml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/api/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/api/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/api/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/deprecation_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/features/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/features/Feature.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/periodic_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/periodic_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/periodic_tasks/fetch_and_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/periodic_tasks/send_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/ApplicationHostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/Default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/FlexibleRolloutStrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutRandom.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutSessionId.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutUserId.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/RemoteAddress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/Strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/UserWithId.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient/variants/
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/variants/Variants.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/UnleashClient/variants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/UnleashClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/basecache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/customcache.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/customstrategies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/eventcallbacks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/filecache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/strategy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/unleashclient.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/docs/wsgi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/scripts/get-spec.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/integration_tests/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/integration_tests/integration_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/integration_tests/integration_unleashheroku.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/integration_tests/integration_unleashhosted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/specification_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/specification_tests/test_client_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/unit_tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/api/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/api/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/api/test_register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/unit_tests/periodic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/periodic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/periodic/test_fetch_and_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_applicationhostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_defaultstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_flexiblerollout.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_gradualrolloutrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_gradualrolloutwithsessionid.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_gradualrolloutwithuserid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_remoteaddress.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/strategies/test_userwithids.py
--rw-r--r--   0 runner    (1001) docker     (123)    23845 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_custom_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/unit_tests/test_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/utilities/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_all_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_bootstrap.json
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_custom_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/mocks/mock_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:56:36.000000 UnleashClient-5.7.0/tests/utilities/old_code/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/old_code/StrategyV2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/old_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tests/utilities/testing_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 11:55:40.000000 UnleashClient-5.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.devcontainer/post_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/add-to-project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/release-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.lift.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/api/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/deprecation_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/features/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/periodic_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/periodic_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/periodic_tasks/fetch_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/periodic_tasks/send_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/ApplicationHostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/Default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/FlexibleRolloutStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutRandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutSessionId.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutUserId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/RemoteAddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/Strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/UserWithId.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient/variants/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/variants/Variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/UnleashClient/variants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/UnleashClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/basecache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/customcache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/customstrategies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/eventcallbacks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/filecache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/strategy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/unleashclient.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/docs/wsgi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/scripts/get-spec.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/integration_tests/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/integration_tests/integration_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/integration_tests/integration_unleashheroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/integration_tests/integration_unleashhosted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/specification_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/specification_tests/test_client_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/unit_tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/api/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/api/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/api/test_register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/unit_tests/periodic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/periodic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/periodic/test_fetch_and_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_applicationhostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_defaultstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_flexiblerollout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_gradualrolloutrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_gradualrolloutwithsessionid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_gradualrolloutwithuserid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_remoteaddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/strategies/test_userwithids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23845 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_custom_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/unit_tests/test_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/utilities/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_all_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_bootstrap.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_custom_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/mocks/mock_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:07.000000 UnleashClient-5.7.1/tests/utilities/old_code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/old_code/StrategyV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/old_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tests/utilities/testing_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 16:10:12.000000 UnleashClient-5.7.1/tox.ini
```

### Comparing `UnleashClient-5.7.0/.devcontainer/Dockerfile` & `UnleashClient-5.7.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/.devcontainer/devcontainer.json` & `UnleashClient-5.7.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `UnleashClient-5.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/.github/PULL_REQUEST_TEMPLATE.md` & `UnleashClient-5.7.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/.github/workflows/codeql-analysis.yml` & `UnleashClient-5.7.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/.github/workflows/pull_request.yml` & `UnleashClient-5.7.1/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/.github/workflows/release-docs.yml` & `UnleashClient-5.7.1/.github/workflows/release-docs.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/.github/workflows/release-package.yml` & `UnleashClient-5.7.1/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/.gitignore` & `UnleashClient-5.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/CHANGELOG.md` & `UnleashClient-5.7.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/CODE_OF_CONDUCT.md` & `UnleashClient-5.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/CONTRIBUTING.md` & `UnleashClient-5.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/LICENSE.md` & `UnleashClient-5.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/Makefile` & `UnleashClient-5.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/PKG-INFO` & `UnleashClient-5.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnleashClient
-Version: 5.7.0
+Version: 5.7.1
 Summary: Python client for the Unleash feature toggle system!
 Author-email: Ivan Lee <ivanklee86@gmail.com>
 Project-URL: Homepage, https://github.com/Unleash/unleash-client-python
 Project-URL: Documentation, https://docs.getunleash.io/unleash-client-python
 Project-URL: Changelog, https://github.com/Unleash/unleash-client-python/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/Unleash/unleash-client-python
 Project-URL: Issues, https://github.com/Unleash/unleash-client-python/issues
```

### Comparing `UnleashClient-5.7.0/README.md` & `UnleashClient-5.7.1/README.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/__init__.py` & `UnleashClient-5.7.1/UnleashClient/__init__.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/api/features.py` & `UnleashClient-5.7.1/UnleashClient/api/features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/api/metrics.py` & `UnleashClient-5.7.1/UnleashClient/api/metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/api/register.py` & `UnleashClient-5.7.1/UnleashClient/api/register.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/cache.py` & `UnleashClient-5.7.1/UnleashClient/cache.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/constants.py` & `UnleashClient-5.7.1/UnleashClient/constants.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/constraints/Constraint.py` & `UnleashClient-5.7.1/UnleashClient/constraints/Constraint.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/deprecation_warnings.py` & `UnleashClient-5.7.1/UnleashClient/deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/events.py` & `UnleashClient-5.7.1/UnleashClient/events.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/features/Feature.py` & `UnleashClient-5.7.1/UnleashClient/features/Feature.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/loader.py` & `UnleashClient-5.7.1/UnleashClient/loader.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/periodic_tasks/fetch_and_load.py` & `UnleashClient-5.7.1/UnleashClient/periodic_tasks/fetch_and_load.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/periodic_tasks/send_metrics.py` & `UnleashClient-5.7.1/UnleashClient/periodic_tasks/send_metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/strategies/FlexibleRolloutStrategy.py` & `UnleashClient-5.7.1/UnleashClient/strategies/FlexibleRolloutStrategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutSessionId.py` & `UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutSessionId.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/strategies/GradualRolloutUserId.py` & `UnleashClient-5.7.1/UnleashClient/strategies/GradualRolloutUserId.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/strategies/RemoteAddress.py` & `UnleashClient-5.7.1/UnleashClient/strategies/RemoteAddress.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/strategies/Strategy.py` & `UnleashClient-5.7.1/UnleashClient/strategies/Strategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/strategies/UserWithId.py` & `UnleashClient-5.7.1/UnleashClient/strategies/UserWithId.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/utils.py` & `UnleashClient-5.7.1/UnleashClient/utils.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient/variants/Variants.py` & `UnleashClient-5.7.1/UnleashClient/variants/Variants.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/UnleashClient.egg-info/PKG-INFO` & `UnleashClient-5.7.1/UnleashClient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnleashClient
-Version: 5.7.0
+Version: 5.7.1
 Summary: Python client for the Unleash feature toggle system!
 Author-email: Ivan Lee <ivanklee86@gmail.com>
 Project-URL: Homepage, https://github.com/Unleash/unleash-client-python
 Project-URL: Documentation, https://docs.getunleash.io/unleash-client-python
 Project-URL: Changelog, https://github.com/Unleash/unleash-client-python/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/Unleash/unleash-client-python
 Project-URL: Issues, https://github.com/Unleash/unleash-client-python/issues
```

### Comparing `UnleashClient-5.7.0/UnleashClient.egg-info/SOURCES.txt` & `UnleashClient-5.7.1/UnleashClient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 UnleashClient/events.py
 UnleashClient/loader.py
 UnleashClient/py.typed
 UnleashClient/utils.py
 UnleashClient.egg-info/PKG-INFO
 UnleashClient.egg-info/SOURCES.txt
 UnleashClient.egg-info/dependency_links.txt
+UnleashClient.egg-info/requires.txt
 UnleashClient.egg-info/top_level.txt
 UnleashClient/api/__init__.py
 UnleashClient/api/features.py
 UnleashClient/api/metrics.py
 UnleashClient/api/register.py
 UnleashClient/constraints/Constraint.py
 UnleashClient/constraints/__init__.py
```

### Comparing `UnleashClient-5.7.0/docs/Makefile` & `UnleashClient-5.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/celery.rst` & `UnleashClient-5.7.1/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/conf.py` & `UnleashClient-5.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/customcache.rst` & `UnleashClient-5.7.1/docs/customcache.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/customstrategies.rst` & `UnleashClient-5.7.1/docs/customstrategies.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/development.rst` & `UnleashClient-5.7.1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/eventcallbacks.rst` & `UnleashClient-5.7.1/docs/eventcallbacks.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/index.rst` & `UnleashClient-5.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/make.bat` & `UnleashClient-5.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/usage.rst` & `UnleashClient-5.7.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/docs/wsgi.rst` & `UnleashClient-5.7.1/docs/wsgi.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/pyproject.toml` & `UnleashClient-5.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,24 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 
+dependencies=[
+    "requests",
+    "fcache",
+    "mmhash3",
+    "apscheduler < 4.0.0",
+    "importlib_metadata",
+    "python-dateutil",
+    "semver < 3.0.0"
+]
+
 [project.urls]
 Homepage = "https://github.com/Unleash/unleash-client-python"
 Documentation = "https://docs.getunleash.io/unleash-client-python"
 Changelog = "https://github.com/Unleash/unleash-client-python/blob/main/CHANGELOG.md"
 Repository = "https://github.com/Unleash/unleash-client-python"
 Issues = "https://github.com/Unleash/unleash-client-python/issues"
```

### Comparing `UnleashClient-5.7.0/tests/conftest.py` & `UnleashClient-5.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/integration_tests/integration.py` & `UnleashClient-5.7.1/tests/integration_tests/integration.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/integration_tests/integration_gitlab.py` & `UnleashClient-5.7.1/tests/integration_tests/integration_gitlab.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/integration_tests/integration_unleashheroku.py` & `UnleashClient-5.7.1/tests/integration_tests/integration_unleashheroku.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/integration_tests/integration_unleashhosted.py` & `UnleashClient-5.7.1/tests/integration_tests/integration_unleashhosted.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/specification_tests/test_client_specs.py` & `UnleashClient-5.7.1/tests/specification_tests/test_client_specs.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/api/test_feature.py` & `UnleashClient-5.7.1/tests/unit_tests/api/test_feature.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/api/test_metrics.py` & `UnleashClient-5.7.1/tests/unit_tests/api/test_metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/api/test_register.py` & `UnleashClient-5.7.1/tests/unit_tests/api/test_register.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py` & `UnleashClient-5.7.1/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/periodic/test_fetch_and_load.py` & `UnleashClient-5.7.1/tests/unit_tests/periodic/test_fetch_and_load.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/strategies/test_flexiblerollout.py` & `UnleashClient-5.7.1/tests/unit_tests/strategies/test_flexiblerollout.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/strategies/test_remoteaddress.py` & `UnleashClient-5.7.1/tests/unit_tests/strategies/test_remoteaddress.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/test_client.py` & `UnleashClient-5.7.1/tests/unit_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/test_constraints.py` & `UnleashClient-5.7.1/tests/unit_tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/test_custom_strategy.py` & `UnleashClient-5.7.1/tests/unit_tests/test_custom_strategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/test_features.py` & `UnleashClient-5.7.1/tests/unit_tests/test_features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/test_loader.py` & `UnleashClient-5.7.1/tests/unit_tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/unit_tests/test_variants.py` & `UnleashClient-5.7.1/tests/unit_tests/test_variants.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/utilities/mocks/mock_all_features.py` & `UnleashClient-5.7.1/tests/utilities/mocks/mock_all_features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/utilities/mocks/mock_constraints.py` & `UnleashClient-5.7.1/tests/utilities/mocks/mock_constraints.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/utilities/mocks/mock_custom_strategy.py` & `UnleashClient-5.7.1/tests/utilities/mocks/mock_custom_strategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/utilities/mocks/mock_features.py` & `UnleashClient-5.7.1/tests/utilities/mocks/mock_features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/utilities/mocks/mock_variants.py` & `UnleashClient-5.7.1/tests/utilities/mocks/mock_variants.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/utilities/old_code/StrategyV2.py` & `UnleashClient-5.7.1/tests/utilities/old_code/StrategyV2.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.7.0/tests/utilities/testing_constants.py` & `UnleashClient-5.7.1/tests/utilities/testing_constants.py`

 * *Files identical despite different names*

