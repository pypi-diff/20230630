# Comparing `tmp/pytest-reportportal-5.1.9.tar.gz` & `tmp/pytest-reportportal-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reportportal-5.1.9.tar", last modified: Thu Jun  8 11:22:11 2023, max compression
+gzip compressed data, was "pytest-reportportal-5.2.0.tar", last modified: Fri Jun 30 15:46:24 2023, max compression
```

## Comparing `pytest-reportportal-5.1.9.tar` & `pytest-reportportal-5.2.0.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/pytest_reportportal/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/rp_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    31902 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/service.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:24.405342 pytest-reportportal-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-30 15:46:24.405342 pytest-reportportal-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:24.405342 pytest-reportportal-5.2.0/pytest_reportportal/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/pytest_reportportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/pytest_reportportal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/pytest_reportportal/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/pytest_reportportal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/pytest_reportportal/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/pytest_reportportal/rp_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32523 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/pytest_reportportal/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:24.405342 pytest-reportportal-5.2.0/pytest_reportportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-30 15:46:24.000000 pytest-reportportal-5.2.0/pytest_reportportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-30 15:46:24.000000 pytest-reportportal-5.2.0/pytest_reportportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:46:24.000000 pytest-reportportal-5.2.0/pytest_reportportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 15:46:24.000000 pytest-reportportal-5.2.0/pytest_reportportal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 15:46:24.000000 pytest-reportportal-5.2.0/pytest_reportportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 15:46:24.000000 pytest-reportportal-5.2.0/pytest_reportportal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-30 15:46:24.405342 pytest-reportportal-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-30 15:46:19.000000 pytest-reportportal-5.2.0/setup.py
```

### Comparing `pytest-reportportal-5.1.9/CONTRIBUTING.rst` & `pytest-reportportal-5.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.9/LICENSE` & `pytest-reportportal-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.9/PKG-INFO` & `pytest-reportportal-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-reportportal
-Version: 5.1.9
+Version: 5.2.0
 Summary: Agent for Reporting results of tests to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-pytest
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,pytest,agent
 Classifier: Framework :: Pytest
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 agent-python-pytest
 ===================
 
@@ -99,33 +98,35 @@
 - The :code:`rp_api_key` can also be set with the environment variable `RP_API_KEY`. This will override the value set for :code:`rp_api_key` in pytest.ini
 
 The following parameters are optional:
 
 - :code:`rp_launch = AnyLaunchName` - launch name (could be overridden by pytest --rp-launch option, default value is 'Pytest Launch').
 - :code:`rp_launch_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing launch (the session will not handle the lifecycle of the given launch).
 - :code:`rp_launch_attributes = 'PyTest' 'Smoke' 'Env:Python3'` - list of attributes for launch.
+- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden by pytest --rp-launch-description option, default value is '').
+- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day).
+- :code:`rp_launch_uuid_print = True` - Enables printing Launch UUID on test run start. Default `False`.
+- :code:`rp_launch_uuid_print_output = stderr` - Launch UUID print output. Default `stdout`. Possible values: [stderr, stdout].
 - :code:`rp_parent_item_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing test item for session to use as parent item for the tests (the session will not handle the lifecycle of the given test item).
 - :code:`rp_tests_attributes = 'PyTest' 'Smoke'` - list of attributes that will be added for each item in the launch.
-- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden by pytest --rp-launch-description option, default value is '').
 - :code:`rp_log_batch_size = 20` - size of batch log request.
 - :code:`rp_log_batch_payload_size = 65000000` - maximum payload size in bytes of async batch log requests.
 - :code:`rp_log_level = INFO` - The log level that will be reported.
 - :code:`rp_log_format = [%(levelname)7s] (%(name)s) %(message)s (%(filename)s:%(lineno)s)` - Format string to be used for logs sent to the service.
 - :code:`rp_ignore_attributes = 'xfail' 'usefixture'` - Ignore specified pytest markers.
-- :code:`rp_is_skipped_an_issue = False` - Treat skipped tests as required investigation. Default is True.
+- :code:`rp_is_skipped_an_issue = False` - Treat skipped tests as required investigation. Default `True`.
 - :code:`rp_hierarchy_dirs_level = 0` - Directory starting hierarchy level (from pytest.ini level) (default `0`).
 - :code:`rp_hierarchy_dirs = True` - Enables hierarchy for tests directories, default `False`. Doesn't support 'xdist' plugin.
 - :code:`rp_hierarchy_dir_path_separator` - Path separator to display directories in test hierarchy. In case of empty value current system path separator will be used (os.path.sep).
 - :code:`rp_hierarchy_code` - Enables hierarchy for inner classes and parametrized tests, default `False`. Doesn't support 'xdist' plugin.
 - :code:`rp_issue_system_url = https://bugzilla.some.com/show_bug.cgi?id={issue_id}` - issue URL (issue_id will be filled by parameter from pytest mark).
 - :code:`rp_issue_id_marks = True` - Enables adding marks for issue ids (e.g. "issue:123456").
 - :code:`rp_verify_ssl = True` - Verify SSL when connecting to the server.
 - :code:`rp_mode = DEFAULT` - DEBUG or DEFAULT launch mode. DEBUG launches are displayed in a separate tab and not visible to anyone except owner.
 - :code:`rp_thread_logging` - EXPERIMENTAL - Enables support for reporting logs from threads by patching the builtin Thread class. Use with caution.
-- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day).
 - :code:`rp_api_retries = 0` - Amount of retries for performing REST calls to RP server.
 
 
 
 If you like to override the above parameters from command line, or from CI environment based on your build, then pass
 - :code:`-o "rp_launch_attributes=Smoke Tests"` during invocation.
```

### Comparing `pytest-reportportal-5.1.9/README.rst` & `pytest-reportportal-5.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -80,33 +80,35 @@
 - The :code:`rp_api_key` can also be set with the environment variable `RP_API_KEY`. This will override the value set for :code:`rp_api_key` in pytest.ini
 
 The following parameters are optional:
 
 - :code:`rp_launch = AnyLaunchName` - launch name (could be overridden by pytest --rp-launch option, default value is 'Pytest Launch').
 - :code:`rp_launch_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing launch (the session will not handle the lifecycle of the given launch).
 - :code:`rp_launch_attributes = 'PyTest' 'Smoke' 'Env:Python3'` - list of attributes for launch.
+- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden by pytest --rp-launch-description option, default value is '').
+- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day).
+- :code:`rp_launch_uuid_print = True` - Enables printing Launch UUID on test run start. Default `False`.
+- :code:`rp_launch_uuid_print_output = stderr` - Launch UUID print output. Default `stdout`. Possible values: [stderr, stdout].
 - :code:`rp_parent_item_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing test item for session to use as parent item for the tests (the session will not handle the lifecycle of the given test item).
 - :code:`rp_tests_attributes = 'PyTest' 'Smoke'` - list of attributes that will be added for each item in the launch.
-- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden by pytest --rp-launch-description option, default value is '').
 - :code:`rp_log_batch_size = 20` - size of batch log request.
 - :code:`rp_log_batch_payload_size = 65000000` - maximum payload size in bytes of async batch log requests.
 - :code:`rp_log_level = INFO` - The log level that will be reported.
 - :code:`rp_log_format = [%(levelname)7s] (%(name)s) %(message)s (%(filename)s:%(lineno)s)` - Format string to be used for logs sent to the service.
 - :code:`rp_ignore_attributes = 'xfail' 'usefixture'` - Ignore specified pytest markers.
-- :code:`rp_is_skipped_an_issue = False` - Treat skipped tests as required investigation. Default is True.
+- :code:`rp_is_skipped_an_issue = False` - Treat skipped tests as required investigation. Default `True`.
 - :code:`rp_hierarchy_dirs_level = 0` - Directory starting hierarchy level (from pytest.ini level) (default `0`).
 - :code:`rp_hierarchy_dirs = True` - Enables hierarchy for tests directories, default `False`. Doesn't support 'xdist' plugin.
 - :code:`rp_hierarchy_dir_path_separator` - Path separator to display directories in test hierarchy. In case of empty value current system path separator will be used (os.path.sep).
 - :code:`rp_hierarchy_code` - Enables hierarchy for inner classes and parametrized tests, default `False`. Doesn't support 'xdist' plugin.
 - :code:`rp_issue_system_url = https://bugzilla.some.com/show_bug.cgi?id={issue_id}` - issue URL (issue_id will be filled by parameter from pytest mark).
 - :code:`rp_issue_id_marks = True` - Enables adding marks for issue ids (e.g. "issue:123456").
 - :code:`rp_verify_ssl = True` - Verify SSL when connecting to the server.
 - :code:`rp_mode = DEFAULT` - DEBUG or DEFAULT launch mode. DEBUG launches are displayed in a separate tab and not visible to anyone except owner.
 - :code:`rp_thread_logging` - EXPERIMENTAL - Enables support for reporting logs from threads by patching the builtin Thread class. Use with caution.
-- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day).
 - :code:`rp_api_retries = 0` - Amount of retries for performing REST calls to RP server.
 
 
 
 If you like to override the above parameters from command line, or from CI environment based on your build, then pass
 - :code:`-o "rp_launch_attributes=Smoke Tests"` during invocation.
```

### Comparing `pytest-reportportal-5.1.9/pytest_reportportal/config.py` & `pytest-reportportal-5.2.0/pytest_reportportal/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,82 @@
 """This module contains class that stores RP agent configuration data."""
+import sys
 import warnings
 
 from distutils.util import strtobool
 from os import getenv
+from typing import Optional, Union, Any, TextIO, Dict
 
+from _pytest.config import Config
 from reportportal_client.logs.log_manager import MAX_LOG_BATCH_PAYLOAD_SIZE
 
 try:
     # This try/except can go away once we support pytest >= 5.4.0
     from _pytest.logging import get_actual_log_level
 except ImportError:
     from _pytest.logging import get_log_level_for_setting as \
         get_actual_log_level
 
 
+OUTPUT_TYPES: Dict[str, TextIO] = {
+    'stdout': sys.stdout,
+    'stderr': sys.stderr
+}
+
+
 class AgentConfig(object):
     """Storage for the RP agent initialization attributes."""
 
-    def __init__(self, pytest_config):
+    rp_rerun: Optional[bool]
+    pconfig: Config
+    rp_endpoint: str
+    rp_hierarchy_code: bool
+    rp_dir_level: int
+    rp_hierarchy_dirs: bool
+    rp_dir_path_separator: str
+    rp_ignore_attributes: set
+    rp_is_skipped_an_issue: bool
+    rp_issue_id_marks: bool
+    rp_issue_system_url: str
+    rp_bts_project: str
+    rp_bts_url: str
+    rp_launch: str
+    rp_launch_id: Optional[str]
+    rp_launch_attributes: Optional[list]
+    rp_launch_description: str
+    rp_log_batch_size: int
+    rp_log_batch_payload_size: int
+    rp_log_level: Optional[int]
+    rp_log_format: Optional[str]
+    rp_mode: str
+    rp_parent_item_id: Optional[str]
+    rp_project: str
+    rp_rerun_of: Optional[str]
+    rp_api_retries: int
+    rp_skip_connection_test: bool
+    rp_api_key: str
+    rp_verify_ssl: Union[bool, str]
+    rp_launch_timeout: int
+    rp_launch_uuid_print: bool
+    rp_launch_uuid_print_output: TextIO
+
+    def __init__(self, pytest_config: Config) -> None:
         """Initialize required attributes."""
         self.rp_rerun = (pytest_config.option.rp_rerun or
                          pytest_config.getini('rp_rerun'))
         self.rp_endpoint = self.find_option(pytest_config, 'rp_endpoint')
         self.rp_hierarchy_code = self.find_option(pytest_config,
                                                   'rp_hierarchy_code')
         self.rp_dir_level = int(self.find_option(pytest_config,
                                                  'rp_hierarchy_dirs_level'))
         self.rp_hierarchy_dirs = self.find_option(pytest_config,
                                                   'rp_hierarchy_dirs')
         self.rp_dir_path_separator = \
             self.find_option(pytest_config, 'rp_hierarchy_dir_path_separator')
-        ignore_attributes = self.find_option(pytest_config,
-                                             'rp_ignore_attributes')
-        self.rp_ignore_attributes = set(ignore_attributes) \
-            if ignore_attributes else set()
+        self.rp_ignore_attributes = set(self.find_option(pytest_config, 'rp_ignore_attributes') or [])
         self.rp_is_skipped_an_issue = self.find_option(
             pytest_config,
             'rp_is_skipped_an_issue'
         )
         self.rp_issue_id_marks = self.find_option(pytest_config,
                                                   'rp_issue_id_marks')
         self.rp_issue_system_url = self.find_option(pytest_config,
@@ -123,16 +162,23 @@
         try:
             self.rp_verify_ssl = bool(strtobool(rp_verify_ssl))
         except (ValueError, AttributeError):
             self.rp_verify_ssl = rp_verify_ssl
         self.rp_launch_timeout = int(
             self.find_option(pytest_config, 'rp_launch_timeout'))
 
+        self.rp_launch_uuid_print = bool(strtobool(self.find_option(
+            pytest_config, 'rp_launch_uuid_print'
+        ) or 'False'))
+        self.rp_launch_uuid_print_output = OUTPUT_TYPES.get((self.find_option(
+            pytest_config, 'rp_launch_uuid_print_output'
+        ) or 'stdout').lower(), OUTPUT_TYPES['stdout'])
+
     # noinspection PyMethodMayBeStatic
-    def find_option(self, pytest_config, option_name, default=None):
+    def find_option(self, pytest_config: Config, option_name: str, default: Any = None):
         """
         Find a single configuration setting from multiple places.
 
         The value is retrieved in the following places in priority order:
 
         1. From `self.pconfig.option.[option_name]`.
         2. From `self.pconfig.getini(option_name)`.
@@ -144,8 +190,8 @@
         """
         value = (
                 getattr(pytest_config.option, option_name, None) or
                 pytest_config.getini(option_name)
         )
         if isinstance(value, bool):
             return value
-        return value if value else default
+        return value or default
```

### Comparing `pytest-reportportal-5.1.9/pytest_reportportal/plugin.py` & `pytest-reportportal-5.2.0/pytest_reportportal/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,17 @@
         log.debug(str(response_error))
         config.py_test_service.rp = None
         config._rp_enabled = False
         return
 
     if is_control(config) and not config._reporter_config.rp_launch_id:
         config.py_test_service.start_launch()
+        if config._reporter_config.rp_launch_uuid_print:
+            launch_id = config.py_test_service.rp.launch_id
+            print(f'Report Portal Launch UUID: {launch_id}', file=config._reporter_config.rp_launch_uuid_print_output)
         if config.pluginmanager.hasplugin('xdist') \
                 or config.pluginmanager.hasplugin('pytest-parallel'):
             if not wait_launch(session.config.py_test_service.rp):
                 log.error(FAILED_LAUNCH_WAIT)
                 config.py_test_service.rp = None
                 config._rp_enabled = False
 
@@ -396,14 +399,24 @@
         name='rp_thread_logging',
         help_str='EXPERIMENTAL: Report logs from threads. '
                  'This option applies a patch to the builtin Thread class, '
                  'and so it is turned off by default. Use with caution.',
         default=False,
         action='store_true'
     )
+    add_shared_option(
+        name='rp_launch_uuid_print',
+        help_str='Enables printing Launch UUID on test run start. Possible values: [True, False]',
+        default='False'
+    )
+    add_shared_option(
+        name='rp_launch_uuid_print_output',
+        help_str='Launch UUID print output. Default `stdout`. Possible values: [stderr, stdout]',
+        default='stdout'
+    )
 
     parser.addini(
         'rp_launch_attributes',
         type='args',
         help='Launch attributes, i.e Performance Regression')
     parser.addini(
         'rp_tests_attributes',
```

### Comparing `pytest-reportportal-5.1.9/pytest_reportportal/plugin.pyi` & `pytest-reportportal-5.2.0/pytest_reportportal/plugin.pyi`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.9/pytest_reportportal/rp_logging.py` & `pytest-reportportal-5.2.0/pytest_reportportal/rp_logging.py`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.9/pytest_reportportal/service.py` & `pytest-reportportal-5.2.0/pytest_reportportal/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """This module includes Service functions for work with pytest agent."""
 import logging
 import os.path
 import sys
 import threading
-from os import getenv, curdir
+from functools import wraps
+from os import curdir
 from time import time, sleep
-from typing import List
+from typing import List, Any, Optional, Set, Dict, Tuple
 
 from _pytest.doctest import DoctestItem
 from aenum import auto, Enum, unique
 from pytest import Class, Function, Module, Package, Item, Session, \
     PytestWarning
 from reportportal_client.core.rp_issues import Issue, ExternalIssue
 
+from .config import AgentConfig
+
 try:
     from pytest import Instance
 except ImportError:
     # in pytest >= 7.0 this type was removed
     Instance = type('dummy', (), {})
 from reportportal_client.client import RPClient
 from reportportal_client.helpers import (
@@ -24,35 +27,36 @@
     gen_attributes,
     get_launch_sys_attrs,
     get_package_version
 )
 
 log = logging.getLogger(__name__)
 
-MAX_ITEM_NAME_LENGTH = 256
-TRUNCATION_STR = '...'
-ROOT_DIR = str(os.path.abspath(curdir))
-PYTEST_MARKS_IGNORE = {'parametrize', 'usefixtures', 'filterwarnings'}
-NOT_ISSUE = Issue('NOT_ISSUE')
-ISSUE_DESCRIPTION_LINE_TEMPLATE = '* {}:{}'
-ISSUE_DESCRIPTION_URL_TEMPLATE = ' [{issue_id}]({url})'
-ISSUE_DESCRIPTION_ID_TEMPLATE = ' {issue_id}'
+MAX_ITEM_NAME_LENGTH: int = 256
+TRUNCATION_STR: str = '...'
+ROOT_DIR: str = str(os.path.abspath(curdir))
+PYTEST_MARKS_IGNORE: Set[str] = {'parametrize', 'usefixtures',
+                                 'filterwarnings'}
+NOT_ISSUE: Issue = Issue('NOT_ISSUE')
+ISSUE_DESCRIPTION_LINE_TEMPLATE: str = '* {}:{}'
+ISSUE_DESCRIPTION_URL_TEMPLATE: str = ' [{issue_id}]({url})'
+ISSUE_DESCRIPTION_ID_TEMPLATE: str = ' {issue_id}'
 
 
 def timestamp():
     """Time for difference between start and finish tests."""
     return str(int(time() * 1000))
 
 
-def trim_docstring(docstring):
+def trim_docstring(docstring: str) -> str:
     """
     Convert docstring.
 
     :param docstring: input docstring
-    :return: docstring
+    :return: trimmed docstring
     """
     if not docstring:
         return ''
     # Convert tabs to spaces (following the normal Python rules)
     # and split into a list of lines:
     lines = docstring.expandtabs().splitlines()
     # Determine minimum indentation (first line doesn't count):
@@ -89,37 +93,60 @@
     """This class stores test item path types."""
 
     CREATED = auto()
     IN_PROGRESS = auto()
     FINISHED = auto()
 
 
-class PyTestServiceClass(object):
+def check_rp_enabled(func):
+    """Verify is RP is enabled in config."""
+
+    @wraps(func)
+    def wrap(*args, **kwargs):
+        if args and isinstance(args[0], PyTestServiceClass):
+            if not args[0].rp:
+                return
+        func(*args, **kwargs)
+
+    return wrap
+
+
+class PyTestServiceClass:
     """Pytest service class for reporting test results to the Report Portal."""
 
-    def __init__(self, agent_config):
+    _config: AgentConfig
+    _issue_types: Dict[str, str]
+    _tree_path: Dict[Item, List[Dict[str, Any]]]
+    _log_levels: Tuple[str, str, str, str, str]
+    _start_tracker: Set[str]
+    _launch_id: Optional[str]
+    agent_name: str
+    agent_version: str
+    ignored_attributes: List[str]
+    parent_item_id: Optional[str]
+    rp: Optional[RPClient]
+    project_settings: Dict[str, Any]
+
+    def __init__(self, agent_config: AgentConfig) -> None:
         """Initialize instance attributes."""
         self._config = agent_config
         self._issue_types = {}
         self._tree_path = {}
         self._log_levels = ('TRACE', 'DEBUG', 'INFO', 'WARN', 'ERROR')
-        self._skip_analytics = getenv('AGENT_NO_ANALYTICS')
         self._start_tracker = set()
-        self._process_level_lock = threading.Lock()
         self._launch_id = None
         self.agent_name = 'pytest-reportportal'
         self.agent_version = get_package_version(self.agent_name)
         self.ignored_attributes = []
-        self.log_batch_size = 20
         self.parent_item_id = None
         self.rp = None
         self.project_settings = {}
 
     @property
-    def issue_types(self):
+    def issue_types(self) -> Dict[str, str]:
         """Issue types for the Report Portal project."""
         if not self._issue_types:
             if not self.project_settings:
                 return self._issue_types
             for values in self.project_settings["subTypes"].values():
                 for item in values:
                     self._issue_types[item["shortName"]] = item["locator"]
@@ -148,22 +175,21 @@
             'description': self._config.rp_launch_description,
             'mode': self._config.rp_mode,
             'rerun': self._config.rp_rerun,
             'rerun_of': self._config.rp_rerun_of
         }
         return start_rq
 
-    def start_launch(self):
+    @check_rp_enabled
+    def start_launch(self) -> Optional[str]:
         """
         Launch test items.
 
         :return: item ID
         """
-        if self.rp is None:
-            return
         sl_pt = self._build_start_launch_rq()
         log.debug('ReportPortal - Start launch: request_body=%s', sl_pt)
         self._launch_id = self.rp.start_launch(**sl_pt)
         log.debug('ReportPortal - Launch started: id=%s', self._launch_id)
         return self._launch_id
 
     def _get_item_dirs(self, item):
@@ -319,23 +345,21 @@
             path.append(leaf)
             for name, child_leaf in leaf['children'].items():
                 self._build_item_paths(child_leaf, path)
             path.pop()
         elif leaf['type'] != LeafType.ROOT:
             self._tree_path[leaf['item']] = path + [leaf]
 
+    @check_rp_enabled
     def collect_tests(self, session):
         """
         Collect all tests.
 
         :param session: pytest.Session
         """
-        if self.rp is None:
-            return
-
         # Create a test tree to be able to apply mutations
         test_tree = self._build_test_tree(session)
         self._remove_root_package(test_tree)
         self._remove_root_dirs(test_tree, self._config.rp_dir_level)
         self._generate_names(test_tree)
         if not self._config.rp_hierarchy_dirs:
             self._merge_dirs(test_tree)
@@ -411,18 +435,16 @@
     def _create_suite(self, leaf):
         if leaf['exec'] != ExecStatus.CREATED:
             return
         item_id = self._start_suite(self._build_start_suite_rq(leaf))
         leaf['item_id'] = item_id
         leaf['exec'] = ExecStatus.IN_PROGRESS
 
+    @check_rp_enabled
     def _create_suite_path(self, item):
-        if self.rp is None:
-            return
-
         path = self._tree_path[item]
         for leaf in path[1:-1]:
             if leaf['exec'] != ExecStatus.CREATED:
                 continue
             self._lock(leaf, lambda p: self._create_suite(p))
 
     def _get_code_ref(self, item):
@@ -652,22 +674,23 @@
 
     def __unique_id(self):
         return str(os.getpid()) + '-' + str(threading.current_thread().ident)
 
     def __started(self):
         return self.__unique_id() in self._start_tracker
 
+    @check_rp_enabled
     def start_pytest_item(self, test_item=None):
         """
         Start pytest_item.
 
         :param test_item: pytest.Item
         :return: item ID
         """
-        if self.rp is None or test_item is None:
+        if test_item is None:
             return
 
         if not self.__started():
             self.start()
 
         self._create_suite_path(test_item)
 
@@ -754,24 +777,22 @@
                 current_status = self._lock(child_leaf, lambda p: p['exec'])
                 if current_status != ExecStatus.FINISHED:
                     return
 
         self._lock(leaf['parent'], lambda p: self._proceed_suite_finish(p))
         self._finish_parents(leaf['parent'])
 
+    @check_rp_enabled
     def finish_pytest_item(self, test_item):
         """
         Finish pytest_item.
 
         :param test_item: pytest.Item
         :return: None
         """
-        if self.rp is None:
-            return
-
         path = self._tree_path[test_item]
         leaf = path[-1]
         self._process_metadata_item_finish(leaf)
         self._finish_step(self._build_finish_step_rq(leaf))
         leaf['exec'] = ExecStatus.FINISHED
         self._finish_parents(leaf)
 
@@ -807,54 +828,50 @@
         }
         return finish_rq
 
     def _finish_launch(self, finish_rq):
         log.debug('ReportPortal - Finish launch: request_body=%s', finish_rq)
         self.rp.finish_launch(**finish_rq)
 
+    @check_rp_enabled
     def finish_launch(self):
         """
         Finish tests launch.
 
         :return: None
         """
-        if self.rp is None:
-            return
-
         # To finish launch session str parameter is needed
         self._finish_launch(self._build_finish_launch_rq())
 
+    @check_rp_enabled
     def post_log(self, test_item, message, log_level='INFO', attachment=None):
         """
         Send a log message to the Report Portal.
 
         :param test_item: pytest.Item
         :param message:    message in log body
         :param log_level:   a level of a log entry (ERROR, WARN, INFO, DEBUG,
         TRACE, FATAL, UNKNOWN)
         :param attachment: attachment file
         :return: None
         """
-        if self.rp is None:
-            return
-
         if log_level not in self._log_levels:
             log.warning('Incorrect loglevel = %s. Force set to INFO. '
                         'Available levels: %s.', log_level, self._log_levels)
         item_id = self._tree_path[test_item][-1]['item_id']
         sl_rq = {
             'item_id': item_id,
             'time': timestamp(),
             'message': message,
             'level': log_level,
             'attachment': attachment
         }
         self.rp.log(**sl_rq)
 
-    def start(self):
+    def start(self) -> None:
         """Start servicing Report Portal requests."""
         self.parent_item_id = self._config.rp_parent_item_id
         self.ignored_attributes = list(
             set(
                 self._config.rp_ignore_attributes or []
             ).union({'parametrize'})
         )
```

### Comparing `pytest-reportportal-5.1.9/pytest_reportportal.egg-info/PKG-INFO` & `pytest-reportportal-5.2.0/pytest_reportportal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-reportportal
-Version: 5.1.9
+Version: 5.2.0
 Summary: Agent for Reporting results of tests to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-pytest
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,pytest,agent
 Classifier: Framework :: Pytest
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 agent-python-pytest
 ===================
 
@@ -99,33 +98,35 @@
 - The :code:`rp_api_key` can also be set with the environment variable `RP_API_KEY`. This will override the value set for :code:`rp_api_key` in pytest.ini
 
 The following parameters are optional:
 
 - :code:`rp_launch = AnyLaunchName` - launch name (could be overridden by pytest --rp-launch option, default value is 'Pytest Launch').
 - :code:`rp_launch_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing launch (the session will not handle the lifecycle of the given launch).
 - :code:`rp_launch_attributes = 'PyTest' 'Smoke' 'Env:Python3'` - list of attributes for launch.
+- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden by pytest --rp-launch-description option, default value is '').
+- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day).
+- :code:`rp_launch_uuid_print = True` - Enables printing Launch UUID on test run start. Default `False`.
+- :code:`rp_launch_uuid_print_output = stderr` - Launch UUID print output. Default `stdout`. Possible values: [stderr, stdout].
 - :code:`rp_parent_item_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing test item for session to use as parent item for the tests (the session will not handle the lifecycle of the given test item).
 - :code:`rp_tests_attributes = 'PyTest' 'Smoke'` - list of attributes that will be added for each item in the launch.
-- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden by pytest --rp-launch-description option, default value is '').
 - :code:`rp_log_batch_size = 20` - size of batch log request.
 - :code:`rp_log_batch_payload_size = 65000000` - maximum payload size in bytes of async batch log requests.
 - :code:`rp_log_level = INFO` - The log level that will be reported.
 - :code:`rp_log_format = [%(levelname)7s] (%(name)s) %(message)s (%(filename)s:%(lineno)s)` - Format string to be used for logs sent to the service.
 - :code:`rp_ignore_attributes = 'xfail' 'usefixture'` - Ignore specified pytest markers.
-- :code:`rp_is_skipped_an_issue = False` - Treat skipped tests as required investigation. Default is True.
+- :code:`rp_is_skipped_an_issue = False` - Treat skipped tests as required investigation. Default `True`.
 - :code:`rp_hierarchy_dirs_level = 0` - Directory starting hierarchy level (from pytest.ini level) (default `0`).
 - :code:`rp_hierarchy_dirs = True` - Enables hierarchy for tests directories, default `False`. Doesn't support 'xdist' plugin.
 - :code:`rp_hierarchy_dir_path_separator` - Path separator to display directories in test hierarchy. In case of empty value current system path separator will be used (os.path.sep).
 - :code:`rp_hierarchy_code` - Enables hierarchy for inner classes and parametrized tests, default `False`. Doesn't support 'xdist' plugin.
 - :code:`rp_issue_system_url = https://bugzilla.some.com/show_bug.cgi?id={issue_id}` - issue URL (issue_id will be filled by parameter from pytest mark).
 - :code:`rp_issue_id_marks = True` - Enables adding marks for issue ids (e.g. "issue:123456").
 - :code:`rp_verify_ssl = True` - Verify SSL when connecting to the server.
 - :code:`rp_mode = DEFAULT` - DEBUG or DEFAULT launch mode. DEBUG launches are displayed in a separate tab and not visible to anyone except owner.
 - :code:`rp_thread_logging` - EXPERIMENTAL - Enables support for reporting logs from threads by patching the builtin Thread class. Use with caution.
-- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day).
 - :code:`rp_api_retries = 0` - Amount of retries for performing REST calls to RP server.
 
 
 
 If you like to override the above parameters from command line, or from CI environment based on your build, then pass
 - :code:`-o "rp_launch_attributes=Smoke Tests"` during invocation.
```

### Comparing `pytest-reportportal-5.1.9/pytest_reportportal.egg-info/SOURCES.txt` & `pytest-reportportal-5.2.0/pytest_reportportal.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 pytest_reportportal/__init__.py
 pytest_reportportal/config.py
-pytest_reportportal/config.pyi
 pytest_reportportal/errors.py
 pytest_reportportal/plugin.py
 pytest_reportportal/plugin.pyi
 pytest_reportportal/rp_logging.py
 pytest_reportportal/service.py
-pytest_reportportal/service.pyi
 pytest_reportportal.egg-info/PKG-INFO
 pytest_reportportal.egg-info/SOURCES.txt
 pytest_reportportal.egg-info/dependency_links.txt
 pytest_reportportal.egg-info/entry_points.txt
 pytest_reportportal.egg-info/requires.txt
 pytest_reportportal.egg-info/top_level.txt
```

### Comparing `pytest-reportportal-5.1.9/setup.py` & `pytest-reportportal-5.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Config for setup package pytest agent."""
 
 import os
 
 from setuptools import setup
 
 
-__version__ = '5.1.9'
+__version__ = '5.2.0'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Filename to be read
     :return:      File content
@@ -30,20 +30,19 @@
     packages=['pytest_reportportal'],
     package_data={'pytest_reportportal': ['*.pyi']},
     install_requires=read_file('requirements.txt').splitlines(),
     license='Apache 2.0',
     keywords=['testing', 'reporting', 'reportportal', 'pytest', 'agent'],
     classifiers=[
         'Framework :: Pytest',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
         ],
     entry_points={
         'pytest11': [
             'pytest_reportportal = pytest_reportportal.plugin',
         ]
     }
 )
```

