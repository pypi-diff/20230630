# Comparing `tmp/bibleit-0.0.8.tar.gz` & `tmp/bibleit-0.0.9.tar.gz`

## Comparing `bibleit-0.0.8.tar` & `bibleit-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bibleit-0.0.8/Makefile
--rwxr-xr-x   0        0        0      753 2020-02-02 00:00:00.000000 bibleit-0.0.8/bump-version.sh
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bibleit-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/__main__.py
--rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/bible.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/config.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/context.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/normalize.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/repl.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/command/__init__.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/command/core.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/command/set.py
--rw-r--r--   0        0        0  4355983 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/translations/acf
--rw-r--r--   0        0        0  4874923 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/translations/kjv
--rw-r--r--   0        0        0  4347261 2020-02-02 00:00:00.000000 bibleit-0.0.8/src/bibleit/translations/nvi
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 bibleit-0.0.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bibleit-0.0.8/LICENSE
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 bibleit-0.0.8/README.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bibleit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 bibleit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bibleit-0.0.9/Makefile
+-rwxr-xr-x   0        0        0      753 2020-02-02 00:00:00.000000 bibleit-0.0.9/bump-version.sh
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bibleit-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/__main__.py
+-rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/bible.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/config.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/context.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/normalize.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/repl.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/command/__init__.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/command/core.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/command/set.py
+-rw-r--r--   0        0        0  4355983 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/translations/acf
+-rw-r--r--   0        0        0  4874923 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/translations/kjv
+-rw-r--r--   0        0        0  4347261 2020-02-02 00:00:00.000000 bibleit-0.0.9/src/bibleit/translations/nvi
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 bibleit-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bibleit-0.0.9/LICENSE
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 bibleit-0.0.9/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bibleit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 bibleit-0.0.9/PKG-INFO
```

### Comparing `bibleit-0.0.8/bump-version.sh` & `bibleit-0.0.9/bump-version.sh`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/.github/workflows/publish.yml` & `bibleit-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/src/bibleit/bible.py` & `bibleit-0.0.9/src/bibleit/bible.py`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/src/bibleit/normalize.py` & `bibleit-0.0.9/src/bibleit/normalize.py`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/src/bibleit/repl.py` & `bibleit-0.0.9/src/bibleit/repl.py`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/src/bibleit/command/__init__.py` & `bibleit-0.0.9/src/bibleit/command/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         if name in ctx.methods:
             fn = getattr(ctx.module, name)
             nargs = [normalize.normalize(arg) for arg in args]
             return fn(ctx, *nargs)
     except AssertionError as e:
         print(f"Error: {e}")
     except Exception as e:
+        print(f"*** {e}\n")
         if config.debug:
-            print("Debug:", e)
             print(traceback.format_exc())
         if module != _default_module:
             core.help(ctx, *[module, *line])
         else:
             core.help(ctx, name)
     else:
         print(f"Error: command '{target}' not found")
```

### Comparing `bibleit-0.0.8/src/bibleit/command/core.py` & `bibleit-0.0.9/src/bibleit/command/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,7 +133,23 @@
      https://www.blueletterbible.org/help/bible_search.cfm
 
 https://www.blueletterbible.org | ©2022 Blue Letter Bible"""
     target = " ".join(args)
     assert target, "you should use blb <terms>"
     _wb.open(f"https://www.blueletterbible.org/search/preSearch.cfm?Criteria={target}")
     return None
+
+
+def notes(ctx, *args):
+    """List all notes."""
+    return "\n".join(ctx.notes) if ctx.notes else None
+
+
+def note(ctx, *args):
+    """Adds a new note.
+    
+     notes <string>"""
+    target = " ".join(args)
+
+    assert target, "you should use notes <string>"
+    ctx.add_note(target)
+    return None
```

### Comparing `bibleit-0.0.8/src/bibleit/command/set.py` & `bibleit-0.0.9/src/bibleit/command/set.py`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/src/bibleit/translations/acf` & `bibleit-0.0.9/src/bibleit/translations/acf`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/src/bibleit/translations/kjv` & `bibleit-0.0.9/src/bibleit/translations/kjv`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/src/bibleit/translations/nvi` & `bibleit-0.0.9/src/bibleit/translations/nvi`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/.gitignore` & `bibleit-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/LICENSE` & `bibleit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bibleit-0.0.8/pyproject.toml` & `bibleit-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bibleit"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Felipe Mamud", email="trovatti@gmail.com" },
 ]
 description = "Interactive bible reading"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `bibleit-0.0.8/PKG-INFO` & `bibleit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibleit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interactive bible reading
 Project-URL: Homepage, https://github.com/fmamud/bibleit
 Project-URL: Bug Tracker, https://github.com/fmamud/bibleit/issues
 Author-email: Felipe Mamud <trovatti@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Felipe Mamud
```

