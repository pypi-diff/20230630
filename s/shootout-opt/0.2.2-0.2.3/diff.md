# Comparing `tmp/shootout-opt-0.2.2.tar.gz` & `tmp/shootout-opt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shootout-opt-0.2.2.tar", last modified: Tue Apr 11 14:50:51 2023, max compression
+gzip compressed data, was "shootout-opt-0.2.3.tar", last modified: Fri Jun 30 13:09:53 2023, max compression
```

## Comparing `shootout-opt-0.2.2.tar` & `shootout-opt-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.437531 shootout-opt-0.2.2/
--rw-r--r--   0 cohen    (11323) creatis    (500)     1072 2023-04-11 14:42:58.000000 shootout-opt-0.2.2/LICENSE
--rw-r--r--   0 cohen    (11323) creatis    (500)     3268 2023-04-11 14:50:51.436531 shootout-opt-0.2.2/PKG-INFO
--rw-r--r--   0 cohen    (11323) creatis    (500)     1630 2023-04-11 14:48:11.000000 shootout-opt-0.2.2/README.md
--rw-r--r--   0 cohen    (11323) creatis    (500)      693 2023-04-11 14:50:42.000000 shootout-opt-0.2.2/pyproject.toml
--rw-r--r--   0 cohen    (11323) creatis    (500)       38 2023-04-11 14:50:51.437531 shootout-opt-0.2.2/setup.cfg
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.432531 shootout-opt-0.2.2/shootout/
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.434531 shootout-opt-0.2.2/shootout/methods/
--rw-r--r--   0 cohen    (11323) creatis    (500)      121 2022-09-01 08:14:10.000000 shootout-opt-0.2.2/shootout/methods/pipeplines.py
--rw-r--r--   0 cohen    (11323) creatis    (500)      972 2022-07-05 13:34:55.000000 shootout-opt-0.2.2/shootout/methods/plotters.py
--rw-r--r--   0 cohen    (11323) creatis    (500)    19524 2023-04-11 12:08:25.000000 shootout-opt-0.2.2/shootout/methods/post_processors.py
--rw-r--r--   0 cohen    (11323) creatis    (500)    10547 2023-04-11 12:08:25.000000 shootout-opt-0.2.2/shootout/methods/runners.py
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.435531 shootout-opt-0.2.2/shootout/tests/
--rw-r--r--   0 cohen    (11323) creatis    (500)        0 2022-09-23 13:27:36.000000 shootout-opt-0.2.2/shootout/tests/test_plotters.py
--rw-r--r--   0 cohen    (11323) creatis    (500)     2746 2023-04-11 09:42:06.000000 shootout-opt-0.2.2/shootout/tests/test_post_processors.py
--rw-r--r--   0 cohen    (11323) creatis    (500)     1918 2023-04-11 12:08:25.000000 shootout-opt-0.2.2/shootout/tests/test_runners.py
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.436531 shootout-opt-0.2.2/shootout_opt.egg-info/
--rw-r--r--   0 cohen    (11323) creatis    (500)     3268 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/PKG-INFO
--rw-r--r--   0 cohen    (11323) creatis    (500)      437 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/SOURCES.txt
--rw-r--r--   0 cohen    (11323) creatis    (500)        1 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/dependency_links.txt
--rw-r--r--   0 cohen    (11323) creatis    (500)       87 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/requires.txt
--rw-r--r--   0 cohen    (11323) creatis    (500)        9 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/top_level.txt
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-06-30 13:09:53.712148 shootout-opt-0.2.3/
+-rw-r--r--   0 cohen    (11323) creatis    (500)     1072 2023-04-11 14:42:58.000000 shootout-opt-0.2.3/LICENSE
+-rw-r--r--   0 cohen    (11323) creatis    (500)     3268 2023-06-30 13:09:53.712148 shootout-opt-0.2.3/PKG-INFO
+-rw-r--r--   0 cohen    (11323) creatis    (500)     1630 2023-04-11 14:48:11.000000 shootout-opt-0.2.3/README.md
+-rw-r--r--   0 cohen    (11323) creatis    (500)      693 2023-06-30 13:07:46.000000 shootout-opt-0.2.3/pyproject.toml
+-rw-r--r--   0 cohen    (11323) creatis    (500)       38 2023-06-30 13:09:53.712148 shootout-opt-0.2.3/setup.cfg
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-06-30 13:09:53.708148 shootout-opt-0.2.3/shootout/
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-06-30 13:09:53.710148 shootout-opt-0.2.3/shootout/methods/
+-rw-r--r--   0 cohen    (11323) creatis    (500)      121 2022-09-01 08:14:10.000000 shootout-opt-0.2.3/shootout/methods/pipeplines.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)      972 2022-07-05 13:34:55.000000 shootout-opt-0.2.3/shootout/methods/plotters.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)    21442 2023-06-29 15:18:46.000000 shootout-opt-0.2.3/shootout/methods/post_processors.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)    10631 2023-04-17 11:04:04.000000 shootout-opt-0.2.3/shootout/methods/runners.py
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-06-30 13:09:53.711148 shootout-opt-0.2.3/shootout/tests/
+-rw-r--r--   0 cohen    (11323) creatis    (500)        0 2022-09-23 13:27:36.000000 shootout-opt-0.2.3/shootout/tests/test_plotters.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)     2746 2023-04-11 09:42:06.000000 shootout-opt-0.2.3/shootout/tests/test_post_processors.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)     1918 2023-04-11 12:08:25.000000 shootout-opt-0.2.3/shootout/tests/test_runners.py
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-06-30 13:09:53.711148 shootout-opt-0.2.3/shootout_opt.egg-info/
+-rw-r--r--   0 cohen    (11323) creatis    (500)     3268 2023-06-30 13:09:53.000000 shootout-opt-0.2.3/shootout_opt.egg-info/PKG-INFO
+-rw-r--r--   0 cohen    (11323) creatis    (500)      437 2023-06-30 13:09:53.000000 shootout-opt-0.2.3/shootout_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 cohen    (11323) creatis    (500)        1 2023-06-30 13:09:53.000000 shootout-opt-0.2.3/shootout_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 cohen    (11323) creatis    (500)       87 2023-06-30 13:09:53.000000 shootout-opt-0.2.3/shootout_opt.egg-info/requires.txt
+-rw-r--r--   0 cohen    (11323) creatis    (500)        9 2023-06-30 13:09:53.000000 shootout-opt-0.2.3/shootout_opt.egg-info/top_level.txt
```

### Comparing `shootout-opt-0.2.2/LICENSE` & `shootout-opt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.2/PKG-INFO` & `shootout-opt-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootout-opt
-Version: 0.2.2
+Version: 0.2.3
 Summary: Run algorithms, store and compare their outputs
 Author-email: "Jeremy E. Cohen" <jeremy.cohen@cnrs.fr>
 License: MIT License
         
         Copyright (c) 2023 Jeremy E. Cohen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `shootout-opt-0.2.2/README.md` & `shootout-opt-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.2/pyproject.toml` & `shootout-opt-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shootout-opt"
-version = "0.2.2"
+version = "0.2.3"
 description="Run algorithms, store and compare their outputs"
 authors=[{name= "Jeremy E. Cohen", email = "jeremy.cohen@cnrs.fr"}]
 license={ file = "LICENSE"}
 readme = "README.md"
 keywords = ["numerical optimisation", "visualisation", "python"]
 dependencies = [
     "numpy >= 1.23",
```

### Comparing `shootout-opt-0.2.2/shootout/methods/plotters.py` & `shootout-opt-0.2.3/shootout/methods/plotters.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.2/shootout/methods/post_processors.py` & `shootout-opt-0.2.3/shootout/methods/post_processors.py`

 * *Files 6% similar despite different names*

```diff
@@ -359,14 +359,46 @@
             new_errors = np.interp(time_grid, df[time_name][idx_errors], errors)
             # we can update the dataframe on the fly
             df["errors_interp"][idx_errors]=new_errors
             df["timings_interp"][idx_errors]=time_grid
 
     return df
 
+def median_or_mean_and_errors(df, value_plotted, ignored_parameters, quantile=0.8, mean=True):
+    """
+    Compute the median or mean of values in column ``value_plotted`` in df, ignoring (i.e. grouping-by) columns in list ``ignored_parameters``.
+    Adds upper/lower estimates (aka error bars) for the values ``df["value_plotted"]``. The estimates are taken over the variables NOT in ``df[x]`` for x in ``parameters`` using quantiles.
+    
+    This function creates a new dataframe with ``3 + len(ignored_parameters)`` columns named ``value_plotted``, ``value_plotted``_08 and ``value_plotted``_02 and the strings in ``ignored_parameters``.
+
+    Parameters
+    ----------
+    df : pandas dataframe
+        input dataframe with column ``value_plotted`` and ``parameters``.
+    value_plotted : string
+        the name of the column in df for which error bars are required.
+    ignored_parameters : list of strings
+        the names of columns which are grouped-by to perform the quantile estimation. They will not be used together for the quantile estimate, use this for instance for the x variable in a y/x plot where error bars are computed on y over several seeds.
+    quantile : float, optional
+        quantile value, by default 0.8
+    mean : boolean, optional
+        True is mean is returned, False if median, by default True
+
+    Return
+    ------
+    pandas dataframe
+    """
+    df_median = df.groupby(ignored_parameters, as_index=False)[value_plotted].mean()
+    df_02 = df.groupby(ignored_parameters, as_index=False)[value_plotted].quantile(q=0.2)
+    df_08 = df.groupby(ignored_parameters, as_index=False)[value_plotted].quantile(q=0.8)
+    value_plotted_08 = value_plotted+"_08"
+    value_plotted_02 = value_plotted+"_02"
+    df_median[value_plotted_08] = df_08[value_plotted]-df_median[value_plotted]
+    df_median[value_plotted_02] = -df_02[value_plotted]+df_median[value_plotted]
+    return df_median
 
 def median_convergence_plot(df_conv, type_x="iterations", err_name="errors", time_name="timings", mean=False):
     """
     Computes the mean or median of several converge plots with respect to either time or iterations (this is determined by ``type_x``). By mean/median of several curve, we mean the mean/median at each ``type_x`` value.
 
     Parameters
     ----------
```

### Comparing `shootout-opt-0.2.2/shootout/methods/runners.py` & `shootout-opt-0.2.3/shootout/methods/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     >>>     # and hyperparameter with 0.1, 1 and 10
     >>>     errors, timings, anything_else = my_algorithm(random_data,n,m,hyperparameter)
     >>>     errors2, timings2, anything_else2 = my_competitor(random_data,n,m,hyperparameter)
     >>>     return {"errors": [errors, errors2], "timings": [timings, timings2]}
 
     The naming of the inputs and outputs is completely free. However, naming errors/loss/utility collected in a list exactly ``errors`` and ``timings`` (time starting from 0) will allow for immediate processing with utilities from shootout such as plotting convergence curves.
 
-    The recommended syntax when many parameters are involved is to define all the parameters in a dictionary, see ``**kwa`` below. For the signature of the inner function, one should also use a dictionary that makes use of the same keys.
+    The recommended syntax when many parameters are involved is to define all the parameters in a dictionary, see ``**kwa`` below. For the signature of the inner function, one should also use a dictionary with the same keys.
 
     Parameters
     ----------
     **kwa: dictionary, optional
         A dictionary containing all the elements in the signature of the function to run. Typically use in the following fashion:
 
         >>> vars = dict(
@@ -98,15 +98,14 @@
     """
     #TODO: better error messages/error catching \
     #    - missmatches input names / loop variables
     #    - solo fun vs several
     #    - algorithm_names length does not match outputs
     
     def inner_run_and_track(fun):    
-        print(f"verbose works?? {verbose}")
         # Preprocessing things
         if skip:
             return
 
         # Preprocessing: converting any single value in kwa to a singleton list
         # also tracking names of list parameters for rebuilding columns
         list_params_keys = []
@@ -117,22 +116,22 @@
                 kwa[i] = [kwa[i]]
             else:
                 # get length of items in the list
                 if type(kwa[i][0])==list:
                     list_params_keys.append(i)
                     list_params_lengths.append(len(kwa[i][0]))
 
+        single_method=True
         if algorithm_names:
             if len(algorithm_names)>1:
                 single_method=False
-            else:
-                single_method=True
         else:
             # TODO Warning
             print("Consider adding algorithm names to benefit from automatic labeling of runs")
+            print("If several outputs are considered in the wrapped function for each key in a list, you must use the algorithm name field to name each such output.")
 
         # Before all, initialize our storage DataFrame
         df = pandas.DataFrame()
 
         # Now we enter the big loop
         for params in itertools.product(*[kwa[key] for key in kwa]):
             # Discrete printing for following the run
```

### Comparing `shootout-opt-0.2.2/shootout/tests/test_post_processors.py` & `shootout-opt-0.2.3/shootout/tests/test_post_processors.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.2/shootout/tests/test_runners.py` & `shootout-opt-0.2.3/shootout/tests/test_runners.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.2/shootout_opt.egg-info/PKG-INFO` & `shootout-opt-0.2.3/shootout_opt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootout-opt
-Version: 0.2.2
+Version: 0.2.3
 Summary: Run algorithms, store and compare their outputs
 Author-email: "Jeremy E. Cohen" <jeremy.cohen@cnrs.fr>
 License: MIT License
         
         Copyright (c) 2023 Jeremy E. Cohen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

