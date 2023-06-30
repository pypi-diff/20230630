# Comparing `tmp/rots-py-1.2.0.tar.gz` & `tmp/rots-py-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rots-py-1.2.0.tar", last modified: Sat Jun 24 16:17:46 2023, max compression
+gzip compressed data, was "rots-py-1.2.1.tar", last modified: Fri Jun 30 13:10:06 2023, max compression
```

## Comparing `rots-py-1.2.0.tar` & `rots-py-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 16:17:46.007294 rots-py-1.2.0/
--rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     6228 2023-06-24 16:17:46.005295 rots-py-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4431 2023-06-24 16:12:35.000000 rots-py-1.2.0/README.md
--rw-rw-rw-   0        0        0      726 2023-06-24 16:12:58.000000 rots-py-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 16:17:46.007294 rots-py-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-24 16:17:45.392735 rots-py-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 16:17:45.586198 rots-py-1.2.0/src/optim_cy/
--rw-rw-rw-   0        0        0      542 2023-06-17 21:26:16.000000 rots-py-1.2.0/src/optim_cy/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 16:17:45.735870 rots-py-1.2.0/src/rots_py.egg-info/
--rw-rw-rw-   0        0        0     6228 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 16:17:46.000295 rots-py-1.2.0/src/rotspy/
--rw-rw-rw-   0        0        0      108 2023-06-23 15:38:53.000000 rots-py-1.2.0/src/rotspy/__init__.py
--rw-rw-rw-   0        0        0      139 2023-06-23 15:31:50.000000 rots-py-1.2.0/src/rotspy/__main__.py
--rw-rw-rw-   0        0        0     3101 2023-04-26 17:07:58.000000 rots-py-1.2.0/src/rotspy/calculateOverlaps1.py
--rw-rw-rw-   0        0        0     2816 2023-04-26 17:08:25.000000 rots-py-1.2.0/src/rotspy/calculateOverlaps2.py
--rw-rw-rw-   0        0        0    10374 2023-06-24 16:05:38.000000 rots-py-1.2.0/src/rotspy/helpers.py
--rw-rw-rw-   0        0        0     2382 2023-06-23 15:38:30.000000 rots-py-1.2.0/src/rotspy/plot_rots.py
--rw-rw-rw-   0        0        0    11320 2023-06-23 15:40:17.000000 rots-py-1.2.0/src/rotspy/rots.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.800663 rots-py-1.2.1/
+-rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       91 2023-06-30 13:08:44.000000 rots-py-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6380 2023-06-30 13:10:06.798663 rots-py-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4583 2023-06-30 10:40:04.000000 rots-py-1.2.1/README.md
+-rw-rw-rw-   0        0        0      858 2023-06-30 13:09:16.000000 rots-py-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     2390 2023-06-29 12:09:31.000000 rots-py-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 13:10:06.800663 rots-py-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.579664 rots-py-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.664664 rots-py-1.2.1/src/optim_cy/
+-rw-rw-rw-   0        0        0   184832 2023-06-18 22:44:29.000000 rots-py-1.2.1/src/optim_cy/optim.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0      542 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/optim_cy/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.756666 rots-py-1.2.1/src/rots_py.egg-info/
+-rw-rw-rw-   0        0        0     6380 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.795666 rots-py-1.2.1/src/rotspy/
+-rw-rw-rw-   0        0        0      108 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/__main__.py
+-rw-rw-rw-   0        0        0     3101 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/calculateOverlaps1.py
+-rw-rw-rw-   0        0        0     2816 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/calculateOverlaps2.py
+-rw-rw-rw-   0        0        0    10374 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/helpers.py
+-rw-rw-rw-   0        0        0     2382 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/plot_rots.py
+-rw-rw-rw-   0        0        0    11320 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/rots.py
```

### Comparing `rots-py-1.2.0/LICENSE` & `rots-py-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.0/PKG-INFO` & `rots-py-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.2.0
+Version: 1.2.1
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,18 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rots-py
 
+[![PyPI](https://img.shields.io/pypi/v/rots-py)](https://pypi.org/project/rots-py/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/rots-py)
+
+
 Python implementation of the __Reproducibility-Optimized Test Statistic (ROTS)__ for gene ranking from the [Bioconductor ROTS](https://www.bioconductor.org/packages/release/bioc/html/ROTS.html) package.
 
 ROTS belongs to a familly of gene ranking statistics that aim to rank genes based on evidence for differential expression in two-group comparisons. ROTS is a non-parametric method that uses a permutation test to assess the significance of the observed differential expression. ROTS is designed to be robust to outliers and to be reproducible across different studies.
 
 __NOTE__: Data should have at least two non-null values per row for both groups.
 
 # Installation 
@@ -68,14 +72,15 @@
 summary = get_summary(result, fdr_c=0.05)
 
 # Plot volcano plot from the results
 plot_rots(result, fdr=0.05, type="volcano")
 ```
 
 # Methods
+
 ## rots(...)
 Runs the ROTS analysis on the given data. Returns a Python dictionary.
 
 ## Parameters
 - `data`: A pandas dataframe with genes/proteins as rows and samples as columns. (required)
 - `group`: A pandas series with the group labels for each sample. (required)
 - `B`: Number of permutations to perform. Default is 500. (optional)
```

### Comparing `rots-py-1.2.0/README.md` & `rots-py-1.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # rots-py
 
+[![PyPI](https://img.shields.io/pypi/v/rots-py)](https://pypi.org/project/rots-py/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/rots-py)
+
+
 Python implementation of the __Reproducibility-Optimized Test Statistic (ROTS)__ for gene ranking from the [Bioconductor ROTS](https://www.bioconductor.org/packages/release/bioc/html/ROTS.html) package.
 
 ROTS belongs to a familly of gene ranking statistics that aim to rank genes based on evidence for differential expression in two-group comparisons. ROTS is a non-parametric method that uses a permutation test to assess the significance of the observed differential expression. ROTS is designed to be robust to outliers and to be reproducible across different studies.
 
 __NOTE__: Data should have at least two non-null values per row for both groups.
 
 # Installation 
@@ -32,14 +36,15 @@
 summary = get_summary(result, fdr_c=0.05)
 
 # Plot volcano plot from the results
 plot_rots(result, fdr=0.05, type="volcano")
 ```
 
 # Methods
+
 ## rots(...)
 Runs the ROTS analysis on the given data. Returns a Python dictionary.
 
 ## Parameters
 - `data`: A pandas dataframe with genes/proteins as rows and samples as columns. (required)
 - `group`: A pandas series with the group labels for each sample. (required)
 - `B`: Number of permutations to perform. Default is 500. (optional)
```

### Comparing `rots-py-1.2.0/pyproject.toml` & `rots-py-1.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # pyproject.toml
 
+[build-system]
+requires      = ["setuptools>=58.1.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
 [project]
 name = "rots-py"
-version = "1.2.0"
+version = "1.2.1"
 description = "ROTS gene ranking implementation in Python"
 readme = "README.md"
 authors = [{ name = "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq", email = "fmamadbe@abo.fi" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -14,14 +18,15 @@
 ]
 keywords = ["rots", "gene", "ranking"]
 dependencies = [
     "numba >= 0.56.4",
     "numpy",
     "pandas",
     "tqdm>=4.64.1",
+    "Cython>=0.29.35",
 ]
 requires-python = ">=3.6"
 
 [project.urls]
 Homepage = "https://github.com/EDISS-intake2-team4/rots-py"
 
 [project.scripts]
```

### Comparing `rots-py-1.2.0/src/optim_cy/setup.py` & `rots-py-1.2.1/src/optim_cy/setup.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.0/src/rots_py.egg-info/PKG-INFO` & `rots-py-1.2.1/src/rots_py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.2.0
+Version: 1.2.1
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,18 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rots-py
 
+[![PyPI](https://img.shields.io/pypi/v/rots-py)](https://pypi.org/project/rots-py/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/rots-py)
+
+
 Python implementation of the __Reproducibility-Optimized Test Statistic (ROTS)__ for gene ranking from the [Bioconductor ROTS](https://www.bioconductor.org/packages/release/bioc/html/ROTS.html) package.
 
 ROTS belongs to a familly of gene ranking statistics that aim to rank genes based on evidence for differential expression in two-group comparisons. ROTS is a non-parametric method that uses a permutation test to assess the significance of the observed differential expression. ROTS is designed to be robust to outliers and to be reproducible across different studies.
 
 __NOTE__: Data should have at least two non-null values per row for both groups.
 
 # Installation 
@@ -68,14 +72,15 @@
 summary = get_summary(result, fdr_c=0.05)
 
 # Plot volcano plot from the results
 plot_rots(result, fdr=0.05, type="volcano")
 ```
 
 # Methods
+
 ## rots(...)
 Runs the ROTS analysis on the given data. Returns a Python dictionary.
 
 ## Parameters
 - `data`: A pandas dataframe with genes/proteins as rows and samples as columns. (required)
 - `group`: A pandas series with the group labels for each sample. (required)
 - `B`: Number of permutations to perform. Default is 500. (optional)
```

### Comparing `rots-py-1.2.0/src/rotspy/calculateOverlaps1.py` & `rots-py-1.2.1/src/rotspy/calculateOverlaps1.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.0/src/rotspy/calculateOverlaps2.py` & `rots-py-1.2.1/src/rotspy/calculateOverlaps2.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.0/src/rotspy/helpers.py` & `rots-py-1.2.1/src/rotspy/helpers.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.0/src/rotspy/plot_rots.py` & `rots-py-1.2.1/src/rotspy/plot_rots.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.0/src/rotspy/rots.py` & `rots-py-1.2.1/src/rotspy/rots.py`

 * *Files identical despite different names*

