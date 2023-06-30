# Comparing `tmp/irene_pro-0.0.76.tar.gz` & `tmp/irene_pro-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.76.tar", last modified: Mon Jun 26 12:55:11 2023, max compression
+gzip compressed data, was "irene_pro-0.0.77.tar", last modified: Fri Jun 30 06:56:00 2023, max compression
```

## Comparing `irene_pro-0.0.76.tar` & `irene_pro-0.0.77.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 12:55:11.333047 irene_pro-0.0.76/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.76/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.76/MANIFEST.in
--rw-rw-rw-   0        0        0     1940 2023-06-26 12:55:11.330160 irene_pro-0.0.76/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.76/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 12:55:11.264232 irene_pro-0.0.76/irene_gui_pkg/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.76/irene_gui_pkg/__init__.py
--rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.76/irene_gui_pkg/logic.py
--rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.76/irene_gui_pkg/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-26 12:55:11.285175 irene_pro-0.0.76/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.76/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     5924 2023-06-26 06:52:40.000000 irene_pro-0.0.76/irene_pro/logic.py
--rw-rw-rw-   0        0        0    34964 2023-06-26 12:54:19.000000 irene_pro-0.0.76/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-26 12:55:11.323126 irene_pro-0.0.76/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1940 2023-06-26 12:55:11.000000 irene_pro-0.0.76/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-06-26 12:55:11.000000 irene_pro-0.0.76/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 12:55:11.000000 irene_pro-0.0.76/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-26 12:55:11.000000 irene_pro-0.0.76/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-26 12:55:11.000000 irene_pro-0.0.76/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 12:55:11.334044 irene_pro-0.0.76/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-26 12:54:32.000000 irene_pro-0.0.76/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:56:00.365151 irene_pro-0.0.77/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.77/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.77/MANIFEST.in
+-rw-rw-rw-   0        0        0     1940 2023-06-30 06:56:00.359165 irene_pro-0.0.77/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.77/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 06:56:00.323300 irene_pro-0.0.77/irene_gui_pkg/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.77/irene_gui_pkg/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.77/irene_gui_pkg/logic.py
+-rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.77/irene_gui_pkg/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:56:00.333234 irene_pro-0.0.77/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.77/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5924 2023-06-26 06:52:40.000000 irene_pro-0.0.77/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    36957 2023-06-30 06:53:50.000000 irene_pro-0.0.77/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:56:00.356175 irene_pro-0.0.77/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 06:56:00.366146 irene_pro-0.0.77/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-29 14:29:59.000000 irene_pro-0.0.77/setup.py
```

### Comparing `irene_pro-0.0.76/PKG-INFO` & `irene_pro-0.0.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.76
+Version: 0.0.77
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.76/README.md` & `irene_pro-0.0.77/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.76/irene_gui_pkg/logic.py` & `irene_pro-0.0.77/irene_gui_pkg/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.76/irene_gui_pkg/widgets.py` & `irene_pro-0.0.77/irene_gui_pkg/widgets.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.76/irene_pro/logic.py` & `irene_pro-0.0.77/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.76/irene_pro/widgets.py` & `irene_pro-0.0.77/irene_pro/widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,83 @@
 from win32api import GetSystemMetrics as ruler
 from math import ceil
 import cv2
 from tkcalendar import Calendar
 import ttkthemes
 import numpy as np
 from textwrap import wrap
+from string import punctuation, ascii_lowercase
+
+punctuations = [i for i in punctuation]
 
 s_width = ruler(0)
 s_height = ruler(1)
 
-
 def w(width:float):
     ratio = width / 1366
     return ceil((ratio * s_width))
 
 def h(height:float):
     ratio = height / 768
     return ceil((ratio * s_height))
 
+class Restrict:
+    def __init__(self, widget) -> None:
+        self.widget = widget
+
+    def restrict_length(self, max_len, add_event = False):
+        if add_event:
+            self.widget.bind("<KeyRelease>", lambda e: restrict(), add = "+")
+        else:
+            self.widget.bind("<KeyRelease>", lambda e: restrict())
+        def restrict():
+            if len(str(self.widget.get())) > max_len:
+                try:
+                    self.widget.delete(max_len-1, END)
+                except TclError:
+                    pass
+    
+    def restrict_delete(self):
+        self.widget.bind("<BackSpace>", lambda _: "break")
+        self.widget.bind("<Delete>", lambda _: "break")
+        self.widget.bind("<KeyPress>", lambda _: "break")
+    
+class Validate:
+    def __init__(self) -> None:
+        pass
+
+    def validate_email(self, email):
+        email = email.strip()
+        if "@gmail.com" in email and not email[0] not in punctuations and " " not in email:
+            return True
+        elif "@" in email and '.com' in email and "gmail" not in email and email[0] not in punctuations and " " not in email:
+            return True
+        return False
+    
+    def all_are_numbers(self, value):
+        nums = [str(i) for i in range(10)]
+        decision = True
+        for i in str(value):
+            if i not in nums:
+                decision = False
+        return decision
+
+    def all_are_letters(self, value):
+        letters = [i for i in ascii_lowercase]
+        decision = True
+        for j in str(value):
+            if j not in letters:
+                decision = False
+            return decision
+
+    def validate_rwf_phone_number(self, phone_number):
+        if phone_number.startswith('0') and len(phone_number) == 10 and self.all_are_numbers(phone_number):
+            return True
+        return False
+        
 class frame(Frame):
     def __init__(self, master, **kwargs):
         super().__init__(master=master,bd = 0, **kwargs)
         num = re.compile("\d{1,}")
         try:
             found_num = num.findall(master['bg'])
             if found_num:
@@ -823,11 +879,13 @@
         details.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
         close_btn = btn(fr, text = "close",activebackground = fr.cget('bg'), command = lambda: fr.destroy())
         close_btn.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
         return delete_btn, edit_btn, status, details
 
+
+
 # CONSTANTS
 comb_syle = 'comb.TCombobox'
 check_style = "TCheckbutton"
 radio_style = "Custom.TRadiobutton"
```

### Comparing `irene_pro-0.0.76/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.77/irene_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.76
+Version: 0.0.77
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.76/setup.py` & `irene_pro-0.0.77/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3736 270d 0a44 4553 4352   '0.0.76'..DESCR
+00000100: 2027 302e 302e 3737 270d 0a44 4553 4352   '0.0.77'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

