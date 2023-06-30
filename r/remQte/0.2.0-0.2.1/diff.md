# Comparing `tmp/remqte-0.2.0.tar.gz` & `tmp/remqte-0.2.1.tar.gz`

## Comparing `remqte-0.2.0.tar` & `remqte-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 remqte-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/__init__.py
--rw-r--r--   0        0        0    22253 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/remQte.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/docs/img/icon.png
--rw-r--r--   0        0        0    19542 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/docs/img/screenshot.png
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/qtui/importcsv_s1.ui
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/qtui/importcsv_s2.ui
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/qtui/importcsv_s3.ui
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/qtui/main_scan_choose_nets.ui
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/qtui/main_scan_nets.ui
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/qtui/main_start.ui
--rw-r--r--   0        0        0    36659 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/qtui/remote.ui
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/resources/__init__.py
--rw-r--r--   0        0        0    84777 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/resources/images.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/resources/importzip.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/resources/icon/icon16x16.png
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/resources/icon/icon24x24.png
--rw-r--r--   0        0        0    23129 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/resources/icon/icon256x256.png
--rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/resources/icon/icon32x32.png
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 remqte-0.2.0/src/remQte/resources/icon/icon48x48.png
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 remqte-0.2.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 remqte-0.2.0/LICENSE
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 remqte-0.2.0/README.md
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 remqte-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 remqte-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 remqte-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/__init__.py
+-rw-r--r--   0        0        0    22840 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/remQte.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/docs/img/icon.ico
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/docs/img/icon.png
+-rw-r--r--   0        0        0    19542 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/docs/img/screenshot.png
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/qtui/importcsv_s1.ui
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/qtui/importcsv_s2.ui
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/qtui/importcsv_s3.ui
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/qtui/main_scan_choose_nets.ui
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/qtui/main_scan_nets.ui
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/qtui/main_start.ui
+-rw-r--r--   0        0        0    36659 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/qtui/remote.ui
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/resources/__init__.py
+-rw-r--r--   0        0        0    84777 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/resources/images.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/resources/importzip.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/resources/icon/icon16x16.png
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/resources/icon/icon24x24.png
+-rw-r--r--   0        0        0    23129 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/resources/icon/icon256x256.png
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/resources/icon/icon32x32.png
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 remqte-0.2.1/src/remQte/resources/icon/icon48x48.png
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 remqte-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 remqte-0.2.1/LICENSE
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 remqte-0.2.1/README.md
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 remqte-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 remqte-0.2.1/PKG-INFO
```

### Comparing `remqte-0.2.0/CODE_OF_CONDUCT.md` & `remqte-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/remQte.py` & `remqte-0.2.1/src/remQte/remQte.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,15 +521,15 @@
             self.btnimportchannels.setVisible(False)
         for i in ini_chn.sections():
             
             self.comboBox.addItem("%s %s"%(ini_chn[i]['type'].upper(), ini_chn[i]['name']), userData=i)
         #s.comboBox.currentIndexChanged.connect(s.pr)
     def remote(s):
         uic.loadUi(pth("/qtui/remote.ui"),s)
-        s.setWindowIcon(gimg('icon').get())
+        #s.setWindowIcon(gimg('icon').get())
         s.btnpwr.clicked.connect(stv.pwr)
         s.btnpwr.setIcon(gimg('pwr').get())
         s.btnsmarthub.clicked.connect(stv.smarthub)
         s.btnsrc.clicked.connect(stv.source)
         s.btnchup.clicked.connect(stv.chup)
         s.btnchup.setIcon(gimg('chup').get())
         s.btnchdw.clicked.connect(stv.chdw)
@@ -621,16 +621,27 @@
         self.args = args
         self.kwargs = kwargs
     def __call__(self,event):
         self.func(event,*self.args, **self.kwargs)
 def startapp():
     global app, window
     initconfigs()
+    if sys.platform.startswith('win'):
+        import ctypes
+        myappid = u'phnoe.remQte.remQte.0.2' # arbitrary string
+        ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
     app = QApplication([])
-    app.setWindowIcon(gimg('icon').get())
+    app_icn = QIcon()
+
+    app_icn.addFile(pth('/resources/icon/icon16x16.png'),QSize(16,16))
+    app_icn.addFile(pth('/resources/icon/icon24x24.png'),QSize(24,24))
+    app_icn.addFile(pth('/resources/icon/icon32x32.png'),QSize(32,32))
+    app_icn.addFile(pth('/resources/icon/icon48x48.png'),QSize(48,48))
+    app_icn.addFile(pth('/resources/icon/icon256x256.png'),QSize(256,256))
     window = MainWindow()
+    app.setWindowIcon(app_icn)
     t = QTimer()
     t.singleShot(1000,window.start)
     sys.exit(app.exec())
 
 if __name__ == '__main__':
     startapp()
```

### Comparing `remqte-0.2.0/src/remQte/docs/img/screenshot.png` & `remqte-0.2.1/src/remQte/docs/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/qtui/importcsv_s1.ui` & `remqte-0.2.1/src/remQte/qtui/importcsv_s1.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/qtui/importcsv_s2.ui` & `remqte-0.2.1/src/remQte/qtui/importcsv_s2.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/qtui/importcsv_s3.ui` & `remqte-0.2.1/src/remQte/qtui/importcsv_s3.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/qtui/main_scan_choose_nets.ui` & `remqte-0.2.1/src/remQte/qtui/main_scan_choose_nets.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/qtui/main_scan_nets.ui` & `remqte-0.2.1/src/remQte/qtui/main_scan_nets.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/qtui/main_start.ui` & `remqte-0.2.1/src/remQte/qtui/main_start.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/qtui/remote.ui` & `remqte-0.2.1/src/remQte/qtui/remote.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/resources/images.py` & `remqte-0.2.1/src/remQte/resources/images.py`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/resources/importzip.py` & `remqte-0.2.1/src/remQte/resources/importzip.py`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/resources/icon/icon16x16.png` & `remqte-0.2.1/src/remQte/resources/icon/icon16x16.png`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/resources/icon/icon24x24.png` & `remqte-0.2.1/src/remQte/resources/icon/icon24x24.png`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/resources/icon/icon256x256.png` & `remqte-0.2.1/src/remQte/resources/icon/icon256x256.png`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/resources/icon/icon32x32.png` & `remqte-0.2.1/src/remQte/resources/icon/icon32x32.png`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/src/remQte/resources/icon/icon48x48.png` & `remqte-0.2.1/src/remQte/resources/icon/icon48x48.png`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/LICENSE` & `remqte-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/README.md` & `remqte-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `remqte-0.2.0/pyproject.toml` & `remqte-0.2.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "remQte"
-version = "0.2.0"
+version = "0.2.1"
 authors = [{ name="Philipp M. Nöhren", email="remQte@proton.me" }]
 description = "Remote-control GUI for Samsung Smart TVs, newer than 2016."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: End Users/Desktop",
@@ -19,14 +19,15 @@
 dependencies = [
 	"samsungtvws",
 	"wakeonlan",
 	"PyQt6",
 	"netifaces",
 	"ssdpy"
 ]
+#icon = "src/remQte/docs/img/icon"
 [project.urls]
 "Homepage" = "https://github.com/barfnordsen/remQte"
 "Bug Tracker" = "https://github.com/barfnordsen/remQte/issues"
 [project.gui-scripts]
 remQte = "remQte.remQte:startapp"
 [tool.hatch.build] 
 exclude = [
```

### Comparing `remqte-0.2.0/PKG-INFO` & `remqte-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remQte
-Version: 0.2.0
+Version: 0.2.1
 Summary: Remote-control GUI for Samsung Smart TVs, newer than 2016.
 Project-URL: Homepage, https://github.com/barfnordsen/remQte
 Project-URL: Bug Tracker, https://github.com/barfnordsen/remQte/issues
 Author-email: "Philipp M. Nöhren" <remQte@proton.me>
 License-File: LICENSE
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

