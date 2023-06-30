# Comparing `tmp/zpretty-3.1.0a1.tar.gz` & `tmp/zpretty-3.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpretty-3.1.0a1.tar", last modified: Thu May  4 07:33:37 2023, max compression
+gzip compressed data, was "zpretty-3.1.0a2.tar", last modified: Tue May  9 16:07:40 2023, max compression
```

## Comparing `zpretty-3.1.0a1.tar` & `zpretty-3.1.0a2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/
--rw-rw-r--   0 ale       (1000) ale       (1000)      565 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/.pre-commit-config.yaml
--rw-rw-r--   0 ale       (1000) ale       (1000)      176 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/.pre-commit-hooks.yaml
--rw-rw-r--   0 ale       (1000) ale       (1000)     4014 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/HISTORY.md
--rw-rw-r--   0 ale       (1000) ale       (1000)     1387 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/LICENSE
--rw-rw-r--   0 ale       (1000) ale       (1000)      238 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/MANIFEST.in
--rw-rw-r--   0 ale       (1000) ale       (1000)      808 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/Makefile
--rw-rw-r--   0 ale       (1000) ale       (1000)    10506 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     5582 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/README.md
--rw-rw-r--   0 ale       (1000) ale       (1000)      325 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/pyproject.toml
--rw-rw-r--   0 ale       (1000) ale       (1000)      106 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/requirements-dev.txt
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/requirements.d/
--rw-rw-r--   0 ale       (1000) ale       (1000)      865 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/requirements.d/requirements-dev-37.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1036 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/requirements.d/requirements-dev.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      289 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1565 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/setup.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      863 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/tox.ini
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7728 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/attributes.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     8249 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/cli.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    13179 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/elements.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     5242 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/prettifier.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/broken/
--rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/broken/broken.xml
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/include-exclude/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.html
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.html
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.zcml
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.html
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.html
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.zcml
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.html
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.html
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)      175 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/mock.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/zpretty/tests/original/
--rw-rw-r--   0 ale       (1000) ale       (1000)       47 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1587 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)      272 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_dtml.dtml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1890 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_html.html
--rw-rw-r--   0 ale       (1000) ale       (1000)     1938 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_html4.html
--rw-rw-r--   0 ale       (1000) ale       (1000)      366 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_html_with_preprocessing_instruction.html
--rw-rw-r--   0 ale       (1000) ale       (1000)     1504 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_pt.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)      667 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_xml.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      126 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/text_with_markup.md
--rw-rw-r--   0 ale       (1000) ale       (1000)     2728 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_attributes.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7639 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_cli.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4423 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_elements.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      952 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_functions.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1908 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_readme.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1399 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_xml.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7715 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_zcml.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7763 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_zpretty.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      943 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/text.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2580 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/xml.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    24594 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/zcml.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty.egg-info/
--rw-rw-r--   0 ale       (1000) ale       (1000)    10506 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     2626 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       44 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/entry_points.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/not-zip-safe
--rw-rw-r--   0 ale       (1000) ale       (1000)      119 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        8 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      565 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/.pre-commit-config.yaml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      176 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/.pre-commit-hooks.yaml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4123 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/HISTORY.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1387 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/LICENSE
+-rw-rw-r--   0 ale       (1000) ale       (1000)      238 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/MANIFEST.in
+-rw-rw-r--   0 ale       (1000) ale       (1000)      978 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/Makefile
+-rw-rw-r--   0 ale       (1000) ale       (1000)    10615 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5582 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/README.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)      325 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      106 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/requirements-dev.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/requirements.d/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      865 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/requirements.d/requirements-dev-37.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1036 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/requirements.d/requirements-dev.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      289 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1565 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/setup.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      863 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/tox.ini
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/zpretty/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7728 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/attributes.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8249 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/cli.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13179 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/elements.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5367 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/prettifier.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/zpretty/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/zpretty/tests/broken/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/broken/broken.xml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.763738 zpretty-3.1.0a2/zpretty/tests/include-exclude/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/bar.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/bar.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/bar.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/bar.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/bar.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/foo.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/foo.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/foo.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/foo.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/.venv/foo.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.763738 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/bar.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/bar.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/bar.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/bar.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/bar.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/foo.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/foo.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/foo.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/foo.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/foo/bar/foo.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/bar.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/bar.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/bar.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/bar.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/bar.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/foo.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/foo.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/foo.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/foo.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/include-exclude/venv/foo.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      175 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/mock.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/zpretty/tests/original/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       47 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/original/sample.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1587 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/original/sample.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      272 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/original/sample_dtml.dtml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1890 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/original/sample_html.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1938 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/original/sample_html4.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)      366 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/original/sample_html_with_preprocessing_instruction.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1504 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/original/sample_pt.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      667 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/original/sample_xml.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      126 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/original/text_with_markup.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2728 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/test_attributes.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7639 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/test_cli.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4423 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/test_elements.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      952 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/test_functions.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1908 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/test_readme.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1399 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/test_xml.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7715 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/test_zcml.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7970 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/tests/test_zpretty.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      943 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/text.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2580 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/xml.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    24594 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty/zcml.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-09 16:07:40.767738 zpretty-3.1.0a2/zpretty.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    10615 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2626 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       44 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty.egg-info/entry_points.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)      119 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        8 2023-05-09 16:07:40.000000 zpretty-3.1.0a2/zpretty.egg-info/top_level.txt
```

### Comparing `zpretty-3.1.0a1/.pre-commit-config.yaml` & `zpretty-3.1.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/HISTORY.md` & `zpretty-3.1.0a2/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
+## 3.1.0a2 (2023-05-09)
+
+- Improve the regular expression that matches the entities
+  (Fixes #130)
+  [ale-rt]
+
 ## 3.1.0a1 (2023-05-04)
 
 - Add command line parameters to include/exclude files and folders
   (Implements #96)
-  [ale-rt]  
+  [ale-rt]
 - Be tolerant with characters forbidden in XML when dealing with tal attributes
   (See #125)
   [ale-rt]
 
 ## 3.0.4 (2023-04-20)
 
 - Fix bogus ampersands in attributes
```

### Comparing `zpretty-3.1.0a1/LICENSE` & `zpretty-3.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/Makefile` & `zpretty-3.1.0a2/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 .PHONY: all
-all: py3/bin/pip
+all: install
 
 .PHONY: test
 test: pre-commit pytest
 
+.venv/bin/pip:
+	python3 -m venv .venv
+
+.PHONY: install
+install: .venv/bin/pip
+	./.venv/bin/pip install -IU pip
+	./.venv/bin/pip install -IU .[development,test]
+	./.venv/bin/pip install -e .
+
 requirements := $(wildcard requirements-dev.txt requirements.d/*.txt)
-py3/bin/pip: $(requirements)
-	python3 -m venv py3
-	./py3/bin/pip install -IU pip
-	./py3/bin/pip install -IU .[development,test]
 
+.venv/bin/pre-commit: $(requirements)
+	make install
 
-./py3/bin/pre-commit: py3/bin/pip
+.venv/bin/pytest: $(requirements)
+	make install
 
 .PHONY: pre-commit
-pre-commit:
-	./py3/bin/pre-commit install
-	./py3/bin/pre-commit run --all
+pre-commit: .venv/bin/pre-commit
+	./.venv/bin/pre-commit install
+	./.venv/bin/pre-commit run --all
 
 .PHONY: pytests
-pytest: py3/bin/pip
-	./py3/bin/pytest
+pytest: .venv/bin/pytest
+	./.venv/bin/pytest
 
 .PHONY: htmlreport
-htmlreport: py3/bin/pip
-	./py3/bin/pytest --cov-report html
+htmlreport: .venv/bin/pytest
+	./.venv/bin/pytest --cov-report html
 
 .PHONY: requirements
-requirements: py3/bin/pip
-	./py3/bin/pip install -Ue .[development,test]
-	./py3/bin/pip freeze --all|egrep -v '^(pip|pkg-resources|wheel|-e|-f)' > requirements.d/requirements-dev.txt
+requirements: .venv/bin/pip
+	./.venv/bin/pip install -Ue .[development,test]
+	./.venv/bin/pip freeze --all|egrep -v '^(pip|pkg-resources|wheel|-e|-f)' > requirements.d/requirements-dev.txt
 	@git difftool -y -x "colordiff -y" requirements.d/requirements-dev.txt
```

### Comparing `zpretty-3.1.0a1/PKG-INFO` & `zpretty-3.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpretty
-Version: 3.1.0a1
+Version: 3.1.0a2
 Summary: An opinionated HTML/XML soup formatter
 Home-page: https://github.com/collective/zpretty
 Author: Alessandro Pisa
 Author-email: alessandro.pisa@gmail.com
 License: BSD
 Keywords: Formatter,HTML,Prettifier,Pretty print,TAL,XML,ZPT
 Classifier: Development Status :: 5 - Production/Stable
@@ -174,19 +174,25 @@
 
 ```bash
 make test
 ```
 
 # Changelog
 
+## 3.1.0a2 (2023-05-09)
+
+- Improve the regular expression that matches the entities
+  (Fixes #130)
+  [ale-rt]
+
 ## 3.1.0a1 (2023-05-04)
 
 - Add command line parameters to include/exclude files and folders
   (Implements #96)
-  [ale-rt]  
+  [ale-rt]
 - Be tolerant with characters forbidden in XML when dealing with tal attributes
   (See #125)
   [ale-rt]
 
 ## 3.0.4 (2023-04-20)
 
 - Fix bogus ampersands in attributes
```

### Comparing `zpretty-3.1.0a1/README.md` & `zpretty-3.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/requirements.d/requirements-dev-37.txt` & `zpretty-3.1.0a2/requirements.d/requirements-dev-37.txt`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/requirements.d/requirements-dev.txt` & `zpretty-3.1.0a2/requirements.d/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/setup.py` & `zpretty-3.1.0a2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 setup(
     name="zpretty",
-    version="3.1.0a1",
+    version="3.1.0a2",
     description="An opinionated HTML/XML soup formatter",
     keywords=["Formatter", "HTML", "Prettifier", "Pretty print", "TAL", "XML", "ZPT"],
     long_description="\n".join((read("README.md"), read("HISTORY.md"))),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
```

### Comparing `zpretty-3.1.0a1/tox.ini` & `zpretty-3.1.0a2/tox.ini`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/attributes.py` & `zpretty-3.1.0a2/zpretty/attributes.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/cli.py` & `zpretty-3.1.0a2/zpretty/cli.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/elements.py` & `zpretty-3.1.0a2/zpretty/elements.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/prettifier.py` & `zpretty-3.1.0a2/zpretty/prettifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,20 +77,24 @@
             pass
         text = re.sub(self._cdata_pattern, self._cdata_marker, text)
         text = re.sub(self._doctype_pattern, self._doctype_marker, text)
 
         # Get all the entities in the text and replace them with a marker
         # The text might contain undefined entities that BeautifulSoup
         # will strip out.
-        entities = set(re.findall(r"&[^;]+;", text))
-        for entitiy in entities:
+        entities = {
+            _[0]
+            for _ in re.findall(
+                r"(&([a-z0-9]+|#[0-9]{1,6}|#x[0-9a-fA-F]{1,6});)", text, re.IGNORECASE
+            )
+        }
+        for entity in entities:
             marker = str(uuid4())
-            self._entity_mapping[entitiy] = marker
-            text = text.replace(entitiy, marker)
-
+            self._entity_mapping[entity] = marker
+            text = text.replace(entity, marker)
         return "\n".join(
             line if line.strip() else self._newlines_marker
             for line in text.splitlines()
         ).replace("&", self._ampersand_marker)
 
     def get_soup(self, text):
         """Tries to get the soup from the given test
```

### Comparing `zpretty-3.1.0a1/zpretty/tests/original/sample.zcml` & `zpretty-3.1.0a2/zpretty/tests/original/sample.zcml`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/original/sample_html.html` & `zpretty-3.1.0a2/zpretty/tests/original/sample_html.html`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/original/sample_html4.html` & `zpretty-3.1.0a2/zpretty/tests/original/sample_html4.html`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/original/sample_pt.pt` & `zpretty-3.1.0a2/zpretty/tests/original/sample_pt.pt`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/original/sample_xml.xml` & `zpretty-3.1.0a2/zpretty/tests/original/sample_xml.xml`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/test_attributes.py` & `zpretty-3.1.0a2/zpretty/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/test_cli.py` & `zpretty-3.1.0a2/zpretty/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/test_elements.py` & `zpretty-3.1.0a2/zpretty/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/test_functions.py` & `zpretty-3.1.0a2/zpretty/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/test_readme.py` & `zpretty-3.1.0a2/zpretty/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/test_xml.py` & `zpretty-3.1.0a2/zpretty/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/test_zcml.py` & `zpretty-3.1.0a2/zpretty/tests/test_zcml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/tests/test_zpretty.py` & `zpretty-3.1.0a2/zpretty/tests/test_zpretty.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,20 @@
     def test_escaped_ampersand_in_attrs(self):
         self.assertPrettified('<root a="&amp;" />', '<root a="&amp;"></root>\n')
         self.assertPrettified('<root a="foo &amp;" />', '<root a="foo &amp;"></root>\n')
         self.assertPrettified('<root a="&amp; bar" />', '<root a="&amp; bar"></root>\n')
         self.assertPrettified('<root a=";&amp;" />', '<root a=";&amp;"></root>\n')
         self.assertPrettified('<root a="&amp;;" />', '<root a="&amp;;"></root>\n')
 
+    def test_ampersand_and_column_in_separate_attrs(self):
+        self.assertPrettified(
+            '<foo a="&" />\n<tal:bar b=";" />',
+            '<foo a="&amp;"></foo>\n<tal:bar b=";" />\n',
+        )
+
     def test_sample_html(self):
         self.prettify("sample_html.html")
 
     def test_sample_html4(self):
         self.prettify("sample_html4.html")
 
     def test_sample_html_with_preprocessing_instruction(self):
```

### Comparing `zpretty-3.1.0a1/zpretty/text.py` & `zpretty-3.1.0a2/zpretty/text.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/xml.py` & `zpretty-3.1.0a2/zpretty/xml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty/zcml.py` & `zpretty-3.1.0a2/zpretty/zcml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.1.0a1/zpretty.egg-info/PKG-INFO` & `zpretty-3.1.0a2/zpretty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpretty
-Version: 3.1.0a1
+Version: 3.1.0a2
 Summary: An opinionated HTML/XML soup formatter
 Home-page: https://github.com/collective/zpretty
 Author: Alessandro Pisa
 Author-email: alessandro.pisa@gmail.com
 License: BSD
 Keywords: Formatter,HTML,Prettifier,Pretty print,TAL,XML,ZPT
 Classifier: Development Status :: 5 - Production/Stable
@@ -174,19 +174,25 @@
 
 ```bash
 make test
 ```
 
 # Changelog
 
+## 3.1.0a2 (2023-05-09)
+
+- Improve the regular expression that matches the entities
+  (Fixes #130)
+  [ale-rt]
+
 ## 3.1.0a1 (2023-05-04)
 
 - Add command line parameters to include/exclude files and folders
   (Implements #96)
-  [ale-rt]  
+  [ale-rt]
 - Be tolerant with characters forbidden in XML when dealing with tal attributes
   (See #125)
   [ale-rt]
 
 ## 3.0.4 (2023-04-20)
 
 - Fix bogus ampersands in attributes
```

### Comparing `zpretty-3.1.0a1/zpretty.egg-info/SOURCES.txt` & `zpretty-3.1.0a2/zpretty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

