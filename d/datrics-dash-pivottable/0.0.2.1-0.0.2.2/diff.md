# Comparing `tmp/datrics_dash_pivottable-0.0.2.1.tar.gz` & `tmp/datrics_dash_pivottable-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datrics_dash_pivottable-0.0.2.1.tar", last modified: Thu Jun 29 18:03:57 2023, max compression
+gzip compressed data, was "datrics_dash_pivottable-0.0.2.2.tar", last modified: Fri Jun 30 12:11:01 2023, max compression
```

## Comparing `datrics_dash_pivottable-0.0.2.1.tar` & `datrics_dash_pivottable-0.0.2.2.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 henprokuror   (501) staff       (20)        0 2023-06-29 18:03:57.300772 datrics_dash_pivottable-0.0.2.1/
--rw-r--r--   0 henprokuror   (501) staff       (20)     1067 2023-06-29 15:59:40.000000 datrics_dash_pivottable-0.0.2.1/LICENSE
--rw-r--r--   0 henprokuror   (501) staff       (20)      187 2023-06-29 15:59:40.000000 datrics_dash_pivottable-0.0.2.1/MANIFEST.in
--rw-r--r--   0 henprokuror   (501) staff       (20)      208 2023-06-29 18:03:57.300627 datrics_dash_pivottable-0.0.2.1/PKG-INFO
--rw-r--r--   0 henprokuror   (501) staff       (20)     3575 2023-06-29 17:36:13.000000 datrics_dash_pivottable-0.0.2.1/README.md
-drwxr-xr-x   0 henprokuror   (501) staff       (20)        0 2023-06-29 18:03:57.299613 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable/
--rw-r--r--   0 henprokuror   (501) staff       (20)     4633 2023-06-29 17:36:13.000000 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable/PivotTable.py
--rw-r--r--   0 henprokuror   (501) staff       (20)     1147 2023-06-29 15:59:40.000000 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable/__init__.py
--rw-r--r--   0 henprokuror   (501) staff       (20)       66 2023-06-29 15:59:40.000000 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable/_imports_.py
-drwxr-xr-x   0 henprokuror   (501) staff       (20)        0 2023-06-29 18:03:57.300399 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable.egg-info/
--rw-r--r--   0 henprokuror   (501) staff       (20)      208 2023-06-29 18:03:57.000000 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable.egg-info/PKG-INFO
--rw-r--r--   0 henprokuror   (501) staff       (20)      383 2023-06-29 18:03:57.000000 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable.egg-info/SOURCES.txt
--rw-r--r--   0 henprokuror   (501) staff       (20)        1 2023-06-29 18:03:57.000000 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable.egg-info/dependency_links.txt
--rw-r--r--   0 henprokuror   (501) staff       (20)        5 2023-06-29 18:03:57.000000 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable.egg-info/requires.txt
--rw-r--r--   0 henprokuror   (501) staff       (20)       24 2023-06-29 18:03:57.000000 datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable.egg-info/top_level.txt
--rw-r--r--   0 henprokuror   (501) staff       (20)       38 2023-06-29 18:03:57.300822 datrics_dash_pivottable-0.0.2.1/setup.cfg
--rw-r--r--   0 henprokuror   (501) staff       (20)      544 2023-06-29 17:59:32.000000 datrics_dash_pivottable-0.0.2.1/setup.py
+drwxr-xr-x   0 henprokuror   (501) staff       (20)        0 2023-06-30 12:11:01.516125 datrics_dash_pivottable-0.0.2.2/
+-rw-r--r--   0 henprokuror   (501) staff       (20)     1067 2023-06-29 15:59:40.000000 datrics_dash_pivottable-0.0.2.2/LICENSE
+-rw-r--r--   0 henprokuror   (501) staff       (20)      187 2023-06-29 15:59:40.000000 datrics_dash_pivottable-0.0.2.2/MANIFEST.in
+-rw-r--r--   0 henprokuror   (501) staff       (20)      208 2023-06-30 12:11:01.515916 datrics_dash_pivottable-0.0.2.2/PKG-INFO
+-rw-r--r--   0 henprokuror   (501) staff       (20)     3575 2023-06-29 17:36:13.000000 datrics_dash_pivottable-0.0.2.2/README.md
+drwxr-xr-x   0 henprokuror   (501) staff       (20)        0 2023-06-30 12:11:01.513108 datrics_dash_pivottable-0.0.2.2/dash_pivottable/
+-rw-r--r--   0 henprokuror   (501) staff       (20) 20503101 2023-06-30 11:42:50.000000 datrics_dash_pivottable-0.0.2.2/dash_pivottable/dash_pivottable.dev.js
+-rw-r--r--   0 henprokuror   (501) staff       (20)  3548617 2023-06-30 11:42:48.000000 datrics_dash_pivottable-0.0.2.2/dash_pivottable/dash_pivottable.min.js
+-rw-r--r--   0 henprokuror   (501) staff       (20)     5652 2023-06-30 11:42:52.000000 datrics_dash_pivottable-0.0.2.2/dash_pivottable/metadata.json
+-rw-r--r--   0 henprokuror   (501) staff       (20)     2030 2023-06-30 11:42:52.000000 datrics_dash_pivottable-0.0.2.2/dash_pivottable/package.json
+drwxr-xr-x   0 henprokuror   (501) staff       (20)        0 2023-06-30 12:11:01.514174 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable/
+-rw-r--r--   0 henprokuror   (501) staff       (20)     4641 2023-06-30 12:10:37.000000 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable/PivotTable.py
+-rw-r--r--   0 henprokuror   (501) staff       (20)     1163 2023-06-30 12:01:49.000000 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable/__init__.py
+-rw-r--r--   0 henprokuror   (501) staff       (20)       66 2023-06-30 12:10:37.000000 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable/_imports_.py
+drwxr-xr-x   0 henprokuror   (501) staff       (20)        0 2023-06-30 12:11:01.515127 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable.egg-info/
+-rw-r--r--   0 henprokuror   (501) staff       (20)      208 2023-06-30 12:11:01.000000 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable.egg-info/PKG-INFO
+-rw-r--r--   0 henprokuror   (501) staff       (20)      564 2023-06-30 12:11:01.000000 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable.egg-info/SOURCES.txt
+-rw-r--r--   0 henprokuror   (501) staff       (20)        1 2023-06-30 12:11:01.000000 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable.egg-info/dependency_links.txt
+-rw-r--r--   0 henprokuror   (501) staff       (20)        5 2023-06-30 12:11:01.000000 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable.egg-info/requires.txt
+-rw-r--r--   0 henprokuror   (501) staff       (20)       24 2023-06-30 12:11:01.000000 datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable.egg-info/top_level.txt
+-rw-r--r--   0 henprokuror   (501) staff       (20)       38 2023-06-30 12:11:01.516182 datrics_dash_pivottable-0.0.2.2/setup.cfg
+-rw-r--r--   0 henprokuror   (501) staff       (20)      544 2023-06-30 12:09:59.000000 datrics_dash_pivottable-0.0.2.2/setup.py
+drwxr-xr-x   0 henprokuror   (501) staff       (20)        0 2023-06-30 12:11:01.515462 datrics_dash_pivottable-0.0.2.2/tests/
+-rw-r--r--   0 henprokuror   (501) staff       (20)      927 2023-06-29 17:36:13.000000 datrics_dash_pivottable-0.0.2.2/tests/test_callbacks.py
+-rw-r--r--   0 henprokuror   (501) staff       (20)      294 2023-06-29 15:59:41.000000 datrics_dash_pivottable-0.0.2.2/tests/test_percy.py
```

### Comparing `datrics_dash_pivottable-0.0.2.1/LICENSE` & `datrics_dash_pivottable-0.0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datrics_dash_pivottable-0.0.2.1/README.md` & `datrics_dash_pivottable-0.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable/PivotTable.py` & `datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable/PivotTable.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 - valueFilter (dict; optional): Value filter for each attribute name.
 - rendererName (string; optional): Which renderer is currently selected. E.g. Table, Line Chart, Scatter
 Chart, etc."""
     @_explicitize_args
     def __init__(self, id=Component.UNDEFINED, data=Component.UNDEFINED, hiddenAttributes=Component.UNDEFINED, hiddenFromAggregators=Component.UNDEFINED, hiddenFromDragDrop=Component.UNDEFINED, menuLimit=Component.UNDEFINED, unusedOrientationCutoff=Component.UNDEFINED, cols=Component.UNDEFINED, colOrder=Component.UNDEFINED, rows=Component.UNDEFINED, rowOrder=Component.UNDEFINED, aggregatorName=Component.UNDEFINED, vals=Component.UNDEFINED, valueFilter=Component.UNDEFINED, rendererName=Component.UNDEFINED, **kwargs):
         self._prop_names = ['id', 'data', 'hiddenAttributes', 'hiddenFromAggregators', 'hiddenFromDragDrop', 'menuLimit', 'unusedOrientationCutoff', 'cols', 'colOrder', 'rows', 'rowOrder', 'aggregatorName', 'vals', 'valueFilter', 'rendererName']
         self._type = 'PivotTable'
-        self._namespace = 'dash_pivottable'
+        self._namespace = 'datrics_dash_pivottable'
         self._valid_wildcard_attributes =            []
         self.available_properties = ['id', 'data', 'hiddenAttributes', 'hiddenFromAggregators', 'hiddenFromDragDrop', 'menuLimit', 'unusedOrientationCutoff', 'cols', 'colOrder', 'rows', 'rowOrder', 'aggregatorName', 'vals', 'valueFilter', 'rendererName']
         self.available_wildcard_properties =            []
 
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs
```

### Comparing `datrics_dash_pivottable-0.0.2.1/datrics_dash_pivottable/__init__.py` & `datrics_dash_pivottable-0.0.2.2/datrics_dash_pivottable/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 _current_path = _os.path.dirname(_os.path.abspath(__file__))
 
 _this_module = _sys.modules[__name__]
 
 
 _js_dist = [
     {
-        'relative_package_path': 'dash_pivottable.min.js',
-        'dev_package_path': 'dash_pivottable.dev.js',
+        'relative_package_path': 'datrics_dash_pivottable.min.js',
+        'dev_package_path': 'datrics_dash_pivottable.dev.js',
         
         'namespace': package_name
     }
 ]
 
 _css_dist = []
```

### Comparing `datrics_dash_pivottable-0.0.2.1/setup.py` & `datrics_dash_pivottable-0.0.2.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     package = json.load(f)
 
 package_name = package["name"].replace(" ", "_").replace("-", "_")
 
 setup(
     name = 'datrics_dash_pivottable',
     description = 'Fixed version of the dash_pivottable=0.0.2',
-    version = '0.0.2.1',
+    version = '0.0.2.2',
     author='Roman Malkevych',
     author_email='rm@datrics.ai',
     packages=[package_name],
     include_package_data=True,
     license=package['license'],
     install_requires=['dash']
 )
```

