# Comparing `tmp/jquants_api_client-1.3.1.tar.gz` & `tmp/jquants_api_client-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jquants_api_client-1.3.1.tar", max compression
+gzip compressed data, was "jquants_api_client-1.4.0.tar", max compression
```

## Comparing `jquants_api_client-1.3.1.tar` & `jquants_api_client-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-06-29 05:37:48.971960 jquants_api_client-1.3.1/LICENSE
--rw-r--r--   0        0        0     5631 2023-06-29 05:37:48.971960 jquants_api_client-1.3.1/README.md
--rw-r--r--   0        0        0       66 2023-06-29 05:37:48.971960 jquants_api_client-1.3.1/jquantsapi/__init__.py
--rw-r--r--   0        0        0    56237 2023-06-29 05:37:48.975960 jquants_api_client-1.3.1/jquantsapi/client.py
--rw-r--r--   0        0        0    15449 2023-06-29 05:37:48.975960 jquants_api_client-1.3.1/jquantsapi/constants.py
--rw-r--r--   0        0        0      517 2023-06-29 05:37:48.975960 jquants_api_client-1.3.1/jquantsapi/enums.py
--rw-r--r--   0        0        0     1676 2023-06-29 05:38:06.759838 jquants_api_client-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     7093 1970-01-01 00:00:00.000000 jquants_api_client-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-30 06:02:17.365636 jquants_api_client-1.4.0/LICENSE
+-rw-r--r--   0        0        0     5631 2023-06-30 06:02:17.365636 jquants_api_client-1.4.0/README.md
+-rw-r--r--   0        0        0       66 2023-06-30 06:02:17.369636 jquants_api_client-1.4.0/jquantsapi/__init__.py
+-rw-r--r--   0        0        0    56414 2023-06-30 06:02:17.369636 jquants_api_client-1.4.0/jquantsapi/client.py
+-rw-r--r--   0        0        0    15725 2023-06-30 06:02:17.369636 jquants_api_client-1.4.0/jquantsapi/constants.py
+-rw-r--r--   0        0        0      517 2023-06-30 06:02:17.369636 jquants_api_client-1.4.0/jquantsapi/enums.py
+-rw-r--r--   0        0        0     1676 2023-06-30 06:02:33.925714 jquants_api_client-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7093 1970-01-01 00:00:00.000000 jquants_api_client-1.4.0/PKG-INFO
```

### Comparing `jquants_api_client-1.3.1/LICENSE` & `jquants_api_client-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.3.1/README.md` & `jquants_api_client-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.3.1/jquantsapi/client.py` & `jquants_api_client-1.4.0/jquantsapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,19 @@
                 date_yyyymmdd=date_yyyymmdd,
                 pagination_key=d["pagination_key"],
             )
             d = json.loads(j)
             data += d["info"]
         df = pd.DataFrame.from_dict(data)
 
-        cols = constants.LISTED_INFO_COLUMNS
+        standard_premium_flag = "MarginCode" in df.columns
+        if standard_premium_flag:
+            cols = constants.LISTED_INFO_STANDARD_PREMIUM_COLUMNS
+        else:
+            cols = constants.LISTED_INFO_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values("Code", inplace=True)
         return df[cols]
 
     @staticmethod
```

### Comparing `jquants_api_client-1.3.1/jquantsapi/constants.py` & `jquants_api_client-1.4.0/jquantsapi/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,29 @@
     "Sector33Code",
     "Sector33CodeName",
     "ScaleCategory",
     "MarketCode",
     "MarketCodeName",
 ]
 
+LISTED_INFO_STANDARD_PREMIUM_COLUMNS = [
+    "Date",
+    "Code",
+    "CompanyName",
+    "Sector17Code",
+    "Sector17CodeName",
+    "Sector33Code",
+    "Sector33CodeName",
+    "ScaleCategory",
+    "MarketCode",
+    "MarketCodeName",
+    "MarginCode",
+    "MarginCodeName",
+]
+
 # ref. ja https://jpx.gitbook.io/j-quants-ja/api-reference/listed_info/sector17code
 # ref. en https://jpx.gitbook.io/j-quants-en/api-reference/listed_info/sector17code
 SECTOR_17_COLUMNS = ["Sector17Code", "Sector17CodeName", "Sector17CodeNameEnglish"]
 SECTOR_17_DATA = [
     ("1", "食品", "FOODS"),
     ("2", "エネルギー資源", "ENERGY RESOURCES"),
     ("3", "建設・資材", "CONSTRUCTION & MATERIALS"),
```

### Comparing `jquants_api_client-1.3.1/jquantsapi/enums.py` & `jquants_api_client-1.4.0/jquantsapi/enums.py`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.3.1/pyproject.toml` & `jquants_api_client-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jquants-api-client"
-version = "1.3.1" # use poetry-dynamic-versioning
+version = "1.4.0" # use poetry-dynamic-versioning
 authors = [
     "J-Quants Project Contributors <j-quants@jpx.co.jp>",
 ]
 description = "J-Quants API Client Library"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `jquants_api_client-1.3.1/PKG-INFO` & `jquants_api_client-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jquants-api-client
-Version: 1.3.1
+Version: 1.4.0
 Summary: J-Quants API Client Library
 Home-page: https://github.com/J-Quants/jquants-api-client-python
 License: Apache-2.0
 Keywords: jquants,api,client,J-Quants
 Author: J-Quants Project Contributors
 Author-email: j-quants@jpx.co.jp
 Requires-Python: >=3.7.1,<4.0.0
```

