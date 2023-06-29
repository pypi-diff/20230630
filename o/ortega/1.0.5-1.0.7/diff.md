# Comparing `tmp/ortega-1.0.5.tar.gz` & `tmp/ortega-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortega-1.0.5.tar", last modified: Thu Jun 29 17:25:11 2023, max compression
+gzip compressed data, was "ortega-1.0.7.tar", last modified: Thu Jun 29 23:27:56 2023, max compression
```

## Comparing `ortega-1.0.5.tar` & `ortega-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:25:11.406441 ortega-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 17:24:56.000000 ortega-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 17:25:11.406441 ortega-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-29 17:24:56.000000 ortega-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:25:11.406441 ortega-1.0.5/ortega/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/STPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (123)    27324 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/ortega.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:25:11.406441 ortega-1.0.5/ortega.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:25:11.406441 ortega-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 17:24:56.000000 ortega-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:27:56.347926 ortega-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 23:27:41.000000 ortega-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 23:27:56.347926 ortega-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-29 23:27:41.000000 ortega-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:27:56.347926 ortega-1.0.7/ortega/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/STPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27623 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/ortega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:27:56.347926 ortega-1.0.7/ortega.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 23:27:56.347926 ortega-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 23:27:41.000000 ortega-1.0.7/setup.py
```

### Comparing `ortega-1.0.5/LICENSE` & `ortega-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ortega-1.0.5/README.md` & `ortega-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ortega-1.0.5/ortega/STPoint.py` & `ortega-1.0.7/ortega/STPoint.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.5/ortega/ellipses.py` & `ortega-1.0.7/ortega/ellipses.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.5/ortega/ortega.py` & `ortega-1.0.7/ortega/ortega.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime as datetime
 from .ellipses import Ellipse, EllipseList
 from pandas.api.types import is_datetime64_dtype
 from typing import List, Tuple
 from .common import __timedifcheck
 from .common import *
-
+from .output import *
 
 def __check_spatial_intersect(item: Ellipse, others: Ellipse) -> bool:
     """
     test
     :param item:
     :param others:
     :return:
@@ -16,24 +16,24 @@
     return (
             item.el.intersects(others.el)
             or item.geom.within(others.geom)
             or others.geom.within(item.geom)
     )
 
 
-def get_time_difference(
-        ellipses_list_id1: List[Ellipse], ellipses_list_id2: List[Ellipse]):
-    time_diff = []
-    for count, item in enumerate(ellipses_list_id1, 1):
-        # spatial intersect
-        sub_ellipses_list = []
-        for item2 in ellipses_list_id2:
-            if __check_spatial_intersect(item, item2):
-                time_diff.append(__timedifcheck(item.t1, item2.t1))
-    return time_diff
+# def get_time_difference(
+#         ellipses_list_id1: List[Ellipse], ellipses_list_id2: List[Ellipse]):
+#     time_diff = []
+#     for count, item in enumerate(ellipses_list_id1, 1):
+#         # spatial intersect
+#         sub_ellipses_list = []
+#         for item2 in ellipses_list_id2:
+#             if __check_spatial_intersect(item, item2):
+#                 time_diff.append(__timedifcheck(item.t1, item2.t1))
+#     return time_diff
 
 
 def get_spatial_intersect_pairs(
         ellipses_list_id1: List[Ellipse], ellipses_list_id2: List[Ellipse],
         ) -> List[Tuple[Ellipse, Ellipse]]:
     intersection_pairs = []
     for count, item in enumerate(ellipses_list_id1, 1):
@@ -302,27 +302,26 @@
     #     return x
 
     df['diff_direction'] = df['P2_direction'] - df['P1_direction']
     df['diff_direction'] = df['diff_direction'].apply(math.cos)
     return df
 
 
-def interaction_compute_time_diff(df:pd.DataFrame):
+def interaction_compute_time_diff(df: pd.DataFrame):
     df['diff_time'] = (df['P2_t_start'] - df['P1_t_start'])/ pd.Timedelta(minutes=1)
     return df
 
 
 class ORTEGA:
     # ORTEGA is the main class for interaction analysis, users need to initialize this object at the very beginning
     def __init__(
             self,
             data: pd.DataFrame,  # movement data of two entities
-            # minute_delay: float,  # allowable delay for intersecting PPAs, in minute
-            minute_min_delay: float = 0,
-            minute_max_delay: float = 0,
+            minute_min_delay: float = 0,  # allowable minimum delay for intersecting PPAs, in minute
+            minute_max_delay: float = 0,  # allowable maximum delay for intersecting PPAs, in minute
             start_time: str = None,  # use this when users want to select a segment of movement data
             end_time: str = None,  # use this when users want to select a segment of movement data
             max_el_time_min: float = 10000,  # PPA's interval greater than this value will be eliminated, in minute
             latitude_field: str = "latitude",  # specify the latitude field name
             longitude_field: str = "longitude",  # specify the longitude field name
             id_field: str = "pid",  # specify the id field name
             time_field: str = "time_local",  # time_field must include month, day, year, hour, minute, second
@@ -332,35 +331,46 @@
         self.data = data
         self.start_time = start_time
         self.end_time = end_time
         self.latitude_field = latitude_field
         self.longitude_field = longitude_field
         self.id_field = id_field
         self.time_field = time_field
-        # self.minute_delay = minute_delay
         self.minute_min_delay = minute_min_delay
         self.minute_max_delay = minute_max_delay
         self.max_el_time_min = max_el_time_min
         self.speed_average = speed_average
         # self.kernel = kernel
         self.__validate()
         self.__start()
-    '''
+
+    @property
+    def minute_min_delay(self):
+        return self._minute_min_delay
+
+    @minute_min_delay.setter
+    def minute_min_delay(self, value):
+        if not isinstance(value, float) and not isinstance(value, int):
+            raise TypeError("Parameter 'minute_min_delay' must be numeric!")
+        if value < 0:
+            raise ValueError("Parameter 'minute_min_delay' must be greater than zero!")
+        self._minute_min_delay = value
+
     @property
-    def minute_delay(self):
-        return self._minute_delay
+    def minute_max_delay(self):
+        return self._minute_max_delay
 
-    @minute_delay.setter
-    def minute_delay(self, value):
+    @minute_max_delay.setter
+    def minute_max_delay(self, value):
         if not isinstance(value, float) and not isinstance(value, int):
-            raise TypeError("Parameter 'minute_delay' must be numeric!")
+            raise TypeError("Parameter 'minute_max_delay' must be numeric!")
         if value <= 0:
-            raise ValueError("Parameter 'minute_delay' must be greater than zero!")
-        self._minute_delay = value
-    '''
+            raise ValueError("Parameter 'minute_max_delay' must be greater than zero!")
+        self._minute_max_delay = value
+
     @property
     def max_el_time_min(self):
         return self._max_el_time_min
 
     @max_el_time_min.setter
     def max_el_time_min(self, value):
         if not isinstance(value, float) and not isinstance(value, int):
@@ -487,14 +497,17 @@
                     (self.data[self.time_field] >= start_time) & (self.data[self.time_field] <= end_time)]
                 self.df1 = self.subset[self.subset[self.id_field] == self.id1]
                 self.df2 = self.subset[self.subset[self.id_field] == self.id2]
             else:
                 self.df1 = self.data[self.data[self.id_field] == self.id1]
                 self.df2 = self.data[self.data[self.id_field] == self.id2]
 
+            if not self.__check_time_lag_and_overlap():
+                raise ValueError(f"Skipping pair {self.id1} and {self.id2} due to time lag greater than {self.minute_max_delay}!")
+
     def __start(self):
         """
         create PPAs for two moving objects (private method, only can be called inside the class)
         ellipses_list: all PPAs for two objects
         ellipses_list_id1: PPAs for object 1
         ellipses_list_id2: PPAs for object 2
         """
@@ -506,61 +519,59 @@
 
     def interaction_analysis(self):
         spatial_pairs = self.__get_spatial_intersect_pairs()
         all_intersection_pairs = get_timedelay_pairs(spatial_pairs, self.minute_min_delay, self.minute_max_delay)
 
         if not all_intersection_pairs:
             print(datetime.now(), 'Complete! No interaction found!')
-            return None, None, None
+            return None
         else:
+            results = ORTEGAResults()
+            results.set_intersection_ellipse_pair(all_intersection_pairs)
             print(datetime.now(), f'Complete! {len(all_intersection_pairs)} pairs of intersecting PPAs found!')
 
             # convert the list of intersecting ellipses to dataframe format - df_all_intersection_pairs
             df_all_intersection_pairs = intersect_ellipse_todataframe(all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_speed_diff(df_all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_direction_diff(df_all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_time_diff(df_all_intersection_pairs)
+            results.set_df_all_intersection_pairs(df_all_intersection_pairs)
 
             # compute duration of interaction and output as a dataframe - df_duration
             print(datetime.now(), 'Compute continues events...')
             df_continues = check_continuous(df_all_intersection_pairs, self.id1, self.id2)
             print(datetime.now(), f'Complete! {df_continues.shape[0]} interaction events identified!')
             if df_continues.shape[0] != 0:
-                return all_intersection_pairs, df_all_intersection_pairs, df_continues
+                results.set_df_interaction_events(df_continues)
+                return results
             else:
-                return None, None, None
-
-    def interaction_analysis2(self):
-
-        print(datetime.now(), 'Implement interaction analysis...')
-        # get list of intersecting Ellipse objects - all_intersection_pairs
-        # all_intersection_pairs = self.__get_spatiotemporal_intersect_pairs()
-        spatial_pairs = self.__get_spatial_intersect_pairs()
-        all_intersection_pairs = get_timedelay_pairs(spatial_pairs, self.minute_min_delay, self.minute_max_delay)
+                return None
 
-        if not all_intersection_pairs:
-            print(datetime.now(), 'Complete! No interaction found!')
-            return None, None, None
-        else:
-            print(datetime.now(), f'Complete! {len(all_intersection_pairs)} pairs of intersecting PPAs found!')
-
-            # convert the list of intersecting ellipses to dataframe format - df_all_intersection_pairs
-            df_all_intersection_pairs = intersect_ellipse_todataframe(all_intersection_pairs)
-            df_all_intersection_pairs = interaction_compute_speed_diff(df_all_intersection_pairs)
-            df_all_intersection_pairs = interaction_compute_direction_diff(df_all_intersection_pairs)
-            df_all_intersection_pairs = interaction_compute_time_diff(df_all_intersection_pairs)
-
-            # compute duration of interaction and output as a dataframe - df_duration
-            print(datetime.now(), 'Compute duration of interaction...')
-            df_duration = durationEstimator(df_all_intersection_pairs, self.id1, self.id2)
-            print(datetime.now(), f'Complete! {df_duration.shape[0]} interaction events identified!')
-            if df_duration.shape[0] != 0:
-                return all_intersection_pairs, df_all_intersection_pairs, df_duration
-            else:
-                return None, None, None
+    def __check_time_lag_and_overlap(self):
+        """
+        Check time overlap and time lag between the movements of two individuals (private method, only can be called inside the class).
+        Returns a boolean value indicating whether the time lag is less than or equal to the allowable maximum delay (True) or not (False).
+        """
+        # Extract the start and end times for each individual
+        start1, end1 = self.df1[self.time_field].min(), self.df1[self.time_field].max()
+        start2, end2 = self.df2[self.time_field].min(), self.df2[self.time_field].max()
+
+        # Calculate the time overlap
+        overlap_start = max(start1, start2)
+        overlap_end = min(end1, end2)
+        overlap_duration = (overlap_end - overlap_start).total_seconds() / 60
+
+        # Check if there is no overlap
+        if overlap_duration <= 0:
+            # Calculate the time lag
+            time_lag = abs((start2 - end1).total_seconds() / 60) if end1 < start2 else abs((start1 - end2).total_seconds() / 60)
+            # Check if time lag is greater than the max delay
+            if time_lag > self.minute_max_delay:
+                return False
+        return True
 
     def __get_ellipse_list(self, df1: pd.DataFrame, df2: pd.DataFrame):
         """
         Create PPA ellipses using as input the two dataframes of GPS tracks of two moving objects
         :param df1: a pandas dataframe of GPS points of individual id1
         :param df2: a pandas dataframe of GPS points of individual id2
         :return:
```

### Comparing `ortega-1.0.5/ortega/visualization.py` & `ortega-1.0.7/ortega/visualization.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.5/setup.py` & `ortega-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == "__main__":
     setup(
         name='ortega',
-        version='1.0.5',
+        version='1.0.7',
         author='MOVE lab@UCSB',
         author_email="rongxiangsu@ucsb.edu",
         packages=["ortega"],
         url='https://github.com/move-ucsb/ORTEGA',
         license='MIT',
         description='ORTEGA',
         install_requires=[
```

