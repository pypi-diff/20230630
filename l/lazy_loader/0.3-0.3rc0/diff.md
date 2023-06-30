# Comparing `tmp/lazy_loader-0.3.tar.gz` & `tmp/lazy_loader-0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_loader-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lazy_loader-0.3rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lazy_loader-0.3.tar` & `lazy_loader-0.3rc0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      207 2023-06-28 01:54:21.971546 lazy_loader-0.3/.github/dependabot.yml
--rw-r--r--   0        0        0      998 2023-06-08 18:17:17.686092 lazy_loader-0.3/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      830 2023-06-08 18:17:17.686092 lazy_loader-0.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      994 2023-06-27 19:28:19.549616 lazy_loader-0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      318 2023-06-08 18:17:17.686092 lazy_loader-0.3/.gitignore
--rw-r--r--   0        0        0     1025 2023-06-28 01:54:21.971546 lazy_loader-0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8274 2023-06-30 21:04:45.684111 lazy_loader-0.3/CHANGELOG.md
--rw-r--r--   0        0        0     1539 2023-06-08 18:17:17.686092 lazy_loader-0.3/LICENSE.md
--rw-r--r--   0        0        0     3361 2023-06-28 01:54:21.971546 lazy_loader-0.3/README.md
--rw-r--r--   0        0        0     1419 2023-06-30 20:21:20.615294 lazy_loader-0.3/RELEASE.md
--rw-r--r--   0        0        0     8555 2023-06-28 01:54:21.972546 lazy_loader-0.3/lazy_loader/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 18:17:17.686092 lazy_loader-0.3/lazy_loader/tests/__init__.py
--rw-r--r--   0        0        0      136 2023-06-08 18:17:17.687091 lazy_loader-0.3/lazy_loader/tests/fake_pkg/__init__.py
--rw-r--r--   0        0        0       33 2023-06-27 20:26:36.582245 lazy_loader-0.3/lazy_loader/tests/fake_pkg/__init__.pyi
--rw-r--r--   0        0        0       74 2023-06-08 18:17:17.687091 lazy_loader-0.3/lazy_loader/tests/fake_pkg/some_func.py
--rw-r--r--   0        0        0     4468 2023-06-28 01:54:21.972546 lazy_loader-0.3/lazy_loader/tests/test_lazy_loader.py
--rw-r--r--   0        0        0     1189 2023-06-30 21:08:43.595186 lazy_loader-0.3/pyproject.toml
--rw-r--r--   0        0        0     4309 1970-01-01 00:00:00.000000 lazy_loader-0.3/PKG-INFO
+-rw-r--r--   0        0        0      207 2023-06-28 01:54:21.971546 lazy_loader-0.3rc0/.github/dependabot.yml
+-rw-r--r--   0        0        0      998 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      830 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      994 2023-06-27 19:28:19.549616 lazy_loader-0.3rc0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      318 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/.gitignore
+-rw-r--r--   0        0        0     1025 2023-06-28 01:54:21.971546 lazy_loader-0.3rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6916 2023-06-30 20:16:43.694958 lazy_loader-0.3rc0/CHANGELOG.md
+-rw-r--r--   0        0        0     1539 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/LICENSE.md
+-rw-r--r--   0        0        0     3361 2023-06-28 01:54:21.971546 lazy_loader-0.3rc0/README.md
+-rw-r--r--   0        0        0     1419 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/RELEASE.md
+-rw-r--r--   0        0        0     8555 2023-06-28 01:54:21.972546 lazy_loader-0.3rc0/lazy_loader/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/lazy_loader/tests/__init__.py
+-rw-r--r--   0        0        0      136 2023-06-08 18:17:17.687091 lazy_loader-0.3rc0/lazy_loader/tests/fake_pkg/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-27 20:26:36.582245 lazy_loader-0.3rc0/lazy_loader/tests/fake_pkg/__init__.pyi
+-rw-r--r--   0        0        0       74 2023-06-08 18:17:17.687091 lazy_loader-0.3rc0/lazy_loader/tests/fake_pkg/some_func.py
+-rw-r--r--   0        0        0     4468 2023-06-28 01:54:21.972546 lazy_loader-0.3rc0/lazy_loader/tests/test_lazy_loader.py
+-rw-r--r--   0        0        0     1192 2023-06-30 20:17:15.640112 lazy_loader-0.3rc0/pyproject.toml
+-rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 lazy_loader-0.3rc0/PKG-INFO
```

### Comparing `lazy_loader-0.3/.github/workflows/coverage.yml` & `lazy_loader-0.3rc0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3/.github/workflows/lint.yml` & `lazy_loader-0.3rc0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3/.github/workflows/test.yml` & `lazy_loader-0.3rc0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3/.pre-commit-config.yaml` & `lazy_loader-0.3rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3/CHANGELOG.md` & `lazy_loader-0.3rc0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,9 @@
 # Changelog
 
-## [v0.3](https://github.com/scientific-python/lazy_loader/tree/v0.3) (2023-06-30)
-
-[Full Changelog](https://github.com/scientific-python/lazy_loader/compare/v0.2...v0.3)
-
-**Merged pull requests:**
-
-- Announce Python 3.12 support [\#63](https://github.com/scientific-python/lazy_loader/pull/63) ([jarrodmillman](https://github.com/jarrodmillman))
-- Ignore B028 [\#62](https://github.com/scientific-python/lazy_loader/pull/62) ([jarrodmillman](https://github.com/jarrodmillman))
-- Use dependabot to update requirements [\#61](https://github.com/scientific-python/lazy_loader/pull/61) ([jarrodmillman](https://github.com/jarrodmillman))
-- Use dependabot to update GH actions [\#60](https://github.com/scientific-python/lazy_loader/pull/60) ([jarrodmillman](https://github.com/jarrodmillman))
-- Use ruff [\#59](https://github.com/scientific-python/lazy_loader/pull/59) ([jarrodmillman](https://github.com/jarrodmillman))
-- Update requirements [\#58](https://github.com/scientific-python/lazy_loader/pull/58) ([jarrodmillman](https://github.com/jarrodmillman))
-- Warn and discourage lazy.load of subpackages [\#57](https://github.com/scientific-python/lazy_loader/pull/57) ([dschult](https://github.com/dschult))
-- Test on Python 3.12.0-beta.2 [\#53](https://github.com/scientific-python/lazy_loader/pull/53) ([jarrodmillman](https://github.com/jarrodmillman))
-
 ## [v0.2](https://github.com/scientific-python/lazy_loader/tree/v0.2)
 
 [Full Changelog](https://github.com/scientific-python/lazy_loader/compare/v0.1...v0.2)
 
 There were no changes since the release candidate, so
 see release notes for v0.2rc0 below for details.
```

### Comparing `lazy_loader-0.3/LICENSE.md` & `lazy_loader-0.3rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3/README.md` & `lazy_loader-0.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3/RELEASE.md` & `lazy_loader-0.3rc0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3/lazy_loader/__init__.py` & `lazy_loader-0.3rc0/lazy_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3/lazy_loader/tests/test_lazy_loader.py` & `lazy_loader-0.3rc0/lazy_loader/tests/test_lazy_loader.py`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3/pyproject.toml` & `lazy_loader-0.3rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.8,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "lazy_loader"
-version = "0.3"
+version = "0.3rc0"
 requires-python = ">=3.7"
 authors = [{name = "Scientific Python Developers"}]
 readme = "README.md"
 license = {file = "LICENSE.md"}
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: BSD License",
```

### Comparing `lazy_loader-0.3/PKG-INFO` & `lazy_loader-0.3rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy_loader
-Version: 0.3
+Version: 0.3rc0
 Summary: lazy_loader
 Author: Scientific Python Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

