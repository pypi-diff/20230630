# Comparing `tmp/rsyncy-0.1.0.tar.gz` & `tmp/rsyncy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsyncy-0.1.0.tar", last modified: Mon Jan  9 22:35:59 2023, max compression
+gzip compressed data, was "rsyncy-0.2.0.tar", last modified: Fri Jun 30 21:03:51 2023, max compression
```

## Comparing `rsyncy-0.1.0.tar` & `rsyncy-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 spark      (501) staff       (20)        0 2023-01-09 22:35:59.237548 rsyncy-0.1.0/
--rw-r--r--   0 spark      (501) staff       (20)     1083 2020-11-15 20:22:13.000000 rsyncy-0.1.0/LICENSE
--rw-r--r--   0 spark      (501) staff       (20)     3174 2023-01-09 22:35:59.237287 rsyncy-0.1.0/PKG-INFO
--rw-r--r--   0 spark      (501) staff       (20)     2921 2023-01-09 22:33:49.000000 rsyncy-0.1.0/README.md
--rwxr-xr-x   0 spark      (501) staff       (20)     8684 2023-01-09 22:33:49.000000 rsyncy-0.1.0/rsyncy
--rwxr-xr-x   0 spark      (501) staff       (20)     8684 2023-01-09 22:33:49.000000 rsyncy-0.1.0/rsyncy-stat
-drwxr-xr-x   0 spark      (501) staff       (20)        0 2023-01-09 22:35:59.236983 rsyncy-0.1.0/rsyncy.egg-info/
--rw-r--r--   0 spark      (501) staff       (20)     3174 2023-01-09 22:35:59.000000 rsyncy-0.1.0/rsyncy.egg-info/PKG-INFO
--rw-r--r--   0 spark      (501) staff       (20)      175 2023-01-09 22:35:59.000000 rsyncy-0.1.0/rsyncy.egg-info/SOURCES.txt
--rw-r--r--   0 spark      (501) staff       (20)        1 2023-01-09 22:35:59.000000 rsyncy-0.1.0/rsyncy.egg-info/dependency_links.txt
--rw-r--r--   0 spark      (501) staff       (20)        7 2023-01-09 22:35:59.000000 rsyncy-0.1.0/rsyncy.egg-info/top_level.txt
--rwxr-xr-x   0 spark      (501) staff       (20)     8684 2023-01-09 22:33:49.000000 rsyncy-0.1.0/rsyncy.py
--rw-r--r--   0 spark      (501) staff       (20)       38 2023-01-09 22:35:59.237620 rsyncy-0.1.0/setup.cfg
--rw-r--r--   0 spark      (501) staff       (20)      550 2023-01-09 22:33:49.000000 rsyncy-0.1.0/setup.py
+drwxr-xr-x   0 spark      (501) staff       (20)        0 2023-06-30 21:03:51.887206 rsyncy-0.2.0/
+-rw-r--r--   0 spark      (501) staff       (20)     1083 2020-11-15 20:22:13.000000 rsyncy-0.2.0/LICENSE
+-rw-r--r--   0 spark      (501) staff       (20)     3187 2023-06-30 21:03:51.886938 rsyncy-0.2.0/PKG-INFO
+-rw-r--r--   0 spark      (501) staff       (20)     2934 2023-06-30 21:01:48.000000 rsyncy-0.2.0/README.md
+-rwxr-xr-x   0 spark      (501) staff       (20)     9068 2023-06-30 20:58:16.000000 rsyncy-0.2.0/rsyncy
+-rwxr-xr-x   0 spark      (501) staff       (20)     9068 2023-06-30 20:58:16.000000 rsyncy-0.2.0/rsyncy-stat
+drwxr-xr-x   0 spark      (501) staff       (20)        0 2023-06-30 21:03:51.886609 rsyncy-0.2.0/rsyncy.egg-info/
+-rw-r--r--   0 spark      (501) staff       (20)     3187 2023-06-30 21:03:51.000000 rsyncy-0.2.0/rsyncy.egg-info/PKG-INFO
+-rw-r--r--   0 spark      (501) staff       (20)      175 2023-06-30 21:03:51.000000 rsyncy-0.2.0/rsyncy.egg-info/SOURCES.txt
+-rw-r--r--   0 spark      (501) staff       (20)        1 2023-06-30 21:03:51.000000 rsyncy-0.2.0/rsyncy.egg-info/dependency_links.txt
+-rw-r--r--   0 spark      (501) staff       (20)        7 2023-06-30 21:03:51.000000 rsyncy-0.2.0/rsyncy.egg-info/top_level.txt
+-rwxr-xr-x   0 spark      (501) staff       (20)     9068 2023-06-30 20:58:16.000000 rsyncy-0.2.0/rsyncy.py
+-rw-r--r--   0 spark      (501) staff       (20)       38 2023-06-30 21:03:51.887288 rsyncy-0.2.0/setup.cfg
+-rw-r--r--   0 spark      (501) staff       (20)      550 2023-06-30 21:02:55.000000 rsyncy-0.2.0/setup.py
```

### Comparing `rsyncy-0.1.0/LICENSE` & `rsyncy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsyncy-0.1.0/PKG-INFO` & `rsyncy-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsyncy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A status/progress bar for rsync.
 Home-page: https://github.com/laktak/rsyncy
 Author: Christian Zangl
 Author-email: laktak@cdak.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -69,15 +69,17 @@
 
 Alternatively you can pipe the output from rsync to rsyncy (in which case you need to specify `--info=progress2 -hv` yourself).
 
 ```
 $ rsync -a --info=progress2 -hv FROM/ TO | rsyncy
 ```
 
-At the moment `rsyncy` itself has no options and only supports my preferred way of viewing rsync progress.
+At the moment `rsyncy` itself has only one option, you can turn off colors via the `NO_COLOR=1` environment variable.
+
+
 
 ## lf support
 
 `rsyncy-stat` can be used to view only the status output on [lf](https://github.com/gokcehan/lf) (or similar terminal file managers).
 
 Example:
```

### Comparing `rsyncy-0.1.0/README.md` & `rsyncy-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,17 @@
 
 Alternatively you can pipe the output from rsync to rsyncy (in which case you need to specify `--info=progress2 -hv` yourself).
 
 ```
 $ rsync -a --info=progress2 -hv FROM/ TO | rsyncy
 ```
 
-At the moment `rsyncy` itself has no options and only supports my preferred way of viewing rsync progress.
+At the moment `rsyncy` itself has only one option, you can turn off colors via the `NO_COLOR=1` environment variable.
+
+
 
 ## lf support
 
 `rsyncy-stat` can be used to view only the status output on [lf](https://github.com/gokcehan/lf) (or similar terminal file managers).
 
 Example:
```

### Comparing `rsyncy-0.1.0/rsyncy` & `rsyncy-0.2.0/rsyncy`

 * *Files 3% similar despite different names*

```diff
@@ -13,50 +13,66 @@
 
 _re_chk = re.compile(r"(..)-.+=(\d+)/(\d+)")
 
 # start inline from laktakpy
 
 
 class CLI:
+    NO_COLOR = os.environ.get("NO_COLOR", "")
+
     class style:
         reset = "\033[0m"
         bold = "\033[01m"
 
     class esc:
         right = "\033[C"
 
         def clear_line(opt=0):
             # 0=to end, 1=from start, 2=all
             return "\033[" + str(opt) + "K"
 
     def get_col_bits():
+        if CLI.NO_COLOR:
+            return 1
         c, t = os.environ.get("COLORTERM", ""), os.environ.get("TERM", "")
         if c in ["truecolor", "24bit"]:
             return 24
         elif c == "8bit" or "256" in t:
             return 8
         else:
             return 4
 
     # 4bit system colors
     def fg4(col):
         # black=0,red=1,green=2,orange=3,blue=4,purple=5,cyan=6,lightgrey=7
         # darkgrey=8,lightred=9,lightgreen=10,yellow=11,lightblue=12,pink=13,lightcyan=14
-        return f"\033[{(30+col) if col<8 else (90-8+col)}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[{(30+col) if col<8 else (90-8+col)}m"
 
     def bg4(col):
         # black=0,red=1,green=2,orange=3,blue=4,purple=5,cyan=6,lightgrey=7
-        return f"\033[{40+col}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[{40+col}m"
 
     # 8bit xterm colors
     def fg8(col):
-        return f"\033[38;5;{col}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[38;5;{col}m"
 
     def bg8(col):
-        return f"\033[48;5;{col}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[48;5;{col}m"
 
     def write(*text):
         for t in text:
             sys.stdout.write(str(t))
         sys.stdout.flush()
 
     def printline(*text, sep=" ", end="\r\n"):
@@ -238,24 +254,24 @@
 
         CLI.printline("")
 
 
 def run_rsync(args, write_pipe, rc):
     # prefix rsync and add args required for progress
     args = ["rsync"] + args + ["--info=progress2", "--no-v", "-hv"]
+    p = None
     try:
         p = subprocess.Popen(args, stdout=write_pipe)
         p.wait()
     finally:
         os.close(write_pipe)
-        rc.put(p.returncode)
+        rc.put(p.returncode if p else 1)
 
 
 if __name__ == "__main__":
-
     if CLI.get_col_bits() >= 8:
         rstyle = {
             "bg": CLI.bg8(238),
             "dim": CLI.fg8(241),
             "text": CLI.fg8(250),
             "bar1": CLI.fg8(243),
             "bar2": CLI.fg8(43),
@@ -272,15 +288,14 @@
             "spin": CLI.fg4(14) + CLI.style.bold,
             "spinner": ["-", "\\", "|", "/"],
         }
     rsyncy = Rsyncy(rstyle)
     rsyncy.stat_mode = os.path.basename(sys.argv[0]) == "rsyncy-stat"
 
     try:
-
         if len(sys.argv) == 1:
             if sys.stdin.isatty():
                 print("rsyncy is an rsync wrapper with a progress bar.")
                 print(
                     "Please specify your rsync options as you normally would but use rsyncy instead of rsync."
                 )
             else:
@@ -289,11 +304,12 @@
         else:
             read_pipe, write_pipe = os.pipe()
             rc = queue.Queue()
             t = Thread(target=run_rsync, args=(sys.argv[1:], write_pipe, rc))
             t.start()
             rsyncy.read(read_pipe)
             t.join()
+
             sys.exit(rc.get())
 
     except KeyboardInterrupt:
-        pass
+        sys.exit(1)
```

### Comparing `rsyncy-0.1.0/rsyncy-stat` & `rsyncy-0.2.0/rsyncy-stat`

 * *Files 3% similar despite different names*

```diff
@@ -13,50 +13,66 @@
 
 _re_chk = re.compile(r"(..)-.+=(\d+)/(\d+)")
 
 # start inline from laktakpy
 
 
 class CLI:
+    NO_COLOR = os.environ.get("NO_COLOR", "")
+
     class style:
         reset = "\033[0m"
         bold = "\033[01m"
 
     class esc:
         right = "\033[C"
 
         def clear_line(opt=0):
             # 0=to end, 1=from start, 2=all
             return "\033[" + str(opt) + "K"
 
     def get_col_bits():
+        if CLI.NO_COLOR:
+            return 1
         c, t = os.environ.get("COLORTERM", ""), os.environ.get("TERM", "")
         if c in ["truecolor", "24bit"]:
             return 24
         elif c == "8bit" or "256" in t:
             return 8
         else:
             return 4
 
     # 4bit system colors
     def fg4(col):
         # black=0,red=1,green=2,orange=3,blue=4,purple=5,cyan=6,lightgrey=7
         # darkgrey=8,lightred=9,lightgreen=10,yellow=11,lightblue=12,pink=13,lightcyan=14
-        return f"\033[{(30+col) if col<8 else (90-8+col)}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[{(30+col) if col<8 else (90-8+col)}m"
 
     def bg4(col):
         # black=0,red=1,green=2,orange=3,blue=4,purple=5,cyan=6,lightgrey=7
-        return f"\033[{40+col}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[{40+col}m"
 
     # 8bit xterm colors
     def fg8(col):
-        return f"\033[38;5;{col}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[38;5;{col}m"
 
     def bg8(col):
-        return f"\033[48;5;{col}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[48;5;{col}m"
 
     def write(*text):
         for t in text:
             sys.stdout.write(str(t))
         sys.stdout.flush()
 
     def printline(*text, sep=" ", end="\r\n"):
@@ -238,24 +254,24 @@
 
         CLI.printline("")
 
 
 def run_rsync(args, write_pipe, rc):
     # prefix rsync and add args required for progress
     args = ["rsync"] + args + ["--info=progress2", "--no-v", "-hv"]
+    p = None
     try:
         p = subprocess.Popen(args, stdout=write_pipe)
         p.wait()
     finally:
         os.close(write_pipe)
-        rc.put(p.returncode)
+        rc.put(p.returncode if p else 1)
 
 
 if __name__ == "__main__":
-
     if CLI.get_col_bits() >= 8:
         rstyle = {
             "bg": CLI.bg8(238),
             "dim": CLI.fg8(241),
             "text": CLI.fg8(250),
             "bar1": CLI.fg8(243),
             "bar2": CLI.fg8(43),
@@ -272,15 +288,14 @@
             "spin": CLI.fg4(14) + CLI.style.bold,
             "spinner": ["-", "\\", "|", "/"],
         }
     rsyncy = Rsyncy(rstyle)
     rsyncy.stat_mode = os.path.basename(sys.argv[0]) == "rsyncy-stat"
 
     try:
-
         if len(sys.argv) == 1:
             if sys.stdin.isatty():
                 print("rsyncy is an rsync wrapper with a progress bar.")
                 print(
                     "Please specify your rsync options as you normally would but use rsyncy instead of rsync."
                 )
             else:
@@ -289,11 +304,12 @@
         else:
             read_pipe, write_pipe = os.pipe()
             rc = queue.Queue()
             t = Thread(target=run_rsync, args=(sys.argv[1:], write_pipe, rc))
             t.start()
             rsyncy.read(read_pipe)
             t.join()
+
             sys.exit(rc.get())
 
     except KeyboardInterrupt:
-        pass
+        sys.exit(1)
```

### Comparing `rsyncy-0.1.0/rsyncy.egg-info/PKG-INFO` & `rsyncy-0.2.0/rsyncy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsyncy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A status/progress bar for rsync.
 Home-page: https://github.com/laktak/rsyncy
 Author: Christian Zangl
 Author-email: laktak@cdak.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -69,15 +69,17 @@
 
 Alternatively you can pipe the output from rsync to rsyncy (in which case you need to specify `--info=progress2 -hv` yourself).
 
 ```
 $ rsync -a --info=progress2 -hv FROM/ TO | rsyncy
 ```
 
-At the moment `rsyncy` itself has no options and only supports my preferred way of viewing rsync progress.
+At the moment `rsyncy` itself has only one option, you can turn off colors via the `NO_COLOR=1` environment variable.
+
+
 
 ## lf support
 
 `rsyncy-stat` can be used to view only the status output on [lf](https://github.com/gokcehan/lf) (or similar terminal file managers).
 
 Example:
```

### Comparing `rsyncy-0.1.0/rsyncy.py` & `rsyncy-0.2.0/rsyncy.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,50 +13,66 @@
 
 _re_chk = re.compile(r"(..)-.+=(\d+)/(\d+)")
 
 # start inline from laktakpy
 
 
 class CLI:
+    NO_COLOR = os.environ.get("NO_COLOR", "")
+
     class style:
         reset = "\033[0m"
         bold = "\033[01m"
 
     class esc:
         right = "\033[C"
 
         def clear_line(opt=0):
             # 0=to end, 1=from start, 2=all
             return "\033[" + str(opt) + "K"
 
     def get_col_bits():
+        if CLI.NO_COLOR:
+            return 1
         c, t = os.environ.get("COLORTERM", ""), os.environ.get("TERM", "")
         if c in ["truecolor", "24bit"]:
             return 24
         elif c == "8bit" or "256" in t:
             return 8
         else:
             return 4
 
     # 4bit system colors
     def fg4(col):
         # black=0,red=1,green=2,orange=3,blue=4,purple=5,cyan=6,lightgrey=7
         # darkgrey=8,lightred=9,lightgreen=10,yellow=11,lightblue=12,pink=13,lightcyan=14
-        return f"\033[{(30+col) if col<8 else (90-8+col)}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[{(30+col) if col<8 else (90-8+col)}m"
 
     def bg4(col):
         # black=0,red=1,green=2,orange=3,blue=4,purple=5,cyan=6,lightgrey=7
-        return f"\033[{40+col}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[{40+col}m"
 
     # 8bit xterm colors
     def fg8(col):
-        return f"\033[38;5;{col}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[38;5;{col}m"
 
     def bg8(col):
-        return f"\033[48;5;{col}m"
+        if CLI.NO_COLOR:
+            return ""
+        else:
+            return f"\033[48;5;{col}m"
 
     def write(*text):
         for t in text:
             sys.stdout.write(str(t))
         sys.stdout.flush()
 
     def printline(*text, sep=" ", end="\r\n"):
@@ -238,24 +254,24 @@
 
         CLI.printline("")
 
 
 def run_rsync(args, write_pipe, rc):
     # prefix rsync and add args required for progress
     args = ["rsync"] + args + ["--info=progress2", "--no-v", "-hv"]
+    p = None
     try:
         p = subprocess.Popen(args, stdout=write_pipe)
         p.wait()
     finally:
         os.close(write_pipe)
-        rc.put(p.returncode)
+        rc.put(p.returncode if p else 1)
 
 
 if __name__ == "__main__":
-
     if CLI.get_col_bits() >= 8:
         rstyle = {
             "bg": CLI.bg8(238),
             "dim": CLI.fg8(241),
             "text": CLI.fg8(250),
             "bar1": CLI.fg8(243),
             "bar2": CLI.fg8(43),
@@ -272,15 +288,14 @@
             "spin": CLI.fg4(14) + CLI.style.bold,
             "spinner": ["-", "\\", "|", "/"],
         }
     rsyncy = Rsyncy(rstyle)
     rsyncy.stat_mode = os.path.basename(sys.argv[0]) == "rsyncy-stat"
 
     try:
-
         if len(sys.argv) == 1:
             if sys.stdin.isatty():
                 print("rsyncy is an rsync wrapper with a progress bar.")
                 print(
                     "Please specify your rsync options as you normally would but use rsyncy instead of rsync."
                 )
             else:
@@ -289,11 +304,12 @@
         else:
             read_pipe, write_pipe = os.pipe()
             rc = queue.Queue()
             t = Thread(target=run_rsync, args=(sys.argv[1:], write_pipe, rc))
             t.start()
             rsyncy.read(read_pipe)
             t.join()
+
             sys.exit(rc.get())
 
     except KeyboardInterrupt:
-        pass
+        sys.exit(1)
```

### Comparing `rsyncy-0.1.0/setup.py` & `rsyncy-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="rsyncy",
-    version="0.1.0",
+    version="0.2.0",
     url="https://github.com/laktak/rsyncy",
     author="Christian Zangl",
     author_email="laktak@cdak.net",
     description="A status/progress bar for rsync.",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=[],
```

