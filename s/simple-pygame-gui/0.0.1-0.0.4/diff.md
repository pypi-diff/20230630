# Comparing `tmp/simple_pygame_gui-0.0.1.tar.gz` & `tmp/simple_pygame_gui-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_pygame_gui-0.0.1.tar", last modified: Thu Jun 29 19:14:55 2023, max compression
+gzip compressed data, was "simple_pygame_gui-0.0.4.tar", last modified: Thu Jun 29 20:05:26 2023, max compression
```

## Comparing `simple_pygame_gui-0.0.1.tar` & `simple_pygame_gui-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 19:14:55.740101 simple_pygame_gui-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-06-29 18:54:28.000000 simple_pygame_gui-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       31 2023-06-29 18:56:38.000000 simple_pygame_gui-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      486 2023-06-29 19:14:55.740602 simple_pygame_gui-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-06-29 18:47:53.000000 simple_pygame_gui-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-06-29 19:07:56.000000 simple_pygame_gui-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      562 2023-06-29 19:14:55.744101 simple_pygame_gui-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 19:14:55.734669 simple_pygame_gui-0.0.1/simple_pygame_gui/
--rw-rw-rw-   0        0        0     1777 2023-06-29 18:21:35.000000 simple_pygame_gui-0.0.1/simple_pygame_gui/Button.py
--rw-rw-rw-   0        0        0     1531 2023-06-29 18:26:59.000000 simple_pygame_gui-0.0.1/simple_pygame_gui/FloatBox.py
--rw-rw-rw-   0        0        0     2443 2023-06-29 19:01:24.000000 simple_pygame_gui-0.0.1/simple_pygame_gui/Switch.py
--rw-rw-rw-   0        0        0      324 2021-08-04 15:37:06.000000 simple_pygame_gui-0.0.1/simple_pygame_gui/Switch_off.png
--rw-rw-rw-   0        0        0      318 2021-08-04 15:38:10.000000 simple_pygame_gui-0.0.1/simple_pygame_gui/Switch_on.png
--rw-rw-rw-   0        0        0     2423 2023-06-29 18:24:21.000000 simple_pygame_gui-0.0.1/simple_pygame_gui/TextBox.py
--rw-rw-rw-   0        0        0      155 2023-06-29 18:29:07.000000 simple_pygame_gui-0.0.1/simple_pygame_gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:14:55.739601 simple_pygame_gui-0.0.1/simple_pygame_gui.egg-info/
--rw-rw-rw-   0        0        0      486 2023-06-29 19:14:55.000000 simple_pygame_gui-0.0.1/simple_pygame_gui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-06-29 19:14:55.000000 simple_pygame_gui-0.0.1/simple_pygame_gui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 19:14:55.000000 simple_pygame_gui-0.0.1/simple_pygame_gui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-29 19:14:55.000000 simple_pygame_gui-0.0.1/simple_pygame_gui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 20:05:26.739230 simple_pygame_gui-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-06-29 18:54:28.000000 simple_pygame_gui-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       64 2023-06-29 19:41:48.000000 simple_pygame_gui-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      486 2023-06-29 20:05:26.739230 simple_pygame_gui-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-06-29 18:47:53.000000 simple_pygame_gui-0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-29 19:07:56.000000 simple_pygame_gui-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      562 2023-06-29 20:05:26.739730 simple_pygame_gui-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 20:05:26.732731 simple_pygame_gui-0.0.4/simple_pygame_gui/
+-rw-rw-rw-   0        0        0     1946 2023-06-29 19:46:50.000000 simple_pygame_gui-0.0.4/simple_pygame_gui/Button.py
+-rw-rw-rw-   0        0        0     1532 2023-06-29 20:03:07.000000 simple_pygame_gui-0.0.4/simple_pygame_gui/FloatBox.py
+-rw-rw-rw-   0        0        0   714456 2023-06-29 19:41:25.000000 simple_pygame_gui-0.0.4/simple_pygame_gui/FreeSans.ttf
+-rw-rw-rw-   0        0        0   359272 2023-06-29 19:59:19.000000 simple_pygame_gui-0.0.4/simple_pygame_gui/FreeSansBold.ttf
+-rw-rw-rw-   0        0        0     2582 2023-06-29 19:44:50.000000 simple_pygame_gui-0.0.4/simple_pygame_gui/Switch.py
+-rw-rw-rw-   0        0        0      324 2021-08-04 15:37:06.000000 simple_pygame_gui-0.0.4/simple_pygame_gui/Switch_off.png
+-rw-rw-rw-   0        0        0      318 2021-08-04 15:38:10.000000 simple_pygame_gui-0.0.4/simple_pygame_gui/Switch_on.png
+-rw-rw-rw-   0        0        0     2549 2023-06-29 19:46:25.000000 simple_pygame_gui-0.0.4/simple_pygame_gui/TextBox.py
+-rw-rw-rw-   0        0        0      159 2023-06-29 20:03:13.000000 simple_pygame_gui-0.0.4/simple_pygame_gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:05:26.738731 simple_pygame_gui-0.0.4/simple_pygame_gui.egg-info/
+-rw-rw-rw-   0        0        0      486 2023-06-29 20:05:26.000000 simple_pygame_gui-0.0.4/simple_pygame_gui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2023-06-29 20:05:26.000000 simple_pygame_gui-0.0.4/simple_pygame_gui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:05:26.000000 simple_pygame_gui-0.0.4/simple_pygame_gui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-29 20:05:26.000000 simple_pygame_gui-0.0.4/simple_pygame_gui.egg-info/top_level.txt
```

### Comparing `simple_pygame_gui-0.0.1/LICENSE` & `simple_pygame_gui-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_pygame_gui-0.0.1/setup.cfg` & `simple_pygame_gui-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 696d 706c 655f 7079 6761 6d65   = simple_pygame
 00000020: 5f67 7569 0d0a 7665 7273 696f 6e20 3d20  _gui..version = 
-00000030: 302e 302e 310d 0a61 7574 686f 7220 3d20  0.0.1..author = 
-00000040: 4b65 7669 6e20 454c 6c0d 0a61 7574 686f  Kevin ELl..autho
+00000030: 302e 302e 340d 0a61 7574 686f 7220 3d20  0.0.4..author = 
+00000040: 4b65 7669 6e20 456c 6c0d 0a61 7574 686f  Kevin Ell..autho
 00000050: 725f 656d 6169 6c20 3d20 6b65 7669 6e65  r_email = kevine
 00000060: 6c6c 3734 4067 6d61 696c 2e63 6f6d 0d0a  ll74@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5573  description = Us
 00000080: 6566 756c 6c20 4755 4920 656c 656d 656e  efull GUI elemen
 00000090: 7473 2066 6f72 2079 6f75 7220 7079 6761  ts for your pyga
 000000a0: 6d65 2070 726f 6a65 6374 730d 0a6c 6f6e  me projects..lon
 000000b0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description =
```

### Comparing `simple_pygame_gui-0.0.1/simple_pygame_gui/Button.py` & `simple_pygame_gui-0.0.4/simple_pygame_gui/Button.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import time
 from abc import abstractmethod
 import pygame
+from importlib import resources
+import io
 
 pygame.init()
 pygame.font.init()
 
 
 class Button:
     def __init__(self, target, x, y, width, height, text="Button", font="FreeSans.ttf", fontSize=20, bold=False, italic=False, textColor=(0, 0, 0), buttonColor=(200, 200, 200)):
         """
         create a new class that overwrites the function "function"
         """
         if (target == None):
             ValueError('No function for target is specified')
         self.target = target
         self.rect = pygame.Rect(x, y, width, height)
-        self.font = pygame.font.SysFont(font, fontSize, bold, italic)
+        
+        with resources.open_binary('simple_pygame_gui', font) as fp:
+            self.font = fp.read()
+        self.font = pygame.font.Font(io.BytesIO(self.font), fontSize)
+        
         txt_width, txt_height = self.font.size(text)
         self.textrect = pygame.Rect(x + (width / 2 - txt_width / 2), y + (height / 2 - txt_height / 2), width, height)
         self.text = text
         self.selected = False
         self.textColor = textColor
         self.buttonColor = buttonColor
         self.time = time.time()
```

### Comparing `simple_pygame_gui-0.0.1/simple_pygame_gui/FloatBox.py` & `simple_pygame_gui-0.0.4/simple_pygame_gui/FloatBox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pygame
 
-from TextBox import TextBox, SELECTED, TEXT_COLOR, FONT
+from .TextBox import TextBox, SELECTED, TEXT_COLOR, FONT
 
 
 class FloatBox(TextBox):
     savedValue = 0
 
     def __init__(self, x, y, width = 25, height = 25, standardValue = 0, name = "", nameColor = (50, 50, 50)):
         super().__init__(x, y, width, height, standardValue, name, nameColor)
```

### Comparing `simple_pygame_gui-0.0.1/simple_pygame_gui/Switch.py` & `simple_pygame_gui-0.0.4/simple_pygame_gui/Switch.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 
 
         self.state = state
         self.name = name
         self.x = x
         self.y = y
         self.width = width
-        self.font = pygame.font.SysFont(font, fontSize)
+        
+        with resources.open_binary('simple_pygame_gui', font) as fp:
+            self.font = fp.read()
+        self.font = pygame.font.Font(io.BytesIO(self.font), fontSize)
+        
         self.bgRect = pygame.Rect(x, y, width, height)
         self.baseRect = pygame.Rect(x + 2, y + 2, width - 4, height - 4)
         self.onRect = pygame.Rect(x + 4, y + 4, (width - 4) / 2 - 2, height - 8)
         self.offRect = pygame.Rect(x + width / 2, y + 4, (width - 4) / 2 - 2, height - 8)
 
 
     def __bool__(self):
```

### Comparing `simple_pygame_gui-0.0.1/simple_pygame_gui/TextBox.py` & `simple_pygame_gui-0.0.4/simple_pygame_gui/TextBox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import pygame
+from importlib import resources
+import io
 
 pygame.init()
 
 SELECTED = pygame.color.Color(220, 255, 255)
 TEXT_COLOR = pygame.color.Color(70, 70, 70)
-FONT = pygame.font.SysFont("FreeSansBold.ttf", size = 30)
+with resources.open_binary('simple_pygame_gui', 'FreeSans.ttf') as fp:
+    FONT = fp.read()
+FONT = pygame.font.Font(io.BytesIO(FONT), 25)
 
 class TextBox:
     def __init__(self, x, y, width = 25, height = 25, standardValue = "", name = "", nameColor = (50, 50, 50)):
         if width < 25 or height < 25:
             raise ValueError("minumum dimensions must be 25")
         self.x = x
         self.y = y
```

