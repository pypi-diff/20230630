# Comparing `tmp/string_treatment-0.0.6.tar.gz` & `tmp/string_treatment-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_treatment-0.0.6.tar", last modified: Fri Jun 30 15:26:52 2023, max compression
+gzip compressed data, was "string_treatment-0.1.0.tar", last modified: Fri Jun 30 15:39:56 2023, max compression
```

## Comparing `string_treatment-0.0.6.tar` & `string_treatment-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:26:52.184462 string_treatment-0.0.6/
--rw-rw-rw-   0        0        0      620 2023-06-30 15:26:52.176884 string_treatment-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-06-30 15:26:14.000000 string_treatment-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 15:26:52.184462 string_treatment-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-06-30 15:26:28.000000 string_treatment-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:26:52.173442 string_treatment-0.0.6/string_treatment.egg-info/
--rw-rw-rw-   0        0        0      620 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4317 2023-06-30 15:13:11.000000 string_treatment-0.0.6/string_treatment.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:39:56.046358 string_treatment-0.1.0/
+-rw-rw-rw-   0        0        0      620 2023-06-30 15:39:56.044366 string_treatment-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-06-30 15:26:14.000000 string_treatment-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 15:39:56.046358 string_treatment-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-06-30 15:39:44.000000 string_treatment-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:39:56.039822 string_treatment-0.1.0/string_treatment.egg-info/
+-rw-rw-rw-   0        0        0      620 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4111 2023-06-30 15:37:14.000000 string_treatment-0.1.0/string_treatment.py
```

### Comparing `string_treatment-0.0.6/PKG-INFO` & `string_treatment-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_treatment
-Version: 0.0.6
+Version: 0.1.0
 Summary: String treatment package
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `string_treatment-0.0.6/README.md` & `string_treatment-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `string_treatment-0.0.6/setup.py` & `string_treatment-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6' 
+VERSION = '0.1.0' 
 DESCRIPTION = 'String treatment package'
 LONG_DESCRIPTION = '''
 Method to treat strings with inconsistencies in your data
 
 Github: https://github.com/guilhermehuther/string_treatment
 '''
```

### Comparing `string_treatment-0.0.6/string_treatment.egg-info/PKG-INFO` & `string_treatment-0.1.0/string_treatment.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-treatment
-Version: 0.0.6
+Version: 0.1.0
 Summary: String treatment package
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `string_treatment-0.0.6/string_treatment.py` & `string_treatment-0.1.0/string_treatment.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,110 +6,109 @@
 
 METRICS_DICT = {
   'jaro_winkler_similarity': jaro_winkler_similarity, 
   'damerau_levenshtein_distance': damerau_levenshtein_distance, 
   'hamming_distance': hamming_distance
 }
 
-class string_treatment:
-  def treat_unreferenced(strings_compared: list, 
-                         metrics: typing.Union[list[str], str] = 'all', 
-                         threshold: float = 0.9):
-    '''    
-    :param strings_compared: list of strings to be compared.
-    :param metrics: metrics to be tested as similiraty measurement of distance between strings.
-    :param threshold: threshold for the metrics similarity values.
-    
-    :return: list of strings 'corrected'.
-    '''
+def treat_unreferenced(strings_compared: list, 
+                        metrics: typing.Union[list[str], str] = 'all', 
+                        threshold: float = 0.9):
+  '''    
+  :param: strings_compared: list of strings to be compared.
+  :param: metrics: metrics to be tested as similiraty measurement of distance between strings.
+  :param: threshold: threshold for the metrics similarity values.
   
-    if metrics == 'all':
-      metrics = list(METRICS_DICT.keys())
-    elif type(metrics) == list or type(metrics) == str:
-      if type(metrics) == str: metrics = [metrics]
-    else:
-      raise TypeError('Metrics must be a list or string')
-    
-    if 0 > threshold > 1:
-      raise ValueError('Threshold must be between 0 and 1')
-    
-    try:
-      metrics_functions = [METRICS_DICT[x] for x in metrics] 
-    except:
-      raise KeyError("Metrics must be a list or string with the following values: 'jaro_winkler_similarity', 'damerau_levenshtein_distance', 'hamming_distance'.")
-    
-    metrics_results = dict()
+  :return: list of strings 'corrected'.
+  '''
+
+  if metrics == 'all':
+    metrics = list(METRICS_DICT.keys())
+  elif type(metrics) == list or type(metrics) == str:
+    if type(metrics) == str: metrics = [metrics]
+  else:
+    raise TypeError('Metrics must be a list or string')
+  
+  if 0 > threshold > 1:
+    raise ValueError('Threshold must be between 0 and 1')
+  
+  try:
+    metrics_functions = [METRICS_DICT[x] for x in metrics] 
+  except:
+    raise KeyError("Metrics must be a list or string with the following values: 'jaro_winkler_similarity', 'damerau_levenshtein_distance', 'hamming_distance'.")
+  
+  metrics_results = dict()
 
-    for metric in metrics_functions:
-      already_corrected = list()
-      strings = strings_compared.copy()
-      metric_sum = [0, 0]
+  for metric in metrics_functions:
+    already_corrected = list()
+    strings = strings_compared.copy()
+    metric_sum = [0, 0]
+    
+    for i in range(len(strings)):
+      distances = dict()
+      if strings[i] in already_corrected: 
+        continue
+      for j in range(i + 1, len(strings)):   
+        if strings[j] in already_corrected: 
+          continue      
+        distances[strings[j]] = metric(strings[i].lower().strip(), strings[j].lower().strip())
+          
+      all_distances = pd.DataFrame(data = distances, index = [0]).unstack().reset_index().drop('level_1', axis = 1)
       
-      for i in range(len(strings)):
-        distances = dict()
-        if strings[i] in already_corrected: 
-          continue
-        for j in range(i + 1, len(strings)):   
-          if strings[j] in already_corrected: 
-            continue      
-          distances[strings[j]] = metric(strings[i].lower().strip(), strings[j].lower().strip())
-            
-        all_distances = pd.DataFrame(data = distances, index = [0]).unstack().reset_index().drop('level_1', axis = 1)
-        
-        if metric.__name__ != 'jaro_winkler_similarity':
-          all_distances[0] = (all_distances[0] - all_distances[0].max()) / (all_distances[0].min() - all_distances[0].max())
-            
-        all_distances = all_distances[all_distances[0] >= threshold]
-        
-        if all_distances.empty: 
-          continue
-        
-        metric_sum[0] += all_distances[0].sum()
-        metric_sum[1] += all_distances[0].shape[0]
-        
-        all_distances_max_string = all_distances[all_distances[0] == max(all_distances[0])]['level_0'].values[0] 
-        
-        already_corrected.append(all_distances_max_string)  
+      if metric.__name__ != 'jaro_winkler_similarity':
+        all_distances[0] = (all_distances[0] - all_distances[0].max()) / (all_distances[0].min() - all_distances[0].max())
           
-        strings = np.where(np.isin(strings, all_distances['level_0'].values) == True, all_distances_max_string, strings) 
+      all_distances = all_distances[all_distances[0] >= threshold]
       
-      metric_sum = metric_sum[0] / metric_sum[1]
-            
-      metrics_results[metric.__name__] = (metric_sum, strings)
+      if all_distances.empty: 
+        continue
+      
+      metric_sum[0] += all_distances[0].sum()
+      metric_sum[1] += all_distances[0].shape[0]
+      
+      all_distances_max_string = all_distances[all_distances[0] == max(all_distances[0])]['level_0'].values[0] 
+      
+      already_corrected.append(all_distances_max_string)  
+        
+      strings = np.where(np.isin(strings, all_distances['level_0'].values) == True, all_distances_max_string, strings) 
     
-    best_metric = max(metrics_results.items(), key = operator.itemgetter(1))
+    metric_sum = metric_sum[0] / metric_sum[1]
+          
+    metrics_results[metric.__name__] = (metric_sum, strings)
+  
+  best_metric = max(metrics_results.items(), key = operator.itemgetter(1))
 
-    print(f"Best metric '{best_metric[0]}' with mean {best_metric[1][0]}.")
-    
-    return best_metric[1][1]
+  print(f"Best metric '{best_metric[0]}' with mean {best_metric[1][0]}.")
+  
+  return best_metric[1][1]
 
 
-  def treat_referenced(strings_compared: list[str], 
-                       reference: list[str],
-                       metric: str = 'jaro_winkler_similarity'):
-    '''    
-    :param strings_compared: list of strings to be compared.
-    :param reference: list of reference strings.
-    :param metric: metric to be used as similiraty measurement of distance between strings.
-    
-    :return: list of strings 'corrected'.
-    '''
-    
-    try:
-      metric = METRICS_DICT[metric]
-    except:
-      raise KeyError("metric must be a string with one of the following values: 'jaro_winkler_similarity' OR 'damerau_levenshtein_distance' OR 'hamming_distance'.")
-    
-    strings_corrected = list()
-    comparations = dict()
+def treat_referenced(strings_compared: list[str], 
+                      reference: list[str],
+                      metric: str = 'jaro_winkler_similarity'):
+  '''    
+  :param strings_compared: list of strings to be compared.
+  :param reference: list of reference strings.
+  :param metric: metric to be used as similiraty measurement of distance between strings.
+  
+  :return: list of strings 'corrected'.
+  '''
+  
+  try:
+    metric = METRICS_DICT[metric]
+  except:
+    raise KeyError("metric must be a string with one of the following values: 'jaro_winkler_similarity' OR 'damerau_levenshtein_distance' OR 'hamming_distance'.")
+  
+  strings_corrected = list()
+  comparations = dict()
 
-    for strings in strings_compared:
-      for ref in reference:
-        comparations[ref] = metric(strings.lower().strip(), ref.lower().strip())
+  for strings in strings_compared:
+    for ref in reference:
+      comparations[ref] = metric(strings.lower().strip(), ref.lower().strip())
 
-      strings_corrected.append(
-          max(comparations.items(), key = operator.itemgetter(1))[0]
-      )
+    strings_corrected.append(
+        max(comparations.items(), key = operator.itemgetter(1))[0]
+    )
 
-      comparations.clear()
+    comparations.clear()
 
-    return strings_corrected
+  return strings_corrected
```

