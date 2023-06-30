# Comparing `tmp/openshift_cluster_login-0.9.0.tar.gz` & `tmp/openshift_cluster_login-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_cluster_login-0.9.0.tar", max compression
+gzip compressed data, was "openshift_cluster_login-1.0.0.tar", max compression
```

## Comparing `openshift_cluster_login-0.9.0.tar` & `openshift_cluster_login-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1073 2022-12-21 09:41:00.149783 openshift_cluster_login-0.9.0/LICENSE
--rw-r--r--   0        0        0     5647 2022-12-21 09:41:00.149783 openshift_cluster_login-0.9.0/README.md
--rw-r--r--   0        0        0        0 2022-12-21 09:41:00.161783 openshift_cluster_login-0.9.0/ocl/__init__.py
--rw-r--r--   0        0        0    12629 2022-12-21 09:41:00.165783 openshift_cluster_login-0.9.0/ocl/__main__.py
--rw-r--r--   0        0        0      284 2022-12-21 09:41:00.165783 openshift_cluster_login-0.9.0/ocl/cluster.gql
--rw-r--r--   0        0        0     1508 2022-12-21 09:41:00.165783 openshift_cluster_login-0.9.0/ocl/cluster.py
--rw-r--r--   0        0        0     1056 2022-12-21 09:41:00.165783 openshift_cluster_login-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6771 1970-01-01 00:00:00.000000 openshift_cluster_login-0.9.0/setup.py
--rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 openshift_cluster_login-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-30 13:14:28.760962 openshift_cluster_login-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5176 2023-06-30 13:14:28.760962 openshift_cluster_login-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 13:14:28.772962 openshift_cluster_login-1.0.0/ocl/__init__.py
+-rw-r--r--   0        0        0    11136 2023-06-30 13:14:28.772962 openshift_cluster_login-1.0.0/ocl/__main__.py
+-rw-r--r--   0        0        0      284 2023-06-30 13:14:28.772962 openshift_cluster_login-1.0.0/ocl/cluster.gql
+-rw-r--r--   0        0        0     1508 2023-06-30 13:14:28.772962 openshift_cluster_login-1.0.0/ocl/cluster.py
+-rw-r--r--   0        0        0     1062 2023-06-30 13:14:28.772962 openshift_cluster_login-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6199 1970-01-01 00:00:00.000000 openshift_cluster_login-1.0.0/PKG-INFO
```

### Comparing `openshift_cluster_login-0.9.0/LICENSE` & `openshift_cluster_login-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-0.9.0/README.md` & `openshift_cluster_login-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -42,44 +42,44 @@
 * `OCL_CLUSTER_NAME` - cluster name
 * `OCL_CLUSTER_CONSOLE` - url to cluster console
 
 ## Features
 
 OCL currently provides the following features (get help with `-h` or `--help`):
 
-- OpenShift console login (oc login) via GitHub authentication
+- OpenShift console login (`oc login`) via GitHub or Red Hat authentication
 - Get cluster information from app-interface or user-defined (`OCL_USER_CLUSTERS``)
-- Open OpenShift console in browser (`--open-in-browser`)
+_ Open the OpenShift `console in `the `browser`` (`--open-in-browser`)
 - Shell completion (`--install-completion`, `--show-completion`)
-- Credentials via environment variables or shell command (e.g. [1password CLI](https://developer.1password.com/docs/cli/))
+- Credentials via environment variables or shell command (e.g., [1password CLI](https://developer.1password.com/docs/cli/))
+- Cache App-Interface queries (via GraphQL) for one week
 
 
 ## Environment Variables
 
-| Variable Name                                       | Description                                                                                                                                 | Required           | Default |
-| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------ | ------- |
-| OCL_GITHUB_USERNAME OCL_GITHUB_USERNAME_COMMAND     | Your GitHub username                                                                                                                        | :heavy_check_mark: |         |
-| OCL_GITHUB_PASSWORD OCL_GITHUB_PASSWORD_COMMAND     | Your GitHub password (e.g. command `op read op://Private/Github/password`)                                                                  | :heavy_check_mark: |         |
-| OCL_GITHUB_TOTP OCL_GITHUB_TOTP_COMMAND             | Your GitHub two factor token (e.g. command `op item get Github --otp`)                                                                      | :heavy_check_mark: |         |
-| OCL_WAIT OCL_WAIT_COMMAND                           | Selenium webdriver wait timeout                                                                                                             |                    | 2       |
-| OCL_APP_INTERFACE_URL OCL_APP_INTERFACE_URL_COMMAND | App-Interface URL                                                                                                                           | :heavy_check_mark: |         |
-| OCL_APP_INT_TOKEN OCL_APP_INT_TOKEN_COMMAND         | App-Interface authentication token                                                                                                          | :heavy_check_mark: |         |
-| USER_CLUSTERS USER_CLUSTERS_COMMAND                 | User defined clusters as json format (e.g. `[{"name": "local-kind", "serverUrl": "https://localhost:6443", "consoleUrl": "not available}]`) |                    | "[]"    |
-
-You can either set a variable, e.g. `export OCL_GITHUB_USERNAME="mail@example.com"` or retrieve it via a command, e.g. `export OCL_GITHUB_USERNAME_COMMAND="op read op://Private/Github/username"`
-
+| Variable Name                                       | Description                                                                                                                                 | Default |
+| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
+| OCL_WAIT OCL_WAIT_COMMAND                           | Selenium webdriver wait timeout                                                                                                             | 2       |
+| OCL_APP_INTERFACE_URL OCL_APP_INTERFACE_URL_COMMAND | App-Interface URL                                                                                                                           |         |
+| OCL_APP_INT_TOKEN OCL_APP_INT_TOKEN_COMMAND         | App-Interface authentication token                                                                                                          |         |
+| USER_CLUSTERS USER_CLUSTERS_COMMAND                 | User defined clusters as json format (e.g. `[{"name": "local-kind", "serverUrl": "https://localhost:6443", "consoleUrl": "not available}]`) | "[]"    |
+
+You can either set a variable, e.g. `export OCL_GITHUB_USERNAME="mail@example.com"` or retrieve it via a command, e.g. `export OCL_GITHUB_USERNAME_COMMAND="op read op://Private/Github/username"`.
+If a variable is not set but needed, OCL will ask for it interactively.
+
+## App-Interface
+
+OCL retrieves the cluster information from app-interface via GraphQL (`OCL_APP_INTERFACE_URL`) and caches them
+in your user *cache directory* (on MacOS, e.g., `~/Library/Caches/ocl/gql_cache/`).
+Remove this directory to force a refresh.
 
 ## Limitations
 
-* MacOS only
-* Only Selenium `webdriver.Chrome` is supported and must be installed manually
-  ```shell
-  $ brew install --cask chromedriver
-  ```
-
+* Kerberos authentication only
+* Works only with a Red Hat associate account
 
 ## Development
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
```

### Comparing `openshift_cluster_login-0.9.0/ocl/__main__.py` & `openshift_cluster_login-1.0.0/ocl/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import json
 import logging
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
-import time
 import webbrowser
 from pathlib import Path
 from typing import (
     Any,
     Optional,
     Tuple,
     Union,
@@ -18,26 +17,27 @@
 
 import requests
 import typer
 from appdirs import AppDirs
 from diskcache import Cache
 from flufl.lock import Lock
 from iterfzf import iterfzf
+from pyquery import PyQuery as pq
+from requests_kerberos import (
+    OPTIONAL,
+    HTTPKerberosAuth,
+)
 from rich import print
 from rich.progress import (
     Progress,
     SpinnerColumn,
     TextColumn,
 )
 from rich.prompt import Prompt
 from rich.text import Text
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.remote.webdriver import WebDriver
 
 from .cluster import (
     ClusterQueryData,
     ClusterV1,
     query_string,
 )
 
@@ -65,24 +65,32 @@
           'cx0XNNWWWNX0xc'        'cx0XNNNNWWNX0xc'      oKXKKKXXKKKKKd'
              ;cloooolc;              ;clloooolc;         oKXKKKXXKKKKKd'
 """
 
 app = typer.Typer(rich_markup_mode="rich")
 
 
-def get_var(var_name: str, default: Any = None) -> str:
-    if cmd := os.getenv(f"OCL_{var_name}_COMMAND"):
+def get_var(var_name: str, default: Any = None, hidden: bool = False) -> str:
+    env_var = f"OCL_{var_name}"
+    if cmd := os.getenv(f"{env_var}_COMMAND"):
         return (
             run(cmd, shell=True, check=True, capture_output=True)
             .stdout.decode("utf-8")
             .rstrip("\n")
         )
     if default is not None:
-        return os.environ.get(f"OCL_{var_name}", default)
-    return os.environ[f"OCL_{var_name}"]
+        return os.environ.get(env_var, default)
+
+    if env_var in os.environ:
+        return os.environ[env_var]
+
+    print(
+        f"[bold red]Missing environment variable [bold green]{env_var}[bold green][/bold red]"
+    )
+    return Prompt.ask(f"Enter OCL_{var_name}", password=hidden)
 
 
 def select_cluster(cluster_name: str = "") -> ClusterV1:
     clusters = clusters_from_app_interface()
     # user defined clusters
     clusters += [
         ClusterV1(**c) for c in json.loads(get_var("USER_CLUSTERS", default="[]"))
@@ -94,15 +102,15 @@
         if not cluster_name:
             sys.exit(0)
     return clusters_dict[cluster_name]
 
 
 def gql_query() -> dict[Any, Any]:
     if "gql_data" not in cache:
-        headers = {"Authorization": get_var("APP_INT_TOKEN")}
+        headers = {"Authorization": get_var("APP_INT_TOKEN", hidden=True)}
         res = requests.post(
             url=get_var("APP_INTERFACE_URL"),
             json={"query": query_string()},
             headers=headers,
         )
         res.raise_for_status()
         cache.set("gql_data", res.json()["data"], expire=ONE_WEEK)
@@ -112,15 +120,25 @@
 def clusters_from_app_interface() -> list[ClusterV1]:
     clusters = ClusterQueryData(**gql_query()).clusters or []
     return [c for c in clusters if c.auth]
 
 
 def auth_url(console_url: str, idp: Optional[str]) -> str:
     apps_suffix = ".".join(console_url.split(".")[1:])
-    return f"https://oauth-openshift.{apps_suffix}/oauth/authorize?client_id=openshift-browser-client{'&idp=' + idp if idp else ''}&redirect_uri=https%3A%2F%2Foauth-openshift.{apps_suffix}%2Foauth%2Ftoken%2Fdisplay&response_type=code"
+    if idp:
+        return f"https://oauth-openshift.{apps_suffix}/oauth/authorize?client_id=openshift-browser-client&idp={idp}&redirect_uri=https%3A%2F%2Foauth-openshift.{apps_suffix}%2Foauth%2Ftoken%2Fdisplay&response_type=code"
+    return f"https://oauth-openshift.{apps_suffix}/oauth/token/display"
+
+
+def select_idp(console_url: str, idps: list[str]) -> Optional[str]:
+    for idp in idps:
+        req = requests.get(auth_url(console_url, idp), allow_redirects=False)
+        if req.status_code != 500:
+            return idp
+    return None
 
 
 def kubeconfig(cluster: ClusterV1, temp_kube_config: bool) -> str:
     kc = f"{Path.home()}/.kube/config_{cluster.name}"
     if temp_kube_config:
         _, temp_file = tempfile.mkstemp(prefix=f"ocl.{cluster.name}.")
         shutil.copyfile(kc, temp_file)
@@ -161,38 +179,16 @@
     try:
         run(["oc", "cluster-info"], cluster=cluster)
         return True
     except subprocess.CalledProcessError:
         return False
 
 
-def setup_driver(user_data_dir_path: Path, debug: bool) -> WebDriver:
-    chrome_options = Options()
-    if not debug:
-        chrome_options.add_argument("--headless")
-    chrome_options.add_argument(f"user-data-dir={user_data_dir_path}")
-    driver = webdriver.Chrome(options=chrome_options)
-    driver.implicitly_wait(int(get_var("WAIT", default=2)))
-    return driver
-
-
-def github_login(driver: WebDriver) -> None:
-    login_el = driver.find_element(By.ID, "login_field")
-    login_el.send_keys(get_var("GITHUB_USERNAME"))
-    pass_el = driver.find_element(By.ID, "password")
-    pass_el.send_keys(get_var("GITHUB_PASSWORD"))
-    # submit form
-    driver.find_element(By.CSS_SELECTOR, ".btn-primary").click()
-    # Filling the OTP token - form is auto submitted
-    otp_el = driver.find_element(By.ID, "totp")
-    otp_el.send_keys(get_var("GITHUB_TOTP"))
-
-
 def oc_setup(
-    cluster: ClusterV1, debug: bool, refresh_login: bool, idp: Optional[str] = None
+    cluster: ClusterV1, debug: bool, refresh_login: bool, idps: list[str]
 ) -> None:
     with Progress(
         SpinnerColumn(), TextColumn("[progress.description]{task.description}")
     ) as progress:
         task = progress.add_task(description="Acquiring lock ...", total=1)
         with lock:
             progress.remove_task(task)
@@ -203,56 +199,23 @@
                 )
                 logged_in = oc_check_login(cluster)
                 progress.remove_task(task)
 
             if not refresh_login and logged_in:
                 return
 
-            if idp:
-                # not logged in or login enforced
-                task = progress.add_task(
-                    description="Opening browser headless ...", total=1
-                )
-                driver = setup_driver(
-                    user_data_dir_path=Path(appdirs.user_cache_dir), debug=debug
-                )
-                progress.remove_task(task)
-
-                try:
-                    task = progress.add_task(
-                        description="Retrieving token ...", total=1
+            if idp := select_idp(cluster.console_url, idps=idps):
+                with requests.Session() as session:
+                    session.auth = HTTPKerberosAuth(mutual_authentication=OPTIONAL)
+                    r = session.get(auth_url(cluster.console_url, idp))
+                    form_data = pq(r.text)("form").serialize_dict()
+                    r = session.post(
+                        auth_url(cluster.console_url, idp=None), data=form_data
                     )
-                    driver.get(auth_url(cluster.console_url, idp))
-
-                    if driver.current_url.startswith("https://github.com/login?"):
-                        subtask = progress.add_task(
-                            description="GitHub  login ...", total=1
-                        )
-                        github_login(driver=driver)
-                        progress.remove_task(subtask)
-                        if driver.current_url.startswith(
-                            "https://github.com/login/oauth/authorize?"
-                        ):
-                            # grant access
-                            subtask = progress.add_task(
-                                description="GitHub  authorize app-sre ...", total=1
-                            )
-                            time.sleep(4)
-                            driver.find_element(By.ID, "js-oauth-authorize-btn").click()
-                            progress.remove_task(subtask)
-
-                    # Clicking the "Display Token" button
-                    driver.find_element(By.CSS_SELECTOR, "button").click()
-                    # Getting the auth token
-                    token = driver.find_element(By.TAG_NAME, "code").text
-                    progress.remove_task(task)
-                finally:
-                    for handle in driver.window_handles:
-                        driver.switch_to.window(handle)
-                        driver.close()
+                    token = pq(r.text)("code")[0].text
             else:
                 webbrowser.open(auth_url(cluster.console_url, idp=None))
                 progress.stop()
                 # manual login
                 token = Prompt.ask("Enter token", password=True)
                 progress.start()
 
@@ -281,34 +244,47 @@
 
 def bye():
     print(
         "Thank you for using openshift-login. :man_bowing: Have a great day ahead! :red_heart-emoji:"
     )
 
 
+def enable_requests_logging():
+    from http.client import HTTPConnection
+
+    HTTPConnection.debuglevel = 1
+    logging.getLogger().setLevel(logging.DEBUG)
+    requests_log = logging.getLogger("urllib3")
+    requests_log.setLevel(logging.DEBUG)
+    requests_log.propagate = True
+
+
 @app.command(epilog="Made with :heart: by [blue]https://github.com/chassing[/]")
 def main(
     cluster_name: str = typer.Argument(None, help="Cluster name"),
     project: str = typer.Argument(None, help="Namespace/Project"),
     debug: bool = typer.Option(False, help="Enable debug mode"),
     open_in_browser: bool = typer.Option(
         False, help="Open the console in browser instead of local shell"
     ),
     display_banner: bool = typer.Option(True, help="Display shiny OCL banner"),
     refresh_login: bool = typer.Option(
         False, help="Enforce a new login to refresh the session."
     ),
-    idp: str = typer.Option(
-        "github-app-sre",
-        help="Automatically login via given IDP. Use 'manual' for manual login.",
+    idp: list[str] = typer.Option(
+        ["redhat-app-sre-auth"],
+        help="Automatically login via given IDPs (use in given order, try next one if failed). Use 'manual' for manual login.",
     ),
 ):
     logging.basicConfig(
         level=logging.INFO if not debug else logging.DEBUG, format="%(message)s"
     )
+    if debug:
+        enable_requests_logging()
+
     if display_banner:
         print(blend_text(BANNER, (32, 32, 255), (255, 32, 255)))
 
     if open_in_browser and cluster_name == ".":
         cluster_name = os.environ.get("OCL_CLUSTER_NAME", "")
         if not cluster_name:
             print("[bold red]environment variable OCL_CLUSTER_NAME not set")
@@ -322,21 +298,20 @@
         console_url += f"/k8s/cluster/projects/{project}"
 
     if open_in_browser:
         print(f"[bold green]Opening [/] {console_url}")
         subprocess.run(["open", console_url])
         bye()
         sys.exit(0)
-
     try:
         oc_setup(
             cluster,
             debug=debug,
             refresh_login=refresh_login,
-            idp=idp if idp != "manual" else None,
+            idps=idp,
         )
     except subprocess.CalledProcessError as e:
         print(f"[bold red]'oc login' failed![/]\nException: {e}")
         sys.exit(1)
 
     if project:
         try:
```

### Comparing `openshift_cluster_login-0.9.0/ocl/cluster.py` & `openshift_cluster_login-1.0.0/ocl/cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-0.9.0/pyproject.toml` & `openshift_cluster_login-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "openshift-cluster-login"
-version = "0.9.0"
+version = "1.0.0"
 description = "Openshift cluster login on command line"
 authors = ["Christian Assing <cassing@redhat.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/chassing/ocl"
 packages = [{ include = "ocl" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-selenium = "^4.3.0"
 iterfzf = "^0.5.0"
 requests = "^2.28.1"
 typer = "^0.6.1"
 rich = "^12.5.1"
 appdirs = "^1.4.4"
 pydantic = "^1.9.2"
 "flufl.lock" = "^7.1.1"
 diskcache = "^5.4.0"
-playwright = "^1.28.0"
+requests-kerberos = "^0.14.0"
+pyquery = "^2.0.0"
 
 [tool.poetry.dev-dependencies]
 types-requests = "^2.28.7"
 flake8 = "^5.0.3"
 mypy = "^0.971"
 qenerate = "^0.1.2"
```

### Comparing `openshift_cluster_login-0.9.0/setup.py` & `openshift_cluster_login-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,140 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: openshift-cluster-login
+Version: 1.0.0
+Summary: Openshift cluster login on command line
+Home-page: http://github.com/chassing/ocl
+License: MIT
+Author: Christian Assing
+Author-email: cassing@redhat.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: diskcache (>=5.4.0,<6.0.0)
+Requires-Dist: flufl.lock (>=7.1.1,<8.0.0)
+Requires-Dist: iterfzf (>=0.5.0,<0.6.0)
+Requires-Dist: pydantic (>=1.9.2,<2.0.0)
+Requires-Dist: pyquery (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests-kerberos (>=0.14.0,<0.15.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: typer (>=0.6.1,<0.7.0)
+Project-URL: Repository, http://github.com/chassing/ocl
+Description-Content-Type: text/markdown
 
-packages = \
-['ocl']
+![logo](images/logo-white-bg.png)
+# OCL (OpenShift Login)
 
-package_data = \
-{'': ['*']}
+[![PyPI](https://img.shields.io/pypi/v/openshift-cluster-login)][pypi-link]
+[![PyPI platforms][pypi-platforms]][pypi-link]
+![PyPI - License](https://img.shields.io/pypi/l/openshift-cluster-login)
+[![Release and Package Application](https://github.com/chassing/ocl/actions/workflows/release.yaml/badge.svg)](https://github.com/chassing/ocl/actions/workflows/release.yaml)
 
-install_requires = \
-['appdirs>=1.4.4,<2.0.0',
- 'diskcache>=5.4.0,<6.0.0',
- 'flufl.lock>=7.1.1,<8.0.0',
- 'iterfzf>=0.5.0,<0.6.0',
- 'playwright>=1.28.0,<2.0.0',
- 'pydantic>=1.9.2,<2.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'rich>=12.5.1,<13.0.0',
- 'selenium>=4.3.0,<5.0.0',
- 'typer>=0.6.1,<0.7.0']
-
-entry_points = \
-{'console_scripts': ['ocl = ocl.__main__:app']}
-
-setup_kwargs = {
-    'name': 'openshift-cluster-login',
-    'version': '0.9.0',
-    'description': 'Openshift cluster login on command line',
-    'long_description': '![logo](images/logo-white-bg.png)\n# OCL (OpenShift Login)\n\n[![PyPI](https://img.shields.io/pypi/v/openshift-cluster-login)][pypi-link]\n[![PyPI platforms][pypi-platforms]][pypi-link]\n![PyPI - License](https://img.shields.io/pypi/l/openshift-cluster-login)\n[![Release and Package Application](https://github.com/chassing/ocl/actions/workflows/release.yaml/badge.svg)](https://github.com/chassing/ocl/actions/workflows/release.yaml)\n\nOCL does an automatic login to an OpenShift cluster. It fetches cluster information from app-interface and performs a login via [Selenium](https://selenium-python.readthedocs.io).\n\n## Installation\n\nYou can install this library from [PyPI][pypi-link] with `pip`:\n\n\n```shell\n$ python3 -m pip install openshift-cluster-login\n```\n\nor install it with `pipx`:\n```shell\n$ pipx install openshift-cluster-login\n```\n\nYou can also use `pipx` to run the library without installing it:\n\n```shell\n$ pipx run openshift-cluster-login\n```\n\n## Usage\n\n```shell\n$ ocl\n```\n\n<img src="demo/quickstart.gif"/>\n\nThis spawns a new shell with the following environment variables are set:\n\n* `KUBECONFIG` - path to kubeconfig file\n* `OCL_CLUSTER_NAME` - cluster name\n* `OCL_CLUSTER_CONSOLE` - url to cluster console\n\n## Features\n\nOCL currently provides the following features (get help with `-h` or `--help`):\n\n- OpenShift console login (oc login) via GitHub authentication\n- Get cluster information from app-interface or user-defined (`OCL_USER_CLUSTERS``)\n- Open OpenShift console in browser (`--open-in-browser`)\n- Shell completion (`--install-completion`, `--show-completion`)\n- Credentials via environment variables or shell command (e.g. [1password CLI](https://developer.1password.com/docs/cli/))\n\n\n## Environment Variables\n\n| Variable Name                                       | Description                                                                                                                                 | Required           | Default |\n| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------ | ------- |\n| OCL_GITHUB_USERNAME OCL_GITHUB_USERNAME_COMMAND     | Your GitHub username                                                                                                                        | :heavy_check_mark: |         |\n| OCL_GITHUB_PASSWORD OCL_GITHUB_PASSWORD_COMMAND     | Your GitHub password (e.g. command `op read op://Private/Github/password`)                                                                  | :heavy_check_mark: |         |\n| OCL_GITHUB_TOTP OCL_GITHUB_TOTP_COMMAND             | Your GitHub two factor token (e.g. command `op item get Github --otp`)                                                                      | :heavy_check_mark: |         |\n| OCL_WAIT OCL_WAIT_COMMAND                           | Selenium webdriver wait timeout                                                                                                             |                    | 2       |\n| OCL_APP_INTERFACE_URL OCL_APP_INTERFACE_URL_COMMAND | App-Interface URL                                                                                                                           | :heavy_check_mark: |         |\n| OCL_APP_INT_TOKEN OCL_APP_INT_TOKEN_COMMAND         | App-Interface authentication token                                                                                                          | :heavy_check_mark: |         |\n| USER_CLUSTERS USER_CLUSTERS_COMMAND                 | User defined clusters as json format (e.g. `[{"name": "local-kind", "serverUrl": "https://localhost:6443", "consoleUrl": "not available}]`) |                    | "[]"    |\n\nYou can either set a variable, e.g. `export OCL_GITHUB_USERNAME="mail@example.com"` or retrieve it via a command, e.g. `export OCL_GITHUB_USERNAME_COMMAND="op read op://Private/Github/username"`\n\n\n## Limitations\n\n* MacOS only\n* Only Selenium `webdriver.Chrome` is supported and must be installed manually\n  ```shell\n  $ brew install --cask chromedriver\n  ```\n\n\n## Development\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n\n\nUse [Conventional Commit messages](https://www.conventionalcommits.org).\nThe most important prefixes you should have in mind are:\n\n* `fix:` which represents bug fixes, and correlates to a [SemVer](https://semver.org/)\n  patch.\n* `feat:` which represents a new feature, and correlates to a SemVer minor.\n* `feat!:`,  or `fix!:`, `refactor!:`, etc., which represent a breaking change\n  (indicated by the `!`) and will result in a SemVer major.\n* `chore: release` to create a new release\n\nConsider using an empty commit:\n\n```\ngit commit --allow-empty -m "chore: release"\n```\n\nWhen a commit to the main branch has `Release-As: x.x.x` (case insensitive) in the **commit body**, Release Please will open a new pull request for the specified version.\n```\ngit commit --allow-empty -m "chore: release 2.0.0" -m "Release-As: 2.0.0"\n```\n\n\n[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github\n[github-discussions-link]:  https://github.com/chassing/ocl/discussions\n[pypi-link]:                https://pypi.org/project/openshift-cluster-login/\n[pypi-platforms]:           https://img.shields.io/pypi/pyversions/openshift-cluster-login\n[pypi-version]:             https://badge.fury.io/py/openshift-cluster-login.svg\n',
-    'author': 'Christian Assing',
-    'author_email': 'cassing@redhat.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'http://github.com/chassing/ocl',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+OCL does an automatic login to an OpenShift cluster. It fetches cluster information from app-interface and performs a login via [Selenium](https://selenium-python.readthedocs.io).
 
+## Installation
+
+You can install this library from [PyPI][pypi-link] with `pip`:
+
+
+```shell
+$ python3 -m pip install openshift-cluster-login
+```
+
+or install it with `pipx`:
+```shell
+$ pipx install openshift-cluster-login
+```
+
+You can also use `pipx` to run the library without installing it:
+
+```shell
+$ pipx run openshift-cluster-login
+```
+
+## Usage
+
+```shell
+$ ocl
+```
+
+<img src="demo/quickstart.gif"/>
+
+This spawns a new shell with the following environment variables are set:
+
+* `KUBECONFIG` - path to kubeconfig file
+* `OCL_CLUSTER_NAME` - cluster name
+* `OCL_CLUSTER_CONSOLE` - url to cluster console
+
+## Features
+
+OCL currently provides the following features (get help with `-h` or `--help`):
+
+- OpenShift console login (`oc login`) via GitHub or Red Hat authentication
+- Get cluster information from app-interface or user-defined (`OCL_USER_CLUSTERS``)
+_ Open the OpenShift `console in `the `browser`` (`--open-in-browser`)
+- Shell completion (`--install-completion`, `--show-completion`)
+- Credentials via environment variables or shell command (e.g., [1password CLI](https://developer.1password.com/docs/cli/))
+- Cache App-Interface queries (via GraphQL) for one week
+
+
+## Environment Variables
+
+| Variable Name                                       | Description                                                                                                                                 | Default |
+| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
+| OCL_WAIT OCL_WAIT_COMMAND                           | Selenium webdriver wait timeout                                                                                                             | 2       |
+| OCL_APP_INTERFACE_URL OCL_APP_INTERFACE_URL_COMMAND | App-Interface URL                                                                                                                           |         |
+| OCL_APP_INT_TOKEN OCL_APP_INT_TOKEN_COMMAND         | App-Interface authentication token                                                                                                          |         |
+| USER_CLUSTERS USER_CLUSTERS_COMMAND                 | User defined clusters as json format (e.g. `[{"name": "local-kind", "serverUrl": "https://localhost:6443", "consoleUrl": "not available}]`) | "[]"    |
+
+You can either set a variable, e.g. `export OCL_GITHUB_USERNAME="mail@example.com"` or retrieve it via a command, e.g. `export OCL_GITHUB_USERNAME_COMMAND="op read op://Private/Github/username"`.
+If a variable is not set but needed, OCL will ask for it interactively.
+
+## App-Interface
+
+OCL retrieves the cluster information from app-interface via GraphQL (`OCL_APP_INTERFACE_URL`) and caches them
+in your user *cache directory* (on MacOS, e.g., `~/Library/Caches/ocl/gql_cache/`).
+Remove this directory to force a refresh.
+
+## Limitations
+
+* Kerberos authentication only
+* Works only with a Red Hat associate account
+
+## Development
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+
+
+Use [Conventional Commit messages](https://www.conventionalcommits.org).
+The most important prefixes you should have in mind are:
+
+* `fix:` which represents bug fixes, and correlates to a [SemVer](https://semver.org/)
+  patch.
+* `feat:` which represents a new feature, and correlates to a SemVer minor.
+* `feat!:`,  or `fix!:`, `refactor!:`, etc., which represent a breaking change
+  (indicated by the `!`) and will result in a SemVer major.
+* `chore: release` to create a new release
+
+Consider using an empty commit:
+
+```
+git commit --allow-empty -m "chore: release"
+```
+
+When a commit to the main branch has `Release-As: x.x.x` (case insensitive) in the **commit body**, Release Please will open a new pull request for the specified version.
+```
+git commit --allow-empty -m "chore: release 2.0.0" -m "Release-As: 2.0.0"
+```
+
+
+[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
+[github-discussions-link]:  https://github.com/chassing/ocl/discussions
+[pypi-link]:                https://pypi.org/project/openshift-cluster-login/
+[pypi-platforms]:           https://img.shields.io/pypi/pyversions/openshift-cluster-login
+[pypi-version]:             https://badge.fury.io/py/openshift-cluster-login.svg
 
-setup(**setup_kwargs)
```

