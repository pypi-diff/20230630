# Comparing `tmp/fa-models-1.0.48.tar.gz` & `tmp/fa-models-1.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.48.tar", last modified: Fri Jun 30 11:40:06 2023, max compression
+gzip compressed data, was "fa-models-1.0.49.tar", last modified: Fri Jun 30 11:41:36 2023, max compression
```

## Comparing `fa-models-1.0.48.tar` & `fa-models-1.0.49.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:40:06.195348 fa-models-1.0.48/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-30 11:40:06.195348 fa-models-1.0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-30 11:39:36.000000 fa-models-1.0.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:40:06.191348 fa-models-1.0.48/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-30 11:40:06.000000 fa-models-1.0.48/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-30 11:40:06.000000 fa-models-1.0.48/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:40:06.000000 fa-models-1.0.48/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 11:40:06.000000 fa-models-1.0.48/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 11:40:06.000000 fa-models-1.0.48/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:40:06.191348 fa-models-1.0.48/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:40:06.195348 fa-models-1.0.48/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/exchange_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/fund.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/signal_supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/state_of_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/state_of_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-30 11:39:36.000000 fa-models-1.0.48/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-30 11:39:58.000000 fa-models-1.0.48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 11:40:06.195348 fa-models-1.0.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-30 11:39:36.000000 fa-models-1.0.48/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:40:06.195348 fa-models-1.0.48/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-30 11:39:36.000000 fa-models-1.0.48/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-30 11:39:36.000000 fa-models-1.0.48/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:41:36.489804 fa-models-1.0.49/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-30 11:41:36.485804 fa-models-1.0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-30 11:41:08.000000 fa-models-1.0.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:41:36.485804 fa-models-1.0.49/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-30 11:41:36.000000 fa-models-1.0.49/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-30 11:41:36.000000 fa-models-1.0.49/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:41:36.000000 fa-models-1.0.49/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 11:41:36.000000 fa-models-1.0.49/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 11:41:36.000000 fa-models-1.0.49/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:41:36.485804 fa-models-1.0.49/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:41:36.485804 fa-models-1.0.49/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/exchange_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/fund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/signal_supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/state_of_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/state_of_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-30 11:41:08.000000 fa-models-1.0.49/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-30 11:41:28.000000 fa-models-1.0.49/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 11:41:36.489804 fa-models-1.0.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-30 11:41:08.000000 fa-models-1.0.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:41:36.485804 fa-models-1.0.49/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-30 11:41:08.000000 fa-models-1.0.49/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-30 11:41:08.000000 fa-models-1.0.49/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.48/PKG-INFO` & `fa-models-1.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.48
+Version: 1.0.49
 Summary: The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.48/README.md` & `fa-models-1.0.49/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.49/fa_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.48
+Version: 1.0.49
 Summary: The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.48/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.49/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/algorithm.py` & `fa-models-1.0.49/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/exchange_key.py` & `fa-models-1.0.49/famodels/models/exchange_key.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/fund.py` & `fa-models-1.0.49/famodels/models/fund.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/investor.py` & `fa-models-1.0.49/famodels/models/investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/order.py` & `fa-models-1.0.49/famodels/models/order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/person.py` & `fa-models-1.0.49/famodels/models/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/processed_signal.py` & `fa-models-1.0.49/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/signal_supplier.py` & `fa-models-1.0.49/famodels/models/signal_supplier.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/state_of_trade.py` & `fa-models-1.0.49/famodels/models/state_of_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/subscription.py` & `fa-models-1.0.49/famodels/models/subscription.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/trade.py` & `fa-models-1.0.49/famodels/models/trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/trading_signal.py` & `fa-models-1.0.49/famodels/models/trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/famodels/models/virtual_order.py` & `fa-models-1.0.49/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/pyproject.toml` & `fa-models-1.0.49/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.48"
+version = "1.0.49"
 description = "The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.48"
+current_version = "1.0.49"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.48/setup.py` & `fa-models-1.0.49/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/tests/test_investor.py` & `fa-models-1.0.49/tests/test_investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.48/tests/test_processed_trading_signal.py` & `fa-models-1.0.49/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

