# Comparing `tmp/cursesplus-2.3.6.tar.gz` & `tmp/cursesplus-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.3.6.tar", last modified: Wed Jun  7 20:51:52 2023, max compression
+gzip compressed data, was "cursesplus-2.3.7.tar", last modified: Fri Jun 30 18:59:43 2023, max compression
```

## Comparing `cursesplus-2.3.6.tar` & `cursesplus-2.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-07 20:51:52.387706 cursesplus-2.3.6/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.6/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1474 2023-06-07 20:51:52.387706 cursesplus-2.3.6/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      871 2023-06-07 20:51:08.000000 cursesplus-2.3.6/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-07 20:51:13.000000 cursesplus-2.3.6/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-07 20:51:52.387706 cursesplus-2.3.6/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-07 20:51:52.387706 cursesplus-2.3.6/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      358 2023-06-07 20:50:43.000000 cursesplus-2.3.6/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-07 20:51:52.387706 cursesplus-2.3.6/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.6/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    16614 2023-06-07 20:49:54.000000 cursesplus-2.3.6/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.6/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.6/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-07 20:51:52.387706 cursesplus-2.3.6/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1474 2023-06-07 20:51:52.000000 cursesplus-2.3.6/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-07 20:51:52.000000 cursesplus-2.3.6/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-07 20:51:52.000000 cursesplus-2.3.6/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-07 20:51:52.000000 cursesplus-2.3.6/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-30 18:59:43.587034 cursesplus-2.3.7/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.7/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1457 2023-06-30 18:59:43.587034 cursesplus-2.3.7/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      854 2023-06-30 18:59:24.000000 cursesplus-2.3.7/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-30 18:59:12.000000 cursesplus-2.3.7/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-30 18:59:43.597034 cursesplus-2.3.7/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-30 18:59:43.587034 cursesplus-2.3.7/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      357 2023-06-30 18:52:19.000000 cursesplus-2.3.7/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-30 18:59:43.587034 cursesplus-2.3.7/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.7/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    17144 2023-06-30 18:58:46.000000 cursesplus-2.3.7/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.7/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.7/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-30 18:59:43.587034 cursesplus-2.3.7/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1457 2023-06-30 18:59:43.000000 cursesplus-2.3.7/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-30 18:59:43.000000 cursesplus-2.3.7/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-30 18:59:43.000000 cursesplus-2.3.7/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-30 18:59:43.000000 cursesplus-2.3.7/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.3.6/LICENSE` & `cursesplus-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.6/PKG-INFO` & `cursesplus-2.3.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.6
+Version: 2.3.7
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.6:
+### Patch 2.3.7:
 
--Add ability to prefill text in new input
+-Fix bugs in cursesinput
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

### Comparing `cursesplus-2.3.6/README.md` & `cursesplus-2.3.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.6:
+### Patch 2.3.7:
 
--Add ability to prefill text in new input
+-Fix bugs in cursesinput
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

### Comparing `cursesplus-2.3.6/pyproject.toml` & `cursesplus-2.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.3.6"
+version = "2.3.7"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.3.6/src/cursesplus/__init__.py` & `cursesplus-2.3.7/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.6/src/cursesplus/cp.py` & `cursesplus-2.3.7/src/cursesplus/cp.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     return [l for l in input if str(l) != ""]  
 def __calc_nbl_list(input:list)->int:
     x = 0
     for ls in input:
         x += len(ls)
     return x
 
-def cursesinput(stdscr,prompt: str,lines=1,maxlen=0,passwordchar:str|None=None,retremptylines=False,prefiltext="") -> str:
+def cursesinput(stdscr,prompt: str,lines=1,maxlen=0,passwordchar:str=None,retremptylines=False,prefiltext="") -> str:
     """
     Get input from the user. Set maxlen to 0 for no maximum. Set passwordchar to None for no password entry. Retremptylines is if the program should return newlines even if the lines are empty
     """
     ERROR = ""
     if passwordchar is not None:
         passworduse = True
     else:
@@ -160,22 +160,37 @@
         stdscr.move(ln+2,col-xoffset+1)
         
         if ERROR != "":
             ERROR = ""
         stdscr.refresh()
         ch = stdscr.getch()
         chn = curses.keyname(ch)
-        if ch == 10 or ch == 13 or ch == curses.KEY_ENTER or ch == curses.KEY_DOWN:
+        if ch == 10 or ch == 13 or ch == curses.KEY_ENTER :
             if lines == 1:
                 stdscr.erase()
                 return "\n".join(["".join(t) for t in text])
             if ln == lines - 1:
                 ERROR = " You have reached the bottom of the page. "
                 curses.beep()
             else:
+                if col < len(text[ln]) - 1:
+                    #Shift down
+                    text[ln+1] = text[ln][col:] + text[ln+1]
+                    stdscr.clear()
+                    if col > 0:
+                        del text[ln][col:]
+                    else:
+                        text[ln] = []
+                ln += 1
+                col = 0
+        elif ch == curses.KEY_DOWN:
+            if ln == lines - 1:
+                ERROR = " You have reached the bottom of the page. "
+                curses.beep()
+            else:
                 ln += 1
                 col = 0
         elif ch == curses.KEY_LEFT:
             if col > 0:
                 col -= 1
                 if xoffset > 0:
                     xoffset -= 1
```

### Comparing `cursesplus-2.3.6/src/cursesplus/filedialog.py` & `cursesplus-2.3.7/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.6/src/cursesplus/messagebox.py` & `cursesplus-2.3.7/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.6/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.3.7/src/cursesplus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.6
+Version: 2.3.7
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.6:
+### Patch 2.3.7:
 
--Add ability to prefill text in new input
+-Fix bugs in cursesinput
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

