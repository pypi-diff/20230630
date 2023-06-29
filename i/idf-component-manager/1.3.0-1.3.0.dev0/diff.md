# Comparing `tmp/idf_component_manager-1.3.0.tar.gz` & `tmp/idf_component_manager-1.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_component_manager-1.3.0.tar", last modified: Thu Jun 29 22:04:19 2023, max compression
+gzip compressed data, was "idf_component_manager-1.3.0.dev0.tar", last modified: Fri Mar 17 13:04:13 2023, max compression
```

## Comparing `idf_component_manager-1.3.0.tar` & `idf_component_manager-1.3.0.dev0.tar`

### file list

```diff
@@ -1,108 +1,104 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.302285 idf_component_manager-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10652 2023-06-29 22:04:19.302285 idf_component_manager-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9376 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.298285 idf_component_manager-1.3.0/idf_component_manager/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4463 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.298285 idf_component_manager-1.3.0/idf_component_manager/cli/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6243 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/cli/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4464 2023-06-29 15:12:23.000000 idf_component_manager-1.3.0/idf_component_manager/cli/component.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-06-29 15:12:23.000000 idf_component_manager-1.3.0/idf_component_manager/cli/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_manager/cli/core.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/cli/manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_manager/cli/project.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_manager/cli/registry.py
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/cli/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6568 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/cmake_component_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)    27373 2023-06-29 15:12:23.000000 idf_component_manager-1.3.0/idf_component_manager/core.py
--rw-rw-rw-   0 root         (0) root         (0)     6209 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9622 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_manager/dependencies.py
--rwxrwxrwx   0 root         (0) root         (0)     8695 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/idf_extensions.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/local_component_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.298285 idf_component_manager-1.3.0/idf_component_manager/prepare_components/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/prepare_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/prepare_components/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4014 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/prepare_components/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     3390 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/service_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.298285 idf_component_manager-1.3.0/idf_component_manager/templates/
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/templates/idf_component_template.yml
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.298285 idf_component_manager-1.3.0/idf_component_manager/version_solver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6279 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.302285 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/assignment.py
--rw-rw-rw-   0 root         (0) root         (0)     3904 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     9409 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/failure.py
--rw-rw-rw-   0 root         (0) root         (0)    14629 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/incompatibility.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/incompatibility_cause.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/package.py
--rw-rw-rw-   0 root         (0) root         (0)     4188 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/package_source.py
--rw-rw-rw-   0 root         (0) root         (0)     7477 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/partial_solution.py
--rw-rw-rw-   0 root         (0) root         (0)    12692 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/range.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/result.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/set_relation.py
--rw-rw-rw-   0 root         (0) root         (0)     6444 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/term.py
--rw-rw-rw-   0 root         (0) root         (0)     6996 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/union.py
--rw-rw-rw-   0 root         (0) root         (0)    15350 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/version_solver.py
--rw-rw-rw-   0 root         (0) root         (0)     6158 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_manager/version_solver/version_solver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.298285 idf_component_manager-1.3.0/idf_component_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10652 2023-06-29 22:04:19.000000 idf_component_manager-1.3.0/idf_component_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3872 2023-06-29 22:04:19.000000 idf_component_manager-1.3.0/idf_component_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 22:04:19.000000 idf_component_manager-1.3.0/idf_component_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-29 22:04:19.000000 idf_component_manager-1.3.0/idf_component_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      586 2023-06-29 22:04:19.000000 idf_component_manager-1.3.0/idf_component_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-29 22:04:19.000000 idf_component_manager-1.3.0/idf_component_manager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.302285 idf_component_manager-1.3.0/idf_component_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-29 21:48:13.000000 idf_component_manager-1.3.0/idf_component_tools/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    18685 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_tools/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/api_client_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_tools/api_schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     2965 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/archive_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3105 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/build_system_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     5273 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_tools/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     6240 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/file_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5324 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/file_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     8366 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/git_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3422 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/hash_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.302285 idf_component_manager-1.3.0/idf_component_tools/lock/
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/lock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4018 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/lock/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.302285 idf_component_manager-1.3.0/idf_component_tools/manifest/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-06-29 21:27:31.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/env_expander.py
--rw-rw-rw-   0 root         (0) root         (0)     5112 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/if_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5012 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     4489 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     9176 2023-06-29 21:27:31.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/solved_component.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/solved_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     7648 2023-06-29 21:27:31.000000 idf_component_manager-1.3.0/idf_component_tools/manifest/validator.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_tools/network_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.302285 idf_component_manager-1.3.0/idf_component_tools/semver/
--rw-rw-rw-   0 root         (0) root         (0)      452 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33154 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/semver/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 22:04:19.302285 idf_component_manager-1.3.0/idf_component_tools/sources/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6591 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_tools/sources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/sources/fetcher.py
--rw-rw-rw-   0 root         (0) root         (0)     7222 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_tools/sources/git.py
--rw-rw-rw-   0 root         (0) root         (0)     1206 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/sources/idf.py
--rw-rw-rw-   0 root         (0) root         (0)     5179 2023-06-29 21:15:05.000000 idf_component_manager-1.3.0/idf_component_tools/sources/local.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/sources/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9847 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/idf_component_tools/sources/web_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2023-06-29 21:48:13.000000 idf_component_manager-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 22:04:19.302285 idf_component_manager-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3165 2023-06-28 11:22:27.000000 idf_component_manager-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11845 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10564 2023-03-17 11:19:02.000000 idf_component_manager-1.3.0.dev0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4448 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5993 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/component.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2023-03-09 10:32:22.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/project.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6568 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cmake_component_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)    23423 2023-03-16 12:16:26.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     6209 2023-01-17 19:22:12.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9022 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/dependencies.py
+-rwxrwxrwx   0 root         (0) root         (0)     7671 2023-03-16 12:16:26.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/idf_extensions.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/local_component_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4014 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     3390 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/service_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/templates/idf_component_template.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/assignment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     9409 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/failure.py
+-rw-rw-rw-   0 root         (0) root         (0)    14629 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/incompatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/incompatibility_cause.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/package.py
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/package_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     7477 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/partial_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12692 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/range.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/result.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/set_relation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6444 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     6996 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/union.py
+-rw-rw-rw-   0 root         (0) root         (0)    15350 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/version_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6130 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/version_solver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11845 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3716 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      583 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-03-17 10:17:13.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15599 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/api_client_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/api_schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2965 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/archive_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/build_system_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4633 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-01-18 12:34:38.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     6240 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/file_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5324 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/file_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     8366 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/git_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2023-01-18 11:58:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/hash_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/lock/
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/lock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4050 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/lock/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/env_expander.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/if_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4859 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11187 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/solved_component.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/solved_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)    13069 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/semver/
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/semver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33154 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/semver/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6349 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2023-01-18 11:58:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/fetcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     7127 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/git.py
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/idf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4528 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/local.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/web_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2023-03-17 11:19:02.000000 idf_component_manager-1.3.0.dev0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3162 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/setup.py
```

### Comparing `idf_component_manager-1.3.0/LICENSE` & `idf_component_manager-1.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/PKG-INFO` & `idf_component_manager-1.3.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf_component_manager
-Version: 1.3.0
+Version: 1.3.0.dev0
 Summary: The component manager for ESP-IDF
 Home-page: https://github.com/espressif/idf-component-manager
 Author: Sergei Silnov
 Author-email: sergei.silnov@espressif.com
 Maintainer: Sergei Silnov
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,36 @@
 
 # IDF Component Manager
 
 The IDF Component manager is a tool that downloads dependencies for any [ESP-IDF](https://www.espressif.com/en/products/sdks/esp-idf) CMake project. It makes sure that the right versions of all components required for a successful build of your project are in place. The download happens automatically during a run of CMake. It can source components either from [the component registry](https://components.espressif.com/) or from a git repository.
 
 **A list of components can be found at https://components.espressif.com/**
 
-## [Official documentation](https://docs.espressif.com/projects/idf-component-manager/en/latest/)
+## Installing the IDF Component Manager
+
+IDF component manager can be used with ESP-IDF v4.1 and later.
+It is installed by default with ESP-IDF v4.4+ and recent bug-fix releases of ESP-IDF 4.1+.
+
+To check the installed version of the IDF component manager, first, activate [ESP-IDF environment](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html#installation). On macOS and Linux:
+
+```bash
+source $IDF_PATH/export.sh
+```
+
+Then run the command:
+
+```bash
+python -m idf_component_manager -h
+```
+
+To update to the most recent version:
+
+```bash
+pip install idf-component-manager --upgrade
+```
 
 ## Disabling the Component Manager
 
 The component manager can be explicitly disabled by setting `IDF_COMPONENT_MANAGER` environment variable to `0`.
 
 ## Using with a project
 
@@ -101,17 +122,31 @@
     version: "*"
     require: no # Download component but don't add it as a requirement
   namespace/pre_release_component:
     version: "*"
     pre_release: true # Allow downloading of pre-release versions
 ```
 
+## Environment variables in manifest
+
+You can use environment variables in values in `idf_component.yml` manifests. `$VAR` or `${VAR}` is replaced with the value of the `VAR` environment variable. If the environment variable is not defined, the component manager will raise an error.
+
+Variable name should be ASCII alphanumeric string (including underscores) and start with an underscore or ASCII letter. The first non-identifier character after the `$` terminates this placeholder specification. You can escape `$` with one more`$` character, i.e., `$$` is replaced with `$`.
+
+One possible use-case is providing authentication to git repositories accessed through HTTPS:
+
+```yaml
+dependencies:
+  my_component:
+    git: https://git:${ACCESS_TOKEN}@git.my_git.com/my_component.git
+```
+
 ## Component metadata caching
 
-By default, information about available versions of components not cached. If you make many requests to the registry from one machine, you can enable caching by setting `IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES` environment variable to the number of minutes to cache the data.
+By default information about available versions of components is cached for 5 minutes. You can adjust caching period by setting the duration in minutes to `IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES` environment variable or disable the cache entirely by setting it to 0.
 
 ## External links
 
 You can add links to the `idf_component.yml` file to the root of the manifest:
 
 ```yaml
 url: "https://example.com/homepage" # URL of the component homepage
@@ -122,15 +157,15 @@
 ```
 
 A link should be a correct HTTP(S) URL like `https://example.com/path` except the `repository` field,
 it is expected to be a valid [Git remote](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes) URL.
 
 ## Add examples to the component
 
-To add examples to your component, place them in the `examples` directory inside your component.
+To add examples to your component place them in the `examples` directory inside your component.
 Examples are discovered recursively in subdirectories at this path.
 A directory with `CMakeLists.txt` that registers a project is considered as an example.
 
 ## Custom example paths
 
 You can specify custom example paths for uploading them to the component registry.
 For that, add `examples` field to the root of the manifest:
@@ -145,25 +180,25 @@
 
 | Variable                                    | Default value (or example for required) | Required? | Description                                                                                     |
 | ------------------------------------------- | --------------------------------------- | --------- | ----------------------------------------------------------------------------------------------- |
 | IDF_COMPONENT_API_TOKEN                     |                                         | no        | API token to access the component registry                                                      |
 | IDF_COMPONENT_REGISTRY_URL                  | https://components.espressif.com/       | no        | URL of the default component registry                                                           |
 | IDF_COMPONENT_STORAGE_URL                   | https://components-file.espressif.com/  | no        | URL of the default file storage server                                                          |
 | IDF_COMPONENT_REGISTRY_PROFILE              | default                                 | no        | Profile in the config file to use for component registry                                        |
-| IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES  | 0                                       | no        | API Cache expiration time in minutes                                                            |
+| IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES  | 5                                       | no        | API Cache expiration time in minutes                                                            |
 | IDF_COMPONENT_CACHE_PATH                    | \* Depends on OS                        | no        | Cache directory for component manager                                                           |
 | COMPONENT_MANAGER_JOB_TIMEOUT               | 300                                     | no        | Timeout in seconds to wait for component processing                                             |
 | IDF_COMPONENT_OVERWRITE_MANAGED_COMPONENTS  | 0                                       | no        | Overwrite files in the managed_component directory, even if they have been modified by the user |
 | IGNORE_UNKNOWN_FILES_FOR_MANAGED_COMPONENTS | 0                                       | no        | Ignore unknown files in managed_components directory                                            |
 
 ## Contributions Guide
 
 We welcome all contributions to the Component Manager project.
 
-You can contribute by fixing bugs, adding features, adding documentation, or reporting an [issue](https://github.com/espressif/idf-component-manager/issues). We accept contributions via [GitHub Pull Requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
+You can contribute by fixing bugs, adding features, adding documentation, or reporting an [issue](https://github.com/espressif/idf-component-manager/issues). We accept contributions via [Github Pull Requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
 
 Before reporting an issue, make sure you've searched for a similar one that was already created. If you are reporting a new issue, please follow the Issue Template.
 
 ## Installing a development version of the component manager
 
 You can install the development version of the component manager from the main branch of this repository:
 
@@ -189,10 +224,9 @@
 python -m pip uninstall -y idf-component-manager
 # install the development version (from the main branch)
 python -m pip install git+https://github.com/espressif/idf-component-manager.git@main
 ```
 
 ## Resources
 
-- The Component manager [Documentation](https://docs.espressif.com/projects/idf-component-manager/en/latest/)
 - The Python Package Index project page https://pypi.org/project/idf-component-manager/
 - The Component Manager section in the [ESP-IDF Programming Guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-guides/tools/idf-component-manager.html)
```

### Comparing `idf_component_manager-1.3.0/README.md` & `idf_component_manager-1.3.0.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 # IDF Component Manager
 
 The IDF Component manager is a tool that downloads dependencies for any [ESP-IDF](https://www.espressif.com/en/products/sdks/esp-idf) CMake project. It makes sure that the right versions of all components required for a successful build of your project are in place. The download happens automatically during a run of CMake. It can source components either from [the component registry](https://components.espressif.com/) or from a git repository.
 
 **A list of components can be found at https://components.espressif.com/**
 
-## [Official documentation](https://docs.espressif.com/projects/idf-component-manager/en/latest/)
+## Installing the IDF Component Manager
+
+IDF component manager can be used with ESP-IDF v4.1 and later.
+It is installed by default with ESP-IDF v4.4+ and recent bug-fix releases of ESP-IDF 4.1+.
+
+To check the installed version of the IDF component manager, first, activate [ESP-IDF environment](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html#installation). On macOS and Linux:
+
+```bash
+source $IDF_PATH/export.sh
+```
+
+Then run the command:
+
+```bash
+python -m idf_component_manager -h
+```
+
+To update to the most recent version:
+
+```bash
+pip install idf-component-manager --upgrade
+```
 
 ## Disabling the Component Manager
 
 The component manager can be explicitly disabled by setting `IDF_COMPONENT_MANAGER` environment variable to `0`.
 
 ## Using with a project
 
@@ -71,17 +92,31 @@
     version: "*"
     require: no # Download component but don't add it as a requirement
   namespace/pre_release_component:
     version: "*"
     pre_release: true # Allow downloading of pre-release versions
 ```
 
+## Environment variables in manifest
+
+You can use environment variables in values in `idf_component.yml` manifests. `$VAR` or `${VAR}` is replaced with the value of the `VAR` environment variable. If the environment variable is not defined, the component manager will raise an error.
+
+Variable name should be ASCII alphanumeric string (including underscores) and start with an underscore or ASCII letter. The first non-identifier character after the `$` terminates this placeholder specification. You can escape `$` with one more`$` character, i.e., `$$` is replaced with `$`.
+
+One possible use-case is providing authentication to git repositories accessed through HTTPS:
+
+```yaml
+dependencies:
+  my_component:
+    git: https://git:${ACCESS_TOKEN}@git.my_git.com/my_component.git
+```
+
 ## Component metadata caching
 
-By default, information about available versions of components not cached. If you make many requests to the registry from one machine, you can enable caching by setting `IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES` environment variable to the number of minutes to cache the data.
+By default information about available versions of components is cached for 5 minutes. You can adjust caching period by setting the duration in minutes to `IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES` environment variable or disable the cache entirely by setting it to 0.
 
 ## External links
 
 You can add links to the `idf_component.yml` file to the root of the manifest:
 
 ```yaml
 url: "https://example.com/homepage" # URL of the component homepage
@@ -92,15 +127,15 @@
 ```
 
 A link should be a correct HTTP(S) URL like `https://example.com/path` except the `repository` field,
 it is expected to be a valid [Git remote](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes) URL.
 
 ## Add examples to the component
 
-To add examples to your component, place them in the `examples` directory inside your component.
+To add examples to your component place them in the `examples` directory inside your component.
 Examples are discovered recursively in subdirectories at this path.
 A directory with `CMakeLists.txt` that registers a project is considered as an example.
 
 ## Custom example paths
 
 You can specify custom example paths for uploading them to the component registry.
 For that, add `examples` field to the root of the manifest:
@@ -115,25 +150,25 @@
 
 | Variable                                    | Default value (or example for required) | Required? | Description                                                                                     |
 | ------------------------------------------- | --------------------------------------- | --------- | ----------------------------------------------------------------------------------------------- |
 | IDF_COMPONENT_API_TOKEN                     |                                         | no        | API token to access the component registry                                                      |
 | IDF_COMPONENT_REGISTRY_URL                  | https://components.espressif.com/       | no        | URL of the default component registry                                                           |
 | IDF_COMPONENT_STORAGE_URL                   | https://components-file.espressif.com/  | no        | URL of the default file storage server                                                          |
 | IDF_COMPONENT_REGISTRY_PROFILE              | default                                 | no        | Profile in the config file to use for component registry                                        |
-| IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES  | 0                                       | no        | API Cache expiration time in minutes                                                            |
+| IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES  | 5                                       | no        | API Cache expiration time in minutes                                                            |
 | IDF_COMPONENT_CACHE_PATH                    | \* Depends on OS                        | no        | Cache directory for component manager                                                           |
 | COMPONENT_MANAGER_JOB_TIMEOUT               | 300                                     | no        | Timeout in seconds to wait for component processing                                             |
 | IDF_COMPONENT_OVERWRITE_MANAGED_COMPONENTS  | 0                                       | no        | Overwrite files in the managed_component directory, even if they have been modified by the user |
 | IGNORE_UNKNOWN_FILES_FOR_MANAGED_COMPONENTS | 0                                       | no        | Ignore unknown files in managed_components directory                                            |
 
 ## Contributions Guide
 
 We welcome all contributions to the Component Manager project.
 
-You can contribute by fixing bugs, adding features, adding documentation, or reporting an [issue](https://github.com/espressif/idf-component-manager/issues). We accept contributions via [GitHub Pull Requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
+You can contribute by fixing bugs, adding features, adding documentation, or reporting an [issue](https://github.com/espressif/idf-component-manager/issues). We accept contributions via [Github Pull Requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
 
 Before reporting an issue, make sure you've searched for a similar one that was already created. If you are reporting a new issue, please follow the Issue Template.
 
 ## Installing a development version of the component manager
 
 You can install the development version of the component manager from the main branch of this repository:
 
@@ -159,10 +194,9 @@
 python -m pip uninstall -y idf-component-manager
 # install the development version (from the main branch)
 python -m pip install git+https://github.com/espressif/idf-component-manager.git@main
 ```
 
 ## Resources
 
-- The Component manager [Documentation](https://docs.espressif.com/projects/idf-component-manager/en/latest/)
 - The Python Package Index project page https://pypi.org/project/idf-component-manager/
 - The Component Manager section in the [ESP-IDF Programming Guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-guides/tools/idf-component-manager.html)
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager/__main__.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
 import os
 import sys
 import warnings
 
@@ -31,30 +31,30 @@
             raise ValueError('--{} is required'.format(_f.replace('_', '-')))
 
 
 def main(command_args=None):  # type: (list[str] | None) -> None
     parser = argparse.ArgumentParser(description='IDF component manager v{}'.format(version))
     parser.add_argument('command', choices=KNOWN_ACTIONS, help='Command to execute')
     parser.add_argument('--path', help='Working directory (default: current directory).', default=os.getcwd())
-    parser.add_argument('--namespace', help='Namespace for the component. Can be set in the config file.')
+    parser.add_argument('--namespace', help='Namespace for the component. Can be set in config file.')
     parser.add_argument(
         '--service-profile',
-        help='Profile for the component registry to use. By default profile named "default" will be used.',
+        help='Profile for component registry to use. By default profile named "default" will be used.',
         default='default',
     )
-    parser.add_argument('--name', help='Component name.')
+    parser.add_argument('--name', help='Component name')
     parser.add_argument('--archive', help='Path of the archive with component to upload.')
     parser.add_argument('--job', help='Background job ID.')
     parser.add_argument('--version', help='Version for upload or deletion.')
     parser.add_argument('--skip-pre-release', help='Do not upload pre-release versions.', action='store_true')
     parser.add_argument(
         '--check-only', help='Check if given component version is already uploaded and exit.', action='store_true')
     parser.add_argument(
         '--allow-existing', help='Return success if existing version is already uploaded.', action='store_true')
-    parser.add_argument('--example', help='Example name.')
+    parser.add_argument('--example', help='Example name')
 
     args = parser.parse_args(args=command_args)
 
     try:
         warnings.showwarning = showwarning
         manager = ComponentManager(args.path)
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager/cli/autocompletion.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/cli/autocompletion.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,66 +120,63 @@
     def wrapper(func):
         func.__doc__ = docstring
         return func
 
     return wrapper
 
 
-def init_autocomplete():
-    @click.command()
-    @click.option('--shell', required=True, type=click.Choice(['bash', 'zsh', 'fish']), help='Shell type')
-    @click.option(
-        '--install',
-        is_flag=True,
-        default=False,
-        help='Create the completion files and inject the sourcing script into your rc files if this flag is set.')
-    @click.option(
-        '--dry-run',
-        is_flag=True,
-        default=False,
-        help='Only useful when flag "--install" is set. Instead of real file system changes, '
-        'log would be printed if this flag is set.')
-    @_doc(_DOC_STRSTRING)
-    def autocomplete(shell, install, dry_run):
-        if shell == 'fish':
-            if CLICK_VERSION < Version('7.1.0'):  # fish support was added in 7.1
-                raise FatalError(
-                    'Autocomplete for the fish shell is only supported by library `click` version 7.1 and higher. '
-                    'An older version is installed on your machine due to an outdated version of python. '
-                    'We recommend using python 3.7 and higher with compote CLI.')
-
-        # the return code could be 1 even succeeded
-        # use || true to swallow the return code
-        autocomplete_script_str = subprocess.check_output(
-            '_{}_COMPLETE={} {} || true'.format(CLI_NAME.upper(), _get_shell_completion(shell), CLI_NAME),
-            shell=True).decode('utf8')  # nosec
-
-        if not install:  # print the autocomplete script only
-            print(autocomplete_script_str)
-            return
-
-        # write autocomplete script
-        completion_filepath = os.path.realpath(os.path.expanduser(_COMPLETE_FILE_PATH[shell]))
-        if not os.path.isdir(os.path.dirname(completion_filepath)):
-            if not dry_run:
-                os.makedirs(os.path.dirname(completion_filepath))
-
-        if dry_run:
-            print_info('Completion file would be created at: {}'.format(completion_filepath))
-        else:
-            with open(completion_filepath, 'w') as fw:
-                fw.write(autocomplete_script_str)
-
-        # write sourcing autocomplete script statements
-        if _RC_FILE_PATH[shell] and _SOURCING_STR[shell]:
-            rc_filepath = os.path.realpath(os.path.expanduser(_RC_FILE_PATH[shell]))
-            # enable zsh autocomplete
-            if shell == 'zsh':
-                _append_text_line('autoload -Uz compinit', rc_filepath, dry_run=dry_run)
-                _append_text_line(['compinit', 'compinit -u'], rc_filepath, dry_run=dry_run)
-
-            _append_text_line(
-                '# ESP-IDF component manager compote CLI autocompletion\n{}'.format(_SOURCING_STR[shell]),
-                rc_filepath,
-                dry_run=dry_run)
-
-    return autocomplete
+@click.command()
+@click.option('--shell', required=True, type=click.Choice(['bash', 'zsh', 'fish']), help='Shell type')
+@click.option(
+    '--install',
+    is_flag=True,
+    default=False,
+    help='Create the completion files and inject the sourcing script into your rc files if this flag is set.')
+@click.option(
+    '--dry-run',
+    is_flag=True,
+    default=False,
+    help='Only useful when flag "--install" is set. Instead of real file system changes, '
+    'log would be printed if this flag is set.')
+@_doc(_DOC_STRSTRING)
+def autocomplete(shell, install, dry_run):
+    if shell == 'fish':
+        if CLICK_VERSION < Version('7.1.0'):  # fish support was added in 7.1
+            raise FatalError(
+                'Autocomplete for the fish shell is only supported by library `click` version 7.1 and higher. '
+                'An older version is installed on your machine due to an outdated version of python. '
+                'We recommend using python 3.7 and higher with compote CLI.')
+
+    # the return code could be 1 even succeeded
+    # use || true to swallow the return code
+    autocomplete_script_str = subprocess.check_output(
+        '_{}_COMPLETE={} {} || true'.format(CLI_NAME.upper(), _get_shell_completion(shell), CLI_NAME),
+        shell=True).decode('utf8')  # nosec
+
+    if not install:  # print the autocomplete script only
+        print(autocomplete_script_str)
+        return
+
+    # write autocomplete script
+    completion_filepath = os.path.realpath(os.path.expanduser(_COMPLETE_FILE_PATH[shell]))
+    if not os.path.isdir(os.path.dirname(completion_filepath)):
+        if not dry_run:
+            os.makedirs(os.path.dirname(completion_filepath))
+
+    if dry_run:
+        print_info('Completion file would be created at: {}'.format(completion_filepath))
+    else:
+        with open(completion_filepath, 'w') as fw:
+            fw.write(autocomplete_script_str)
+
+    # write sourcing autocomplete script statements
+    if _RC_FILE_PATH[shell] and _SOURCING_STR[shell]:
+        rc_filepath = os.path.realpath(os.path.expanduser(_RC_FILE_PATH[shell]))
+        # enable zsh autocomplete
+        if shell == 'zsh':
+            _append_text_line('autoload -Uz compinit', rc_filepath, dry_run=dry_run)
+            _append_text_line(['compinit', 'compinit -u'], rc_filepath, dry_run=dry_run)
+
+        _append_text_line(
+            '# ESP-IDF component manager compote CLI autocompletion\n{}'.format(_SOURCING_STR[shell]),
+            rc_filepath,
+            dry_run=dry_run)
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager/cli/cache.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/cli/cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 import click
 
 from idf_component_manager.utils import print_info
 from idf_component_tools.file_cache import FileCache
 from idf_component_tools.file_tools import human_readable_size
 
 
-def init_cache():
-    @click.group()
-    def cache():
-        """
-        Group of commands to manage cache of the IDF Component Manager.
-        """
-        pass
-
-    @cache.command()
-    def clear():
-        """
-        Clear the cache of components and API client cache.
-        """
-        FileCache().clear()
-        print_info('Successfully cleared cache at\n\t{}'.format(FileCache().path()))
-
-    @cache.command()
-    def path():
-        """
-        Print the cache path.
-        """
-        print_info(FileCache().path())
-
-    @cache.command()
-    @click.option('--bytes', is_flag=True, default=False, help='Print size in bytes')
-    def size(bytes):
-        """
-        Print the cache size in human readable format.
-        """
-        size = FileCache().size()
-        if bytes:
-            print_info(str(size))
-        else:
-            print_info(human_readable_size(size))
-
-    return cache
+@click.group()
+def cache():
+    """
+    Group of cache related commands
+    """
+    pass
+
+
+@cache.command()
+def clear():
+    """
+    Clear cache of components and API client cache
+    """
+    FileCache().clear()
+    print_info('Successfully cleared cache at\n\t{}'.format(FileCache().path()))
+
+
+@cache.command()
+def path():
+    """
+    Print cache path
+    """
+    print_info(FileCache().path())
+
+
+@cache.command()
+@click.option('--bytes', is_flag=True, default=False, help='Print size in bytes')
+def size(bytes):
+    """
+    Print cache size of cache in human readable format
+    """
+    size = FileCache().size()
+    if bytes:
+        print_info(str(size))
+    else:
+        print_info(human_readable_size(size))
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager/cli/component.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/cli/component.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,114 +1,84 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import click
 
-from .constants import get_dest_dir_option, get_namespace_name_options, get_project_dir_option, get_project_options
+from .constants import NAMESPACE_NAME_OPTIONS, PROJECT_DIR_OPTION, PROJECT_OPTIONS
 from .utils import add_options
 
 
-def init_component():
+@click.group()
+def component():
+    """
+    Group of component related commands
+    """
+    pass
 
-    PROJECT_DIR_OPTION = get_project_dir_option()
-    PROJECT_OPTIONS = get_project_options()
-    NAMESPACE_NAME_OPTIONS = get_namespace_name_options()
-    DEST_DIR_OPTION = get_dest_dir_option()
-
-    @click.group()
-    def component():
-        """
-        Group of commands to interact with components.
-        """
-        pass
-
-    COMPONENT_VERSION_OPTION = [
-        click.option(
-            '--version',
-            help='Set version if not defined in the manifest. Use "git" to get version from the git tag. '
-            '(command would fail if running not from a git tag)',
-        )
-    ]
-
-    @component.command()
-    @add_options(PROJECT_DIR_OPTION + NAMESPACE_NAME_OPTIONS + COMPONENT_VERSION_OPTION + DEST_DIR_OPTION)
-    def pack(manager, namespace, name, version, dest_dir):  # noqa: namespace is not used
-        """
-        Create component archive and store it in the dist directory.
-        """
-        manager.pack_component(name=name, version=version, dest_dir=dest_dir)
-
-    @component.command()
-    @add_options(PROJECT_OPTIONS + NAMESPACE_NAME_OPTIONS + COMPONENT_VERSION_OPTION + DEST_DIR_OPTION)
-    @click.option(
-        '--archive',
-        help='Path of the archive with a component to upload. '
-        'When not provided the component will be packed automatically.',
+
+COMPONENT_VERSION_OPTION = [
+    click.option(
+        '--version',
+        help='Set version if not defined in the manifest. Use "git" to get version from the git tag. '
+        '(command would fail if running not from a git tag)',
     )
-    @click.option('--skip-pre-release', is_flag=True, default=False, help='Do not upload pre-release versions.')
-    @click.option(
-        '--check-only',
-        is_flag=True,
-        default=False,
-        help='Check if given component version is already uploaded and exit.')
-    @click.option(
-        '--allow-existing', is_flag=True, default=False, help='Return success if existing version is already uploaded.')
-    @click.option(
-        '--dry-run',
-        is_flag=True,
-        default=False,
-        help='Upload component for validation without creating a version in the registry.')
-    def upload(
-            manager, service_profile, namespace, name, version, archive, skip_pre_release, check_only, allow_existing,
-            dry_run, dest_dir):
-        """
-        Upload component to the component registry.
-
-        If the component doesn't exist in the registry it will be created automatically.
-        """
-        manager.upload_component(
-            name,
-            version=version,
-            service_profile=service_profile,
-            namespace=namespace,
-            archive=archive,
-            skip_pre_release=skip_pre_release,
-            check_only=check_only,
-            allow_existing=allow_existing,
-            dry_run=dry_run,
-            dest_dir=dest_dir,
-        )
-
-    @component.command()
-    @add_options(PROJECT_OPTIONS)
-    @click.option('--job', required=True, help='Upload job ID')
-    def upload_status(manager, service_profile, job):
-        """
-        Check the component uploading status.
-        """
-        manager.upload_component_status(job, service_profile=service_profile)
-
-    @component.command()
-    @add_options(PROJECT_OPTIONS + NAMESPACE_NAME_OPTIONS)
-    @click.option('--version', required=True, help='Component version to delete.')
-    def delete(manager, service_profile, namespace, name, version):
-        """
-        Delete specified version of the component from the component registry.
-        The deleted version cannot be restored or re-uploaded.
-        """
-        manager.delete_version(name, version, service_profile=service_profile, namespace=namespace)
-
-    @component.command()
-    @add_options(PROJECT_OPTIONS + NAMESPACE_NAME_OPTIONS)
-    @click.option('--version', required=True, help='Component version to yank version.')
-    @click.option(
-        '--message',
-        required=True,
-        help='Message explaining why the component version is being removed from the registry.')
-    def yank(manager, service_profile, namespace, name, version, message):
-        """
-        Yank specified version of the component from the component registry.
-        Yanked version can be downloaded from the registry with warning message.
-        """
-        manager.yank_version(name, version, message, service_profile=service_profile, namespace=namespace)
+]
+
+
+@component.command()
+@add_options(PROJECT_DIR_OPTION + NAMESPACE_NAME_OPTIONS + COMPONENT_VERSION_OPTION)
+def pack(manager, namespace, name, version):  # noqa: namespace is not used
+    """
+    Create component archive and store it in the dist directory.
+    """
+    manager.pack_component(name, version)
+
+
+@component.command()
+@add_options(PROJECT_OPTIONS + NAMESPACE_NAME_OPTIONS + COMPONENT_VERSION_OPTION)
+@click.option(
+    '--archive',
+    help='Path of the archive with a component to upload. '
+    'When not provided the component will be packed automatically.',
+)
+@click.option('--skip-pre-release', is_flag=True, default=False, help='Do not upload pre-release versions.')
+@click.option(
+    '--check-only', is_flag=True, default=False, help='Check if given component version is already uploaded and exit.')
+@click.option(
+    '--allow-existing', is_flag=True, default=False, help='Return success if existing version is already uploaded.')
+def upload(manager, service_profile, namespace, name, version, archive, skip_pre_release, check_only, allow_existing):
+    """
+    Upload component to the component registry.
+
+    If the component doesn't exist in the registry it will be created automatically.
+    """
+    manager.upload_component(
+        name,
+        version=version,
+        service_profile=service_profile,
+        namespace=namespace,
+        archive=archive,
+        skip_pre_release=skip_pre_release,
+        check_only=check_only,
+        allow_existing=allow_existing,
+    )
+
 
-    return component
+@component.command()
+@add_options(PROJECT_OPTIONS)
+@click.option('--job', required=True, help='Upload job ID')
+def upload_status(manager, service_profile, job):
+    """
+    Check the component uploading status.
+    """
+    manager.upload_component_status(job, service_profile=service_profile)
+
+
+@component.command()
+@add_options(PROJECT_OPTIONS + NAMESPACE_NAME_OPTIONS)
+@click.option('--version', required=True, help='Component version to delete')
+def delete(manager, service_profile, namespace, name, version):
+    """
+    Delete specified version of the component from the component registry.
+    The deleted version cannot be restored or re-uploaded.
+    """
+    manager.delete_version(name, version, service_profile=service_profile, namespace=namespace)
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager/cli/project.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/cli/project.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import click
 
-from .constants import get_project_dir_option
+from .constants import PROJECT_DIR_OPTION
 from .utils import add_options
 
 
-def init_project():
-
-    PROJECT_DIR_OPTION = get_project_dir_option()
-
-    @click.group()
-    def project():
-        """
-        Group of project related commands
-        """
-        pass
-
-    @project.command()
-    @add_options(PROJECT_DIR_OPTION)
-    @click.option(
-        '-p',
-        '--path',
-        default=None,
-        help='Path of the new project. The project will be created directly in the given folder if it is empty.')
-    @click.argument('example', required=True)
-    def create_from_example(manager, example, path):
-        """
-        Create a project from an example.
-
-        You can specify EXAMPLE in the format like:
-        namespace/name=1.0.0:example
-
-        where "=1.0.0" is a version specification.
-
-        An example command:
-
-        compote project create-from-example example/cmp^3.3.8:cmp_ex
-
-        Namespace and version are optional in the EXAMPLE argument.
-        """
-        manager.create_project_from_example(example, path=path)
-
-    @project.command()
-    @add_options(PROJECT_DIR_OPTION)
-    def remove_managed_components(manager):
-        """
-        Remove the managed_components folder.
-        """
-        manager.remove_managed_components()
-
-    return project
+@click.group()
+def project():
+    """
+    Group of project related commands
+    """
+    pass
+
+
+@project.command()
+@add_options(PROJECT_DIR_OPTION)
+@click.option(
+    '-p',
+    '--path',
+    default=None,
+    help='Path of the new project. The project will be created directly in the given folder if it is empty.')
+@click.argument('example', required=True)
+def create_from_example(manager, example, path):
+    """
+    Create a project from an example.
+
+    You can specify EXAMPLE in the format like:
+      namespace/name=1.0.0:example
+
+    where "=1.0.0" is a version specification.
+
+    An example command:
+
+      compote project create-from-example example/cmp^3.3.8:cmp_ex
+
+    Namespace and version are optional in the EXAMPLE argument.
+    """
+    manager.create_project_from_example(example, path=path)
+
+
+@project.command()
+@add_options(PROJECT_DIR_OPTION)
+def remove_managed_components(manager):
+    """
+    Remove the managed_components folder.
+    """
+    manager.remove_managed_components()
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager/cmake_component_requirements.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/cmake_component_requirements.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/core.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 from datetime import datetime, timedelta
 from io import open
 from pathlib import Path
 
 import requests
 
 from idf_component_manager.utils import print_info, print_warn
-from idf_component_tools.api_client_errors import APIClientError, ComponentNotFound, NetworkConnectionError
+from idf_component_tools.api_client_errors import APIClientError, NetworkConnectionError, VersionNotFound
 from idf_component_tools.archive_tools import pack_archive, unpack_archive
-from idf_component_tools.build_system_tools import build_name, is_component
-from idf_component_tools.environment import getenv_int
-from idf_component_tools.errors import (
-    FatalError, GitError, ManifestError, NothingToDoError, VersionAlreadyExistsError, VersionNotFoundError)
+from idf_component_tools.build_system_tools import build_name
+from idf_component_tools.errors import FatalError, GitError, ManifestError, NothingToDoError
 from idf_component_tools.file_tools import check_unexpected_component_files, copy_filtered_directory, create_directory
 from idf_component_tools.git_client import GitClient
 from idf_component_tools.hash_tools import (
     HashDoesNotExistError, HashNotEqualError, HashNotSHA256Error, validate_managed_component_hash)
 from idf_component_tools.manifest import (
     MANIFEST_FILENAME, WEB_DEPENDENCY_REGEX, Manifest, ManifestManager, ProjectRequirements)
 from idf_component_tools.semver import SimpleSpec, Version
@@ -40,25 +38,21 @@
 from .service_details import service_details
 
 try:
     from typing import Optional, Tuple
 except ImportError:
     pass
 
-
-# PROCESSING_TIMEOUT
-def get_processing_timeout():
-    try:
-        return getenv_int('COMPONENT_MANAGER_JOB_TIMEOUT', 300)
-    except ValueError:
-        print_warn(
-            'Cannot parse value of COMPONENT_MANAGER_JOB_TIMEOUT.'
-            ' It should be number of seconds to wait for job result.')
-        return 300
-
+try:
+    PROCESSING_TIMEOUT = int(os.getenv('COMPONENT_MANAGER_JOB_TIMEOUT', 300))
+except TypeError:
+    print_warn(
+        'Cannot parse value of COMPONENT_MANAGER_JOB_TIMEOUT.'
+        ' It should be number of seconds to wait for job result.')
+    PROCESSING_TIMEOUT = 300
 
 CHECK_INTERVAL = 3
 MAX_PROGRESS = 100  # Expected progress is in percent
 
 
 def general_error_handler(func):
     @functools.wraps(func)
@@ -70,99 +64,72 @@
                 'Cannot establish a connection to the component registry. Are you connected to the internet?')
         except APIClientError as e:
             raise FatalError(e)
 
     return wrapper
 
 
-def _create_manifest_if_missing(manifest_dir):  # type: (str) -> bool
-    manifest_filepath = os.path.join(manifest_dir, MANIFEST_FILENAME)
-    if os.path.exists(manifest_filepath):
-        return False
-    example_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'templates', 'idf_component_template.yml')
-    create_directory(manifest_dir)
-    shutil.copyfile(example_path, manifest_filepath)
-    print_info('Created "{}"'.format(manifest_filepath))
-    return True
-
-
 class ComponentManager(object):
     def __init__(self, path, lock_path=None, manifest_path=None, interface_version=0):
         # type: (str, Optional[str], Optional[str], int) -> None
 
         # Working directory
-        path = os.path.abspath(path)
-        self.path = path
+        self.path = os.path.abspath(path)
 
         # Set path of the project's main component
-        self.main_component_path = os.path.join(path, 'main')
+        self.main_component_path = os.path.join(self.path, 'main')
 
         # Set path of the manifest file for the project's main component
         self.main_manifest_path = manifest_path or (
             os.path.join(path, 'main', MANIFEST_FILENAME) if os.path.isdir(path) else path)
-        self.main_component_path = os.path.normpath(self.main_component_path)
 
         # Lock path
         if not lock_path:
             if os.path.isfile(path):
                 self.lock_path = path
             else:
                 self.lock_path = os.path.join(path, 'dependencies.lock')
         elif os.path.isabs(lock_path):
             self.lock_path = lock_path
         else:
             self.lock_path = os.path.join(path, lock_path)
 
-        self.lock_path = os.path.abspath(self.lock_path)
-
         # Components directories
         self.components_path = os.path.join(self.path, 'components')
         self.managed_components_path = os.path.join(self.path, 'managed_components')
 
         # Dist directory
         self.dist_path = os.path.join(self.path, 'dist')
 
         self.interface_version = interface_version
 
-    def _get_manifest_dir(self, component='main', path=None):  # type: (str, Optional[str]) -> str
-        if component != 'main' and path is not None:
-            raise FatalError('Cannot determine manifest directory. Please specify either component or path.')
-
-        # If path is specified
-        if path is not None:
-            manifest_dir = os.path.abspath(path)
-        # If the current working directory is in the context of a component
-        elif is_component(Path(os.getcwd())):
-            manifest_dir = os.getcwd()
-        else:
-            # If the current working directory is in the context of a project
-            base_dir = self.path if component == 'main' else self.components_path
-            manifest_dir = os.path.join(base_dir, component)
+    def _get_manifest(self, component='main'):  # type: (str) -> Tuple[str, bool]
+        base_dir = self.path if component == 'main' else self.components_path
+        manifest_dir = os.path.join(base_dir, component)
 
         if not os.path.isdir(manifest_dir):
             raise FatalError(
                 'Directory "{}" does not exist! '
-                'Please specify a valid component under {} or try to use --path'.format(manifest_dir, self.path))
-        if not manifest_dir.startswith(self.path):
-            raise FatalError(
-                'Directory "{}" is not under project directory! '
                 'Please specify a valid component under {}'.format(manifest_dir, self.path))
 
-        return manifest_dir
-
-    def _get_manifest(self, component='main', path=None):  # type: (str, Optional[str]) -> Tuple[str, bool]
-        manifest_dir = self._get_manifest_dir(component=component, path=path)
         manifest_filepath = os.path.join(manifest_dir, MANIFEST_FILENAME)
+        created = False
         # Create manifest file if it doesn't exist in work directory
-        manifest_created = _create_manifest_if_missing(manifest_dir)
-        return manifest_filepath, manifest_created
+        if not os.path.exists(manifest_filepath):
+            example_path = os.path.join(
+                os.path.dirname(os.path.realpath(__file__)), 'templates', 'idf_component_template.yml')
+            create_directory(manifest_dir)
+            shutil.copyfile(example_path, manifest_filepath)
+            print_info('Created "{}"'.format(manifest_filepath))
+            created = True
+        return manifest_filepath, created
 
     @general_error_handler
-    def create_manifest(self, component='main', path=None):  # type: (str, Optional[str]) -> None
-        manifest_filepath, created = self._get_manifest(component=component, path=path)
+    def create_manifest(self, component='main'):  # type: (str) -> None
+        manifest_filepath, created = self._get_manifest(component)
         if not created:
             print_info('"{}" already exists, skipping...'.format(manifest_filepath))
 
     @general_error_handler
     def create_project_from_example(self, example, path=None, service_profile=None):
         # type: (str, str | None, str | None) -> None
 
@@ -178,46 +145,36 @@
 
         if os.path.isdir(project_path) and os.listdir(project_path):
             raise FatalError(
                 'The directory {} is not empty. To create an example you must empty the directory or '
                 'choose a different path.'.format(project_path),
                 exit_code=3)
 
-        component_details = client.component(component_name=component_name, version=version_spec)
+        try:
+            component_details = client.component(component_name=component_name, version=version_spec)
+        except VersionNotFound as e:
+            raise FatalError(e)
+        except APIClientError:
+            raise FatalError('Selected component "{}" doesn\'t exist.'.format(component_name))
 
         try:
             example_url = [example for example in component_details.examples if example_name == example['name']][-1]
         except IndexError:
             raise FatalError(
                 'Cannot find example "{}" for "{}" version "{}"'.format(example_name, component_name, version_spec),
                 exit_code=2)
 
         response = requests.get(example_url['url'], stream=True)
         with tarfile.open(fileobj=response.raw, mode='r|gz') as tar:
             tar.extractall(project_path)
         print_info('Example "{}" successfully downloaded to {}'.format(example_name, os.path.abspath(project_path)))
 
     @general_error_handler
-    def add_dependency(
-            self,
-            dependency,
-            component='main',
-            path=None,
-            service_profile=None):  # type: (str, str, Optional[str], str | None) -> None
-
-        client, _ = service_details(None, service_profile, token_required=False)
-
-        manifest_filepath, _ = self._get_manifest(component=component, path=path)
-
-        if path is not None:
-            component_path = os.path.abspath(path)
-            component = os.path.basename(component_path)
-        # If the path refers to a component context we need to use the components name as the component
-        elif is_component(Path(os.getcwd())):
-            component = os.path.basename(os.path.normpath(self.path))
+    def add_dependency(self, dependency, component='main'):  # type: (str, str) -> None
+        manifest_filepath, _ = self._get_manifest(component)
 
         match = re.match(WEB_DEPENDENCY_REGEX, dependency)
         if match:
             name, spec = match.groups()
         else:
             raise FatalError('Invalid dependency: "{}". Please use format "namespace/name".'.format(dependency))
 
@@ -227,18 +184,14 @@
         try:
             SimpleSpec(spec)
         except ValueError:
             raise FatalError(
                 'Invalid dependency version requirement: {}. Please use format like ">=1" or "*".'.format(spec))
 
         name = WebServiceSource().normalized_name(name)
-
-        # Check if dependency exists in the registry
-        client.component(component_name=name, version=spec)
-
         manifest_manager = ManifestManager(manifest_filepath, component)
         manifest = manifest_manager.load()
 
         for dep in manifest.dependencies:
             if dep.name == name:
                 raise FatalError('Dependency "{}" already exists for in manifest "{}"'.format(name, manifest_filepath))
 
@@ -269,46 +222,43 @@
                 "It's likely due to the 4 spaces used for indentation we recommend using 2 spaces indent. "
                 'Please check the manifest file:\n{}'.format(manifest_filepath))
 
         shutil.move(temp_manifest_file.name, manifest_filepath)
         print_info('Successfully added dependency "{}{}" to component "{}"'.format(name, spec, manifest_manager.name))
 
     @general_error_handler
-    def pack_component(self, name, version, dest_dir=None):  # type: (str, str, Optional[str]) -> Tuple[str, Manifest]
-
-        dest_path = os.path.join(self.path, dest_dir) if dest_dir else self.dist_path
-
+    def pack_component(self, name, version):  # type: (str, str) -> Tuple[str, Manifest]
         if version == 'git':
             try:
                 version = str(GitClient().get_tag_version())
             except GitError:
                 raise FatalError('An error happened while getting version from git tag')
         elif version:
             try:
                 Version.parse(version)
             except ValueError:
                 raise FatalError('Version parameter must be either "git" or a valid semantic version')
 
         manifest_manager = ManifestManager(self.path, name, check_required_fields=True, version=version)
         manifest = manifest_manager.load()
-        dest_temp_dir = Path(dest_path, dist_name(manifest))
+        dist_temp_dir = Path(self.dist_path, dist_name(manifest))
         include = set(manifest.files['include'])
         exclude = set(manifest.files['exclude'])
-        copy_filtered_directory(self.path, str(dest_temp_dir), include=include, exclude=exclude)
+        copy_filtered_directory(self.path, str(dist_temp_dir), include=include, exclude=exclude)
 
         if manifest.examples:
-            copy_examples_folders(manifest.examples, Path(self.path), dest_temp_dir, include=include, exclude=exclude)
+            copy_examples_folders(manifest.examples, Path(self.path), dist_temp_dir, include=include, exclude=exclude)
 
-        manifest_manager.dump(str(dest_temp_dir))
+        manifest_manager.dump(str(dist_temp_dir))
 
-        check_unexpected_component_files(str(dest_temp_dir))
+        check_unexpected_component_files(str(dist_temp_dir))
 
-        archive_filepath = os.path.join(dest_path, archive_filename(manifest))
+        archive_filepath = os.path.join(self.dist_path, archive_filename(manifest))
         print_info('Saving archive to "{}"'.format(archive_filepath))
-        pack_archive(str(dest_temp_dir), archive_filepath)
+        pack_archive(str(dist_temp_dir), archive_filepath)
         return archive_filepath, manifest
 
     @general_error_handler
     def delete_version(
             self,
             name,  # type: str
             version,  # type: str
@@ -321,43 +271,21 @@
             raise FatalError('Argument "version" is required')
 
         component_name = '/'.join([namespace, name])
         # Checking if current version already uploaded
         versions = client.versions(component_name=component_name).versions
 
         if version not in versions:
-            raise VersionNotFoundError(
-                'Version {} of the component "{}" is not on the registry'.format(version, component_name))
+            raise NothingToDoError(
+                'Version {} of the component "{}" is not on the service'.format(version, component_name))
 
         client.delete_version(component_name=component_name, component_version=version)
         print_info('Deleted version {} of the component {}'.format(component_name, version))
 
     @general_error_handler
-    def yank_version(
-            self,
-            name,  # type: str
-            version,  # type: str
-            message,  # type: str
-            service_profile=None,  # type: str | None
-            namespace=None  # type: str | None
-    ):
-        client, namespace = service_details(namespace, service_profile)
-        component_name = '/'.join([namespace, name])
-
-        versions = client.versions(component_name=component_name).versions
-
-        if version not in versions:
-            raise VersionNotFoundError(
-                'Version {} of the component "{}" is not on the registry'.format(version, component_name))
-
-        client.yank_version(component_name=component_name, component_version=version, yank_message=message)
-        print_info(
-            'Version {} of the component {} was yanked due to reason "{}"'.format(component_name, version, message))
-
-    @general_error_handler
     def remove_managed_components(self, **kwargs):  # kwargs here to keep idf_extension.py compatibility
         managed_components_dir = Path(self.path, 'managed_components')
 
         if not managed_components_dir.is_dir():
             return
 
         undeleted_components = []
@@ -386,106 +314,85 @@
             name,  # type: str
             version=None,  # type: str | None
             service_profile=None,  # type: str | None
             namespace=None,  # type: str | None
             archive=None,  # type: str | None
             skip_pre_release=False,  # type: bool
             check_only=False,  # type: bool
-            allow_existing=False,  # type: bool
-            dry_run=False,  # type: bool
-            dest_dir=None):  # type: (...) -> None
+            allow_existing=False):  # type: (...) -> None
         client, namespace = service_details(namespace, service_profile)
-
         if archive:
             if not os.path.isfile(archive):
                 raise FatalError('Cannot find archive to upload: {}'.format(archive))
 
             if version:
                 raise FatalError('Parameters "version" and "archive" are not supported at the same time')
 
             tempdir = tempfile.mkdtemp()
             try:
                 unpack_archive(archive, tempdir)
                 manifest = ManifestManager(tempdir, name, check_required_fields=True).load()
             finally:
                 shutil.rmtree(tempdir)
         else:
-            archive, manifest = self.pack_component(name=name, version=version, dest_dir=dest_dir)
+            archive, manifest = self.pack_component(name, version)
 
         if not manifest.version:
             raise FatalError('"version" field is required when uploading the component')
 
         if not manifest.version.is_semver:
             raise FatalError('Only components with semantic versions are allowed on the service')
 
         if manifest.version.semver.prerelease and skip_pre_release:
             raise NothingToDoError('Skipping pre-release version {}'.format(manifest.version))
 
         component_name = '/'.join([namespace, manifest.name])
         # Checking if current version already uploaded
-        try:
-            versions = client.versions(component_name=component_name, spec='*').versions
+        versions = client.versions(component_name=component_name, spec='*').versions
+        if manifest.version in versions:
+            if allow_existing:
+                return
 
-            if manifest.version in versions:
-                if allow_existing:
-                    return
-
-                raise VersionAlreadyExistsError(
-                    'Version {} of the component "{}" is already on the registry'.format(
-                        manifest.version, component_name))
-        except ComponentNotFound:
-            # It's ok if component doesn't exist yet
-            pass
+            raise NothingToDoError(
+                'Version {} of the component "{}" is already on the service'.format(manifest.version, component_name))
 
         # Exit if check flag was set
         if check_only:
             return
 
-        # Uploading/validating the component
-        info_message = 'Uploading' if not dry_run else 'Validating'
-        print_info('%s archive %s' % (info_message, archive))
-        job_id = client.upload_version(component_name=component_name, file_path=archive, validate_only=dry_run)
+        # Uploading the component
+        print_info('Uploading archive: %s' % archive)
+        job_id = client.upload_version(component_name=component_name, file_path=archive)
 
         # Wait for processing
         print_info(
             'Wait for processing, it is safe to press CTRL+C and exit\n'
             'You can check the state of processing by running CLI command '
             '"compote component upload-status --job=%s"' % job_id)
 
-        timeout_at = datetime.now() + timedelta(seconds=get_processing_timeout())
+        timeout_at = datetime.now() + timedelta(seconds=PROCESSING_TIMEOUT)
 
         try:
-            warnings = set()
             with ProgressBar(total=MAX_PROGRESS, unit='%') as progress_bar:
                 while True:
                     if datetime.now() > timeout_at:
                         raise TimeoutError()
                     status = client.task_status(job_id=job_id)
                     progress_bar.set_description(status.message)
                     progress_bar.update_to(status.progress)
 
-                    for warning in status.warnings:
-                        if warning not in warnings:
-                            print_warn(warning)
-                            warnings.add(warning)
-
                     if status.status == 'failure':
-                        if dry_run:
-                            raise FatalError(
-                                'Uploaded version did not pass validation successfully.\n%s' % status.message)
-                        else:
-                            raise FatalError("Uploaded version wasn't processed successfully.\n%s" % status.message)
+                        raise FatalError("Uploaded version wasn't processed successfully.\n%s" % status.message)
                     elif status.status == 'success':
                         return
 
                     time.sleep(CHECK_INTERVAL)
         except TimeoutError:
             raise FatalError(
-                "Component wasn't processed in {} seconds. Check processing status later.".format(
-                    get_processing_timeout()))
+                "Component wasn't processed in {} seconds. Check processing status later.".format(PROCESSING_TIMEOUT))
 
     @general_error_handler
     def upload_component_status(self, job_id, service_profile=None):  # type: (str, str | None) -> None
         client, _ = service_details(None, service_profile)
         status = client.task_status(job_id=job_id)
         if status.status == 'failure':
             raise FatalError("Uploaded version wasn't processed successfully.\n%s" % status.message)
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager/core_utils.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/core_utils.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/dependencies.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/dependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,49 +75,42 @@
     # type: (ProjectRequirements, SolvedManifest) -> bool
 
     if not solution.manifest_hash:
         print_info('Dependencies lock doesn\'t exist, solving dependencies.')
         return True
 
     if project_requirements.manifest_hash != solution.manifest_hash:
-        print_info('Manifest files have changed, solving dependencies.')
+        print_info('Manifest hash changed, solving dependencies.')
         return True
 
     if solution.target and project_requirements.target != solution.target:
         print_info(
             'Target changed from {} to {}, solving dependencies.'.format(solution.target, project_requirements.target))
         return True
 
     for component in solution.dependencies:
-        try:
-            # For downloadable volatile dependencies, like ones from git, if manifest didn't change, no need to solve
-            if component.source.downloadable and component.source.volatile:
-                continue
+        # Handle meta components, like ESP-IDF
+        if not component.source.meta:
+            continue
 
+        try:
             component_version = component.source.versions(component.name).versions[0]  # type: HashedComponentVersion
 
-            # Handle meta components, like ESP-IDF, and volatile components, like local
-            if component.source.meta or component.source.volatile:
-                if component_version != component.version:
-                    print_info(
-                        'Dependency "{}" version has changed from {} to {}, solving dependencies.'.format(
-                            component, component.version, component_version))
-                    return True
+            if component_version != component.version:
+                print_info(
+                    'Dependency "{}" version changed from {} to {}, solving dependencies.'.format(
+                        component, component.version, component_version))
+                return True
 
-            # Should check for all types of source, but after version checking
             if component_version.component_hash != component.component_hash:
-                if component.source.volatile:
-                    print_info('Dependency "{}" has changed, solving dependencies.'.format(component))
-                    return True
-                else:
-                    raise InvalidComponentHashError(
-                        'The hash sum of the component "{}" does not match the one recorded in your dependencies.lock '
-                        'file. This could be due to a potential spoofing of the download server, or your lock file may '
-                        'have become corrupted. Please review the lock file and verify the download server\'s '
-                        'authenticity to ensure the component\'s security and integrity.'.format(component))
+                raise InvalidComponentHashError(
+                    'The hash sum of the component "{}" does not match the one recorded in your dependencies.lock '
+                    'file. This could be due to a potential spoofing of the download server, or your lock file may '
+                    'have become corrupted. Please review the lock file and verify the download server\'s '
+                    'authenticity to ensure the component\'s security and integrity.'.format(component))
 
         except IndexError:
             print_info('Dependency "{}" version changed, solving dependencies.'.format(component))
             return True
 
     return False
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager/idf_extensions.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/idf_extensions.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     from typing import Any, Dict, List
 except ImportError:
     pass
 
 SERVICE_PROFILE = [
     {
         'names': ['--service-profile'],
-        'help': 'Profile for the component registry to use. By default profile named "default" will be used.',
+        'help': 'Profile for component registry to use. By default profile named "default" will be used.',
         'envvar': 'IDF_COMPONENT_SERVICE_PROFILE',
     },
 ]  # type: List[Dict[str, Any]]
 
 NAMESPACE = [
     {
         'names': ['--namespace'],
-        'help': 'Namespace for the component. Can be set in the config file.',
+        'help': 'Namespace for the component. Can be set in config file.',
         'envvar': 'IDF_COMPONENT_NAMESPACE',
     },
 ]  # type: List[Dict[str, Any]]
 
 NAME = [
     {
         'names': ['--name'],
@@ -41,19 +41,15 @@
 SERVICE_OPTIONS = SERVICE_PROFILE + NAMESPACE + NAME
 
 LOCAL_MANIFEST_OPTIONS = [
     {
         'names': ['--component'],
         'default': 'main',
         'help': 'Name of the component in the project.',
-    }, {
-        'names': ['-p', '--path'],
-        'help': 'Path to the component. The component name is ignored when path the is specified.',
-        'default': None
-    }
+    },
 ]  # type: list[dict[str, Any]]
 
 if CLICK_SUPPORTS_SHOW_DEFAULT:
     LOCAL_MANIFEST_OPTIONS[0]['show_default'] = True
 
 VERSION_PARAMETER = [
     {
@@ -103,41 +99,29 @@
                 tasks.insert(index + 1, reconfigure)
 
     return {
         'global_action_callbacks': [global_callback],
         'actions': {
             'create-manifest': {
                 'callback': callback,
-                'help': (
-                    'Create manifest for specified component.\n'
-                    'By default:\n'
-                    'If you run the command in the directory with project, the manifest'
-                    ' will be created in the "main" directory.\n'
-                    'If you run the command in the directory with a component, '
-                    'the manifest will be created right in that directory.\n'
-                    'You can explicitly specify directory using the --path option.'),
+                'help': 'Create manifest for specified component.',
                 'options': LOCAL_MANIFEST_OPTIONS,
             },
             'add-dependency': {
                 'callback': callback,
                 'help': (
-                    'Add dependency to the manifest file.\n'
-                    'By default:\n'
-                    'If you run the command in the directory with project, the dependency'
-                    ' will be added to the manifest in the "main" directory.\n'
-                    'If you run the command in the directory with a component, '
-                    'the dependency will be added to the manifest right in that directory.\n'
-                    'You can explicitly specify directory using the --path option.'),
+                    'Add dependency to the manifest file. '
+                    'For now we only support adding dependencies from the component registry.'),
                 'arguments': [
                     {
                         'names': ['dependency'],
                         'required': True,
                     },
                 ],
-                'options': LOCAL_MANIFEST_OPTIONS + SERVICE_PROFILE,
+                'options': LOCAL_MANIFEST_OPTIONS,
             },
             'remove_managed_components': {
                 'callback': callback,
                 'hidden': True
             },
             'upload-component': {
                 'callback': callback,
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager/local_component_list.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/local_component_list.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/prepare_components/prepare.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/prepare.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/service_details.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/service_details.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/templates/idf_component_template.yml` & `idf_component_manager-1.3.0.dev0/idf_component_manager/templates/idf_component_template.yml`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/utils.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/utils.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/helper.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/helper.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/assignment.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/assignment.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/constraint.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/constraint.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/failure.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/failure.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/incompatibility.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/incompatibility.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/incompatibility_cause.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/incompatibility_cause.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/package.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/package.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/package_source.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/package_source.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/partial_solution.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/partial_solution.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/range.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/range.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/result.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/result.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/term.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/term.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/union.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/union.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/mixology/version_solver.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/version_solver.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_manager/version_solver/version_solver.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/version_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                             req,
                             self._local_root_requirements[req.name],
                         ))
                     _req = self._local_root_requirements[req.name]
                 else:
                     _req = req
 
-                deps[Package(_req.name, _req.source)] = _req.source.normalize_spec(_req.version_spec)
+                deps[Package(_req.name, _req.source)] = _req.version_spec
 
             self._source.add(
                 Package(requirement.name, requirement.source),
                 version,
                 deps=deps,
             )
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager.egg-info/PKG-INFO` & `idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-component-manager
-Version: 1.3.0
+Version: 1.3.0.dev0
 Summary: The component manager for ESP-IDF
 Home-page: https://github.com/espressif/idf-component-manager
 Author: Sergei Silnov
 Author-email: sergei.silnov@espressif.com
 Maintainer: Sergei Silnov
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,36 @@
 
 # IDF Component Manager
 
 The IDF Component manager is a tool that downloads dependencies for any [ESP-IDF](https://www.espressif.com/en/products/sdks/esp-idf) CMake project. It makes sure that the right versions of all components required for a successful build of your project are in place. The download happens automatically during a run of CMake. It can source components either from [the component registry](https://components.espressif.com/) or from a git repository.
 
 **A list of components can be found at https://components.espressif.com/**
 
-## [Official documentation](https://docs.espressif.com/projects/idf-component-manager/en/latest/)
+## Installing the IDF Component Manager
+
+IDF component manager can be used with ESP-IDF v4.1 and later.
+It is installed by default with ESP-IDF v4.4+ and recent bug-fix releases of ESP-IDF 4.1+.
+
+To check the installed version of the IDF component manager, first, activate [ESP-IDF environment](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html#installation). On macOS and Linux:
+
+```bash
+source $IDF_PATH/export.sh
+```
+
+Then run the command:
+
+```bash
+python -m idf_component_manager -h
+```
+
+To update to the most recent version:
+
+```bash
+pip install idf-component-manager --upgrade
+```
 
 ## Disabling the Component Manager
 
 The component manager can be explicitly disabled by setting `IDF_COMPONENT_MANAGER` environment variable to `0`.
 
 ## Using with a project
 
@@ -101,17 +122,31 @@
     version: "*"
     require: no # Download component but don't add it as a requirement
   namespace/pre_release_component:
     version: "*"
     pre_release: true # Allow downloading of pre-release versions
 ```
 
+## Environment variables in manifest
+
+You can use environment variables in values in `idf_component.yml` manifests. `$VAR` or `${VAR}` is replaced with the value of the `VAR` environment variable. If the environment variable is not defined, the component manager will raise an error.
+
+Variable name should be ASCII alphanumeric string (including underscores) and start with an underscore or ASCII letter. The first non-identifier character after the `$` terminates this placeholder specification. You can escape `$` with one more`$` character, i.e., `$$` is replaced with `$`.
+
+One possible use-case is providing authentication to git repositories accessed through HTTPS:
+
+```yaml
+dependencies:
+  my_component:
+    git: https://git:${ACCESS_TOKEN}@git.my_git.com/my_component.git
+```
+
 ## Component metadata caching
 
-By default, information about available versions of components not cached. If you make many requests to the registry from one machine, you can enable caching by setting `IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES` environment variable to the number of minutes to cache the data.
+By default information about available versions of components is cached for 5 minutes. You can adjust caching period by setting the duration in minutes to `IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES` environment variable or disable the cache entirely by setting it to 0.
 
 ## External links
 
 You can add links to the `idf_component.yml` file to the root of the manifest:
 
 ```yaml
 url: "https://example.com/homepage" # URL of the component homepage
@@ -122,15 +157,15 @@
 ```
 
 A link should be a correct HTTP(S) URL like `https://example.com/path` except the `repository` field,
 it is expected to be a valid [Git remote](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes) URL.
 
 ## Add examples to the component
 
-To add examples to your component, place them in the `examples` directory inside your component.
+To add examples to your component place them in the `examples` directory inside your component.
 Examples are discovered recursively in subdirectories at this path.
 A directory with `CMakeLists.txt` that registers a project is considered as an example.
 
 ## Custom example paths
 
 You can specify custom example paths for uploading them to the component registry.
 For that, add `examples` field to the root of the manifest:
@@ -145,25 +180,25 @@
 
 | Variable                                    | Default value (or example for required) | Required? | Description                                                                                     |
 | ------------------------------------------- | --------------------------------------- | --------- | ----------------------------------------------------------------------------------------------- |
 | IDF_COMPONENT_API_TOKEN                     |                                         | no        | API token to access the component registry                                                      |
 | IDF_COMPONENT_REGISTRY_URL                  | https://components.espressif.com/       | no        | URL of the default component registry                                                           |
 | IDF_COMPONENT_STORAGE_URL                   | https://components-file.espressif.com/  | no        | URL of the default file storage server                                                          |
 | IDF_COMPONENT_REGISTRY_PROFILE              | default                                 | no        | Profile in the config file to use for component registry                                        |
-| IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES  | 0                                       | no        | API Cache expiration time in minutes                                                            |
+| IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES  | 5                                       | no        | API Cache expiration time in minutes                                                            |
 | IDF_COMPONENT_CACHE_PATH                    | \* Depends on OS                        | no        | Cache directory for component manager                                                           |
 | COMPONENT_MANAGER_JOB_TIMEOUT               | 300                                     | no        | Timeout in seconds to wait for component processing                                             |
 | IDF_COMPONENT_OVERWRITE_MANAGED_COMPONENTS  | 0                                       | no        | Overwrite files in the managed_component directory, even if they have been modified by the user |
 | IGNORE_UNKNOWN_FILES_FOR_MANAGED_COMPONENTS | 0                                       | no        | Ignore unknown files in managed_components directory                                            |
 
 ## Contributions Guide
 
 We welcome all contributions to the Component Manager project.
 
-You can contribute by fixing bugs, adding features, adding documentation, or reporting an [issue](https://github.com/espressif/idf-component-manager/issues). We accept contributions via [GitHub Pull Requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
+You can contribute by fixing bugs, adding features, adding documentation, or reporting an [issue](https://github.com/espressif/idf-component-manager/issues). We accept contributions via [Github Pull Requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
 
 Before reporting an issue, make sure you've searched for a similar one that was already created. If you are reporting a new issue, please follow the Issue Template.
 
 ## Installing a development version of the component manager
 
 You can install the development version of the component manager from the main branch of this repository:
 
@@ -189,10 +224,9 @@
 python -m pip uninstall -y idf-component-manager
 # install the development version (from the main branch)
 python -m pip install git+https://github.com/espressif/idf-component-manager.git@main
 ```
 
 ## Resources
 
-- The Component manager [Documentation](https://docs.espressif.com/projects/idf-component-manager/en/latest/)
 - The Python Package Index project page https://pypi.org/project/idf-component-manager/
 - The Component Manager section in the [ESP-IDF Programming Guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-guides/tools/idf-component-manager.html)
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager.egg-info/SOURCES.txt` & `idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 idf_component_manager/cli/autocompletion.py
 idf_component_manager/cli/cache.py
 idf_component_manager/cli/component.py
 idf_component_manager/cli/constants.py
 idf_component_manager/cli/core.py
 idf_component_manager/cli/manifest.py
 idf_component_manager/cli/project.py
-idf_component_manager/cli/registry.py
 idf_component_manager/cli/utils.py
 idf_component_manager/prepare_components/__init__.py
 idf_component_manager/prepare_components/__main__.py
 idf_component_manager/prepare_components/prepare.py
 idf_component_manager/templates/idf_component_template.yml
 idf_component_manager/version_solver/__init__.py
 idf_component_manager/version_solver/helper.py
@@ -62,26 +61,23 @@
 idf_component_tools/constants.py
 idf_component_tools/environment.py
 idf_component_tools/errors.py
 idf_component_tools/file_cache.py
 idf_component_tools/file_tools.py
 idf_component_tools/git_client.py
 idf_component_tools/hash_tools.py
-idf_component_tools/network_tools.py
 idf_component_tools/serialization.py
 idf_component_tools/lock/__init__.py
 idf_component_tools/lock/manager.py
 idf_component_tools/manifest/__init__.py
 idf_component_tools/manifest/constants.py
 idf_component_tools/manifest/env_expander.py
 idf_component_tools/manifest/if_parser.py
 idf_component_tools/manifest/manager.py
 idf_component_tools/manifest/manifest.py
-idf_component_tools/manifest/metadata.py
-idf_component_tools/manifest/schemas.py
 idf_component_tools/manifest/solved_component.py
 idf_component_tools/manifest/solved_manifest.py
 idf_component_tools/manifest/validator.py
 idf_component_tools/semver/__init__.py
 idf_component_tools/semver/base.py
 idf_component_tools/sources/__init__.py
 idf_component_tools/sources/base.py
```

### Comparing `idf_component_manager-1.3.0/idf_component_manager.egg-info/requires.txt` & `idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+future
 packaging
 requests<3
-urllib3<2
 requests-file
 requests-toolbelt
 schema
 six
 tqdm<5
 
 [:python_version < "3"]
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/api_client.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 """Classes to work with Espressif Component Web Service"""
 import os
 import platform
-import re
 from collections import namedtuple
 from functools import wraps
 from io import open
 
 import requests
 from cachecontrol import CacheControlAdapter
 from cachecontrol.caches import FileCache
@@ -17,52 +16,52 @@
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 from schema import Schema, SchemaError
 from tqdm import tqdm
 
 # Import whole module to avoid circular dependencies
 import idf_component_tools as tools
 from idf_component_tools.__version__ import __version__
-from idf_component_tools.environment import getenv_int
 from idf_component_tools.errors import warn
 from idf_component_tools.file_cache import FileCache as ComponentFileCache
 from idf_component_tools.semver import SimpleSpec, Version
 
 from .api_client_errors import (
     KNOWN_API_ERRORS, APIClientError, ComponentNotFound, NetworkConnectionError, NoRegistrySet, StorageFileNotFound,
     VersionNotFound)
 from .api_schemas import (
-    API_INFORMATION_SCHEMA, API_TOKEN_SCHEMA, COMPONENT_SCHEMA, ERROR_SCHEMA, TASK_STATUS_SCHEMA, VERSION_UPLOAD_SCHEMA)
-from .manifest import BUILD_METADATA_KEYS, Manifest
+    API_INFORMATION_SCHEMA, COMPONENT_SCHEMA, ERROR_SCHEMA, TASK_STATUS_SCHEMA, VERSION_UPLOAD_SCHEMA)
+from .manifest import Manifest
 
 try:
     from typing import TYPE_CHECKING, Any, Callable
 
     if TYPE_CHECKING:
         from idf_component_tools.sources import BaseSource
 except ImportError:
     pass
 
-TaskStatus = namedtuple('TaskStatus', ['message', 'status', 'progress', 'warnings'])
+TaskStatus = namedtuple('TaskStatus', ['message', 'status', 'progress'])
 
 DEFAULT_TIMEOUT = (
     6.05,  # Connect timeout
     30.1,  # Read timeout
 )
 
-DEFAULT_API_CACHE_EXPIRATION_MINUTES = 0
+DEFAULT_API_CACHE_EXPIRATION_MINUTES = 5
 MAX_RETRIES = 3
 
 
 def env_cache_time():
     try:
-        return getenv_int('IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES', DEFAULT_API_CACHE_EXPIRATION_MINUTES)
+        return int(os.environ.get('IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES', DEFAULT_API_CACHE_EXPIRATION_MINUTES))
     except ValueError:
         warn(
             'IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES is set to a non-numeric value. '
-            'Please set the variable to the number of minutes. Disabling caching.')
+            'Please set the variable to the number of minutes. '
+            'Using the default value of {} minutes.'.format(DEFAULT_API_CACHE_EXPIRATION_MINUTES))
         return DEFAULT_API_CACHE_EXPIRATION_MINUTES
 
 
 def create_session(
         cache=False,  # type: bool
         cache_path=None,  # type: str | None
         cache_time=None,  # type: int | None
@@ -88,39 +87,14 @@
     session.mount('http://', api_adapter)
     session.mount('https://', api_adapter)
     session.mount('file://', FileAdapter())
 
     return session
 
 
-def filter_versions(versions, version_filter, component_name):  # type: (list[dict], str, str) -> list[dict]
-    if version_filter and version_filter != '*':
-        requested_version = SimpleSpec(str(version_filter))
-        filtered_versions = [v for v in versions if requested_version.match(Version(v['version']))]
-
-        if not filtered_versions or not any([bool(v.get('yanked_at')) for v in filtered_versions]):
-            return filtered_versions
-
-        clause = requested_version.clause.simplify()
-        # Some clauses don't have an operator attribute, need to check
-        if hasattr(clause, 'operator') and clause.operator == '==' and filtered_versions[0]['yanked_at']:
-            warn(
-                'The version "{}" of the "{}" component you have selected has been yanked from the repository '
-                'due to the following reason: "{}". We recommend that you update to a different version. '
-                'Please note that continuing to use a yanked version can result in unexpected behavior and '
-                'issues with your project.'.format(
-                    clause.target, component_name.lower(), filtered_versions[0]['yanked_message']))
-        else:
-            filtered_versions = [v for v in filtered_versions if not v.get('yanked_at')]
-    else:
-        filtered_versions = [v for v in versions if not v.get('yanked_at')]
-
-    return filtered_versions
-
-
 class ComponentDetails(Manifest):
     def __init__(
             self,
             download_url=None,  # type: str | None # Direct url for tarball download
             documents=None,  # type: list[dict[str, str]] | None # List of documents of the component
             license=None,  # type: dict[str, str] | None # Information about license
             examples=None,  # type: list[dict[str, str]] | None # List of examples of the component
@@ -185,32 +159,19 @@
         os=platform.system(),
         release=platform.release(),
         arch=platform.machine(),
         py_version=platform.python_version(),
     )
 
 
-def _component_request(request, component_name):
-    """Get component information from storage. Used by `versions` and `component`."""
-    try:
-        return request(
-            'get',
-            ['components', component_name.lower()],
-            schema=COMPONENT_SCHEMA,
-        )
-    except StorageFileNotFound:
-        raise ComponentNotFound('Component "{}" not found'.format(component_name))
-
-
 class APIClient(object):
     def __init__(self, base_url=None, storage_url=None, source=None, auth_token=None):
         # type: (str | None, str | None, BaseSource | None, str | None) -> None
         self.base_url = base_url
         self._storage_url = storage_url
-        self._frontend_url = None
         self.source = source
         self.auth_token = auth_token
 
     def _version_dependencies(self, version):
         dependencies = []
         for dependency in version.get('dependencies', []):
             # Support only idf and service sources
@@ -232,15 +193,14 @@
     def _base_request(
             self,
             url,  # type: str
             session,  # type: requests.Session
             method,  # type: str
             path,  # type: list[str]
             data=None,  # type: dict | None
-            json=None,  # type: dict | None
             headers=None,  # type: dict | None
             schema=None,  # type: Schema | None
             use_storage=False,  # type: bool
     ):
         # type: (...) -> dict
         endpoint = join_url(url, *path)
 
@@ -253,15 +213,14 @@
             pass
 
         try:
             response = session.request(
                 method,
                 endpoint,
                 data=data,
-                json=json,
                 headers=headers,
                 timeout=timeout,
                 allow_redirects=True,
             )
 
             if response.status_code == 204:  # NO CONTENT
                 return {}
@@ -274,44 +233,37 @@
                 handle_4xx_error(response)
 
             elif 500 <= response.status_code < 600:
                 raise APIClientError(
                     'Internal server error happended while processing requrest to:\n{}\nStatus code: {}'.format(
                         endpoint, response.status_code))
 
-            response_json = response.json()
+            json = response.json()
         except requests.exceptions.ConnectionError as e:
             raise NetworkConnectionError(str(e))
         except requests.exceptions.RequestException:
             raise APIClientError('HTTP request error')
 
         try:
             if schema is not None:
-                schema.validate(response_json)
+                schema.validate(json)
         except SchemaError as e:
             raise APIClientError('API Endpoint "{}: returned unexpected JSON:\n{}'.format(endpoint, str(e)))
 
         except (ValueError, KeyError, IndexError):
             raise APIClientError('Unexpected component server response')
 
-        return response_json
+        return json
 
     @property
     def storage_url(self):
         if not self._storage_url:
             self._storage_url = self.api_information()['components_base_url']
         return self._storage_url
 
-    @property
-    def frontend_url(self):
-        if not self._frontend_url:
-            self._frontend_url = re.sub(r'/api/?$', '', self.base_url)
-
-        return self._frontend_url
-
     def _request(cache=False, use_storage=False):  # type: (APIClient | bool, bool) -> Callable
         def decorator(f):  # type: (Callable[..., Any]) -> Callable
             @wraps(f)  # type: ignore
             def wrapper(self, *args, **kwargs):
                 url = self.base_url
                 if use_storage:
                     url = self.storage_url
@@ -323,27 +275,19 @@
                         'IDF_COMPONENT_REGISTRY_URL environment variable or "registry_url" field for your current '
                         'profile in "idf_component_manager.yml" file. To use the default IDF component registry '
                         'unset IDF_COMPONENT_STORAGE_URL environment variable or remove "storage_url" field '
                         'from the "idf_component_manager.yml" file')
 
                 session = create_session(cache=cache, token=self.auth_token)
 
-                def request(method, path, data=None, json=None, headers=None, schema=None):
+                def request(method, path, data=None, headers=None, schema=None):
                     if use_storage:
                         path[-1] += '.json'
                     return self._base_request(
-                        url,
-                        session,
-                        method,
-                        path,
-                        data=data,
-                        json=json,
-                        headers=headers,
-                        schema=schema,
-                        use_storage=use_storage)
+                        url, session, method, path, data=data, headers=headers, schema=schema, use_storage=use_storage)
 
                 return f(self, request=request, *args, **kwargs)
 
             return wrapper
 
         return decorator
 
@@ -351,66 +295,60 @@
     def api_information(self, request):
         return request(
             'get',
             [],
             schema=API_INFORMATION_SCHEMA,
         )
 
-    @auth_required
-    @_request(cache=False)
-    def token_information(self, request):
-        return request(
-            'get',
-            ['tokens', 'current'],
-            schema=API_TOKEN_SCHEMA,
-        )
-
     @_request(cache=True, use_storage=True)
     def versions(self, request, component_name, spec='*'):
         """List of versions for given component with required spec"""
-
-        component_name = component_name.lower()
         semantic_spec = SimpleSpec(spec or '*')
-        body = _component_request(request, component_name)
-
-        versions = []
-        for version in body['versions']:
-            if not semantic_spec.match(Version(version['version'])):
-                continue
-
-            all_build_keys_known = True
-            if version.get('build_metadata_keys', None) is not None:
-                for build_key in version.get('build_metadata_keys'):
-                    if build_key not in BUILD_METADATA_KEYS:
-                        all_build_keys_known = False
-                        break
-
-            if all_build_keys_known:
-                versions.append((version, all_build_keys_known))
+        component_name = component_name.lower()
+        try:
+            body = request(
+                'get',
+                ['components', component_name],
+                schema=COMPONENT_SCHEMA,
+            )
+        except (ComponentNotFound, StorageFileNotFound):
+            versions = []
+        else:
+            versions = []
+            for version in body['versions']:
+                if semantic_spec.match(Version(version['version'])):
+                    versions.append(version)
 
         return tools.manifest.ComponentWithVersions(
             name=component_name,
             versions=[
                 tools.manifest.HashedComponentVersion(
                     version_string=version['version'],
                     component_hash=version['component_hash'],
                     dependencies=self._version_dependencies(version),
                     targets=version['targets'],
-                    all_build_keys_known=all_build_keys_known) for version, all_build_keys_known in versions
+                ) for version in versions
             ],
         )
 
     @_request(cache=True, use_storage=True)
     def component(self, request, component_name, version=None):
         """Manifest for given version of component, if version is None highest version is returned"""
-
-        component_name = component_name.lower()
-        response = _component_request(request, component_name)
+        response = request(
+            'get',
+            ['components', component_name.lower()],
+            schema=COMPONENT_SCHEMA,
+        )
         versions = response['versions']
-        filtered_versions = filter_versions(versions, version, component_name)
+
+        if version and version != '*':
+            requested_version = SimpleSpec(str(version))
+            filtered_versions = [v for v in versions if requested_version.match(Version(v['version']))]
+        else:
+            filtered_versions = versions
 
         if not filtered_versions:
             raise VersionNotFound(
                 'Version of the component "{}" satisfying the spec "{}" was not found.'.format(
                     component_name, str(version)))
 
         best_version = max(filtered_versions, key=lambda v: Version(v['version']))
@@ -436,53 +374,42 @@
             download_url=download_url,
             documents=documents,
             license=license_info,
             examples=examples)
 
     @auth_required
     @_request(cache=False)
-    def upload_version(self, request, component_name, file_path, validate_only=False):
+    def upload_version(self, request, component_name, file_path):
         with open(file_path, 'rb') as file:
             filename = os.path.basename(file_path)
 
             encoder = MultipartEncoder({'file': (filename, file, 'application/octet-stream')})
             headers = {'Content-Type': encoder.content_type}
 
             progress_bar = tqdm(total=encoder.len, unit_scale=True, unit='B', disable=None)
 
             def callback(monitor, memo={'progress': 0}):  # type: (MultipartEncoderMonitor, dict) -> None
                 progress_bar.update(monitor.bytes_read - memo['progress'])
                 memo['progress'] = monitor.bytes_read
 
             data = MultipartEncoderMonitor(encoder, callback)
 
-            if validate_only:
-                endpoint = ['components', 'validate']
-            else:
-                endpoint = ['components', component_name.lower(), 'versions']
-
             try:
                 return request(
                     'post',
-                    endpoint,
+                    ['components', component_name.lower(), 'versions'],
                     data=data,
                     headers=headers,
                     schema=VERSION_UPLOAD_SCHEMA,
                 )['job_id']
             finally:
                 progress_bar.close()
 
     @auth_required
     @_request(cache=False)
     def delete_version(self, request, component_name, component_version):
         request('delete', ['components', component_name.lower(), component_version])
 
-    @auth_required
-    @_request(cache=False)
-    def yank_version(self, request, component_name, component_version, yank_message):
-        request(
-            'post', ['components', component_name.lower(), component_version, 'yank'], json={'message': yank_message})
-
     @_request(cache=False)
     def task_status(self, request, job_id):  # type: (Callable, str) -> TaskStatus
         body = request('get', ['tasks', job_id], schema=TASK_STATUS_SCHEMA)
-        return TaskStatus(body['message'], body['status'], body['progress'], body.get('warnings', []))
+        return TaskStatus(body['message'], body['status'], body['progress'])
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/api_client_errors.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/api_client_errors.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/api_schemas.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/api_schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 from schema import Optional, Or, Schema, Use
 from six import string_types
 
 STRING = Or(*string_types)
 OPTIONAL_STRING = Or(None, *string_types)
@@ -45,15 +45,15 @@
 )
 
 VERSION_UPLOAD_SCHEMA = Schema(
     {
         'job_id': STRING,
         Optional(STRING): object,
     },
-    error='Unexpected response during archive processing',
+    error='Unexpected response to version upload',
 )
 
 TASK_STATUS_SCHEMA = Schema(
     {
         'id': STRING,
         'status': STRING,
         Optional('message'): OPTIONAL_STRING,
@@ -66,19 +66,7 @@
         'components_base_url': STRING,
         'info': STRING,
         'status': STRING,
         'version': STRING
     },
     error='Unexpected response to API information',
 )
-
-API_TOKEN_SCHEMA = Schema(
-    {
-        'id': STRING,
-        'scope': STRING,
-        'created_at': OPTIONAL_STRING,
-        'expires_at': OPTIONAL_STRING,
-        'description': OPTIONAL_STRING,
-        'access_token_prefix': STRING,
-    },
-    error='Unexpected response to current token information',
-)
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/archive_tools.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/archive_tools.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/config.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,78 +10,55 @@
 from six import string_types
 
 from idf_component_tools.constants import COMPILED_URL_RE
 from idf_component_tools.errors import FatalError, UserDeprecationWarning
 
 from .constants import IDF_COMPONENT_REGISTRY_URL, IDF_COMPONENT_STORAGE_URL
 
-try:
-    from typing import Any, Iterator
-except ImportError:
-    pass
-
 DEFAULT_CONFIG_DIR = os.path.join('~', '.espressif')
+CONFIG_DIR = os.environ.get('IDF_TOOLS_PATH') or os.path.expanduser(DEFAULT_CONFIG_DIR)
 
 CONFIG_SCHEMA = Schema(
     {
         Optional('profiles'): {
             Or(*string_types): {
                 Optional('registry_url'): Or('default', Regex(COMPILED_URL_RE)),
                 Optional('default_namespace'): And(Or(*string_types), len),
                 Optional('api_token'): And(Or(*string_types), len)
             }
         }
     })
 
 
-def config_dir():
-    return os.environ.get('IDF_TOOLS_PATH') or os.path.expanduser(DEFAULT_CONFIG_DIR)
-
-
 class ConfigError(FatalError):
     pass
 
 
 class Config(object):
-    def __init__(self, config=None):  # type: (dict | None) -> None
+    def __init__(self, config=None):
         self._config = config or {}
 
-    def __getitem__(self, key):  # type: (Any) -> Any
-        return self._config[key]
-
-    def __setitem__(self, key, value):  # type: (Any, Any) -> None
-        self._config[key] = value
-
-    def __delitem__(self, key):  # type: (Any) -> None
-        del self._config[key]
-
-    def __len__(self):  # type: () -> int
-        return len(self._config)
-
-    def __iter__(self):  # type: () -> Iterator[Any]
+    def __iter__(self):
         return iter(self._config.items())
 
-    def __contains__(self, item):  # type: (Any) -> bool
-        return item in self._config
-
     @property
-    def profiles(self):  # type: () -> dict
+    def profiles(self):
         return self._config.setdefault('profiles', {})
 
-    def validate(self):  # type: () -> Config
+    def validate(self):
         try:
             self._config = CONFIG_SCHEMA.validate(self._config)
             return self
         except SchemaError as e:
             raise ConfigError('Config format is not valid:\n%s' % str(e))
 
 
 class ConfigManager(object):
     def __init__(self, path=None):
-        self.config_path = path or os.path.join(config_dir(), 'idf_component_manager.yml')
+        self.config_path = path or os.path.join(CONFIG_DIR, 'idf_component_manager.yml')
 
     def load(self):  # type: () -> Config
         """Loads config from disk"""
         if not os.path.isfile(self.config_path):
             return Config({})
 
         with open(self.config_path, mode='r', encoding='utf-8') as f:
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/constants.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 #
 # Contains elements taken from "is-git-url" github repository
 # https://github.com/jonschlinkert/is-git-url
 # Copyright (c) 2017, Jon Schlinkert.
 # Originally released under the MIT License.
 
 import re
-import sys
 
 URL_RE = (
     r'^https?://'  # http:// or https://
     # here use A-Za-z even with re.IGNORECASE is because json schema does not support flags
     r'(?:(?:[A-Za-z0-9](?:[A-Za-z0-9-]{0,61}[A-Za-z0-9])?\.)+(?:[A-Za-z]{2,6}\.?|[A-Za-z0-9-]{2,}\.?)|'  # domain
     r'localhost|'  # or localhost
     r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'  # or ip
@@ -22,12 +21,7 @@
 GIT_URL_RE = r'^(?:git|ssh|https?|git@[-\w.]+):(\/\/)?(.*)(\.git)?(/?|#[-\d\w._]+?)$'
 COMPILED_GIT_URL_RE = re.compile(GIT_URL_RE, re.IGNORECASE)
 
 # Registry related constants
 DEFAULT_NAMESPACE = 'espressif'
 IDF_COMPONENT_REGISTRY_URL = 'https://components.espressif.com/'
 IDF_COMPONENT_STORAGE_URL = 'https://components-file.espressif.com/'
-
-UPDATE_SUGGESTION = """SUGGESTION: This component may be using a newer version of the component manager.
-You can try to update the component manager by running:
-    {} -m pip install --upgrade idf-component-manager
-""".format(sys.executable)
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/environment.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/environment.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/file_cache.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/file_cache.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/file_tools.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/file_tools.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/git_client.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/git_client.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/hash_tools.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/hash_tools.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/lock/manager.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/lock/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from yaml import dump as dump_yaml
 from yaml import safe_load
 
 import idf_component_tools as tools
 
 from ..build_system_tools import get_env_idf_target, get_idf_version
 from ..errors import LockError
-from ..manifest import ComponentVersion, SolvedComponent, SolvedManifest, known_targets
+from ..manifest import ComponentVersion, SolvedComponent, SolvedManifest
+from ..manifest.validator import known_targets
 from ..sources import IDFSource
 
 FORMAT_VERSION = '1.0.0'
 
 EMPTY_LOCK = {
     'manifest_hash': None,
     'version': FORMAT_VERSION,
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/manifest/__init__.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
-from .constants import FULL_SLUG_REGEX, MANIFEST_FILENAME, SLUG_REGEX, WEB_DEPENDENCY_REGEX, known_targets
+from .constants import FULL_SLUG_REGEX, MANIFEST_FILENAME, SLUG_REGEX, WEB_DEPENDENCY_REGEX
 from .manager import ManifestManager
 from .manifest import (
     ComponentRequirement, ComponentVersion, ComponentWithVersions, HashedComponentVersion, Manifest,
     ProjectRequirements)
-from .schemas import BUILD_METADATA_KEYS, INFO_METADATA_KEYS, JSON_SCHEMA
 from .solved_component import SolvedComponent
 from .solved_manifest import SolvedManifest
 from .validator import ManifestValidator
 
 __all__ = [
     'ComponentRequirement',
     'ComponentVersion',
@@ -22,12 +21,8 @@
     'ManifestManager',
     'ManifestValidator',
     'ProjectRequirements',
     'SLUG_REGEX',
     'SolvedComponent',
     'SolvedManifest',
     'WEB_DEPENDENCY_REGEX',
-    'JSON_SCHEMA',
-    'BUILD_METADATA_KEYS',
-    'INFO_METADATA_KEYS',
-    'known_targets',
 ]
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/manifest/env_expander.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/env_expander.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/manifest/if_parser.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/if_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,35 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
+
+import inspect
 import re
 from ast import literal_eval
 
 from schema import SchemaError
 
 from idf_component_tools.build_system_tools import get_env_idf_target, get_idf_version
-from idf_component_tools.errors import FetchingError, ProcessingError
 from idf_component_tools.manifest.constants import IF_IDF_VERSION_REGEX, IF_TARGET_REGEX
 from idf_component_tools.semver import SimpleSpec, Version
 from idf_component_tools.serialization import serializable
 
 IF_IDF_VERSION_REGEX_COMPILED = re.compile(IF_IDF_VERSION_REGEX)
 IF_TARGET_REGEX_COMPILED = re.compile(IF_TARGET_REGEX)
 
+COMMON_ERR_MSG = inspect.cleandoc(
+    """
+Invalid if clause. Here are some valid examples:
+    For keyword "idf_version", you could use:
+        - if: "idf_version ~= 5.0.0"
+        - if: "idf_version >=3.3,<5.0"
+    For keyword "target", you could use:
+        - if: "target not in [esp32, esp32c3]"
+        - if: "target != esp32"
+""")
+
 
 @serializable
 class IfClause:
     _serialization_properties = [
         'clause',
         'bool_value',
     ]
@@ -50,91 +62,68 @@
     _s = s.strip()
     if not (_s[0] == _s[-1] == '"'):
         _s = '"{}"'.format(_s.replace('"', r'\"'))
 
     try:
         return literal_eval(_s)
     except (ValueError, SyntaxError):
-        raise SchemaError(None, 'Invalid string "{}" in "if" clause'.format(s))
+        raise SchemaError(None, ['Invalid string `{}`'.format(s), COMMON_ERR_MSG])
 
 
 def _eval_list(s):  # type: (str) -> list[str]
     _s = s.strip()
 
     if _s[0] == '[' and _s[-1] == ']':
         _s = _s[1:-1]
 
     try:
         return [_eval_str(part) for part in _s.split(',')]
     except (ValueError, SyntaxError):
-        raise SchemaError(None, 'Invalid list "{}" in "if" clause'.format(s))
+        raise SchemaError(None, ['Invalid list `{}`'.format(s), COMMON_ERR_MSG])
 
 
 def _parse_if_idf_version_clause(mat):  # type: (re.Match) -> IfClause
     comparison = mat.group('comparison')
     spec = mat.group('spec')
     spec = ','.join([part.strip() for part in spec.split(',')])
 
     try:
         simple_spec = SimpleSpec('{}{}'.format(_eval_str(comparison), _eval_str(spec)))
-    except ValueError:
-        raise SchemaError(
-            None, 'Invalid version specification for "idf_version": {clause}. Please use a format like '
-            '"idf_version >=4.4,<5.3"\nDocumentation: '
-            'https://docs.espressif.com/projects/idf-component-manager/en/latest/reference/manifest_file.html#rules'.
-            format(clause=mat.string))
-
-    try:
-        idf_version = get_idf_version()
-    except FetchingError:
-        idf_version = None
-        bool_value = False
-    else:
-        bool_value = simple_spec.match(Version(idf_version))
+    except ValueError as e:
+        raise SchemaError(None, [str(e), COMMON_ERR_MSG])
 
-    return IfClause('{} {}'.format(idf_version, simple_spec.expression), bool_value)
+    idf_version = get_idf_version()
+    return IfClause('{} {}'.format(idf_version, simple_spec.expression), simple_spec.match(Version(idf_version)))
 
 
 def _parser_if_target_clause(mat):  # type: (re.Match) -> IfClause
     comparison = mat.group('comparison')
-    targets = mat.group('targets').strip()
+    versions = mat.group('versions').strip()
 
-    try:
-        env_target = get_env_idf_target()
-    except ProcessingError:
-        env_target = None
-        bool_value = False
+    env_target = get_env_idf_target()
+    if comparison == '!=':
+        bool_value = env_target != _eval_str(versions)
+    elif comparison == '==':
+        bool_value = env_target == _eval_str(versions)
+    elif comparison == 'not in':
+        bool_value = env_target not in _eval_list(versions)
+    elif comparison == 'in':
+        bool_value = env_target in _eval_list(versions)
     else:
-        if comparison == '!=':
-            bool_value = env_target != _eval_str(targets)
-        elif comparison == '==':
-            bool_value = env_target == _eval_str(targets)
-        elif comparison == 'not in':
-            bool_value = env_target not in _eval_list(targets)
-        elif comparison == 'in':
-            bool_value = env_target in _eval_list(targets)
-        else:
-            raise SchemaError(
-                None, 'Invalid if clause format for target: {clause}. You can specify rules based on target using '
-                '"==", "!=", "in" or "not in" like: "target in [esp32, esp32c3]", "target == esp32"\n'
-                'Documentation: '
-                'https://docs.espressif.com/projects/idf-component-manager/en/latest/reference'
-                '/manifest_file.html#rules'.format(clause=mat.string))
+        raise SchemaError(None, COMMON_ERR_MSG)
 
-    return IfClause('{} {} {}'.format(env_target, comparison, targets), bool_value)
+    return IfClause('{} {} {}'.format(env_target, comparison, versions), bool_value)
 
 
 def parse_if_clause(if_clause):  # type: (str) -> IfClause
+    is_idf_version = True
     res = IF_IDF_VERSION_REGEX_COMPILED.match(if_clause)
-    if res:
-        return _parse_if_idf_version_clause(res)
+    if not res:
+        is_idf_version = False
+        res = IF_TARGET_REGEX_COMPILED.match(if_clause)
+    if not res:
+        raise SchemaError(None, COMMON_ERR_MSG)
 
-    res = IF_TARGET_REGEX_COMPILED.match(if_clause)
-    if res:
+    if is_idf_version:
+        return _parse_if_idf_version_clause(res)
+    else:
         return _parser_if_target_clause(res)
-
-    raise SchemaError(
-        None,
-        'Invalid if clause format "{clause}". You can specify rules based on current ESP-IDF version or target like: '
-        '"idf_version >=3.3,<5.0" or "target in [esp32, esp32c3]"\nDocumentation: '
-        'https://docs.espressif.com/projects/idf-component-manager/en/latest/reference/manifest_file.html#rules'.format(
-            clause=if_clause))
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/manifest/manager.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
-import copy
 import os
+import sys
 from io import open
 
 import yaml
 
-from ..constants import UPDATE_SUGGESTION
-from ..errors import ManifestError, MetadataError
+from ..errors import ManifestError
 from .constants import MANIFEST_FILENAME
 from .env_expander import dump_yaml, expand_env_vars
 from .manifest import Manifest
-from .metadata import Metadata
 from .validator import ManifestValidator
 
 try:
     from typing import Any, Dict, List, Optional
 except ImportError:
     pass
 
 EMPTY_MANIFEST = dict()  # type: Dict[str, Any]
 
+UPDATE_SUGGESTION = """
+SUGGESTION: This component may be using a newer version of the component manager.
+You can try to update the component manager by running:
+    {} -m pip install --upgrade idf-component-manager
+""".format(sys.executable)
+
 
 def dump_tree(path, manifest_tree):  # type: (str, dict) -> None
     if os.path.isdir(path):
         path = os.path.join(path, MANIFEST_FILENAME)
 
     dump_yaml(manifest_tree, path)
 
@@ -43,43 +47,34 @@
         self._normalized_manifest_tree = None  # type: Optional[Dict]
         self._manifest = None
         self._is_valid = None
         self._validation_errors = []  # type: List[str]
         self.check_required_fields = check_required_fields
 
     def validate(self):
-        try:
-            metadata = Metadata.load(self.manifest_tree)
-        except MetadataError as e:
-            self._validation_errors = e.args
-        else:
-            validator = ManifestValidator(
-                self.manifest_tree,
-                check_required_fields=self.check_required_fields,
-                version=self.version,
-                metadata=metadata)
-            self._validation_errors = validator.validate_normalize()
-            self._is_valid = not self._validation_errors
-            self._normalized_manifest_tree = copy.deepcopy(validator.manifest_tree)
-
+        validator = ManifestValidator(
+            self.manifest_tree, check_required_fields=self.check_required_fields, version=self.version)
+        self._validation_errors = validator.validate_normalize()
+        self._is_valid = not self._validation_errors
+        self._normalized_manifest_tree = validator.manifest_tree
         return self
 
     @property
     def is_valid(self):
         if self._is_valid is None:
             self.validate()
 
         return self._is_valid
 
     @property
     def validation_errors(self):
         return self._validation_errors
 
     @property
-    def path(self):  # type: () -> str
+    def path(self):
         if self._path_checked:
             return self._path
 
         if os.path.isdir(self._path):
             self._path = os.path.join(self._path, MANIFEST_FILENAME)
             self._path_checked = True
 
@@ -140,16 +135,16 @@
 
             error_desc.append(UPDATE_SUGGESTION)
 
             raise ManifestError('\n'.join(error_desc))
 
         for name, details in self.normalized_manifest_tree.get('dependencies', {}).items():
             if 'rules' in details:
-                self.normalized_manifest_tree['dependencies'][name]['rules'] = [rule['if'] for rule in details['rules']]
+                self.manifest_tree['dependencies'][name]['rules'] = [rule['if'] for rule in details['rules']]
 
-        return Manifest.fromdict(self.normalized_manifest_tree, name=self.name, manifest_manager=self)
+        return Manifest.fromdict(self.manifest_tree, name=self.name, manifest_manager=self)
 
     def dump(self, path=None):  # type: (str | None) -> None
         if path is None:
             path = self.path
 
         dump_tree(path, self.manifest_tree)
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/manifest/manifest.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 except ImportError:
     from collections import Mapping  # type: ignore
 
 try:
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
-        from typing import Any
-
         from ..sources import BaseSource
         from . import ManifestManager
 except ImportError:
     pass
 
 # Ignore error with using variable in namedtuple
 ComponentLinks = namedtuple('ComponentLinks', LINKS)  # type: ignore
@@ -148,19 +146,18 @@
     @property
     def dependencies(self):  # type: () -> list[ComponentRequirement]
         return sorted(self._dependencies, key=lambda d: d.name)
 
     @property
     def manifest_hash(self):  # type: () -> str
         if self._manifest_hash:
-            return self._manifest_hash
+            return self.manifest_hash
 
         serialized = self.serialize(serialize_default=False)  # type: ignore
-        self._manifest_hash = hash_object(serialized)
-        return self._manifest_hash
+        return hash_object(serialized)
 
     @property
     def path(self):  # type: () -> str
         return self._manifest_manager.path if self._manifest_manager else ''
 
 
 @serializable
@@ -184,15 +181,15 @@
             source,  # type: BaseSource
             version_spec='*',  # type: str
             public=None,  # type: bool | None
             if_clauses=None,  # type: list[IfClause] | None
             require=None,  # type: str | bool | None
     ):
         # type: (...) -> None
-        self.version_spec = version_spec
+        self._version_spec = version_spec
         self.source = source
         self._name = name
         self.public = None  # type: bool | None
         if require == 'public' or public:
             self.public = True
         elif public is False or require == 'private':
             self.public = False
@@ -204,26 +201,34 @@
         return self.source.meta
 
     @property
     def name(self):
         return self.source.normalized_name(self._name)
 
     @property
+    def version_spec(self):
+        return self.source.normalize_spec(self._version_spec)
+
+    @property
     def meet_optional_dependencies(self):
         if not self.if_clauses:
             return True
 
         return all(if_clause.bool_value for if_clause in self.if_clauses)
 
     def __repr__(self):  # type: () -> str
         return 'ComponentRequirement("{}", {}, version_spec="{}", public={})'.format(
             self._name, self.source, self.version_spec, self.public)
 
     def __str__(self):  # type: () -> str
-        return '{}({})'.format(self._name, self.version_spec)
+        # if local source, avoid circular dependency
+        if self.source.name == 'local':
+            return '{}({})'.format(self._name, self.source._path)  # type: ignore
+        else:
+            return '{}({})'.format(self._name, self._version_spec)
 
 
 @total_ordering
 @serializable(like='str')
 class ComponentVersion(object):
     def __init__(self, version_string, dependencies=None):  # type: (str, list[ComponentRequirement] | None) -> None
         """
@@ -272,25 +277,23 @@
         if self.is_semver and self._semver:
             return self._semver
         else:
             raise TypeError('Version is not semantic')
 
 
 class HashedComponentVersion(ComponentVersion):
-    def __init__(self, *args, **kwargs):  # type: (Any, Any) -> None
+    def __init__(self, *args, **kwargs):
         component_hash = kwargs.pop('component_hash', None)
         dependencies = kwargs.pop('dependencies', []) or []
         targets = kwargs.pop('targets', [])
-        all_build_keys_known = kwargs.pop('all_build_keys_known', True)
         super(HashedComponentVersion, self).__init__(*args, **kwargs)
 
         self.component_hash = component_hash
         self.dependencies = dependencies  # type: list[ComponentRequirement]
         self.targets = targets
-        self.all_build_keys_known = all_build_keys_known
 
     def __hash__(self):
         return hash(self.component_hash) if self.component_hash else hash(str(self))
 
     @property
     def text(self):
         return str(self)
@@ -302,15 +305,15 @@
         self.name = name
 
 
 class ProjectRequirements(object):
     '''Representation of all manifests required by project'''
     def __init__(self, manifests):  # type: (list[Manifest]) -> None
         self.manifests = manifests
-        self._manifest_hash = None  # type: str | None
+        self._manifest_hash = None
         self._target = None  # type: str | None
 
     @property
     def target(self):  # type: () -> str
         if not self._target:
             self._target = get_env_idf_target()
         return self._target
@@ -322,9 +325,8 @@
     @property
     def manifest_hash(self):  # type: () -> str
         '''Lazily calculate requirements hash'''
         if self._manifest_hash:
             return self._manifest_hash
 
         manifest_hashes = [manifest.manifest_hash for manifest in self.manifests]
-        self._manifest_hash = hash_object(manifest_hashes)
-        return self._manifest_hash
+        return hash_object(manifest_hashes)
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/manifest/solved_component.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/solved_component.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/manifest/solved_manifest.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/solved_manifest.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/semver/base.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/semver/base.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/serialization.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/serialization.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/sources/__init__.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/sources/base.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -150,22 +150,14 @@
         return False
 
     @property
     def meta(self):  # type: () -> bool
         """Returns True for meta components. Meta components are not included in the build directly"""
         return False
 
-    @property
-    def volatile(self):  # type: () -> bool
-        """
-        Returns True for volatile components.
-        Volatile components may change their content, even if their version stays the same.
-        """
-        return False
-
     def normalized_name(self, name):  # type: (str) -> str
         return name
 
     def up_to_date(self, component, path):  # type: (SolvedComponent, str) -> bool
         if self.component_hash_required and not component.component_hash:
             raise FetchingError('Cannot install component with unknown hash')
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/sources/fetcher.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/fetcher.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/sources/git.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 import re
 import shutil
 import tempfile
 from hashlib import sha256
@@ -32,26 +32,25 @@
 
 
 class GitSource(BaseSource):
     NAME = 'git'
 
     def __init__(self, source_details=None, **kwargs):
         super(GitSource, self).__init__(source_details=source_details, **kwargs)
-        self.git_repo = self.source_details['git']
-        self.component_path = self.source_details.get('path') or '.'
+        self.git_repo = source_details['git']
+        self.component_path = source_details.get('path') or '.'
 
         self._client = GitClient()
 
     def _checkout_git_source(
             self,
             version,  # type: str | ComponentVersion | None
             path,  # type: str
             selected_paths=None  # type: list[str] | None
     ):  # type: (...) -> str
-
         if version is not None:
             version = None if version == '*' else str(version)
         return self._client.prepare_ref(
             repo=self.git_repo,
             bare_path=self.cache_path(),
             checkout_path=path,
             ref=version,
@@ -84,18 +83,14 @@
             url = urlparse(self.git_repo)
             netloc = url.netloc
             path = '/'.join(filter(None, url.path.split('/')))
             normalized_path = '/'.join([netloc, path])
             self._hash_key = sha256(normalized_path.encode('utf-8')).hexdigest()
         return self._hash_key
 
-    @property
-    def volatile(self):  # type: () -> bool
-        return True
-
     def cache_path(self):
         # Using `b_` prefix for bare git repos in cache
         path = os.path.join(self.system_cache_path, 'b_{}_{}'.format(self.NAME, self.hash_key[:8]))
         return path
 
     def download(self, component, download_path):  # type: (SolvedComponent, str) -> str | None
         # Check for required components
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/sources/idf.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/idf.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.0/idf_component_tools/sources/local.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/local.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 class LocalSource(BaseSource):
     NAME = 'local'
 
     def __init__(self, source_details, **kwargs):
         super(LocalSource, self).__init__(source_details=source_details, **kwargs)
 
-        self.is_overrider = 'override_path' in self.source_details
-        self._raw_path = Path(self.source_details.get('override_path' if self.is_overrider else 'path'))
+        self.is_overrider = 'override_path' in source_details
+        self._raw_path = Path(source_details.get('override_path' if self.is_overrider else 'path'))
 
     @property
     def _path(self):  # type: () -> Path
         try:
             if self._manifest_manager:
                 path = (Path(self._manifest_manager.path).parent / self._raw_path).resolve()
             elif not self._manifest_manager and self._raw_path.is_absolute():
@@ -42,31 +42,22 @@
                 raise ManifestContextError(
                     "Can't reliably evaluate relative path without context: {}".format(str(self._raw_path)))
 
             if not path.is_dir():  # for Python > 3.6, where .resolve(strict=False)
                 raise OSError()
 
         except OSError:
-            raise SourcePathError(
-                "The 'override_path' field in the manifest file '{}' does not point to a directory. You can safely "
-                'remove this field from the manifest if this project is an example copied from a component '
-                'repository. The dependency will be downloaded from the ESP component registry. Documentation: '
-                'https://docs.espressif.com/projects/idf-component-manager/en/latest/reference/manifest_file.html'
-                '#override-path'.format(str(self._raw_path / 'idf_component.yml')))
+            raise SourcePathError('Invalid source path, should be a directory: %s' % str(self._raw_path))
 
         if self.is_overrider and path / 'CMakeLists.txt' not in path.iterdir():
             raise SourcePathError(
                 'The override_path you\'re using is pointing to directory "%s" that is not a component.' % str(path))
 
         return path
 
-    @property
-    def component_hash_required(self):  # type: () -> bool
-        return False
-
     @classmethod
     def required_keys(cls):
         return {'path': 'str'}
 
     @classmethod
     def optional_keys(cls):
         return {'override_path': 'str'}
@@ -75,18 +66,14 @@
     def is_me(name, details):
         return bool(details.get('path', None)) or 'override_path' in details
 
     @property
     def hash_key(self):
         return self.source_details.get('path')
 
-    @property
-    def volatile(self):  # type: () -> bool
-        return True
-
     def download(self, component, download_path):
         directory_name = os.path.basename(str(self._path))
         component_with_namespace = component.name.replace('/', '__')
         namespace_and_component = component.name.split('/')
         component_without_namespace = namespace_and_component[-1]
         if component_without_namespace != directory_name and component_with_namespace != directory_name:
             alternative_name = ' or "{}"'.format(component_with_namespace) if len(namespace_and_component) == 2 else ''
```

### Comparing `idf_component_manager-1.3.0/idf_component_tools/sources/web_service.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/web_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import requests
 
 import idf_component_tools.api_client as api_client
 from idf_component_tools.semver import SimpleSpec
 
 from ..archive_tools import ArchiveError, get_format_from_path, unpack_archive
 from ..config import component_registry_url
-from ..constants import IDF_COMPONENT_REGISTRY_URL, IDF_COMPONENT_STORAGE_URL, UPDATE_SUGGESTION
+from ..constants import IDF_COMPONENT_REGISTRY_URL, IDF_COMPONENT_STORAGE_URL
 from ..errors import FetchingError, hint
 from ..file_tools import copy_directory
 from ..hash_tools import validate_filtered_dir
 from . import utils
 from .base import BaseSource
 
 try:
@@ -140,29 +140,24 @@
         return path
 
     def versions(self, name, details=None, spec='*', target=None):
         cmp_with_versions = self.api_client.versions(component_name=name, spec=spec)
         versions = []
         other_targets_versions = []
         pre_release_versions = []
-        newer_component_manager_versions = []
 
         for version in cmp_with_versions.versions:
             if target and version.targets and target not in version.targets:
                 other_targets_versions.append(version)
                 continue
 
             if not self.pre_release and version.semver.prerelease and not SimpleSpec(spec).contains_prerelease:
                 pre_release_versions.append(str(version))
                 continue
 
-            if not version.all_build_keys_known:
-                newer_component_manager_versions.append(str(version))
-                continue
-
             versions.append(version)
 
         cmp_with_versions.versions = versions
         if not versions:
             current_target = '"{}"'.format(target) if target else ''
 
             if pre_release_versions:
@@ -173,20 +168,14 @@
 
             if other_targets_versions:
                 targets = {t for v in other_targets_versions for t in v.targets}
                 hint(
                     'Component "{}" has suitable versions for other targets: "{}". '
                     'Is your current target {} set correctly?'.format(name, '", "'.join(targets), current_target))
 
-            if newer_component_manager_versions:
-                hint(
-                    'Component "{}" has versions "{}" that support only newer version of idf-component-manager '
-                    'that satisfy your requirements.\n'
-                    '{}'.format(name, '", "'.join(newer_component_manager_versions), UPDATE_SUGGESTION))
-
             raise FetchingError(
                 'Cannot find versions of "{}" satisfying "{}" '
                 'for the current target {}.'.format(name, spec, current_target))
 
         return cmp_with_versions
 
     @property
```

### Comparing `idf_component_manager-1.3.0/setup.py` & `idf_component_manager-1.3.0.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     'click<8.0.0;python_version=="3.5.*"',
     'click<8.1.0;python_version=="3.6.*"',
     'click;python_version>="3.7"',
     'colorama;python_version=="2.7.*"',
     'colorama;python_version>="3.5"',
     'contextlib2<=0.6.0;python_version<"3.6"',
     'contextlib2>0.6.0;python_version>="3.6"',
+    'future',
     'packaging',
     'pathlib;python_version<"3.4"',
     'pyyaml<=5.2;python_version=="3.4.*"',
     'pyyaml>5.2;python_version>="3.5"',
     'pyyaml<=5.2;python_version=="2.7.*"',
     'requests<3',
-    'urllib3<2',
     'requests-file',
     'requests-toolbelt',
     'schema',
     'six',
     'tqdm<5',
 ]
```

