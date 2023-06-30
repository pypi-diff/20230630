# Comparing `tmp/wbpFonttools-0.2.0.tar.gz` & `tmp/wbpFonttools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpFonttools-0.2.0.tar", last modified: Mon Jun 12 15:12:31 2023, max compression
+gzip compressed data, was "wbpFonttools-0.2.1.tar", last modified: Fri Jun 30 15:19:25 2023, max compression
```

## Comparing `wbpFonttools-0.2.0.tar` & `wbpFonttools-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:12:31.855611 wbpFonttools-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:12:31.852611 wbpFonttools-0.2.0/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:12:31.854611 wbpFonttools-0.2.0/Lib/wbpFonttools/
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4895 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6779 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/control.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3730 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/selectFontsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3277 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/template.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2332 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/view.py
--rw-rw-rw-   0 root         (0) root         (0)    12103 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/window.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/windowUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:12:31.855611 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      594 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-12 15:12:31.856611 wbpFonttools-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-06-12 15:12:31.856611 wbpFonttools-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:19:25.712499 wbpFonttools-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:19:25.707499 wbpFonttools-0.2.1/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:19:25.710499 wbpFonttools-0.2.1/Lib/wbpFonttools/
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4895 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6779 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/control.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/selectFontsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3277 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2332 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    12100 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/window.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/Lib/wbpFonttools/windowUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:19:25.711499 wbpFonttools-0.2.1/Lib/wbpFonttools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-30 15:19:25.000000 wbpFonttools-0.2.1/Lib/wbpFonttools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      594 2023-06-30 15:19:25.000000 wbpFonttools-0.2.1/Lib/wbpFonttools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 15:19:25.000000 wbpFonttools-0.2.1/Lib/wbpFonttools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-30 15:19:25.000000 wbpFonttools-0.2.1/Lib/wbpFonttools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-30 15:19:25.000000 wbpFonttools-0.2.1/Lib/wbpFonttools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 15:19:25.000000 wbpFonttools-0.2.1/Lib/wbpFonttools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-30 15:19:25.712499 wbpFonttools-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-30 15:19:25.712499 wbpFonttools-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-30 15:19:24.000000 wbpFonttools-0.2.1/setup.py
```

### Comparing `wbpFonttools-0.2.0/LICENSE` & `wbpFonttools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/__init__.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     WebFont_WOFF_2_Template,
     WebFont_WOFF_Template,
 )
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 def CurrentFont() -> Optional[TTFont]:
     """
     Get the currently active font
     """
     app: App = wx.GetApp()
```

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/config.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/config.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/control.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/control.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/dialog.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/dialog.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/document.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/document.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/selectFontsDialogUI.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/selectFontsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/template.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/template.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/tools.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         tableClass = getTableClass(tableTag)
         if tableClass is None:
             tableClass = DefaultTable
         self.table = tableClass(tableTag)
         self.font[tableTag] = self.table
         self.contentStack.append([])
         self.stackSize = 1
-        parser = ParserCreate("latin1")
+        parser = ParserCreate()
         parser.StartElementHandler = self.startElementHandler
         parser.EndElementHandler = self.endElementHandler
         parser.CharacterDataHandler = self.characterDataHandler
         parser.Parse(tableData, True)
 
     def startElementHandler(self, name, attrs):
         stackSize = self.stackSize
```

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/view.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/view.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/window.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         wx.EndBusyCursor()
 
     def compileTable(self, tableTag:str) -> bool:
         font = self.font
         self.tableParser.font = font
         tableSave = font[tableTag]
         try:
-            self.tableParser.parse(self.textEditor.TextRaw, tableTag)
+            self.tableParser.parse(self.textEditor.Text, tableTag)
             table = font[tableTag]
             table.decompile(table.compile(font), font)
             return True
         except:
             traceback.print_exc()  # for debugging purposes
             wx.LogError(
                 "Compiling of table %s failed!\n%s\nSee full traceback in Output panel"
```

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools/windowUI.py` & `wbpFonttools-0.2.1/Lib/wbpFonttools/windowUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/PKG-INFO` & `wbpFonttools-0.2.1/Lib/wbpFonttools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.2.0
+Version: 0.2.1
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
```

### Comparing `wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/SOURCES.txt` & `wbpFonttools-0.2.1/Lib/wbpFonttools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/PKG-INFO` & `wbpFonttools-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.2.0
+Version: 0.2.1
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
```

### Comparing `wbpFonttools-0.2.0/README.md` & `wbpFonttools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.0/setup.cfg` & `wbpFonttools-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -53,16 +53,16 @@
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	wbBase>=0.2
-	fonttools[ufo,lxml,woff,unicode,interpolatable,plot,symfont]>=4.39.4
+	wbBase>=0.2.2
+	fonttools[ufo,lxml,woff,unicode,interpolatable,plot,symfont]>=4.40.0
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = fonttools = wbpFonttools
```

