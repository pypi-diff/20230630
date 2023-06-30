# Comparing `tmp/remotivelabs_cli-0.0.1a8.tar.gz` & `tmp/remotivelabs_cli-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotivelabs_cli-0.0.1a8.tar", max compression
+gzip compressed data, was "remotivelabs_cli-0.0.1a9.tar", max compression
```

## Comparing `remotivelabs_cli-0.0.1a8.tar` & `remotivelabs_cli-0.0.1a9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      608 2023-06-19 13:55:54.232642 remotivelabs_cli-0.0.1a8/LICENSE
--rw-r--r--   0        0        0     2095 2023-06-22 08:12:57.643193 remotivelabs_cli-0.0.1a8/README.md
--rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a8/cli/__about__.py
--rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a8/cli/__init__.py
--rw-r--r--   0        0        0     4011 2023-06-21 12:52:00.336557 remotivelabs_cli-0.0.1a8/cli/brokers.py
--rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a8/cli/cloud/__init__.py
--rw-r--r--   0        0        0     3538 2023-06-22 08:03:29.813439 remotivelabs_cli-0.0.1a8/cli/cloud/auth.py
--rw-r--r--   0        0        0     2942 2023-06-28 08:27:04.993369 remotivelabs_cli-0.0.1a8/cli/cloud/auth_keys.py
--rw-r--r--   0        0        0     2323 2023-06-22 08:07:25.218764 remotivelabs_cli-0.0.1a8/cli/cloud/brokers.py
--rw-r--r--   0        0        0     1580 2023-06-21 13:16:22.379502 remotivelabs_cli-0.0.1a8/cli/cloud/cloud_cli.py
--rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a8/cli/cloud/configs.py
--rw-r--r--   0        0        0     1366 2023-06-20 19:11:51.341364 remotivelabs_cli-0.0.1a8/cli/cloud/projects.py
--rw-r--r--   0        0        0     9353 2023-06-28 11:30:46.601114 remotivelabs_cli-0.0.1a8/cli/cloud/recordings.py
--rw-r--r--   0        0        0     3498 2023-06-28 09:33:40.616990 remotivelabs_cli-0.0.1a8/cli/cloud/rest_helper.py
--rw-r--r--   0        0        0     1990 2023-06-20 13:21:18.023240 remotivelabs_cli-0.0.1a8/cli/cloud/service_account_keys.py
--rw-r--r--   0        0        0     1615 2023-06-21 14:06:01.150934 remotivelabs_cli-0.0.1a8/cli/cloud/service_accounts.py
--rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a8/cli/lib/__about__.py
--rw-r--r--   0        0        0     4938 2023-06-21 12:13:16.823623 remotivelabs_cli-0.0.1a8/cli/lib/broker.py
--rw-r--r--   0        0        0      432 2023-06-22 08:58:34.023633 remotivelabs_cli-0.0.1a8/cli/remotive.py
--rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a8/cli/requirements.txt
--rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a8/cli/test/test_simple.py
--rw-r--r--   0        0        0      498 2023-06-28 11:40:42.815263 remotivelabs_cli-0.0.1a8/pyproject.toml
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a8/PKG-INFO
+-rw-r--r--   0        0        0      608 2023-06-19 13:55:54.232642 remotivelabs_cli-0.0.1a9/LICENSE
+-rw-r--r--   0        0        0     2095 2023-06-22 08:12:57.643193 remotivelabs_cli-0.0.1a9/README.md
+-rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a9/cli/__about__.py
+-rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a9/cli/__init__.py
+-rw-r--r--   0        0        0     4011 2023-06-21 12:52:00.336557 remotivelabs_cli-0.0.1a9/cli/brokers.py
+-rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a9/cli/cloud/__init__.py
+-rw-r--r--   0        0        0     3538 2023-06-22 08:03:29.813439 remotivelabs_cli-0.0.1a9/cli/cloud/auth.py
+-rw-r--r--   0        0        0     2942 2023-06-28 08:27:04.993369 remotivelabs_cli-0.0.1a9/cli/cloud/auth_keys.py
+-rw-r--r--   0        0        0     2323 2023-06-22 08:07:25.218764 remotivelabs_cli-0.0.1a9/cli/cloud/brokers.py
+-rw-r--r--   0        0        0     1348 2023-06-28 13:44:40.439138 remotivelabs_cli-0.0.1a9/cli/cloud/cloud_cli.py
+-rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a9/cli/cloud/configs.py
+-rw-r--r--   0        0        0     1366 2023-06-20 19:11:51.341364 remotivelabs_cli-0.0.1a9/cli/cloud/projects.py
+-rw-r--r--   0        0        0    10198 2023-06-28 12:28:20.774338 remotivelabs_cli-0.0.1a9/cli/cloud/recordings.py
+-rw-r--r--   0        0        0     3498 2023-06-28 09:33:40.616990 remotivelabs_cli-0.0.1a9/cli/cloud/rest_helper.py
+-rw-r--r--   0        0        0     1990 2023-06-20 13:21:18.023240 remotivelabs_cli-0.0.1a9/cli/cloud/service_account_keys.py
+-rw-r--r--   0        0        0     1615 2023-06-21 14:06:01.150934 remotivelabs_cli-0.0.1a9/cli/cloud/service_accounts.py
+-rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a9/cli/lib/__about__.py
+-rw-r--r--   0        0        0     4938 2023-06-21 12:13:16.823623 remotivelabs_cli-0.0.1a9/cli/lib/broker.py
+-rw-r--r--   0        0        0      432 2023-06-22 08:58:34.023633 remotivelabs_cli-0.0.1a9/cli/remotive.py
+-rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a9/cli/requirements.txt
+-rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a9/cli/test/test_simple.py
+-rw-r--r--   0        0        0      498 2023-06-28 13:49:00.509600 remotivelabs_cli-0.0.1a9/pyproject.toml
+-rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a9/PKG-INFO
```

### Comparing `remotivelabs_cli-0.0.1a8/LICENSE` & `remotivelabs_cli-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/README.md` & `remotivelabs_cli-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/brokers.py` & `remotivelabs_cli-0.0.1a9/cli/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/auth.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/auth.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/auth_keys.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/auth_keys.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/brokers.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/cloud_cli.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/cloud_cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 import typer
 
 from . import recordings, brokers, configs, auth, service_accounts, projects
 from . import rest_helper as rest
 
 app = typer.Typer()
 
@@ -10,31 +12,23 @@
 def licenses(
         organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
         filter: str = typer.Option("all", help="all, valid, expired")
 ):
     rest.handle_get(f"/api/bu/{organisation}/licenses", {'filter': filter})
 
 
-#@app.command(help="Get your organisation and projects with permissions")
-#def home(
-#        organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
-#):
-#    rest.handle_get(f"/api/bu/{organisation}/me")
-
-
-# @app.command(help="Get your organisation and projects with permissions")
-# def home2():
-#    rest.handle_get(f"/api/home")
-
-
-#@app.command(help="List users in an organisation")
-#def users(
-#        organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
-#):
-#    rest.handle_get(f"/api/bu/{organisation}/users")
+@app.command(help="List your available organisations")
+def organisations():
+    r = rest.handle_get(f"/api/home", return_response=True)
+    if r.status_code == 200:
+        j = list(map(lambda x : x["billableUnitUser"]["billableUnit"]["uid"], r.json()))
+        print(json.dumps(j))
+    else:
+        print(f"Got status code: {r.status_code}")
+        print(r.text)
 
 
 app.add_typer(projects.app, name="projects", help="Manage projects")
 app.add_typer(auth.app, name="auth")
 app.add_typer(brokers.app, name="brokers", help="Manage cloud broker lifecycle")
 app.add_typer(recordings.app, name="recordings", help="Manage recordings")
 app.add_typer(configs.app, name="signal-databases", help="Manage signal databases")
```

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/configs.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/configs.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/projects.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/projects.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/recordings.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/recordings.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,25 +68,27 @@
         body = {"size": "S", 'apiKey': api_key}
     return rest.handle_post(f"/api/project/{project}/brokers/{name}", body=json.dumps(body),
                             return_response=return_response)
 
 
 @app.command(help="Plays all recording files or a single recording")
 def play(recording_session: str = typer.Argument(..., help="Recording session id"),
-         ensure_broker_started: bool = typer.Option(default=False, help="Ensure broker exists, start otherwise"),
          broker: str = typer.Option(..., help="Broker name to play on"),
+         ensure_broker_started: bool = typer.Option(default=False, help="Ensure broker exists, start otherwise"),
+         broker_config_name: str = typer.Option("default", help="Specify a custom broker configuration to use" ),
          project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')):
     with Progress(
             SpinnerColumn(),
             TextColumn("[progress.description]{task.description}"),
             transient=True,
     ) as progress:
         rest.ensure_auth_token()
         v = progress.add_task(description=f"Verifying broker {broker} exists...", total=100)
-        r = requests.get(f'{rest.base_url}/api/project/{project}/brokers/{broker}', headers=rest.headers)
+
+        r = requests.get(f'{rest.base_url}/api/project/{project}/brokers/{broker}', headers=rest.headers, )
         progress.update(v, advance=100.0)
         if r.status_code == 404:
             if ensure_broker_started:
                 progress.add_task(description=f"Starting broker {broker}...", total=1)
                 r = doStart(broker, project, '', return_response=True)
                 if r.status_code != 200:
                     print(r.text)
@@ -101,15 +103,19 @@
         progress.add_task(
             description=f"Uploading recording {recording_session} to {broker} and setting play mode to pause...",
             total=None)
         # if recording_file == "":
         #    rest.handle_get(f"/api/project/{project}/files/recording/{recording_session}/upload",
         #                    params={'brokerName': broker})
         # else:
-        rest.handle_get(f"/api/project/{project}/files/recording/{recording_session}/upload",
+        broker_config_query=""
+        if (broker_config_name != "default"):
+            broker_config_query = f"?brokerConfigName={broker_config_name}"
+
+        rest.handle_get(f"/api/project/{project}/files/recording/{recording_session}/upload{broker_config_query}",
                         params={'brokerName': broker})
 
 
 @app.command(help="Downloads the specified recording file to disk")
 def download_recording_file(
         recording_file_name: str = typer.Argument(..., help="Recording file to download"),
         recording_session: str = typer.Option(..., help="Recording session id that this file belongs to", envvar='REMOTIVE_CLOUD_RECORDING_SESSION'),
@@ -201,14 +207,25 @@
     # print(r.status_code)
     # print(r.headers)
     # print(get_filename_from_cd(r.headers.get('content-disposition')))
     filename = get_filename_from_cd(r.headers.get('content-disposition'))
     open(filename, 'wb').write(r.content)
     print(f'Downloaded file {filename}')
 
+@app.command(help="Downloads the specified broker configuration directory as zip file")
+def delete_configuration(
+        broker_config_name: str = typer.Argument(..., help="Broker config name"),
+        recording_session: str = typer.Option(..., help="Recording session id", envvar='REMOTIVE_CLOUD_RECORDING_SESSION'),
+        project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')
+):
+
+    rest.handle_delete(
+        url=f"/api/project/{project}/files/recording/{recording_session}/configuration/{broker_config_name}")
+
+
 
 def get_filename_from_cd(cd):
     """
     Get filename from content-disposition
     """
     if not cd:
         return None
```

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/rest_helper.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/rest_helper.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/service_account_keys.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/service_account_keys.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/cloud/service_accounts.py` & `remotivelabs_cli-0.0.1a9/cli/cloud/service_accounts.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/cli/lib/broker.py` & `remotivelabs_cli-0.0.1a9/cli/lib/broker.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a8/PKG-INFO` & `remotivelabs_cli-0.0.1a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotivelabs-cli
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: 
 Author: Johan Rask
 Author-email: johan.rask@remotivelabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

