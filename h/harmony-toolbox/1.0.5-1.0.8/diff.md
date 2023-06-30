# Comparing `tmp/harmony_toolbox-1.0.5.tar.gz` & `tmp/harmony_toolbox-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony_toolbox-1.0.5.tar", last modified: Tue Jan 31 04:53:32 2023, max compression
+gzip compressed data, was "harmony_toolbox-1.0.8.tar", last modified: Fri Jun 30 15:15:06 2023, max compression
```

## Comparing `harmony_toolbox-1.0.5.tar` & `harmony_toolbox-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 serviceuser  (1000) serviceuser  (1000)        0 2023-01-31 04:53:32.474864 harmony_toolbox-1.0.5/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2022-12-13 19:10:58.000000 harmony_toolbox-1.0.5/LICENSE
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2021-12-09 23:46:49.000000 harmony_toolbox-1.0.5/MANIFEST.in
--rw-r--r--   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-01-31 04:53:32.474864 harmony_toolbox-1.0.5/PKG-INFO
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-01-26 17:25:29.000000 harmony_toolbox-1.0.5/README.md
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2022-12-09 23:10:58.000000 harmony_toolbox-1.0.5/pyproject.toml
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      133 2022-12-16 04:48:27.000000 harmony_toolbox-1.0.5/requirements.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-01-31 04:53:32.474864 harmony_toolbox-1.0.5/setup.cfg
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2021-12-09 23:46:49.000000 harmony_toolbox-1.0.5/setup.py
-drwxr-xr-x   0 serviceuser  (1000) serviceuser  (1000)        0 2023-01-31 04:53:32.464864 harmony_toolbox-1.0.5/src/
-drwxr-xr-x   0 serviceuser  (1000) serviceuser  (1000)        0 2023-01-31 04:53:32.464864 harmony_toolbox-1.0.5/src/harmony_toolbox.egg-info/
--rw-r--r--   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-01-31 04:53:32.000000 harmony_toolbox-1.0.5/src/harmony_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 serviceuser  (1000) serviceuser  (1000)      344 2023-01-31 04:53:32.000000 harmony_toolbox-1.0.5/src/harmony_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 serviceuser  (1000) serviceuser  (1000)        1 2023-01-31 04:53:32.000000 harmony_toolbox-1.0.5/src/harmony_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 serviceuser  (1000) serviceuser  (1000)        8 2023-01-31 04:53:32.000000 harmony_toolbox-1.0.5/src/harmony_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 serviceuser  (1000) serviceuser  (1000)        0 2023-01-31 04:53:32.474864 harmony_toolbox-1.0.5/src/toolbox/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2022-12-09 23:37:06.000000 harmony_toolbox-1.0.5/src/toolbox/__init__.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1768 2023-01-31 04:53:11.000000 harmony_toolbox-1.0.5/src/toolbox/config.py
--rw-r--r--   0 serviceuser  (1000) serviceuser  (1000)    43414 2023-01-26 17:33:50.000000 harmony_toolbox-1.0.5/src/toolbox/library.py
--rw-r--r--   0 serviceuser  (1000) serviceuser  (1000)    30853 2023-01-31 04:51:35.000000 harmony_toolbox-1.0.5/src/toolbox/toolbox.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-06-30 15:15:06.559696 harmony_toolbox-1.0.8/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/LICENSE
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/MANIFEST.in
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-06-30 15:15:06.560698 harmony_toolbox-1.0.8/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/README.md
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/pyproject.toml
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      151 2023-06-28 21:56:07.000000 harmony_toolbox-1.0.8/requirements.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-06-30 15:15:06.568699 harmony_toolbox-1.0.8/setup.cfg
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/setup.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-06-30 15:15:06.095536 harmony_toolbox-1.0.8/src/
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-06-30 15:15:06.373089 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-06-30 15:15:05.000000 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      344 2023-06-30 15:15:06.000000 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/SOURCES.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        1 2023-06-30 15:15:05.000000 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/dependency_links.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        8 2023-06-30 15:15:05.000000 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-06-30 15:15:06.521301 harmony_toolbox-1.0.8/src/toolbox/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-03-24 16:13:56.000000 harmony_toolbox-1.0.8/src/toolbox/__init__.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     2478 2023-06-30 15:08:41.000000 harmony_toolbox-1.0.8/src/toolbox/config.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    51262 2023-06-28 22:08:54.000000 harmony_toolbox-1.0.8/src/toolbox/library.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    33700 2023-06-28 22:24:38.000000 harmony_toolbox-1.0.8/src/toolbox/toolbox.py
```

### Comparing `harmony_toolbox-1.0.5/LICENSE` & `harmony_toolbox-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.0.5/PKG-INFO` & `harmony_toolbox-1.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony_toolbox
-Version: 1.0.5
+Version: 1.0.8
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.0.5/README.md` & `harmony_toolbox-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.0.5/setup.cfg` & `harmony_toolbox-1.0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = harmony_toolbox
-version = 1.0.5
+version = 1.0.8
 author = EasyNode.PRO
 author_email = support@easynode.pro
 description = Harmony ONE Validator Node Toolbox and Easy Setup
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/easy-node-pro/harmony-toolbox
 project_urls =
```

### Comparing `harmony_toolbox-1.0.5/src/harmony_toolbox.egg-info/PKG-INFO` & `harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony-toolbox
-Version: 1.0.5
+Version: 1.0.8
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.0.5/src/toolbox/library.py` & `harmony_toolbox-1.0.8/src/toolbox/library.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import psutil, platform, dotenv, time, os, subprocess, requests, pyhmy, shutil, hashlib, re
+import psutil, platform, dotenv, os, subprocess, requests, pyhmy, shutil, hashlib, re, json, subprocess
 from os import environ
 from dotenv import load_dotenv
 from simple_term_menu import TerminalMenu
-from colorama import Fore, Style
+from colorama import Fore, Style, Back
 from pathlib import Path
-from pyhmy import validator, account, staking, numbers
+from pyhmy import account, staking, validator, numbers
 from json import load, dump
-from toolbox.config import easy_env
+from toolbox.config import EnvironmentVariables
 from collections import namedtuple
 from datetime import datetime
+from subprocess import PIPE, run
 
-load_dotenv(easy_env.dotenv_file)
+load_dotenv(EnvironmentVariables.dotenv_file)
 
 
 class print_stuff:
     def __init__(self, reset: int = 0):
         self.reset = reset
         self.print_stars = "*" * 93
         self.reset_stars = self.print_stars + Style.RESET_ALL + Fore.GREEN
@@ -38,14 +39,15 @@
 
 print_whitespace = print_stuff.printWhitespace
 print_stars = print_stuff().printStars
 string_stars = print_stuff().stringStars
 print_stars_reset = print_stuff(reset=1).printStars
 string_stars_reset = print_stuff(reset=1).stringStars
 
+
 # check if a var exists in your .env file, unset and reset if exists to avoid bad stuff
 def set_var(env_file, key_name, update_name):
     if environ.get(key_name):
         dotenv.unset_key(env_file, key_name)
     dotenv.set_key(env_file, key_name, update_name)
     load_var_file(env_file)
     return
@@ -72,17 +74,18 @@
                             ____ ____ ____ ____ ____ ____ ____                          
                             ||T |||o |||o |||l |||b |||o |||x ||                         
                             ||__|||__|||__|||__|||__|||__|||__||                         
                             |/__\|/__\|/__\|/__\|/__\|/__\|/__\|   
     """
     print(p)
 
+
 # Install Harmony ONE
 def install_hmy():
-    os.chdir(f"{easy_env.harmony_dir}")
+    os.chdir(f"{EnvironmentVariables.harmony_dir}")
     os.system(f"curl -LO https://harmony.one/hmycli && mv hmycli hmy && chmod +x hmy")
     print_stars()
     print("* hmy application installed.")
 
 
 # Code to update the harmony.conf after an upgrade and other text files.
 def update_text_file(fileName, originalText, newText):
@@ -97,69 +100,220 @@
 
 # Setup a wallet, ask if they need to import one (not required but no toolbox menu without a wallet)
 def recover_wallet():
     question = ask_yes_no(f"* Would you like to import a wallet? (YES/NO) ")
     # if yes, find recovery type
     if question:
         recovery_type()
-        load_var_file(easy_env.dotenv_file)
+        load_var_file(EnvironmentVariables.dotenv_file)
         print(
-            f'\n* Verify the address above matches the address below:\n* Detected Wallet: {Fore.YELLOW}{environ.get("VALIDATOR_WALLET")}{Fore.GREEN}\n* If a different wallet is showing you can remove it and retry it after installation.\n*\n* .{easy_env.hmy_app} keys remove {easy_env.active_user}\n*\n* To restore a wallet once again, run the following:\n*\n* .{easy_env.hmy_app} keys recover-from-mnemonic {easy_env.active_user} {environ.get("PASS_SWITCH")}\n*'
+            f'\n* Verify the address above matches the address below:\n* Detected Wallet: {Fore.YELLOW}{environ.get("VALIDATOR_WALLET")}{Fore.GREEN}\n* If a different wallet is showing you can remove it and retry it after installation.\n*\n* .{EnvironmentVariables.hmy_app} keys remove {EnvironmentVariables.active_user}\n*\n* To restore a wallet once again, run the following:\n*\n* .{EnvironmentVariables.hmy_app} keys recover-from-mnemonic {EnvironmentVariables.active_user} {environ.get("PASS_SWITCH")}\n*'
         )
         print_stars()
         input("* Verify your wallet information above.\n* Press ENTER to continue Installation.")
     else:
         wallet = input(
             f"* If you'd like to use the management menu, we need a one1 address, please input your address now: "
         )
-        set_var(easy_env.dotenv_file, "VALIDATOR_WALLET", wallet)
+        set_var(EnvironmentVariables.dotenv_file, "VALIDATOR_WALLET", wallet)
         return
 
 
 def pull_harmony_update(harmony_dir, bls_key_file, harmony_conf):
     arch = os.uname().machine
     os.chdir(f"{harmony_dir}")
     if environ.get("NETWORK") == "testnet":
         os.system("curl -LO https://harmony.one/binary_testnet && mv binary_testnet harmony && chmod +x harmony")
         os.system("./harmony config dump --network testnet harmony.conf")
         update_text_file(harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
     if environ.get("NETWORK") == "mainnet":
-        if arch.startswith('arm'):
+        if arch.startswith("arm"):
             os.system("curl -LO https://harmony.one/binary-arm64 && mv binary-arm64 harmony && chmod +x harmony")
-        if arch == 'x86_64':
+        if arch == "x86_64":
             os.system("curl -LO https://harmony.one/binary && mv binary harmony && chmod +x harmony")
             os.system("./harmony config dump harmony.conf")
             update_text_file(harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
     print_stars()
     print("* harmony.conf MaxKeys modified to 13")
     if os.path.exists(bls_key_file):
         update_text_file(harmony_conf, 'PassFile = ""', f'PassFile = "blskey.pass"')
         print("* blskey.pass found, updated harmony.conf")
     print_stars()
     print(f"* Harmony {environ.get('NETWORK')} application installed & ~/harmony/harmony.conf created. ")
     return
 
 
+# Search harmony.conf for the proper port to hit
+def find_port(folder):
+    with open(f"{EnvironmentVariables.user_home_dir}/{folder}/harmony.conf") as f:
+        data_file = f.readlines()
+    count = 0
+    for line in data_file:
+        line = line.rstrip()
+        if "Port =" in line:
+            if count == 3:
+                return line[9:]
+            count += 1
+
+
+# build list of installs
+def get_folders():
+    folders = {}
+    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony/harmony.conf"):
+        port = find_port(f"harmony")
+        folders["harmony"] = port
+        print(f"* Found ~/harmony folder, on port {port}")
+        print_stars()
+    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony0/harmony.conf"):
+        port = find_port(f"harmony0")
+        folders["harmony0"] = port
+        print(f"* Found ~/harmony1 folder, on port {port}")
+        print_stars()
+    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony1/harmony.conf"):
+        port = find_port(f"harmony1")
+        folders["harmony1"] = port
+        print(f"* Found ~/harmony1 folder, on port {port}")
+        print_stars()
+    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony2/harmony.conf"):
+        port = find_port(f"harmony2")
+        folders["harmony2"] = port
+        print(f"* Found ~/harmony2 folder, on port {port}")
+        print_stars()
+    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony3/harmony.conf"):
+        port = find_port(f"harmony3")
+        folders["harmony3"] = port
+        print(f"* Found ~/harmony3 folder, on port {port}")
+        print_stars()
+    return folders
+
+
+def validator_stats_output(folders) -> None:
+    # Get server stats & wallet balances
+    load_1, load_5, load_15 = os.getloadavg()
+    sign_percentage = get_sign_pct()
+    total_balance = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
+    # Print Menu
+    print_stars()
+    print(
+        f"{Fore.GREEN}* harmony-toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{EnvironmentVariables.easy_version}{Style.RESET_ALL}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*"
+    )
+    print_stars()
+    print(
+        f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(EnvironmentVariables.rpc_endpoints, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {EnvironmentVariables.server_host_name} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
+    )
+    for folder in folders:
+        harmony_service_status(folder)
+    print(
+        f"* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current user home dir free space: {Fore.CYAN}{free_space_check(EnvironmentVariables.user_home_dir): >6}{Fore.GREEN}"
+    )
+    print(
+        f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min"
+    )
+    print_stars()
+    remote_shard_0 = [
+        f"{EnvironmentVariables.user_home_dir}/{list(folders.items())[0][0]}/hmy",
+        "utility",
+        "metadata",
+        f"--node=https://api.s0.t.hmny.io",
+    ]
+    result_shard_0 = run(remote_shard_0, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+    remote_0_data = json.loads(result_shard_0.stdout)
+    print(
+        f"* Remote Shard 0 Epoch: {remote_0_data['result']['current-epoch']}, Current Block: {remote_0_data['result']['current-block-number']}"
+    )
+    print_stars()
+    for folder in folders:
+        current_full_path = f"{EnvironmentVariables.user_home_dir}/{folder}"
+        software_versions = version_checks(current_full_path)
+        print(
+            f'* Results for the current folder: {current_full_path}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
+        )
+        local_server = [
+            f"{EnvironmentVariables.user_home_dir}/{folder}/hmy",
+            "utility",
+            "metadata",
+            f"--node=http://localhost:{folders[folder]}",
+        ]
+        result_local_server = run(local_server, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+        local_data = json.loads(result_local_server.stdout)
+        remote_server = [
+            f"{EnvironmentVariables.user_home_dir}/{folder}/hmy",
+            "utility",
+            "metadata",
+            f"--node=https://api.s{local_data['result']['shard-id']}.t.hmny.io",
+        ]
+        result_remote_server = run(remote_server, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+        remote_data = json.loads(result_remote_server.stdout)
+        print(
+            f"* Remote Shard {local_data['result']['shard-id']} Epoch: {remote_data['result']['current-epoch']}, Current Block: {remote_data['result']['current-block-number']}"
+        )
+        print(
+            f"*  Local Shard {local_data['result']['shard-id']} Epoch: {local_data['result']['current-epoch']}, Current Block: {(local_data['result']['current-block-number'])}\n*   Local Shard 0 Size: {get_db_size(f'{current_full_path}', '0')}\n*   Local Shard {local_data['result']['shard-id']} Size: {get_db_size(f'{current_full_path}', local_data['result']['shard-id'])}"
+        )
+        print_stars()
+
+
+def harmony_service_status(service="harmony") -> None:
+    status = subprocess.call(["systemctl", "is-active", "--quiet", service])
+    if status == 0:
+        if service == "harmony":
+            print(
+                f"* {service} Service is:               "
+                + Fore.BLACK
+                + Back.GREEN
+                + "   Online  "
+                + Style.RESET_ALL
+                + Fore.GREEN
+            )
+        else:
+            print(
+                f"* {service} Service is:              "
+                + Fore.BLACK
+                + Back.GREEN
+                + "   Online  "
+                + Style.RESET_ALL
+                + Fore.GREEN
+            )
+    else:
+        print(
+            f"* {service} Service is:               "
+            + Fore.WHITE
+            + Back.RED
+            + "  *** Offline *** "
+            + Style.RESET_ALL
+            + Fore.GREEN
+        )
+
+
 def set_wallet_env():
     if environ.get("NODE_WALLET") == "true":
         if not environ.get("VALIDATOR_WALLET"):
-            output = subprocess.getoutput(f"{easy_env.hmy_app} keys list | grep {easy_env.active_user}")
-            output_stripped = output.lstrip(easy_env.active_user)
+            output = subprocess.getoutput(
+                f"{EnvironmentVariables.hmy_app} keys list | grep {EnvironmentVariables.active_user}"
+            )
+            output_stripped = output.lstrip(EnvironmentVariables.active_user)
             output_stripped = output_stripped.strip()
-            set_var(easy_env.dotenv_file, "VALIDATOR_WALLET", output_stripped)
+            set_var(EnvironmentVariables.dotenv_file, "VALIDATOR_WALLET", output_stripped)
             return output_stripped
         else:
-            load_var_file(easy_env.dotenv_file)
+            load_var_file(EnvironmentVariables.dotenv_file)
             validator_wallet = environ.get("VALIDATOR_WALLET")
             return validator_wallet
 
 
+def get_db_size(harmony_dir, our_shard) -> str:
+    harmony_db_size = subprocess.getoutput(f"du -h {harmony_dir}/harmony_db_{our_shard}")
+    harmony_db_size = harmony_db_size.rstrip("\t")
+    countTrim = len(EnvironmentVariables.harmony_dir) + 13
+    return harmony_db_size[:-countTrim]
+
+
 def recovery_type():
     subprocess.run("clear")
-    set_var(easy_env.dotenv_file, "NODE_WALLET", "true")
+    set_var(EnvironmentVariables.dotenv_file, "NODE_WALLET", "true")
     passphrase_status()
     passphrase_switch = environ.get("PASS_SWITCH")
     print_stars()
     print("* Wallet Recovery Type!                                                                     *")
     print_stars()
     print("* [0] = Mnemonic phrase recovery (aka seed phrase)                                          *")
     print("* [1] = Private Key recovery                                                                *")
@@ -170,61 +324,65 @@
     ]
     terminal_menu = TerminalMenu(
         menu_options, title="* Which type of restore method would you like to use for your validator wallet?"
     )
     results = terminal_menu.show()
     if results == 0:
         # Mnemonic Recovery Here
-        os.system(f"{easy_env.hmy_app} keys recover-from-mnemonic {easy_env.active_user} {passphrase_switch}")
+        os.system(
+            f"{EnvironmentVariables.hmy_app} keys recover-from-mnemonic {EnvironmentVariables.active_user} {passphrase_switch}"
+        )
         print_stars()
         set_wallet_env()
     elif results == 1:
         # Private Key Recovery Here
         print("* Private key recovery requires your private information in the command itself.")
         private = input("* Please enter your private key to restore your wallet: ")
-        os.system(f"{easy_env.hmy_app} keys import-private-key {private} {easy_env.active_user} --passphrase")
+        os.system(
+            f"{EnvironmentVariables.hmy_app} keys import-private-key {private} {EnvironmentVariables.active_user} --passphrase"
+        )
         print_stars()
         set_wallet_env()
 
 
 def passphrase_status():
-    load_var_file(easy_env.dotenv_file)
+    load_var_file(EnvironmentVariables.dotenv_file)
     if environ.get("NODE_WALLET") == "true":
         passphrase_set()
         set_var(
-            easy_env.dotenv_file,
+            EnvironmentVariables.dotenv_file,
             "PASS_SWITCH",
-            f"--passphrase-file {easy_env.harmony_dir}/passphrase.txt",
+            f"--passphrase-file {EnvironmentVariables.harmony_dir}/passphrase.txt",
         )
     if environ.get("NODE_WALLET") == "false":
-        set_var(easy_env.dotenv_file, "PASS_SWITCH", "--passphrase")
+        set_var(EnvironmentVariables.dotenv_file, "PASS_SWITCH", "--passphrase")
 
 
 def passphrase_set():
-    if os.path.exists(easy_env.password_path):
+    if os.path.exists(EnvironmentVariables.password_path):
         return
     import getpass
 
-    print(f"* Setup {easy_env.harmony_dir}/passphrase.txt file for use with autobidder & harmony-toolbox.")
+    print(f"* Setup {EnvironmentVariables.harmony_dir}/passphrase.txt file for use with autobidder & harmony-toolbox.")
     print_stars()
     # take input
     while True:
         print("* ")
         password_1 = getpass.getpass(
             prompt="* Please set a wallet password for this node\n* Enter your password now: ", stream=None
         )
         password_2 = getpass.getpass(prompt="* Re-enter your password: ", stream=None)
         if not password_1 == password_2:
             print("* Passwords do NOT match, Please try again..")
         else:
             print("* Passwords Match!")
             break
     # Save file, we won't encrypt because if someone has access to the file, they will also have the salt and decrypt code at their disposal.
-    save_text(easy_env.password_path, password_1)
-    load_var_file(easy_env.dotenv_file)
+    save_text(EnvironmentVariables.password_path, password_1)
+    load_var_file(EnvironmentVariables.dotenv_file)
     passphrase_status()
 
 
 def process_command(command: str) -> None:
     process = subprocess.Popen(command, shell=True)
     output, error = process.communicate()
 
@@ -276,20 +434,20 @@
             "[0] - Shard 0",
             "[1] - Shard 1",
             "[2] - Shard 2",
             "[3] - Shard 3",
         ]
         terminal_menu = TerminalMenu(menu_options, title="* Which Shard will this node operate on? ")
         our_shard = str(terminal_menu.show())
-        set_var(easy_env.dotenv_file, "SHARD", our_shard)
+        set_var(EnvironmentVariables.dotenv_file, "SHARD", our_shard)
         return our_shard
 
 
 def get_node_type() -> None:
-    if not os.path.exists(easy_env.hmy_wallet_store):
+    if not os.path.exists(EnvironmentVariables.hmy_wallet_store):
         if environ.get("NODE_TYPE") == None:
             subprocess.run("clear")
             print_stars()
             print("* Which type of node would you like to run on this server?                                  *")
             print_stars()
             print("* [0] - Standard w/ Wallet - Harmony Validator Signing Node with Wallet                     *")
             print("* [1] - Standard No Wallet - Harmony Validator Signing Node no Wallet                       *")
@@ -299,28 +457,28 @@
                 "[0] Signing Node w/ Wallet",
                 "[1] Signing Node No Wallet",
                 "[2] Full Node Non Validating Dev/RPC",
             ]
             terminal_menu = TerminalMenu(menu_options, title="Regular or Full Node Server")
             results = terminal_menu.show()
             if results == 0:
-                set_var(easy_env.dotenv_file, "NODE_TYPE", "regular")
-                set_var(easy_env.dotenv_file, "NODE_WALLET", "true")
+                set_var(EnvironmentVariables.dotenv_file, "NODE_TYPE", "regular")
+                set_var(EnvironmentVariables.dotenv_file, "NODE_WALLET", "true")
             if results == 1:
-                set_var(easy_env.dotenv_file, "NODE_TYPE", "regular")
-                set_var(easy_env.dotenv_file, "NODE_WALLET", "false")
+                set_var(EnvironmentVariables.dotenv_file, "NODE_TYPE", "regular")
+                set_var(EnvironmentVariables.dotenv_file, "NODE_WALLET", "false")
             if results == 2:
-                set_var(easy_env.dotenv_file, "NODE_TYPE", "full")
+                set_var(EnvironmentVariables.dotenv_file, "NODE_TYPE", "full")
             subprocess.run("clear")
             return
         set_wallet_env()
     if not environ.get("NODE_TYPE"):
-        set_var(easy_env.dotenv_file, "NODE_TYPE", "regular")
+        set_var(EnvironmentVariables.dotenv_file, "NODE_TYPE", "regular")
     if not environ.get("NODE_WALLET"):
-        set_var(easy_env.dotenv_file, "NODE_WALLET", "true")
+        set_var(EnvironmentVariables.dotenv_file, "NODE_WALLET", "true")
 
 
 def set_main_or_test() -> None:
     if not environ.get("NETWORK"):
         subprocess.run("clear")
         print_stars()
         print("* Setup config not found, which blockchain does this node run on?                           *")
@@ -331,23 +489,23 @@
         menu_options = [
             "[0] Mainnet",
             "[1] Testnet",
         ]
         terminal_menu = TerminalMenu(menu_options, title="Mainnet or Testnet")
         results = terminal_menu.show()
         if results == 0:
-            set_var(easy_env.dotenv_file, "NETWORK", "mainnet")
-            set_var(easy_env.dotenv_file, "NETWORK_SWITCH", "t")
-            set_var(easy_env.dotenv_file, "RPC_NET", "https://rpc.s0.t.hmny.io")
-            set_var(easy_env.dotenv_file, "RPC_NET_SHARD", f"https://rpc.s{environ.get('SHARD')}.t.hmny.io")
+            set_var(EnvironmentVariables.dotenv_file, "NETWORK", "mainnet")
+            set_var(EnvironmentVariables.dotenv_file, "NETWORK_SWITCH", "t")
+            set_var(EnvironmentVariables.dotenv_file, "RPC_NET", "https://rpc.s0.t.hmny.io")
+            set_var(EnvironmentVariables.dotenv_file, "RPC_NET_SHARD", f"https://rpc.s{environ.get('SHARD')}.t.hmny.io")
         if results == 1:
-            set_var(easy_env.dotenv_file, "NETWORK", "testnet")
-            set_var(easy_env.dotenv_file, "NETWORK_SWITCH", "b")
-            set_var(easy_env.dotenv_file, "RPC_NET", "https://rpc.s0.b.hmny.io")
-            set_var(easy_env.dotenv_file, "RPC_NET_SHARD", f"https://rpc.s{environ.get('SHARD')}.b.hmny.io")
+            set_var(EnvironmentVariables.dotenv_file, "NETWORK", "testnet")
+            set_var(EnvironmentVariables.dotenv_file, "NETWORK_SWITCH", "b")
+            set_var(EnvironmentVariables.dotenv_file, "RPC_NET", "https://rpc.s0.b.hmny.io")
+            set_var(EnvironmentVariables.dotenv_file, "RPC_NET_SHARD", f"https://rpc.s{environ.get('SHARD')}.b.hmny.io")
         subprocess.run("clear")
     return
 
 
 def get_express_status() -> None:
     if environ.get("SETUP_STATUS") == "0":
         subprocess.run("clear")
@@ -357,49 +515,35 @@
         print("* Would you like the turbo express setup or Manual approval of each step?                   *")
         print_stars()
         menu_options = [
             "[0] - Express Install",
             "[1] - Manual Approval",
         ]
         terminal_menu = TerminalMenu(menu_options, title="* Express Or Manual Setup")
-        set_var(easy_env.dotenv_file, "EXPRESS", str(terminal_menu.show()))
+        set_var(EnvironmentVariables.dotenv_file, "EXPRESS", str(terminal_menu.show()))
 
 
 def get_wallet_address():
     print("* Signing Node, No Wallet!                                                                  *")
     print("* You are attempting to launch the menu but no wallet has been loaded, as you chose         *")
     print("* If you would like to use the menu on the server, complete the following:                  *")
     print_stars()
     print("* Edit ~/.easynode.env and add your wallet address on a new line like this example:         *")
     print("* VALIDATOR_WALLET='one1thisisjustanexamplewalletreplaceme'                                 *")
     print_stars()
     raise SystemExit(0)
 
 
-def set_api_paths():
-    if not environ.get("NETWORK_0_CALL"):
-        set_var(
-            easy_env.dotenv_file,
-            "NETWORK_0_CALL",
-            f"{easy_env.hmy_app} --node='https://api.s0.{environ.get('NETWORK_SWITCH')}.hmny.io' ",
-        )
-        set_var(
-            easy_env.dotenv_file,
-            "NETWORK_S_CALL",
-            f"{easy_env.hmy_app} --node='https://api.s{environ.get('SHARD')}.{environ.get('NETWORK_SWITCH')}.hmny.io' ",
-        )
-
-
 def get_validator_info():
     if environ.get("NETWORK") == "mainnet":
-        endpoint = len(easy_env.rpc_endpoints)
+        endpoint = len(EnvironmentVariables.rpc_endpoints)
     if environ.get("NETWORK") == "testnet":
-        endpoint = len(easy_env.rpc_endpoints_test)
+        endpoint = len(EnvironmentVariables.rpc_endpoints_test)
     current = 0
-    max_tries = easy_env.rpc_endpoints_max_connection_retries
+    max_tries = EnvironmentVariables.rpc_endpoints_max_connection_retries
     validator_data = -1
 
     while current < max_tries:
         try:
             validator_data = staking.get_validator_information(environ.get("VALIDATOR_WALLET"), endpoint)
             return validator_data
         except Exception:
@@ -407,40 +551,35 @@
             continue
 
     return validator_data
 
 
 def current_price():
     try:
-        response = requests.get(easy_env.onePriceURL, timeout=5)
+        response = requests.get(EnvironmentVariables.onePriceURL, timeout=5)
     except (ValueError, KeyError, TypeError):
         response = "0.0000"
         return response
     data_dict = response.json()
     type(data_dict)
     data_dict.keys()
     return data_dict["lastPrice"][:-4]
 
 
 def get_wallet_balance(wallet_addr):
-    endpoints_count = len(easy_env.rpc_endpoints)
-
-    for i in range(endpoints_count):
-        wallet_balance = get_wallet_balance_by_endpoint(easy_env.rpc_endpoints[i], wallet_addr)
-        wallet_balance_test = get_wallet_balance_by_endpoint(easy_env.rpc_endpoints_test[i], wallet_addr)
-
-        if wallet_balance >= 0 and wallet_balance_test >= 0:
-            return wallet_balance, wallet_balance_test
-
-    raise ConnectionError("Couldn't fetch RPC data for current epoch.")
+    config = EnvironmentVariables()
+    rpc_endpoint = config.working_rpc_endpoint
+    wallet_balance = get_wallet_balance_by_endpoint(rpc_endpoint, wallet_addr)
+    if wallet_balance is not None:
+        return wallet_balance
 
 
 def get_wallet_balance_by_endpoint(endpoint, wallet_addr):
     current = 0
-    max_tries = easy_env.rpc_endpoints_max_connection_retries
+    max_tries = EnvironmentVariables.rpc_endpoints_max_connection_retries
     get_balance = 0
 
     while current < max_tries:
         try:
             get_balance = pyhmy.numbers.convert_atto_to_one(account.get_balance(wallet_addr, endpoint))
             return get_balance
         except Exception:
@@ -460,15 +599,15 @@
             return wallet_balance
 
     raise ConnectionError("Couldn't fetch RPC data for current epoch.")
 
 
 def get_rewards_balance_by_endpoint(endpoint, wallet_addr):
     current = 0
-    max_tries = easy_env.rpc_endpoints_max_connection_retries
+    max_tries = EnvironmentVariables.rpc_endpoints_max_connection_retries
     totalRewards = 0
 
     try:
         validator_rewards = staking.get_delegations_by_delegator(wallet_addr, endpoint)
     except Exception:
         return totalRewards
 
@@ -501,83 +640,90 @@
     for i in walletBalance["result"]:
         totalRewards = totalRewards + i["reward"]
     totalRewards = "{:,}".format(round(totalRewards * 0.000000000000000001, 2))
     return totalRewards
 
 
 def get_sign_pct() -> str:
+    config = EnvironmentVariables()
+    hmy_external_rpc = f"{EnvironmentVariables.hmy_app} --node='{config.working_rpc_endpoint}'"
     output = subprocess.getoutput(
-        f"{environ.get('NETWORK_0_CALL')} blockchain validator information {environ.get('VALIDATOR_WALLET')} | grep signing-percentage"
+        f"{hmy_external_rpc} blockchain validator information {environ.get('VALIDATOR_WALLET')} | grep signing-percentage"
     )
     output_stripped = output.lstrip('        "current-epoch-signing-percentage": "').rstrip('",')
     try:
         math = float(output_stripped)
         signPerc = math * 100
         roundSignPerc = round(signPerc, 6)
         return str(roundSignPerc)
     except (OSError, ValueError):
         output_stripped = "0"
         return str(output_stripped)
 
 
 def get_local_version(folder):
     harmony_version = subprocess.getoutput(f"{folder}/harmony -V")
-    output_harmony_version = re.search(r'version (v\d+-v\d+\.\d+\.\d+-\d+-g[0-9a-f]+ )\(', harmony_version)
+    output_harmony_version = re.search(r"version (v\d+-v\d+\.\d+\.\d+-\d+-g[0-9a-f]+ )\(", harmony_version)
     hmy_version = subprocess.getoutput(f"{folder}/hmy version")
     return output_harmony_version.group(1)[:-2], hmy_version[62:-15]
 
+
 def set_mod_x(file):
     subprocess.run(["chmod", "+x", file])
 
 
 def check_online_version():
     try:
         subprocess.check_output(
-            ["wget", "https://harmony.one/binary", "-O", easy_env.harmony_tmp_path], stderr=subprocess.STDOUT
+            ["wget", "https://harmony.one/binary", "-O", EnvironmentVariables.harmony_tmp_path],
+            stderr=subprocess.STDOUT,
         )
-        set_mod_x(easy_env.harmony_tmp_path)
-        harmony_ver = subprocess.getoutput(f"{easy_env.harmony_tmp_path} -V")
-        output_harmony_version = re.search(r'version (v\d+-v\d+\.\d+\.\d+-\d+-g[0-9a-f]+ )\(', harmony_ver)
+        set_mod_x(EnvironmentVariables.harmony_tmp_path)
+        harmony_ver = subprocess.getoutput(f"{EnvironmentVariables.harmony_tmp_path} -V")
+        output_harmony_version = re.search(r"version (v\d+-v\d+\.\d+\.\d+-\d+-g[0-9a-f]+ )\(", harmony_ver)
     except subprocess.CalledProcessError:
         print(f"* Error - Website for harmony upgrade is offline, setting to offline.")
         harmony_ver = "Offline"
     try:
         subprocess.check_output(
-            ["wget", "https://harmony.one/hmycli", "-O", easy_env.hmy_tmp_path], stderr=subprocess.STDOUT
+            ["wget", "https://harmony.one/hmycli", "-O", EnvironmentVariables.hmy_tmp_path], stderr=subprocess.STDOUT
         )
-        set_mod_x(easy_env.hmy_tmp_path)
-        hmy_ver = subprocess.getoutput(f"{easy_env.hmy_tmp_path} version")
+        set_mod_x(EnvironmentVariables.hmy_tmp_path)
+        hmy_ver = subprocess.getoutput(f"{EnvironmentVariables.hmy_tmp_path} version")
         hmy_ver = hmy_ver[62:-15]
     except subprocess.CalledProcessError:
         print(f"* Error - Website for hmy upgrade is offline, setting to offline.")
         hmy_ver = "Offline"
     return output_harmony_version.group(1)[:-2], hmy_ver
 
 
-
 def first_env_check(env_file, home_dir) -> None:
     if os.path.exists(env_file):
         load_var_file(env_file)
     else:
         os.system(f"touch {home_dir}/.easynode.env")
         load_var_file(env_file)
 
 
 def version_checks(harmony_folder):
     software_versions = {}
-    software_versions["harmony_version"], software_versions["hmy_version"] = get_local_version(
-        f"{harmony_folder}"
-    )
+    software_versions["harmony_version"], software_versions["hmy_version"] = get_local_version(f"{harmony_folder}")
     software_versions["online_harmony_version"], software_versions["online_hmy_version"] = check_online_version()
     # Check versions, if matching False (No Upgrade Required), non-match True (Upgrade Required)
-    if software_versions["harmony_version"] == software_versions["online_harmony_version"] or software_versions["online_harmony_version"] == "Offline":
+    if (
+        software_versions["harmony_version"] == software_versions["online_harmony_version"]
+        or software_versions["online_harmony_version"] == "Offline"
+    ):
         software_versions["harmony_upgrade"] = "False"
     else:
         software_versions["harmony_upgrade"] = "True"
-    if software_versions["hmy_version"] == software_versions["online_hmy_version"] or software_versions["online_hmy_version"] == "Offline":
+    if (
+        software_versions["hmy_version"] == software_versions["online_hmy_version"]
+        or software_versions["online_hmy_version"] == "Offline"
+    ):
         software_versions["hmy_upgrade"] = "False"
     else:
         software_versions["hmy_upgrade"] = "True"
     return software_versions
 
 
 def first_setup():
@@ -585,38 +731,35 @@
     get_shard_menu()
     # Express - no prompts for each step, Manual - prompts for each step
     get_express_status()
     # Get Regular validator with/without wallet or Full RPC Node
     get_node_type()
     # Get Mainnet or Testnet
     set_main_or_test()
-    # Set the API for previous choices
-    set_api_paths()
     # Setup status done
-    set_var(easy_env.dotenv_file, "SETUP_STATUS", "0")
+    set_var(EnvironmentVariables.dotenv_file, "SETUP_STATUS", "0")
     # Look for a harmony install or install.
     check_for_install()
     print_stars()
     return
 
 
 def recheck_vars():
     # recheck some stuff just in case the .easynode.env isn't proper
-    load_var_file(easy_env.dotenv_file)
+    load_var_file(EnvironmentVariables.dotenv_file)
     get_shard_menu()
     get_node_type()
     set_main_or_test()
-    set_api_paths()
     return
 
 
 # looks for ~/harmony or installs it if it's not there. Asks to overwrite if it finds it, run at your own risk.
 def check_for_install() -> str:
-    load_var_file(easy_env.dotenv_file)
-    if not os.path.exists(easy_env.harmony_dir):
+    load_var_file(EnvironmentVariables.dotenv_file)
+    if not os.path.exists(EnvironmentVariables.harmony_dir):
         print(f"* You selected Shard: {environ.get('SHARD')}. ")
         install_harmony()
         if environ.get("NODE_WALLET") == "true":
             restore_wallet()
         print_stars()
         print("* All harmony files now installed. Database download starting now...")
         print_stars()
@@ -654,42 +797,44 @@
         if mntCount > 1:
             print("* You have multiple mounts in /mnt - Review mounts, only 1 allowed for our installer at this time!")
             raise SystemExit(0)
         # Checks Passed at this point, only 1 folder in /mnt and it's probably our volume (can scope this down further later)
         if environ.get("SHARD") == "0":
             if mntCount == 1:
                 myLongHmyPath = myVolumePath + "/harmony"
-                dotenv.set_key(easy_env.dotenv_file, "MOUNT_POINT", myLongHmyPath)
+                dotenv.set_key(EnvironmentVariables.dotenv_file, "MOUNT_POINT", myLongHmyPath)
                 print("* Creating all Harmony Files & Folders")
-                os.system(f"sudo chown {easy_env.active_user} {myVolumePath}")
+                os.system(f"sudo chown {EnvironmentVariables.active_user} {myVolumePath}")
                 os.system(f"mkdir -p {myLongHmyPath}/.hmy/blskeys")
-                os.system(f"ln -s {myLongHmyPath} {easy_env.harmony_dir}")
+                os.system(f"ln -s {myLongHmyPath} {EnvironmentVariables.harmony_dir}")
             # Let's make sure your volume is mounted
             if mntCount == 0:
                 question = ask_yes_no(
                     "* You have a volume but it is not mounted.\n* Would you like to install Harmony in ~/harmony on your main disk instead of your volume? (Yes/No) "
                 )
                 if question:
-                    dotenv.set_key(easy_env.dotenv_file, "MOUNT_POINT", easy_env.harmony_dir)
+                    dotenv.set_key(EnvironmentVariables.dotenv_file, "MOUNT_POINT", EnvironmentVariables.harmony_dir)
                 else:
                     raise SystemExit(0)
     # Setup folders now that symlink exists or we know we're using ~/harmony
-    if not os.path.isdir(f"{easy_env.user_home_dir}/.hmy_cli/account-keys/"):
-        os.system(f"mkdir -p {easy_env.user_home_dir}/.hmy_cli/account-keys/")
-    if not os.path.isdir(f"{easy_env.harmony_dir}/.hmy/blskeys"):
+    if not os.path.isdir(f"{EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/"):
+        os.system(f"mkdir -p {EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/")
+    if not os.path.isdir(f"{EnvironmentVariables.harmony_dir}/.hmy/blskeys"):
         print("* Creating all Harmony Files & Folders")
-        os.system(f"mkdir -p {easy_env.harmony_dir}/.hmy/blskeys")
+        os.system(f"mkdir -p {EnvironmentVariables.harmony_dir}/.hmy/blskeys")
     # Change to ~/harmony folder
-    os.chdir(f"{easy_env.harmony_dir}")
+    os.chdir(f"{EnvironmentVariables.harmony_dir}")
     print_stars()
     # Install hmy
     install_hmy()
     print_stars()
     # Install harmony
-    pull_harmony_update(easy_env.harmony_dir, easy_env.bls_key_file, easy_env.harmony_conf)
+    pull_harmony_update(
+        EnvironmentVariables.harmony_dir, EnvironmentVariables.bls_key_file, EnvironmentVariables.harmony_conf
+    )
     # install hmy files
     print("* Installing rclone application & rclone configuration files")
     print_stars()
     # check for working rclone site and download
     try:
         os.system("curl https://rclone.org/install.sh | sudo bash")
     except (ValueError, KeyError, TypeError):
@@ -697,57 +842,57 @@
             "* rclone site is offline, we can install rclone from the Ubuntu repo as a workaround, do you want to continue? (Y/N): "
         )
         if result:
             # If rclone curl is down, install rclone with apt instead
             subprocess.run("sudo apt install rclone -y")
 
     os.system(
-        f"mkdir -p {easy_env.user_home_dir}/.config/rclone && cp {easy_env.toolbox_location}/src/bin/rclone.conf {easy_env.user_home_dir}/.config/rclone/"
+        f"mkdir -p {EnvironmentVariables.user_home_dir}/.config/rclone && cp {EnvironmentVariables.toolbox_location}/src/bin/rclone.conf {EnvironmentVariables.user_home_dir}/.config/rclone/"
     )
     print_stars()
     # Setup the harmony service file
     print("* Customizing, Moving & Enabling your harmony.service systemd file")
-    if easy_env.active_user == "root":
+    if EnvironmentVariables.active_user == "root":
         os.system(
-            f"sudo cp {easy_env.toolbox_location}/src/bin/harmony.service . && sed -i 's/home\/serviceharmony/{easy_env.active_user}/g' 'harmony.service' && sed -i 's/serviceharmony/{easy_env.active_user}/g' 'harmony.service' && sudo mv harmony.service /etc/systemd/system/harmony.service && sudo chmod a-x /etc/systemd/system/harmony.service && sudo systemctl enable harmony.service"
+            f"sudo cp {EnvironmentVariables.toolbox_location}/src/bin/harmony.service . && sed -i 's/home\/serviceharmony/{EnvironmentVariables.active_user}/g' 'harmony.service' && sed -i 's/serviceharmony/{EnvironmentVariables.active_user}/g' 'harmony.service' && sudo mv harmony.service /etc/systemd/system/harmony.service && sudo chmod a-x /etc/systemd/system/harmony.service && sudo systemctl enable harmony.service"
         )
     else:
         os.system(
-            f"sudo cp {easy_env.toolbox_location}/src/bin/harmony.service . && sed -i 's/serviceharmony/{easy_env.active_user}/g' 'harmony.service' && sudo mv harmony.service /etc/systemd/system/harmony.service && sudo chmod a-x /etc/systemd/system/harmony.service && sudo systemctl enable harmony.service"
+            f"sudo cp {EnvironmentVariables.toolbox_location}/src/bin/harmony.service . && sed -i 's/serviceharmony/{EnvironmentVariables.active_user}/g' 'harmony.service' && sudo mv harmony.service /etc/systemd/system/harmony.service && sudo chmod a-x /etc/systemd/system/harmony.service && sudo systemctl enable harmony.service"
         )
 
 
 # Database Downloader
 def clone_shards():
     # Move to ~/harmony
-    os.chdir(f"{easy_env.harmony_dir}")
+    os.chdir(f"{EnvironmentVariables.harmony_dir}")
 
     if environ.get("SHARD") != "0":
         # If we're not on shard 0, download the numbered shard DB here.
         print(f"* Now cloning shard {environ.get('SHARD')}")
         print_stars()
         os.system(
-            f"rclone -P sync release:pub.harmony.one/{environ.get('NETWORK')}.min/harmony_db_{environ.get('SHARD')} {easy_env.harmony_dir}/harmony_db_{environ.get('SHARD')} --multi-thread-streams 4 --transfers=32"
+            f"rclone -P sync release:pub.harmony.one/{environ.get('NETWORK')}.min/harmony_db_{environ.get('SHARD')} {EnvironmentVariables.harmony_dir}/harmony_db_{environ.get('SHARD')} --multi-thread-streams 4 --transfers=32"
         )
         print_stars()
         print(f"Shard {environ.get('SHARD')} completed.")
         print_stars()
     else:
         # If we're on shard 0, grab the snap DB here.
         print("* Now cloning Shard 0, kick back and relax for awhile...")
         print_stars()
         os.system(
-            f"rclone -P -L --checksum sync release:pub.harmony.one/{environ.get('NETWORK')}.snap/harmony_db_0 {easy_env.harmony_dir}/harmony_db_0 --multi-thread-streams 4 --transfers=32"
+            f"rclone -P -L --checksum sync release:pub.harmony.one/{environ.get('NETWORK')}.snap/harmony_db_0 {EnvironmentVariables.harmony_dir}/harmony_db_0 --multi-thread-streams 4 --transfers=32"
         )
 
 
 # Code to restore a wallet
 def restore_wallet() -> str:
     if environ.get("NODE_WALLET") == "true":
-        if not os.path.exists(easy_env.hmy_wallet_store):
+        if not os.path.exists(EnvironmentVariables.hmy_wallet_store):
             subprocess.run("clear")
             print_stars()
             print("* Harmony ONE Validator Wallet Import")
             print_stars()
             if environ.get("EXPRESS") == "1":
                 question = ask_yes_no(
                     "\n* You will directly utilize the harmony application interface"
@@ -772,23 +917,23 @@
     # First let's make sure your volume is mounted
     totalDir = len(os.listdir("/mnt"))
     if totalDir > 0:
         volumeMountPath = os.listdir("/mnt")
         myVolumePath = "/mnt/" + str(volumeMountPath[0])
         myLongHmyPath = myVolumePath + "/harmony"
     else:
-        myVolumePath = easy_env.harmony_dir
+        myVolumePath = EnvironmentVariables.harmony_dir
     if totalDir == 1:
-        dotenv.set_key(easy_env.dotenv_file, "MOUNT_POINT", myLongHmyPath)
+        dotenv.set_key(EnvironmentVariables.dotenv_file, "MOUNT_POINT", myLongHmyPath)
     else:
-        dotenv.set_key(easy_env.dotenv_file, "MOUNT_POINT", f"{easy_env.harmony_dir}")
+        dotenv.set_key(EnvironmentVariables.dotenv_file, "MOUNT_POINT", f"{EnvironmentVariables.harmony_dir}")
 
 
 def finish_node_install():
-    load_var_file(easy_env.dotenv_file)
+    load_var_file(EnvironmentVariables.dotenv_file)
     print_stars()
     print(
         "* Installation is completed"
         + "\n* Create a new wallet or recover your existing wallet into ./hmy"
         + "\n* Create or upload your bls key & pass files into ~/harmony/.hmy/blskeys"
         + "\n* Finally, reboot to start synchronization."
     )
@@ -812,15 +957,15 @@
             + "\n* To create BLS keys run:"
             + f'\n* ./hmy keys generate-bls-keys --count 1 --shard {environ.get("SHARD")} {environ.get("PASS_SWITCH")}'
             + "\n*"
         )
     print_stars()
     print("* Thanks for using Easy Node - Validator Node Server Software Installer!")
     print_stars()
-    set_var(easy_env.dotenv_file, "SETUP_STATUS", "1")
+    set_var(EnvironmentVariables.dotenv_file, "SETUP_STATUS", "1")
     raise SystemExit(0)
 
 
 def free_space_check(mount) -> str:
     ourDiskMount = get_mount_point(mount)
     _, _, free = shutil.disk_usage(ourDiskMount)
     freeConverted = str(converted_unit(free))
@@ -1071,15 +1216,19 @@
         os.system("sudo reboot")
     else:
         print("Invalid option.")
 
 
 def finish_node():
     print(
-        "* Thanks for using Easy Node - EZ Mode!\n* We serve up free tools.\n* Please consider supporting us one time or monthly at https://github.com/sponsors/easy-node-pro today!\n*\n* Goodbye!"
+        "* Thanks for using Easy Node Toolbox - Making everything Easy Mode!"
+        + "\n*\n* We serve up free tools and guides for validators every day."
+        + "\n*\n* Check our guides out at https://docs.easynode.pro\n*\n"
+        + "* Please consider joining our discord & supporting us one time or monthly\n* for our"
+        + " tools and guides at https://bit.ly/easynodediscord today!\n*\n* Goodbye!"
     )
     print_stars()
     raise SystemExit(0)
 
 
 def compare_two_files(input1, input2) -> None:
     # open the files
```

### Comparing `harmony_toolbox-1.0.5/src/toolbox/toolbox.py` & `harmony_toolbox-1.0.8/src/toolbox/toolbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os, requests, time, json, subprocess
 from pytimedinput import timedInteger
 from subprocess import Popen, PIPE, run
 from ast import literal_eval
-from toolbox.config import easy_env
+from toolbox.config import EnvironmentVariables
 from os import environ
 from datetime import datetime
 from colorama import Fore, Back, Style
 from pyhmy import blockchain, transaction
 from requests.exceptions import HTTPError
 from toolbox.library import (
     process_command,
@@ -28,216 +28,328 @@
     all_sys_info,
     coming_soon,
     menu_ubuntu_updates,
     menu_error,
     menu_reboot_server,
     finish_node,
     pull_harmony_update,
-    version_checks
+    version_checks,
+    harmony_service_status,
+    loader_intro,
+    get_folders,
+    validator_stats_output,
+    get_db_size
 )
 
+
+def parse_flags(parser):
+    # Add the arguments
+    parser.add_argument(
+        "-s",
+        "--stats",
+        action="store_true",
+        help="Run your stats if Harmony is installed and running.",
+    )
+    
+    parser.add_argument(
+        "-c",
+        "--collect",
+        action="store_true",
+        help="Collect your rewards to your validator wallet",
+    )
+    
+    parser.add_argument(
+        "-cs",
+        "--collect-send",
+        action="store_true",
+        help="Collect your rewards to your validator wallet and send them to your rewards wallet",
+    )
+
+    args = parser.parse_args()
+
+    subprocess.run("clear")
+    print(Fore.RESET)
+
+    if args.stats:
+        run_multistats()
+        finish_node()
+        
+    if args.collect:
+        rewards_collector(EnvironmentVariables.hmy_app, True)
+        finish_node()
+        
+    if args.collect_send:
+        rewards_collector(EnvironmentVariables.hmy_app, True, True)
+        finish_node()
+
+
+def run_multistats():
+    loader_intro()
+    refresh_stats(1)
+    folders = get_folders()
+    validator_stats_output(folders)
+    return
+
+
 def collect_rewards(networkCall):
     os.system(
         f"{networkCall} staking collect-rewards --delegator-addr {environ.get('VALIDATOR_WALLET')} --gas-price 100 {environ.get('PASS_SWITCH')}"
     )
 
+
 def send_rewards(networkCall, sendAmount, rewards_wallet):
     os.system(
         f"{networkCall} transfer --amount {sendAmount} --from {environ.get('VALIDATOR_WALLET')} --from-shard 0 --to {rewards_wallet} --to-shard 0 --gas-price 100 {environ.get('PASS_SWITCH')}"
     )
 
-def rewards_collector(rewards_wallet, validator_wallet, rpc) -> None:
+
+def rewards_collector(rpc, bypass = False, send_out_rewards = False, rewards_wallet = environ.get('REWARDS_WALLET'), validator_wallet = environ.get('VALIDATOR_WALLET')) -> None:
     print("* Harmony ONE Rewards Collection")
     print_stars()
-    question = ask_yes_no(
-        f"*\n* For your validator wallet {validator_wallet}\n* You have {get_rewards_balance(rpc, validator_wallet)} $ONE pending.\n* Would you like to collect your rewards on the Harmony mainnet? (YES/NO) "
-    )
-    if question:
-        collect_rewards(environ.get('NETWORK_0_CALL'))
+    if bypass == False:
+        question = ask_yes_no(
+            f"*\n* For your validator wallet {validator_wallet}\n* You have {get_rewards_balance(rpc, validator_wallet)} $ONE pending.\n* Would you like to collect your rewards on the Harmony mainnet? (YES/NO) "
+        )
+        bypass = True
+    if bypass:
+        collect_rewards(EnvironmentVariables.hmy_app)
         print_stars()
         print(
-            Fore.GREEN
-            + f"* mainnet rewards for {validator_wallet} have been collected."
-            + Style.RESET_ALL
-+ Fore.GREEN
+            Fore.GREEN + f"* mainnet rewards for {validator_wallet} have been collected." + Style.RESET_ALL + Fore.GREEN
         )
         print_stars()
     else:
         return
-    wallet_balance, wallet_balance_test = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
+    wallet_balance = get_wallet_balance(validator_wallet)
     suggested_send = wallet_balance - int(environ.get("GAS_RESERVE"))
-    print("*\n*\n")
-    print_stars()
-    print("\n* Send your Harmony ONE Rewards?")
-    print_stars()
     if suggested_send >= 1:
-        question = ask_yes_no(
-            f"* You have {wallet_balance} $ONE available to send. We suggest sending {suggested_send} $ONE using your reservation settings.\n* Would you like to send {suggested_send} $ONE to {rewards_wallet} now? (YES/NO)"
-        )
-        if question:
-            send_rewards(environ.get("NETWORK_0_CALL"), suggested_send, rewards_wallet)
+        if send_rewards == False:
+            print("*\n*\n")
+            print_stars()
+            print("\n* Send your Harmony ONE Rewards?")
+            print_stars()
+            question = ask_yes_no(
+                f"* You have {wallet_balance} $ONE available to send. We suggest sending {suggested_send} $ONE using your reservation settings.\n* Would you like to send {suggested_send} $ONE to {rewards_wallet} now? (YES/NO)"
+            )
+            if question:
+                send_out_rewards = True
+        if send_out_rewards:
+            print("*\n*\n")
+            print_stars()
+            print("\n* Sending your Harmony ONE Rewards, awaiting confirmation...")
+            print_stars()
+            send_rewards(EnvironmentVariables.hmy_app, suggested_send, rewards_wallet)
+        wallet_balance = get_wallet_balance(validator_wallet)
+        print(f"*\n*\n* Current Wallet Balance: {wallet_balance} $ONE\n*\n*")
+        return
+    else:
+        wallet_balance = get_wallet_balance(validator_wallet)
+        print(f"*\n*\n* Current Wallet Balance: {wallet_balance} $ONE\n*\n*")
         return
 
+
 def menu_topper_regular(software_versions) -> None:
     # Get stats & balances
     try:
         load_1, load_5, load_15 = os.getloadavg()
         sign_percentage = get_sign_pct()
-        total_balance, total_balance_test = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
+        total_balance = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
         remote_data_shard_0, local_data_shard, remote_data_shard = menu_validator_stats()
     except (ValueError, KeyError, TypeError) as e:
-        print(f'* Error fetching data: {e}')
+        print(f"* Error fetching data: {e}")
     subprocess.run("clear")
     # Print Menu
     print_stars()
-    print(f'{Fore.GREEN}* Validator Toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*')
+    print(
+        f'{Fore.GREEN}* Validator Toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*'
+    )
     print_stars()
-    print(f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(easy_env.rpc_endpoints, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {Fore.BLUE}{easy_env.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{easy_env.external_ip}{Fore.GREEN}')
+    print(
+        f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(EnvironmentVariables.rpc_endpoints, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {Fore.BLUE}{EnvironmentVariables.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
+    )
     harmony_service_status()
-    print(f'* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current disk space free: {Fore.CYAN}{free_space_check(easy_env.harmony_dir): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}')
+    print(
+        f'* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current disk space free: {Fore.CYAN}{free_space_check(EnvironmentVariables.harmony_dir): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
+    )
     print_stars()
     if environ.get("SHARD") != "0":
-        print(f"* Note: Running on shard {environ.get('SHARD')}, Shard 0 is no longer needed locally and should be under 200MB\n* Remote Shard 0 Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}, Local Shard 0 Size: {get_db_size(easy_env.harmony_dir, '0')}")
-        print(f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard['result']['shard-chain-header']['number'])}")
-        print(f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}, Local Shard {environ.get('SHARD')} Size: {get_db_size(easy_env.harmony_dir, environ.get('SHARD'))}")
+        print(
+            f"* Note: Running on shard {environ.get('SHARD')}, Shard 0 is no longer needed locally and should be under 300MB\n* Remote Shard 0 Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}, Local Shard 0 Size: {get_db_size(EnvironmentVariables.harmony_dir, '0')}"
+        )
+        print(
+            f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard['result']['shard-chain-header']['number'])}"
+        )
+        print(
+            f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}, Local Shard {environ.get('SHARD')} Size: {get_db_size(EnvironmentVariables.harmony_dir, environ.get('SHARD'))}"
+        )
     if environ.get("SHARD") == "0":
-        print(f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}")
-        print(f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}")
-    print(f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min")
+        print(
+            f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}"
+        )
+        print(
+            f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}"
+        )
+    print(
+        f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min"
+    )
     print_stars()
 
+
 def menu_topper_full() -> None:
     try:
         load_1, load_5, load_15 = os.getloadavg()
         remote_data_shard_0, local_data_shard, remote_data_shard = menu_validator_stats()
     except (ValueError, KeyError, TypeError) as e:
-        print(f'* Error fetching data: {e}')
+        print(f"* Error fetching data: {e}")
     subprocess.run("clear")
     # Print Menu
     print_stars()
-    print(f'{Fore.GREEN}* Validator Toolbox for Harmony ONE Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*')
+    print(
+        f'{Fore.GREEN}* Validator Toolbox for Harmony ONE Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*'
+    )
     print_stars()
-    print(f'* Server Hostname & IP:             {Fore.BLUE}{easy_env.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{easy_env.external_ip}{Fore.GREEN}')
+    print(
+        f"* Server Hostname & IP:             {Fore.BLUE}{EnvironmentVariables.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}"
+    )
     harmony_service_status()
-    print(f'* Current disk space free: {Fore.CYAN}{free_space_check(easy_env.harmony_dir): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{environ.get("HARMONY_VERSION")}{Fore.GREEN}, has upgrade available: {environ.get("HARMONY_UPGRADE_AVAILABLE")}\n* Current hmy version: {Fore.YELLOW}{environ.get("HMY_VERSION")}{Fore.GREEN}, has upgrade available: {environ.get("HMY_UPGRADE_AVAILABLE")}')
-    print(f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}")
-    print(f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}")
-    print(f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min")
+    print(
+        f'* Current disk space free: {Fore.CYAN}{free_space_check(EnvironmentVariables.harmony_dir): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{environ.get("HARMONY_VERSION")}{Fore.GREEN}, has upgrade available: {environ.get("HARMONY_UPGRADE_AVAILABLE")}\n* Current hmy version: {Fore.YELLOW}{environ.get("HMY_VERSION")}{Fore.GREEN}, has upgrade available: {environ.get("HMY_UPGRADE_AVAILABLE")}'
+    )
+    print(
+        f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}"
+    )
+    print(
+        f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}"
+    )
+    print(
+        f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min"
+    )
     print_stars()
 
+
 def menu_regular(software_versions) -> None:
     menu_topper_regular(software_versions)
-    for x in return_txt(easy_env.main_menu_regular):
+    for x in return_txt(EnvironmentVariables.main_menu_regular):
         x = x.strip()
         try:
             x = eval(x)
         except SyntaxError:
             pass
         if x:
             print(x)
 
+
 def menu_full() -> None:
     menu_topper_full()
-    for x in return_txt(easy_env.main_menu_full):
+    for x in return_txt(EnvironmentVariables.main_menu_full):
         x = x.strip()
         try:
             x = eval(x)
         except SyntaxError:
             pass
         if x:
             print(x)
 
+
 def get_wallet_json(wallet: str) -> str:
     test_or_main = environ.get("NETWORK")
     try:
         response = requests.get(f"https://api.stake.hmny.io/networks/{test_or_main}/validators/{wallet}")
         response.raise_for_status()
         # access JSOn content
         json_response = response.json()
     #        print("Entire JSON response")
     #        print(json_response)
     except HTTPError as http_err:
         print(f"HTTP error occurred: {http_err}")
         print(
-            f'* You have not created your validator yet, try again after you add one!\n* cd ~/harmony\n* ./hmy keys recover-from-mnemonic {easy_env.active_user} {environ.get("PASS_SWITCH")}'
+            f'* You have not created your validator yet, try again after you add one!\n* cd ~/harmony\n* ./hmy keys recover-from-mnemonic {EnvironmentVariables.active_user} {environ.get("PASS_SWITCH")}'
         )
         input("Press ENTER to return to the main menu.")
         return
     except Exception as err:
         print(f"Other error occurred: {err}")
         input("Press ENTER to return to the main menu.")
         return
     return json_response
 
+
 def tmi_server_info() -> None:
     validator_wallet = environ.get("VALIDATOR_WALLET")
     json_response = get_wallet_json(validator_wallet)
     for key, value in json_response.items():
         print(key, ":", value)
     print_stars()
     input("Press ENTER to return to the main menu.")
 
+
 def set_rewards_wallet() -> None:
     rewards_wallet = environ.get("REWARDS_WALLET")
     gas_reserve = environ.get("GAS_RESERVE")
     if rewards_wallet is None:
         question = ask_yes_no("* Would you like to add an address to send your rewards too? (YES/NO)")
         if question:
             rewards_wallet = input(f"* Input your one1 address to send rewards into, please input your address now: ")
             if rewards_wallet.startswith("one1"):
-                set_var(easy_env.dotenv_file, "REWARDS_WALLET", rewards_wallet)
+                set_var(EnvironmentVariables.dotenv_file, "REWARDS_WALLET", rewards_wallet)
             else:
                 print("* Wallet does not start with one1, please try again.")
                 return
         return
     else:
         question = ask_yes_no(
             f"* Your current saved rewards wallet address is {rewards_wallet}\n* Would you like to update the address you send your rewards too? (YES/NO)"
         )
         if question:
             rewards_wallet = input(f"* Input your one1 address to send rewards into, please input your address now: ")
             if rewards_wallet.startswith("one1"):
-                set_var(easy_env.dotenv_file, "REWARDS_WALLET", rewards_wallet)
+                set_var(EnvironmentVariables.dotenv_file, "REWARDS_WALLET", rewards_wallet)
             else:
                 print("* Wallet does not start with one1, please try again.")
                 return
             set_gas_reserve()
             return
         else:
             question = ask_yes_no(
                 f"* Your current wallet gas reservation is {gas_reserve} $ONE\n* Would you like to update your reservation total? (YES/NO)"
             )
             if question:
                 set_gas_reserve()
                 return
     return
 
+
 def set_gas_reserve() -> None:
     gas_reserve = environ.get("GAS_RESERVE")
     question = ask_yes_no(
         f"* Your current total of $ONE to reserve for fees is {gas_reserve}\n* Would you like to update the reserve total? (YES/NO)"
     )
     if question:
         ask_reserve_total()
     return
 
+
 def ask_reserve_total() -> None:
     reserve_total = input("* How much $ONE would you like to keep reserved for fees? ")
     set_reserve_total(reserve_total)
     return
 
+
 def set_reserve_total(reserve_total):
-    set_var(easy_env.dotenv_file, "GAS_RESERVE", reserve_total)
+    set_var(EnvironmentVariables.dotenv_file, "GAS_RESERVE", reserve_total)
+
 
 def drive_check() -> None:
-    server_drive_check(easy_env.dotenv_file, easy_env.harmony_dir)
+    server_drive_check(EnvironmentVariables.dotenv_file, EnvironmentVariables.harmony_dir)
     return
 
+
 def run_check_balance() -> None:
-    menu_check_balance(easy_env.rpc_endpoints, environ.get("VALIDATOR_WALLET"))
+    menu_check_balance(EnvironmentVariables.rpc_endpoints, environ.get("VALIDATOR_WALLET"))
+
 
 def run_full_node() -> None:
     menu_options = {
         # 0: finish_node,
         1: refresh_stats,
         2: coming_soon,
         3: coming_soon,
@@ -252,15 +364,15 @@
         12: menu_ubuntu_updates,
         13: drive_check,
         14: coming_soon,
         15: all_sys_info,
         999: menu_reboot_server,
     }
     while True:
-        load_var_file(easy_env.dotenv_file)
+        load_var_file(EnvironmentVariables.dotenv_file)
         menu_full()
         if environ.get("HARMONY_UPGRADE_AVAILABLE") == "True":
             print(
                 f"* The harmony binary has an update available, Option #10 will upgrade you but you may miss a block while it restarts.\n"
             )
             print_stars()
         if environ.get("HMY_UPGRADE_AVAILABLE") == "True":
@@ -274,77 +386,107 @@
             menu_error()
             run_full_node(environ.get("NODE_TYPE"))
         if option == 0:
             return finish_node()
         subprocess.run("clear")
         menu_options[option]()
 
+
 def bingo_checker():
-    os.system(f"grep BINGO {easy_env.harmony_dir}/latest/zerolog-harmony.log | tail -10")
+    os.system(f"grep BINGO {EnvironmentVariables.harmony_dir}/latest/zerolog-harmony.log | tail -10")
     print_stars()
     print("* Press enter to return to the main menu.")
     print_stars()
     input()
 
+
 def run_rewards_collector() -> None:
-    rewards_collector(environ.get("REWARDS_WALLET"), environ.get('VALIDATOR_WALLET'), easy_env.rpc_endpoints)
+    rewards_collector(
+        EnvironmentVariables.hmy_app
+    )
     return
 
+
 def safety_defaults() -> None:
-    if environ.get("GAS_RESERVE") is None: set_var(easy_env.dotenv_file, "GAS_RESERVE", "5")
-    if environ.get("REFRESH_TIME") is None: set_var(easy_env.dotenv_file, "REFRESH_TIME", "30")
-    if environ.get("REFRESH_OPTION") is None: set_var(easy_env.dotenv_file, "REFRESH_OPTION", "True")
-    if environ.get("HARMONY_FOLDER") is None: 
-        if os.path.isdir(f'{easy_env.user_home_dir}/harmony'):
-            set_var(easy_env.dotenv_file, "HARMONY_FOLDER", f'{easy_env.user_home_dir}/harmony')
-        elif os.path.exists(f'{easy_env.user_home_dir}/harmony'):
+    if environ.get("GAS_RESERVE") is None:
+        set_var(EnvironmentVariables.dotenv_file, "GAS_RESERVE", "5")
+    if environ.get("REFRESH_TIME") is None:
+        set_var(EnvironmentVariables.dotenv_file, "REFRESH_TIME", "30")
+    if environ.get("REFRESH_OPTION") is None:
+        set_var(EnvironmentVariables.dotenv_file, "REFRESH_OPTION", "True")
+    if environ.get("HARMONY_FOLDER") is None:
+        if os.path.isdir(f"{EnvironmentVariables.user_home_dir}/harmony"):
+            set_var(EnvironmentVariables.dotenv_file, "HARMONY_FOLDER", f"{EnvironmentVariables.user_home_dir}/harmony")
+        elif os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony"):
             try:
-                subprocess.run(f'{easy_env.user_home_dir}/harmony --version', check=True)
-                set_var(set_var(easy_env.dotenv_file, "HARMONY_FOLDER", f'{easy_env.user_home_dir}'))
+                subprocess.run(f"{EnvironmentVariables.user_home_dir}/harmony --version", check=True)
+                set_var(
+                    set_var(EnvironmentVariables.dotenv_file, "HARMONY_FOLDER", f"{EnvironmentVariables.user_home_dir}")
+                )
             except subprocess.CalledProcessError as e:
-                print('* Harmony not found, contact Easy Node for custom configs.')
+                print("* Harmony not found, contact Easy Node for custom configs.")
                 raise SystemExit(0)
         else:
-            print('* Harmony not found, contact Easy Node for custom configs.')
+            print("* Harmony not found, contact Easy Node for custom configs.")
             raise SystemExit(0)
-    set_var(easy_env.dotenv_file, "EASY_VERSION", easy_env.easy_version)
+    set_var(EnvironmentVariables.dotenv_file, "EASY_VERSION", EnvironmentVariables.easy_version)
+
 
 def refresh_toggle() -> None:
     if environ.get("REFRESH_OPTION") == "True":
-        answer = ask_yes_no(f'* Refresh is currently enabled. Would you like to disable it? (Y/N) ')
+        answer = ask_yes_no(f"* Refresh is currently enabled. Would you like to disable it? (Y/N) ")
         if answer:
-            set_var(easy_env.dotenv_file, "REFRESH_OPTION", "False")
+            set_var(EnvironmentVariables.dotenv_file, "REFRESH_OPTION", "False")
         else:
-            answer = ask_yes_no(f'* Your current refresh time is {str(environ.get("REFRESH_TIME"))} seconds. Would you like to change the delay? (Y/N) ')
+            answer = ask_yes_no(
+                f'* Your current refresh time is {str(environ.get("REFRESH_TIME"))} seconds. Would you like to change the delay? (Y/N) '
+            )
             if answer:
-                delay_time = timedInteger("* Enter the number of seconds to wait before auto-refreshing: ", timeout=-1, resetOnInput=True, allowNegative=False)
-                set_var(easy_env.dotenv_file, "REFRESH_TIME", str(delay_time[0]))
+                delay_time = timedInteger(
+                    "* Enter the number of seconds to wait before auto-refreshing: ",
+                    timeout=-1,
+                    resetOnInput=True,
+                    allowNegative=False,
+                )
+                set_var(EnvironmentVariables.dotenv_file, "REFRESH_TIME", str(delay_time[0]))
     else:
-        answer = ask_yes_no(f'* Refresh is currently disabled. Would you like to enable it? (Y/N) ')
+        answer = ask_yes_no(f"* Refresh is currently disabled. Would you like to enable it? (Y/N) ")
         if answer:
-            set_var(easy_env.dotenv_file, "REFRESH_OPTION", "True")
-        answer = ask_yes_no(f'* Your current refresh time is {str(environ.get("REFRESH_TIME"))} seconds. Would you like to change the delay? (Y/N) ')
+            set_var(EnvironmentVariables.dotenv_file, "REFRESH_OPTION", "True")
+        answer = ask_yes_no(
+            f'* Your current refresh time is {str(environ.get("REFRESH_TIME"))} seconds. Would you like to change the delay? (Y/N) '
+        )
         if answer:
-            delay_time = timedInteger("* Enter the number of seconds to wait before auto-refreshing: ", timeout=-1, resetOnInput=True, allowNegative=False)
-            set_var(easy_env.dotenv_file, "REFRESH_TIME", str(delay_time[0]))
-    load_var_file(easy_env.dotenv_file)
+            delay_time = timedInteger(
+                "* Enter the number of seconds to wait before auto-refreshing: ",
+                timeout=-1,
+                resetOnInput=True,
+                allowNegative=False,
+            )
+            set_var(EnvironmentVariables.dotenv_file, "REFRESH_TIME", str(delay_time[0]))
+    load_var_file(EnvironmentVariables.dotenv_file)
     return
 
+
 def refresh_status_option():
     if environ.get("REFRESH_OPTION") == "True":
-        print(f"*  20 - Disable auto-refresh      - Disable Refresh or Change Delay Timer: {str(environ.get('REFRESH_TIME'))} seconds")
+        print(
+            f"*  20 - Disable auto-refresh      - Disable Refresh or Change Delay Timer: {str(environ.get('REFRESH_TIME'))} seconds"
+        )
     else:
         print(f"*  20 - Enable Auto refresh       - Enable Refresh Timeout")
 
+
 def start_regular_node() -> None:
     # Check online versions of harmony & hmy and compare to our local copy.
     refresh_stats(1)
     software_versions = version_checks(environ.get("HARMONY_FOLDER"))
     run_regular_node(software_versions)
 
+
 def run_regular_node(software_versions) -> None:
     menu_options = {
         0: finish_node,
         1: refresh_stats,
         2: menu_active_bls,
         3: coming_soon,
         4: run_rewards_collector,
@@ -359,219 +501,235 @@
         13: drive_check,
         14: tmi_server_info,
         15: all_sys_info,
         20: refresh_toggle,
         999: menu_reboot_server,
     }
     while True:
-        load_var_file(easy_env.dotenv_file)
+        load_var_file(EnvironmentVariables.dotenv_file)
         menu_regular(software_versions)
         if software_versions["harmony_upgrade"] == "True":
             print(
                 f'* The harmony binary has an update available to version {software_versions["online_harmony_version"]}\n* Option #10 will upgrade you, but you may miss a block while it upgrades & restarts.\n* Currently installed version {software_versions["harmony_version"]}'
             )
             print_stars()
         if software_versions["hmy_upgrade"] == "True":
             print(
                 f'* The hmy binary has an update available to version {software_versions["online_hmy_version"]}\n* Option #11 will upgrade you.\n* Currently installed version {software_versions["hmy_version"]}'
             )
             print_stars()
         if environ.get("REFRESH_OPTION") == "True":
             try:
                 # run timed input
-                option, timedOut = timedInteger(f"* Auto refresh enabled, Enter your menu choice: ", timeout=int(environ.get("REFRESH_TIME")), resetOnInput=True, allowNegative=False)
+                option, timedOut = timedInteger(
+                    f"* Auto refresh enabled, Enter your menu choice: ",
+                    timeout=int(environ.get("REFRESH_TIME")),
+                    resetOnInput=True,
+                    allowNegative=False,
+                )
                 if timedOut:
                     start_regular_node()
                 else:
                     subprocess.run("clear")
                     print_stars()
                     menu_options[option]()
                     if option != 1:
                         start_regular_node()
             except KeyError:
-                print(f'* Bad option, try again. Press enter to continue.')
+                print(f"* Bad option, try again. Press enter to continue.")
                 print_stars()
                 input()
                 start_regular_node()
         else:
             try:
-                option, timedOut = timedInteger("* Auto refresh disabled, Enter your menu choice: ", timeout=-1, resetOnInput=True, allowNegative=False)
+                option, timedOut = timedInteger(
+                    "* Auto refresh disabled, Enter your menu choice: ",
+                    timeout=-1,
+                    resetOnInput=True,
+                    allowNegative=False,
+                )
                 subprocess.run("clear")
                 print_stars()
                 menu_options[option]()
                 if option != 1:
                     start_regular_node()
             except KeyError:
                 print(f"* Bad option, try again. Press enter to continue.")
                 print_stars()
                 input()
                 start_regular_node()
 
-def harmony_service_status() -> None:
-    status = subprocess.call(["systemctl", "is-active", "--quiet", "harmony"])
-    if status == 0:
-        print("* Harmony Service is:               " + Fore.BLACK + Back.GREEN + "   Online  " + Style.RESET_ALL + Fore.GREEN)
-    else:
-        print("* Harmony Service is:               " + Fore.WHITE + Back.RED + "  *** Offline *** " + Style.RESET_ALL + Fore.GREEN)
 
 def service_menu_option() -> None:
     status = os.system("systemctl is-active --quiet harmony")
     if status == 0:
-        print(f'*   8 - {Fore.RED}Stop Harmony Service      {Fore.GREEN}- {Fore.YELLOW}{Back.RED}WARNING: You will miss blocks while stopped!   {Style.RESET_ALL}{Fore.GREEN}')
-        print(f'*   9 - Restart Harmony Service   - {Back.RED}{Fore.YELLOW}WARNING: You will miss blocks during a restart!{Style.RESET_ALL}{Fore.GREEN}')
+        print(
+            f"*   8 - {Fore.RED}Stop Harmony Service      {Fore.GREEN}- {Fore.YELLOW}{Back.RED}WARNING: You will miss blocks while stopped!   {Style.RESET_ALL}{Fore.GREEN}"
+        )
+        print(
+            f"*   9 - Restart Harmony Service   - {Back.RED}{Fore.YELLOW}WARNING: You will miss blocks during a restart!{Style.RESET_ALL}{Fore.GREEN}"
+        )
     else:
-        print(f'*   8 - Start Harmony Service')
+        print(f"*   8 - Start Harmony Service")
+
 
 def make_backup_dir() -> str:
-    folder_name = f'{easy_env.harmony_dir}/harmony_backup/{datetime.now().strftime("%Y%m%d%H%M")}'
+    folder_name = f'{EnvironmentVariables.harmony_dir}/harmony_backup/{datetime.now().strftime("%Y%m%d%H%M")}'
     os.system(f"mkdir -p {folder_name}")
     return folder_name
 
+
 def hmy_cli_upgrade():
     question = ask_yes_no(
         "* Are you sure you would like to proceed with updating the Harmony CLI file?\n\nType 'Yes' or 'No' to continue"
     )
     if question:
         folder_name = make_backup_dir()
-        os.system(f"cp {easy_env.hmy_app} {folder_name}")
+        os.system(f"cp {EnvironmentVariables.hmy_app} {folder_name}")
         print_stars()
         install_hmy()
         print_stars()
         print("Harmony cli has been updated to: ")
-        os.system(f"{easy_env.hmy_app} version")
+        os.system(f"{EnvironmentVariables.hmy_app} version")
         print_stars()
-        set_var(easy_env.dotenv_file, "HMY_UPGRADE_AVAILABLE", "False")
+        set_var(EnvironmentVariables.dotenv_file, "HMY_UPGRADE_AVAILABLE", "False")
         input("* Update completed, press ENTER to return to the main menu. ")
 
+
 def update_harmony_app():
-    os.chdir(f"{easy_env.harmony_dir}")
+    os.chdir(f"{EnvironmentVariables.harmony_dir}")
     print_stars()
     print("Currently installed version: ")
     os.system("./harmony -V")
     folder_name = make_backup_dir()
-    os.system(f"cp {easy_env.harmony_dir}/harmony {easy_env.harmony_dir}/harmony.conf {folder_name}")
+    os.system(
+        f"cp {EnvironmentVariables.harmony_dir}/harmony {EnvironmentVariables.harmony_dir}/harmony.conf {folder_name}"
+    )
     print_stars()
     print("Downloading current harmony binary file from harmony.one: ")
     print_stars()
-    pull_harmony_update(easy_env.harmony_dir, easy_env.bls_key_file, easy_env.harmony_conf)
+    pull_harmony_update(
+        EnvironmentVariables.harmony_dir, EnvironmentVariables.bls_key_file, EnvironmentVariables.harmony_conf
+    )
     print_stars()
     print("Updated version: ")
     os.system("./harmony -V")
     if environ.get("SHARD") != "0":
         size = 0
-        for path, dirs, files in os.walk(f"{easy_env.harmony_dir}/harmony_db_0"):
+        for path, dirs, files in os.walk(f"{EnvironmentVariables.harmony_dir}/harmony_db_0"):
             for f in files:
                 fp = os.path.join(path, f)
                 size += os.path.getsize(fp)
             if size >= 400000000:
                 question = ask_yes_no(
                     Fore.WHITE
                     + "* Are you sure you would like to proceed with upgrading and trimming database 0?\n\nType 'Yes' or 'No' to continue"
                 )
                 if question:
                     os.system("sudo service harmony stop")
                     os.system(
-                        f"mv {easy_env.harmony_dir}/harmony_db_0 {easy_env.harmony_dir}/harmony_db_0_old"
+                        f"mv {EnvironmentVariables.harmony_dir}/harmony_db_0 {EnvironmentVariables.harmony_dir}/harmony_db_0_old"
                     )
                     os.system("sudo service harmony start")
-                    os.system(f"rm -r {easy_env.harmony_dir}/harmony_db_0_old")
+                    os.system(f"rm -r {EnvironmentVariables.harmony_dir}/harmony_db_0_old")
                 else:
                     print("Skipping removal of 0, but it's no longer required, fyi!")
             else:
                 print("Your database 0 is already trimmed, enjoy!")
     os.system("sudo service harmony restart")
     print_stars()
     print("Harmony Service is restarting, waiting 10 seconds for restart.")
-    set_var(easy_env.dotenv_file, "HARMONY_UPGRADE_AVAILABLE", "False")
+    set_var(EnvironmentVariables.dotenv_file, "HARMONY_UPGRADE_AVAILABLE", "False")
     time.sleep(10)
 
+
 def menu_validator_stats():
-    load_var_file(easy_env.dotenv_file)
+    load_var_file(EnvironmentVariables.dotenv_file)
     remote_shard_0 = [
-        f"{easy_env.hmy_app}",
+        f"{EnvironmentVariables.hmy_app}",
         "blockchain",
         "latest-headers",
         f'--node=https://api.s0.{environ.get("NETWORK_SWITCH")}.hmny.io',
     ]
     try:
         result_remote_shard_0 = run(remote_shard_0, stdout=PIPE, stderr=PIPE, universal_newlines=True)
         remote_data_shard_0 = json.loads(result_remote_shard_0.stdout)
     except (ValueError, KeyError, TypeError) as e:
-        print(f'* Remote Shard 0 Offline, Error {e}')
+        print(f"* Remote Shard 0 Offline, Error {e}")
     try:
-        local_shard = [f"{easy_env.hmy_app}", "blockchain", "latest-headers"]
+        local_shard = [f"{EnvironmentVariables.hmy_app}", "blockchain", "latest-headers"]
         result_local_shard = run(local_shard, stdout=PIPE, stderr=PIPE, universal_newlines=True)
         local_data_shard = json.loads(result_local_shard.stdout)
     except (ValueError, KeyError, TypeError) as e:
-        print(f'* Local Server Offline, restart your service or troubleshoot the issue by running the following in your ~/harmony directory:\n* ./harmony -c harmony.conf, Error: {e}')
-            
+        print(
+            f"* Local Server Offline, restart your service or troubleshoot the issue by running the following in your ~/harmony directory:\n* ./harmony -c harmony.conf, Error: {e}"
+        )
+
     if environ.get("SHARD") != "0":
         remote_shard = [
-            f"{easy_env.hmy_app}",
+            f"{EnvironmentVariables.hmy_app}",
             "blockchain",
             "latest-headers",
             f'--node=https://api.s{environ.get("SHARD")}.{environ.get("NETWORK_SWITCH")}.hmny.io',
         ]
         try:
             result_remote_shard = run(remote_shard, stdout=PIPE, stderr=PIPE, universal_newlines=True)
             remote_data_shard = json.loads(result_remote_shard.stdout)
             return remote_data_shard_0, local_data_shard, remote_data_shard
         except (ValueError, KeyError, TypeError):
             return
-        
+
     return remote_data_shard_0, local_data_shard, None
 
+
 def refresh_stats(clear=0) -> str:
     print(Fore.GREEN)
     if clear == 0:
         subprocess.run("clear")
     print_stars()
-    print(f'* Getting the latest local & blockchain information now, one moment while we load...')
+    print(f"* Getting the latest local & blockchain information now, one moment while we load...")
     print_stars()
     return
 
-def get_db_size(harmony_dir, our_shard) -> str:
-    harmony_db_size = subprocess.getoutput(f"du -h {harmony_dir}/harmony_db_{our_shard}")
-    harmony_db_size = harmony_db_size.rstrip("\t")
-    countTrim = len(easy_env.harmony_dir) + 13
-    return harmony_db_size[:-countTrim]
 
 def shard_stats(our_shard) -> str:
     our_uptime = subprocess.getoutput("uptime")
-    db_0_size = get_db_size(easy_env.harmony_dir, "0")
+    db_0_size = get_db_size(EnvironmentVariables.harmony_dir, "0")
     if our_shard == "0":
         print(
             f"""
     * Uptime :: {our_uptime}\n\n Harmony DB 0 Size  ::  {db_0_size}
     {string_stars()}
         """
         )
     else:
         print(
             f"""
     * Uptime :: {our_uptime}
     *
     * Harmony DB 0 Size  ::  {db_0_size}
-    * Harmony DB {our_shard} Size  ::   {get_db_size(easy_env.harmony_dir, str(our_shard))}
+    * Harmony DB {our_shard} Size  ::   {get_db_size(EnvironmentVariables.harmony_dir, str(our_shard))}
     *
     *
     {string_stars()}
         """
         )
 
+
 def harmony_binary_upgrade():
     question = ask_yes_no(
         Fore.RED
         + "* WARNING: YOU WILL MISS BLOCKS WHILE YOU UPGRADE THE HARMONY SERVICE.\n\n"
         + Fore.WHITE
         + "* Are you sure you would like to proceed?\n\nType 'Yes' or 'No' to continue"
     )
     if question:
         update_harmony_app()
 
+
 def menu_service_stop_start() -> str:
     status = os.system("systemctl is-active --quiet harmony")
     if status != 0:
         os.system("sudo service harmony start")
         print()
         print("* Harmony Service Has Been Started.")
         print()
@@ -588,52 +746,56 @@
             os.system("sudo service harmony stop")
             print()
             print(
                 "* Harmony Service Has Been Stopped. "
                 + Fore.RED
                 + "YOU ARE MISSING BLOCKS ON THIS NODE."
                 + Style.RESET_ALL
-+ Fore.GREEN
+                + Fore.GREEN
             )
             print()
             input("* Press ENTER to return to the main menu.")
 
+
 def menu_service_restart() -> str:
     question = ask_yes_no(
         "*********\n"
         + Fore.RED
         + "WARNING: YOU WILL MISS BLOCKS UNTIL RESTART IS COMPLETED & SYNC CATCHES UP!\n\n"
         + Fore.WHITE
         + "Are you sure you would like to proceed?\n\nType 'Yes' or 'No' to continue"
     )
     if question:
         os.system("sudo service harmony restart")
         print()
         print("* The Harmony Service Has Been Restarted")
         input("* Press ENTER to return to the main menu.")
 
+
 def menu_active_bls() -> str:
     validator_wallet = environ.get("VALIDATOR_WALLET")
     json_response = get_wallet_json(validator_wallet)
     print("* This is a list of your BLS Keys that are active for the next election.")
     for i, x in enumerate(json_response["bls-public-keys"]):
         print(f"BLS Key {i+1} {x}")
     print_stars()
     print("* Press ENTER to return to the main menu.")
     print_stars()
     input()
 
+
 # is this used?
 def is_float(value):
     try:
         float(value)
         return True
     except ValueError:
         return False
 
+
 def menu_check_balance(rpc, validator_wallet) -> None:
     if environ.get("NODE_TYPE") == "regular":
         print("* Calling mainnet and testnet for balances...")
         print_stars()
         total_balance, total_balance_test = get_wallet_balance(validator_wallet)
         print(f"* Your Validator Wallet Balance on Mainnet is: {total_balance} Harmony ONE Coins")
         print(f"* Your Pending Validator Rewards are: {get_rewards_balance(rpc, validator_wallet)}")
@@ -651,45 +813,48 @@
         while i < 1:
             question = ask_yes_no("* Would you like to check a Harmony ONE Address? (YES/NO) ")
             if question:
                 balanceCheckAny()
             else:
                 i = 1
 
+
 def balanceCheckAny():
     check_wallet = input(
         "* Type the address of the Harmony ONE Wallet you would like to check.\n"
         + "* Only one wallets will work, no 0x addresses : "
     )
     print("* Calling mainnet and testnet for balances...")
     print_stars()
     total_balance, total_balance_test = get_wallet_balance(check_wallet)
     print(
         f"* The Mainnet Wallet Balance is: {total_balance} Harmony ONE Coins\n* The Testnet Wallet Balance is: {total_balance_test} Harmony ONE Test Coins"
     )
     print_stars()
     input("* Press ENTER to continue.")
 
+
 def get_current_epoch():
     if environ.get("NETWORK") == "mainnet":
-        endpoints_count = len(easy_env.rpc_endpoints)
+        endpoints_count = len(EnvironmentVariables.rpc_endpoints)
     if environ.get("NETWORK") == "testnet":
-        endpoints_count = len(easy_env.rpc_endpoints_test)
+        endpoints_count = len(EnvironmentVariables.rpc_endpoints_test)
 
     for i in range(endpoints_count):
-        current_epoch = get_current_epochByEndpoint(easy_env.rpc_endpoints[i])
+        current_epoch = get_current_epochByEndpoint(EnvironmentVariables.rpc_endpoints[i])
 
         if current_epoch != -1:
             return current_epoch
     current_epoch = 0
     return current_epoch
 
+
 def get_current_epochByEndpoint(endpoint):
     current = 0
-    max_tries = easy_env.rpc_endpoints_max_connection_retries
+    max_tries = EnvironmentVariables.rpc_endpoints_max_connection_retries
     current_epoch = -1
 
     while current < max_tries:
         try:
             current_epoch = blockchain.get_current_epoch(endpoint)
             return current_epoch
         except Exception:
```

