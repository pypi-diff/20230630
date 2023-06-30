# Comparing `tmp/beavers-0.0.1rc0.tar.gz` & `tmp/beavers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beavers-0.0.1rc0.tar", max compression
+gzip compressed data, was "beavers-0.0.2.tar", max compression
```

## Comparing `beavers-0.0.1rc0.tar` & `beavers-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-05-09 16:24:59.768622 beavers-0.0.1rc0/LICENSE
--rw-r--r--   0        0        0     2986 2023-05-09 16:24:59.768622 beavers-0.0.1rc0/README.md
--rw-r--r--   0        0        0        0 2023-05-09 16:24:59.768622 beavers-0.0.1rc0/beavers/__init__.py
--rw-r--r--   0        0        0    12715 2023-05-09 16:24:59.768622 beavers-0.0.1rc0/beavers/engine.py
--rw-r--r--   0        0        0     1639 2023-05-09 16:25:21.120949 beavers-0.0.1rc0/pyproject.toml
--rw-r--r--   0        0        0     4142 1970-01-01 00:00:00.000000 beavers-0.0.1rc0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-30 10:34:01.950532 beavers-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2948 2023-06-30 10:34:01.950532 beavers-0.0.2/README.md
+-rw-r--r--   0        0        0      116 2023-06-30 10:34:22.162736 beavers-0.0.2/beavers/__init__.py
+-rw-r--r--   0        0        0    18570 2023-06-30 10:34:01.954532 beavers-0.0.2/beavers/engine.py
+-rw-r--r--   0        0        0     9235 2023-06-30 10:34:01.954532 beavers-0.0.2/beavers/replay.py
+-rw-r--r--   0        0        0     1657 2023-06-30 10:34:01.954532 beavers-0.0.2/beavers/testing.py
+-rw-r--r--   0        0        0     1877 2023-06-30 10:34:22.162736 beavers-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3800 1970-01-01 00:00:00.000000 beavers-0.0.2/PKG-INFO
```

### Comparing `beavers-0.0.1rc0/LICENSE` & `beavers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beavers-0.0.1rc0/README.md` & `beavers-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,55 @@
+
 [![PyPI Version][pypi-image]][pypi-url]
 [![Python Version][versions-image]][versions-url]
 [![Github Stars][stars-image]][stars-url]
 [![codecov][codecov-image]][codecov-url]
 [![Build Status][build-image]][build-url]
 [![Documentation][doc-image]][doc-url]
 [![License][license-image]][license-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Downloads][downloads-month-image]][downloads-month-url]
 [![Code style: black][codestyle-image]][codestyle-url]
-[![snyk][snyk-image]][snyk-url]
-
-
 
 # Beavers
 _____
 
-**Beavers** is a python library for stream processing, optimize for analytics. 
+**Beavers** is a python library for stream processing, optimized for analytics. 
 
 
 It is used at [Tradewell Technologies](https://www.tradewelltech.co/), 
 to calculate analytics and serve model predictions,
 in both realtime and batch jobs.
 
 # Key Features
 
 
-* Works in real time (eg: reading from kafka) and replay mode (eg: reading from parquet)
+* Works in **real time** (eg: reading from kafka) and **replay mode** (eg: reading from parquet)
 * Optimized for analytics, it uses micro-batching (instead of processing records one by one)
 * Similar to [incremental](https://github.com/janestreet/incremental), it  updates nodes in a dag incrementally
 * Taking inspiration from [kafka streams](https://www.confluent.io/blog/kafka-streams-tables-part-1-event-streaming/), there are two types of nodes in the dag:
   * Stream: ephemeral micro-batches of events (cleared after every cycle)
   * State: durable state derived from streams
-* Clear separation between the dag (which contains the business logic) and the IO (where the data comes from/goes). 
+* Clear separation between the business logic and the IO. 
   So the same dag can be used in real time mode, replay mode or can be easily tested.
-
+* functional interface (no inheritance required)
 
 [pypi-image]: https://img.shields.io/pypi/v/beavers
 [pypi-url]: https://pypi.org/project/beavers/
 [build-image]: https://github.com/tradewelltech/beavers/actions/workflows/ci.yaml/badge.svg
 [build-url]: https://github.com/tradewelltech/beavers/actions/workflows/ci.yaml
 [stars-image]: https://img.shields.io/github/stars/tradewelltech/beavers
 [stars-url]: https://github.com/tradewelltech/beavers
 [versions-image]: https://img.shields.io/pypi/pyversions/beavers
 [versions-url]: https://pypi.org/project/beavers/
 [doc-image]: https://readthedocs.org/projects/beavers/badge/?version=latest
 [doc-url]: https://beavers.readthedocs.io/en/latest/?badge=latest
 [license-image]: http://img.shields.io/:license-Apache%202-blue.svg
-[license-url]: https://github.com/tradewelltech/beavers/blob/master/LICENSE
-[codecov-image]: https://codecov.io/gh/tradewelltech/beavers/branch/master/graph/badge.svg?token=XMFH27IL70
+[license-url]: https://github.com/tradewelltech/beavers/blob/main/LICENSE
+[codecov-image]: https://codecov.io/gh/tradewelltech/beavers/branch/main/graph/badge.svg?token=GY6KL7NT1Q
 [codecov-url]: https://codecov.io/gh/tradewelltech/beavers
 [downloads-image]: https://pepy.tech/badge/beavers
 [downloads-url]: https://static.pepy.tech/badge/beavers
 [downloads-month-image]: https://pepy.tech/badge/beavers/month
 [downloads-month-url]: https://static.pepy.tech/badge/beavers/month
 [codestyle-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [codestyle-url]: https://github.com/ambv/black
```

### Comparing `beavers-0.0.1rc0/pyproject.toml` & `beavers-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 
 [tool.poetry]
 name = "beavers"
-version = "0.0.1rc0"
+version = "0.0.2"
 description = "Python stream processing"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "beavers" }
 ]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/tradewelltech/beavers"
 documentation = "https://beavers.readthedocs.io/en/latest/"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 keywords = ["apache-arrow", "streaming", "data"]
 
 [tool.poetry.dependencies]
 pandas = ">1.4.0"
-python = ">=3.8,<3.12"
+python = ">=3.10,<3.12"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 coverage = ">=6.5.0"
 flake8 = ">=5.0.4"
 isort = ">=5.10.1"
 mkdocs = ">=1.4.2"
 pip-tools = "^6.12.1"
 pre-commit = ">=2.20.0"
 pylint = ">=2.15.0"
 pytest = ">=7.2.0"
-mkdocs-material = "^9.0.3"
+mkdocs-material = ">=9.0.3"
+mkdocstrings = { version = ">=0.21.2", extras = ['python'] }
+
+[tool.poetry.group.docs.dependencies]
+markdown-include = "*"
+mkdocs = "*"
+mkdocs-material = "*"
+mkdocs-material-extensions = "*"
+mkdocstrings = {version = "*", extras = ['python']}
+pymdown-extensions = "*"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
@@ -62,7 +69,10 @@
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["*/__init__.py"]
 folders = [ {path = "beavers"}]
 
 [tool.ruff]
 line-length = 88
+
+[tool.pydocstyle]
+ignore = ["D102", "D107", "D203", "D212"]
```

### Comparing `beavers-0.0.1rc0/PKG-INFO` & `beavers-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,78 @@
 Metadata-Version: 2.1
 Name: beavers
-Version: 0.0.1rc0
+Version: 0.0.2
 Summary: Python stream processing
 Home-page: https://github.com/tradewelltech/beavers
 License: Apache-2.0
 Keywords: apache-arrow,streaming,data
 Author: Tradewell Tech
 Author-email: engineering@tradewelltech.co
 Maintainer: 0x26res
 Maintainer-email: 0x26res@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: pandas (>1.4.0)
 Project-URL: Documentation, https://beavers.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/tradewelltech/beavers
 Description-Content-Type: text/markdown
 
+
 [![PyPI Version][pypi-image]][pypi-url]
 [![Python Version][versions-image]][versions-url]
 [![Github Stars][stars-image]][stars-url]
 [![codecov][codecov-image]][codecov-url]
 [![Build Status][build-image]][build-url]
 [![Documentation][doc-image]][doc-url]
 [![License][license-image]][license-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Downloads][downloads-month-image]][downloads-month-url]
 [![Code style: black][codestyle-image]][codestyle-url]
-[![snyk][snyk-image]][snyk-url]
-
-
 
 # Beavers
 _____
 
-**Beavers** is a python library for stream processing, optimize for analytics. 
+**Beavers** is a python library for stream processing, optimized for analytics. 
 
 
 It is used at [Tradewell Technologies](https://www.tradewelltech.co/), 
 to calculate analytics and serve model predictions,
 in both realtime and batch jobs.
 
 # Key Features
 
 
-* Works in real time (eg: reading from kafka) and replay mode (eg: reading from parquet)
+* Works in **real time** (eg: reading from kafka) and **replay mode** (eg: reading from parquet)
 * Optimized for analytics, it uses micro-batching (instead of processing records one by one)
 * Similar to [incremental](https://github.com/janestreet/incremental), it  updates nodes in a dag incrementally
 * Taking inspiration from [kafka streams](https://www.confluent.io/blog/kafka-streams-tables-part-1-event-streaming/), there are two types of nodes in the dag:
   * Stream: ephemeral micro-batches of events (cleared after every cycle)
   * State: durable state derived from streams
-* Clear separation between the dag (which contains the business logic) and the IO (where the data comes from/goes). 
+* Clear separation between the business logic and the IO. 
   So the same dag can be used in real time mode, replay mode or can be easily tested.
-
+* functional interface (no inheritance required)
 
 [pypi-image]: https://img.shields.io/pypi/v/beavers
 [pypi-url]: https://pypi.org/project/beavers/
 [build-image]: https://github.com/tradewelltech/beavers/actions/workflows/ci.yaml/badge.svg
 [build-url]: https://github.com/tradewelltech/beavers/actions/workflows/ci.yaml
 [stars-image]: https://img.shields.io/github/stars/tradewelltech/beavers
 [stars-url]: https://github.com/tradewelltech/beavers
 [versions-image]: https://img.shields.io/pypi/pyversions/beavers
 [versions-url]: https://pypi.org/project/beavers/
 [doc-image]: https://readthedocs.org/projects/beavers/badge/?version=latest
 [doc-url]: https://beavers.readthedocs.io/en/latest/?badge=latest
 [license-image]: http://img.shields.io/:license-Apache%202-blue.svg
-[license-url]: https://github.com/tradewelltech/beavers/blob/master/LICENSE
-[codecov-image]: https://codecov.io/gh/tradewelltech/beavers/branch/master/graph/badge.svg?token=XMFH27IL70
+[license-url]: https://github.com/tradewelltech/beavers/blob/main/LICENSE
+[codecov-image]: https://codecov.io/gh/tradewelltech/beavers/branch/main/graph/badge.svg?token=GY6KL7NT1Q
 [codecov-url]: https://codecov.io/gh/tradewelltech/beavers
 [downloads-image]: https://pepy.tech/badge/beavers
 [downloads-url]: https://static.pepy.tech/badge/beavers
 [downloads-month-image]: https://pepy.tech/badge/beavers/month
 [downloads-month-url]: https://static.pepy.tech/badge/beavers/month
 [codestyle-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [codestyle-url]: https://github.com/ambv/black
```

