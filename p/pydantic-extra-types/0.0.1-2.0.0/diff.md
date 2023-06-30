# Comparing `tmp/pydantic_extra_types-0.0.1.tar.gz` & `tmp/pydantic_extra_types-2.0.0.tar.gz`

## Comparing `pydantic_extra_types-0.0.1.tar` & `pydantic_extra_types-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,38 @@
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pydantic_extra_types-0.0.1/pydantic_extra_types/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pydantic_extra_types-0.0.1/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_extra_types-0.0.1/LICENSE
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pydantic_extra_types-0.0.1/README.md
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 pydantic_extra_types-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 pydantic_extra_types-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/Makefile
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/mkdocs.yml
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/docs/color_types.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/docs/favicon.png
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/docs/logo-white.svg
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/docs/payment_cards.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/docs/phone_numbers.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/docs/routing_numbers.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/docs/extra/terminal.css
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/docs/extra/tweaks.css
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/docs/theme/main.html
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/pydantic_extra_types/__init__.py
+-rw-r--r--   0        0        0    21389 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/pydantic_extra_types/color.py
+-rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/pydantic_extra_types/country.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/pydantic_extra_types/payment.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/pydantic_extra_types/phone_numbers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/pydantic_extra_types/py.typed
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/pydantic_extra_types/routing_number.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/requirements/all.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/requirements/linting.in
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/requirements/linting.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/requirements/pyproject.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/requirements/testing.in
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/requirements/testing.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/tests/test_country_code.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/tests/test_json_schema.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/tests/test_phone_numbers.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/tests/test_routing_number.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/tests/test_types_color.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/tests/test_types_payment.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/LICENSE
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/README.md
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pydantic_extra_types-2.0.0/PKG-INFO
```

### Comparing `pydantic_extra_types-0.0.1/LICENSE` & `pydantic_extra_types-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_extra_types-0.0.1/pyproject.toml` & `pydantic_extra_types-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 path = 'pydantic_extra_types/__init__.py'
 
 [project]
 name = 'pydantic-extra-types'
 description = 'Extra Pydantic types.'
 authors = [
     {name = 'Samuel Colvin', email = 's@muelcolvin.com'},
+    {name = 'Yasser Tahiri', email = 'hello@yezz.me'},
 ]
 license = 'MIT'
 readme = 'README.md'
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
@@ -27,101 +28,82 @@
     'Intended Audience :: Information Technology',
     'Intended Audience :: System Administrators',
     'License :: OSI Approved :: MIT License',
     'Operating System :: Unix',
     'Operating System :: POSIX :: Linux',
     'Environment :: Console',
     'Environment :: MacOS X',
+    'Framework :: Pydantic',
+    'Framework :: Pydantic :: 2',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 requires-python = '>=3.7'
 dependencies = [
-    'pydantic',
+    'pydantic>=2.0b3',
 ]
 dynamic = ['version']
 
+[project.optional-dependencies]
+all = [
+    'phonenumbers>=8,<9',
+    'pycountry>=22,<23',
+]
+
 [project.urls]
 Homepage = 'https://github.com/pydantic/pydantic-extra-types'
 Source = 'https://github.com/pydantic/pydantic-extra-types'
 Changelog = 'https://github.com/pydantic/pydantic-extra-types/releases'
-# TODO: Documentation
-
-[tool.pytest.ini_options]
-testpaths = 'tests'
-filterwarnings = [
-    'error',
-]
+Documentation = 'https://docs.pydantic.dev/dev-v2/usage/types/types/'
 
-[tool.flake8]
-max_line_length = 120
-max_complexity = 14
-inline_quotes = 'single'
-multiline_quotes = 'double'
-ignore = ['E203', 'W503']
+[tool.ruff]
+line-length = 120
+extend-select = ['Q', 'RUF100', 'C90', 'UP', 'I']
+isort = { known-first-party = ['pydantic_extra_types', 'tests'] }
+flake8-quotes = {inline-quotes = 'single', multiline-quotes = 'double'}
+mccabe = { max-complexity = 14 }
 
 [tool.coverage.run]
 source = ['pydantic_extra_types']
 branch = true
 context = '${CONTEXT}'
 
+[tool.coverage.paths]
+source = [
+    'pydantic_extra_types/',
+    '/Users/runner/work/pydantic-extra-types/pydantic-extra-types/pydantic_extra_types/',
+    'D:\a\pydantic-extra-types\pydantic-extra-types\pydantic_extra_types',
+]
+
 [tool.coverage.report]
 precision = 2
+fail_under = 100
+show_missing = true
+skip_covered = true
 exclude_lines = [
     'pragma: no cover',
     'raise NotImplementedError',
-    'raise NotImplemented',
     'if TYPE_CHECKING:',
     '@overload',
 ]
 
-
-[tool.coverage.paths]
-source = [
-    'pydantic_extra_types/',
-]
-
 [tool.black]
 color = true
 line-length = 120
-target-version = ['py310']
+target-version = ['py37']
 skip-string-normalization = true
 
-[tool.isort]
-line_length = 120
-known_first_party = 'pydantic_extra_types'
-known_third_party = 'pydantic'
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-combine_as_imports = true
-
 [tool.mypy]
-python_version = '3.10'
-show_error_codes = true
-follow_imports = 'silent'
-strict_optional = true
-warn_redundant_casts = true
-warn_unused_ignores = true
-disallow_any_generics = true
-check_untyped_defs = true
-no_implicit_reexport = true
-warn_unused_configs = true
-disallow_subclassing_any = true
-disallow_incomplete_defs = true
-disallow_untyped_decorators = true
-disallow_untyped_calls = true
-
-# for strict mypy: (this is the tricky one :-))
-disallow_untyped_defs = true
-
-# remaining arguments from `mypy --strict` which cause errors
-# no_implicit_optional = true
-# warn_return_any = true
-
-# ansi2html and devtools are required to avoid the need to install these packages when running linting,
-# they're used in the docs build script
-[[tool.mypy.overrides]]
-module = [
-    'dotenv.*',
+strict = true
+plugins = 'pydantic.mypy'
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    'error',
+    # This ignore will be removed when pycountry will drop py36 & support py311
+    'ignore:::pkg_resources',
 ]
-ignore_missing_imports = true
+
+# configuring https://github.com/pydantic/hooky
+[tool.hooky]
+reviewers = ['yezz123', 'Kludex']
+require_change_file = false
```

