# Comparing `tmp/bronzivka-0.0.2.tar.gz` & `tmp/bronzivka-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bronzivka-0.0.2.tar", max compression
+gzip compressed data, was "bronzivka-0.0.3.tar", max compression
```

## Comparing `bronzivka-0.0.2.tar` & `bronzivka-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1287 2023-06-30 19:08:01.315142 bronzivka-0.0.2/bronzivka/__init__.py
--rw-r--r--   0        0        0     2127 2023-06-30 19:08:01.315142 bronzivka-0.0.2/bronzivka/theme/bronzivka.css
--rw-r--r--   0        0        0      541 2023-06-30 19:08:01.315142 bronzivka-0.0.2/bronzivka/theme/class.rst
--rw-r--r--   0        0        0     1432 2023-06-30 19:08:01.315142 bronzivka-0.0.2/bronzivka/theme/navbar-logo.html
--rw-r--r--   0        0        0      102 2023-06-30 19:08:01.315142 bronzivka-0.0.2/bronzivka/theme/theme.conf
--rw-r--r--   0        0        0      660 2023-06-30 19:08:01.319141 bronzivka-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       72 2023-06-30 19:08:01.319141 bronzivka-0.0.2/readme.md
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 bronzivka-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1287 2023-06-30 19:33:27.113448 bronzivka-0.0.3/bronzivka/__init__.py
+-rw-r--r--   0        0        0     2127 2023-06-30 19:33:27.113448 bronzivka-0.0.3/bronzivka/theme/bronzivka.css
+-rw-r--r--   0        0        0      541 2023-06-30 19:33:27.113448 bronzivka-0.0.3/bronzivka/theme/class.rst
+-rw-r--r--   0        0        0     1432 2023-06-30 19:33:27.113448 bronzivka-0.0.3/bronzivka/theme/navbar-logo.html
+-rw-r--r--   0        0        0      102 2023-06-30 19:33:27.113448 bronzivka-0.0.3/bronzivka/theme/theme.conf
+-rw-r--r--   0        0        0      658 2023-06-30 19:33:27.113448 bronzivka-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-06-30 19:33:27.113448 bronzivka-0.0.3/readme.md
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 bronzivka-0.0.3/PKG-INFO
```

### Comparing `bronzivka-0.0.2/bronzivka/__init__.py` & `bronzivka-0.0.3/bronzivka/__init__.py`

 * *Files identical despite different names*

### Comparing `bronzivka-0.0.2/bronzivka/theme/bronzivka.css` & `bronzivka-0.0.3/bronzivka/theme/bronzivka.css`

 * *Files identical despite different names*

### Comparing `bronzivka-0.0.2/bronzivka/theme/class.rst` & `bronzivka-0.0.3/bronzivka/theme/class.rst`

 * *Files identical despite different names*

### Comparing `bronzivka-0.0.2/bronzivka/theme/navbar-logo.html` & `bronzivka-0.0.3/bronzivka/theme/navbar-logo.html`

 * *Files identical despite different names*

### Comparing `bronzivka-0.0.2/pyproject.toml` & `bronzivka-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bronzivka"
-version = "0.0.2"
+version = "0.0.3"
 description = "My Python packages sphinx documentation theme"
 authors = ["Lionel Garcia"]
 license = "MIT"
 readme = "readme.md"
 include = ["bronzivka/theme", "bronzivka/theme/**/*"]
 repository = "https://github.com/lgrcia/bronzivka"
 
@@ -18,12 +18,12 @@
 myst-nb = "*"
 sphinx-copybutton = "*"
 sphinx-design = "*"
 toml = "*"
 ipywidgets = "*"
 
 [tool.poetry.plugins."sphinx.html_themes"]
-pobronzivka = "bronzivka"
+bronzivka = "bronzivka"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bronzivka-0.0.2/PKG-INFO` & `bronzivka-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bronzivka
-Version: 0.0.2
+Version: 0.0.3
 Summary: My Python packages sphinx documentation theme
 Home-page: https://github.com/lgrcia/bronzivka
 License: MIT
 Author: Lionel Garcia
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

