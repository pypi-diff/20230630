# Comparing `tmp/minilog-2.2.tar.gz` & `tmp/minilog-2.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minilog-2.2.tar", max compression
+gzip compressed data, was "minilog-2.2b1.tar", max compression
```

## Comparing `minilog-2.2.tar` & `minilog-2.2b1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1088 2018-03-03 02:40:31.000000 minilog-2.2/LICENSE.md
--rw-r--r--   0        0        0     1997 2022-03-07 13:41:26.747503 minilog-2.2/README.md
--rw-r--r--   0        0        0      223 2022-03-07 13:39:41.102054 minilog-2.2/log/__init__.py
--rw-r--r--   0        0        0      741 2020-02-15 16:25:02.000000 minilog-2.2/log/filters.py
--rw-r--r--   0        0        0     1813 2022-03-07 13:39:41.102743 minilog-2.2/log/helpers.py
--rw-r--r--   0        0        0      892 2022-03-07 13:39:41.103237 minilog-2.2/log/logger.py
--rw-r--r--   0        0        0        0 2023-06-29 23:30:18.877396 minilog-2.2/log/py.typed
--rw-r--r--   0        0        0      101 2022-03-07 13:39:41.103657 minilog-2.2/log/settings.py
--rw-r--r--   0        0        0       72 2022-06-19 19:08:23.154866 minilog-2.2/log/state.py
--rw-r--r--   0        0        0       34 2018-03-03 02:40:31.000000 minilog-2.2/log/tests/__init__.py
--rw-r--r--   0        0        0      291 2022-03-07 13:39:41.105263 minilog-2.2/log/tests/conftest.py
--rw-r--r--   0        0        0      697 2022-03-07 13:39:41.105813 minilog-2.2/log/tests/test_api.py
--rw-r--r--   0        0        0     1426 2022-03-07 13:39:41.106375 minilog-2.2/log/tests/test_helpers.py
--rw-r--r--   0        0        0      368 2022-03-07 13:39:41.107035 minilog-2.2/log/tests/test_logger.py
--rw-r--r--   0        0        0     1609 2022-03-07 13:41:26.748844 minilog-2.2/log/tests/test_utils.py
--rw-r--r--   0        0        0     1834 2022-06-19 19:10:39.285791 minilog-2.2/log/utils.py
--rw-r--r--   0        0        0     2062 2023-06-29 23:52:30.754482 minilog-2.2/pyproject.toml
--rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 minilog-2.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2018-03-03 02:40:31.000000 minilog-2.2b1/LICENSE.md
+-rw-r--r--   0        0        0     1997 2022-03-07 13:41:26.747503 minilog-2.2b1/README.md
+-rw-r--r--   0        0        0      223 2022-03-07 13:39:41.102054 minilog-2.2b1/log/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-15 16:25:02.000000 minilog-2.2b1/log/filters.py
+-rw-r--r--   0        0        0     1813 2022-03-07 13:39:41.102743 minilog-2.2b1/log/helpers.py
+-rw-r--r--   0        0        0      892 2022-03-07 13:39:41.103237 minilog-2.2b1/log/logger.py
+-rw-r--r--   0        0        0      101 2022-03-07 13:39:41.103657 minilog-2.2b1/log/settings.py
+-rw-r--r--   0        0        0       72 2022-06-19 19:08:23.154866 minilog-2.2b1/log/state.py
+-rw-r--r--   0        0        0       34 2018-03-03 02:40:31.000000 minilog-2.2b1/log/tests/__init__.py
+-rw-r--r--   0        0        0      291 2022-03-07 13:39:41.105263 minilog-2.2b1/log/tests/conftest.py
+-rw-r--r--   0        0        0      697 2022-03-07 13:39:41.105813 minilog-2.2b1/log/tests/test_api.py
+-rw-r--r--   0        0        0     1426 2022-03-07 13:39:41.106375 minilog-2.2b1/log/tests/test_helpers.py
+-rw-r--r--   0        0        0      368 2022-03-07 13:39:41.107035 minilog-2.2b1/log/tests/test_logger.py
+-rw-r--r--   0        0        0     1609 2022-03-07 13:41:26.748844 minilog-2.2b1/log/tests/test_utils.py
+-rw-r--r--   0        0        0     1834 2022-06-19 19:10:39.285791 minilog-2.2b1/log/utils.py
+-rw-r--r--   0        0        0     2064 2022-11-23 14:30:35.814791 minilog-2.2b1/pyproject.toml
+-rw-r--r--   0        0        0     2634 2022-11-23 14:38:09.897711 minilog-2.2b1/setup.py
+-rw-r--r--   0        0        0     2987 2022-11-23 14:38:09.897970 minilog-2.2b1/PKG-INFO
```

### Comparing `minilog-2.2/LICENSE.md` & `minilog-2.2b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `minilog-2.2/README.md` & `minilog-2.2b1/README.md`

 * *Files identical despite different names*

### Comparing `minilog-2.2/log/filters.py` & `minilog-2.2b1/log/filters.py`

 * *Files identical despite different names*

### Comparing `minilog-2.2/log/helpers.py` & `minilog-2.2b1/log/helpers.py`

 * *Files identical despite different names*

### Comparing `minilog-2.2/log/logger.py` & `minilog-2.2b1/log/logger.py`

 * *Files identical despite different names*

### Comparing `minilog-2.2/log/tests/test_api.py` & `minilog-2.2b1/log/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `minilog-2.2/log/tests/test_helpers.py` & `minilog-2.2b1/log/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `minilog-2.2/log/tests/test_utils.py` & `minilog-2.2b1/log/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `minilog-2.2/log/utils.py` & `minilog-2.2b1/log/utils.py`

 * *Files identical despite different names*

### Comparing `minilog-2.2/pyproject.toml` & `minilog-2.2b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "minilog"
-version = "2.2"
+version = "2.2b1"
 description = "Minimalistic wrapper for Python logging."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -38,25 +38,25 @@
 [tool.poetry.dev-dependencies]
 
 # Formatters
 black = "^22.1"
 isort = "^5.10"
 
 # Linters
-pylint = "~2.15"
+pylint = "~2.6.0"
 pydocstyle = "*"
-mypy = "^1.3"
+mypy = "~0.931"
 types-freezegun = "*"
 
 # Testing
 pytest = "^7.2"
 pytest-describe = "^2.0"
 pytest-expecter = "^3.0"
 pytest-ordering = "*"
-pytest-cov = "^4.1"
+pytest-cov = "*"
 pytest-repeat = "*"
 pytest-profiling = "*"
 freezegun = "*"
 
 # Reports
 coveragespace = "^6.0.1"
```

### Comparing `minilog-2.2/PKG-INFO` & `minilog-2.2b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: minilog
-Version: 2.2
+Version: 2.2b1
 Summary: Minimalistic wrapper for Python logging.
 Home-page: https://pypi.org/project/minilog
 License: MIT
 Keywords: logging
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Logging
 Project-URL: Documentation, https://minilog.readthedocs.io
 Project-URL: Repository, https://github.com/jacebrowning/minilog
 Description-Content-Type: text/markdown
 
 # minilog
```

