# Comparing `tmp/drive-0.4.2.tar.gz` & `tmp/drive-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive-0.4.2.tar", max compression
+gzip compressed data, was "drive-0.4.3.tar", max compression
```

## Comparing `drive-0.4.2.tar` & `drive-0.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-06-26 14:40:38.276769 drive-0.4.2/LICENSE
--rw-r--r--   0        0        0     4045 2023-06-26 14:40:38.276769 drive-0.4.2/README.md
--rw-r--r--   0        0        0      128 2023-06-26 14:40:38.276769 drive-0.4.2/drive/__init__.py
--rw-r--r--   0        0        0     1363 2023-06-26 14:40:38.276769 drive-0.4.2/drive/auth.py
--rw-r--r--   0        0        0    17433 2023-06-26 14:40:38.276769 drive-0.4.2/drive/client.py
--rw-r--r--   0        0        0      124 2023-06-26 14:40:38.276769 drive-0.4.2/drive/exceptions.py
--rw-r--r--   0        0        0     9546 2023-06-26 14:40:38.276769 drive-0.4.2/drive/files.py
--rw-r--r--   0        0        0     1076 2023-06-26 14:40:38.276769 drive-0.4.2/drive/mimetypes.py
--rw-r--r--   0        0        0        0 2023-06-26 14:40:38.276769 drive-0.4.2/drive/py.typed
--rw-r--r--   0        0        0     1459 2023-06-26 14:40:38.276769 drive-0.4.2/drive/sheets.py
--rw-r--r--   0        0        0     1111 2023-06-26 14:40:38.276769 drive-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4885 1970-01-01 00:00:00.000000 drive-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-29 15:18:00.276063 drive-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4045 2023-06-29 15:18:00.276063 drive-0.4.3/README.md
+-rw-r--r--   0        0        0      128 2023-06-29 15:18:00.276063 drive-0.4.3/drive/__init__.py
+-rw-r--r--   0        0        0     1363 2023-06-29 15:18:00.276063 drive-0.4.3/drive/auth.py
+-rw-r--r--   0        0        0    17433 2023-06-29 15:18:00.276063 drive-0.4.3/drive/client.py
+-rw-r--r--   0        0        0      124 2023-06-29 15:18:00.276063 drive-0.4.3/drive/exceptions.py
+-rw-r--r--   0        0        0     9546 2023-06-29 15:18:00.276063 drive-0.4.3/drive/files.py
+-rw-r--r--   0        0        0     1076 2023-06-29 15:18:00.276063 drive-0.4.3/drive/mimetypes.py
+-rw-r--r--   0        0        0        0 2023-06-29 15:18:00.276063 drive-0.4.3/drive/py.typed
+-rw-r--r--   0        0        0     1532 2023-06-29 15:18:00.276063 drive-0.4.3/drive/sheets.py
+-rw-r--r--   0        0        0     1111 2023-06-29 15:18:00.276063 drive-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4885 1970-01-01 00:00:00.000000 drive-0.4.3/PKG-INFO
```

### Comparing `drive-0.4.2/LICENSE` & `drive-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drive-0.4.2/README.md` & `drive-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `drive-0.4.2/drive/auth.py` & `drive-0.4.3/drive/auth.py`

 * *Files identical despite different names*

### Comparing `drive-0.4.2/drive/client.py` & `drive-0.4.3/drive/client.py`

 * *Files identical despite different names*

### Comparing `drive-0.4.2/drive/files.py` & `drive-0.4.3/drive/files.py`

 * *Files identical despite different names*

### Comparing `drive-0.4.2/drive/mimetypes.py` & `drive-0.4.3/drive/mimetypes.py`

 * *Files identical despite different names*

### Comparing `drive-0.4.2/drive/sheets.py` & `drive-0.4.3/drive/sheets.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,31 +5,34 @@
 
 from .auth import authorize_credentials
 
 __all__ = ['SheetClient']
 
 
 class SheetClient:
-    """Experimental Google Sheets client."""
+    """Google Sheets client."""
 
     def __init__(self, credentials_path: Optional[str] = None):
         http = authorize_credentials(credentials_path)
         service = discovery.build('sheets', 'v4', http=http)
         self.service = service.spreadsheets()
 
     def get_sheet_range(self, sheet_id: str, sheet_tab: str, cell_range: str):
         req = self.service.values().get(spreadsheetId=sheet_id, range=f"{sheet_tab}!{cell_range}")
         # Note this often raises errors 500 or 503
         resp = req.execute()
         return resp["values"]
 
     def iter_sheet_lines(self, sheet_id: str, sheet_tab: str, column_start: str, column_end: str,
-                         *, batch_size=400, sleep=0.5) \
+                         *,
+                         offset=0,
+                         batch_size=400,
+                         sleep=0.5) \
             -> Iterable[list]:
-        offset = 1  # lines start at 1
+        offset += 1  # lines start at 1
         while True:
             cell_range = f"{column_start}{offset}:{column_end}{offset + batch_size}"
             lines = self.get_sheet_range(sheet_id, sheet_tab, cell_range)
             yield from lines
             if len(lines) < batch_size:
                 break
             offset += batch_size
```

### Comparing `drive-0.4.2/pyproject.toml` & `drive-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drive"
-version = "0.4.2"
+version = "0.4.3"
 description = "Google Drive client"
 authors = ["Baptiste Fontaine <b@ptistefontaine.fr>"]
 license = "MIT"
 include = ["drive/py.typed"]
 readme = "README.md"
 packages = [
     { include = "drive" },
```

### Comparing `drive-0.4.2/PKG-INFO` & `drive-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drive
-Version: 0.4.2
+Version: 0.4.3
 Summary: Google Drive client
 License: MIT
 Author: Baptiste Fontaine
 Author-email: b@ptistefontaine.fr
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

