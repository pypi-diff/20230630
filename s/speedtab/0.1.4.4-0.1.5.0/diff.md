# Comparing `tmp/speedtab-0.1.4.4.tar.gz` & `tmp/speedtab-0.1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.4.4.tar", max compression
+gzip compressed data, was "speedtab-0.1.5.0.tar", max compression
```

## Comparing `speedtab-0.1.4.4.tar` & `speedtab-0.1.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-06-20 10:33:01.350911 speedtab-0.1.4.4/pyproject.toml
--rw-r--r--   0        0        0      365 2023-06-09 12:04:52.821400 speedtab-0.1.4.4/speedtab/__init__.py
--rw-r--r--   0        0        0    50278 2023-06-20 10:30:24.690346 speedtab-0.1.4.4/speedtab/client.py
--rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.4.4/speedtab/enums.py
--rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.4.4/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-06-20 10:33:07.196287 speedtab-0.1.4.4/setup.py
--rw-r--r--   0        0        0      808 2023-06-20 10:33:07.196287 speedtab-0.1.4.4/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-06-30 16:05:22.132158 speedtab-0.1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      365 2023-06-09 12:04:52.821400 speedtab-0.1.5.0/speedtab/__init__.py
+-rw-r--r--   0        0        0    50614 2023-06-30 16:03:40.365716 speedtab-0.1.5.0/speedtab/client.py
+-rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.5.0/speedtab/enums.py
+-rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.5.0/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-06-30 16:05:25.447351 speedtab-0.1.5.0/setup.py
+-rw-r--r--   0        0        0      808 2023-06-30 16:05:25.447351 speedtab-0.1.5.0/PKG-INFO
```

### Comparing `speedtab-0.1.4.4/pyproject.toml` & `speedtab-0.1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.4.4"
+version = "0.1.5.0"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.4.4/speedtab/client.py` & `speedtab-0.1.5.0/speedtab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,14 @@
         self.base = base
         self.data_cell = data_cell
 
     def _increment_task(self):
         return len(self._task_queue)
 
     def add_combo_chart(self,
-                        data_start,
                         left_columns,
                         right_columns,
                         chart_type_left: ChartType = ChartType.COLUMN,
                         chart_type_right: ChartType = ChartType.LINE,
                         index_column: int = 0,
                         stacked_type: StackedType = StackedType.NONE,
                         title: str = None,
@@ -394,17 +393,18 @@
                         y_axis_min_right: float = None,
                         y_axis_max_left: float = None,
                         y_axis_max_right: float = None,
                         x_scale: int = 1,
                         y_scale: int = 1,
                         offset_x_pixels: int = 0,
                         offset_y_pixels: int = 0,
-                        data_sheet_name=None,
                         header_count: int = 1,
-                        nrows: int = None
+                        nrows: int = None,
+                        data_sheet_name=None,
+                        data_start=(0, 0)
                         ):
 
         data_start_cell = parse_range(data_start)
         series = [{
             'series': {
                 'sourceRange': {
                     'sources': [
@@ -503,15 +503,16 @@
                             'offsetYPixels': offset_y_pixels,
                             'widthPixels': 800 * x_scale,
                             'heightPixels': 400 * y_scale,
                         }
                     }}}}, self.work_zone))
         return self
 
-    def add_chart(self, columns,
+    def add_chart(self,
+                  columns,
                   target_axis: AxisPosition = AxisPosition.LEFT_AXIS,
                   index_column: int = 0,
                   chart_type: ChartType = ChartType.LINE,
                   stacked_type: StackedType = StackedType.NONE,
                   title: str = None,
                   legend_position: LegendPosition = LegendPosition.BOTTOM_LEGEND,
                   x_axis_name: str = None,
@@ -522,17 +523,18 @@
                   y_left_axis_max: float = None,
                   y_right_axis_max: float = None,
                   x_scale: int = 1,
                   y_scale: int = 1,
                   offset_x_pixels: int = 0,
                   offset_y_pixels: int = 0,
                   header_count: int = 1,
-                  data_start: tuple = (0, 0),
                   nrows: int = None,
-                  data_sheet_name=None,):
+                  data_sheet_name=None,
+                  data_start=(0, 0)
+                  ):
 
         data_start_cell = parse_range(data_start)
         target_axis = [target_axis] if not isinstance(target_axis, (list, tuple)) else target_axis
 
         if len(columns) < len(target_axis):
             raise ValueError('Amount of target_axis must be lower than amount of columns in chart')
 
@@ -1014,15 +1016,21 @@
                                                 for sheet_name, grid in zip(sheets, hide_grid_lines)]})
                          .execute().get('spreadsheetId'), token_path=self.token_path,
                          credentials=self.credentials, connect_v4=self.connect_v4, connect_v3=self.connect_v3)
         self.list_of_spreadsheets.append(ss)
         return ss
 
     def create_copy_of_spreadsheet(self, file_id: str, new_title: str):
-        return self.connect_v3.files().copy(fileId=file_id, body={'name': new_title}, supportsAllDrives=True).execute()
+        ss = SpreedSheet(self.connect_v3.files().copy(fileId=file_id, body={'name': new_title}, supportsAllDrives=True).execute()['id'],
+                         token_path=self.token_path,
+                         credentials=self.credentials,
+                         connect_v4=self.connect_v4,
+                         connect_v3=self.connect_v3)
+        self.list_of_spreadsheets.append(ss)
+        return ss
 
     def create_folder(self, folder_name: str, parent_id: str = None):
         return self.connect_v3.files().create(body={
             'name': folder_name,
             'mimeType': "application/vnd.google-apps.folder",
             'parents': [parent_id] if parent_id else None,
         }, supportsAllDrives=True).execute()['id']
```

### Comparing `speedtab-0.1.4.4/speedtab/enums.py` & `speedtab-0.1.5.0/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.4.4/speedtab/formats.py` & `speedtab-0.1.5.0/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.4.4/setup.py` & `speedtab-0.1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.4.4',
+    'version': '0.1.5.0',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.4.4/PKG-INFO` & `speedtab-0.1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.4.4
+Version: 0.1.5.0
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

