# Comparing `tmp/finops-0.1.4.tar.gz` & `tmp/finops-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.1.4.tar", last modified: Thu Jun 29 13:56:00 2023, max compression
+gzip compressed data, was "finops-0.1.5.tar", last modified: Fri Jun 30 14:58:50 2023, max compression
```

## Comparing `finops-0.1.4.tar` & `finops-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-29 13:55:48.000000 finops-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-29 13:56:00.862787 finops-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-29 13:55:48.000000 finops-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/finops/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 13:55:48.000000 finops-0.1.4/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-29 13:55:48.000000 finops-0.1.4/finops/codal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-29 13:55:48.000000 finops-0.1.4/finops/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 13:55:48.000000 finops-0.1.4/finops/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-29 13:55:48.000000 finops-0.1.4/finops/tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-29 13:55:48.000000 finops-0.1.4/finops/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/finops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:56:00.862787 finops-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-29 13:55:48.000000 finops-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:55:48.000000 finops-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_utils/test_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:50.342915 finops-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-30 14:58:41.000000 finops-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-30 14:58:50.342915 finops-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-30 14:58:41.000000 finops-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:50.338915 finops-0.1.5/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 14:58:41.000000 finops-0.1.5/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-30 14:58:41.000000 finops-0.1.5/finops/codal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-30 14:58:41.000000 finops-0.1.5/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 14:58:41.000000 finops-0.1.5/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-30 14:58:41.000000 finops-0.1.5/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-30 14:58:41.000000 finops-0.1.5/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:50.338915 finops-0.1.5/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:41.000000 finops-0.1.5/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-30 14:58:41.000000 finops-0.1.5/finops/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-06-30 14:58:41.000000 finops-0.1.5/finops/utils/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-30 14:58:41.000000 finops-0.1.5/finops/utils/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-30 14:58:41.000000 finops-0.1.5/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:50.338915 finops-0.1.5/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-30 14:58:50.000000 finops-0.1.5/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 14:58:50.000000 finops-0.1.5/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:58:50.000000 finops-0.1.5/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 14:58:50.000000 finops-0.1.5/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 14:58:50.000000 finops-0.1.5/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:58:50.342915 finops-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-30 14:58:41.000000 finops-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:50.338915 finops-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:41.000000 finops-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-30 14:58:41.000000 finops-0.1.5/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-30 14:58:41.000000 finops-0.1.5/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:50.342915 finops-0.1.5/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:41.000000 finops-0.1.5/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-30 14:58:41.000000 finops-0.1.5/tests/test_utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-30 14:58:41.000000 finops-0.1.5/tests/test_utils/test_scraper.py
```

### Comparing `finops-0.1.4/LICENSE` & `finops-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/PKG-INFO` & `finops-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.1.4/README.md` & `finops-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/finops/codal.py` & `finops-0.1.5/finops/codal.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,25 +13,30 @@
 from finops.utils.preprocessor import Preprocessor
 from finops.utils.wrappers import sleep, retry
 from finops.config import (
     CODAL_SEARCH_BASE_URL,
     CODAL_LETTERS_LIST_COLUMNS,
     BALANCE_SHEET_ID,
     PNL_SHEET_ID,
+    CASH_FLOW_SHEET_ID,
     BALANCE_SHEET_COLUMNS,
     PNL_SHEET_COLUMNS,
     CODAL_BASIC_INFO_COLUMNS,
+    CASH_FLOW_SHEET_COLUMNS,
 )
 from finops.logger import logger
 
 
 class Codal(Scraper, Preprocessor):
-    def __init__(self, search_params, driver_path="selenium/chromedriver"):
+    def __init__(self, store_path, driver_path="selenium/chromedriver"):
         self.driver = self._initialize_driver(driver_path)
-        self.search_params = search_params
+        self.balance_sheets_path = os.path.join(store_path, "balance_sheets.csv")
+        self.pnl_path = os.path.join(store_path, "pnl.csv")
+        self.cash_flow_path = os.path.join(store_path, "cash_flow.csv")
+        self.letters_list_path = os.path.join(store_path, "letters_list.csv")
 
     def _initialize_driver(self, driver_path):
         service = Service(driver_path)
         options = webdriver.ChromeOptions()
         options.add_argument("--disable-extensions")
         options.add_argument("--headless")
         options.add_argument("--no-sandbox")
@@ -42,46 +47,51 @@
         return driver
 
     def _create_search_url(self, **kwargs):
         url = CODAL_SEARCH_BASE_URL
         url += "&".join([f"{key}={value}" for key, value in kwargs.items()])
         return url
 
-    def _get_letters_list_pages_number(self):
-        search_url = self._create_search_url(**self.search_params)
+    def _get_letters_list_pages_number(self, search_params):
+        search_url = self._create_search_url(**search_params)
         response = self._download(search_url)
         parsed_response = self._parse_json_response(response)
         n_pages = parsed_response["Page"]
         return n_pages
 
     @sleep
     @retry(max_retries=3, wait_time=1)
-    def _scrap_letters_list_one_page(self, page_number):
-        search_params = self.search_params.copy()
+    def _scrap_letters_list_one_page(self, search_params, page_number):
         search_params["PageNumber"] = page_number
         search_url = self._create_search_url(**search_params)
         response = self._download(search_url)
         parsed_response = self._parse_json_response(response)
         letters_list_df = self._preprocess_letters_list(parsed_response)
         return letters_list_df
 
-    def _scrap_letters_list(self, store_path, stocks=None, verbose=True):
-        letters_list = self._load_or_create_csv(store_path, CODAL_LETTERS_LIST_COLUMNS)
+    def scrap_letters_list(
+        self, search_params, start_page_number=None, stocks=None, verbose=True
+    ):
+        letters_list = self._load_or_create_csv(
+            self.letters_list_path, CODAL_LETTERS_LIST_COLUMNS
+        )
         scraped_letters = self._get_scraped_ids(letters_list, "tracing_id")
-        n_pages = self._get_letters_list_pages_number()
-        for page_number in range(1, n_pages + 1):
-            letters_list_one_page = self._scrap_letters_list_one_page(page_number)
+        n_pages = self._get_letters_list_pages_number(search_params)
+        for page_number in range(start_page_number or 1, n_pages + 1):
+            letters_list_one_page = self._scrap_letters_list_one_page(
+                search_params, page_number
+            )
             if stocks is not None:
                 letters_list_one_page = letters_list_one_page[
                     letters_list_one_page.symbol.isin(stocks)
                 ]
             letters_list_one_page = letters_list_one_page[
                 ~letters_list_one_page.tracing_id.isin(scraped_letters)
             ]
-            self._save_csv(letters_list_one_page, store_path)
+            self._save_csv(letters_list_one_page, self.letters_list_path)
             time.sleep(1)
             if verbose:
                 logger.info(f"Page {page_number} of {n_pages} is scrapped.")
 
     @sleep
     @retry(max_retries=3, wait_time=1)
     def _scrap_letter(self, letter_url):
@@ -98,54 +108,62 @@
         letter = []
         for row in parsed_response.find_all("tr"):
             letter.append([cell.text for cell in row.find_all("td")])
         return pd.DataFrame(letter)
 
     def scrap_letters(
         self,
-        store_path,
-        stocks=None,
-        letters_list_path=None,
-        scrape_balance_sheets=True,
-        scrape_pnl_sheets=True,
+        is_scrap_balance_sheets=True,
+        is_scrap_pnl_sheets=True,
+        is_scrap_cash_flow=True,
     ):
-        balance_sheets_path = os.path.join(store_path, "balance_sheets.csv")
         balance_sheets = self._load_or_create_csv(
-            balance_sheets_path, BALANCE_SHEET_COLUMNS + CODAL_BASIC_INFO_COLUMNS
+            self.balance_sheets_path, BALANCE_SHEET_COLUMNS + CODAL_BASIC_INFO_COLUMNS
         )
-        pnl_path = os.path.join(store_path, "pnl.csv")
         pnl_sheets = self._load_or_create_csv(
-            pnl_path, PNL_SHEET_COLUMNS + CODAL_BASIC_INFO_COLUMNS
+            self.pnl_path, PNL_SHEET_COLUMNS + CODAL_BASIC_INFO_COLUMNS
         )
-        if letters_list_path is None:
-            letters_list_path = os.path.join(store_path, "letters_list.csv")
-            letters_list = self._scrap_letters_list(letters_list_path, stocks)
-        letters_list = self._load_or_create_csv(
-            letters_list_path, CODAL_LETTERS_LIST_COLUMNS
+        cash_flow_sheets = self._load_or_create_csv(
+            self.cash_flow_path, CASH_FLOW_SHEET_COLUMNS + CODAL_BASIC_INFO_COLUMNS
         )
+        letters_list = self._load_csv(self.letters_list_path)
         for index, row in letters_list.iterrows():
             try:
-                if scrape_balance_sheets:
+                if is_scrap_balance_sheets:
                     if row["tracing_id"] not in balance_sheets.tracing_id.values:
                         letter_df = self._preprocess_balance_sheet_df(
                             self._scrap_letter(
                                 row["url"] + f"&sheetId={BALANCE_SHEET_ID}"
                             )
                         )
                         self._add_basic_letter_info(letter_df, row)
-                        self._save_csv(letter_df, balance_sheets_path)
+                        self._save_csv(letter_df, self.balance_sheets_path)
 
             except Exception as e:
                 print(e)
                 print(row["url"] + f"&sheetId={BALANCE_SHEET_ID}")
 
             try:
-                if scrape_pnl_sheets:
+                if is_scrap_pnl_sheets:
                     if row["tracing_id"] not in pnl_sheets.tracing_id.values:
                         letter_df = self._preprocess_pnl_df(
                             self._scrap_letter(row["url"] + f"&sheetId={PNL_SHEET_ID}")
                         )
                         self._add_basic_letter_info(letter_df, row)
-                        self._save_csv(letter_df, pnl_path)
+                        self._save_csv(letter_df, self.pnl_path)
             except Exception as e:
                 print(e)
                 print(row["url"] + f"&sheetId={PNL_SHEET_ID}")
+
+            try:
+                if is_scrap_cash_flow:
+                    if row["tracing_id"] not in cash_flow_sheets.tracing_id.values:
+                        letter_df = self._preprocess_cash_flow_df(
+                            self._scrap_letter(
+                                row["url"] + f"&sheetId={CASH_FLOW_SHEET_ID}"
+                            )
+                        )
+                        self._add_basic_letter_info(letter_df, row)
+                        self._save_csv(letter_df, self.cash_flow_path)
+            except Exception as e:
+                print(e)
+                print(row["url"] + f"&sheetId={CASH_FLOW_SHEET_ID}")
```

### Comparing `finops-0.1.4/finops/config.py` & `finops-0.1.5/finops/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -55,19 +55,34 @@
     "جمع بدهی‌های جاری",
     "جمع بدهی‌های غیرجاری",
     "جمع بدهی‌ها",
     "جمع حقوق صاحبان سهام",
     "جمع بدهی‌ها و حقوق صاحبان سهام",
 ]
 
+CASH_FLOW_SHEET_COLUMNS = [
+    "جریان ‌خالص ‌ورود‌ (خروج) ‌نقد حاصل از فعالیت‌های ‌عملیاتی",
+    "جریان خالص ورود (خروج) نقد حاصل از فعالیت‌های سرمایه‌گذاری",
+    "جریان خالص ورود (خروج) نقد قبل از فعالیت‌های تامین مالی",
+    "جریان خالص ورود (خروج) نقد حاصل از فعالیت‌های تامین مالی",
+    "خالص افزایش (کاهش) در موجودی نقد",
+    "مانده موجودی نقد در ابتدای سال",
+    "مانده موجودی نقد در پایان سال",
+    "تاثیر تغییرات نرخ ارز",
+    "معاملات غیرنقدی",
+]
+
 CODAL_BASIC_INFO_COLUMNS = [
     "tracing_id",
     "symbol",
     "is_audited",
     "is_correction",
+    "is_consolidated",
+    "period_type",
+    "period_length",
     "period_end_date",
 ]
 LOG_COLUMNS = [
     "id",
     "date",
 ]
 
@@ -121,17 +136,29 @@
     "بهاى تمام شده درآمدهای عملیاتی": "جمع هزینه های عملیاتی",
     "سود(زیان) عملیاتى": "سود (زیان) عملیاتی",
     "سود(زیان) ناخالص": "سود (زیان) ناخالص",
     "سود(زیان) خالص عملیات در حال تداوم": "سود (زیان) خالص عملیات در حال تداوم",
     "سود(زیان) خالص": "سود (زیان) خالص",
     "سود(زیان) پایه هر سهم": "سود (زیان) پایه هر سهم",
     "سود هر سهم پس از کسر مالیات": "سود (زیان) خالص هر سهم – ریال",
-    "سود (زیان) خالص پس از کسر مالیات":  "سود (زیان) خالص",
+    "سود (زیان) خالص پس از کسر مالیات": "سود (زیان) خالص",
     "سود(زیان) عملیات در حال تداوم قبل از مالیات": "سود (زیان) قبل از کسر مالیات",
     "سود (زیان) عملیات در حال تداوم قبل از مالیات": "سود (زیان) قبل از کسر مالیات",
     "سود (زیان) قبل از مالیات": "سود (زیان) قبل از کسر مالیات",
     "سود (زیان) ناخالص فعالیتهای بیمه ای": "سود (زیان) ناخالص",
 }
 
+CASH_FLOW_FIX_MISTAKE_MAP = {
+    "جریان خالص ورود (خروج) وجه نقد ناشی از فعالیت‌های سرمایه‌گذاری": "جریان خالص ورود (خروج) نقد حاصل از فعالیت‌های سرمایه‌گذاری",
+    "جریان خالص ورود (خروج) وجه نقد ناشی از فعالیت‌های عملیاتی": "جریان ‌خالص ‌ورود‌ (خروج) ‌نقد حاصل از فعالیت‌های ‌عملیاتی",
+    "جریان خالص ورود (خروج) وجه نقد قبل از فعالیت‌های تامین مالی": "جریان خالص ورود (خروج) نقد قبل از فعالیت‌های تامین مالی",
+    "جریان خالص ورود (خروج) وجه نقد ناشی از فعالیت‌های تامین مالی": "جریان خالص ورود (خروج) نقد حاصل از فعالیت‌های تامین مالی",
+    "موجودی نقد در ابتدای دوره": "مانده موجودی نقد در ابتدای سال",
+    "تآثیر تغییرات نرخ ارز": "تاثیر تغییرات نرخ ارز",
+    "موجودی نقد در پایان دوره": "مانده موجودی نقد در پایان سال",
+    "مبادلات غیرنقدی": "معاملات غیرنقدی",
+}
+
 # CODAL CODES
 BALANCE_SHEET_ID = 0
 PNL_SHEET_ID = 1
+CASH_FLOW_SHEET_ID = 9
```

### Comparing `finops-0.1.4/finops/tehran_stock_exchange.py` & `finops-0.1.5/finops/tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/finops/ticker.py` & `finops-0.1.5/finops/ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/finops/utils/downloader.py` & `finops-0.1.5/finops/utils/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,18 @@
     @staticmethod
     def _parse_csv_response(response):
         return pd.read_csv(io.StringIO(response.content.decode("utf8")))
 
     @staticmethod
     def _parse_html_response(response):
         return BeautifulSoup(response.text, "html.parser")
+    
+    @staticmethod
+    def _load_csv(path, **kwargs):
+        return pd.read_csv(path, **kwargs)
 
     def _load_or_create_csv(self, path, columns, **kwargs):
         self._create_csv_file(path, columns=columns)
         return pd.read_csv(path, **kwargs)
 
     @staticmethod
     def _save_csv(data, path):
```

### Comparing `finops-0.1.4/finops/utils/preprocessor.py` & `finops-0.1.5/finops/utils/preprocessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,18 @@
     PRICE_HISTORY_DATA_COLUMNS,
     LOG_COLUMNS,
     USER_AGENT,
     PRICE_HISTORY_FIELD_MAP,
     SHAREHOLDER_FIELD_MAP,
     BALANCE_SHEET_COLUMNS,
     PNL_SHEET_COLUMNS,
+    CASH_FLOW_SHEET_COLUMNS,
     BALANCE_SHEET_FIX_MISTAKE_MAP,
     PNL_SHEET_FIX_MISTAKE_MAP,
+    CASH_FLOW_FIX_MISTAKE_MAP,
 )
 
 
 class Preprocessor:
     @staticmethod
     def _convert_isin_to_type(isin: str) -> str:
         """
@@ -40,15 +42,17 @@
         tickers = tickers_table.find_all("tr")
         tickers_data = []
         for ticker in tickers:
             cells = ticker.find_all("td")
             if cells:
                 ticker_url = cells[0].find("a")["href"]
                 data = {
-                    "name": self._preprocess_ticker_name(re.findall(r"\(([^()]+)\)", cells[0].text.strip())[0]),
+                    "name": self._preprocess_ticker_name(
+                        re.findall(r"\(([^()]+)\)", cells[0].text.strip())[0]
+                    ),
                     "full_name": cells[0].text.strip().split("(")[0],
                     "ticker_index": re.findall(r"(\d+)", ticker_url)[-1],
                     "instrument_isin": cells[1].text.strip(),
                     "en_name": cells[2].text.strip(),
                     "code": cells[3].text.strip(),
                     "company_isin": cells[4].text.strip(),
                     "market": cells[5].text.strip(),
@@ -79,22 +83,23 @@
         preprocessed_price_history = (
             parsed_response.rename(columns=PRICE_HISTORY_FIELD_MAP)
             .drop("per", axis=1)
             .assign(ticker_index=ticker_index)
             .assign(date=lambda df: pd.to_datetime(df["date"], format="%Y%m%d"))
         )
         return preprocessed_price_history
-    
+
     @staticmethod
     def _preprocess_persian_text(text):
         if text is None:
             return None
 
         text = text.replace("ي", "ی")
         text = text.replace("ك", "ک")
+        text = text.replace("أ", "ا")
 
         digits_mapping = {
             "۰": "0",
             "۱": "1",
             "۲": "2",
             "۳": "3",
             "۴": "4",
@@ -103,15 +108,15 @@
             "۷": "7",
             "۸": "8",
             "۹": "9",
         }
         for digit, replacement in digits_mapping.items():
             text = text.replace(digit, replacement)
         return text
-    
+
     def _preprocess_ticker_name(self, ticker_name):
         ticker_name = self._preprocess_persian_text(ticker_name)
         if ticker_name is None:
             return None
         ticker_name = ticker_name.replace("\u200c", "")
         return ticker_name
 
@@ -135,15 +140,15 @@
     @staticmethod
     def safe_select_columns(df, columns):
         selected_columns = []
         for column in columns:
             try:
                 selected_columns.append(df.loc[:, column])
             except KeyError:
-                selected_columns.append(pd.Series(dtype='object', name=column))
+                selected_columns.append(pd.Series(dtype="object", name=column))
         return pd.concat(selected_columns, axis=1)
 
     def _preprocess_balance_sheet_df(self, df):
         df = df.applymap(self._preprocess_codal_text)
         if len(df.columns) == 12:
             df = df.iloc[:, 1:3]
         if len(df.columns) == 10:
@@ -178,14 +183,28 @@
         df["title"] = df["title"].map(PNL_SHEET_FIX_MISTAKE_MAP).fillna(df["title"])
         df = df.drop_duplicates(subset=["title"], keep="first")
         df = df[df["title"].isin(PNL_SHEET_COLUMNS)]
         df = df.set_index("title").T.reset_index(drop=True)
         df = self.safe_select_columns(df, PNL_SHEET_COLUMNS)
         return df
 
+    def _preprocess_cash_flow_df(self, df):
+        df = df.applymap(self._preprocess_codal_text)
+        if len(df.columns) == 12:
+            df = df.iloc[:, 1:3]
+        df = df.iloc[:, :2]
+        df = df.dropna(how="any")
+        df.columns = ["title", "value"]
+        df["title"] = df["title"].map(CASH_FLOW_FIX_MISTAKE_MAP).fillna(df["title"])
+        df = df.drop_duplicates(subset=["title"], keep="first")
+        df = df[df["title"].isin(CASH_FLOW_SHEET_COLUMNS)]
+        df = df.set_index("title").T.reset_index(drop=True)
+        df = self.safe_select_columns(df, CASH_FLOW_SHEET_COLUMNS)
+        return df
+
     @staticmethod
     def _preprocess_letters_list(parsed_response):
         letters = parsed_response["Letters"]
         letters_list = []
         for letter in letters:
             letters_list.append(
                 {
@@ -200,14 +219,24 @@
 
     @staticmethod
     def _add_basic_letter_info(letter_df, info):
         letter_df["tracing_id"] = info["tracing_id"]
         letter_df["symbol"] = info["symbol"]
         letter_df["is_audited"] = "حسابرسی شده" in info["letter_title"]
         letter_df["is_correction"] = "اصلاحیه" in info["letter_title"]
+        letter_df["is_consolidated"] = "تلفیقی" in info["letter_title"]
+        letter_df["period_type"] = re.search(
+            r"(سال مالی|میاندوره‌ای)", info["letter_title"]
+        ).group()
+
+        letter_df["period_length"] = (
+            re.search(r"\d+(?= ماهه)", info["letter_title"]).group()
+            if re.search(r"\d+(?= ماهه)", info["letter_title"])
+            else None
+        )
         letter_df["period_end_date"] = (
             jdatetime.datetime.strptime(
                 re.search(r"\d{4}/\d{2}/\d{2}", info["letter_title"]).group(),
                 "%Y/%m/%d",
             )
             .date()
             .togregorian()
```

### Comparing `finops-0.1.4/finops/utils/scraper.py` & `finops-0.1.5/finops/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/finops/utils/wrappers.py` & `finops-0.1.5/finops/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/finops.egg-info/PKG-INFO` & `finops-0.1.5/finops.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.1.4/finops.egg-info/SOURCES.txt` & `finops-0.1.5/finops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/setup.py` & `finops-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='finops',
-    version='0.1.4',
+    version='0.1.5',
     description='A Python package for financial operations.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `finops-0.1.4/tests/test_tehran_stock_exchange.py` & `finops-0.1.5/tests/test_tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/tests/test_ticker.py` & `finops-0.1.5/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/tests/test_utils/test_downloader.py` & `finops-0.1.5/tests/test_utils/test_downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.4/tests/test_utils/test_scraper.py` & `finops-0.1.5/tests/test_utils/test_scraper.py`

 * *Files identical despite different names*

