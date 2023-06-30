# Comparing `tmp/TEST_TC-0.1.8.tar.gz` & `tmp/TEST_TC-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-0.1.8.tar", last modified: Tue Jun 27 15:44:24 2023, max compression
+gzip compressed data, was "TEST_TC-0.1.9.tar", last modified: Tue Jun 27 16:25:49 2023, max compression
```

## Comparing `TEST_TC-0.1.8.tar` & `TEST_TC-0.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.296789 TEST_TC-0.1.8/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 15:44:24.295788 TEST_TC-0.1.8/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/README.md
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.227731 TEST_TC-0.1.8/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      997 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/top_level.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1126 2023-06-27 14:56:18.000000 TEST_TC-0.1.8/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 15:44:24.296877 TEST_TC-0.1.8/setup.cfg
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.229764 TEST_TC-0.1.8/tc_uc4/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 15:37:10.000000 TEST_TC-0.1.8/tc_uc4/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.236762 TEST_TC-0.1.8/tc_uc4/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5803 2023-06-27 15:13:46.000000 TEST_TC-0.1.8/tc_uc4/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-06-27 15:13:53.000000 TEST_TC-0.1.8/tc_uc4/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.241036 TEST_TC-0.1.8/tc_uc4/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2810 2023-06-27 15:04:47.000000 TEST_TC-0.1.8/tc_uc4/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.245181 TEST_TC-0.1.8/tc_uc4/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7308 2023-06-27 15:01:58.000000 TEST_TC-0.1.8/tc_uc4/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.253045 TEST_TC-0.1.8/tc_uc4/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17975 2023-06-27 15:15:06.000000 TEST_TC-0.1.8/tc_uc4/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3126 2023-06-27 15:15:12.000000 TEST_TC-0.1.8/tc_uc4/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.255555 TEST_TC-0.1.8/tc_uc4/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.256558 TEST_TC-0.1.8/tc_uc4/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/datavisualization/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.270014 TEST_TC-0.1.8/tc_uc4/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      949 2023-06-27 14:58:09.000000 TEST_TC-0.1.8/tc_uc4/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.8/tc_uc4/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2119 2023-06-27 14:58:38.000000 TEST_TC-0.1.8/tc_uc4/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6328 2023-06-27 15:43:46.000000 TEST_TC-0.1.8/tc_uc4/utility/tele_logger.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.292790 TEST_TC-0.1.8/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2762 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15261 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1864 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2873 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2169 2023-06-27 15:42:28.000000 TEST_TC-0.1.8/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2947 2023-06-27 15:44:13.000000 TEST_TC-0.1.8/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.805646 TEST_TC-0.1.9/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 16:25:49.804646 TEST_TC-0.1.9/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.9/README.md
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.723596 TEST_TC-0.1.9/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 16:25:49.000000 TEST_TC-0.1.9/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      997 2023-06-27 16:25:49.000000 TEST_TC-0.1.9/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 16:25:49.000000 TEST_TC-0.1.9/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 16:25:49.000000 TEST_TC-0.1.9/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 16:25:49.000000 TEST_TC-0.1.9/TEST_TC.egg-info/top_level.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1126 2023-06-27 14:56:18.000000 TEST_TC-0.1.9/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 16:25:49.805646 TEST_TC-0.1.9/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.727495 TEST_TC-0.1.9/tc_uc4/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 16:23:19.000000 TEST_TC-0.1.9/tc_uc4/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.737115 TEST_TC-0.1.9/tc_uc4/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.9/tc_uc4/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5803 2023-06-27 15:13:46.000000 TEST_TC-0.1.9/tc_uc4/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-06-27 15:13:53.000000 TEST_TC-0.1.9/tc_uc4/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.742114 TEST_TC-0.1.9/tc_uc4/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.9/tc_uc4/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2810 2023-06-27 15:04:47.000000 TEST_TC-0.1.9/tc_uc4/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.748205 TEST_TC-0.1.9/tc_uc4/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.9/tc_uc4/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7298 2023-06-27 16:21:28.000000 TEST_TC-0.1.9/tc_uc4/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.756718 TEST_TC-0.1.9/tc_uc4/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.9/tc_uc4/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17975 2023-06-27 15:15:06.000000 TEST_TC-0.1.9/tc_uc4/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3126 2023-06-27 15:15:12.000000 TEST_TC-0.1.9/tc_uc4/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.759239 TEST_TC-0.1.9/tc_uc4/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.9/tc_uc4/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.761718 TEST_TC-0.1.9/tc_uc4/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.9/tc_uc4/datavisualization/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.776105 TEST_TC-0.1.9/tc_uc4/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.9/tc_uc4/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      949 2023-06-27 14:58:09.000000 TEST_TC-0.1.9/tc_uc4/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.9/tc_uc4/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2119 2023-06-27 14:58:38.000000 TEST_TC-0.1.9/tc_uc4/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6328 2023-06-27 15:43:46.000000 TEST_TC-0.1.9/tc_uc4/utility/tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 16:25:49.801962 TEST_TC-0.1.9/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:54:10.000000 TEST_TC-0.1.9/tests/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 14:54:10.000000 TEST_TC-0.1.9/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2762 2023-06-27 14:54:10.000000 TEST_TC-0.1.9/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15261 2023-06-27 14:54:10.000000 TEST_TC-0.1.9/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1864 2023-06-27 14:54:10.000000 TEST_TC-0.1.9/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 14:54:10.000000 TEST_TC-0.1.9/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2873 2023-06-27 14:54:10.000000 TEST_TC-0.1.9/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 14:54:10.000000 TEST_TC-0.1.9/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2169 2023-06-27 15:42:28.000000 TEST_TC-0.1.9/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3089 2023-06-27 15:51:58.000000 TEST_TC-0.1.9/tests/test_tele_logger.py
```

### Comparing `TEST_TC-0.1.8/README.md` & `TEST_TC-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-0.1.9/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/pyproject.toml` & `TEST_TC-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tc_uc4/algorithms/algorithm.py` & `TEST_TC-0.1.9/tc_uc4/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tc_uc4/algorithms/prophet_utils.py` & `TEST_TC-0.1.9/tc_uc4/algorithms/prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tc_uc4/analytics/evaluationMetrics.py` & `TEST_TC-0.1.9/tc_uc4/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tc_uc4/datahandler/datahandler.py` & `TEST_TC-0.1.9/tc_uc4/datahandler/datahandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from typing import Any
 
 import geopandas as gpd
 import pandas as pd
 from typing_extensions import Self
 from tc_uc4.utility.exceptions import InputTypeError
 from tc_uc4.utility.resources import log_exception
-from tc_uc4.utility.tele_logger import logger
+from __main__ import logger
 
 class DataHandler:
+    
     def __init__(self, data_folder : str) -> Self:
         """Class which will handle the read and write of .parquet data
 
         Parameters
         ----------
         data_folder : str
             Main folder where to find the data, if given as a parameter
         """
+
         if type(data_folder) != str:
             raise InputTypeError('DataHandler')
 
         self.data_folder = data_folder
 
     @log_exception(logger)
     def read(self, filename: str, folder: str = "input", in_attr: bool = False, **kwargs: Any) -> pd.DataFrame:
```

### Comparing `TEST_TC-0.1.8/tc_uc4/datapreparation/datapreparation_utils.py` & `TEST_TC-0.1.9/tc_uc4/datapreparation/datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tc_uc4/datapreparation/prep.py` & `TEST_TC-0.1.9/tc_uc4/datapreparation/prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tc_uc4/utility/constants.py` & `TEST_TC-0.1.9/tc_uc4/utility/constants.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tc_uc4/utility/exceptions.py` & `TEST_TC-0.1.9/tc_uc4/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tc_uc4/utility/resources.py` & `TEST_TC-0.1.9/tc_uc4/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tc_uc4/utility/tele_logger.py` & `TEST_TC-0.1.9/tc_uc4/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tests/test_algorithm.py` & `TEST_TC-0.1.9/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tests/test_datahandler.py` & `TEST_TC-0.1.9/tests/test_datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tests/test_datapreparation_utils.py` & `TEST_TC-0.1.9/tests/test_datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tests/test_evaluations.py` & `TEST_TC-0.1.9/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tests/test_exceptions.py` & `TEST_TC-0.1.9/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tests/test_prep.py` & `TEST_TC-0.1.9/tests/test_prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tests/test_prophet_utils.py` & `TEST_TC-0.1.9/tests/test_prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.8/tests/test_resources.py` & `TEST_TC-0.1.9/tests/test_resources.py`

 * *Files identical despite different names*

