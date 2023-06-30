# Comparing `tmp/quickstatements_client-0.0.2.tar.gz` & `tmp/quickstatements_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstatements_client-0.0.2.tar", last modified: Sun Feb 26 13:24:33 2023, max compression
+gzip compressed data, was "quickstatements_client-0.0.3.tar", last modified: Fri Jun 30 12:23:08 2023, max compression
```

## Comparing `quickstatements_client-0.0.2.tar` & `quickstatements_client-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,47 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-26 13:24:33.592920 quickstatements_client-0.0.2/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-02-25 17:43:09.000000 quickstatements_client-0.0.2/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      399 2023-02-25 17:43:09.000000 quickstatements_client-0.0.2/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     9795 2023-02-26 13:24:33.593090 quickstatements_client-0.0.2/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     8376 2023-02-25 21:22:03.000000 quickstatements_client-0.0.2/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-26 13:24:33.575487 quickstatements_client-0.0.2/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-26 13:24:33.581761 quickstatements_client-0.0.2/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)      291 2023-02-25 17:43:09.000000 quickstatements_client-0.0.2/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7382 2023-02-26 13:24:32.000000 quickstatements_client-0.0.2/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      383 2023-02-25 19:00:39.000000 quickstatements_client-0.0.2/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      579 2023-02-25 17:43:09.000000 quickstatements_client-0.0.2/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      132 2023-02-25 18:53:21.000000 quickstatements_client-0.0.2/docs/source/usage.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      377 2023-02-25 17:43:09.000000 quickstatements_client-0.0.2/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2634 2023-02-26 13:24:33.594001 quickstatements_client-0.0.2/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-26 13:24:33.576176 quickstatements_client-0.0.2/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-26 13:24:33.585879 quickstatements_client-0.0.2/src/quickstatements_client/
--rw-r--r--   0 cthoyt     (501) staff       (20)      644 2023-02-25 21:01:30.000000 quickstatements_client-0.0.2/src/quickstatements_client/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      339 2023-02-25 17:43:09.000000 quickstatements_client-0.0.2/src/quickstatements_client/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      939 2023-02-25 17:43:09.000000 quickstatements_client-0.0.2/src/quickstatements_client/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2871 2023-02-26 13:24:26.000000 quickstatements_client-0.0.2/src/quickstatements_client/client.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     6985 2023-02-26 13:24:26.000000 quickstatements_client-0.0.2/src/quickstatements_client/model.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-02-25 17:43:09.000000 quickstatements_client-0.0.2/src/quickstatements_client/py.typed
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-26 13:24:33.590104 quickstatements_client-0.0.2/src/quickstatements_client/sources/
--rw-r--r--   0 cthoyt     (501) staff       (20)       77 2023-02-26 13:24:26.000000 quickstatements_client-0.0.2/src/quickstatements_client/sources/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     9870 2023-02-26 13:24:26.000000 quickstatements_client-0.0.2/src/quickstatements_client/sources/licenses.json
--rw-r--r--   0 cthoyt     (501) staff       (20)     7518 2023-02-26 13:24:26.000000 quickstatements_client-0.0.2/src/quickstatements_client/sources/pypi.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1122 2023-02-26 13:24:26.000000 quickstatements_client-0.0.2/src/quickstatements_client/sources/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1064 2023-02-26 13:24:32.000000 quickstatements_client-0.0.2/src/quickstatements_client/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-26 13:24:33.588725 quickstatements_client-0.0.2/src/quickstatements_client.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     9795 2023-02-26 13:24:33.000000 quickstatements_client-0.0.2/src/quickstatements_client.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1023 2023-02-26 13:24:33.000000 quickstatements_client-0.0.2/src/quickstatements_client.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-02-26 13:24:33.000000 quickstatements_client-0.0.2/src/quickstatements_client.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       75 2023-02-26 13:24:33.000000 quickstatements_client-0.0.2/src/quickstatements_client.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-02-25 18:33:35.000000 quickstatements_client-0.0.2/src/quickstatements_client.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      153 2023-02-26 13:24:33.000000 quickstatements_client-0.0.2/src/quickstatements_client.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       23 2023-02-26 13:24:33.000000 quickstatements_client-0.0.2/src/quickstatements_client.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-26 13:24:33.592418 quickstatements_client-0.0.2/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       72 2023-02-25 17:43:09.000000 quickstatements_client-0.0.2/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)   184010 2022-10-11 22:04:04.000000 quickstatements_client-0.0.2/tests/sample_orcid.json
--rw-r--r--   0 cthoyt     (501) staff       (20)     4109 2023-02-25 19:11:23.000000 quickstatements_client-0.0.2/tests/test_models.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.074242 quickstatements_client-0.0.3/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-02-25 17:43:09.000000 quickstatements_client-0.0.3/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      399 2023-02-25 17:43:09.000000 quickstatements_client-0.0.3/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9795 2023-06-30 12:23:08.074392 quickstatements_client-0.0.3/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8376 2023-02-26 14:22:10.000000 quickstatements_client-0.0.3/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.050459 quickstatements_client-0.0.3/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.057052 quickstatements_client-0.0.3/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      291 2023-02-25 17:43:09.000000 quickstatements_client-0.0.3/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7395 2023-06-30 12:23:07.000000 quickstatements_client-0.0.3/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      383 2023-02-25 19:00:39.000000 quickstatements_client-0.0.3/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      579 2023-02-25 17:43:09.000000 quickstatements_client-0.0.3/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      132 2023-02-25 18:53:21.000000 quickstatements_client-0.0.3/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      377 2023-02-25 17:43:09.000000 quickstatements_client-0.0.3/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2638 2023-06-30 12:23:08.075971 quickstatements_client-0.0.3/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.051272 quickstatements_client-0.0.3/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.061478 quickstatements_client-0.0.3/src/quickstatements_client/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      644 2023-02-25 21:01:30.000000 quickstatements_client-0.0.3/src/quickstatements_client/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      339 2023-02-25 17:43:09.000000 quickstatements_client-0.0.3/src/quickstatements_client/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      939 2023-02-25 17:43:09.000000 quickstatements_client-0.0.3/src/quickstatements_client/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2931 2023-06-28 11:59:30.000000 quickstatements_client-0.0.3/src/quickstatements_client/client.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.065719 quickstatements_client-0.0.3/src/quickstatements_client/language_codes/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      532 2023-06-30 12:21:29.000000 quickstatements_client-0.0.3/src/quickstatements_client/language_codes/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4444 2023-06-30 12:21:29.000000 quickstatements_client-0.0.3/src/quickstatements_client/language_codes/data.json
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.067844 quickstatements_client-0.0.3/src/quickstatements_client/maintenance/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       52 2023-05-28 12:30:24.000000 quickstatements_client-0.0.3/src/quickstatements_client/maintenance/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1192 2023-06-28 11:59:30.000000 quickstatements_client-0.0.3/src/quickstatements_client/maintenance/annotate_missing_followed_by.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1202 2023-06-28 11:59:30.000000 quickstatements_client-0.0.3/src/quickstatements_client/maintenance/annotate_missing_follows.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8026 2023-06-30 12:21:29.000000 quickstatements_client-0.0.3/src/quickstatements_client/model.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-02-25 17:43:09.000000 quickstatements_client-0.0.3/src/quickstatements_client/py.typed
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.070358 quickstatements_client-0.0.3/src/quickstatements_client/sources/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       77 2023-02-26 13:24:26.000000 quickstatements_client-0.0.3/src/quickstatements_client/sources/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9870 2023-02-26 13:24:26.000000 quickstatements_client-0.0.3/src/quickstatements_client/sources/licenses.json
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7729 2023-06-28 11:59:30.000000 quickstatements_client-0.0.3/src/quickstatements_client/sources/pypi.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1314 2023-06-28 11:59:30.000000 quickstatements_client-0.0.3/src/quickstatements_client/sources/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1064 2023-06-30 12:23:07.000000 quickstatements_client-0.0.3/src/quickstatements_client/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.064972 quickstatements_client-0.0.3/src/quickstatements_client.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9795 2023-06-30 12:23:07.000000 quickstatements_client-0.0.3/src/quickstatements_client.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1318 2023-06-30 12:23:08.000000 quickstatements_client-0.0.3/src/quickstatements_client.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-06-30 12:23:07.000000 quickstatements_client-0.0.3/src/quickstatements_client.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       75 2023-06-30 12:23:07.000000 quickstatements_client-0.0.3/src/quickstatements_client.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-02-25 18:33:35.000000 quickstatements_client-0.0.3/src/quickstatements_client.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      157 2023-06-30 12:23:07.000000 quickstatements_client-0.0.3/src/quickstatements_client.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       23 2023-06-30 12:23:07.000000 quickstatements_client-0.0.3/src/quickstatements_client.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-30 12:23:08.073924 quickstatements_client-0.0.3/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       72 2023-02-25 17:43:09.000000 quickstatements_client-0.0.3/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)   184010 2022-10-11 22:04:04.000000 quickstatements_client-0.0.3/tests/sample_orcid.json
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5265 2023-06-30 12:21:29.000000 quickstatements_client-0.0.3/tests/test_models.py
```

### Comparing `quickstatements_client-0.0.2/LICENSE` & `quickstatements_client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickstatements_client-0.0.2/PKG-INFO` & `quickstatements_client-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstatements_client
-Version: 0.0.2
+Version: 0.0.3
 Summary: A data model and client for Wikidata QuickStatements
 Home-page: https://github.com/cthoyt/quickstatements-client
 Download-URL: https://github.com/cthoyt/quickstatements-client/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quickstatements_client Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: quickstatements_client Version: 0.0.3 Summary: A
 data model and client for Wikidata QuickStatements Home-page: https://
 github.com/cthoyt/quickstatements-client Download-URL: https://github.com/
 cthoyt/quickstatements-client/releases Author: Charles Tapley Hoyt Author-
 email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-email:
 cthoyt@gmail.com License: MIT Project-URL: Bug Tracker, https://github.com/
 cthoyt/quickstatements-client/issues Project-URL: Source Code, https://
 github.com/cthoyt/quickstatements-client Keywords:
```

### Comparing `quickstatements_client-0.0.2/README.md` & `quickstatements_client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `quickstatements_client-0.0.2/docs/source/conf.py` & `quickstatements_client-0.0.3/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "quickstatements_client"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.0.2"
+release = "0.0.3"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
@@ -136,15 +136,15 @@
 #
 if os.path.exists("logo.png"):
     html_logo = "logo.png"
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = "QuickStatements Clientdoc"
+htmlhelp_basename = "quickstatements_client_doc"
 
 # -- Options for LaTeX output ------------------------------------------------
 
 # latex_elements = {
 #     The paper size ('letterpaper' or 'a4paper').
 #
 #     'papersize': 'letterpaper',
@@ -225,15 +225,15 @@
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "https://docs.python.org/3/": None,
+    "python": ("https://docs.python.org/3/", None),
     "pandas": ("https://pandas.pydata.org/docs/", None),
     "sklearn": ("https://scikit-learn.org/stable/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
 }
 
 autoclass_content = "both"
```

### Comparing `quickstatements_client-0.0.2/docs/source/installation.rst` & `quickstatements_client-0.0.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `quickstatements_client-0.0.2/setup.cfg` & `quickstatements_client-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = quickstatements_client
-version = 0.0.2
+version = 0.0.3
 description = A data model and client for Wikidata QuickStatements
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/quickstatements-client
 download_url = https://github.com/cthoyt/quickstatements-client/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/quickstatements-client/issues
@@ -56,15 +56,15 @@
 where = src
 
 [options.extras_require]
 tests = 
 	pytest
 	coverage
 docs = 
-	sphinx
+	sphinx<7.0
 	sphinx-rtd-theme
 	sphinx-click
 	sphinx-autodoc-typehints
 	sphinx_automodapi
 
 [options.entry_points]
 console_scripts =
```

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client/__init__.py` & `quickstatements_client-0.0.3/src/quickstatements_client/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client/cli.py` & `quickstatements_client-0.0.3/src/quickstatements_client/cli.py`

 * *Files identical despite different names*

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client/client.py` & `quickstatements_client-0.0.3/src/quickstatements_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,19 @@
         """Post a batch of QuickStatements with an optional name."""
         params = Post(
             username=self.username,
             token=self.token,
             data=render_lines(lines),
             batchname=batch_name,
         )
-        res = requests.post(self.endpoint, data=params.dict())
+        res = requests.post(
+            self.endpoint,
+            data=params.dict(),
+            timeout=300,
+        )
         return Response.parse_obj(res.json())
 
     @staticmethod
     def open_new_tab(lines: Sequence[Line]):
         """Open a web browser on the host system."""
         return webbrowser.open_new_tab(lines_to_url(lines))
```

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client/model.py` & `quickstatements_client-0.0.3/src/quickstatements_client/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import webbrowser
 from typing import Iterable, List, Optional, Sequence, Type, Union
 from urllib.parse import quote
 
 from pydantic import BaseModel, Field
 from typing_extensions import Annotated, Literal, get_args
 
+from .language_codes import LANGUAGE_CODES
+
 __all__ = [
     # Data model
     "EntityQualifier",
     "DateQualifier",
     "TextQualifier",
     "Qualifier",
     "CreateLine",
@@ -58,14 +60,23 @@
     @classmethod
     def end_time(
         cls, target: Union[str, datetime.datetime], *, precision: Optional[int] = None
     ) -> "DateQualifier":
         """Get a qualifier for an end time."""
         return cls(predicate="P582", target=prepare_date(target, precision=precision))
 
+    @classmethod
+    def retrieved(
+        cls, namespace: Literal["P", "S"], precision: Optional[int] = 11
+    ) -> "DateQualifier":
+        """Get a qualifier for retrieving data now."""
+        # FIXME this doesn't appear to work with higher granularity like 14
+        now = datetime.datetime.now()
+        return cls(predicate=f"{namespace}813", target=prepare_date(now, precision=precision))
+
 
 def format_date(
     *,
     precision: int,
     year: int,
     month: int = 0,
     day: int = 0,
@@ -156,16 +167,30 @@
 
 
 class BaseLine(BaseModel):
     """A shared model for entity and text lines."""
 
     subject: str = Field(regex=r"^(LAST)|(Q\d+)$")
     predicate: str = Field(
-        regex=r"^(P\d+)|(Len)|(Den)$",
-        description="Either a predicate, `Len` (label), or `Den` (description)",
+        regex=rf"^(P\d+)|([ADL]({'|'.join(LANGUAGE_CODES)}))$",
+        description="""\
+        The predicate can be one of two things:
+
+        1. A Wikidata predicate, which starts with an upper case letter P, followed by a sequence of digits
+        2. A combination of a single letter command code and an ISO639 language code.
+           The single letter command codes can be:
+           - ``L`` for label
+           - ``A`` for alias (i.e., synonym)
+           - ``D`` for description
+
+           See Wikidata documentation at https://www.wikidata.org/w/index.php?title=Help:QuickStatements&\
+section=6#Adding_labels,_aliases,_descriptions_and_sitelinks
+
+        To do: add support for sitelinks.
+        """,
     )
     qualifiers: List[Qualifier] = Field(default_factory=list)
 
     def get_target(self) -> str:
         """Get the target of the line."""
         return self.target
```

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client/sources/licenses.json` & `quickstatements_client-0.0.3/src/quickstatements_client/sources/licenses.json`

 * *Files identical despite different names*

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client/sources/pypi.py` & `quickstatements_client-0.0.3/src/quickstatements_client/sources/pypi.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pathlib import Path
 from typing import Iterable, Mapping, Optional, Sequence
 
 import requests
 
 from quickstatements_client.model import (
     CreateLine,
+    DateQualifier,
     EntityLine,
     EntityQualifier,
     Line,
     TextLine,
     TextQualifier,
     lines_to_new_tab,
 )
@@ -110,15 +111,17 @@
         .. warning::
 
             Use this with care, as not all entries on Wikidata are
             fully annotated, and this could lead to duplicate entries
     :yields: QuickStatements lines
     """
     pypi_project = pypi_project.replace("_", "-")
-    metadata = requests.get(f"https://pypi.org/pypi/{pypi_project}/json").json()["info"]
+    metadata = requests.get(f"https://pypi.org/pypi/{pypi_project}/json", timeout=300).json()[
+        "info"
+    ]
 
     package_qid = get_package_qid(pypi_project)
     if not package_qid:
         if not create:
             return
         yield CreateLine()
         package_qid = "LAST"
@@ -126,91 +129,93 @@
         yield TextLine(subject=package_qid, predicate="Len", target=name)
         yield TextLine(subject=package_qid, predicate="Den", target="Python software package")
 
     pypi_qualifier = TextQualifier(
         predicate="S854",  # reference URL
         target=f"https://pypi.org/project/{pypi_project}",
     )
+    retrieved_qualifier = DateQualifier.retrieved(namespace="S")
+    qualifiers = [pypi_qualifier, retrieved_qualifier]
 
     yield EntityLine(
         subject=package_qid,
         predicate="P31",  # instance of
         target="Q29642950",  # Python library
-        qualifiers=[pypi_qualifier],
+        qualifiers=qualifiers,
     )
     yield EntityLine(
         subject=package_qid,
         predicate="P31",  # instance of
         target="Q7397",  # software
-        qualifiers=[pypi_qualifier],
+        qualifiers=qualifiers,
     )
     yield EntityLine(
         subject=package_qid,
         predicate="P277",  # programmed in
         target="Q28865",  # Python
-        qualifiers=[pypi_qualifier],
+        qualifiers=qualifiers,
     )
     yield TextLine(
         subject=package_qid,
         predicate="P5568",  # PyPI Project
         target=pypi_project,
-        qualifiers=[pypi_qualifier],
+        qualifiers=qualifiers,
     )
 
     license_qid = get_license_qid(metadata.get("license") or "")
     if license_qid:
         yield EntityLine(
             subject=package_qid,
             predicate="P6216",  # copyright status
             target="Q50423863",  # copyrighted
-            qualifiers=[pypi_qualifier],
+            qualifiers=qualifiers,
         )
         yield EntityLine(
             subject=package_qid,
             predicate="P275",  # copyright license
             target=license_qid,
-            qualifiers=[pypi_qualifier],
+            qualifiers=qualifiers,
         )
 
     docs_url = metadata.get("docs_url")
     if docs_url:
         yield TextLine(
             subject=package_qid,
             predicate="P2078",  # user manual URL
             target=docs_url.rstrip("/"),
-            qualifiers=[pypi_qualifier],
+            qualifiers=qualifiers,
         )
 
     project_urls = metadata.get("project_urls") or {}
     for predicate, keys in [
         ("P856", ["homepage"]),  # official website
         ("P1401", ["tracker", "bug tracker"]),  # issue tracker URL
     ]:
         target_url = _dict_get(project_urls, keys)
         if not target_url:
             continue
         yield TextLine(
             subject=package_qid,
             predicate=predicate,
             target=target_url.rstrip("/"),
-            qualifiers=[pypi_qualifier],
+            qualifiers=qualifiers,
         )
 
     for url in [
         _dict_get(project_urls, ["homepage"]),
         _dict_get(project_urls, ["source", "source code"]),
         metadata.get("home_page", ""),
     ]:
         if url and url.startswith("https://github.com/"):
             yield TextLine(
                 subject=package_qid,
                 predicate="P1324",  # source code repository
                 target=url.rstrip("/"),
                 qualifiers=[
-                    pypi_qualifier,
+                    *qualifiers,
                     git_qualifier,
                     github_qualifier,
                 ],
             )
             break
 
     for requirement in metadata.get("requires_dist") or []:
@@ -223,15 +228,15 @@
         if not requirement_qid:
             logger.warning(f"[pypi:{pypi_project}] could not look up requirement: {parts[0]}")
             continue
         yield EntityLine(
             subject=package_qid,
             predicate="P1547",  # depends on software
             target=requirement_qid,
-            qualifiers=[pypi_qualifier],
+            qualifiers=qualifiers,
         )
 
 
 def _norm(s: Optional[str]) -> str:
     if not s:
         return ""
     return s.lower().replace(" ", "").replace("-", "")
@@ -243,8 +248,9 @@
     for key in keys:
         if key in data:
             return data[key]
     return None
 
 
 if __name__ == "__main__":
-    lines_to_new_tab(iter_pypi_lines("y0"))
+    # print(render_lines(iter_pypi_lines("quickstatements-client"), sep="\t", newline="\n"))
+    lines_to_new_tab(iter_pypi_lines("bioregistry"))
```

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client/sources/utils.py` & `quickstatements_client-0.0.3/src/quickstatements_client/sources/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 """Utilities for Wikidata."""
 
 from typing import Any, List, Mapping
 
 import requests
 
+from ..version import get_version
+
 __all__ = [
     "WIKIDATA_ENDPOINT",
     "query_wikidata",
     "removeprefix",
 ]
 
 #: Wikidata SPARQL endpoint. See https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service#Interfacing
@@ -18,15 +20,23 @@
 
 def query_wikidata(sparql: str) -> List[Mapping[str, Any]]:
     """Query Wikidata's sparql service.
 
     :param sparql: A SPARQL query string
     :return: A list of bindings
     """
-    res = requests.get(WIKIDATA_ENDPOINT, params={"query": sparql, "format": "json"})
+    headers = {
+        "User-Agent": f"quickstatements_client v{get_version()}",
+    }
+    res = requests.get(
+        WIKIDATA_ENDPOINT,
+        params={"query": sparql, "format": "json"},
+        headers=headers,
+        timeout=300,
+    )
     res.raise_for_status()
     res_json = res.json()
     return [
         {key: _clean_value(value["value"]) for key, value in record.items()}
         for record in res_json["results"]["bindings"]
     ]
```

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client/version.py` & `quickstatements_client-0.0.3/src/quickstatements_client/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`quickstatements_client` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client.egg-info/PKG-INFO` & `quickstatements_client-0.0.3/src/quickstatements_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstatements-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: A data model and client for Wikidata QuickStatements
 Home-page: https://github.com/cthoyt/quickstatements-client
 Download-URL: https://github.com/cthoyt/quickstatements-client/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quickstatements-client Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: quickstatements-client Version: 0.0.3 Summary: A
 data model and client for Wikidata QuickStatements Home-page: https://
 github.com/cthoyt/quickstatements-client Download-URL: https://github.com/
 cthoyt/quickstatements-client/releases Author: Charles Tapley Hoyt Author-
 email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-email:
 cthoyt@gmail.com License: MIT Project-URL: Bug Tracker, https://github.com/
 cthoyt/quickstatements-client/issues Project-URL: Source Code, https://
 github.com/cthoyt/quickstatements-client Keywords:
```

### Comparing `quickstatements_client-0.0.2/src/quickstatements_client.egg-info/SOURCES.txt` & `quickstatements_client-0.0.3/src/quickstatements_client.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 src/quickstatements_client.egg-info/PKG-INFO
 src/quickstatements_client.egg-info/SOURCES.txt
 src/quickstatements_client.egg-info/dependency_links.txt
 src/quickstatements_client.egg-info/entry_points.txt
 src/quickstatements_client.egg-info/not-zip-safe
 src/quickstatements_client.egg-info/requires.txt
 src/quickstatements_client.egg-info/top_level.txt
+src/quickstatements_client/language_codes/__init__.py
+src/quickstatements_client/language_codes/data.json
+src/quickstatements_client/maintenance/__init__.py
+src/quickstatements_client/maintenance/annotate_missing_followed_by.py
+src/quickstatements_client/maintenance/annotate_missing_follows.py
 src/quickstatements_client/sources/__init__.py
 src/quickstatements_client/sources/licenses.json
 src/quickstatements_client/sources/pypi.py
 src/quickstatements_client/sources/utils.py
 tests/__init__.py
 tests/sample_orcid.json
 tests/test_models.py
```

### Comparing `quickstatements_client-0.0.2/tests/sample_orcid.json` & `quickstatements_client-0.0.3/tests/sample_orcid.json`

 * *Files identical despite different names*

### Comparing `quickstatements_client-0.0.2/tests/test_models.py` & `quickstatements_client-0.0.3/tests/test_models.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 import datetime
 import json
 import unittest
 from pathlib import Path
 from typing import Tuple, Union
 
+import pydantic.error_wrappers
+
 from quickstatements_client.model import (
+    BaseLine,
     DateQualifier,
     EntityLine,
     EntityQualifier,
     TextLine,
     TextQualifier,
     prepare_date,
 )
@@ -18,14 +21,41 @@
 HERE = Path(__file__).parent.resolve()
 SAMPLE_ORCID_PATH = HERE.joinpath("sample_orcid.json")
 
 
 class TestQuickStatements(unittest.TestCase):
     """Tests for quickstatements."""
 
+    def test_base_line(self):
+        """Test instantiating the base line object."""
+        for subject, predicate in [
+            ("LAST", "Len"),
+            ("LAST", "Den"),
+            ("Q1234", "Len"),
+            ("Q1234", "Den"),
+            ("LAST", "P1234"),
+            ("Q1234", "P1234"),
+        ]:
+            with self.subTest(subject=subject, prediate=predicate):
+                BaseLine(subject=subject, predicate=predicate)
+
+        for subject, predicate, text in [
+            ("Q1", "Afr", "Le monde"),  # french
+            ("Q1", "DNL.", "XXX"),  # no language description
+            ("Q1", "Lde", "XXX"),
+        ]:
+            with self.subTest(subject=subject, prediate=predicate, text=text):
+                TextLine(subject=subject, predicate=predicate, target=text)
+
+        for subject, predicate, text in [("Q1", "Lxyz", "XXX")]:
+            with self.subTest(subject=subject, prediate=predicate, text=text), self.assertRaises(
+                pydantic.error_wrappers.ValidationError
+            ):
+                TextLine(subject=subject, predicate=predicate, target=text)
+
     def test_prepare_date(self):
         """Test the date cleaning function."""
         sample_orcid_data = json.loads(SAMPLE_ORCID_PATH.read_text())
         education_data = sample_orcid_data["activities-summary"]["educations"]["education-summary"]
 
         test_start_date, start_date_precision = _get_date(education_data[1])
         test_end_date, end_date_precision = _get_date(education_data[1], start_or_end="end")
```

