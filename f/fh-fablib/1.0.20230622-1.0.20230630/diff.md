# Comparing `tmp/fh_fablib-1.0.20230622.tar.gz` & `tmp/fh_fablib-1.0.20230630.tar.gz`

## Comparing `fh_fablib-1.0.20230622.tar` & `fh_fablib-1.0.20230630.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/.editorconfig
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/.pre-commit-config.yaml
--rw-r--r--   0        0        0    19712 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/CHANGELOG.rst
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/bumpversion.sh
--rw-r--r--   0        0        0    26616 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/__init__.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/extract_js_gettext_strings.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/.editorconfig
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/.eslintrc.js
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/pyproject.toml
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/webpack.library.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/.gitignore
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/LICENSE
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/README.rst
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/pyproject.toml
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/.editorconfig
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    19912 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/CHANGELOG.rst
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/bumpversion.sh
+-rw-r--r--   0        0        0    26697 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/__init__.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/extract_js_gettext_strings.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/.editorconfig
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/.eslintrc.js
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/pyproject.toml
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/webpack.library.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/LICENSE
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/README.rst
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/pyproject.toml
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/PKG-INFO
```

### Comparing `fh_fablib-1.0.20230622/.pre-commit-config.yaml` & `fh_fablib-1.0.20230630/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230622/CHANGELOG.rst` & `fh_fablib-1.0.20230630/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 ==========
 Change log
 ==========
 
 Next version
 ~~~~~~~~~~~~
 
+1.0.20230630
+~~~~~~~~~~~~
+
+- Fixed the ``find`` command which deletes old ``static`` files.
+- Updated the example Webpack configuration to work with the newest version of
+  ``postcss-custom-media``.
+
 1.0.20230622
 ~~~~~~~~~~~~
 
 - Changed the JavaScript string extractor to strip trailing commas from
   argument lists.
 - Switched to not deleting everything under ``static/`` when deploying, only
   delete old files.
```

### Comparing `fh_fablib-1.0.20230622/fh_fablib/__init__.py` & `fh_fablib-1.0.20230630/fh_fablib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fabric import Connection, task
 from invoke import Collection  # noqa, re-export
 from speckenv_django import django_database_url
 
 from fh_fablib.extract_js_gettext_strings import generate_strings
 
 
-__version__ = "1.0.20230622"
+__version__ = "1.0.20230630"
 
 
 # I don't care, in this context.
 warnings.simplefilter("ignore", category=ResourceWarning)
 
 
 def ansi(code):
@@ -882,15 +882,18 @@
     if not fast:
         run_local(ctx, "NODE_ENV=production yarn run webpack --mode production --bail")
 
     with Connection(config.host) as conn, conn.cd(config.domain):
         _deploy_sync_origin_url(ctx, conn)
         _deploy_django(conn)
         if not fast:
-            run(conn, "find static/ -mtime +60 -delete")
+            run(
+                conn,
+                "if [ -e static ]; then find static/ -type f -mtime +60 -delete;fi",
+            )
             _rsync_static(ctx, delete=False)
         _deploy_staticfiles(conn)
         _nine_restart(conn)
 
     fetch(ctx)
     progress(f"Successfully deployed the {config.environment} environment.")
```

### Comparing `fh_fablib-1.0.20230622/fh_fablib/extract_js_gettext_strings.py` & `fh_fablib-1.0.20230630/fh_fablib/extract_js_gettext_strings.py`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230622/fh_fablib/dotfiles/.pre-commit-config.yaml` & `fh_fablib-1.0.20230630/fh_fablib/dotfiles/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230622/fh_fablib/dotfiles/pyproject.toml` & `fh_fablib-1.0.20230630/fh_fablib/dotfiles/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230622/fh_fablib/dotfiles/webpack.library.js` & `fh_fablib-1.0.20230630/fh_fablib/dotfiles/webpack.library.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -11,17 +11,20 @@
         ...base,
         devServer: devServer({ backendPort: env.backend }),
         module: {
           rules: [
             assetRule(),
             postcssRule({
               plugins: [
-                "postcss-nested",
-                "postcss-import",
+                [
+                  "@csstools/postcss-global-data",
+                  { files: ["./frontend/custom-media.css"] },
+                ],
                 "postcss-custom-media",
+                "postcss-nesting",
                 "autoprefixer",
               ],
             }),
             babelWithPreactRule(),
           ],
         },
       }
```

### Comparing `fh_fablib-1.0.20230622/LICENSE` & `fh_fablib-1.0.20230630/LICENSE`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230622/README.rst` & `fh_fablib-1.0.20230630/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230622")
+       fl.require("1.0.20230630")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -90,15 +90,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230622")
+    fl.require("1.0.20230630")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20230622/pyproject.toml` & `fh_fablib-1.0.20230630/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230622/PKG-INFO` & `fh_fablib-1.0.20230630/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fh-fablib
-Version: 1.0.20230622
+Version: 1.0.20230630
 Summary: fh-fablib
 Project-URL: Homepage, https://github.com/feinheit/fh-fablib/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9
@@ -28,15 +28,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230622")
+       fl.require("1.0.20230630")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -104,15 +104,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230622")
+    fl.require("1.0.20230630")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

