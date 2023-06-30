# Comparing `tmp/influxdb3-python-cli-0.2.0.tar.gz` & `tmp/influxdb3-python-cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-cli-0.2.0.tar", last modified: Mon Jun 26 11:17:34 2023, max compression
+gzip compressed data, was "influxdb3-python-cli-0.2.1.tar", last modified: Fri Jun 30 14:36:39 2023, max compression
```

## Comparing `influxdb3-python-cli-0.2.0.tar` & `influxdb3-python-cli-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/influxdb_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8351 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/influxdb_cli/influx3.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/influxdb_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/influxdb_cli/config_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9564 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/influxdb_cli/influx3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/setup.py
```

### Comparing `influxdb3-python-cli-0.2.0/LICENSE` & `influxdb3-python-cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.2.0/PKG-INFO` & `influxdb3-python-cli-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -59,40 +59,27 @@
 - To install the client to a user-specific directory (without administrative rights), pass the `--user` flag in the `pip` command.
 - To install the client in your system-wide path, use `sudo` with admin privileges.
 
 ## Add a config
 
 To configure the CLI, do _one_ of the following:
 
-- Use the `influx3 config` command to create or modify config--for example:
+- Use the `influx3 create config` command to create or modify config--for example:
 
     ```bash
-    influx3 config \
+    influx3 create config \
     --name="my-config" \
     --database="<database or bucket name>" \
     --host="us-east-1-1.aws.cloud2.influxdata.com" \
     --token="<your token>" \
     --org="<your org ID>"
     ```
     
-  The output is the configuration in a `config.json` file.
+  The output is the configuration in a `config.json` file. This is saved within a directory called `config` located with the influx3 application.
 
-- In your editor, create or edit the `config.json` file, and then save it to the directory where you're using the `influx3` command--for example:
-
-    ```json
-    {
-        "my-config": {
-            "database": "your-database",
-            "host": "your-host",
-            "token": "your-token",
-            "org": "your-org-id",
-            "active": true
-        }
-    }
-    ```
 
 If you're running the CLI against InfluxDB Cloud Serverless, replace `your-database` in the examples with your Cloud Serverless _bucket name_.
 
 ## Run as a command
 
 ```
 influx3 sql "select * from anomalies"
@@ -171,14 +158,73 @@
 
 The following example shows how to write CSV data from the [`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol):
 
 ```bash
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
+## Config Commands
+
+The `config` command allows you to manage configurations for your application. It has the following subcommands: `create`, `update`, `use`, `delete`, and `list`.
+
+### Create
+
+The `create` subcommand creates a new configuration. It requires the `--name`, `--host`, `--token`, `--database`, and `--org` parameters. The `--active` parameter is optional and can be used to set the new configuration as the active one.
+
+Example usage:
+
+```bash
+influx3.py config create --name="my-config" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --database="<database or bucket name>" --org="<your org ID>" --active
+```
+
+### Update
+
+The `update` subcommand updates an existing configuration. The `--name` parameter is required to specify which configuration to update. All other parameters (`--host`, `--token`, `--database`, `--org`, `--active`) are optional.
+
+Example usage:
+
+```bash
+influx3.py config update --name="my-config" --host="new-host.com"
+```
+
+### Use
+
+The `use` subcommand sets a specific configuration as the active one. The `--name` parameter is required to specify which configuration to use.
+
+Example usage:
+
+```bash
+influx3.py config use --name="my-config"
+```
+
+### Delete
+
+The `delete` subcommand deletes a configuration. The `--name` parameter is required to specify which configuration to delete.
+
+Example usage:
+
+```bash
+influx3.py config delete --name="my-config"
+```
+
+### List
+
+The `list` subcommand lists all the configurations.
+
+Example usage:
+
+```bash
+influx3.py config list
+```
+
+Please replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `"<your token>"`, `"<database or bucket name>"`, and `"<your org ID>"` with your actual values.
+
+
+
+
 ## Client library
 
 The underlying client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
 
 ## Contribution
 
 When developing a new feature for the CLI or the client library, make sure to test your feature in both for breaking changes.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.1 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -22,46 +22,64 @@
 the CLI in a _virtual environment_. [See how to create and use a `venv` or
 `conda` Python virtual environment](https://docs.influxdata.com/influxdb/cloud-
 serverless/query-data/execute-queries/flight-sql/python/#create-a-python-
 virtual-environment). - To install the client to a user-specific directory
 (without administrative rights), pass the `--user` flag in the `pip` command. -
 To install the client in your system-wide path, use `sudo` with admin
 privileges. ## Add a config To configure the CLI, do _one_ of the following: -
-Use the `influx3 config` command to create or modify config--for example:
-```bash influx3 config \ --name="my-config" \ --database="" \ --host="us-east-
-1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The output is the
-configuration in a `config.json` file. - In your editor, create or edit the
-`config.json` file, and then save it to the directory where you're using the
-`influx3` command--for example: ```json { "my-config": { "database": "your-
-database", "host": "your-host", "token": "your-token", "org": "your-org-id",
-"active": true } } ``` If you're running the CLI against InfluxDB Cloud
-Serverless, replace `your-database` in the examples with your Cloud Serverless
-_bucket name_. ## Run as a command ``` influx3 sql "select * from anomalies"
-``` ``` influx3 write testmes f=7 ``` ## Query and write interactively In your
-terminal, enter the following command: ``` influx3 ``` `influx3` displays the `
-(>)` interactive prompt and waits for input. ``` Welcome to my IOx CLI. (>) ```
-To query, type `sql` at the prompt. ``` (>) sql ``` At the `(sql >)` prompt,
-enter your query statement: ``` (sql >) select * from home ``` The `influx3`
-CLI displays query results in Markdown table format--for example: ``` | | co |
-hum | room | temp | time | |----:|-----:|------:|:------------|-------:|:------
-------------------------| | 0 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:00 |
-| 1 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:50 | ``` To write, type
-`write` at the `(>)` prompt. ``` (>) write ``` At the `(write >)` prompt, enter
-line protocol data. ``` (>) write home,room=kitchen temp=70.5,hum=80 ``` To
-exit a prompt, enter `exit`. ## Write from a file The InfluxDB CLI and client
-library can write data from a CSV file. The CSV file must contain the
-following: - A header row with column names - A column that contains a
-timestamp for each row The following CLI options specify how data is parsed: *
-`--file` - The path to the csv file. * `--time` - The name of the column
-containing the timestamp. * `--measurement` - The name of the measurment to
-store the CSV data under. (Currently only supports user specified string) * `--
-tags` - (optional) Specify an array of column names to use as tags. (Currently
-only supports user specified strings) for example: `--tags=host,region` The
-following example shows how to write CSV data from the [`./Examples/
-example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/
-main/Examples/example.csv) to InfluxDB (as line protocol): ```bash influx3
-write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags
-host,region ``` ## Client library The underlying client library is also
-available for use in your own code: https://github.com/InfluxCommunity/
-influxdb3-python ## Contribution When developing a new feature for the CLI or
-the client library, make sure to test your feature in both for breaking
-changes. #
+Use the `influx3 create config` command to create or modify config--for
+example: ```bash influx3 create config \ --name="my-config" \ --database="" \ -
+-host="us-east-1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The
+output is the configuration in a `config.json` file. This is saved within a
+directory called `config` located with the influx3 application. If you're
+running the CLI against InfluxDB Cloud Serverless, replace `your-database` in
+the examples with your Cloud Serverless _bucket name_. ## Run as a command ```
+influx3 sql "select * from anomalies" ``` ``` influx3 write testmes f=7 ``` ##
+Query and write interactively In your terminal, enter the following command:
+``` influx3 ``` `influx3` displays the `(>)` interactive prompt and waits for
+input. ``` Welcome to my IOx CLI. (>) ``` To query, type `sql` at the prompt.
+``` (>) sql ``` At the `(sql >)` prompt, enter your query statement: ``` (sql
+>) select * from home ``` The `influx3` CLI displays query results in Markdown
+table format--for example: ``` | | co | hum | room | temp | time | |----:|----
+-:|------:|:------------|-------:|:------------------------------| | 0 | 0 |
+35.9 | Kitchen | 21 | 2023-03-09 08:00:00 | | 1 | 0 | 35.9 | Kitchen | 21 |
+2023-03-09 08:00:50 | ``` To write, type `write` at the `(>)` prompt. ``` (>)
+write ``` At the `(write >)` prompt, enter line protocol data. ``` (>) write
+home,room=kitchen temp=70.5,hum=80 ``` To exit a prompt, enter `exit`. ## Write
+from a file The InfluxDB CLI and client library can write data from a CSV file.
+The CSV file must contain the following: - A header row with column names - A
+column that contains a timestamp for each row The following CLI options specify
+how data is parsed: * `--file` - The path to the csv file. * `--time` - The
+name of the column containing the timestamp. * `--measurement` - The name of
+the measurment to store the CSV data under. (Currently only supports user
+specified string) * `--tags` - (optional) Specify an array of column names to
+use as tags. (Currently only supports user specified strings) for example: `--
+tags=host,region` The following example shows how to write CSV data from the
+[`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-
+python/blob/main/Examples/example.csv) to InfluxDB (as line protocol): ```bash
+influx3 write_csv --file ./Examples/example.csv --measurement table2 --time
+Date --tags host,region ``` ## Config Commands The `config` command allows you
+to manage configurations for your application. It has the following
+subcommands: `create`, `update`, `use`, `delete`, and `list`. ### Create The
+`create` subcommand creates a new configuration. It requires the `--name`, `--
+host`, `--token`, `--database`, and `--org` parameters. The `--active`
+parameter is optional and can be used to set the new configuration as the
+active one. Example usage: ```bash influx3.py config create --name="my-config"
+--host="us-east-1-1.aws.cloud2.influxdata.com" --token="" --database="" --
+org="" --active ``` ### Update The `update` subcommand updates an existing
+configuration. The `--name` parameter is required to specify which
+configuration to update. All other parameters (`--host`, `--token`, `--
+database`, `--org`, `--active`) are optional. Example usage: ```bash influx3.py
+config update --name="my-config" --host="new-host.com" ``` ### Use The `use`
+subcommand sets a specific configuration as the active one. The `--name`
+parameter is required to specify which configuration to use. Example usage:
+```bash influx3.py config use --name="my-config" ``` ### Delete The `delete`
+subcommand deletes a configuration. The `--name` parameter is required to
+specify which configuration to delete. Example usage: ```bash influx3.py config
+delete --name="my-config" ``` ### List The `list` subcommand lists all the
+configurations. Example usage: ```bash influx3.py config list ``` Please
+replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`, `""`,
+and `""` with your actual values. ## Client library The underlying client
+library is also available for use in your own code: https://github.com/
+InfluxCommunity/influxdb3-python ## Contribution When developing a new feature
+for the CLI or the client library, make sure to test your feature in both for
+breaking changes. #
```

### Comparing `influxdb3-python-cli-0.2.0/README.md` & `influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: influxdb3-python-cli
+Version: 0.2.1
+Summary: Community Python client for InfluxDB 3.0 (CLI)
+Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
+Author: InfluxData
+Author-email: contact@influxdata.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
     <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python-cli/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python-cli.svg" alt="PyPI version">
@@ -40,40 +59,27 @@
 - To install the client to a user-specific directory (without administrative rights), pass the `--user` flag in the `pip` command.
 - To install the client in your system-wide path, use `sudo` with admin privileges.
 
 ## Add a config
 
 To configure the CLI, do _one_ of the following:
 
-- Use the `influx3 config` command to create or modify config--for example:
+- Use the `influx3 create config` command to create or modify config--for example:
 
     ```bash
-    influx3 config \
+    influx3 create config \
     --name="my-config" \
     --database="<database or bucket name>" \
     --host="us-east-1-1.aws.cloud2.influxdata.com" \
     --token="<your token>" \
     --org="<your org ID>"
     ```
     
-  The output is the configuration in a `config.json` file.
-
-- In your editor, create or edit the `config.json` file, and then save it to the directory where you're using the `influx3` command--for example:
+  The output is the configuration in a `config.json` file. This is saved within a directory called `config` located with the influx3 application.
 
-    ```json
-    {
-        "my-config": {
-            "database": "your-database",
-            "host": "your-host",
-            "token": "your-token",
-            "org": "your-org-id",
-            "active": true
-        }
-    }
-    ```
 
 If you're running the CLI against InfluxDB Cloud Serverless, replace `your-database` in the examples with your Cloud Serverless _bucket name_.
 
 ## Run as a command
 
 ```
 influx3 sql "select * from anomalies"
@@ -152,14 +158,73 @@
 
 The following example shows how to write CSV data from the [`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol):
 
 ```bash
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
+## Config Commands
+
+The `config` command allows you to manage configurations for your application. It has the following subcommands: `create`, `update`, `use`, `delete`, and `list`.
+
+### Create
+
+The `create` subcommand creates a new configuration. It requires the `--name`, `--host`, `--token`, `--database`, and `--org` parameters. The `--active` parameter is optional and can be used to set the new configuration as the active one.
+
+Example usage:
+
+```bash
+influx3.py config create --name="my-config" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --database="<database or bucket name>" --org="<your org ID>" --active
+```
+
+### Update
+
+The `update` subcommand updates an existing configuration. The `--name` parameter is required to specify which configuration to update. All other parameters (`--host`, `--token`, `--database`, `--org`, `--active`) are optional.
+
+Example usage:
+
+```bash
+influx3.py config update --name="my-config" --host="new-host.com"
+```
+
+### Use
+
+The `use` subcommand sets a specific configuration as the active one. The `--name` parameter is required to specify which configuration to use.
+
+Example usage:
+
+```bash
+influx3.py config use --name="my-config"
+```
+
+### Delete
+
+The `delete` subcommand deletes a configuration. The `--name` parameter is required to specify which configuration to delete.
+
+Example usage:
+
+```bash
+influx3.py config delete --name="my-config"
+```
+
+### List
+
+The `list` subcommand lists all the configurations.
+
+Example usage:
+
+```bash
+influx3.py config list
+```
+
+Please replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `"<your token>"`, `"<database or bucket name>"`, and `"<your org ID>"` with your actual values.
+
+
+
+
 ## Client library
 
 The underlying client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
 
 ## Contribution
 
 When developing a new feature for the CLI or the client library, make sure to test your feature in both for breaking changes.
```

#### html2text {}

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.1 Summary:
+Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
+InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
+contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
+License Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown License-File: LICENSE
                                  [Your Image]
  [PyPI_version] [PyPI_downloads] [Lint_Code_Base] [Lint_Code_Base] [Community
                                     Slack]
 # influxdb3-python-cli ## About This repository contains a CLI extension to the
 [influxdb 3.0 python client library](https://github.com/InfluxCommunity/
 influxdb3-python). While this code is built on officially supported APIs, the
 library and CLI here are not officially support by InfluxData. ## Install To
@@ -12,46 +22,64 @@
 the CLI in a _virtual environment_. [See how to create and use a `venv` or
 `conda` Python virtual environment](https://docs.influxdata.com/influxdb/cloud-
 serverless/query-data/execute-queries/flight-sql/python/#create-a-python-
 virtual-environment). - To install the client to a user-specific directory
 (without administrative rights), pass the `--user` flag in the `pip` command. -
 To install the client in your system-wide path, use `sudo` with admin
 privileges. ## Add a config To configure the CLI, do _one_ of the following: -
-Use the `influx3 config` command to create or modify config--for example:
-```bash influx3 config \ --name="my-config" \ --database="" \ --host="us-east-
-1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The output is the
-configuration in a `config.json` file. - In your editor, create or edit the
-`config.json` file, and then save it to the directory where you're using the
-`influx3` command--for example: ```json { "my-config": { "database": "your-
-database", "host": "your-host", "token": "your-token", "org": "your-org-id",
-"active": true } } ``` If you're running the CLI against InfluxDB Cloud
-Serverless, replace `your-database` in the examples with your Cloud Serverless
-_bucket name_. ## Run as a command ``` influx3 sql "select * from anomalies"
-``` ``` influx3 write testmes f=7 ``` ## Query and write interactively In your
-terminal, enter the following command: ``` influx3 ``` `influx3` displays the `
-(>)` interactive prompt and waits for input. ``` Welcome to my IOx CLI. (>) ```
-To query, type `sql` at the prompt. ``` (>) sql ``` At the `(sql >)` prompt,
-enter your query statement: ``` (sql >) select * from home ``` The `influx3`
-CLI displays query results in Markdown table format--for example: ``` | | co |
-hum | room | temp | time | |----:|-----:|------:|:------------|-------:|:------
-------------------------| | 0 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:00 |
-| 1 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:50 | ``` To write, type
-`write` at the `(>)` prompt. ``` (>) write ``` At the `(write >)` prompt, enter
-line protocol data. ``` (>) write home,room=kitchen temp=70.5,hum=80 ``` To
-exit a prompt, enter `exit`. ## Write from a file The InfluxDB CLI and client
-library can write data from a CSV file. The CSV file must contain the
-following: - A header row with column names - A column that contains a
-timestamp for each row The following CLI options specify how data is parsed: *
-`--file` - The path to the csv file. * `--time` - The name of the column
-containing the timestamp. * `--measurement` - The name of the measurment to
-store the CSV data under. (Currently only supports user specified string) * `--
-tags` - (optional) Specify an array of column names to use as tags. (Currently
-only supports user specified strings) for example: `--tags=host,region` The
-following example shows how to write CSV data from the [`./Examples/
-example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/
-main/Examples/example.csv) to InfluxDB (as line protocol): ```bash influx3
-write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags
-host,region ``` ## Client library The underlying client library is also
-available for use in your own code: https://github.com/InfluxCommunity/
-influxdb3-python ## Contribution When developing a new feature for the CLI or
-the client library, make sure to test your feature in both for breaking
-changes. #
+Use the `influx3 create config` command to create or modify config--for
+example: ```bash influx3 create config \ --name="my-config" \ --database="" \ -
+-host="us-east-1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The
+output is the configuration in a `config.json` file. This is saved within a
+directory called `config` located with the influx3 application. If you're
+running the CLI against InfluxDB Cloud Serverless, replace `your-database` in
+the examples with your Cloud Serverless _bucket name_. ## Run as a command ```
+influx3 sql "select * from anomalies" ``` ``` influx3 write testmes f=7 ``` ##
+Query and write interactively In your terminal, enter the following command:
+``` influx3 ``` `influx3` displays the `(>)` interactive prompt and waits for
+input. ``` Welcome to my IOx CLI. (>) ``` To query, type `sql` at the prompt.
+``` (>) sql ``` At the `(sql >)` prompt, enter your query statement: ``` (sql
+>) select * from home ``` The `influx3` CLI displays query results in Markdown
+table format--for example: ``` | | co | hum | room | temp | time | |----:|----
+-:|------:|:------------|-------:|:------------------------------| | 0 | 0 |
+35.9 | Kitchen | 21 | 2023-03-09 08:00:00 | | 1 | 0 | 35.9 | Kitchen | 21 |
+2023-03-09 08:00:50 | ``` To write, type `write` at the `(>)` prompt. ``` (>)
+write ``` At the `(write >)` prompt, enter line protocol data. ``` (>) write
+home,room=kitchen temp=70.5,hum=80 ``` To exit a prompt, enter `exit`. ## Write
+from a file The InfluxDB CLI and client library can write data from a CSV file.
+The CSV file must contain the following: - A header row with column names - A
+column that contains a timestamp for each row The following CLI options specify
+how data is parsed: * `--file` - The path to the csv file. * `--time` - The
+name of the column containing the timestamp. * `--measurement` - The name of
+the measurment to store the CSV data under. (Currently only supports user
+specified string) * `--tags` - (optional) Specify an array of column names to
+use as tags. (Currently only supports user specified strings) for example: `--
+tags=host,region` The following example shows how to write CSV data from the
+[`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-
+python/blob/main/Examples/example.csv) to InfluxDB (as line protocol): ```bash
+influx3 write_csv --file ./Examples/example.csv --measurement table2 --time
+Date --tags host,region ``` ## Config Commands The `config` command allows you
+to manage configurations for your application. It has the following
+subcommands: `create`, `update`, `use`, `delete`, and `list`. ### Create The
+`create` subcommand creates a new configuration. It requires the `--name`, `--
+host`, `--token`, `--database`, and `--org` parameters. The `--active`
+parameter is optional and can be used to set the new configuration as the
+active one. Example usage: ```bash influx3.py config create --name="my-config"
+--host="us-east-1-1.aws.cloud2.influxdata.com" --token="" --database="" --
+org="" --active ``` ### Update The `update` subcommand updates an existing
+configuration. The `--name` parameter is required to specify which
+configuration to update. All other parameters (`--host`, `--token`, `--
+database`, `--org`, `--active`) are optional. Example usage: ```bash influx3.py
+config update --name="my-config" --host="new-host.com" ``` ### Use The `use`
+subcommand sets a specific configuration as the active one. The `--name`
+parameter is required to specify which configuration to use. Example usage:
+```bash influx3.py config use --name="my-config" ``` ### Delete The `delete`
+subcommand deletes a configuration. The `--name` parameter is required to
+specify which configuration to delete. Example usage: ```bash influx3.py config
+delete --name="my-config" ``` ### List The `list` subcommand lists all the
+configurations. Example usage: ```bash influx3.py config list ``` Please
+replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`, `""`,
+and `""` with your actual values. ## Client library The underlying client
+library is also available for use in your own code: https://github.com/
+InfluxCommunity/influxdb3-python ## Contribution When developing a new feature
+for the CLI or the client library, make sure to test your feature in both for
+breaking changes. #
```

### Comparing `influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/PKG-INFO` & `influxdb3-python-cli-0.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: influxdb3-python-cli
-Version: 0.2.0
-Summary: Community Python client for InfluxDB 3.0 (CLI)
-Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
-Author: InfluxData
-Author-email: contact@influxdata.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
     <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python-cli/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python-cli.svg" alt="PyPI version">
@@ -59,40 +40,27 @@
 - To install the client to a user-specific directory (without administrative rights), pass the `--user` flag in the `pip` command.
 - To install the client in your system-wide path, use `sudo` with admin privileges.
 
 ## Add a config
 
 To configure the CLI, do _one_ of the following:
 
-- Use the `influx3 config` command to create or modify config--for example:
+- Use the `influx3 create config` command to create or modify config--for example:
 
     ```bash
-    influx3 config \
+    influx3 create config \
     --name="my-config" \
     --database="<database or bucket name>" \
     --host="us-east-1-1.aws.cloud2.influxdata.com" \
     --token="<your token>" \
     --org="<your org ID>"
     ```
     
-  The output is the configuration in a `config.json` file.
-
-- In your editor, create or edit the `config.json` file, and then save it to the directory where you're using the `influx3` command--for example:
+  The output is the configuration in a `config.json` file. This is saved within a directory called `config` located with the influx3 application.
 
-    ```json
-    {
-        "my-config": {
-            "database": "your-database",
-            "host": "your-host",
-            "token": "your-token",
-            "org": "your-org-id",
-            "active": true
-        }
-    }
-    ```
 
 If you're running the CLI against InfluxDB Cloud Serverless, replace `your-database` in the examples with your Cloud Serverless _bucket name_.
 
 ## Run as a command
 
 ```
 influx3 sql "select * from anomalies"
@@ -171,14 +139,73 @@
 
 The following example shows how to write CSV data from the [`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol):
 
 ```bash
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
+## Config Commands
+
+The `config` command allows you to manage configurations for your application. It has the following subcommands: `create`, `update`, `use`, `delete`, and `list`.
+
+### Create
+
+The `create` subcommand creates a new configuration. It requires the `--name`, `--host`, `--token`, `--database`, and `--org` parameters. The `--active` parameter is optional and can be used to set the new configuration as the active one.
+
+Example usage:
+
+```bash
+influx3.py config create --name="my-config" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --database="<database or bucket name>" --org="<your org ID>" --active
+```
+
+### Update
+
+The `update` subcommand updates an existing configuration. The `--name` parameter is required to specify which configuration to update. All other parameters (`--host`, `--token`, `--database`, `--org`, `--active`) are optional.
+
+Example usage:
+
+```bash
+influx3.py config update --name="my-config" --host="new-host.com"
+```
+
+### Use
+
+The `use` subcommand sets a specific configuration as the active one. The `--name` parameter is required to specify which configuration to use.
+
+Example usage:
+
+```bash
+influx3.py config use --name="my-config"
+```
+
+### Delete
+
+The `delete` subcommand deletes a configuration. The `--name` parameter is required to specify which configuration to delete.
+
+Example usage:
+
+```bash
+influx3.py config delete --name="my-config"
+```
+
+### List
+
+The `list` subcommand lists all the configurations.
+
+Example usage:
+
+```bash
+influx3.py config list
+```
+
+Please replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `"<your token>"`, `"<database or bucket name>"`, and `"<your org ID>"` with your actual values.
+
+
+
+
 ## Client library
 
 The underlying client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
 
 ## Contribution
 
 When developing a new feature for the CLI or the client library, make sure to test your feature in both for breaking changes.
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.0 Summary:
-Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
-InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
-contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown License-File: LICENSE
                                  [Your Image]
  [PyPI_version] [PyPI_downloads] [Lint_Code_Base] [Lint_Code_Base] [Community
                                     Slack]
 # influxdb3-python-cli ## About This repository contains a CLI extension to the
 [influxdb 3.0 python client library](https://github.com/InfluxCommunity/
 influxdb3-python). While this code is built on officially supported APIs, the
 library and CLI here are not officially support by InfluxData. ## Install To
@@ -22,46 +12,64 @@
 the CLI in a _virtual environment_. [See how to create and use a `venv` or
 `conda` Python virtual environment](https://docs.influxdata.com/influxdb/cloud-
 serverless/query-data/execute-queries/flight-sql/python/#create-a-python-
 virtual-environment). - To install the client to a user-specific directory
 (without administrative rights), pass the `--user` flag in the `pip` command. -
 To install the client in your system-wide path, use `sudo` with admin
 privileges. ## Add a config To configure the CLI, do _one_ of the following: -
-Use the `influx3 config` command to create or modify config--for example:
-```bash influx3 config \ --name="my-config" \ --database="" \ --host="us-east-
-1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The output is the
-configuration in a `config.json` file. - In your editor, create or edit the
-`config.json` file, and then save it to the directory where you're using the
-`influx3` command--for example: ```json { "my-config": { "database": "your-
-database", "host": "your-host", "token": "your-token", "org": "your-org-id",
-"active": true } } ``` If you're running the CLI against InfluxDB Cloud
-Serverless, replace `your-database` in the examples with your Cloud Serverless
-_bucket name_. ## Run as a command ``` influx3 sql "select * from anomalies"
-``` ``` influx3 write testmes f=7 ``` ## Query and write interactively In your
-terminal, enter the following command: ``` influx3 ``` `influx3` displays the `
-(>)` interactive prompt and waits for input. ``` Welcome to my IOx CLI. (>) ```
-To query, type `sql` at the prompt. ``` (>) sql ``` At the `(sql >)` prompt,
-enter your query statement: ``` (sql >) select * from home ``` The `influx3`
-CLI displays query results in Markdown table format--for example: ``` | | co |
-hum | room | temp | time | |----:|-----:|------:|:------------|-------:|:------
-------------------------| | 0 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:00 |
-| 1 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:50 | ``` To write, type
-`write` at the `(>)` prompt. ``` (>) write ``` At the `(write >)` prompt, enter
-line protocol data. ``` (>) write home,room=kitchen temp=70.5,hum=80 ``` To
-exit a prompt, enter `exit`. ## Write from a file The InfluxDB CLI and client
-library can write data from a CSV file. The CSV file must contain the
-following: - A header row with column names - A column that contains a
-timestamp for each row The following CLI options specify how data is parsed: *
-`--file` - The path to the csv file. * `--time` - The name of the column
-containing the timestamp. * `--measurement` - The name of the measurment to
-store the CSV data under. (Currently only supports user specified string) * `--
-tags` - (optional) Specify an array of column names to use as tags. (Currently
-only supports user specified strings) for example: `--tags=host,region` The
-following example shows how to write CSV data from the [`./Examples/
-example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/
-main/Examples/example.csv) to InfluxDB (as line protocol): ```bash influx3
-write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags
-host,region ``` ## Client library The underlying client library is also
-available for use in your own code: https://github.com/InfluxCommunity/
-influxdb3-python ## Contribution When developing a new feature for the CLI or
-the client library, make sure to test your feature in both for breaking
-changes. #
+Use the `influx3 create config` command to create or modify config--for
+example: ```bash influx3 create config \ --name="my-config" \ --database="" \ -
+-host="us-east-1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The
+output is the configuration in a `config.json` file. This is saved within a
+directory called `config` located with the influx3 application. If you're
+running the CLI against InfluxDB Cloud Serverless, replace `your-database` in
+the examples with your Cloud Serverless _bucket name_. ## Run as a command ```
+influx3 sql "select * from anomalies" ``` ``` influx3 write testmes f=7 ``` ##
+Query and write interactively In your terminal, enter the following command:
+``` influx3 ``` `influx3` displays the `(>)` interactive prompt and waits for
+input. ``` Welcome to my IOx CLI. (>) ``` To query, type `sql` at the prompt.
+``` (>) sql ``` At the `(sql >)` prompt, enter your query statement: ``` (sql
+>) select * from home ``` The `influx3` CLI displays query results in Markdown
+table format--for example: ``` | | co | hum | room | temp | time | |----:|----
+-:|------:|:------------|-------:|:------------------------------| | 0 | 0 |
+35.9 | Kitchen | 21 | 2023-03-09 08:00:00 | | 1 | 0 | 35.9 | Kitchen | 21 |
+2023-03-09 08:00:50 | ``` To write, type `write` at the `(>)` prompt. ``` (>)
+write ``` At the `(write >)` prompt, enter line protocol data. ``` (>) write
+home,room=kitchen temp=70.5,hum=80 ``` To exit a prompt, enter `exit`. ## Write
+from a file The InfluxDB CLI and client library can write data from a CSV file.
+The CSV file must contain the following: - A header row with column names - A
+column that contains a timestamp for each row The following CLI options specify
+how data is parsed: * `--file` - The path to the csv file. * `--time` - The
+name of the column containing the timestamp. * `--measurement` - The name of
+the measurment to store the CSV data under. (Currently only supports user
+specified string) * `--tags` - (optional) Specify an array of column names to
+use as tags. (Currently only supports user specified strings) for example: `--
+tags=host,region` The following example shows how to write CSV data from the
+[`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-
+python/blob/main/Examples/example.csv) to InfluxDB (as line protocol): ```bash
+influx3 write_csv --file ./Examples/example.csv --measurement table2 --time
+Date --tags host,region ``` ## Config Commands The `config` command allows you
+to manage configurations for your application. It has the following
+subcommands: `create`, `update`, `use`, `delete`, and `list`. ### Create The
+`create` subcommand creates a new configuration. It requires the `--name`, `--
+host`, `--token`, `--database`, and `--org` parameters. The `--active`
+parameter is optional and can be used to set the new configuration as the
+active one. Example usage: ```bash influx3.py config create --name="my-config"
+--host="us-east-1-1.aws.cloud2.influxdata.com" --token="" --database="" --
+org="" --active ``` ### Update The `update` subcommand updates an existing
+configuration. The `--name` parameter is required to specify which
+configuration to update. All other parameters (`--host`, `--token`, `--
+database`, `--org`, `--active`) are optional. Example usage: ```bash influx3.py
+config update --name="my-config" --host="new-host.com" ``` ### Use The `use`
+subcommand sets a specific configuration as the active one. The `--name`
+parameter is required to specify which configuration to use. Example usage:
+```bash influx3.py config use --name="my-config" ``` ### Delete The `delete`
+subcommand deletes a configuration. The `--name` parameter is required to
+specify which configuration to delete. Example usage: ```bash influx3.py config
+delete --name="my-config" ``` ### List The `list` subcommand lists all the
+configurations. Example usage: ```bash influx3.py config list ``` Please
+replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`, `""`,
+and `""` with your actual values. ## Client library The underlying client
+library is also available for use in your own code: https://github.com/
+InfluxCommunity/influxdb3-python ## Contribution When developing a new feature
+for the CLI or the client library, make sure to test your feature in both for
+breaking changes. #
```

### Comparing `influxdb3-python-cli-0.2.0/influxdb_cli/influx3.py` & `influxdb3-python-cli-0.2.1/influxdb_cli/influx3.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import argparse
 import json
 from prompt_toolkit import PromptSession
 from prompt_toolkit.lexers import PygmentsLexer
 from pygments.lexers import SqlLexer
 from influxdb_client_3 import InfluxDBClient3
 import os
+from config_helper import config_helper
 
 _usage_string = """
 to write data use influxdb line protocol:
 > influx3 write testmes,tag1=tagvalue field1=0.0 <optional timestamp>
 
 to read data with sql:
 > influx3 sql select * from testmes where time > now() - interval'1 minute'
@@ -24,51 +25,53 @@
 
 class IOXCLI(cmd.Cmd):
     intro = 'Welcome to my IOx CLI.\n'
     prompt = '(>) '
 
     def __init__(self):
         super().__init__()
-        self._configurations = {}
-        self._load_config()
+        self.config_helper = config_helper()
+        self.active_config = self.config_helper._get_active()
+        self._setup_client()
         self._sql_prompt_session = PromptSession(lexer=PygmentsLexer(SqlLexer))
         self._write_prompt_session = PromptSession(lexer=None)
+       
 
     def do_sql(self, arg):
-        if self._configurations == {}:
+        if self.active_config == {}:
             print("can't query, no active configs")
             return
         try: 
             table = self.influxdb_client.query(query=arg, language="sql")
             print(table.to_pandas().to_markdown())
         except Exception as e:
             print(e)
 
     def do_influxql(self, arg):
-        if self._configurations == {}:
+        if self.active_config == {}:
             print("can't query, no active configs")
             return
         try: 
             table = self.influxdb_client.query(query=arg, language="influxql")
             print(table.to_pandas().to_markdown())
         except Exception as e:
             print(e)
 
     def do_write(self, arg):
-        if self._configurations == {}:
+        if self.active_config == {}:
             print("can't write, no active configs")
             return
         if arg == "":
             print("can't write, no line protocol supplied")
             return
         
         self.influxdb_client.write(record=arg)
     
     def do_write_csv(self, args):
-        if self._configurations == {}:
+        if self.active_config == {}:
             print("can't write, no active configs")
             return
 
         temp = {}
         attributes = ['file', 'measurement', 'time', 'tags']
         temp['tags'] = []
 
@@ -118,58 +121,47 @@
             except KeyboardInterrupt:
                 print(f'Ctrl-D pressed, exiting {mode_name}...')
                 break
             except EOFError:
                 print(f'Ctrl-D pressed, exiting {mode_name}...')
                 break
     
-    def config(self, args):
-        if args.name in self._configurations:
-            config = self._configurations[args.name]
-        else:
-            config = {}
+    def create_config(self, args):
+        self.config_helper._create(args)
 
-        attributes = ['database', 'host', 'token', 'org']
+    
+    def delete_config(self, args):
+        self.config_helper._delete(args)
 
-        for attribute in attributes:
-            arg_value = getattr(args, attribute)
-            if arg_value is not None:
-                config[attribute] = arg_value
+    
+    def list_config(self, args):
+        self.config_helper._list(args)
+    
+    def use_config(self, args):
+        self.config_helper._set_active(args)
 
-        config['active'] = True
 
-        missing_attributes = [attribute for attribute in attributes if attribute not in config]
+    def update_config(self, args):
+        self.config_helper._update(args)
 
-        if missing_attributes:
-            print(f"configuration {args.name} is missing the following required attributes: {missing_attributes}")
 
-        self._configurations[args.name] = config
-        with open('config.json', 'w') as f:
-            f.write(json.dumps(self._configurations))
         
-    
-    def _load_config(self):
-        if not os.path.exists('config.json'):
-            return
-        f = open('config.json', 'r')
+    def _setup_client(self):
+        try:
+            self._database = self.active_config['database']
+
+            self.influxdb_client = InfluxDBClient3(
+                host=self.active_config['host'],
+                org=self.active_config['org'],
+                token=self.active_config['token'],
+                database=self.active_config['database']
+            )
+        except Exception as e:
+            print("No active config found, please run 'config' command to create a new config")
 
-        self._configurations = json.loads(f.read())
-        active_conf = None
-        for c in self._configurations.keys():
-            if self._configurations[c]["active"]:
-                active_conf = self._configurations[c]
-        if active_conf is None:
-            print("no active configuration found")
-        self._database = active_conf['database']
-
-        self.influxdb_client = InfluxDBClient3(host=f"{active_conf['host']}",
-                                                 org=active_conf['org'],
-                                                 token=active_conf['token'],
-                                                 database=active_conf['database']
-                                                 )
 
 class StoreRemainingInput(argparse.Action):
     def __call__(self, parser, database, values, option_string=None):
         setattr(database, self.dest, ' '.join(values))
 
 def parse_args():
     parser = argparse.ArgumentParser(description= _description_string
@@ -187,38 +179,72 @@
     write_csv_parser = subparsers.add_parser('write_csv', help='write CSV data to InfluxDB')
     write_csv_parser.add_argument('--file', help='the CSV file to import', required=True)
     write_csv_parser.add_argument('--measurement', help='Define the name of the measurement', required=True)
     write_csv_parser.add_argument('--time', help='Define the name of the time column with the csv file', required=True)
     write_csv_parser.add_argument('--tags', help='(optional) array of column names which are tags. Format should be: ["tag1", "tag2"]', required=False)
 
     config_parser = subparsers.add_parser("config", help="configure the application")
-    config_parser.add_argument("--name", help="Configuration name", required=True)
-    config_parser.add_argument("--host", help="Host string")
-    config_parser.add_argument("--token", help="Token string")
-    config_parser.add_argument("--database", help="Database string")
-    config_parser.add_argument("--org", help="Organization string")
+    config_subparsers = config_parser.add_subparsers(dest='config_command')
+
+    create_parser = config_subparsers.add_parser("create", help="create a new configuration")
+    create_parser.add_argument("--name", help="Configuration name", required=True)
+    create_parser.add_argument("--host", help="Host string", required=True)
+    create_parser.add_argument("--token", help="Token string", required=True)
+    create_parser.add_argument("--database", help="Database string", required=True)
+    create_parser.add_argument("--org", help="Organization string", required=True)
+    create_parser.add_argument("--active", help="Set this configuration as active", required=False, action='store_true')
+
+        # Update command
+    update_parser = config_subparsers.add_parser("update", help="update an existing configuration")
+    update_parser.add_argument("--name", help="Configuration name", required=True)
+    update_parser.add_argument("--host", help="Host string", required=False)
+    update_parser.add_argument("--token", help="Token string", required=False)
+    update_parser.add_argument("--database", help="Database string", required=False)
+    update_parser.add_argument("--org", help="Organization string", required=False)
+    update_parser.add_argument("--active", help="Set this configuration as active", required=False, action='store_true')
+
+    # Use command
+    use_parser = config_subparsers.add_parser("use", help="use a specific configuration")
+    use_parser.add_argument("--name", help="Configuration name", required=True)
+
+    delete_parser = config_subparsers.add_parser("delete", help="delete a configuration")
+    delete_parser.add_argument("--name", help="Configuration name", required=True)
+
+    list_parser = config_subparsers.add_parser("list", help="list all configurations")
 
     config_parser = subparsers.add_parser("help")
 
     return parser.parse_args()
 
 def main():
     args = parse_args()
     app = IOXCLI()
 
+
     if args.command == 'sql':
         app.do_sql(args.query)
     if args.command == 'influxql':
         app.do_influxql(args.query)
     if args.command == 'write':
         app.do_write(args.line_protocol)
     if args.command == 'write_csv':
         app.do_write_csv(args)
     if args.command == 'config':
-        app.config(args)
+        if args.config_command == 'create':
+            app.create_config(args)
+        elif args.config_command == 'delete':
+            app.delete_config(args)
+        elif args.config_command == 'list':
+            app.list_config(args)
+        elif args.config_command == 'update':
+            app.update_config(args)
+        elif args.config_command == 'use':
+            app.use_config(args)
+        else:
+             print(_usage_string)
     if args.command == 'help':
         print(_usage_string)
     if args.command is None:
         app.cmdloop()
     
 
 if __name__ == '__main__':
```

### Comparing `influxdb3-python-cli-0.2.0/setup.py` & `influxdb3-python-cli-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,34 +14,33 @@
     if not match:
         return None
 
     return match.group(1)
 
 def get_version():
     # If running in GitHub Actions, get version from GITHUB_REF
+
     version = get_version_from_github_ref()
     if version:
         return version
-
-    # Fallback to a default version if not in GitHub Actions
-    return "v0.0.0"
-
+    else:
+        raise "No version found in GITHUB_REF"
 
 
 setup(
     name='influxdb3-python-cli',
     version=get_version(),
     description='Community Python client for InfluxDB 3.0 (CLI)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='InfluxData',
     author_email='contact@influxdata.com',
     url='https://github.com/InfluxCommunity/influxdb-python-cli',
     packages=['influxdb_cli'],
-    install_requires=['influxdb3-python','pathlib', 'pygments', 'prompt_toolkit', 'pandas', 'tabulate'],
+    install_requires=['influxdb3-python', 'pygments', 'prompt_toolkit', 'pandas', 'tabulate'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

