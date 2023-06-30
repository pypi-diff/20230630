# Comparing `tmp/irene_pro-0.0.77.tar.gz` & `tmp/irene_pro-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.77.tar", last modified: Fri Jun 30 06:56:00 2023, max compression
+gzip compressed data, was "irene_pro-0.0.79.tar", last modified: Fri Jun 30 08:49:55 2023, max compression
```

## Comparing `irene_pro-0.0.77.tar` & `irene_pro-0.0.79.tar`

### file list

```diff
@@ -1,21 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 06:56:00.365151 irene_pro-0.0.77/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.77/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.77/MANIFEST.in
--rw-rw-rw-   0        0        0     1940 2023-06-30 06:56:00.359165 irene_pro-0.0.77/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.77/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 06:56:00.323300 irene_pro-0.0.77/irene_gui_pkg/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.77/irene_gui_pkg/__init__.py
--rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.77/irene_gui_pkg/logic.py
--rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.77/irene_gui_pkg/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:56:00.333234 irene_pro-0.0.77/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.77/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     5924 2023-06-26 06:52:40.000000 irene_pro-0.0.77/irene_pro/logic.py
--rw-rw-rw-   0        0        0    36957 2023-06-30 06:53:50.000000 irene_pro-0.0.77/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:56:00.356175 irene_pro-0.0.77/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1940 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-30 06:56:00.000000 irene_pro-0.0.77/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 06:56:00.366146 irene_pro-0.0.77/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-29 14:29:59.000000 irene_pro-0.0.77/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:49:55.944471 irene_pro-0.0.79/
+-rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.79/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.79/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-06-30 08:49:55.940289 irene_pro-0.0.79/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.79/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 08:49:55.895003 irene_pro-0.0.79/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.79/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5918 2023-06-30 07:20:45.000000 irene_pro-0.0.79/irene_pro/logics.py
+-rw-rw-rw-   0        0        0    36831 2023-06-30 08:35:02.000000 irene_pro-0.0.79/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:49:55.931269 irene_pro-0.0.79/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-06-30 08:49:55.000000 irene_pro-0.0.79/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-30 08:49:55.000000 irene_pro-0.0.79/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 08:49:55.000000 irene_pro-0.0.79/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-30 08:49:55.000000 irene_pro-0.0.79/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-30 08:49:55.000000 irene_pro-0.0.79/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 08:49:55.945469 irene_pro-0.0.79/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-30 08:48:54.000000 irene_pro-0.0.79/setup.py
```

### Comparing `irene_pro-0.0.77/irene_gui_pkg/logic.py` & `irene_pro-0.0.79/irene_pro/logics.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -167,8 +167,8 @@
             else:
                 conn.execute(f"DELETE FROM {table_name} WHERE {cond}")
 
     def Columns(self, table_name):
         conn = self.Conn
         with conn:
             all_data = conn.execute(f"PRAGMA table_info({table_name})").fetchall()
-            return [(row[1], row[2]) for row in all_data]
+            return [(row[1], row[2]) for row in all_data]
```

### Comparing `irene_pro-0.0.77/irene_gui_pkg/widgets.py` & `irene_pro-0.0.79/irene_pro/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,82 @@
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
+        if "@" in email and '.com' in email and email[0] not in punctuations and " " not in email:
+            return True
+        else:
+            return False
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
@@ -49,15 +104,15 @@
             pass
 
 class treeview(ttk.Treeview):
     def __init__(self, master, columns, col_width = w(130), rowheight = h(100),include_index = False, **kwargs) -> None:
         super().__init__(master, **kwargs)
         self.master = master
 
-        self.alter_rows()
+        # self.alter_rows()
 
         style = ttk.Style()
         style.configure("Treeview", font = ('arial', w(11)), background=master['bg'], fieldbackground=master['bg'], foreground="#000", rowheight = rowheight)
         self.include_index = include_index
         
         self["column"] = columns
         index_zero_width = 0
@@ -83,15 +138,16 @@
         style = ttkthemes.ThemedStyle(self.master)
         style.theme_use("clam")
         style.map("Treeview", background=[('selected', 'gray40')], foreground = [('selected', 'gold')])
         self.tag_configure('odd', background=odd_color)
         self.tag_configure('even', background=even_color)
 
 
-    def insert_data(self,data, wrap_length = 70):
+    def insert_data(self,data, wrap_length = 70, odd_color = 'gray70', even_color = 'khaki'):
+        self.alter_rows(odd_color=odd_color, even_color=even_color)
         def wrapping(data_list):
             """I assume that datalist is a list as the name implies"""
             all_row = []
             for item in data_list:
                 # print(f"CURRENT ITEM: {item}")
                 if type(item) == str:
                     wrapped = wrap(item, wrap_length)
@@ -134,59 +190,76 @@
         except IndexError:
             pass
 
 class btn(Button):
     def __init__(self, master,image = None, **kwargs):
         super().__init__(master=master, compound = "left", bd = 0,font = w(12),image = image, **kwargs)
         
+        prev_color = 'gray90'
         # configure save button
         if 'save' in str(self['text']).lower():
             self.config(bg = "#9400D3", fg = "#fff", image = image)
+            prev_color = self.cget('bg')
         
         elif 'edit' in str(self['text']).lower():
             self.config(bg = "#0b4", fg = "#fff", image = image)
+            prev_color = self.cget('bg')
 
         elif 'date' in str(self['text']).lower():
             self.config(bg = "#00BFFF", fg = "#000", image = image)
+            prev_color = self.cget('bg')
         
         elif "add" in str(self['text']).lower():
             self.config(bg = "#008000", fg = "#fff", image = image)
+            prev_color = self.cget('bg')
 
         elif "delete" in str(self['text']).lower():
             self.config(bg = "#600", fg = "#fff", image=image)
+            prev_color = self.cget('bg')
 
         elif 'set' in str(self['text']).lower():
             self.config(bg = "#DAA520", fg = "#fff", image=image)
+            prev_color = self.cget('bg')
 
         elif 'close' in str(self['text']).lower():
             self.config(image = image, bg = "maroon", fg = "#fff")
+            prev_color = self.cget('bg')
 
         elif 'display' in str(self['text']).lower() or 'show' in str(self['text']).lower(): 
             self.config(bg = "#008080", fg = "#fff", image=image)
+            prev_color = self.cget('bg')
 
         elif "cancel" in str(self['text']).lower():
             self.config(image = image, bg = "gray50")
+            prev_color = self.cget('bg')
         
         elif "attach" in str(self["text"]).lower() or "browse" in str(self["text"]).lower():
             self.config(image = image, bg = "#b04", fg = "#fff")
+            prev_color = self.cget('bg')
         
         elif "send" in str(self['text']).lower():
             self.config(image = image, bg = "#FF6E00", fg = "#fff")
+            prev_color = self.cget('bg')
         
         elif "print" in str(self['text']).lower():
             self.config(bg = "#FEE3B8", image = image)
+            prev_color = self.cget('bg')
         
         elif "plan" in str(self['text']).lower():
             self.config(bg = "#600", fg = "#fff", image = image)
+            prev_color = self.cget('bg')
 
         if " all" in str(self['text']).lower():
             self.config(image = image)
         
         if " id" in str(self['text']).lower():
             self.config(image = image)
+        
+        self.bind('<Enter>', lambda e: self.config(bg = '#39ff13'))
+        self.bind('<Leave>', lambda e: self.config(bg = prev_color))
     
 
 class Display_image:
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
     
     def image(self, img:str):
@@ -196,15 +269,15 @@
             cv2.resizeWindow("Image", w(800), h(600))
             cv2.imshow("Image", frame)
         except cv2.error:
             pass
 
 class panedw(ttk.Panedwindow):
     def __init__(self, master, **kwargs):
-        super().__init__(master=master, bd = 0, **kwargs)
+        super().__init__(master=master, **kwargs)
 
 class EntryBtns:
     def __init__(self, parent, saved_data_holder, entry_tags, entry_fr_height = h(50),
                         entry_fr_side = TOP, fill = X, widget_2_create = 'entry'
                         , browse = False, ent_id_width = 5, default = None):
         
         self.saved_data_holder = saved_data_holder
@@ -345,27 +418,45 @@
             if len(str(self.get()).strip()) == 0:
                 self.insert(END, default)
                 self.config(fg = "gray50")
 
 
 #=====================COMBOBOX=======================
 class combo(ttk.Combobox):
-    def __init__(self, master, label_txt = None, label_side = LEFT,bd_color = "#0b4", **kwargs):
+    def __init__(self, master, label_txt = None, label_side = LEFT,bd_color = "#0b4", default = None, **kwargs):
         super().__init__(master, font = ('arial', w(12)),**kwargs)
         self.master = master
         self.st = ttk.Style()
         self.st.theme_use('clam')
         
         self.st.configure('comb.TCombobox', foreground = "#023", fieldbackground = self.master['bg'],
                             bordercolor = bd_color, background = bd_color)
         try:
             if label_txt:
                 label(master=self.master, text = label_txt).pack(side = label_side, padx = w(2), pady=w(2))
         except Exception:
             pass
+        
+        def remove_default():
+            if self.get() == default:
+                self.set('')
+        
+        def set_default():
+            print("LEAVING COMBOBOX.....")
+            if self.get().strip() == "" or len(self.get().strip()) == 0:
+                self.set(default)
+                print("[DEFAULT SET]")
+            else:
+                print(f"COMBO VALUE FOUND: {self.get().strip()}: length: {len(self.get().strip())}")
+
+        if self.cget('state') != 'readonly':
+            if default:
+                self.set(default)
+                self.bind("<Button-1>", lambda e: remove_default())
+                self.bind("<Leave>", lambda e: set_default())
 
     
 class checkb(ttk.Checkbutton):
     def __init__(self, master, **kwargs):
         super().__init__(master = master, **kwargs)
         style = ttk.Style()
         style.configure("TCheckbutton", background = master['bg'], foreground="#023", font=("Arial", w(12)))
@@ -787,11 +878,13 @@
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

### Comparing `irene_pro-0.0.77/setup.py` & `irene_pro-0.0.79/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3737 270d 0a44 4553 4352   '0.0.77'..DESCR
+00000100: 2027 302e 302e 3739 270d 0a44 4553 4352   '0.0.79'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

