# Comparing `tmp/tendril-artefacts-0.1.6.tar.gz` & `tmp/tendril-artefacts-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-artefacts-0.1.6.tar", last modified: Wed Apr 19 09:33:22 2023, max compression
+gzip compressed data, was "tendril-artefacts-0.1.7.tar", last modified: Fri Jun 30 17:13:17 2023, max compression
```

## Comparing `tendril-artefacts-0.1.6.tar` & `tendril-artefacts-0.1.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.993175 tendril-artefacts-0.1.6/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3540 2023-04-19 09:33:22.993175 tendril-artefacts-0.1.6/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.985175 tendril-artefacts-0.1.6/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-19 09:33:22.993175 tendril-artefacts-0.1.6/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3170 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.985175 tendril-artefacts-0.1.6/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/artefacts/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       39 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/base.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/artefacts/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1049 2022-12-11 07:25:27.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1722 2023-04-19 09:30:08.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/db/model.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.6/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.6/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      205 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.6/src/tendril/authz/roles/artefacts.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3540 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      932 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      513 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.993175 tendril-artefacts-0.1.6/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.647240 tendril-artefacts-0.1.7/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3540 2023-06-30 17:13:17.647240 tendril-artefacts-0.1.7/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.635240 tendril-artefacts-0.1.7/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.639240 tendril-artefacts-0.1.7/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.639240 tendril-artefacts-0.1.7/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.639240 tendril-artefacts-0.1.7/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.639240 tendril-artefacts-0.1.7/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-06-30 17:13:17.647240 tendril-artefacts-0.1.7/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3170 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.635240 tendril-artefacts-0.1.7/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/artefacts/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       39 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/base.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/artefacts/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1049 2022-12-11 07:25:27.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1810 2023-06-30 15:45:59.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/db/model.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.7/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.7/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      205 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.7/src/tendril/authz/roles/artefacts.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3540 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      932 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      513 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/tox.ini
```

### Comparing `tendril-artefacts-0.1.6/.gitignore` & `tendril-artefacts-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/.readthedocs.yml` & `tendril-artefacts-0.1.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/.travis.yml` & `tendril-artefacts-0.1.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/LICENSE` & `tendril-artefacts-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/PKG-INFO` & `tendril-artefacts-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-artefacts
-Version: 0.1.6
+Version: 0.1.7
 Summary: Core Artefact Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-artefacts
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-artefacts.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-artefacts/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-artefacts
```

### Comparing `tendril-artefacts-0.1.6/README.rst` & `tendril-artefacts-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/docs/Makefile` & `tendril-artefacts-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/docs/_static/custom.css` & `tendril-artefacts-0.1.7/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/docs/_static/favicon.ico` & `tendril-artefacts-0.1.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/docs/_static/logo.png` & `tendril-artefacts-0.1.7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/docs/_static/logo_packed.png` & `tendril-artefacts-0.1.7/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/docs/_templates/about.html` & `tendril-artefacts-0.1.7/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/docs/conf.py` & `tendril-artefacts-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/docs/index.rst` & `tendril-artefacts-0.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/docs/installation.rst` & `tendril-artefacts-0.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/setup.py` & `tendril-artefacts-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/src/tendril/artefacts/db/controller.py` & `tendril-artefacts-0.1.7/src/tendril/artefacts/db/controller.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/src/tendril/artefacts/db/model.py` & `tendril-artefacts-0.1.7/src/tendril/artefacts/db/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 from sqlalchemy import Boolean
 from sqlalchemy_json import mutable_json_type
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy import ForeignKey
 from sqlalchemy.orm import relationship
 from sqlalchemy.ext.declarative import declared_attr
 
-
+from tendril.db.mixins.interests import InterestMixin
 from tendril.utils.db import DeclBase
 from tendril.utils.db import BaseMixin
 from tendril.utils.db import TimestampMixin
 from tendril.authn.db.mixins import UserMixin
 
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
-class ArtefactModel(DeclBase, BaseMixin, TimestampMixin, UserMixin):
+class ArtefactModel(DeclBase, BaseMixin, TimestampMixin,
+                    UserMixin, InterestMixin):
     _type_name = "artefact"
     type = Column(String(50), nullable=False, default=_type_name)
     title = Column(String(255), nullable=True)
     label = Column(String(50), nullable=True)
     active = Column(Boolean, nullable=False, default=True)
 
     # @declared_attr
```

### Comparing `tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/PKG-INFO` & `tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-artefacts
-Version: 0.1.6
+Version: 0.1.7
 Summary: Core Artefact Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-artefacts
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-artefacts.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-artefacts/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-artefacts
```

### Comparing `tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/SOURCES.txt` & `tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/requires.txt` & `tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/tests/coveralls.py` & `tendril-artefacts-0.1.7/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.6/tox.ini` & `tendril-artefacts-0.1.7/tox.ini`

 * *Files identical despite different names*

