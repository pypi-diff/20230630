# Comparing `tmp/com.castsoftware.uc.python.common-1.0.8.tar.gz` & `tmp/com.castsoftware.uc.python.common-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-1.0.8.tar", last modified: Tue Jun 20 20:52:47 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-1.0.9.tar", last modified: Thu Jun 22 13:15:23 2023, max compression
```

## Comparing `com.castsoftware.uc.python.common-1.0.8.tar` & `com.castsoftware.uc.python.common-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 20:52:47.945505 com.castsoftware.uc.python.common-1.0.8/
--rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      714 2023-06-20 20:52:47.938477 com.castsoftware.uc.python.common-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 20:52:47.857826 com.castsoftware.uc.python.common-1.0.8/cast_common/
--rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    13723 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0     4469 2023-06-19 13:01:19.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/greenIt.py
--rw-rw-rw-   0        0        0     9980 2023-06-20 20:44:31.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/highlight.py
--rw-rw-rw-   0        0        0     5625 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1778 2023-06-14 17:36:16.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/logger.py
--rw-rw-rw-   0        0        0    13409 2023-06-19 13:18:16.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/powerpoint.py
--rw-rw-rw-   0        0        0     5457 2023-06-20 20:37:23.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     7380 2023-06-14 13:23:51.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:52:47.915660 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      714 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      643 2023-06-12 16:21:04.000000 com.castsoftware.uc.python.common-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 20:52:47.945505 com.castsoftware.uc.python.common-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 20:52:47.925268 com.castsoftware.uc.python.common-1.0.8/test/
--rw-rw-rw-   0        0        0      494 2023-06-12 17:37:07.000000 com.castsoftware.uc.python.common-1.0.8/test/TestMultiInstance.py
+drwxrwxrwx   0        0        0        0 2023-06-22 13:15:23.157626 com.castsoftware.uc.python.common-1.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      714 2023-06-22 13:15:23.147721 com.castsoftware.uc.python.common-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 13:15:23.035275 com.castsoftware.uc.python.common-1.0.9/cast_common/
+-rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.9/cast_common/abstractClass.py
+-rw-rw-rw-   0        0        0    13723 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.9/cast_common/aipRestCall.py
+-rw-rw-rw-   0        0        0     4549 2023-06-20 22:05:23.000000 com.castsoftware.uc.python.common-1.0.9/cast_common/greenIt.py
+-rw-rw-rw-   0        0        0     9980 2023-06-20 20:44:31.000000 com.castsoftware.uc.python.common-1.0.9/cast_common/highlight.py
+-rw-rw-rw-   0        0        0     5625 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.9/cast_common/hlRestCall.py
+-rw-rw-rw-   0        0        0     1778 2023-06-14 17:36:16.000000 com.castsoftware.uc.python.common-1.0.9/cast_common/logger.py
+-rw-rw-rw-   0        0        0    14042 2023-06-20 21:59:01.000000 com.castsoftware.uc.python.common-1.0.9/cast_common/powerpoint.py
+-rw-rw-rw-   0        0        0     5612 2023-06-22 13:12:21.000000 com.castsoftware.uc.python.common-1.0.9/cast_common/restAPI.py
+-rw-rw-rw-   0        0        0     7054 2023-06-22 13:06:20.000000 com.castsoftware.uc.python.common-1.0.9/cast_common/util.py
+drwxrwxrwx   0        0        0        0 2023-06-22 13:15:23.096323 com.castsoftware.uc.python.common-1.0.9/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-06-22 13:15:22.000000 com.castsoftware.uc.python.common-1.0.9/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2023-06-22 13:15:22.000000 com.castsoftware.uc.python.common-1.0.9/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 13:15:22.000000 com.castsoftware.uc.python.common-1.0.9/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-22 13:15:22.000000 com.castsoftware.uc.python.common-1.0.9/com.castsoftware.uc.python.common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-22 13:15:22.000000 com.castsoftware.uc.python.common-1.0.9/com.castsoftware.uc.python.common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      643 2023-06-22 13:08:32.000000 com.castsoftware.uc.python.common-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 13:15:23.157626 com.castsoftware.uc.python.common-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 13:15:23.108770 com.castsoftware.uc.python.common-1.0.9/test/
+-rw-rw-rw-   0        0        0      494 2023-06-12 17:37:07.000000 com.castsoftware.uc.python.common-1.0.9/test/TestMultiInstance.py
```

### Comparing `com.castsoftware.uc.python.common-1.0.8/LICENSE` & `com.castsoftware.uc.python.common-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.8/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.8
+Version: 1.0.9
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.8/cast_common/abstractClass.py` & `com.castsoftware.uc.python.common-1.0.9/cast_common/abstractClass.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.8/cast_common/aipRestCall.py` & `com.castsoftware.uc.python.common-1.0.9/cast_common/aipRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.8/cast_common/greenIt.py` & `com.castsoftware.uc.python.common-1.0.9/cast_common/greenIt.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
             detail.sort_values(by=['Occurrences'],ascending=False,inplace=True)
             detail['Contribution'] = detail['Contribution'].apply(lambda x: '{0:.2f}%'.format(x).rjust(10))
             detail['Occurrences'] = detail['Occurrences'].apply(lambda x: '{0:.0f}'.format(x).rjust(10))
             hl.create_excel(app,detail)
 
             #detail = detail.astype({'Contribution':'string'})
             #detail['Contribution'] = detail['Contribution'].str.ljust(20)
-            prs.update_table('greenDetailTable',detail,include_index=False,max_rows=8)
+            prs.update_table('app1GreenDetailTable',detail,include_index=False,max_rows=8)
+            prs.update_chart('app1GreenTechPieChart',detail['Technology'])
         except Exception as ex:
             self.log.error(ex)
             status = False
 
         return status
 
     def get_green_indexes(self,app_name:str) -> Series:
```

### Comparing `com.castsoftware.uc.python.common-1.0.8/cast_common/highlight.py` & `com.castsoftware.uc.python.common-1.0.9/cast_common/highlight.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.8/cast_common/hlRestCall.py` & `com.castsoftware.uc.python.common-1.0.9/cast_common/hlRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.8/cast_common/logger.py` & `com.castsoftware.uc.python.common-1.0.9/cast_common/logger.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.8/cast_common/powerpoint.py` & `com.castsoftware.uc.python.common-1.0.9/cast_common/powerpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pptx import Presentation
 from pptx.parts.chart import ChartPart
+from pptx.chart.data import CategoryChartData
 from pptx.parts.embeddedpackage import EmbeddedXlsxPart
 from pptx.table import _Cell,Table, _Row, _Column
 from pptx.dml.color import RGBColor
 from pptx.oxml.xmlchemy import OxmlElement
 
 from cast_common.logger import Logger, INFO,DEBUG
 from os.path import abspath,exists
@@ -125,14 +126,30 @@
         if len(paragraph.runs) > 0:   
             run = paragraph.runs[0]
             run.text = cur_text
         else: 
             run = paragraph.add_run()
         return run
 
+    def update_chart(self, name,df):
+        shape = self.get_shape_by_name(name)
+        if shape != None:
+            titles = list(df.index.values)
+            data = df.to_numpy()
+            for i in range(0,len(data)):
+                if (isinstance(data[i],str)):
+                    data[i] = int(data[i].replace(',',''))
+
+            if shape.has_chart:
+                chart_data = CategoryChartData()
+                chart_data.categories = titles
+                chart_data.add_series('Series 1', data)
+                shape.chart.replace_data(chart_data)
+
+
     """ ***********************************************************************************************************
                                                 Update Table Functionality
     *********************************************************************************************************** """
     def update_table(self, name, df:DataFrame, include_index=True, 
                      background=None, forground=None,neg_num_bkg:list=None, 
                      has_header=True,max_rows=-1):
         table_shape = self.get_shape_by_name(name)
```

### Comparing `com.castsoftware.uc.python.common-1.0.8/cast_common/restAPI.py` & `com.castsoftware.uc.python.common-1.0.9/cast_common/restAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,36 +21,41 @@
 class RestCall(Logger):
 
     _base_url = None
     _auth = None
     _time_tracker_df  = DataFrame()
     _track_time = True
 
-    def __init__(self, base_url, user=None, password=None, track_time=False,log_level=INFO):
+    def __init__(self, base_url, user=None, password=None, basic_auth=None, track_time=False,log_level=INFO):
         super().__init__(level=log_level)
         if base_url[-1]=='/': 
             base_url=base_url[:-1]
         self._base_url = base_url
         self._track_time = track_time
 
         self._session = Session()
         self._max_retries = 5
 
         self._adapter = HTTPAdapter(
                 max_retries = Retry(
                     total = self._max_retries,
                     backoff_factor = 1,
                     status_forcelist = [408, 500, 502, 503, 504],
+#                    status_forcelist = [408],
                 )
         )
 
         self._session.mount('http://', self._adapter)
         self._session.mount('https://', self._adapter)
 
-        self._auth = HTTPBasicAuth(user, password)
+        if basic_auth is None:
+            self._auth = HTTPBasicAuth(user, password)
+        else:
+            self._auth = basic_auth
+
         self._session.headers.update({'Accept': 'application/json'})
         #self._session.headers.update({'Authorization': self._auth})
 
 
 #    def get(self, url = "", headers = {'Accept': 'application/json'}):
     def get(self, url = "",header=None):
         start_dttm = ctime()
```

### Comparing `com.castsoftware.uc.python.common-1.0.8/cast_common/util.py` & `com.castsoftware.uc.python.common-1.0.9/cast_common/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,31 +205,22 @@
     table_options={
                 'total_row':total_line,
                 'columns':columns,
                 'header_row':True,
                 'autofilter':True,
                 'banded_rows':True
                 }
-
     worksheet.add_table(0, 0, rows, cols,table_options)
-    
-    header_format = workbook.add_format({'text_wrap':True,
-                                        'align': 'center'})
 
     col_width = 10
     if width == None:
         width = []
         for i in range(1,len(data.columns)+1):
            width.append(col_width)
 
-    for col_num, value in enumerate(data.columns.values):
-        worksheet.write(0, col_num, value, header_format)
-        w=width[col_num]
-        worksheet.set_column(col_num, col_num, w)
-
     return worksheet
 
 
 def convert_LOC(total:int):
     unit = ''
     if 1000 <= total <= 1000000:
         unit = 'KLoc'
```

### Comparing `com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.9/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.8
+Version: 1.0.9
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/SOURCES.txt` & `com.castsoftware.uc.python.common-1.0.9/com.castsoftware.uc.python.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.8/pyproject.toml` & `com.castsoftware.uc.python.common-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='1.0.8' #prod version
+version='1.0.9' #prod version
 
 dependencies = ['pandas','requests','XlsxWriter']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

