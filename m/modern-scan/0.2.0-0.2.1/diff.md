# Comparing `tmp/modern_scan-0.2.0.tar.gz` & `tmp/modern_scan-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modern_scan-0.2.0.tar", max compression
+gzip compressed data, was "modern_scan-0.2.1.tar", max compression
```

## Comparing `modern_scan-0.2.0.tar` & `modern_scan-0.2.1.tar`

### file list

```diff
@@ -1,67 +1,18 @@
--rw-r--r--   0        0        0        0 2023-02-04 20:22:15.763683 modern_scan-0.2.0/mscan/__init__.py
--rw-r--r--   0        0        0     2053 2023-02-05 00:37:11.339321 modern_scan-0.2.0/mscan/main.py
--rw-r--r--   0        0        0        0 2023-02-04 20:22:15.763683 modern_scan-0.2.0/mscan/scanner/__init__.py
--rw-r--r--   0        0        0      151 2023-02-04 20:23:31.196782 modern_scan-0.2.0/mscan/scanner/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1904 2023-02-04 23:18:22.690779 modern_scan-0.2.0/mscan/scanner/__pycache__/arp.cpython-38.pyc
--rw-r--r--   0        0        0     2412 2023-02-04 23:18:22.327543 modern_scan-0.2.0/mscan/scanner/__pycache__/interface.cpython-38.pyc
--rw-r--r--   0        0        0      621 2023-02-04 23:18:22.706418 modern_scan-0.2.0/mscan/scanner/__pycache__/multi_ping.cpython-38.pyc
--rw-r--r--   0        0        0      800 2023-02-04 23:18:22.706418 modern_scan-0.2.0/mscan/scanner/__pycache__/network.cpython-38.pyc
--rw-r--r--   0        0        0      589 2023-02-04 23:18:22.706418 modern_scan-0.2.0/mscan/scanner/__pycache__/platform_detector.cpython-38.pyc
--rw-r--r--   0        0        0     3293 2023-02-04 23:59:58.459939 modern_scan-0.2.0/mscan/scanner/__pycache__/scanner.cpython-38.pyc
--rw-r--r--   0        0        0     1617 2023-02-04 23:10:29.170150 modern_scan-0.2.0/mscan/scanner/arp.py
--rw-r--r--   0        0        0     1429 2023-02-04 23:10:57.582752 modern_scan-0.2.0/mscan/scanner/interface.py
--rw-r--r--   0        0        0      261 2023-02-04 23:13:02.072257 modern_scan-0.2.0/mscan/scanner/multi_ping.py
--rw-r--r--   0        0        0      458 2023-02-04 23:14:12.322281 modern_scan-0.2.0/mscan/scanner/network.py
--rw-r--r--   0        0        0      396 2023-02-04 23:14:39.003126 modern_scan-0.2.0/mscan/scanner/ping.py
--rw-r--r--   0        0        0      265 2023-02-05 00:16:29.448165 modern_scan-0.2.0/mscan/scanner/platform_detector.py
--rw-r--r--   0        0        0     2507 2023-02-04 23:56:19.183830 modern_scan-0.2.0/mscan/scanner/scanner.py
--rw-r--r--   0        0        0      673 2023-02-05 00:05:48.570266 modern_scan-0.2.0/mscan/settings.py
--rw-r--r--   0        0        0     4395 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/asset-manifest.json
--rw-r--r--   0        0        0   109976 2023-02-04 20:22:15.794946 modern_scan-0.2.0/mscan/static/favicon.ico
--rw-r--r--   0        0        0      834 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/index.html
--rw-r--r--   0        0        0     8819 2023-02-04 20:22:15.794946 modern_scan-0.2.0/mscan/static/logo192.png
--rw-r--r--   0        0        0    37002 2023-02-04 20:22:15.794946 modern_scan-0.2.0/mscan/static/logo512.png
--rw-r--r--   0        0        0      517 2023-02-04 20:22:15.794946 modern_scan-0.2.0/mscan/static/manifest.json
--rw-r--r--   0        0        0       70 2023-02-04 20:22:15.794946 modern_scan-0.2.0/mscan/static/robots.txt
--rw-r--r--   0        0        0     9524 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/css/main.4410bb71.css
--rw-r--r--   0        0        0    12833 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/css/main.4410bb71.css.map
--rw-r--r--   0        0        0   386606 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/js/main.1c24d240.js
--rw-r--r--   0        0        0     1768 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/js/main.1c24d240.js.LICENSE.txt
--rw-r--r--   0        0        0  1461026 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/js/main.1c24d240.js.map
--rw-r--r--   0        0        0    21303 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/empty.8be6f3ae16ca45ad1516147683979f97.svg
--rw-r--r--   0        0        0    65164 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-all-300-normal.168d6383e73339293ac3.woff
--rw-r--r--   0        0        0    65456 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff
--rw-r--r--   0        0        0    65756 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-all-500-normal.0ab669b7a0d19b178f57.woff
--rw-r--r--   0        0        0    65556 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-all-700-normal.a457fde362a540fcadff.woff
--rw-r--r--   0        0        0     9576 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-cyrillic-300-normal.1431d1cef06ad04f5458.woff2
--rw-r--r--   0        0        0     9628 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-cyrillic-400-normal.71a33b6b50457b2c903a.woff2
--rw-r--r--   0        0        0     9840 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-cyrillic-500-normal.cad7d3d9cb265e334e58.woff2
--rw-r--r--   0        0        0     9644 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-cyrillic-700-normal.d010f1f324e111a22e53.woff2
--rw-r--r--   0        0        0    15000 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-cyrillic-ext-300-normal.4777461b144e55145268.woff2
--rw-r--r--   0        0        0    15344 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-cyrillic-ext-400-normal.804378952da8a10faae2.woff2
--rw-r--r--   0        0        0    14968 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-cyrillic-ext-500-normal.62ced72e5832f02c2796.woff2
--rw-r--r--   0        0        0    14684 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-cyrillic-ext-700-normal.be4d02458ce53887dc37.woff2
--rw-r--r--   0        0        0     7120 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-greek-300-normal.db2632771401f61463fe.woff2
--rw-r--r--   0        0        0     7112 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-greek-400-normal.c35e4c3958e209d17b31.woff2
--rw-r--r--   0        0        0     7016 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-greek-500-normal.9ac81fefbe6c319ea40b.woff2
--rw-r--r--   0        0        0     6936 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-greek-700-normal.50e795c1345353b0e996.woff2
--rw-r--r--   0        0        0     1480 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-greek-ext-300-normal.35b9d6be04b95f0f0530.woff2
--rw-r--r--   0        0        0     1484 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-greek-ext-400-normal.169619821ea93019d1bb.woff2
--rw-r--r--   0        0        0     1500 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-greek-ext-500-normal.6fb9cffb1d3e72bf9293.woff2
--rw-r--r--   0        0        0     1432 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-greek-ext-700-normal.bd9854c751441ccc1a70.woff2
--rw-r--r--   0        0        0    15740 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-latin-300-normal.c48fb6765a9fcb00b330.woff2
--rw-r--r--   0        0        0    15744 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-latin-400-normal.b009a76ad6afe4ebd301.woff2
--rw-r--r--   0        0        0    15920 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-latin-500-normal.f25d774ecfe0996f8eb5.woff2
--rw-r--r--   0        0        0    15860 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-latin-700-normal.227c93190fe7f82de3f8.woff2
--rw-r--r--   0        0        0    11796 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-latin-ext-300-normal.dc7dcec8e3f654e0ed63.woff2
--rw-r--r--   0        0        0    11872 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-latin-ext-400-normal.861b791f9de857a6e7bc.woff2
--rw-r--r--   0        0        0    11800 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-latin-ext-500-normal.9165081d10e1ba601384.woff2
--rw-r--r--   0        0        0    11824 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-latin-ext-700-normal.ed67ad54b1a8f5d21150.woff2
--rw-r--r--   0        0        0     5468 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-vietnamese-300-normal.32fc45a3d1e8ea11fabc.woff2
--rw-r--r--   0        0        0     5560 2023-02-05 00:41:08.634309 modern_scan-0.2.0/mscan/static/static/media/roboto-vietnamese-400-normal.3230f9b040f3c630e0c3.woff2
--rw-r--r--   0        0        0     5604 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-vietnamese-500-normal.d8642a3d1d4ef6179644.woff2
--rw-r--r--   0        0        0     5548 2023-02-05 00:41:08.649899 modern_scan-0.2.0/mscan/static/static/media/roboto-vietnamese-700-normal.3425a701027d0699e369.woff2
--rw-r--r--   0        0        0      574 2023-02-05 00:41:13.367912 modern_scan-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      564 2023-02-04 20:22:15.763683 modern_scan-0.2.0/README.md
--rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 modern_scan-0.2.0/setup.py
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 modern_scan-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-29 21:24:14.687475 modern_scan-0.2.1/mscan/__init__.py
+-rw-r--r--   0        0        0     2221 2023-06-30 09:00:30.770192 modern_scan-0.2.1/mscan/main.py
+-rw-r--r--   0        0        0        0 2023-06-29 21:24:14.687475 modern_scan-0.2.1/mscan/scanner/__init__.py
+-rw-r--r--   0        0        0     2799 2023-06-29 21:30:51.774192 modern_scan-0.2.1/mscan/scanner/arp.py
+-rw-r--r--   0        0        0     1429 2023-06-29 21:24:14.687475 modern_scan-0.2.1/mscan/scanner/interface.py
+-rw-r--r--   0        0        0      261 2023-06-29 21:24:14.687475 modern_scan-0.2.1/mscan/scanner/multi_ping.py
+-rw-r--r--   0        0        0      458 2023-06-29 21:24:14.687475 modern_scan-0.2.1/mscan/scanner/network.py
+-rw-r--r--   0        0        0      396 2023-06-29 21:24:14.687475 modern_scan-0.2.1/mscan/scanner/ping.py
+-rw-r--r--   0        0        0      454 2023-06-30 08:56:46.738083 modern_scan-0.2.1/mscan/scanner/platform_detector.py
+-rw-r--r--   0        0        0     3659 2023-06-30 09:05:08.856351 modern_scan-0.2.1/mscan/scanner/scanner.py
+-rw-r--r--   0        0        0      672 2023-06-30 09:58:08.696667 modern_scan-0.2.1/mscan/settings.py
+-rw-r--r--   0        0        0    11171 2023-06-30 18:18:53.780723 modern_scan-0.2.1/mscan/static/assets/index-560f337d.css
+-rw-r--r--   0        0        0   210569 2023-06-30 18:18:53.780723 modern_scan-0.2.1/mscan/static/assets/index-8def36ff.js
+-rw-r--r--   0        0        0      445 2023-06-30 18:18:53.780723 modern_scan-0.2.1/mscan/static/index.html
+-rw-r--r--   0        0        0     6060 2023-06-30 17:29:52.188606 modern_scan-0.2.1/mscan/static/logo.png
+-rw-r--r--   0        0        0      574 2023-06-30 18:24:41.029437 modern_scan-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      877 2023-06-30 18:17:33.765589 modern_scan-0.2.1/README.md
+-rw-r--r--   0        0        0     1558 1970-01-01 00:00:00.000000 modern_scan-0.2.1/PKG-INFO
```

### Comparing `modern_scan-0.2.0/mscan/main.py` & `modern_scan-0.2.1/mscan/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from mscan.scanner.scanner import Scanner
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.staticfiles import StaticFiles
 from starlette.responses import FileResponse
 import uvicorn
 import socket
+import asyncio
 
 app = FastAPI()
 scanner = Scanner()
 imanager = InterfaceManager()
 
 origins = ["*"]
 app.add_middleware(
@@ -57,14 +58,19 @@
 
 
 def open_in_browser(host):
     webbrowser.open(f'{settings.PROTOCOL}://{host}:{settings.PORT}')
 
 
 def main():
+    # interfaces = list(imanager.get_interfaces())
+    # i = interfaces[3]
+    # res = await scanner.scan(i)
+    # print(res)
+    # return
     host = settings.HOST
     if settings.HOST == '0.0.0.0':
         host = local_ip() or settings.HOST
 
     print(f"Mscan running at {settings.PROTOCOL}://{host}:{settings.PORT}/")
     threading.Timer(1.25, open_in_browser, (host, ) ).start()
     uvicorn.run(
@@ -75,7 +81,9 @@
         workers=1,
         log_level=settings.LOG_LEVEL
     )
 
 
 if __name__ == '__main__':
     main()
+    
+
```

### Comparing `modern_scan-0.2.0/mscan/scanner/interface.py` & `modern_scan-0.2.1/mscan/scanner/interface.py`

 * *Files identical despite different names*

### Comparing `modern_scan-0.2.0/mscan/scanner/scanner.py` & `modern_scan-0.2.1/mscan/scanner/scanner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import concurrent.futures
 import socket
 from dataclasses import dataclass, asdict
 from typing import List
-
 from mac_vendor_lookup import AsyncMacLookup
-
+from .platform_detector import Platform
 from .arp import Arp, Host as ArpHost
 from .interface import Interface
 from .multi_ping import MultiPinger
 from .network import Network
-
+import re
 
 @dataclass
 class LiveHost:
     ip: str
     mac: str
     vendor: str
     hostname: str
@@ -23,15 +22,31 @@
 
 
 class Scanner:
     BLACKLIST_PREFIX = [str(i) for i in range(220, 265)]
     BLACKLIST_SUFFIX = ['255']
 
     @staticmethod
-    def get_hostnames(hosts: List[ArpHost], max_workers=20):
+    def get_hostname(host):
+        try:
+            return socket.gethostbyaddr(host['ip'])[0]
+        except:
+            return ''
+
+    @staticmethod
+    def get_hostnames(hosts):
+        with concurrent.futures.ThreadPoolExecutor(max_workers=2500) as executer:
+            results = []
+            for host, result in zip(hosts, executer.map(Scanner.get_hostname, hosts)):
+                if result:
+                    results.append({**host, 'hostname': result})
+        return results
+
+    @staticmethod
+    def get_hostnames(hosts: List[ArpHost], max_workers=2500):
 
         def job(arp_host: ArpHost):
             try:
                 hostname = socket.gethostbyaddr(arp_host.addr)[0]
             except:
                 hostname = "unknown"
             return {"host": arp_host, "name": hostname}
@@ -65,14 +80,28 @@
             prefix = host.addr[:3]
             if prefix not in Scanner.BLACKLIST_PREFIX and suffix not in Scanner.BLACKLIST_SUFFIX:
                 vendor = await Scanner.get_vendor(host.hwaddr)
                 live_host = LiveHost(host.addr, host.hwaddr, vendor, hostnames.get(host.addr, "unknown"))
                 live_hosts.append(live_host)
         return live_hosts
 
+
+    def arp_scan(self, hosts):
+        with concurrent.futures.ThreadPoolExecutor(max_workers=2500) as executer:
+            results = []
+            for host, result in zip(hosts, executer.map(Arp.get_mac, hosts)):
+                if result:
+                    result = re.sub(r'(..)', r'\1:', result)[:-1]
+                    result = result.upper()
+                    results.append(ArpHost(addr=host, hwaddr=result, addr_type='dynamic'))
+        return results
+    
     async def scan(self, iface: Interface) -> List[LiveHost]:
         network = Network.from_interface(iface)
         ips = [str(i) for i in network.ips]
-        await MultiPinger().ping(ips)
-        hosts = Arp.get_tables(iface)
+        if Platform.WINDOWS:
+            hosts = self.arp_scan(ips)
+        else:
+            await MultiPinger().ping(ips)
+            hosts = Arp.get_tables(iface)
         live = await self.get_live_hosts(hosts)
         return live
```

### Comparing `modern_scan-0.2.0/mscan/settings.py` & `modern_scan-0.2.1/mscan/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
 # Server settings
 PROTOCOL = 'http'
 HOST = args.host
 PORT = args.port
 
 # UI settings
-UI_BUILD_PATH = (Path(__file__).parent / ("../../ui/build" if DEV_MODE else 'static')).resolve().absolute()
+UI_BUILD_PATH = (Path(__file__).parent / ("../../ui/dist" if DEV_MODE else 'static')).resolve().absolute()
 UI_BUILD_PATH.mkdir(exist_ok=True)
```

### Comparing `modern_scan-0.2.0/pyproject.toml` & `modern_scan-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "modern-scan"
 packages = [
     {include = "mscan"}
 ]
-version = "0.2.0"
+version = "0.2.1"
 description = "Modern network scanner"
 authors = ["thewh1teagle <61390950+thewh1teagle@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = "^0.89.1"
```

### Comparing `modern_scan-0.2.0/PKG-INFO` & `modern_scan-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modern-scan
-Version: 0.2.0
+Version: 0.2.1
 Summary: Modern network scanner
 Author: thewh1teagle
 Author-email: 61390950+thewh1teagle@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,23 +19,34 @@
 
 # Mscan
 
 <img with="150px" height="150px" src="https://user-images.githubusercontent.com/61390950/182006521-350c306a-2567-49eb-b77a-42224783768f.png">  
 
 ## A modern network scanner
 ## 🖥 User Interface
-![image](https://user-images.githubusercontent.com/61390950/182006567-5e5cfcbe-7549-4205-902e-54706d2c1793.png)
+![image](https://user-images.githubusercontent.com/61390950/216823967-a06601df-4d3f-41a2-9324-ca0c5c5b9a52.png)
 
 ## 💿 Installation
 Install from pypi
 ```
 pip3 install --upgrade modern-scan
 ```
-then simply execute
-```mscan```
-
+## 🖥 Usage
+Simply run the command mscan
+```shell
+$ mscan
+Mscan running at http://127.0.0.1:8000/
+```
 ## ✨ Features
 
 - 🕹 Simple and clear user interface
+- 🌐️️ Cross platform
 - 🚀 Super fast
 - 🛠 More features in development
 
+## 🔌 API
+Mscan offers an API which you can access at the following route:
+```
+/docs
+```
+This endpoint contains all the necessary information to get started with using the Mscan API in your software.
+
```

