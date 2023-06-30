# Comparing `tmp/plottah-0.1.8.tar.gz` & `tmp/plottah-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plottah-0.1.8.tar", max compression
+gzip compressed data, was "plottah-0.1.9.tar", max compression
```

## Comparing `plottah-0.1.8.tar` & `plottah-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1123 2023-06-29 11:03:06.506744 plottah-0.1.8/README.md
--rw-r--r--   0        0        0       22 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/__init__.py
--rw-r--r--   0        0        0     2648 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/__main__.py
--rw-r--r--   0        0        0     1339 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/colors.py
--rw-r--r--   0        0        0     4841 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/config.py
--rw-r--r--   0        0        0       24 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/plot_builder/__init__.py
--rw-r--r--   0        0        0     3821 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/plot_builder/builders.py
--rw-r--r--   0        0        0     7563 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plot_handler/PlotHandler.py
--rw-r--r--   0        0        0       37 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plot_handler/__init__.py
--rw-r--r--   0        0        0    10631 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/BinEventRatePlot.py
--rw-r--r--   0        0        0     3987 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/DistPlot.py
--rw-r--r--   0        0        0     3030 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/PlotProtocol.py
--rw-r--r--   0        0        0     3578 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/RocCurvePlot.py
--rw-r--r--   0        0        0      117 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/__init__.py
--rw-r--r--   0        0        0     4179 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/utils.py
--rw-r--r--   0        0        0      529 2023-06-29 11:03:46.395293 plottah-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 plottah-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-06-29 11:51:33.915381 plottah-0.1.9/README.md
+-rw-r--r--   0        0        0       22 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/__init__.py
+-rw-r--r--   0        0        0     2648 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/__main__.py
+-rw-r--r--   0        0        0     1339 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/colors.py
+-rw-r--r--   0        0        0     4841 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/config.py
+-rw-r--r--   0        0        0       24 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/plot_builder/__init__.py
+-rw-r--r--   0        0        0     3821 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/plot_builder/builders.py
+-rw-r--r--   0        0        0     7563 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/plot_handler/PlotHandler.py
+-rw-r--r--   0        0        0       37 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/plot_handler/__init__.py
+-rw-r--r--   0        0        0    10631 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/plots/BinEventRatePlot.py
+-rw-r--r--   0        0        0     3987 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/plots/DistPlot.py
+-rw-r--r--   0        0        0     3016 2023-06-29 11:51:36.043379 plottah-0.1.9/plottah/plots/PlotProtocol.py
+-rw-r--r--   0        0        0     3578 2023-06-29 11:51:36.047379 plottah-0.1.9/plottah/plots/RocCurvePlot.py
+-rw-r--r--   0        0        0      117 2023-06-29 11:51:36.047379 plottah-0.1.9/plottah/plots/__init__.py
+-rw-r--r--   0        0        0     4179 2023-06-29 11:51:36.047379 plottah-0.1.9/plottah/utils.py
+-rw-r--r--   0        0        0      529 2023-06-29 11:52:17.247197 plottah-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 plottah-0.1.9/PKG-INFO
```

### Comparing `plottah-0.1.8/README.md` & `plottah-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/plottah/__main__.py` & `plottah-0.1.9/plottah/__main__.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/plottah/colors.py` & `plottah-0.1.9/plottah/colors.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/plottah/config.py` & `plottah-0.1.9/plottah/config.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/plottah/plot_builder/builders.py` & `plottah-0.1.9/plottah/plot_builder/builders.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/plottah/plot_handler/PlotHandler.py` & `plottah-0.1.9/plottah/plot_handler/PlotHandler.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/plottah/plots/BinEventRatePlot.py` & `plottah-0.1.9/plottah/plots/BinEventRatePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/plottah/plots/DistPlot.py` & `plottah-0.1.9/plottah/plots/DistPlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/plottah/plots/PlotProtocol.py` & `plottah-0.1.9/plottah/plots/PlotProtocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def get_y_axes_layout(self, row: int, col: int) -> dict:
         ...
 
     def get_annotations(self, ref: str) -> List[dict]:
         ...
 
-    def get_secondary_y_axis_title(self) -> str | None:
+    def get_secondary_y_axis_title(self):
         return None
 
     def show_plot(self, show_figure: bool = True) -> go.Figure:
         # create figure with single graph
         figure = make_subplots(rows=1, cols=1, specs=[[{"secondary_y": True}]])
         row, col = 1, 1
```

### Comparing `plottah-0.1.8/plottah/plots/RocCurvePlot.py` & `plottah-0.1.9/plottah/plots/RocCurvePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/plottah/utils.py` & `plottah-0.1.9/plottah/utils.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.8/pyproject.toml` & `plottah-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plottah"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Niels Ota"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pre-commit = "^3.3.3"
```

### Comparing `plottah-0.1.8/PKG-INFO` & `plottah-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plottah
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Niels Ota
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

