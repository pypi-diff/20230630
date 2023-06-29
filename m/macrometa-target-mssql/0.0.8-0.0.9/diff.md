# Comparing `tmp/macrometa-target-mssql-0.0.8.tar.gz` & `tmp/macrometa-target-mssql-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mssql-0.0.8.tar", max compression
+gzip compressed data, was "macrometa-target-mssql-0.0.9.tar", max compression
```

## Comparing `macrometa-target-mssql-0.0.8.tar` & `macrometa-target-mssql-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-29 18:13:48.824964 macrometa-target-mssql-0.0.8/LICENSE
--rw-r--r--   0        0        0    24115 2023-06-29 18:13:48.824964 macrometa-target-mssql-0.0.8/macrometa_target_mssql/__init__.py
--rw-r--r--   0        0        0    34142 2023-06-29 18:13:48.828964 macrometa-target-mssql-0.0.8/macrometa_target_mssql/db_sync.py
--rw-r--r--   0        0        0     1554 2023-06-29 18:13:49.076965 macrometa-target-mssql-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.8/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 18:29:02.540852 macrometa-target-mssql-0.0.9/LICENSE
+-rw-r--r--   0        0        0    24117 2023-06-29 18:29:02.540852 macrometa-target-mssql-0.0.9/macrometa_target_mssql/__init__.py
+-rw-r--r--   0        0        0    34144 2023-06-29 18:29:02.540852 macrometa-target-mssql-0.0.9/macrometa_target_mssql/db_sync.py
+-rw-r--r--   0        0        0     1554 2023-06-29 18:29:02.800850 macrometa-target-mssql-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.9/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.9/PKG-INFO
```

### Comparing `macrometa-target-mssql-0.0.8/LICENSE` & `macrometa-target-mssql-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.8/macrometa_target_mssql/__init__.py` & `macrometa-target-mssql-0.0.9/macrometa_target_mssql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                            default_value='1433'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
                            description='Microsoft SQL Server username.',
                            placeholder_value='username'),
             ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, True, False,
                            description='Microsoft SQL Server password.',
                            placeholder_value='password'),
-            ConfigProperty('dbname', 'Database Name', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('database', 'Database Name', ConfigAttributeType.STRING, True, False,
                            description='Microsoft SQL Server database name.',
                            default_value='master'),
             ConfigProperty('default_target_schema', 'Target Schema', ConfigAttributeType.STRING, True, True,
                            description='Destination Schema name.',
                            placeholder_value='public'),
             ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, True,
                            description='Destination table name.',
```

### Comparing `macrometa-target-mssql-0.0.8/macrometa_target_mssql/db_sync.py` & `macrometa-target-mssql-0.0.9/macrometa_target_mssql/db_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def validate_config(config):
     errors = []
     required_config_keys = [
         'host',
         'port',
         'user',
         'password',
-        'dbname',
+        'database',
         'default_target_schema',
         'target_table',
     ]
 
     # Check if mandatory keys exist
     for k in required_config_keys:
         if not config.get(k, None):
```

### Comparing `macrometa-target-mssql-0.0.8/pyproject.toml` & `macrometa-target-mssql-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mssql"
-version='0.0.8'
+version='0.0.9'
 description = "Macrometa target connector for writing data into Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-mssql-0.0.8/setup.py` & `macrometa-target-mssql-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mssql = macrometa_target_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mssql',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Macrometa target connector for writing data into Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mssql-0.0.8/PKG-INFO` & `macrometa-target-mssql-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mssql
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa target connector for writing data into Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MicrosoftSQLServer
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

