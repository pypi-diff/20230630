# Comparing `tmp/riseup_vpn_configurator-1.0.0.tar.gz` & `tmp/riseup_vpn_configurator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riseup_vpn_configurator-1.0.0.tar", max compression
+gzip compressed data, was "riseup_vpn_configurator-1.0.1.tar", max compression
```

## Comparing `riseup_vpn_configurator-1.0.0.tar` & `riseup_vpn_configurator-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-02-13 13:46:29.483007 riseup_vpn_configurator-1.0.0/LICENSE
--rw-r--r--   0        0        0     5520 2023-06-04 19:44:35.142687 riseup_vpn_configurator-1.0.0/README.md
--rw-r--r--   0        0        0     1137 2023-06-04 19:45:13.419493 riseup_vpn_configurator-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    16767 2023-06-04 19:41:37.418707 riseup_vpn_configurator-1.0.0/riseup_vpn_configurator/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 16:23:10.812807 riseup_vpn_configurator-1.0.0/riseup_vpn_configurator/latency.py
--rw-r--r--   0        0        0      305 2023-02-27 16:08:48.769650 riseup_vpn_configurator-1.0.0/riseup_vpn_configurator/riseup-vpn.yaml
--rw-r--r--   0        0        0     6442 1970-01-01 00:00:00.000000 riseup_vpn_configurator-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-13 13:46:29.483007 riseup_vpn_configurator-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5798 2023-06-30 10:33:47.769553 riseup_vpn_configurator-1.0.1/README.md
+-rw-r--r--   0        0        0     1137 2023-06-30 10:35:45.850012 riseup_vpn_configurator-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    18316 2023-06-30 10:29:51.668637 riseup_vpn_configurator-1.0.1/riseup_vpn_configurator/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-27 16:23:10.812807 riseup_vpn_configurator-1.0.1/riseup_vpn_configurator/latency.py
+-rw-r--r--   0        0        0      305 2023-02-27 16:08:48.769650 riseup_vpn_configurator-1.0.1/riseup_vpn_configurator/riseup-vpn.yaml
+-rw-r--r--   0        0        0     6720 1970-01-01 00:00:00.000000 riseup_vpn_configurator-1.0.1/PKG-INFO
```

### Comparing `riseup_vpn_configurator-1.0.0/LICENSE` & `riseup_vpn_configurator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `riseup_vpn_configurator-1.0.0/README.md` & `riseup_vpn_configurator-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,18 @@
   --uninstall           remove all files in /opt/riseup-vpn
   -l, --list-gateways   show available VPN server
   -b, --benchmark       use with --list - pings the gateway and shows the latency
   -c, --check-config    check syntax of /etc/riseup-vpn.yaml. Generates default config
   -g, --generate-config
                         Generate openvpn config (/etc/openvpn/client/riseup.conf)
   -s, --status          show current state of riseup-vpn
+  --start               starts openvpn service
+  --stop                stops openvpn service
+  --restart             restarts openvpn service
+  --log                 show systemd log
   --version             show version
 ```
 
 Default config file `/etc/riseup-vpn.yaml`
 ```yamy
 ---
 # /etc/riseup-vpn.yaml
@@ -78,14 +82,19 @@
 root@linbox:riseup-vpn-configurator poetry run mypy riseup_vpn_configurator/
 ```
 
 # How it works
 
 The code for the RiseupVPN Linux client can be found [here](https://0xacab.org/leap/bitmask-vpn). It uses OpenVPN. Everyone uses the same client certificate/key to authenticate. The client certificate is only valid for 90 days. The VPN gateway list and client certificate can be fetched by a public API.
 
+# Allow for non-root user
+```bash
+kmille ALL = NOPASSWD: /usr/bin/riseup-vpn-configurator
+```
+
 # Monitoring with py3status
 
 If you use [py3status](https://github.com/ultrabug/py3status) as i3bar implementation, you can use [monitor_riseupvpn.py](/monitoring/monitor_riseupvpn.py) for monitoring.
 
 # Known issues
 
 RiseupVPN does not support IPv6. It's routed over the tunnel but then gets blocked. Also, the VPN hangs after suspend ([see Arch Wiki](https://wiki.archlinux.org/title/OpenVPN#Client_daemon_not_reconnecting_after_suspend)). To solve this issue, the AUR package uses [openvpn-reconnect](https://aur.archlinux.org/packages/openvpn-reconnect) as a dependency.
```

### Comparing `riseup_vpn_configurator-1.0.0/pyproject.toml` & `riseup_vpn_configurator-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "riseup-vpn-configurator"
-version = "1.0.0"
+version = "1.0.1"
 description = "a simple command line tool to get RiseupVPN up and running"
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 packages = [{include = "riseup_vpn_configurator"}]
 license = "GPL-3.0-only"
 repository = "https://github.com/kmille/riseup-vpn-configurator"
 homepage = "https://github.com/kmille/riseup-vpn-configurator"
```

### Comparing `riseup_vpn_configurator-1.0.0/riseup_vpn_configurator/__init__.py` & `riseup_vpn_configurator-1.0.1/riseup_vpn_configurator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 import sys
 import os
 import logging
 import argparse
 import json
 import yaml
+import subprocess
 import pwd
 import grp
 from jinja2 import Template
 from pathlib import Path
 import requests
 from ipaddress import ip_network
 from pyasn1_modules import pem, rfc2459
@@ -404,14 +405,43 @@
 
     delete(working_dir)
     delete(config_file)
     delete(ovpn_file)
     sys.exit(0)
 
 
+def print_error_log():
+    logging.info("Printing debug log")
+    try:
+        p = subprocess.run(["journalctl", "-u", "openvpn-client@riseup", "-n", "50"], capture_output=True)
+        logging.info(p.stdout.decode())
+    except subprocess.CalledProcessError as e:
+        logging.error(f"Could not start riseup vpn: {e}")
+
+
+def start_openvpn():
+    try:
+        subprocess.run(["systemctl", "start", "openvpn-client@riseup"], check=True, capture_output=True)
+    except subprocess.CalledProcessError as e:
+        logging.error(f"Could not start riseup vpn: {e}")
+        print_error_log()
+    else:
+        logging.info("riseupvpn sucessfully started")
+
+
+def stop_openvpn():
+    try:
+        subprocess.run(["systemctl", "stop", "openvpn-client@riseup"], check=True, capture_output=True)
+    except subprocess.CalledProcessError as e:
+        logging.error(f"Could not stop riseup vpn: {e}")
+        print_error_log()
+    else:
+        logging.info("riseupvpn sucessfully stopped")
+
+
 def show_version():
     from importlib.metadata import version
     app_name = "riseup-vpn-configurator"
     logging.info(f"Running {app_name} v{version(app_name)}")
     sys.exit()
 
 
@@ -424,14 +454,18 @@
     parser.add_argument("-u", "--update", action="store_true", help="update gateway list and client certificate/key")
     parser.add_argument("--uninstall", action="store_true", help=f"remove all files in {working_dir}")
     parser.add_argument("-l", "--list-gateways", action="store_true", help="show available VPN server")
     parser.add_argument("-b", "--benchmark", action="store_true", help="use with --list - pings the gateway and shows the latency")
     parser.add_argument("-c", "--check-config", action="store_true", help=f"check syntax of {config_file}. Generates default config")
     parser.add_argument("-g", "--generate-config", action="store_true", help=f"Generate openvpn config ({ovpn_file})")
     parser.add_argument("-s", "--status", action="store_true", help="show current state of riseup-vpn")
+    parser.add_argument("--start", action="store_true", help="starts openvpn service")
+    parser.add_argument("--stop", action="store_true", help="stops openvpn service")
+    parser.add_argument("--restart", action="store_true", help="restarts openvpn service")
+    parser.add_argument("--log", action="store_true", help="show systemd log")
     parser.add_argument("--version", action="store_true", help="show version")
 
     args = parser.parse_args()
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
 
@@ -462,11 +496,20 @@
         list_gateways(args.benchmark)
     elif args.generate_config:
         check_config_file()
         generate_configuration()
     elif args.status:
         check_config_file()
         show_status()
+    elif args.start:
+        start_openvpn()
+    elif args.stop:
+        stop_openvpn()
+    elif args.restart:
+        stop_openvpn()
+        start_openvpn()
+    elif args.log:
+        print_error_log()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `riseup_vpn_configurator-1.0.0/PKG-INFO` & `riseup_vpn_configurator-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riseup-vpn-configurator
-Version: 1.0.0
+Version: 1.0.1
 Summary: a simple command line tool to get RiseupVPN up and running
 Home-page: https://github.com/kmille/riseup-vpn-configurator
 License: GPL-3.0-only
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -61,14 +61,18 @@
   --uninstall           remove all files in /opt/riseup-vpn
   -l, --list-gateways   show available VPN server
   -b, --benchmark       use with --list - pings the gateway and shows the latency
   -c, --check-config    check syntax of /etc/riseup-vpn.yaml. Generates default config
   -g, --generate-config
                         Generate openvpn config (/etc/openvpn/client/riseup.conf)
   -s, --status          show current state of riseup-vpn
+  --start               starts openvpn service
+  --stop                stops openvpn service
+  --restart             restarts openvpn service
+  --log                 show systemd log
   --version             show version
 ```
 
 Default config file `/etc/riseup-vpn.yaml`
 ```yamy
 ---
 # /etc/riseup-vpn.yaml
@@ -101,14 +105,19 @@
 root@linbox:riseup-vpn-configurator poetry run mypy riseup_vpn_configurator/
 ```
 
 # How it works
 
 The code for the RiseupVPN Linux client can be found [here](https://0xacab.org/leap/bitmask-vpn). It uses OpenVPN. Everyone uses the same client certificate/key to authenticate. The client certificate is only valid for 90 days. The VPN gateway list and client certificate can be fetched by a public API.
 
+# Allow for non-root user
+```bash
+kmille ALL = NOPASSWD: /usr/bin/riseup-vpn-configurator
+```
+
 # Monitoring with py3status
 
 If you use [py3status](https://github.com/ultrabug/py3status) as i3bar implementation, you can use [monitor_riseupvpn.py](/monitoring/monitor_riseupvpn.py) for monitoring.
 
 # Known issues
 
 RiseupVPN does not support IPv6. It's routed over the tunnel but then gets blocked. Also, the VPN hangs after suspend ([see Arch Wiki](https://wiki.archlinux.org/title/OpenVPN#Client_daemon_not_reconnecting_after_suspend)). To solve this issue, the AUR package uses [openvpn-reconnect](https://aur.archlinux.org/packages/openvpn-reconnect) as a dependency.
```

