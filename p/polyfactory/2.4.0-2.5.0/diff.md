# Comparing `tmp/polyfactory-2.4.0.tar.gz` & `tmp/polyfactory-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.4.0.tar", max compression
+gzip compressed data, was "polyfactory-2.5.0.tar", max compression
```

## Comparing `polyfactory-2.4.0.tar` & `polyfactory-2.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1092 2023-06-25 17:54:51.308744 polyfactory-2.4.0/LICENSE
--rw-r--r--   0        0        0    16840 2023-06-25 17:54:51.308744 polyfactory-2.4.0/README.md
--rw-r--r--   0        0        0      425 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/__init__.py
--rw-r--r--   0        0        0      875 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    33164 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1897 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2392 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2217 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    11187 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1598 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     7314 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3317 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/py.typed
--rw-r--r--   0        0        0     2919 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3488 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     3113 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1885 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1125 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13607 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      522 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      529 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      535 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3636 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6186 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6554 2023-06-25 17:54:51.312744 polyfactory-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    18762 1970-01-01 00:00:00.000000 polyfactory-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-30 19:43:25.009172 polyfactory-2.5.0/LICENSE
+-rw-r--r--   0        0        0    24136 2023-06-30 19:43:25.009172 polyfactory-2.5.0/docs/PYPI_README.md
+-rw-r--r--   0        0        0      425 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/__init__.py
+-rw-r--r--   0        0        0      875 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    33045 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1681 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2392 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2192 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    10468 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1431 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     7084 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3317 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/py.typed
+-rw-r--r--   0        0        0     2850 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3852 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3498 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     1605 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1885 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1125 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13429 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      433 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      440 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      446 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3635 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6172 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6733 2023-06-30 19:43:25.013172 polyfactory-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0    26005 1970-01-01 00:00:00.000000 polyfactory-2.5.0/PKG-INFO
```

### Comparing `polyfactory-2.4.0/LICENSE` & `polyfactory-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/README.md` & `polyfactory-2.5.0/docs/PYPI_README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,31 @@
-# Polyfactory
-
 <!-- markdownlint-disable -->
 <p align="center">
-  <img src="https://github.com/litestar-org/branding/blob/e27cda904e0649e5065ac1c26df6a279ba5d06b5/assets/Branding%20-%20SVG%20-%20Transparent/Polyfactory%20-%20Banner%20-%20Inline%20-%20Light.svg#gh-light-mode-only" alt="Litestar - Polyfactory Logo - Light" width="100%" height="auto" />
-  <img src="https://github.com/litestar-org/branding/blob/e27cda904e0649e5065ac1c26df6a279ba5d06b5/assets/Branding%20-%20SVG%20-%20Transparent/Polyfactory%20-%20Banner%20-%20Inline%20-%20Dark.svg#gh-dark-mode-only" alt="Litestar - Polyfactory Logo - Dark" width="100%" height="auto" />
+  <img src="https://github.com/litestar-org/branding/blob/473f54621e55cde9acbb6fcab7fc03036173eb3d/assets/Branding%20-%20PNG%20-%20Transparent/Polyfactory%20-%20Banner%20-%20Inline%20-%20Light.png?raw=true" alt="Polyfactory Logo - Light" width="100%" height="auto" />
 </p>
 <!-- markdownlint-restore -->
 
-<!-- markdownlint-disable -->
 <div align="center">
+<!-- prettier-ignore-start -->
 
-![PyPI - License](https://img.shields.io/pypi/l/polyfactory?color=blue)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/polyfactory)
-
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_polyfactory&metric=coverage)](https://sonarcloud.io/summary/new_code?id=litestar-org_polyfactory)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_polyfactory&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_polyfactory)
-[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_polyfactory&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_polyfactory)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_polyfactory&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_polyfactory)
-[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_polyfactory&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_polyfactory)
-
-[![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
-[![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
-[![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
-[![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
-
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-
-[![All Contributors](https://img.shields.io/badge/all_contributors-29-orange.svg?style=flat-square)](#contributors-)
+| Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| --------- | :-- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| CI/CD     |     | [![Publish package](https://github.com/litestar-org/polyfactory/actions/workflows/publish.yaml/badge.svg)](https://github.com/litestar-org/polyfactory/actions/workflows/publish.yaml) [![ci](https://github.com/litestar-org/polyfactory/actions/workflows/ci.yaml/badge.svg)](https://github.com/litestar-org/polyfactory/actions/workflows/ci.yaml) [![pages-build-deployment](https://github.com/litestar-org/polyfactory/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/litestar-org/polyfactory/actions/workflows/pages/pages-build-deployment)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| Quality   |     | [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=coverage)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)                                                                                                                                                                                                                                                                                                                                                                                                            |
+| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/polyfactory?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/polyfactory) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/polyfactory?labelColor=202235&color=edb641&logo=python&logoColor=edb641) ![Pydantic Factories PyPI - Downloads](https://img.shields.io/pypi/dm/pydantic-factories?logo=python&label=Pydantic%20Factories%20downloads&labelColor=202235&color=edb641&logoColor=edb641) ![Polyfactory PyPI - Downloads](https://img.shields.io/pypi/dm/polyfactory?logo=python&label=Polyfactory%20downloads&labelColor=202235&color=edb641&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/X3FJqy8d2j) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                                                                                                                                                   |
+| Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Polyfactory-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/polyfactory) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=python&labelColor=202235&logoColor=edb641)](https://github.com/psf/black) [![Sourcery](https://img.shields.io/badge/Sourcery-enabled-edb641?labelColor=202235&logoColor=edb641)](https://sourcery.ai) [![All Contributors](https://img.shields.io/github/all-contributors/litestar-org/polyfactory?labelColor=202235&color=edb641&logoColor=edb641)](#contributors-) |
 
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
+<!-- prettier-ignore-end -->
 
 </div>
 <!-- markdownlint-restore -->
 
+# Polyfactory
+
 Polyfactory is a simple and powerful mock data generation library, based around type
 hints and supporting dataclasses, typed-dicts, pydantic models, msgspec structs and more.
 
 Polyfactory part of the Litestar project and as such actively maintained by a community of maintainers and contributors.
 
 ## Example
 
@@ -102,51 +91,51 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://schutt.io"><img src="https://avatars.githubusercontent.com/u/20659309?v=4?s=100" width="100px;" alt="Peter Schutt"/><br /><sub><b>Peter Schutt</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=peterschutt" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#maintenance-Goldziher" title="Maintenance">🚧</a> <a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#maintenance-JacobCoffee" title="Maintenance">🚧</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://schutt.io"><img src="https://avatars.githubusercontent.com/u/20659309?v=4?s=100" width="100px;" alt="Peter Schutt"/><br /><sub><b>Peter Schutt</b></sub></a><br /><a href="#maintenance-peterschutt" title="Maintenance">🚧</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=peterschutt" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=peterschutt" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=peterschutt" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sygutss"><img src="https://avatars.githubusercontent.com/u/48909366?v=4?s=100" width="100px;" alt="sygutss"/><br /><sub><b>sygutss</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/issues?q=author%3Asygutss" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=sygutss" title="Code">💻</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/guacs"><img src="https://avatars.githubusercontent.com/u/126393040?v=4?s=100" width="100px;" alt="guacs"/><br /><sub><b>guacs</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=guacs" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/VSHUMILIN97"><img src="https://avatars.githubusercontent.com/u/27234763?v=4?s=100" width="100px;" alt="Vadim"/><br /><sub><b>Vadim</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=VSHUMILIN97" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Simske"><img src="https://avatars.githubusercontent.com/u/2445660?v=4?s=100" width="100px;" alt="Simske"/><br /><sub><b>Simske</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=Simske" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sondrelg"><img src="https://avatars.githubusercontent.com/u/25310870?v=4?s=100" width="100px;" alt="Sondre Lillebø Gundersen"/><br /><sub><b>Sondre Lillebø Gundersen</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=sondrelg" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://mciszczon.pl/"><img src="https://avatars.githubusercontent.com/u/1078369?v=4?s=100" width="100px;" alt="Mateusz Ciszczoń"/><br /><sub><b>Mateusz Ciszczoń</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mciszczon" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/pedro-bernardes/"><img src="https://avatars.githubusercontent.com/u/18899993?v=4?s=100" width="100px;" alt="Pedro Bernardes"/><br /><sub><b>Pedro Bernardes</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=phbernardes" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lindycoder"><img src="https://avatars.githubusercontent.com/u/12926519?v=4?s=100" width="100px;" alt="Martin Roy"/><br /><sub><b>Martin Roy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=lindycoder" title="Code">💻</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/roeeyn"><img src="https://avatars.githubusercontent.com/u/13385000?v=4?s=100" width="100px;" alt="Rodrigo Medina"/><br /><sub><b>Rodrigo Medina</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=roeeyn" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://gerritegnew.info/"><img src="https://avatars.githubusercontent.com/u/35822787?v=4?s=100" width="100px;" alt="Gerrit Egnew"/><br /><sub><b>Gerrit Egnew</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=gegnew" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/danielkatzan"><img src="https://avatars.githubusercontent.com/u/9249066?v=4?s=100" width="100px;" alt="danielkatzan"/><br /><sub><b>danielkatzan</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=danielkatzan" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/gigelu"><img src="https://avatars.githubusercontent.com/u/270697?v=4?s=100" width="100px;" alt="gigelu"/><br /><sub><b>gigelu</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=gigelu" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="http://linkedin.com/in/roman-reznikov"><img src="https://avatars.githubusercontent.com/u/44291988?v=4?s=100" width="100px;" alt="Roman Reznikov"/><br /><sub><b>Roman Reznikov</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=ReznikovRoman" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/anthonyh209"><img src="https://avatars.githubusercontent.com/u/33107540?v=4?s=100" width="100px;" alt="anthonyh209"/><br /><sub><b>anthonyh209</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=anthonyh209" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/avihai-yosef"><img src="https://avatars.githubusercontent.com/u/79567307?v=4?s=100" width="100px;" alt="avihai-yosef"/><br /><sub><b>avihai-yosef</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=avihai-yosef" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lindycoder"><img src="https://avatars.githubusercontent.com/u/12926519?v=4?s=100" width="100px;" alt="Martin Roy"/><br /><sub><b>Martin Roy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=lindycoder" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://matthewtyleraylward.com"><img src="https://avatars.githubusercontent.com/u/19205392?v=4?s=100" width="100px;" alt="Matthew Aylward "/><br /><sub><b>Matthew Aylward </b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=Butch78" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/EltonChou"><img src="https://avatars.githubusercontent.com/u/12560310?v=4?s=100" width="100px;" alt="Elton H.Y. Chou"/><br /><sub><b>Elton H.Y. Chou</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=EltonChou" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nguyent"><img src="https://avatars.githubusercontent.com/u/576848?v=4?s=100" width="100px;" alt="Thang"/><br /><sub><b>Thang</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=nguyent" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/DaanRademaker"><img src="https://avatars.githubusercontent.com/u/29598493?v=4?s=100" width="100px;" alt="Daan"/><br /><sub><b>Daan</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=DaanRademaker" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://lyz-code.github.io/blue-book/"><img src="https://avatars.githubusercontent.com/u/24810987?v=4?s=100" width="100px;" alt="Lyz"/><br /><sub><b>Lyz</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=lyz-code" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://portfolio.schiffer.pro/"><img src="https://avatars.githubusercontent.com/u/3502492?v=4?s=100" width="100px;" alt="Thorin Schiffer"/><br /><sub><b>Thorin Schiffer</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=thorin-schiffer" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Iipin"><img src="https://avatars.githubusercontent.com/u/52832022?v=4?s=100" width="100px;" alt="Iipin"/><br /><sub><b>Iipin</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=Iipin" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://portfolio.schiffer.pro/"><img src="https://avatars.githubusercontent.com/u/3502492?v=4?s=100" width="100px;" alt="Thorin Schiffer"/><br /><sub><b>Thorin Schiffer</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=thorin-schiffer" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://lyz-code.github.io/blue-book/"><img src="https://avatars.githubusercontent.com/u/24810987?v=4?s=100" width="100px;" alt="Lyz"/><br /><sub><b>Lyz</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=lyz-code" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/DaanRademaker"><img src="https://avatars.githubusercontent.com/u/29598493?v=4?s=100" width="100px;" alt="Daan"/><br /><sub><b>Daan</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=DaanRademaker" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nguyent"><img src="https://avatars.githubusercontent.com/u/576848?v=4?s=100" width="100px;" alt="Thang"/><br /><sub><b>Thang</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=nguyent" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/EltonChou"><img src="https://avatars.githubusercontent.com/u/12560310?v=4?s=100" width="100px;" alt="Elton H.Y. Chou"/><br /><sub><b>Elton H.Y. Chou</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=EltonChou" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/avihai-yosef"><img src="https://avatars.githubusercontent.com/u/79567307?v=4?s=100" width="100px;" alt="avihai-yosef"/><br /><sub><b>avihai-yosef</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=avihai-yosef" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/anthonyh209"><img src="https://avatars.githubusercontent.com/u/33107540?v=4?s=100" width="100px;" alt="anthonyh209"/><br /><sub><b>anthonyh209</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=anthonyh209" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://linkedin.com/in/roman-reznikov"><img src="https://avatars.githubusercontent.com/u/44291988?v=4?s=100" width="100px;" alt="Roman Reznikov"/><br /><sub><b>Roman Reznikov</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=ReznikovRoman" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/gigelu"><img src="https://avatars.githubusercontent.com/u/270697?v=4?s=100" width="100px;" alt="gigelu"/><br /><sub><b>gigelu</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=gigelu" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/roeeyn"><img src="https://avatars.githubusercontent.com/u/13385000?v=4?s=100" width="100px;" alt="Rodrigo Medina"/><br /><sub><b>Rodrigo Medina</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=roeeyn" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://gerritegnew.info/"><img src="https://avatars.githubusercontent.com/u/35822787?v=4?s=100" width="100px;" alt="Gerrit Egnew"/><br /><sub><b>Gerrit Egnew</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=gegnew" title="Code">💻</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="http://matthewtyleraylward.com"><img src="https://avatars.githubusercontent.com/u/19205392?v=4?s=100" width="100px;" alt="Matthew Aylward "/><br /><sub><b>Matthew Aylward </b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=Butch78" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/danielkatzan"><img src="https://avatars.githubusercontent.com/u/9249066?v=4?s=100" width="100px;" alt="danielkatzan"/><br /><sub><b>danielkatzan</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=danielkatzan" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `polyfactory-2.4.0/polyfactory/constants.py` & `polyfactory-2.5.0/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/decorators.py` & `polyfactory-2.5.0/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/exceptions.py` & `polyfactory-2.5.0/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/factories/base.py` & `polyfactory-2.5.0/polyfactory/factories/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,77 +4,82 @@
 from collections import Counter, abc, deque
 from contextlib import suppress
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from enum import EnumMeta
 from functools import partial
 from importlib import import_module
-from inspect import isclass
 from ipaddress import (
     IPv4Address,
     IPv4Interface,
     IPv4Network,
     IPv6Address,
     IPv6Interface,
     IPv6Network,
     ip_address,
     ip_interface,
     ip_network,
 )
 from os.path import realpath
 from pathlib import Path
-from random import Random
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
+    Collection,
     Generic,
     Mapping,
     Sequence,
     Type,
     TypeVar,
     cast,
 )
 from uuid import NAMESPACE_DNS, UUID, uuid1, uuid3, uuid5
 
 from faker import Faker
 from typing_extensions import get_args
 
+from polyfactory.constants import DEFAULT_RANDOM
 from polyfactory.exceptions import (
     ConfigurationException,
     MissingBuildKwargException,
     ParameterException,
 )
 from polyfactory.fields import Fixture, Ignore, PostGenerated, Require, Use
 from polyfactory.utils.helpers import unwrap_annotation, unwrap_args, unwrap_optional
 from polyfactory.utils.predicates import (
     get_type_origin,
+    is_any,
     is_literal,
     is_optional_union,
     is_safe_subclass,
+    is_union,
 )
-from polyfactory.value_generators.complex_types import handle_complex_type
+from polyfactory.value_generators.complex_types import handle_collection_type
 from polyfactory.value_generators.constrained_collections import handle_constrained_collection
 from polyfactory.value_generators.constrained_dates import handle_constrained_date
 from polyfactory.value_generators.constrained_numbers import (
     handle_constrained_decimal,
     handle_constrained_float,
     handle_constrained_int,
 )
 from polyfactory.value_generators.constrained_path import handle_constrained_path
 from polyfactory.value_generators.constrained_strings import handle_constrained_string_or_bytes
 from polyfactory.value_generators.constrained_url import handle_constrained_url
 from polyfactory.value_generators.constrained_uuid import handle_constrained_uuid
 from polyfactory.value_generators.primitives import (
     create_random_boolean,
     create_random_bytes,
+    create_random_string,
 )
 
 if TYPE_CHECKING:
+    from random import Random
+
     from typing_extensions import TypeGuard
 
     from polyfactory.field_meta import Constraints, FieldMeta
     from polyfactory.persistence import AsyncPersistenceProtocol, SyncPersistenceProtocol
 
 
 def _create_pydantic_type_map(cls: type[BaseFactory[Any]]) -> dict[type, Callable[[], Any]]:
@@ -114,15 +119,15 @@
             pydantic.PastDate: cls.__faker__.past_date,
             pydantic.FutureDate: cls.__faker__.future_date,
         }
 
     except ImportError:
         mapping = {}
 
-    try:
+    with suppress(ImportError):
         # v1 only values - these will raise an exception in v2
         # in pydantic v2 these are all aliases for Annotated with a constraint.
         # we therefore do not need them in v2
         from pydantic import (
             UUID1,
             UUID3,
             UUID4,
@@ -148,41 +153,25 @@
                 UUID1: uuid1,
                 UUID3: lambda: uuid3(NAMESPACE_DNS, cls.__faker__.pystr()),
                 UUID4: cls.__faker__.uuid4,
                 UUID5: lambda: uuid5(NAMESPACE_DNS, cls.__faker__.pystr()),
             }
         )
 
-    except ImportError:
-        pass
-
-    try:
+    with suppress(ImportError):
         # this might be removed by pydantic 2
         from pydantic import color
 
         mapping[color.Color] = cls.__faker__.hex_color  # pyright: ignore
-    except ImportError:
-        pass
-
     return mapping
 
 
 T = TypeVar("T")
 
 
-def is_factory(value: Any) -> "TypeGuard[type[BaseFactory[Any]]]":
-    """Determine if a given value is a subclass of ModelFactory.
-
-    :param value: An arbitrary value.
-    :returns: A boolean typeguard.
-
-    """
-    return isclass(value) and issubclass(value, BaseFactory)
-
-
 class BaseFactory(ABC, Generic[T]):
     """Base Factory class - this class holds the main logic of the library"""
 
     # configuration attributes
     __model__: type[T]
     """
     The model for the factory.
@@ -213,15 +202,15 @@
 
     Note: this value can only be set when '__is_base_factory__' is 'True'.
     """
     __faker__: ClassVar["Faker"] = Faker()
     """
     A faker instance to use. Can be a user provided value.
     """
-    __random__: ClassVar["Random"] = Random()
+    __random__: ClassVar["Random"] = DEFAULT_RANDOM
     """
     An instance of 'random.Random' to use.
     """
     __random_seed__: ClassVar[int]
     """
     An integer to seed the factory's Faker and Random instances with.
     This attribute can be used to control random generation.
@@ -299,53 +288,47 @@
         """Handle a value defined on the factory class itself.
 
         :param field_value: A value defined as an attribute on the factory class.
         :param field_build_parameters: Any build parameters passed to the factory as kwarg values.
 
         :returns: An arbitrary value correlating with the given field_meta value.
         """
-        if is_factory(field_value):
+        if is_safe_subclass(field_value, BaseFactory):
             if isinstance(field_build_parameters, Mapping):
                 return field_value.build(**field_build_parameters)
 
             if isinstance(field_build_parameters, Sequence):
                 return [field_value.build(**parameter) for parameter in field_build_parameters]
 
             return field_value.build()
 
         if isinstance(field_value, Use):
             return field_value.to_value()
 
         if isinstance(field_value, Fixture):
             return field_value.to_value()
 
-        if callable(field_value):
-            return field_value()
-
-        return field_value
+        return field_value() if callable(field_value) else field_value
 
     @classmethod
-    def _get_or_create_factory(
-        cls,
-        model: type,
-    ) -> type[BaseFactory[Any]]:
+    def _get_or_create_factory(cls, model: type) -> type[BaseFactory[Any]]:
         """Get a factory from registered factories or generate a factory dynamically.
 
         :param model: A model type.
         :returns: A Factory sub-class.
 
         """
-        if cls.__base_factory_overrides__ and (
-            factory := cls.__base_factory_overrides__.get(model, cls.__base_factory_overrides__.get(type(model)))
-        ):
-            return factory.create_factory(model)
-
         if factory := BaseFactory._factory_type_mapping.get(model):
             return factory
 
+        if cls.__base_factory_overrides__:
+            for model_ancestor in model.mro():
+                if factory := cls.__base_factory_overrides__.get(model_ancestor):
+                    return factory.create_factory(model)
+
         for factory in reversed(BaseFactory._base_factories):
             if factory.is_supported_type(model):
                 return factory.create_factory(model)
 
         raise ParameterException(f"unsupported model type {model.__name__}")  # pragma: no cover
 
     # Public Methods
@@ -363,15 +346,15 @@
     def is_batch_factory_type(cls, annotation: Any) -> bool:
         """Determine whether a given field is annotated with a sequence of supported factory types.
 
         :param annotation: A type annotation.
         :returns: Boolean dictating whether the annotation is a batch factory type
         """
         origin = get_type_origin(annotation) or annotation
-        if is_safe_subclass(origin, Sequence) and (args := unwrap_args(annotation, random=cls.__random__)):  # type: ignore
+        if is_safe_subclass(origin, Sequence) and (args := unwrap_args(annotation, random=cls.__random__)):
             return len(args) == 1 and BaseFactory.is_factory_type(annotation=args[0])
         return False
 
     @classmethod
     def extract_field_build_parameters(cls, field_meta: FieldMeta, build_args: dict[str, Any]) -> Any:
         """Extract from the build kwargs any build parameters passed for a given field meta - if it is a factory type.
 
@@ -483,37 +466,14 @@
             Callable: _create_generic_fn,
             abc.Callable: _create_generic_fn,
             Counter: lambda: Counter(cls.__faker__.pystr()),
             **_create_pydantic_type_map(cls),
         }
 
     @classmethod
-    def get_mock_value(cls, annotation: type) -> Any:
-        """Return a mock value for a given type.
-
-        :param annotation: An arbitrary type.
-        :returns: An arbitrary value.
-
-        """
-
-        if handler := cls.get_provider_map().get(annotation):
-            return handler()
-
-        if isclass(annotation):
-            # if value is a class we can try to naively instantiate it.
-            # this will work for classes that do not require any parameters passed to __init__
-            with suppress(Exception):
-                return annotation()
-
-        raise ParameterException(
-            f"Unsupported type: {annotation!r}"
-            f"\n\nEither extend the providers map or add a factory function for this type."
-        )
-
-    @classmethod
     def create_factory(
         cls,
         model: type,
         bases: tuple[type[BaseFactory[Any]], ...] | None = None,
         **kwargs: Any,
     ) -> type[BaseFactory[Any]]:
         """Generate a factory for the given type dynamically.
@@ -670,18 +630,36 @@
 
         if BaseFactory.is_batch_factory_type(annotation=unwrapped_annotation):
             factory = cls._get_or_create_factory(model=field_meta.type_args[0])
             if isinstance(field_build_parameters, Sequence):
                 return [factory.build(**field_parameters) for field_parameters in field_build_parameters]
             return factory.batch(size=cls.__random__.randint(1, 10))
 
-        if field_meta.children:
-            return handle_complex_type(field_meta=field_meta, factory=cls)
+        if (origin := get_type_origin(unwrapped_annotation)) and issubclass(origin, Collection):
+            return handle_collection_type(field_meta, origin, cls)
+
+        if is_union(field_meta.annotation) and field_meta.children:
+            return cls.get_field_value(cls.__random__.choice(field_meta.children))
+
+        if is_any(unwrapped_annotation) or isinstance(unwrapped_annotation, TypeVar):
+            return create_random_string(cls.__random__, min_length=1, max_length=10)
 
-        return cls.get_mock_value(annotation=unwrapped_annotation)
+        if provider := cls.get_provider_map().get(unwrapped_annotation):
+            return provider()
+
+        if callable(unwrapped_annotation):
+            # if value is a callable we can try to naively call it.
+            # this will work for callables that do not require any parameters passed
+            with suppress(Exception):
+                return unwrapped_annotation()
+
+        raise ParameterException(
+            f"Unsupported type: {unwrapped_annotation!r}"
+            f"\n\nEither extend the providers map or add a factory function for this type."
+        )
 
     @classmethod
     def should_set_none_value(cls, field_meta: FieldMeta) -> bool:
         """Determine whether a given model field_meta should be set to None.
 
         :param field_meta: Field metadata.
```

### Comparing `polyfactory-2.4.0/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.5.0/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.5.0/polyfactory/factories/dataclass_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 from __future__ import annotations
 
 from dataclasses import MISSING, fields, is_dataclass
-from inspect import isclass
-from typing import TYPE_CHECKING, Any, Generic
+from typing import Any, Generic
 
-from typing_extensions import get_type_hints
+from typing_extensions import TypeGuard, get_type_hints
 
 from polyfactory.factories.base import BaseFactory, T
 from polyfactory.field_meta import FieldMeta, Null
 
-if TYPE_CHECKING:
-    from typing_extensions import TypeGuard
-
 
 class DataclassFactory(Generic[T], BaseFactory[T]):
     """Dataclass base factory"""
 
     __is_base_factory__ = True
 
     @classmethod
-    def is_supported_type(cls, value: Any) -> "TypeGuard[type[T]]":
+    def is_supported_type(cls, value: Any) -> TypeGuard[type[T]]:
         """Determine whether the given value is supported by the factory.
 
         :param value: An arbitrary value.
         :returns: A typeguard
         """
-        try:
-            return isclass(value) and is_dataclass(value)
-        except (TypeError, AttributeError):  # pragma: no cover
-            return False
+        return bool(is_dataclass(value))
 
     @classmethod
     def get_model_fields(cls) -> list["FieldMeta"]:
         """Retrieve a list of fields from the factory's model.
 
 
         :returns: A list of field MetaData instances.
```

### Comparing `polyfactory-2.4.0/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.5.0/polyfactory/factories/msgspec_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.5.0/polyfactory/factories/odmantic_odm_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     @classmethod
     def is_supported_type(cls, value: Any) -> "TypeGuard[type[T]]":
         """Determine whether the given value is supported by the factory.
 
         :param value: An arbitrary value.
         :returns: A typeguard
         """
-        return is_safe_subclass(value, Model) or is_safe_subclass(value, EmbeddedModel)
+        return is_safe_subclass(value, (Model, EmbeddedModel))
 
     @classmethod
     def get_provider_map(cls) -> dict[Any, Callable[[], Any]]:
         provider_map = super().get_provider_map()
         provider_map.update(
             {
                 odbson.Int64: lambda: odbson.Int64.validate(cls.__faker__.pyint()),
```

### Comparing `polyfactory-2.4.0/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.5.0/polyfactory/factories/pydantic_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from contextlib import suppress
-from inspect import isclass
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Generic,
     Literal,
     Mapping,
@@ -13,65 +12,48 @@
     cast,
 )
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import Constraints, FieldMeta, Null
 from polyfactory.utils.helpers import unwrap_new_type, unwrap_optional
-from polyfactory.utils.predicates import is_optional_union
+from polyfactory.utils.predicates import is_optional_union, is_safe_subclass
 
 try:
     from pydantic import BaseModel
-
+    from pydantic.fields import FieldInfo
 except ImportError as e:
     raise MissingDependencyException("pydantic is not installed") from e
 
 try:
     from pydantic.fields import ModelField  # type: ignore[attr-defined]
 
     pydantic_version: Literal[1, 2] = 1
 except ImportError:
     pydantic_version = 2
 
     ModelField = Any
-    from pydantic._internal._fields import Undefined
+    from pydantic_core import PydanticUndefined as Undefined
 
 if TYPE_CHECKING:
     from random import Random
 
-    from pydantic.fields import FieldInfo
     from typing_extensions import TypeGuard
 
-T = TypeVar("T", bound=BaseModel)
-
-
-def is_pydantic_model(value: Any) -> "TypeGuard[type[BaseModel]]":
-    """Determine whether the given value is a subclass of BaseModel.
 
-    :param value: A value to test.
-
-    :returns: A type guard.
-
-    """
-    try:
-        return isclass(value) and issubclass(value, BaseModel)
-    except TypeError:  # pragma: no cover
-        # isclass(value) returns True for python 3.9+ typings such as list[str] etc.
-        # this raises a TypeError in issubclass, and so we need to handle it.
-        return False
+T = TypeVar("T", bound=BaseModel)
 
 
 class PydanticFieldMeta(FieldMeta):
     """Field meta subclass capable of handling pydantic ModelFields"""
 
-    # FIXME: remove the pragma when switching to pydantic v2 permanently
     @classmethod
     def from_field_info(
         cls, field_name: str, field_info: FieldInfo, use_alias: bool, random: Random
-    ) -> PydanticFieldMeta:  # pragma: no cover
+    ) -> PydanticFieldMeta:
         """Create an instance from a pydantic field info.
 
         :param field_name: The name of the field.
         :param field_info: A pydantic FieldInfo instance.
         :param use_alias: Whether to use the field alias.
         :param random: A random.Random instance.
 
@@ -85,16 +67,14 @@
         name = field_info.alias if field_info.alias and use_alias else field_name
 
         annotation = unwrap_new_type(field_info.annotation)
 
         if is_optional_union(field_info.annotation):
             # pydantic v2 do not propagate metadata for Union types #[?]
             # hence we cannot acquire any constraints w/ straightforward approach
-            from pydantic.fields import FieldInfo
-
             field_info = FieldInfo.from_annotation(unwrap_optional(annotation))
 
         if metadata := [v for v in field_info.metadata if v is not None]:
             constraints = cls.parse_constraints(metadata=metadata)
         else:
             constraints = {}
 
@@ -107,15 +87,17 @@
             random=random,
             annotation=annotation,
             default=default_value,
             constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
         )
 
     @classmethod
-    def from_model_field(cls, model_field: ModelField, use_alias: bool) -> PydanticFieldMeta:  # pyright: ignore
+    def from_model_field(
+        cls, model_field: ModelField, use_alias: bool  # pyright: ignore
+    ) -> PydanticFieldMeta:  # pragma: no cover
         """Create an instance from a pydantic model field.
 
         :param model_field: A pydantic ModelField.
         :param use_alias: Whether to use the field alias.
 
         :returns: A PydanticFieldMeta instance.
 
@@ -128,17 +110,17 @@
         else:
             default_value = model_field.default if model_field.default is not Undefined else Null
 
         name = model_field.alias if model_field.alias and use_alias else model_field.name
 
         outer_type = unwrap_new_type(model_field.outer_type_)
         annotation = (
-            unwrap_new_type(model_field.annotation)
-            if not isinstance(model_field.annotation, DeferredType)
-            else model_field.outer_type_
+            model_field.outer_type_
+            if isinstance(model_field.annotation, DeferredType)
+            else unwrap_new_type(model_field.annotation)
         )
 
         constraints = cast(
             "Constraints",
             {
                 "constant": bool(model_field.field_info.const) or None,
                 "ge": getattr(outer_type, "ge", model_field.field_info.ge),
@@ -204,21 +186,21 @@
         super().__init_subclass__(*args, **kwargs)
 
         if not cls.__is_base_factory__ and hasattr(cls.__model__, "update_forward_refs"):
             with suppress(NameError):  # pragma: no cover
                 cls.__model__.update_forward_refs(**cls.__forward_ref_resolution_type_mapping__)
 
     @classmethod
-    def is_supported_type(cls, value: Any) -> "TypeGuard[type[T]]":
+    def is_supported_type(cls, value: Any) -> TypeGuard[type[T]]:
         """Determine whether the given value is supported by the factory.
 
         :param value: An arbitrary value.
         :returns: A typeguard
         """
-        return is_pydantic_model(value)
+        return is_safe_subclass(value, BaseModel)
 
     @classmethod
     def get_model_fields(cls) -> list["FieldMeta"]:
         """Retrieve a list of fields from the factory's model.
 
 
         :returns: A list of field MetaData instances.
@@ -229,16 +211,15 @@
                 cls._fields_metadata = [
                     PydanticFieldMeta.from_model_field(
                         field,
                         use_alias=not cls.__model__.__config__.allow_population_by_field_name,
                     )
                     for field in cls.__model__.__fields__.values()  # type: ignore[attr-defined]
                 ]
-            # FIXME: remove the pragma when switching to pydantic v2 permanently
-            else:  # pragma: no cover
+            else:
                 cls._fields_metadata = [
                     PydanticFieldMeta.from_field_info(
                         field_info=field_info,
                         field_name=field_name,
                         random=cls.__random__,
                         use_alias=not cls.__model__.model_config.get("populate_by_name", False),
                     )
```

### Comparing `polyfactory-2.4.0/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.5.0/polyfactory/factories/typed_dict_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,40 +12,35 @@
 
 class TypedDictFactory(Generic[TypedDictT], BaseFactory[TypedDictT]):
     """TypedDict base factory"""
 
     __is_base_factory__ = True
 
     @classmethod
-    def is_supported_type(cls, value: Any) -> "TypeGuard[type[TypedDictT]]":
+    def is_supported_type(cls, value: Any) -> TypeGuard[type[TypedDictT]]:
         """Determine whether the given value is supported by the factory.
 
         :param value: An arbitrary value.
         :returns: A typeguard
         """
-        try:
-            return is_typeddict(value)
-        except (TypeError, AttributeError):  # pragma: no cover
-            return False
+        return is_typeddict(value)
 
     @classmethod
     def get_model_fields(cls) -> list["FieldMeta"]:
         """Retrieve a list of fields from the factory's model.
 
 
         :returns: A list of field MetaData instances.
 
         """
-        fields_meta: list["FieldMeta"] = []
-
         model_type_hints = get_type_hints(cls.__model__, include_extras=True)
 
-        for field_name, annotation in model_type_hints.items():
-            fields_meta.append(
-                FieldMeta.from_type(
-                    annotation=annotation,
-                    random=cls.__random__,
-                    name=field_name,
-                    default=getattr(cls.__model__, field_name, Null),
-                )
+        fields_meta: list["FieldMeta"] = [
+            FieldMeta.from_type(
+                annotation=annotation,
+                random=cls.__random__,
+                name=field_name,
+                default=getattr(cls.__model__, field_name, Null),
             )
+            for field_name, annotation in model_type_hints.items()
+        ]
         return fields_meta
```

### Comparing `polyfactory-2.4.0/polyfactory/field_meta.py` & `polyfactory-2.5.0/polyfactory/field_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,16 +108,15 @@
         :param default: Default value, if any.
         :param constraints: A dictionary of constraints, if any.
 
         :returns: A field meta instance.
         """
         field_type = normalize_annotation(annotation, random=random)
 
-        # FIXME: remove the pragma when switching to pydantic v2 permanently
-        if not constraints and is_annotated(annotation):  # pragma: no cover
+        if not constraints and is_annotated(annotation):
             _, metadata = unwrap_annotated(annotation, random=random)
             constraints = cls.parse_constraints(metadata)
 
         field = cls(
             annotation=TYPE_MAPPING[field_type] if field_type in TYPE_MAPPING else field_type,
             random=random,
             name=name,
@@ -127,34 +126,33 @@
         )
         if field.type_args:
             field.children = [
                 FieldMeta.from_type(annotation=unwrap_new_type(arg), random=random) for arg in field.type_args
             ]
         return field
 
-    # FIXME: remove the pragma when switching to pydantic v2 permanently
     @classmethod
-    def parse_constraints(cls, metadata: list[Any]) -> "Constraints":  # pragma: no cover
+    def parse_constraints(cls, metadata: list[Any]) -> "Constraints":
         constraints = {}
 
         for value in metadata:
             if is_annotated(value):
                 _, inner_metadata = unwrap_annotated(value, random=DEFAULT_RANDOM)
                 constraints.update(cast("dict[str, Any]", cls.parse_constraints(metadata=inner_metadata)))
             elif func := getattr(value, "func", None):
                 if func is str.islower:
-                    constraints.update({"lower_case": True})
+                    constraints["lower_case"] = True
                 elif func is str.isupper:
-                    constraints.update({"upper_case": True})
+                    constraints["upper_case"] = True
                 elif func is str.isascii:
-                    constraints.update({"pattern": "[[:ascii:]]"})
+                    constraints["pattern"] = "[[:ascii:]]"
                 elif func is str.isdigit:
-                    constraints.update({"pattern": "[[:digit:]]"})
+                    constraints["pattern"] = "[[:digit:]]"
             elif is_dataclass(value) and (value_dict := asdict(value)) and ("allowed_schemes" in value_dict):
-                constraints.update({"url": {k: v for k, v in value_dict.items() if v is not None}})
+                constraints["url"] = {k: v for k, v in value_dict.items() if v is not None}
             else:
                 constraints.update(
                     {
                         k: v
                         for k, v in {
                             "allow_inf_nan": getattr(value, "allow_inf_nan", None),
                             "constant": getattr(value, "const", None) is not None,
```

### Comparing `polyfactory-2.4.0/polyfactory/fields.py` & `polyfactory-2.5.0/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/persistence.py` & `polyfactory-2.5.0/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/pytest_plugin.py` & `polyfactory-2.5.0/polyfactory/pytest_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 from __future__ import annotations
 
 import re
 from typing import (
-    TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Literal,
     Union,
 )
 
-from pytest import fixture
+from pytest import Config, fixture
 
 from polyfactory.exceptions import ParameterException
-
-if TYPE_CHECKING:
-    from pytest import Config  # nopycln: import
-
-    from polyfactory.factories.base import BaseFactory
-
+from polyfactory.factories.base import BaseFactory
+from polyfactory.utils.predicates import is_safe_subclass
 
 Scope = Union[
     Literal["session", "package", "module", "class", "function"],
-    Callable[[str, "Config"], Literal["session", "package", "module", "class", "function"]],
+    Callable[[str, Config], Literal["session", "package", "module", "class", "function"]],
 ]
 
 
 split_pattern_1 = re.compile(r"([A-Z]+)([A-Z][a-z])")
 split_pattern_2 = re.compile(r"([a-z\d])([A-Z])")
 
 
@@ -64,17 +59,15 @@
         :param name: Fixture name
         """
         self.scope = scope
         self.autouse = autouse
         self.name = name
 
     def __call__(self, factory: type[BaseFactory[Any]]) -> Any:
-        from polyfactory.factories.base import is_factory
-
-        if not is_factory(factory):
+        if not is_safe_subclass(factory, BaseFactory):
             raise ParameterException(f"{factory.__name__} is not a BaseFactory subclass.")
 
         fixture_name = self.name or _get_fixture_name(factory.__name__)
         fixture_register = fixture(scope=self.scope, name=fixture_name, autouse=self.autouse)  # pyright: ignore
 
         def _factory_fixture() -> type[BaseFactory[Any]]:
             """The wrapped factory"""
```

### Comparing `polyfactory-2.4.0/polyfactory/utils/helpers.py` & `polyfactory-2.5.0/polyfactory/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,15 @@
     :returns: A tuple of type args.
 
     """
     args = [arg for arg in get_args(annotation) if arg is not None]
     return unwrap_annotation(args[0], random=random), args[1:]
 
 
-# FIXME: remove the pragma when switching to pydantic v2 permanently
-def normalize_annotation(annotation: Any, random: Random) -> Any:  # pragma: no cover
+def normalize_annotation(annotation: Any, random: Random) -> Any:
     """Normalize an annotation.
 
     :param annotation: A type annotation.
 
     :returns: A normalized type annotation.
 
     """
```

### Comparing `polyfactory-2.4.0/polyfactory/utils/predicates.py` & `polyfactory-2.5.0/polyfactory/utils/predicates.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,27 +24,27 @@
     UNION_TYPES = {Union}
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
-def is_safe_subclass(annotation: Any, super_class: type[T]) -> "TypeGuard[type[T]]":
+def is_safe_subclass(annotation: Any, class_or_tuple: type[T] | tuple[type[T], ...]) -> "TypeGuard[type[T]]":
     """Determine whether a given annotation is a subclass of a give type
 
     :param annotation: A type annotation.
-    :param super_class: A potential super class.
+    :param class_or_tuple: A potential super class or classes.
 
     :returns: A typeguard
     """
     origin = get_type_origin(annotation)
     if not origin and not isclass(annotation):
         return False
     try:
-        return issubclass(origin or annotation, super_class)
+        return issubclass(origin or annotation, class_or_tuple)
     except TypeError:  # pragma: no cover
         return False
 
 
 def is_any(annotation: Any) -> "TypeGuard[Any]":
     """Determine whether a given annotation is 'typing.Any'.
 
@@ -122,10 +122,8 @@
     :param annotation: A type annotation.
 
     :returns: A type annotation.
     """
     origin = get_origin(annotation)
     if origin in (Annotated, Required, NotRequired):
         origin = get_args(annotation)[0]
-    if mapped_type := TYPE_MAPPING.get(origin):  # pyright: ignore
-        return mapped_type
-    return origin
+    return mapped_type if (mapped_type := TYPE_MAPPING.get(origin)) else origin
```

### Comparing `polyfactory-2.4.0/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.5.0/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.5.0/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.5.0/polyfactory/value_generators/constrained_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,17 +185,15 @@
     minimum, maximum = get_value_or_none(lt=lt, le=le, gt=gt, ge=ge, t_type=t_type)
 
     if minimum is not None and maximum is not None and maximum < minimum:
         raise ParameterException("maximum value must be greater than minimum value")
 
     if multiple_of is None:
         if minimum is not None and maximum is None:
-            if minimum == 0:
-                return minimum, seed  # pyright: ignore
-            return minimum, minimum + seed
+            return (minimum, seed) if minimum == 0 else (minimum, minimum + seed)  # pyright: ignore
         if maximum is not None and minimum is None:
             return maximum - seed, maximum
     else:
         if multiple_of == 0.0:
             raise ParameterException("multiple_of can not be zero")
         if (
             minimum is not None
@@ -220,26 +218,24 @@
     :param minimum: A minimum value.
     :param maximum: A maximum value.
     :param multiple_of: A multiple of value.
     :param method: A function that generates numbers of type T.
 
     :returns: A value of type T.
     """
-    if minimum is not None and maximum is not None:
-        if multiple_of is None:
-            return method(random=random, minimum=minimum, maximum=maximum)
-        if multiple_of >= minimum:
-            return multiple_of
-        result = minimum
-        while not passes_pydantic_multiple_validator(result, multiple_of):
-            result = round(method(random=random, minimum=minimum, maximum=maximum) / multiple_of) * multiple_of
-        return result
-    if multiple_of is not None:
+    if minimum is None or maximum is None:
+        return multiple_of if multiple_of is not None else method(random=random)
+    if multiple_of is None:
+        return method(random=random, minimum=minimum, maximum=maximum)
+    if multiple_of >= minimum:
         return multiple_of
-    return method(random=random)
+    result = minimum
+    while not passes_pydantic_multiple_validator(result, multiple_of):
+        result = round(method(random=random, minimum=minimum, maximum=maximum) / multiple_of) * multiple_of
+    return result
 
 
 def handle_constrained_int(
     random: Random,
     multiple_of: int | None = None,
     gt: int | None = None,
     ge: int | None = None,
@@ -344,28 +340,28 @@
 
     """
     string_number = str(generated_decimal)
     sign = "-" if "-" in string_number else "+"
     string_number = string_number.replace("-", "")
     whole_numbers, decimals = string_number.split(".")
 
-    if max_digits is not None and decimal_places is not None:
-        if len(whole_numbers) + decimal_places > max_digits:
-            # max digits determines decimal length
-            max_decimals = max_digits - len(whole_numbers)
-        else:
-            # decimal places determines max decimal length
-            max_decimals = decimal_places
-    elif max_digits is not None:
+    if (
+        max_digits is not None
+        and decimal_places is not None
+        and len(whole_numbers) + decimal_places > max_digits
+        or (max_digits is None or decimal_places is None)
+        and max_digits is not None
+    ):
         max_decimals = max_digits - len(whole_numbers)
+    elif max_digits is not None:
+        max_decimals = decimal_places  # type: ignore[assignment]
     else:
         max_decimals = cast("int", decimal_places)
 
-    if max_decimals < 0:
-        # in this case there are fewer digits than the len of whole_numbers
+    if max_decimals < 0:  # pyright: ignore
         return Decimal(sign + whole_numbers[:max_decimals])
 
     decimals = decimals[:max_decimals]
     return Decimal(sign + whole_numbers + "." + decimals[:decimal_places])
 
 
 def handle_constrained_decimal(
```

### Comparing `polyfactory-2.4.0/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.5.0/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.4.0/polyfactory/value_generators/primitives.py` & `polyfactory-2.5.0/polyfactory/value_generators/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     if lower_case:
         result = result.lower()
     elif upper_case:
         result = result.upper()
 
     if max_length and len(result) > max_length:
         end = random.randint(min_length or 0, max_length)
-        return result[0:end]
+        return result[:end]
 
     return result
 
 
 def create_random_string(
     random: Random,
     min_length: int | None = None,
```

### Comparing `polyfactory-2.4.0/polyfactory/value_generators/regex.py` & `polyfactory-2.5.0/polyfactory/value_generators/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,14 @@
         candidates = list(chain(*(self._handle_state(i) for i in value)))
         if candidates and candidates[0] is False:
             candidates = list(set(printable).difference(candidates[1:]))
             return self._random.choice(candidates)
         return self._random.choice(candidates)
 
     def _handle_repeat(self, start_range: int, end_range: Any, value: SubPattern) -> str:
-        result: list[str] = []
         end_range = min(end_range, self._limit)
 
-        for _ in range(self._random.randint(start_range, max(start_range, end_range))):
-            result.append("".join(self._handle_state(v) for v in list(value)))  # pyright:ignore
-
+        result = [
+            "".join(self._handle_state(v) for v in list(value))  # pyright: ignore
+            for _ in range(self._random.randint(start_range, max(start_range, end_range)))
+        ]
         return "".join(result)
```

### Comparing `polyfactory-2.4.0/pyproject.toml` & `polyfactory-2.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.4.0"
+version = "2.5.0"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
@@ -13,15 +13,15 @@
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
 license = "MIT"
-readme = "README.md"
+readme = "docs/PYPI_README.md"
 homepage = "https://github.com/litestar-org/polyfactory"
 repository = "https://github.com/litestar-org/polyfactory"
 documentation = "https://github.com/litestar-org/polyfactory"
 keywords = [
     "beanie",
     "dataclasses",
     "factory",
@@ -56,23 +56,19 @@
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 packages = [{ include = "polyfactory" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-beanie = { version = "*", optional = true, extras = ["beanie"] }
+beanie = { version = "*", optional = true }
 faker = "*"
-msgspec = { version = "*", optional = true, extras = ["msgspec"] }
-odmantic = { version = "*", optional = true, extras = ["odmantic"] }
-pydantic = { version = "*", optional = true, extras = [
-    "pydantic",
-    "odmantic",
-    "beanie",
-] }
+msgspec = { version = "*", optional = true }
+odmantic = { version = "*", optional = true }
+pydantic = { version = "*", optional = true }
 typing-extensions = "*"
 
 [tool.poetry.group.dev.dependencies]
 beanie = "*"
 email-validator = "*"
 hypothesis = "*"
 mongomock-motor = "*"
@@ -112,77 +108,83 @@
 include = ["polyfactory", "tests", "examples"]
 
 [tool.coverage.run]
 omit = ["*/tests/*"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
+filterwarnings = [
+    "ignore:.*pkg_resources.declare_namespace\\('sphinxcontrib'\\).*:DeprecationWarning",
+    "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
+    # Get rid those above once sphinxcontrib-mermaid doesn't use pkg_resources anymore
+    # https://github.com/mgaitan/sphinxcontrib-mermaid/issues/119
+]
 
 [tool.coverage.report]
 exclude_lines = [
     'pragma: no cover',
     'if TYPE_CHECKING:',
     'except ImportError:',
     'except ImportError as e:',
     '\.\.\.',
 ]
 
 [tool.ruff]
 select = [
-    "A",   # flake8-builtins
-    "B",   # flake8-bugbear
+    "A", # flake8-builtins
+    "B", # flake8-bugbear
     "BLE", # flake8-blind-except
-    "C4",  # flake8-comprehensions
-    "D",   # pydocstyle
-    "DJ",  # flake8-django
+    "C4", # flake8-comprehensions
+    "D", # pydocstyle
+    "DJ", # flake8-django
     "DTZ", # flake8-datetimez
-    "E",   # pycodestyle errors
+    "E", # pycodestyle errors
     "ERA", # eradicate
     "EXE", # flake8-executable
-    "F",   # pyflakes
-    "G",   # flake8-logging-format
-    "I",   # isort
+    "F", # pyflakes
+    "G", # flake8-logging-format
+    "I", # isort
     "ICN", # flake8-import-conventions
     "ISC", # flake8-implicit-str-concat
-    "N",   # pep8-naming
+    "N", # pep8-naming
     "PIE", # flake8-pie
     "PLC", # pylint - convention
     "PLE", # pylint - error
     "PLW", # pylint - warning
     "PTH", # flake8-use-pathlib
-    "Q",   # flake8-quotes
+    "Q", # flake8-quotes
     "RET", # flake8-return
     "RUF", # Ruff-specific rules
-    "S",   # flake8-bandit
+    "S", # flake8-bandit
     "SIM", # flake8-simplify
     "T10", # flake8-debugger
     "T20", # flake8-print
     "TCH", # flake8-type-checking
     "TID", # flake8-tidy-imports
-    "UP",  # pyupgrade
-    "W",   # pycodestyle - warning
+    "UP", # pyupgrade
+    "W", # pycodestyle - warning
     "YTT", # flake8-2020
 ]
 
 ignore = [
-    "A003",  # flake8-builtins - class attribute {name} is shadowing a python builtin
-    "B010",  # flake8-bugbear - do not call setattr with a constant attribute value
-    "D100",  # pydocstyle - missing docstring in public module
-    "D101",  # pydocstyle - missing docstring in public class
-    "D102",  # pydocstyle - missing docstring in public method
-    "D103",  # pydocstyle - missing docstring in public function
-    "D104",  # pydocstyle - missing docstring in public package
-    "D105",  # pydocstyle - missing docstring in magic method
-    "D106",  # pydocstyle - missing docstring in public nested class
-    "D107",  # pydocstyle - missing docstring in __init__
-    "D202",  # pydocstyle - no blank lines allowed after function docstring
-    "D205",  # pydocstyle - 1 blank line required between summary line and description
-    "D415",  # pydocstyle - first line should end with a period, question mark, or exclamation point
-    "E501",  # pycodestyle line too long, handled by black
-    "N818",  # pep8-naming - exception name should be named with an Error suffix
+    "A003", # flake8-builtins - class attribute {name} is shadowing a python builtin
+    "B010", # flake8-bugbear - do not call setattr with a constant attribute value
+    "D100", # pydocstyle - missing docstring in public module
+    "D101", # pydocstyle - missing docstring in public class
+    "D102", # pydocstyle - missing docstring in public method
+    "D103", # pydocstyle - missing docstring in public function
+    "D104", # pydocstyle - missing docstring in public package
+    "D105", # pydocstyle - missing docstring in magic method
+    "D106", # pydocstyle - missing docstring in public nested class
+    "D107", # pydocstyle - missing docstring in __init__
+    "D202", # pydocstyle - no blank lines allowed after function docstring
+    "D205", # pydocstyle - 1 blank line required between summary line and description
+    "D415", # pydocstyle - first line should end with a period, question mark, or exclamation point
+    "E501", # pycodestyle line too long, handled by black
+    "N818", # pep8-naming - exception name should be named with an Error suffix
     "UP037", # pyupgrade - removes quotes from type annotation
 ]
 line-length = 120
 src = ["polyfactory", "tests", "docs/examples"]
 target-version = "py38"
 
 [tool.ruff.pydocstyle]
```

