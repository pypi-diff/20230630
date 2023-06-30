# Comparing `tmp/ecoindex_scraper-3.1.0.tar.gz` & `tmp/ecoindex_scraper-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoindex_scraper-3.1.0.tar", max compression
+gzip compressed data, was "ecoindex_scraper-3.2.0.tar", max compression
```

## Comparing `ecoindex_scraper-3.1.0.tar` & `ecoindex_scraper-3.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    18648 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/LICENSE
--rw-r--r--   0        0        0     4500 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/README.md
--rw-r--r--   0        0        0       35 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/ecoindex_scraper/__init__.py
--rw-r--r--   0        0        0     8450 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/ecoindex_scraper/scrap.py
--rw-r--r--   0        0        0      667 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/ecoindex_scraper/utils.py
--rw-r--r--   0        0        0      733 2023-06-19 15:57:41.764360 ecoindex_scraper-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 ecoindex_scraper-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    18648 2023-06-30 10:13:35.921999 ecoindex_scraper-3.2.0/LICENSE
+-rw-r--r--   0        0        0     4500 2023-06-30 10:13:35.921999 ecoindex_scraper-3.2.0/README.md
+-rw-r--r--   0        0        0       35 2023-06-30 10:13:35.921999 ecoindex_scraper-3.2.0/ecoindex_scraper/__init__.py
+-rw-r--r--   0        0        0     7997 2023-06-30 10:13:35.921999 ecoindex_scraper-3.2.0/ecoindex_scraper/scrap.py
+-rw-r--r--   0        0        0      667 2023-06-30 10:13:35.921999 ecoindex_scraper-3.2.0/ecoindex_scraper/utils.py
+-rw-r--r--   0        0        0      733 2023-06-30 10:13:35.921999 ecoindex_scraper-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 ecoindex_scraper-3.2.0/PKG-INFO
```

### Comparing `ecoindex_scraper-3.1.0/LICENSE` & `ecoindex_scraper-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.1.0/README.md` & `ecoindex_scraper-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.1.0/ecoindex_scraper/scrap.py` & `ecoindex_scraper-3.2.0/ecoindex_scraper/scrap.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+import asyncio
 from datetime import datetime
-from json import loads
+from genericpath import exists
 from os import remove
 from shutil import copyfile
 from time import sleep
 from typing import Dict, Tuple
 from uuid import uuid4
 
 import undetected_chromedriver as uc
 from ecoindex.ecoindex import get_ecoindex
 from ecoindex.models import PageMetrics, PageType, Result, ScreenShot, WindowSize
 from pydantic.networks import HttpUrl
 from selenium.common.exceptions import JavascriptException, NoSuchElementException
-from selenium.webdriver import DesiredCapabilities
 
 from ecoindex_scraper.utils import convert_screenshot_to_webp, set_screenshot_rights
 
 
 class EcoindexScraper:
     def __init__(
         self,
@@ -37,43 +37,76 @@
         self.screenshot = screenshot
         self.screenshot_uid = screenshot_uid
         self.screenshot_gid = screenshot_gid
         self.chrome_version_main = chrome_version_main
         self.page_load_timeout = page_load_timeout
 
         self.chrome_options = uc.ChromeOptions()
-        self.chrome_options.headless = True
         self.chrome_options.add_argument(f"--window-size={self.window_size}")
         self.chrome_options.add_argument("--no-sandbox")
         self.chrome_options.add_argument("--disable-dev-shm-usage")
         self.chrome_options.add_argument("--ignore-certificate-errors")
+        self.chrome_options.add_argument("--headless=new")
 
-        self.capbs = DesiredCapabilities.CHROME.copy()
-
-        self.capbs["goog:loggingPrefs"] = {"performance": "ALL"}  # type: ignore
+        self.all_requests = {}
+        self.page_response = False
 
         if driver_executable_path:
             self.driver_executable_path = f"/tmp/chromedriver_{uuid4()}"
             copyfile(driver_executable_path, self.driver_executable_path)
         else:
             self.driver_executable_path = None
 
     def __del__(self):
         if hasattr(self, "driver"):
             self.driver.quit()
 
-        if self.driver_executable_path:
+        if self.driver_executable_path and exists(self.driver_executable_path):
             remove(self.driver_executable_path)
 
+    def _handle_network_response_received(self, eventdata):
+        if eventdata["params"]["response"]["url"].startswith("http"):
+            self.all_requests[eventdata["params"]["requestId"]] = {
+                "url": eventdata["params"]["response"]["url"],
+                "size": 0,
+                "type": eventdata["params"]["type"],
+            }
+
+            if not self.page_response:
+                self.page_response = True
+                asyncio.run(self.check_page_response(eventdata["params"]["response"]))
+
+    def _handle_network_data_received(self, eventdata):
+        if eventdata["params"]["requestId"] in self.all_requests:
+            self.all_requests[eventdata["params"]["requestId"]]["size"] += eventdata[
+                "params"
+            ]["encodedDataLength"]
+
+    def _handle_network_loading_finished(self, eventdata):
+        if eventdata["params"]["requestId"] in self.all_requests:
+            self.all_requests[eventdata["params"]["requestId"]]["size"] = eventdata[
+                "params"
+            ]["encodedDataLength"]
+
     def init_chromedriver(self):
         self.driver = uc.Chrome(
             options=self.chrome_options,
-            desired_capabilities=self.capbs,
             version_main=self.chrome_version_main,
             driver_executable_path=self.driver_executable_path,
+            enable_cdp_events=True,
+        )
+
+        self.driver.add_cdp_listener(
+            "Network.dataReceived", self._handle_network_data_received
+        )
+        self.driver.add_cdp_listener(
+            "Network.responseReceived", self._handle_network_response_received
+        )
+        self.driver.add_cdp_listener(
+            "Network.loadingFinished", self._handle_network_loading_finished
         )
 
         if self.page_load_timeout is not None:
             self.driver.set_page_load_timeout(float(self.page_load_timeout))
 
         return self
 
@@ -141,69 +174,23 @@
             )
         except JavascriptException:
             pass
 
     async def get_page_metrics(self) -> PageMetrics:
         nodes = self.driver.find_elements("xpath", "//*")
         nb_svg_children = await self.get_svg_children_count()
-        all_requests = await self.get_all_requests()
 
-        downloaded_data = [request["size"] for request in all_requests.values()]
+        downloaded_data = [request["size"] for request in self.all_requests.values()]
 
         return PageMetrics(
             size=sum(downloaded_data) / (10**3),
             nodes=(len(nodes) - nb_svg_children),
-            requests=len(all_requests),
+            requests=len(self.all_requests),
         )
 
-    async def get_all_requests(self) -> Dict:
-        all_requests = {}
-        page_response = False
-        performance_logs = self.driver.get_log("performance")
-
-        for log in performance_logs:
-            message = loads(log["message"])
-
-            if (
-                "INFO" == log["level"]
-                and "Network.responseReceived" == message["message"]["method"]
-                and message["message"]["params"]["response"]["url"].startswith("http")
-            ):
-                all_requests[message["message"]["params"]["requestId"]] = {
-                    "url": message["message"]["params"]["response"]["url"],
-                    "size": 0,
-                    "type": message["message"]["params"]["type"],
-                }
-
-                if not page_response:
-                    page_response = True
-                    await self.check_page_response(
-                        message["message"]["params"]["response"]
-                    )
-
-            if (
-                "INFO" == log["level"]
-                and "Network.dataReceived" == message["message"]["method"]
-                and message["message"]["params"]["requestId"] in all_requests
-            ):
-                all_requests[message["message"]["params"]["requestId"]][
-                    "size"
-                ] += message["message"]["params"]["encodedDataLength"]
-
-            if (
-                "INFO" == log["level"]
-                and "Network.loadingFinished" == message["message"]["method"]
-                and message["message"]["params"]["requestId"] in all_requests
-            ):
-                all_requests[message["message"]["params"]["requestId"]][
-                    "size"
-                ] = message["message"]["params"]["encodedDataLength"]
-
-        return all_requests
-
     @staticmethod
     async def check_page_response(response: Dict) -> None:
         if response["mimeType"] != "text/html":
             raise TypeError(
                 {
                     "mimetype": response["mimeType"],
                     "message": (
```

### Comparing `ecoindex_scraper-3.1.0/ecoindex_scraper/utils.py` & `ecoindex_scraper-3.2.0/ecoindex_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.1.0/pyproject.toml` & `ecoindex_scraper-3.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "ecoindex_scraper"
-version = "3.1.0"
+version = "3.2.0"
 description = "Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser"
 authors = ["Vincent Vatelot <vincent.vatelot@ik.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://www.ecoindex.fr"
 repository = "https://github.com/cnumr/ecoindex_scraper_python"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ecoindex = "^5.4.2"
-undetected-chromedriver = "3.4.7"
+undetected-chromedriver = "3.5.0"
 Pillow = "^9.2.0"
 selenium = "4.9"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3"
+pytest = "^7.4"
 black = {version = "^23.3.0", allow-prereleases = true}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ecoindex_scraper-3.1.0/PKG-INFO` & `ecoindex_scraper-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ecoindex-scraper
-Version: 3.1.0
+Version: 3.2.0
 Summary: Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser
 Home-page: http://www.ecoindex.fr
 License: MIT
 Author: Vincent Vatelot
 Author-email: vincent.vatelot@ik.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: ecoindex (>=5.4.2,<6.0.0)
 Requires-Dist: selenium (==4.9)
-Requires-Dist: undetected-chromedriver (==3.4.7)
+Requires-Dist: undetected-chromedriver (==3.5.0)
 Project-URL: Repository, https://github.com/cnumr/ecoindex_scraper_python
 Description-Content-Type: text/markdown
 
 # ECOINDEX SCRAPER PYTHON
 
 ![Quality check](https://github.com/cnumr/ecoindex_scrap_python/workflows/Quality%20checks/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ecoindex-scraper.svg)](https://badge.fury.io/py/ecoindex-scraper)
```

