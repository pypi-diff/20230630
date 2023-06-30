# Comparing `tmp/hydroloader-0.1.5.tar.gz` & `tmp/hydroloader-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydroloader-0.1.5.tar", last modified: Wed Jun 28 22:50:39 2023, max compression
+gzip compressed data, was "hydroloader-0.1.6.tar", last modified: Fri Jun 30 04:56:56 2023, max compression
```

## Comparing `hydroloader-0.1.5.tar` & `hydroloader-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-28 22:50:39.759535 hydroloader-0.1.5/
--rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-06-07 22:04:25.000000 hydroloader-0.1.5/LICENSE.txt
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-28 22:50:39.759585 hydroloader-0.1.5/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)        0 2023-06-07 22:04:25.000000 hydroloader-0.1.5/README.md
--rw-r--r--   0 klippold   (501) staff       (20)       80 2023-06-07 22:04:25.000000 hydroloader-0.1.5/pyproject.toml
--rw-r--r--   0 klippold   (501) staff       (20)      352 2023-06-28 22:50:39.759823 hydroloader-0.1.5/setup.cfg
--rw-r--r--   0 klippold   (501) staff       (20)       93 2023-06-07 22:04:25.000000 hydroloader-0.1.5/setup.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-28 22:50:39.757469 hydroloader-0.1.5/src/
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-28 22:50:39.758607 hydroloader-0.1.5/src/hydroloader/
--rw-r--r--   0 klippold   (501) staff       (20)      396 2023-06-26 22:58:34.000000 hydroloader-0.1.5/src/hydroloader/__init__.py
--rw-r--r--   0 klippold   (501) staff       (20)      314 2023-06-14 20:27:28.000000 hydroloader-0.1.5/src/hydroloader/exceptions.py
--rw-r--r--   0 klippold   (501) staff       (20)    15694 2023-06-28 22:36:11.000000 hydroloader-0.1.5/src/hydroloader/main.py
--rw-r--r--   0 klippold   (501) staff       (20)     7984 2023-06-28 22:35:17.000000 hydroloader-0.1.5/src/hydroloader/models.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-28 22:50:39.759413 hydroloader-0.1.5/src/hydroloader.egg-info/
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-28 22:50:39.000000 hydroloader-0.1.5/src/hydroloader.egg-info/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)      391 2023-06-28 22:50:39.000000 hydroloader-0.1.5/src/hydroloader.egg-info/SOURCES.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-28 22:50:39.000000 hydroloader-0.1.5/src/hydroloader.egg-info/dependency_links.txt
--rw-r--r--   0 klippold   (501) staff       (20)      101 2023-06-28 22:50:39.000000 hydroloader-0.1.5/src/hydroloader.egg-info/requires.txt
--rw-r--r--   0 klippold   (501) staff       (20)       12 2023-06-28 22:50:39.000000 hydroloader-0.1.5/src/hydroloader.egg-info/top_level.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-07 22:05:51.000000 hydroloader-0.1.5/src/hydroloader.egg-info/zip-safe
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-30 04:56:56.654976 hydroloader-0.1.6/
+-rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-06-07 22:04:25.000000 hydroloader-0.1.6/LICENSE.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-30 04:56:56.655042 hydroloader-0.1.6/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)        0 2023-06-07 22:04:25.000000 hydroloader-0.1.6/README.md
+-rw-r--r--   0 klippold   (501) staff       (20)       80 2023-06-07 22:04:25.000000 hydroloader-0.1.6/pyproject.toml
+-rw-r--r--   0 klippold   (501) staff       (20)      352 2023-06-30 04:56:56.655308 hydroloader-0.1.6/setup.cfg
+-rw-r--r--   0 klippold   (501) staff       (20)       93 2023-06-07 22:04:25.000000 hydroloader-0.1.6/setup.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-30 04:56:56.652407 hydroloader-0.1.6/src/
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-30 04:56:56.653893 hydroloader-0.1.6/src/hydroloader/
+-rw-r--r--   0 klippold   (501) staff       (20)      396 2023-06-26 22:58:34.000000 hydroloader-0.1.6/src/hydroloader/__init__.py
+-rw-r--r--   0 klippold   (501) staff       (20)      314 2023-06-14 20:27:28.000000 hydroloader-0.1.6/src/hydroloader/exceptions.py
+-rw-r--r--   0 klippold   (501) staff       (20)    15495 2023-06-30 04:55:39.000000 hydroloader-0.1.6/src/hydroloader/main.py
+-rw-r--r--   0 klippold   (501) staff       (20)     7984 2023-06-28 22:35:17.000000 hydroloader-0.1.6/src/hydroloader/models.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-30 04:56:56.654693 hydroloader-0.1.6/src/hydroloader.egg-info/
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-30 04:56:56.000000 hydroloader-0.1.6/src/hydroloader.egg-info/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)      391 2023-06-30 04:56:56.000000 hydroloader-0.1.6/src/hydroloader.egg-info/SOURCES.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-30 04:56:56.000000 hydroloader-0.1.6/src/hydroloader.egg-info/dependency_links.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      101 2023-06-30 04:56:56.000000 hydroloader-0.1.6/src/hydroloader.egg-info/requires.txt
+-rw-r--r--   0 klippold   (501) staff       (20)       12 2023-06-30 04:56:56.000000 hydroloader-0.1.6/src/hydroloader.egg-info/top_level.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-07 22:05:51.000000 hydroloader-0.1.6/src/hydroloader.egg-info/zip-safe
```

### Comparing `hydroloader-0.1.5/LICENSE.txt` & `hydroloader-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydroloader-0.1.5/src/hydroloader/main.py` & `hydroloader-0.1.6/src/hydroloader/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 class HydroLoader:
 
     client: requests.Session
     service: Union[AnyHttpUrl, str]
     conf: HydroLoaderConf
 
+    file_result_timestamp: Optional[datetime]
     datastreams: Dict[str, HydroLoaderDatastream]
     chunk_size: conint(gt=0) = 10000
 
     timestamp_column_index: Optional[conint(gt=0)]
     datastream_column_indexes: Dict[Union[str, int], int]
     observation_bodies: Dict[str, List[List[str]]]
 
@@ -128,64 +129,55 @@
             self.get_datastreams()
 
         if not self.conf.file_access.path:
             return
 
         with open(self.conf.file_access.path) as data_file:
             data_reader = csv.reader(data_file, delimiter=self.conf.file_access.delimiter)
+            file_parsing_error = False
             failed_datastreams = []
             for i, row in enumerate(data_reader):
                 try:
                     self.parse_data_file_row(i + 1, row)
                 except HeaderParsingError as e:
                     logger.error(
                         f'Failed to parse data file headers for "{self.conf.file_access.path}" ' +
                         f'with error: {str(e)}'
                     )
-                    raise ValueError from e
+                    file_parsing_error = True
+                    break
                 except TimestampParsingError as e:
                     logger.error(
                         f'Failed to parse timestamp on row {i + 1} for "{self.conf.file_access.path}" ' +
                         f'with error: {str(e)}'
                     )
-                    raise ValueError from e
+                    file_parsing_error = True
+                    break
                 if i > 0 and i % self.chunk_size == 0:
                     responses = self.post_observations(
                         skip_datastreams=failed_datastreams
                     )
                     failed_datastreams = self.handle_post_responses(
                         responses=responses,
                         failed_datastreams=failed_datastreams
                     )
-            responses = self.post_observations(
-                skip_datastreams=failed_datastreams
-            )
-            self.handle_post_responses(
-                responses=responses,
-                failed_datastreams=failed_datastreams
-            )
+            if not file_parsing_error:
+                responses = self.post_observations(
+                    skip_datastreams=failed_datastreams
+                )
+                self.handle_post_responses(
+                    responses=responses,
+                    failed_datastreams=failed_datastreams
+                )
 
         return {
-            'data_thru': self.get_data_thru_date(),
-            'success': len(failed_datastreams) == 0
+            'data_thru': self.file_result_timestamp,
+            'success': len(failed_datastreams) == 0 and file_parsing_error is False
         }
 
-    def get_data_thru_date(self):
-        """"""
-
-        data_thru_date = None
-
-        for datastream in self.datastreams.values():
-            if datastream.file_result_end_time and (
-                    data_thru_date is None or datastream.file_result_end_time > data_thru_date
-            ):
-                data_thru_date = datastream.file_result_end_time
-
-        return data_thru_date
-
     @staticmethod
     def handle_post_responses(responses, failed_datastreams):
         """
         The handle_post_responses function takes a list of responses from SensorThings observations POST requests and
         a list of datastreams that have failed to post observations. It iterates through each response,
         and if the status code is not 201 (created), it logs an error message with information about
         the request URL, chunk start time, chunk end time, status code and reason for failure. If the
@@ -314,21 +306,21 @@
 
         if timestamp.tzinfo is None:
             if not self.conf.file_timestamp.offset:
                 timestamp = timestamp.replace(
                     tzinfo=timezone.utc
                 )
 
+        self.file_result_timestamp = timestamp
+
         for datastream in [
             ds for ds in self.conf.datastreams if str(ds.datastream_id) in self.datastreams.keys()
         ]:
             ds_timestamp = self.datastreams[str(datastream.datastream_id)].result_time
 
-            self.datastreams[str(datastream.datastream_id)].file_result_end_time = timestamp
-
             if not self.datastreams[str(datastream.datastream_id)].file_row_start_index:
                 if ds_timestamp is None or timestamp > ds_timestamp:
                     self.datastreams[str(datastream.datastream_id)].file_row_start_index = index
 
             if self.datastreams[str(datastream.datastream_id)].file_row_start_index and \
                     self.datastreams[str(datastream.datastream_id)].file_row_start_index <= index:
                 if str(datastream.datastream_id) not in self.observation_bodies.keys():
```

### Comparing `hydroloader-0.1.5/src/hydroloader/models.py` & `hydroloader-0.1.6/src/hydroloader/models.py`

 * *Files identical despite different names*

