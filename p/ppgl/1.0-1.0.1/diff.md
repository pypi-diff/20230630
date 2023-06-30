# Comparing `tmp/ppgl-1.0.tar.gz` & `tmp/ppgl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppgl-1.0.tar", last modified: Fri Jun 30 19:02:53 2023, max compression
+gzip compressed data, was "ppgl-1.0.1.tar", last modified: Fri Jun 30 19:08:30 2023, max compression
```

## Comparing `ppgl-1.0.tar` & `ppgl-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:02:53.223683 ppgl-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-30 19:02:42.000000 ppgl-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 19:02:53.223683 ppgl-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 19:02:42.000000 ppgl-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:02:53.219683 ppgl-1.0/ppgl/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-30 19:02:42.000000 ppgl-1.0/ppgl/ppgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:02:53.223683 ppgl-1.0/ppgl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 19:02:53.000000 ppgl-1.0/ppgl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-30 19:02:53.000000 ppgl-1.0/ppgl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:02:53.000000 ppgl-1.0/ppgl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 19:02:53.000000 ppgl-1.0/ppgl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:02:53.223683 ppgl-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-30 19:02:42.000000 ppgl-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:08:30.435822 ppgl-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-30 19:08:20.000000 ppgl-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-30 19:08:30.435822 ppgl-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-30 19:08:20.000000 ppgl-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:08:30.431822 ppgl-1.0.1/ppgl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-30 19:08:20.000000 ppgl-1.0.1/ppgl/ppgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:08:30.435822 ppgl-1.0.1/ppgl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-30 19:08:30.000000 ppgl-1.0.1/ppgl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-30 19:08:30.000000 ppgl-1.0.1/ppgl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:08:30.000000 ppgl-1.0.1/ppgl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 19:08:30.000000 ppgl-1.0.1/ppgl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:08:30.435822 ppgl-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-30 19:08:20.000000 ppgl-1.0.1/setup.py
```

### Comparing `ppgl-1.0/LICENSE` & `ppgl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ppgl-1.0/ppgl/ppgl.py` & `ppgl-1.0.1/ppgl/ppgl.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # gui class that is reusable meaning it easy
 class GUI:
     def __init__(self, width, height):
         self.width = width
         self.height = height
         self.root = tk.Tk()
-        self.root.title("YATP")
+        self.root.title("PPGL")
         self.root.resizable(True, True)
         self.root.geometry(f"{self.width}x{self.height}")
         self.statistics = {}
 
     def start(self):
         self.root.mainloop()
```

