# Comparing `tmp/uedition-0.4.0.tar.gz` & `tmp/uedition-0.5.0.tar.gz`

## Comparing `uedition-0.4.0.tar` & `uedition-0.5.0.tar`

### file list

```diff
@@ -1,67 +1,70 @@
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 uedition-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.4.0/tox.ini
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/workflows/codestyle.yml
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/test_about.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/test_build.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/test_check.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/test_settings.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/basic/uEdition.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/empty/.gitkeep
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/invalid_core_files/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/invalid_core_files/en/_config.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/invalid_core_files/en/_toc.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_core_files/uEdition.yaml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/references.bib
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/en/_config.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/en/_toc.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/en/intro.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root/en/_config.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root/en/_toc.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root_file/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root_file/en/_config.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root_file/en/_toc.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/references.bib
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/_config.yml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/_toc.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/a-1-page.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/a-2-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/a-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/b-page.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/intro.md
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/_config.yml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/_toc.yml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/a-1-page.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/a-2-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/a-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/b-page.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/intro.md
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/yaml/uEdition.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/__about__.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/__main__.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/settings.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/cli/__init__.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/cli/build.py
--rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/cli/check.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/cli/serve.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/__init__.py
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/config.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/language_switcher.js
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/language_switcher.py
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/tei.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.4.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.4.0/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uedition-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 uedition-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 uedition-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.5.0/tox.ini
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 uedition-0.5.0/.github/workflows/codestyle.yml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.5.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.5.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/test_about.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/test_build.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/test_check.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/test_settings.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/basic/uEdition.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/empty/.gitkeep
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/invalid_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/invalid_core_files/en/_config.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/invalid_core_files/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_files/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_files/references.bib
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_files/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_files/en/_config.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_files/en/_toc.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_files/en/intro.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_toc_root/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_toc_root/en/_config.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_toc_root/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_toc_root_file/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_toc_root_file/en/_config.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/missing_toc_root_file/en/_toc.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/references.bib
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/de/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/de/_toc.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/de/a-1-page.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/de/a-2-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/de/a-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/de/b-page.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/de/intro.md
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/en/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/en/_toc.yml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/en/a-1-page.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/en/a-2-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/en/a-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/en/b-page.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/multilang/en/intro.md
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.5.0/tests/fixtures/yaml/uEdition.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/__about__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/__main__.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/settings.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/cli/__init__.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/cli/build.py
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/cli/check.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/cli/create.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/cli/language.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/cli/serve.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/cli/update.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/ext/__init__.py
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/ext/config.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/ext/language_switcher.js
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/ext/language_switcher.py
+-rw-r--r--   0        0        0    11380 2020-02-02 00:00:00.000000 uedition-0.5.0/uedition/ext/tei.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.5.0/README.md
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 uedition-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 uedition-0.5.0/PKG-INFO
```

### Comparing `uedition-0.4.0/.github/workflows/coverage.yml` & `uedition-0.5.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/.github/workflows/release.yml` & `uedition-0.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/.github/workflows/tests.yml` & `uedition-0.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/tests/conftest.py` & `uedition-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/tests/test_build.py` & `uedition-0.5.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/tests/test_check.py` & `uedition-0.5.0/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/tests/test_settings.py` & `uedition-0.5.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/tests/fixtures/missing_files/references.bib` & `uedition-0.5.0/tests/fixtures/missing_files/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/tests/fixtures/missing_files/en/_config.yml` & `uedition-0.5.0/tests/fixtures/missing_files/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/tests/fixtures/multilang/references.bib` & `uedition-0.5.0/tests/fixtures/multilang/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/tests/fixtures/multilang/de/_config.yml` & `uedition-0.5.0/tests/fixtures/multilang/de/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/tests/fixtures/multilang/en/_config.yml` & `uedition-0.5.0/tests/fixtures/multilang/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/uedition/settings.py` & `uedition-0.5.0/uedition/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2023-present Mark Hall <mark.hall@work.room3b.eu>
+#
+# SPDX-License-Identifier: MIT
 """Application settings.
 
 All application settings are accessed via the `settings` dictionary.
 """
 import os
 
 from pydantic import BaseSettings, BaseModel
```

### Comparing `uedition-0.4.0/uedition/cli/__init__.py` & `uedition-0.5.0/uedition/cli/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,20 +2,35 @@
 #
 # SPDX-License-Identifier: MIT
 """uEdtion Command-line Tool."""
 import typer
 
 from rich import print as print_cli
 
-from . import check as check_module, build as build_module, serve as serve_module
+from . import (
+    check as check_module,
+    build as build_module,
+    serve as serve_module,
+    create as create_module,
+    update as update_module,
+    language as language_module,
+)
 from ..__about__ import __version__
 from ..settings import settings
 
 
 app = typer.Typer()
+language_app = typer.Typer()
+app.add_typer(language_app, name="language")
+
+
+@app.command()
+def create(path: str) -> None:
+    """Create a new μEdition."""
+    create_module.run(path)
 
 
 @app.command()
 def build() -> None:
     """Build the μEdition."""
     build_module.run()
 
@@ -29,11 +44,29 @@
 @app.command()
 def check() -> None:
     """Check that the μEdition is set up correctly."""
     check_module.run()
 
 
 @app.command()
+def update() -> None:
+    """Update the μEdition."""
+    update_module.run()
+
+
+@app.command()
 def version() -> None:
     """Output the current μEdition version."""
     print_cli(f"μEdition: {__version__}")
     print_cli(f'Configuration: {settings["version"]}')
+
+
+@language_app.command()
+def language_add(path: str) -> None:
+    """Add a language to the μEdition."""
+    language_module.add(path)
+
+
+@language_app.command()
+def language_update(path: str) -> None:
+    """Update a language."""
+    language_module.update(path)
```

### Comparing `uedition-0.4.0/uedition/cli/build.py` & `uedition-0.5.0/uedition/cli/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,188 +1,195 @@
-00000000: 2222 2242 7569 6c64 2066 756e 6374 696f  """Build functio
-00000010: 6e61 6c69 7479 2e22 2222 0a69 6d70 6f72  nality.""".impor
-00000020: 7420 6a73 6f6e 0a69 6d70 6f72 7420 7375  t json.import su
-00000030: 6270 726f 6365 7373 0a0a 6672 6f6d 206f  bprocess..from o
-00000040: 7320 696d 706f 7274 2070 6174 682c 206d  s import path, m
-00000050: 616b 6564 6972 730a 6672 6f6d 2073 6875  akedirs.from shu
-00000060: 7469 6c20 696d 706f 7274 2072 6d74 7265  til import rmtre
-00000070: 652c 2063 6f70 7974 7265 650a 0a66 726f  e, copytree..fro
-00000080: 6d20 2e2e 7365 7474 696e 6773 2069 6d70  m ..settings imp
-00000090: 6f72 7420 7365 7474 696e 6773 0a0a 0a64  ort settings...d
-000000a0: 6566 206c 616e 6469 6e67 5f62 7569 6c64  ef landing_build
-000000b0: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-000000c0: 2222 2242 7569 6c64 2074 6865 206c 616e  """Build the lan
-000000d0: 6469 6e67 2070 6167 652e 2222 220a 2020  ding page.""".  
-000000e0: 2020 6966 206e 6f74 2070 6174 682e 6578    if not path.ex
-000000f0: 6973 7473 2873 6574 7469 6e67 735b 226f  ists(settings["o
-00000100: 7574 7075 7422 5d29 3a0a 2020 2020 2020  utput"]):.      
-00000110: 2020 6d61 6b65 6469 7273 2873 6574 7469    makedirs(setti
-00000120: 6e67 735b 226f 7574 7075 7422 5d2c 2065  ngs["output"], e
-00000130: 7869 7374 5f6f 6b3d 5472 7565 290a 2020  xist_ok=True).  
-00000140: 2020 7769 7468 206f 7065 6e28 7061 7468    with open(path
-00000150: 2e6a 6f69 6e28 7365 7474 696e 6773 5b22  .join(settings["
-00000160: 6f75 7470 7574 225d 2c20 2263 6f6e 6669  output"], "confi
-00000170: 672e 6a73 6f6e 2229 2c20 2277 2229 2061  g.json"), "w") a
-00000180: 7320 6f75 745f 663a 0a20 2020 2020 2020  s out_f:.       
-00000190: 206a 736f 6e2e 6475 6d70 2873 6574 7469   json.dump(setti
-000001a0: 6e67 732c 206f 7574 5f66 290a 2020 2020  ngs, out_f).    
-000001b0: 7769 7468 206f 7065 6e28 7061 7468 2e6a  with open(path.j
-000001c0: 6f69 6e28 7365 7474 696e 6773 5b22 6f75  oin(settings["ou
-000001d0: 7470 7574 225d 2c20 2269 6e64 6578 2e68  tput"], "index.h
-000001e0: 746d 6c22 292c 2022 7722 2920 6173 206f  tml"), "w") as o
-000001f0: 7574 5f66 3a0a 2020 2020 2020 2020 6f75  ut_f:.        ou
-00000200: 745f 662e 7772 6974 6528 0a20 2020 2020  t_f.write(.     
-00000210: 2020 2020 2020 2022 2222 5c0a 3c21 444f         """\.<!DO
-00000220: 4354 5950 4520 6874 6d6c 3e0a 3c68 746d  CTYPE html>.<htm
-00000230: 6c3e 0a20 203c 6865 6164 3e0a 2020 2020  l>.  <head>.    
-00000240: 3c6d 6574 6120 6e61 6d65 3d22 6368 6172  <meta name="char
-00000250: 7365 7422 2076 616c 7565 3d22 7574 662d  set" value="utf-
-00000260: 3822 3e0a 2020 2020 3c74 6974 6c65 3e52  8">.    <title>R
-00000270: 6564 6972 6563 7469 6e67 2e2e 2e20 506c  edirecting... Pl
-00000280: 6561 7365 2077 6169 742e 2e2e 3c2f 7469  ease wait...</ti
-00000290: 746c 653e 0a20 203c 2f68 6561 643e 0a20  tle>.  </head>. 
-000002a0: 203c 626f 6479 3e0a 2020 2020 3c68 313e   <body>.    <h1>
-000002b0: 596f 7520 6172 6520 6265 696e 6720 7265  You are being re
-000002c0: 6469 7265 6374 6564 2e20 506c 6561 7365  directed. Please
-000002d0: 2077 6169 742e 3c2f 6831 3e0a 2020 2020   wait.</h1>.    
-000002e0: 3c70 3e0a 2020 2020 2020 5765 2061 7265  <p>.      We are
-000002f0: 2063 6865 636b 696e 6720 6966 2074 6865   checking if the
-00000300: 7265 2069 7320 6120 7369 7465 2069 6e20  re is a site in 
-00000310: 796f 7572 2070 7265 6665 7272 6564 206c  your preferred l
-00000320: 616e 6775 6167 6520 616e 6420 7769 6c6c  anguage and will
-00000330: 2072 6564 6972 6563 7420 796f 7520 746f   redirect you to
-00000340: 2074 6861 742c 2069 6620 706f 7373 6962   that, if possib
-00000350: 6c65 2e0a 2020 2020 2020 4f74 6865 7277  le..      Otherw
-00000360: 6973 6520 7765 2077 696c 6c20 7265 6469  ise we will redi
-00000370: 7265 6374 2079 6f75 2074 6f20 7468 6520  rect you to the 
-00000380: 6465 6661 756c 7420 6c61 6e67 7561 6765  default language
-00000390: 2073 6974 652e 0a20 2020 203c 2f70 3e0a   site..    </p>.
-000003a0: 2020 2020 3c73 6372 6970 743e 0a20 2020      <script>.   
-000003b0: 2020 2061 7379 6e63 2066 756e 6374 696f     async functio
-000003c0: 6e20 7265 6469 7265 6374 2829 207b 0a20  n redirect() {. 
-000003d0: 2020 2020 2020 2063 6f6e 7374 2072 6573         const res
-000003e0: 706f 6e73 6520 3d20 6177 6169 7420 6665  ponse = await fe
-000003f0: 7463 6828 2763 6f6e 6669 672e 6a73 6f6e  tch('config.json
-00000400: 2729 3b0a 2020 2020 2020 2020 6966 2028  ');.        if (
-00000410: 7265 7370 6f6e 7365 2e73 7461 7475 7320  response.status 
-00000420: 213d 3d20 3230 3029 207b 0a20 2020 2020  !== 200) {.     
-00000430: 2020 2020 2072 6574 7572 6e3b 0a20 2020       return;.   
-00000440: 2020 2020 207d 0a20 2020 2020 2020 2063       }.        c
-00000450: 6f6e 7374 2063 6f6e 6669 6720 3d20 6177  onst config = aw
-00000460: 6169 7420 7265 7370 6f6e 7365 2e6a 736f  ait response.jso
-00000470: 6e28 290a 2020 2020 2020 2020 6c65 7420  n().        let 
-00000480: 666f 756e 6420 3d20 6661 6c73 653b 0a20  found = false;. 
-00000490: 2020 2020 2020 2066 6f72 2028 6c65 7420         for (let 
-000004a0: 636f 6465 206f 6620 6e61 7669 6761 746f  code of navigato
-000004b0: 722e 6c61 6e67 7561 6765 7329 207b 0a20  r.languages) {. 
-000004c0: 2020 2020 2020 2020 2069 6620 2863 6f64           if (cod
-000004d0: 652e 696e 6465 784f 6628 272d 2729 203e  e.indexOf('-') >
-000004e0: 2030 2920 7b0a 2020 2020 2020 2020 2020   0) {.          
-000004f0: 2020 636f 6465 203d 2063 6f64 652e 7375    code = code.su
-00000500: 6273 7472 696e 6728 302c 2063 6f64 652e  bstring(0, code.
-00000510: 696e 6465 784f 6628 272d 2729 293b 0a20  indexOf('-'));. 
-00000520: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00000530: 2020 2020 2066 6f72 2028 636f 6e73 7420       for (const 
-00000540: 636f 6e66 6967 4c61 6e67 7561 6765 206f  configLanguage o
-00000550: 6620 636f 6e66 6967 2e6c 616e 6775 6167  f config.languag
-00000560: 6573 2920 7b0a 2020 2020 2020 2020 2020  es) {.          
-00000570: 2020 6966 2028 636f 6465 203d 3d3d 2063    if (code === c
-00000580: 6f6e 6669 674c 616e 6775 6167 652e 636f  onfigLanguage.co
-00000590: 6465 2920 7b0a 2020 2020 2020 2020 2020  de) {.          
-000005a0: 2020 2020 7769 6e64 6f77 2e6c 6f63 6174      window.locat
-000005b0: 696f 6e20 3d20 7769 6e64 6f77 2e6c 6f63  ion = window.loc
-000005c0: 6174 696f 6e2e 6872 6566 202b 2063 6f6e  ation.href + con
-000005d0: 6669 674c 616e 6775 6167 652e 7061 7468  figLanguage.path
-000005e0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-000005f0: 666f 756e 6420 3d20 7472 7565 3b0a 2020  found = true;.  
-00000600: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00000610: 6b0a 2020 2020 2020 2020 2020 2020 7d0a  k.            }.
-00000620: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000630: 2020 2020 2020 6966 2028 666f 756e 6429        if (found)
-00000640: 207b 0a20 2020 2020 2020 2020 2020 2062   {.            b
-00000650: 7265 616b 0a20 2020 2020 2020 2020 207d  reak.          }
-00000660: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00000670: 2020 2069 6620 2821 666f 756e 6429 207b     if (!found) {
-00000680: 0a20 2020 2020 2020 2020 2077 696e 646f  .          windo
-00000690: 772e 6c6f 6361 7469 6f6e 203d 2077 696e  w.location = win
-000006a0: 646f 772e 6c6f 6361 7469 6f6e 2e68 7265  dow.location.hre
-000006b0: 6620 2b20 636f 6e66 6967 2e6c 616e 6775  f + config.langu
-000006c0: 6167 6573 5b30 5d2e 7061 7468 3b0a 2020  ages[0].path;.  
-000006d0: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
-000006e0: 2020 2020 2020 7265 6469 7265 6374 2829        redirect()
-000006f0: 3b0a 2020 2020 3c2f 7363 7269 7074 3e0a  ;.    </script>.
-00000700: 2020 3c2f 626f 6479 3e0a 3c2f 6874 6d6c    </body>.</html
-00000710: 3e0a 2222 220a 2020 2020 2020 2020 290a  >.""".        ).
-00000720: 0a0a 6465 6620 6675 6c6c 5f62 7569 6c64  ..def full_build
-00000730: 286c 616e 673a 2064 6963 7429 202d 3e20  (lang: dict) -> 
-00000740: 4e6f 6e65 3a0a 2020 2020 2222 2252 756e  None:.    """Run
-00000750: 2074 6865 2066 756c 6c20 6275 696c 6420   the full build 
-00000760: 7072 6f63 6573 7320 666f 7220 6120 7369  process for a si
-00000770: 6e67 6c65 206c 616e 6775 6167 652e 2222  ngle language.""
-00000780: 220a 2020 2020 6c61 6e64 696e 675f 6275  ".    landing_bu
-00000790: 696c 6428 290a 2020 2020 7375 6270 726f  ild().    subpro
-000007a0: 6365 7373 2e72 756e 280a 2020 2020 2020  cess.run(.      
-000007b0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000007c0: 226a 7570 7974 6572 2d62 6f6f 6b22 2c0a  "jupyter-book",.
-000007d0: 2020 2020 2020 2020 2020 2020 2262 7569              "bui
-000007e0: 6c64 222c 0a20 2020 2020 2020 2020 2020  ld",.           
-000007f0: 2022 2d2d 616c 6c22 2c0a 2020 2020 2020   "--all",.      
-00000800: 2020 2020 2020 222d 2d70 6174 682d 6f75        "--path-ou
-00000810: 7470 7574 222c 0a20 2020 2020 2020 2020  tput",.         
-00000820: 2020 2070 6174 682e 6a6f 696e 2822 5f62     path.join("_b
-00000830: 7569 6c64 222c 206c 616e 675b 2263 6f64  uild", lang["cod
-00000840: 6522 5d29 2c0a 2020 2020 2020 2020 2020  e"]),.          
-00000850: 2020 6c61 6e67 5b22 7061 7468 225d 2c0a    lang["path"],.
-00000860: 2020 2020 2020 2020 5d0a 2020 2020 290a          ].    ).
-00000870: 2020 2020 636f 7079 7472 6565 280a 2020      copytree(.  
-00000880: 2020 2020 2020 7061 7468 2e6a 6f69 6e28        path.join(
-00000890: 225f 6275 696c 6422 2c20 6c61 6e67 5b22  "_build", lang["
-000008a0: 636f 6465 225d 2c20 225f 6275 696c 6422  code"], "_build"
-000008b0: 2c20 2268 746d 6c22 292c 0a20 2020 2020  , "html"),.     
-000008c0: 2020 2070 6174 682e 6a6f 696e 2873 6574     path.join(set
-000008d0: 7469 6e67 735b 226f 7574 7075 7422 5d2c  tings["output"],
-000008e0: 206c 616e 675b 2263 6f64 6522 5d29 2c0a   lang["code"]),.
-000008f0: 2020 2020 2020 2020 6469 7273 5f65 7869          dirs_exi
-00000900: 7374 5f6f 6b3d 5472 7565 2c0a 2020 2020  st_ok=True,.    
-00000910: 290a 0a0a 6465 6620 7061 7274 6961 6c5f  )...def partial_
-00000920: 6275 696c 6428 6c61 6e67 3a20 6469 6374  build(lang: dict
-00000930: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-00000940: 2222 5275 6e20 7468 6520 6173 2d6e 6565  ""Run the as-nee
-00000950: 6465 6420 6275 696c 6420 7072 6f63 6573  ded build proces
-00000960: 7320 666f 7220 6120 7369 6e67 6c65 206c  s for a single l
-00000970: 616e 6775 6167 652e 2222 220a 2020 2020  anguage.""".    
-00000980: 6c61 6e64 696e 675f 6275 696c 6428 290a  landing_build().
-00000990: 2020 2020 7375 6270 726f 6365 7373 2e72      subprocess.r
-000009a0: 756e 280a 2020 2020 2020 2020 5b0a 2020  un(.        [.  
-000009b0: 2020 2020 2020 2020 2020 226a 7570 7974            "jupyt
-000009c0: 6572 2d62 6f6f 6b22 2c0a 2020 2020 2020  er-book",.      
-000009d0: 2020 2020 2020 2262 7569 6c64 222c 0a20        "build",. 
-000009e0: 2020 2020 2020 2020 2020 2022 2d2d 7061             "--pa
-000009f0: 7468 2d6f 7574 7075 7422 2c0a 2020 2020  th-output",.    
-00000a00: 2020 2020 2020 2020 7061 7468 2e6a 6f69          path.joi
-00000a10: 6e28 225f 6275 696c 6422 2c20 6c61 6e67  n("_build", lang
-00000a20: 5b22 636f 6465 225d 292c 0a20 2020 2020  ["code"]),.     
-00000a30: 2020 2020 2020 206c 616e 675b 2270 6174         lang["pat
-00000a40: 6822 5d2c 0a20 2020 2020 2020 205d 0a20  h"],.        ]. 
-00000a50: 2020 2029 0a20 2020 2063 6f70 7974 7265     ).    copytre
-00000a60: 6528 0a20 2020 2020 2020 2070 6174 682e  e(.        path.
-00000a70: 6a6f 696e 2822 5f62 7569 6c64 222c 206c  join("_build", l
-00000a80: 616e 675b 2263 6f64 6522 5d2c 2022 5f62  ang["code"], "_b
-00000a90: 7569 6c64 222c 2022 6874 6d6c 2229 2c0a  uild", "html"),.
-00000aa0: 2020 2020 2020 2020 7061 7468 2e6a 6f69          path.joi
-00000ab0: 6e28 7365 7474 696e 6773 5b22 6f75 7470  n(settings["outp
-00000ac0: 7574 225d 2c20 6c61 6e67 5b22 636f 6465  ut"], lang["code
-00000ad0: 225d 292c 0a20 2020 2020 2020 2064 6972  "]),.        dir
-00000ae0: 735f 6578 6973 745f 6f6b 3d54 7275 652c  s_exist_ok=True,
-00000af0: 0a20 2020 2029 0a0a 0a64 6566 2072 756e  .    )...def run
-00000b00: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-00000b10: 2222 2242 7569 6c64 2074 6865 2066 756c  """Build the ful
-00000b20: 6c20 7545 6469 7469 6f6e 2e22 2222 0a20  l uEdition.""". 
-00000b30: 2020 2069 6620 7061 7468 2e65 7869 7374     if path.exist
-00000b40: 7328 7365 7474 696e 6773 5b22 6f75 7470  s(settings["outp
-00000b50: 7574 225d 293a 0a20 2020 2020 2020 2072  ut"]):.        r
-00000b60: 6d74 7265 6528 7365 7474 696e 6773 5b22  mtree(settings["
-00000b70: 6f75 7470 7574 225d 290a 2020 2020 666f  output"]).    fo
-00000b80: 7220 6c61 6e67 2069 6e20 7365 7474 696e  r lang in settin
-00000b90: 6773 5b22 6c61 6e67 7561 6765 7322 5d3a  gs["languages"]:
-00000ba0: 0a20 2020 2020 2020 2066 756c 6c5f 6275  .        full_bu
-00000bb0: 696c 6428 6c61 6e67 290a                 ild(lang).
+00000000: 2320 5350 4458 2d46 696c 6543 6f70 7972  # SPDX-FileCopyr
+00000010: 6967 6874 5465 7874 3a20 3230 3233 2d70  ightText: 2023-p
+00000020: 7265 7365 6e74 204d 6172 6b20 4861 6c6c  resent Mark Hall
+00000030: 203c 6d61 726b 2e68 616c 6c40 776f 726b   <mark.hall@work
+00000040: 2e72 6f6f 6d33 622e 6575 3e0a 230a 2320  .room3b.eu>.#.# 
+00000050: 5350 4458 2d4c 6963 656e 7365 2d49 6465  SPDX-License-Ide
+00000060: 6e74 6966 6965 723a 204d 4954 0a22 2222  ntifier: MIT."""
+00000070: 4275 696c 6420 6675 6e63 7469 6f6e 616c  Build functional
+00000080: 6974 792e 2222 220a 696d 706f 7274 206a  ity.""".import j
+00000090: 736f 6e0a 696d 706f 7274 2073 7562 7072  son.import subpr
+000000a0: 6f63 6573 730a 0a66 726f 6d20 6f73 2069  ocess..from os i
+000000b0: 6d70 6f72 7420 7061 7468 2c20 6d61 6b65  mport path, make
+000000c0: 6469 7273 0a66 726f 6d20 7368 7574 696c  dirs.from shutil
+000000d0: 2069 6d70 6f72 7420 726d 7472 6565 2c20   import rmtree, 
+000000e0: 636f 7079 7472 6565 0a0a 6672 6f6d 202e  copytree..from .
+000000f0: 2e73 6574 7469 6e67 7320 696d 706f 7274  .settings import
+00000100: 2073 6574 7469 6e67 730a 0a0a 6465 6620   settings...def 
+00000110: 6c61 6e64 696e 675f 6275 696c 6428 2920  landing_build() 
+00000120: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+00000130: 4275 696c 6420 7468 6520 6c61 6e64 696e  Build the landin
+00000140: 6720 7061 6765 2e22 2222 0a20 2020 2069  g page.""".    i
+00000150: 6620 6e6f 7420 7061 7468 2e65 7869 7374  f not path.exist
+00000160: 7328 7365 7474 696e 6773 5b22 6f75 7470  s(settings["outp
+00000170: 7574 225d 293a 0a20 2020 2020 2020 206d  ut"]):.        m
+00000180: 616b 6564 6972 7328 7365 7474 696e 6773  akedirs(settings
+00000190: 5b22 6f75 7470 7574 225d 2c20 6578 6973  ["output"], exis
+000001a0: 745f 6f6b 3d54 7275 6529 0a20 2020 2077  t_ok=True).    w
+000001b0: 6974 6820 6f70 656e 2870 6174 682e 6a6f  ith open(path.jo
+000001c0: 696e 2873 6574 7469 6e67 735b 226f 7574  in(settings["out
+000001d0: 7075 7422 5d2c 2022 636f 6e66 6967 2e6a  put"], "config.j
+000001e0: 736f 6e22 292c 2022 7722 2920 6173 206f  son"), "w") as o
+000001f0: 7574 5f66 3a0a 2020 2020 2020 2020 6a73  ut_f:.        js
+00000200: 6f6e 2e64 756d 7028 7365 7474 696e 6773  on.dump(settings
+00000210: 2c20 6f75 745f 6629 0a20 2020 2077 6974  , out_f).    wit
+00000220: 6820 6f70 656e 2870 6174 682e 6a6f 696e  h open(path.join
+00000230: 2873 6574 7469 6e67 735b 226f 7574 7075  (settings["outpu
+00000240: 7422 5d2c 2022 696e 6465 782e 6874 6d6c  t"], "index.html
+00000250: 2229 2c20 2277 2229 2061 7320 6f75 745f  "), "w") as out_
+00000260: 663a 0a20 2020 2020 2020 206f 7574 5f66  f:.        out_f
+00000270: 2e77 7269 7465 280a 2020 2020 2020 2020  .write(.        
+00000280: 2020 2020 2222 225c 0a3c 2144 4f43 5459      """\.<!DOCTY
+00000290: 5045 2068 746d 6c3e 0a3c 6874 6d6c 3e0a  PE html>.<html>.
+000002a0: 2020 3c68 6561 643e 0a20 2020 203c 6d65    <head>.    <me
+000002b0: 7461 206e 616d 653d 2263 6861 7273 6574  ta name="charset
+000002c0: 2220 7661 6c75 653d 2275 7466 2d38 223e  " value="utf-8">
+000002d0: 0a20 2020 203c 7469 746c 653e 5265 6469  .    <title>Redi
+000002e0: 7265 6374 696e 672e 2e2e 2050 6c65 6173  recting... Pleas
+000002f0: 6520 7761 6974 2e2e 2e3c 2f74 6974 6c65  e wait...</title
+00000300: 3e0a 2020 3c2f 6865 6164 3e0a 2020 3c62  >.  </head>.  <b
+00000310: 6f64 793e 0a20 2020 203c 6831 3e59 6f75  ody>.    <h1>You
+00000320: 2061 7265 2062 6569 6e67 2072 6564 6972   are being redir
+00000330: 6563 7465 642e 2050 6c65 6173 6520 7761  ected. Please wa
+00000340: 6974 2e3c 2f68 313e 0a20 2020 203c 703e  it.</h1>.    <p>
+00000350: 0a20 2020 2020 2057 6520 6172 6520 6368  .      We are ch
+00000360: 6563 6b69 6e67 2069 6620 7468 6572 6520  ecking if there 
+00000370: 6973 2061 2073 6974 6520 696e 2079 6f75  is a site in you
+00000380: 7220 7072 6566 6572 7265 6420 6c61 6e67  r preferred lang
+00000390: 7561 6765 2061 6e64 2077 696c 6c20 7265  uage and will re
+000003a0: 6469 7265 6374 2079 6f75 2074 6f20 7468  direct you to th
+000003b0: 6174 2c20 6966 2070 6f73 7369 626c 652e  at, if possible.
+000003c0: 0a20 2020 2020 204f 7468 6572 7769 7365  .      Otherwise
+000003d0: 2077 6520 7769 6c6c 2072 6564 6972 6563   we will redirec
+000003e0: 7420 796f 7520 746f 2074 6865 2064 6566  t you to the def
+000003f0: 6175 6c74 206c 616e 6775 6167 6520 7369  ault language si
+00000400: 7465 2e0a 2020 2020 3c2f 703e 0a20 2020  te..    </p>.   
+00000410: 203c 7363 7269 7074 3e0a 2020 2020 2020   <script>.      
+00000420: 6173 796e 6320 6675 6e63 7469 6f6e 2072  async function r
+00000430: 6564 6972 6563 7428 2920 7b0a 2020 2020  edirect() {.    
+00000440: 2020 2020 636f 6e73 7420 7265 7370 6f6e      const respon
+00000450: 7365 203d 2061 7761 6974 2066 6574 6368  se = await fetch
+00000460: 2827 636f 6e66 6967 2e6a 736f 6e27 293b  ('config.json');
+00000470: 0a20 2020 2020 2020 2069 6620 2872 6573  .        if (res
+00000480: 706f 6e73 652e 7374 6174 7573 2021 3d3d  ponse.status !==
+00000490: 2032 3030 2920 7b0a 2020 2020 2020 2020   200) {.        
+000004a0: 2020 7265 7475 726e 3b0a 2020 2020 2020    return;.      
+000004b0: 2020 7d0a 2020 2020 2020 2020 636f 6e73    }.        cons
+000004c0: 7420 636f 6e66 6967 203d 2061 7761 6974  t config = await
+000004d0: 2072 6573 706f 6e73 652e 6a73 6f6e 2829   response.json()
+000004e0: 0a20 2020 2020 2020 206c 6574 2066 6f75  .        let fou
+000004f0: 6e64 203d 2066 616c 7365 3b0a 2020 2020  nd = false;.    
+00000500: 2020 2020 666f 7220 286c 6574 2063 6f64      for (let cod
+00000510: 6520 6f66 206e 6176 6967 6174 6f72 2e6c  e of navigator.l
+00000520: 616e 6775 6167 6573 2920 7b0a 2020 2020  anguages) {.    
+00000530: 2020 2020 2020 6966 2028 636f 6465 2e69        if (code.i
+00000540: 6e64 6578 4f66 2827 2d27 2920 3e20 3029  ndexOf('-') > 0)
+00000550: 207b 0a20 2020 2020 2020 2020 2020 2063   {.            c
+00000560: 6f64 6520 3d20 636f 6465 2e73 7562 7374  ode = code.subst
+00000570: 7269 6e67 2830 2c20 636f 6465 2e69 6e64  ring(0, code.ind
+00000580: 6578 4f66 2827 2d27 2929 3b0a 2020 2020  exOf('-'));.    
+00000590: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000005a0: 2020 666f 7220 2863 6f6e 7374 2063 6f6e    for (const con
+000005b0: 6669 674c 616e 6775 6167 6520 6f66 2063  figLanguage of c
+000005c0: 6f6e 6669 672e 6c61 6e67 7561 6765 7329  onfig.languages)
+000005d0: 207b 0a20 2020 2020 2020 2020 2020 2069   {.            i
+000005e0: 6620 2863 6f64 6520 3d3d 3d20 636f 6e66  f (code === conf
+000005f0: 6967 4c61 6e67 7561 6765 2e63 6f64 6529  igLanguage.code)
+00000600: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000610: 2077 696e 646f 772e 6c6f 6361 7469 6f6e   window.location
+00000620: 203d 2077 696e 646f 772e 6c6f 6361 7469   = window.locati
+00000630: 6f6e 2e68 7265 6620 2b20 636f 6e66 6967  on.href + config
+00000640: 4c61 6e67 7561 6765 2e70 6174 683b 0a20  Language.path;. 
+00000650: 2020 2020 2020 2020 2020 2020 2066 6f75               fou
+00000660: 6e64 203d 2074 7275 653b 0a20 2020 2020  nd = true;.     
+00000670: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00000680: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00000690: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+000006a0: 2020 2069 6620 2866 6f75 6e64 2920 7b0a     if (found) {.
+000006b0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+000006c0: 6b0a 2020 2020 2020 2020 2020 7d0a 2020  k.          }.  
+000006d0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000006e0: 6966 2028 2166 6f75 6e64 2920 7b0a 2020  if (!found) {.  
+000006f0: 2020 2020 2020 2020 7769 6e64 6f77 2e6c          window.l
+00000700: 6f63 6174 696f 6e20 3d20 7769 6e64 6f77  ocation = window
+00000710: 2e6c 6f63 6174 696f 6e2e 6872 6566 202b  .location.href +
+00000720: 2063 6f6e 6669 672e 6c61 6e67 7561 6765   config.language
+00000730: 735b 305d 2e70 6174 683b 0a20 2020 2020  s[0].path;.     
+00000740: 2020 207d 0a20 2020 2020 207d 0a20 2020     }.      }.   
+00000750: 2020 2072 6564 6972 6563 7428 293b 0a20     redirect();. 
+00000760: 2020 203c 2f73 6372 6970 743e 0a20 203c     </script>.  <
+00000770: 2f62 6f64 793e 0a3c 2f68 746d 6c3e 0a22  /body>.</html>."
+00000780: 2222 0a20 2020 2020 2020 2029 0a0a 0a64  "".        )...d
+00000790: 6566 2066 756c 6c5f 6275 696c 6428 6c61  ef full_build(la
+000007a0: 6e67 3a20 6469 6374 2920 2d3e 204e 6f6e  ng: dict) -> Non
+000007b0: 653a 0a20 2020 2022 2222 5275 6e20 7468  e:.    """Run th
+000007c0: 6520 6675 6c6c 2062 7569 6c64 2070 726f  e full build pro
+000007d0: 6365 7373 2066 6f72 2061 2073 696e 676c  cess for a singl
+000007e0: 6520 6c61 6e67 7561 6765 2e22 2222 0a20  e language.""". 
+000007f0: 2020 206c 616e 6469 6e67 5f62 7569 6c64     landing_build
+00000800: 2829 0a20 2020 2073 7562 7072 6f63 6573  ().    subproces
+00000810: 732e 7275 6e28 0a20 2020 2020 2020 205b  s.run(.        [
+00000820: 0a20 2020 2020 2020 2020 2020 2022 6a75  .            "ju
+00000830: 7079 7465 722d 626f 6f6b 222c 0a20 2020  pyter-book",.   
+00000840: 2020 2020 2020 2020 2022 6275 696c 6422           "build"
+00000850: 2c0a 2020 2020 2020 2020 2020 2020 222d  ,.            "-
+00000860: 2d61 6c6c 222c 0a20 2020 2020 2020 2020  -all",.         
+00000870: 2020 2022 2d2d 7061 7468 2d6f 7574 7075     "--path-outpu
+00000880: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00000890: 7061 7468 2e6a 6f69 6e28 225f 6275 696c  path.join("_buil
+000008a0: 6422 2c20 6c61 6e67 5b22 636f 6465 225d  d", lang["code"]
+000008b0: 292c 0a20 2020 2020 2020 2020 2020 206c  ),.            l
+000008c0: 616e 675b 2270 6174 6822 5d2c 0a20 2020  ang["path"],.   
+000008d0: 2020 2020 205d 0a20 2020 2029 0a20 2020       ].    ).   
+000008e0: 2063 6f70 7974 7265 6528 0a20 2020 2020   copytree(.     
+000008f0: 2020 2070 6174 682e 6a6f 696e 2822 5f62     path.join("_b
+00000900: 7569 6c64 222c 206c 616e 675b 2263 6f64  uild", lang["cod
+00000910: 6522 5d2c 2022 5f62 7569 6c64 222c 2022  e"], "_build", "
+00000920: 6874 6d6c 2229 2c0a 2020 2020 2020 2020  html"),.        
+00000930: 7061 7468 2e6a 6f69 6e28 7365 7474 696e  path.join(settin
+00000940: 6773 5b22 6f75 7470 7574 225d 2c20 6c61  gs["output"], la
+00000950: 6e67 5b22 636f 6465 225d 292c 0a20 2020  ng["code"]),.   
+00000960: 2020 2020 2064 6972 735f 6578 6973 745f       dirs_exist_
+00000970: 6f6b 3d54 7275 652c 0a20 2020 2029 0a0a  ok=True,.    )..
+00000980: 0a64 6566 2070 6172 7469 616c 5f62 7569  .def partial_bui
+00000990: 6c64 286c 616e 673a 2064 6963 7429 202d  ld(lang: dict) -
+000009a0: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2252  > None:.    """R
+000009b0: 756e 2074 6865 2061 732d 6e65 6564 6564  un the as-needed
+000009c0: 2062 7569 6c64 2070 726f 6365 7373 2066   build process f
+000009d0: 6f72 2061 2073 696e 676c 6520 6c61 6e67  or a single lang
+000009e0: 7561 6765 2e22 2222 0a20 2020 206c 616e  uage.""".    lan
+000009f0: 6469 6e67 5f62 7569 6c64 2829 0a20 2020  ding_build().   
+00000a00: 2073 7562 7072 6f63 6573 732e 7275 6e28   subprocess.run(
+00000a10: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+00000a20: 2020 2020 2020 2022 6a75 7079 7465 722d         "jupyter-
+00000a30: 626f 6f6b 222c 0a20 2020 2020 2020 2020  book",.         
+00000a40: 2020 2022 6275 696c 6422 2c0a 2020 2020     "build",.    
+00000a50: 2020 2020 2020 2020 222d 2d70 6174 682d          "--path-
+00000a60: 6f75 7470 7574 222c 0a20 2020 2020 2020  output",.       
+00000a70: 2020 2020 2070 6174 682e 6a6f 696e 2822       path.join("
+00000a80: 5f62 7569 6c64 222c 206c 616e 675b 2263  _build", lang["c
+00000a90: 6f64 6522 5d29 2c0a 2020 2020 2020 2020  ode"]),.        
+00000aa0: 2020 2020 6c61 6e67 5b22 7061 7468 225d      lang["path"]
+00000ab0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+00000ac0: 290a 2020 2020 636f 7079 7472 6565 280a  ).    copytree(.
+00000ad0: 2020 2020 2020 2020 7061 7468 2e6a 6f69          path.joi
+00000ae0: 6e28 225f 6275 696c 6422 2c20 6c61 6e67  n("_build", lang
+00000af0: 5b22 636f 6465 225d 2c20 225f 6275 696c  ["code"], "_buil
+00000b00: 6422 2c20 2268 746d 6c22 292c 0a20 2020  d", "html"),.   
+00000b10: 2020 2020 2070 6174 682e 6a6f 696e 2873       path.join(s
+00000b20: 6574 7469 6e67 735b 226f 7574 7075 7422  ettings["output"
+00000b30: 5d2c 206c 616e 675b 2263 6f64 6522 5d29  ], lang["code"])
+00000b40: 2c0a 2020 2020 2020 2020 6469 7273 5f65  ,.        dirs_e
+00000b50: 7869 7374 5f6f 6b3d 5472 7565 2c0a 2020  xist_ok=True,.  
+00000b60: 2020 290a 0a0a 6465 6620 7275 6e28 2920    )...def run() 
+00000b70: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+00000b80: 4275 696c 6420 7468 6520 6675 6c6c 2075  Build the full u
+00000b90: 4564 6974 696f 6e2e 2222 220a 2020 2020  Edition.""".    
+00000ba0: 6966 2070 6174 682e 6578 6973 7473 2873  if path.exists(s
+00000bb0: 6574 7469 6e67 735b 226f 7574 7075 7422  ettings["output"
+00000bc0: 5d29 3a0a 2020 2020 2020 2020 726d 7472  ]):.        rmtr
+00000bd0: 6565 2873 6574 7469 6e67 735b 226f 7574  ee(settings["out
+00000be0: 7075 7422 5d29 0a20 2020 2066 6f72 206c  put"]).    for l
+00000bf0: 616e 6720 696e 2073 6574 7469 6e67 735b  ang in settings[
+00000c00: 226c 616e 6775 6167 6573 225d 3a0a 2020  "languages"]:.  
+00000c10: 2020 2020 2020 6675 6c6c 5f62 7569 6c64        full_build
+00000c20: 286c 616e 6729 0a                        (lang).
```

### Comparing `uedition-0.4.0/uedition/cli/check.py` & `uedition-0.5.0/uedition/cli/check.py`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/uedition/cli/serve.py` & `uedition-0.5.0/uedition/cli/serve.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2023-present Mark Hall <mark.hall@work.room3b.eu>
+#
+# SPDX-License-Identifier: MIT
 """Local server that automatically rebuilds on changes."""
 from livereload import Server
 from os import path
 from typing import Callable
 
 from .build import full_build, partial_build
 from ..settings import settings
```

### Comparing `uedition-0.4.0/uedition/ext/config.py` & `uedition-0.5.0/uedition/ext/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2023-present Mark Hall <mark.hall@work.room3b.eu>
+#
+# SPDX-License-Identifier: MIT
 """uEdition configuration handling.
 
 This module handles reading the uEdition-specific configuration settings, validating them and
 adding any required default values.
 """
 from pydantic import BaseModel, validator, ValidationError
 from sphinx.application import Sphinx
```

### Comparing `uedition-0.4.0/uedition/ext/language_switcher.js` & `uedition-0.5.0/uedition/ext/language_switcher.js`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/uedition/ext/language_switcher.py` & `uedition-0.5.0/uedition/ext/language_switcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2023-present Mark Hall <mark.hall@work.room3b.eu>
+#
+# SPDX-License-Identifier: MIT
 """The Language Switcher extension."""
 import json
 
 from importlib.resources import files, as_file
 from os import path
 from sphinx.application import Sphinx
 from sphinx.util.fileutil import copy_asset_file
```

### Comparing `uedition-0.4.0/uedition/ext/tei.py` & `uedition-0.5.0/uedition/ext/tei.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2023-present Mark Hall <mark.hall@work.room3b.eu>
+#
+# SPDX-License-Identifier: MIT
 """TEI parsing extension for Sphinx."""
 from docutils import nodes
 from lxml import etree
 from sphinx.application import Sphinx
 from sphinx.parsers import Parser as SphinxParser
 from sphinx.writers.html import HTMLWriter
```

### Comparing `uedition-0.4.0/LICENSE.txt` & `uedition-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/README.md` & `uedition-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `uedition-0.4.0/pyproject.toml` & `uedition-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 dependencies = [
   "jupyter-book>=0.15.1,<1.0.0",
   "pydantic[dotenv]>=1.0.0,<2.0.0",
   "PyYAML>=6.0.0,<7.0.0",
   "typer[all]<1.0.0",
   "lxml>=4.9.2,<5.0.0",
   "livereload",
+  "copier>=8.0.0,<9.0.0",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 uEdition = "uedition.cli:app"
 
 [project.urls]
```

### Comparing `uedition-0.4.0/PKG-INFO` & `uedition-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: uEdition
-Version: 0.4.0
+Version: 0.5.0
 Project-URL: Documentation, https://github.com/unknown/uedition#readme
 Project-URL: Issues, https://github.com/unknown/uedition/issues
 Project-URL: Source, https://github.com/unknown/uedition
 Author-email: Mark Hall <mark.hall@work.room3b.eu>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
+Requires-Dist: copier<9.0.0,>=8.0.0
 Requires-Dist: jupyter-book<1.0.0,>=0.15.1
 Requires-Dist: livereload
 Requires-Dist: lxml<5.0.0,>=4.9.2
 Requires-Dist: pydantic[dotenv]<2.0.0,>=1.0.0
 Requires-Dist: pyyaml<7.0.0,>=6.0.0
 Requires-Dist: typer[all]<1.0.0
 Description-Content-Type: text/markdown
```

