# Comparing `tmp/wbBase-0.2.0.tar.gz` & `tmp/wbBase-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbBase-0.2.0.tar", last modified: Mon Jun 12 09:36:34 2023, max compression
+gzip compressed data, was "wbBase-0.2.2.tar", last modified: Fri Jun 30 13:31:43 2023, max compression
```

## Comparing `wbBase-0.2.0.tar` & `wbBase-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.919423 wbBase-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-12 09:36:33.000000 wbBase-0.2.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.912423 wbBase-0.2.0/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.915423 wbBase-0.2.0/Lib/wbBase/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23696 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/application.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/applicationInfo.py
--rw-rw-rw-   0 root         (0) root         (0)    20622 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/applicationWindow.py
--rw-rw-rw-   0 root         (0) root         (0)   309800 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/artprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.917423 wbBase-0.2.0/Lib/wbBase/control/
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/externalToolConfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/externalToolConfigUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/filling.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/iePanel.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/propgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    47198 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/textEditControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.918423 wbBase-0.2.0/Lib/wbBase/dialog/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2342 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/dialog/multiSaveModifiedDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    20381 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/dialog/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.919423 wbBase-0.2.0/Lib/wbBase/document/
--rw-rw-rw-   0 root         (0) root         (0)    23492 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36912 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     8016 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/template.py
--rw-rw-rw-   0 root         (0) root         (0)     9208 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/view.py
--rw-rw-rw-   0 root         (0) root         (0)    21455 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/panelManager.py
--rw-rw-rw-   0 root         (0) root         (0)     3366 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/pluginManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/pluginManager_old.py
--rw-rw-rw-   0 root         (0) root         (0)     8814 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/scripting.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.916423 wbBase-0.2.0/Lib/wbBase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2751 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1027 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2751 2023-06-12 09:36:34.919423 wbBase-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-06-12 09:36:33.000000 wbBase-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2032 2023-06-12 09:36:34.920423 wbBase-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 09:36:33.000000 wbBase-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.669727 wbBase-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-30 13:31:42.000000 wbBase-0.2.2/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.663727 wbBase-0.2.2/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.666727 wbBase-0.2.2/Lib/wbBase/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25590 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/applicationInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)    20784 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/applicationWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)   309861 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/artprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.668727 wbBase-0.2.2/Lib/wbBase/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/externalToolConfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/externalToolConfigUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/iePanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/propgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    47198 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/textEditControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.668727 wbBase-0.2.2/Lib/wbBase/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/dialog/multiSaveModifiedDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    20381 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/dialog/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.669727 wbBase-0.2.2/Lib/wbBase/document/
+-rw-rw-rw-   0 root         (0) root         (0)    23492 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36912 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     8016 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     9208 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    22086 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/panelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3362 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/pluginManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/pluginManager_old.py
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/scripting.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.666727 wbBase-0.2.2/Lib/wbBase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-06-30 13:31:43.669727 wbBase-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2023-06-30 13:31:42.000000 wbBase-0.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-06-30 13:31:43.670727 wbBase-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-30 13:31:42.000000 wbBase-0.2.2/setup.py
```

### Comparing `wbBase-0.2.0/LICENSE` & `wbBase-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/application.py` & `wbBase-0.2.2/Lib/wbBase/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from io import BytesIO
 from typing import TYPE_CHECKING, ClassVar, List, Optional, Union
 
 import wx
 from wx.adv import (
     SPLASH_CENTER_ON_SCREEN,
     SPLASH_NO_TIMEOUT,
+    ShowTip,
     SplashScreen,
+    TipProvider,
 )
 
 from .applicationInfo import ApplicationInfo
 from .applicationWindow import ApplicationWindow
 from .artprovider import Artprovider
 from .document import DOC_SILENT
 from .pluginManager import PluginManager
@@ -98,43 +100,81 @@
                 if os.path.exists(arg):
                     topWin.documentManager.CreateDocument(arg, DOC_SILENT)
             topWin.RequestUserAttention()
         self.Start(200)
 
 
 class AppSplashScreen(SplashScreen):
+    """
+    Window with a thin border, displaying a bitmap describing the application.
+    Shown in application initialization.
+    """
     def __init__(
         self,
         bitmap: wx.Bitmap,
         splashStyle: int,
         milliseconds: int,
-        parent: wx.Frame,
         id: int = wx.ID_ANY,
         pos: wx.Point = wx.DefaultPosition,
         size: wx.Size = wx.DefaultSize,
         style: int = wx.BORDER_SIMPLE | wx.FRAME_NO_TASKBAR | wx.STAY_ON_TOP,
     ):
         super().__init__(
-            bitmap, splashStyle, milliseconds, parent, id, pos, size, style
+            bitmap, splashStyle, milliseconds, None, id, pos, size, style
         )
         position = wx.Point(0, bitmap.Height - 20)
         size = wx.Size(bitmap.Width, 20)
         self.message = wx.StaticText(
             self,
             wx.ID_ANY,
             "Loading App ...",
             position,
             size,
             wx.ALIGN_CENTER_HORIZONTAL | wx.ST_ELLIPSIZE_MIDDLE | wx.TRANSPARENT_WINDOW,
         )
 
-    def setMessage(self, text:str) -> None:
+    def setMessage(self, text: str) -> None:
         self.message.SetLabel(text)
 
 
+class ResourceTipProvider(TipProvider):
+    """
+    TipProvider with tips loaded from application resources.
+    """
+    def __init__(self, currentTip:int):
+        super().__init__(currentTip)
+        self._currentTyp = currentTip
+        self.tips:List[str] = []
+        tips = self.app.getResource("tips.txt")
+        if isinstance(tips, str):
+            self.tips = tips.splitlines()
+
+    @property
+    def app(self) -> App:
+        """
+        The running Workbench application.
+        """
+        return wx.GetApp()
+
+    @property
+    def hasTips(self) -> bool:
+        """True is any tips are available."""
+        return len(self.tips) > 0
+
+    def GetCurrentTip(self) -> int:
+        return self._currentTyp
+
+    def GetTip(self) -> str:
+        tip = self.tips[self._currentTyp]
+        self._currentTyp += 1
+        if self._currentTyp >= len(self.tips) -1:
+            self._currentTyp = 0
+        return tip
+    
+
 class App(wx.App):
     """
     Implements the main application object
     """
 
     # modes for external changes test
     EXT_CHANGE_TEST_ON_REQUEST: ClassVar[int] = 0
@@ -291,37 +331,59 @@
                     y = round(cfg.ReadInt("y", -1) + (height - bmp.Height) / 2)
                     pos = wx.Point(x, y)
                     # size = wx.Size(cfg.ReadInt("width", -1), cfg.ReadInt("height", -1))
                     splashScreen = AppSplashScreen(
                         bitmap=bmp,
                         splashStyle=SPLASH_NO_TIMEOUT,
                         milliseconds=1000,
-                        parent=None,
+                        # parent=None,
                         id=wx.ID_ANY,
                         pos=pos,
                         size=wx.DefaultSize,
                     )
                     splashScreen.SetPosition(pos)
                     return splashScreen
         return AppSplashScreen(
-            bmp, SPLASH_CENTER_ON_SCREEN | SPLASH_NO_TIMEOUT, 1000, None
+            bmp, SPLASH_CENTER_ON_SCREEN | SPLASH_NO_TIMEOUT, 1000
         )
 
     def _execFirstRunScript(self):
+        """
+        Execute firstRun.py when application runns for the first time
+        """
         if self.test:
             return
         cfg = self.config
         if cfg.ReadBool("/Application/firstRunDone", False):
             return
         scriptName = "firstRun.py"
         firstRunCode = self.getResource(scriptName)
         if firstRunCode:
             execsource(firstRunCode, scriptName)
         cfg.WriteBool("/Application/firstRunDone", True)
 
+    def _showTipOfTheDay(self):
+        """
+        Show Tip of the day dialog.
+        """
+        if self.test:
+            return
+        cfg = self.config
+        with wx.ConfigPathChanger(cfg, "/Application/Start/"):
+            showTipOfTheDay = cfg.ReadBool("showTipOfTheDay", True)
+            if not showTipOfTheDay:
+                return
+            currentTip = cfg.ReadInt("currentTipOfTheDay", 0)
+            tipProvider = ResourceTipProvider(currentTip)
+            if not tipProvider.hasTips:
+                return
+            showTipOfTheDay = ShowTip(self.TopWindow, tipProvider, showTipOfTheDay)
+            cfg.WriteBool("showTipOfTheDay", showTipOfTheDay)
+            cfg.WriteBool("currentTipOfTheDay", tipProvider.GetCurrentTip())
+
     # =========================================================================
     # Public methods
     # =========================================================================
 
     def OnPreInit(self) -> None:
         wx.App.OnPreInit(self)
         self.globalObjects = [
@@ -363,23 +425,26 @@
     def OnRun(self) -> int:
         """
         Run the application
 
             - Show the main application window
             - handle command line arguments
             - close the splash screen
+            - show tip of the day
             - enter the main application event loop
 
         :return: Return code
         """
         self.TopWindow.Show(True)
         self._handleCmdLineArguments()
         if self._splashScreen:
+            self._splashScreen.Hide()
             self._splashScreen.Destroy()
             self._splashScreen = None
+        self._showTipOfTheDay()
         main = sys.modules.get("__main__")
         if "main" in main.__dict__:
             del main.__dict__["main"]
         return super().OnRun()
 
     def run(self) -> int:
         """
@@ -562,42 +627,42 @@
         defaultFolder = os.path.join(
             self.Traits.StandardPaths.UserLocalDataDir, "shared"
         )
         with wx.ConfigPathChanger(cfg, "/Application/SharedData/"):
             folder = cfg.Read("Dir", defaultFolder)
             url = cfg.Read("URL", "")
             pull_on_start = cfg.ReadBool("PullOnStart", False)
-            if folder:
-                if not os.path.isdir(folder) and not self.test:
-                    try:
-                        os.makedirs(folder)
-                    except PermissionError:
-                        folder = ""
-                self.sharedDataDir = folder
-            if has_git and url and folder:
+        if folder:
+            if not os.path.isdir(folder) and not self.test:
                 try:
-                    repo = Repo(folder)
-                except InvalidGitRepositoryError:
-                    repo = Repo.init(folder)
-                if not repo.remotes:
+                    os.makedirs(folder)
+                except PermissionError:
+                    folder = ""
+            self.sharedDataDir = folder
+        if has_git and url and folder:
+            try:
+                repo = Repo(folder)
+            except InvalidGitRepositoryError:
+                repo = Repo.init(folder)
+            if not repo.remotes:
+                remote = repo.create_remote("origin", url)
+            else:
+                try:
+                    remote = repo.remote(name="origin")
+                except ValueError:
                     remote = repo.create_remote("origin", url)
-                else:
-                    try:
-                        remote = repo.remote(name="origin")
-                    except ValueError:
-                        remote = repo.create_remote("origin", url)
-                urls = [u for u in remote.urls]
-                old_url = None
-                if url not in urls:
-                    if len(urls) == 1:
-                        old_url = urls[0]
-                    remote.set_url(url, old_url)
-                if pull_on_start:
-                    self.splashMessage("Pulling shared data")
-                    self.pullSharedData()
+            urls = [u for u in remote.urls]
+            old_url = None
+            if url not in urls:
+                if len(urls) == 1:
+                    old_url = urls[0]
+                remote.set_url(url, old_url)
+            if pull_on_start:
+                self.splashMessage("Pulling shared data")
+                self.pullSharedData()
 
     def pullSharedData(self) -> None:
         if self.test:
             return
         if has_git:
             if self.sharedDataDir:
                 try:
@@ -622,17 +687,17 @@
         self.splashMessage("Preparing private data folder")
         cfg = self.config
         defaultFolder = os.path.join(
             self.Traits.StandardPaths.UserLocalDataDir, "private"
         )
         with wx.ConfigPathChanger(cfg, "/Application/PrivateData/"):
             folder = cfg.Read("Dir", defaultFolder)
-            if not os.path.isdir(folder) and not self.test:
-                os.makedirs(folder)
-            self.privateDataDir = folder
+        if not os.path.isdir(folder) and not self.test:
+            os.makedirs(folder)
+        self.privateDataDir = folder
 
     def MacOpenFiles(self, fileNames) -> None:
         for filename in fileNames:
             self.documentManager.CreateDocument(filename, DOC_SILENT)
 
     # def MacNewFile(self):
     #     docManager = self.documentManager
```

### Comparing `wbBase-0.2.0/Lib/wbBase/applicationInfo.py` & `wbBase-0.2.2/Lib/wbBase/applicationInfo.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/applicationWindow.py` & `wbBase-0.2.2/Lib/wbBase/applicationWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """
 
     panelManagerClass: ClassVar[type[PanelManager]] = PanelManager
     documentManagerClass: ClassVar[type[DocumentManager]] = DocumentManager
 
     MenuBar: wx.MenuBar
 
-    def __init__(self, iconName:str=""):
+    def __init__(self, iconName: str = ""):
         self._toolbarEdit: Optional[aui.AuiToolBar] = None
         self._showTooltip: bool = False
         app: App = wx.GetApp()
         wx.Frame.__init__(
             self,
             parent=None,
             id=wx.ID_ANY,
@@ -183,15 +183,16 @@
                 wx.ID_ANY,
                 wx.DefaultPosition,
                 wx.DefaultSize,
                 aui.AUI_TB_HORZ_LAYOUT | aui.AUI_TB_PLAIN_BACKGROUND | wx.NO_BORDER,
             )
             tb.SetName("Edit")
             tb.SetToolBitmapSize(wx.Size(16, 16))
-            lastItem = menu.MenuItems[0]
+            lastItem: wx.MenuItem = menu.MenuItems[0]
+            item: wx.MenuItem
             for item in menu.MenuItems:
                 if item.IsSeparator() and not lastItem.IsSeparator():
                     pass
                 elif item.IsSubMenu():
                     continue
                 elif item.Bitmap.IsOk() and item.Id != wx.ID_EXIT:
                     if lastItem.IsSeparator():
@@ -249,33 +250,33 @@
 
         # copy/cut/paste
         mnu.AppendSeparator()
 
         item = menuItem(id=wx.ID_COPY)
         item.SetBitmap(getBitmap(wx.ART_COPY))
         mnu.Append(item)
-        
+
         item = menuItem(id=wx.ID_CUT)
         item.SetBitmap(getBitmap(wx.ART_CUT))
         mnu.Append(item)
-        
+
         item = menuItem(id=wx.ID_PASTE)
         item.SetBitmap(getBitmap(wx.ART_PASTE))
         mnu.Append(item)
 
         # select all
         mnu.AppendSeparator()
 
         item = menuItem(id=wx.ID_SELECTALL)
         item.SetBitmap(getBitmap("SELECT_ALL"))
         mnu.Append(item)
 
         # find/replace
         mnu.AppendSeparator()
-        
+
         item = menuItem(id=wx.ID_FIND)
         item.SetBitmap(getBitmap(wx.ART_FIND))
         mnu.Append(item)
 
         item = wx.MenuItem(mnu, wx.ID_ANY, "Find Next\tF3", "Find next", wx.ITEM_NORMAL)
         item.SetBitmap(getBitmap("FIND_NEXT"))
         mnu.Append(item)
@@ -353,27 +354,29 @@
             x = cfg.ReadInt("x", -1)
             y = cfg.ReadInt("y", -1)
             self.Position = (x, y)
             width = cfg.ReadInt("width", 800)
             height = cfg.ReadInt("height", 600)
             self.Size = (width, height)
             self.showTooltip = cfg.ReadBool("showTooltip", True)
+            self.StatusBar.Show(cfg.ReadBool("showStatusBar", True))
         with wx.ConfigPathChanger(cfg, "/Application/"):
             self._externalTools = eval(cfg.Read("ExternalTools", "[]"))
 
     def saveConfig(self) -> None:
         cfg = self.config
         with wx.ConfigPathChanger(cfg, "/Window/"):
             x, y = self.Position
             cfg.WriteInt("x", x)
             cfg.WriteInt("y", y)
             width, height = self.Size
             cfg.WriteInt("width", width)
             cfg.WriteInt("height", height)
             cfg.WriteBool("showTooltip", self.showTooltip)
+            cfg.WriteBool("showStatusBar", self.StatusBar.IsShown())
         self.panelManager.saveConfig()
 
     # -----------------------------------------------------------------------------
     # Event handler
     # -----------------------------------------------------------------------------
 
     def on_sys_colour_chnaged(self, event):
@@ -395,15 +398,15 @@
         cfg = self.app.config
         with wx.ConfigPathChanger(cfg, "/Window/Panels/"):
             setColour = self.panelManager.ArtProvider.SetColour
             for artColour in dockArtColours:
                 setColour(getattr(aui, artColour), wx.Colour(cfg.ReadInt(artColour)))
             self.panelManager.Update()
 
-    def on_resize(self, event:wx.SizeEvent) -> None:
+    def on_resize(self, event: wx.SizeEvent) -> None:
         self._panelManager.checkToolBars()
         event.Skip()
 
     def on_close(self, event: wx.CommandEvent):
         if self._documentManager.Clear():
             self.saveConfig()
             self._panelManager.UnInit()
@@ -537,15 +540,15 @@
 
     def on_edit_preferences(self, event: wx.CommandEvent):
         prefDlg: PreferencesDialog
         with PreferencesDialog(self) as prefDlg:
             prefDlg.ShowModal()
 
     def on_externalTool(self, event: wx.CommandEvent):
-        menuItem:wx.MenuItem = self.MenuBar.FindItemById(event.GetId())
+        menuItem: wx.MenuItem = self.MenuBar.FindItemById(event.GetId())
         for tool in self.externalTools:
             if tool["name"] == menuItem.ItemLabelText:
                 from .tools import startfile  # The wx.App object must be created first!
 
                 oldDir = os.getcwd()
                 if os.path.isdir(tool["folder"]):
                     os.chdir(tool["folder"])
```

### Comparing `wbBase-0.2.0/Lib/wbBase/artprovider.py` & `wbBase-0.2.2/Lib/wbBase/artprovider.py`

 * *Files 0% similar despite different names*

```diff
@@ -4397,16 +4397,19 @@
 			return itemSize[wx.ART_OTHER]
 		elif itemSize:
 			return list(itemSize.values())[0]
 
 
 class Artprovider(wx.ArtProvider):
 	def CreateBitmap(self, artId:str, client:str, size:wx.Size):
+		bitmap = wx.NullBitmap
 		data = getArtData(artId, client, size.width)
 		if data is None:
-			return wx.NullBitmap
+			return bitmap
+		if wx.GetApp() is None:
+			return bitmap
 		image = wx.Image(BytesIO(zlib.decompress(data)))
 		if artId.endswith(disabled):
 			bitmap = wx.Bitmap(image.ConvertToGreyscale())
 		else:
 			bitmap = wx.Bitmap(image)
 		return bitmap
```

### Comparing `wbBase-0.2.0/Lib/wbBase/control/__init__.py` & `wbBase-0.2.2/Lib/wbBase/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/control/externalToolConfig.py` & `wbBase-0.2.2/Lib/wbBase/control/externalToolConfig.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/control/externalToolConfigUI.py` & `wbBase-0.2.2/Lib/wbBase/control/externalToolConfigUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/control/filling.py` & `wbBase-0.2.2/Lib/wbBase/control/filling.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/control/iePanel.py` & `wbBase-0.2.2/Lib/wbBase/control/iePanel.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/control/propgrid.py` & `wbBase-0.2.2/Lib/wbBase/control/propgrid.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/control/textEditControl.py` & `wbBase-0.2.2/Lib/wbBase/control/textEditControl.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/dialog/multiSaveModifiedDialog.py` & `wbBase-0.2.2/Lib/wbBase/dialog/multiSaveModifiedDialog.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py` & `wbBase-0.2.2/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/dialog/preferences.py` & `wbBase-0.2.2/Lib/wbBase/dialog/preferences.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/document/__init__.py` & `wbBase-0.2.2/Lib/wbBase/document/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/document/manager.py` & `wbBase-0.2.2/Lib/wbBase/document/manager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/document/notebook.py` & `wbBase-0.2.2/Lib/wbBase/document/notebook.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/document/template.py` & `wbBase-0.2.2/Lib/wbBase/document/template.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/document/view.py` & `wbBase-0.2.2/Lib/wbBase/document/view.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/panelManager.py` & `wbBase-0.2.2/Lib/wbBase/panelManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,21 @@
             mnu.AppendSeparator()
             item = wx.MenuItem(
                 mnu, wx.ID_ANY, "Tooltips", "Show/Hide Tooltips ", wx.ITEM_CHECK
             )
             mnu.Append(item)
             self.Bind(wx.EVT_MENU, self.on_menu_tooltip, id=item.Id)
             self.Bind(wx.EVT_UPDATE_UI, self.update_menu_tooltip, id=item.Id)
+
+            item = wx.MenuItem(
+                mnu, wx.ID_ANY, "Statusbar", "Show/Hide Statusbar ", wx.ITEM_CHECK
+            )
+            mnu.Append(item)
+            self.Bind(wx.EVT_MENU, self.on_menu_statusbar, id=item.Id)
+            self.Bind(wx.EVT_UPDATE_UI, self.update_menu_statusbar, id=item.Id)
         return self._menu
 
     @property
     def toolbar(self) -> aui.AuiToolBar:
         if not self._toolbar.GetToolCount():
             menu = self.menu
             tb = self._toolbar
@@ -578,7 +585,15 @@
             self.Update()
 
     def on_menu_tooltip(self, event: wx.CommandEvent):
         self.app.TopWindow.showTooltip = event.IsChecked()
 
     def update_menu_tooltip(self, event: wx.UpdateUIEvent):
         event.Check(self.app.TopWindow.showTooltip)
+
+    def on_menu_statusbar(self, event: wx.CommandEvent):
+        self.app.TopWindow.StatusBar.Show(event.IsChecked())
+        self.app.TopWindow.SendSizeEvent()
+        self.app.TopWindow.Refresh()
+
+    def update_menu_statusbar(self, event: wx.UpdateUIEvent):
+        event.Check(self.app.TopWindow.StatusBar.IsShown())
```

### Comparing `wbBase-0.2.0/Lib/wbBase/pluginManager.py` & `wbBase-0.2.2/Lib/wbBase/pluginManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,24 +74,24 @@
                     self[name] = module
                 except ImportError:
                     log.exception(
                         "=============== Can't load plugin %s ===============", name
                     )
                     if plugin.Installation == "required":
                         if app._splashScreen:
-                            app._splashScreen.Destroy()
+                            app._splashScreen.Hide()
                         wx.LogError(
                             "Required plugin error\n\n"
                             f"Can't load plugin '{name}'\n"
-                            "See terminal output for traceback."
+                            "See terminal output for traceback.\n"
                             "Application will terminate."
                         )
                         sys.exit(1)
             elif plugin.Installation == "required":
                 if app._splashScreen:
-                    app._splashScreen.Destroy()
+                    app._splashScreen.Hide()
                 wx.LogError(
                     "Missing required plugin\n\n"
                     f"Can't load plugin '{name}'\n"
                     "Application will terminate."
                 )
                 sys.exit(1)
```

### Comparing `wbBase-0.2.0/Lib/wbBase/pluginManager_old.py` & `wbBase-0.2.2/Lib/wbBase/pluginManager_old.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/scripting.py` & `wbBase-0.2.2/Lib/wbBase/scripting.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase/tools.py` & `wbBase-0.2.2/Lib/wbBase/tools.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/Lib/wbBase.egg-info/PKG-INFO` & `wbBase-0.2.2/Lib/wbBase.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.2.0
+Version: 0.2.2
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
@@ -65,7 +65,9 @@
     integrates the Widgetinspector in Workbench applications.
 - [wbpFilebrowser](https://pypi.org/project/wbpfilebrowser/),
     a file browser panel for Workbench applications.
 - [wbpTextedit](https://pypi.org/project/wbptextedit/),
     document templates to create, view and edit some text file types.
 - [wbpUItools](https://pypi.org/project/wbpuitools/),
     collection of some useful functions for user interaction in Python scripts.
+- [wbpHTMLpanel](https://pypi.org/project/wbpHTMLpanel/),
+    a panel to display arbitrary html.
```

### Comparing `wbBase-0.2.0/Lib/wbBase.egg-info/SOURCES.txt` & `wbBase-0.2.2/Lib/wbBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.0/PKG-INFO` & `wbBase-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.2.0
+Version: 0.2.2
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
@@ -65,7 +65,9 @@
     integrates the Widgetinspector in Workbench applications.
 - [wbpFilebrowser](https://pypi.org/project/wbpfilebrowser/),
     a file browser panel for Workbench applications.
 - [wbpTextedit](https://pypi.org/project/wbptextedit/),
     document templates to create, view and edit some text file types.
 - [wbpUItools](https://pypi.org/project/wbpuitools/),
     collection of some useful functions for user interaction in Python scripts.
+- [wbpHTMLpanel](https://pypi.org/project/wbpHTMLpanel/),
+    a panel to display arbitrary html.
```

### Comparing `wbBase-0.2.0/README.md` & `wbBase-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,7 +29,9 @@
     integrates the Widgetinspector in Workbench applications.
 - [wbpFilebrowser](https://pypi.org/project/wbpfilebrowser/),
     a file browser panel for Workbench applications.
 - [wbpTextedit](https://pypi.org/project/wbptextedit/),
     document templates to create, view and edit some text file types.
 - [wbpUItools](https://pypi.org/project/wbpuitools/),
     collection of some useful functions for user interaction in Python scripts.
+- [wbpHTMLpanel](https://pypi.org/project/wbpHTMLpanel/),
+    a panel to display arbitrary html.
```

### Comparing `wbBase-0.2.0/setup.cfg` & `wbBase-0.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.2
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
```

