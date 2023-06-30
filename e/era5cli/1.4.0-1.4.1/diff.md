# Comparing `tmp/era5cli-1.4.0.tar.gz` & `tmp/era5cli-1.4.1.tar.gz`

## Comparing `era5cli-1.4.0.tar` & `era5cli-1.4.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 era5cli-1.4.0/.bumpversion.cfg
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 era5cli-1.4.0/CITATION.cff
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 era5cli-1.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 era5cli-1.4.0/mkdocs.yml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 era5cli-1.4.0/readthedocs.yml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/.codecov.yml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/workflows/cffconvert.yml
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/workflows/test_and_build.yml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/workflows/test_codecov.yml
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/contribute.md
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/development_era5cli.md
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/formulating_requests.md
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/gen_reference_pages.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/general_development.md
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/getting_started.md
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/hourly_monthly.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/index.md
--rw-r--r--   0        0        0   107756 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/assets/era5cli_favicon.png
--rw-r--r--   0        0        0    96539 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/assets/era5cli_logo_colors.png
--rw-r--r--   0        0        0   135504 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/assets/era5cli_logo_colors_border.png
--rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/assets/era5cli_logo_white.svg
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/reference/arguments.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/reference/cli_usage.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/reference/variables.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/__version__.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/_request_size.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/cli.py
--rw-r--r--   0        0        0    21049 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/fetch.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/info.py
--rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/inputref.py
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/key_management.py
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/utils.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/__init__.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/common.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/config.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/info.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/periods.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_cli.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_config.py
--rw-r--r--   0        0        0    21778 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_fetch.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_info.py
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_integration.py
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_utils.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_version.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 era5cli-1.4.0/.gitignore
--rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 era5cli-1.4.0/LICENSE
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 era5cli-1.4.0/README.md
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 era5cli-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 era5cli-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 era5cli-1.4.1/.bumpversion.cfg
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 era5cli-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 era5cli-1.4.1/CITATION.cff
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 era5cli-1.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 era5cli-1.4.1/mkdocs.yml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 era5cli-1.4.1/readthedocs.yml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 era5cli-1.4.1/.github/.codecov.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 era5cli-1.4.1/.github/workflows/cffconvert.yml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 era5cli-1.4.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 era5cli-1.4.1/.github/workflows/test_and_build.yml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 era5cli-1.4.1/.github/workflows/test_codecov.yml
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/contribute.md
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/development_era5cli.md
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/formulating_requests.md
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/gen_reference_pages.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/general_development.md
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/getting_started.md
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/hourly_monthly.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/index.md
+-rw-r--r--   0        0        0   107756 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/assets/era5cli_favicon.png
+-rw-r--r--   0        0        0    96539 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/assets/era5cli_logo_colors.png
+-rw-r--r--   0        0        0   135504 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/assets/era5cli_logo_colors_border.png
+-rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/assets/era5cli_logo_white.svg
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/reference/arguments.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/reference/cli_usage.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/reference/variables.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 era5cli-1.4.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/__version__.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/_request_size.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/cli.py
+-rw-r--r--   0        0        0    21211 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/fetch.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/info.py
+-rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/inputref.py
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/key_management.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/utils.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/args/__init__.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/args/common.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/args/config.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/args/info.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 era5cli-1.4.1/era5cli/args/periods.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 era5cli-1.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 era5cli-1.4.1/tests/test_cli.py
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 era5cli-1.4.1/tests/test_config.py
+-rw-r--r--   0        0        0    22038 2020-02-02 00:00:00.000000 era5cli-1.4.1/tests/test_fetch.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 era5cli-1.4.1/tests/test_info.py
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 era5cli-1.4.1/tests/test_integration.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 era5cli-1.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 era5cli-1.4.1/tests/test_version.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 era5cli-1.4.1/.gitignore
+-rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 era5cli-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 era5cli-1.4.1/README.md
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 era5cli-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 era5cli-1.4.1/PKG-INFO
```

### Comparing `era5cli-1.4.0/CITATION.cff` & `era5cli-1.4.1/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -93,8 +93,8 @@
 doi: 10.5281/zenodo.3252665
 keywords:
   - "ERA5"
 license: Apache-2.0
 message: "If you use this software, please cite it using these metadata."
 repository-code: "https://github.com/ewatercycle/era5cli"
 title: era5cli
-version: "1.4.0"
+version: "1.4.1"
```

### Comparing `era5cli-1.4.0/CONTRIBUTING.md` & `era5cli-1.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/mkdocs.yml` & `era5cli-1.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/.github/workflows/publish-to-pypi.yml` & `era5cli-1.4.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/.github/workflows/test_and_build.yml` & `era5cli-1.4.1/.github/workflows/test_and_build.yml`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/.github/workflows/test_codecov.yml` & `era5cli-1.4.1/.github/workflows/test_codecov.yml`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/CHANGELOG.md` & `era5cli-1.4.1/docs/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,50 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+
+## 1.4.1 - 2023-06-30
+**Fixed:**
+
+ - Fix a bug that prevented the creation of the configuration file, if the "~/.config" folder did not exist yet ([#153](https://github.com/eWaterCycle/era5cli/pull/154)).
+
+**Added:**
+
+- The developer documentation now contains instructions on how to maintain the conda-forge feedstock for era5cli ([#150](https://github.com/eWaterCycle/era5cli/pull/154)).
+
+**Changed:**
+ 
+ - Before asking for a user input, a check is made if the code is running in an interactive terminal or not. If not (e.g. if era5cli is called through a different script and stdin is not available), the input request is skipped ([#152](https://github.com/eWaterCycle/era5cli/pull/154)).
+
+**Dev changes:**
+
+ - A pre-commit hook has been added, to facilitate pre-commit users. Documentation on the setup is added to the developer documentation ([#153](https://github.com/eWaterCycle/era5cli/pull/154)). 
+
+
 ## 1.4.0 - 2023-04-21
 **Added:**
 
  - Add validator for user's CDS keys. This should provide better feedback to users and reduce user error ([#138](https://github.com/eWaterCycle/era5cli/pull/138)).
- - Added `--splitmonths` argument for `era5cli hourly`. This allows users to avoid a Request Too Large error ([#138](https://github.com/eWaterCycle/era5cli/pull/138)).
- - When a request would encounter a Request Too Large error in the CDS API, they are warned, and given a suggestion to use the new `--splitmonths` argument ([#138](https://github.com/eWaterCycle/era5cli/pull/138)).
+ - Added `--splitmonths` argument for `era5cli hourly`. This allows users to avoid a Request Too Large error ([#139](https://github.com/eWaterCycle/era5cli/pull/139)).
+ - When a request would encounter a Request Too Large error in the CDS API, they are warned, and given a suggestion to use the new `--splitmonths` argument ([#139](https://github.com/eWaterCycle/era5cli/pull/139)).
  - Added -`-dashed-varname` argument, to produce file names where the variable name is separated using dashes. For example: `soil-type` vs. `soil_type`. For the ongoing discussion, see [#53](https://github.com/eWaterCycle/era5cli/issues/53).
 
 **Changed:**
 
  - Change CDS keys from cdsapi default `.cdsapirc` file to `.config/era5cli/cds_key.txt` file ([#138](https://github.com/eWaterCycle/era5cli/pull/138)).
    - This will avoid conflict with e.g. ADS keys
    - The user can configure the keys using `era5cli config`, no need to create a file in the right location.
- - When a request would encounter a Request Too Large error in the CDS API, they are warned, and given a suggestion to use `--splitmonths` ([#138](https://github.com/eWaterCycle/era5cli/pull/138)).
- - If a user makes a request without `--splitmonths` they are warned that the behavior will change in the future, and that they have to choose between `--splitmonths False` and `--splitmonths True` 
+ - When a request would encounter a Request Too Large error in the CDS API, they are warned, and given a suggestion to use `--splitmonths` ([#139](https://github.com/eWaterCycle/era5cli/pull/139)).
+ - If a user makes a request without `--splitmonths` they are warned that the behavior will change in the future, and that they have to choose between `--splitmonths False` and `--splitmonths True`
  - When a file already exists and would be overwritten, the user is prompted for confirmation. This should prevent accidental overwriting of files. This check can be skipped with the `--overwrite` flag ([#143](https://github.com/eWaterCycle/era5cli/pull/143)).
- - The earliest valid start year of requests has been updated to 1950 ([#146](https://github.com/eWaterCycle/era5cli/pull/146)).
+ - The earliest valid start year of ERA5 requests has been updated to 1940 (for ERA5-land it is still 1950) ([#146](https://github.com/eWaterCycle/era5cli/pull/146)).
  - Usage of `--prelimbe` now raises a deprecation warning. It will be deprecated in a future release, as all the back extension years are now included in the main products ([#147](https://github.com/eWaterCycle/era5cli/pull/147)).
  - The documentation has been fully overhauled, and now uses Markdown files & MkDocs ([#142](https://github.com/eWaterCycle/era5cli/pull/142), [#144](https://github.com/eWaterCycle/era5cli/pull/144)).
 
 **Dev changes:**
 
  - `cli.py` has been refactored to make the structure more clear. Seperate argument builders are now in their own modules ([#139](https://github.com/eWaterCycle/era5cli/pull/139)).
```

### Comparing `era5cli-1.4.0/docs/CODE_OF_CONDUCT.md` & `era5cli-1.4.1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/contribute.md` & `era5cli-1.4.1/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/development_era5cli.md` & `era5cli-1.4.1/docs/development_era5cli.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/formulating_requests.md` & `era5cli-1.4.1/docs/formulating_requests.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/gen_reference_pages.py` & `era5cli-1.4.1/docs/gen_reference_pages.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/general_development.md` & `era5cli-1.4.1/docs/general_development.md`

 * *Files 24% similar despite different names*

```diff
@@ -76,14 +76,25 @@
 
 ```sh
 hatch run format
 ```
 
 This will apply the `black` and `isort` formatting, and then check the code style.
 
+??? tip "Using pre-commit"
+    For pre-commit users, a pre-commit configuration has been added. This hook will execute the `hatch run format` command. 
+
+    After installing pre-commit in your python environment (`pip install pre-commit`), you can do
+    ```
+    pre-commit install
+    ```
+    to set up the git hook scripts.
+
+    For more information, see the [pre-commit website](https://pre-commit.com/).
+
 ## Generating the documentation
 
 To view the documentation locally, simply run the following command:
 
 ```sh
 hatch run docs:serve
 ```
@@ -115,22 +126,22 @@
 Open [releases](https://github.com/eWaterCycle/era5cli/releases) and draft a new release.
 Copy the changelog for this version into the description.
 Tag the release according to [semantic versioning guidelines](https://semver.org/), preceded with a `v` (e.g.: v1.0.0).
 The release title is the tag and the release date together (e.g.: v1.0.0 (2019-07-25)).
 
 ??? note "Release candidates"
     When releasing a release candidate on Github, tick the pre-release box, and amend the version tag with `-rc` and the candidate number.
-    Ensure the release candidate version is accurate in `CITATION.cff` and `era5cli/__version__.py`. 
+    Ensure the release candidate version is accurate in `CITATION.cff` and `era5cli/__version__.py`.
     If the version number in these files is not updated, Zenodo release workflows will fail.
 
     Publishing a new release in github triggers the github Action workflow that builds and publishes the package to test.PyPI or PyPI.
     Versions with "rc" (release candidate) in their version tag will only be published to test.PyPI.
-    Other version tags will trigger a PyPI release. 
+    Other version tags will trigger a PyPI release.
     Inspect `.github/workflows/publish-to-pypi.yml` for more information.
-    
+
     Confirm a release candidate on test.PyPI with:
     ```
     pip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ era5cli
     ```
 
 The release will:
 
@@ -145,7 +156,14 @@
 2. The publishing action ran successfully, and that `pip install era5cli` installs the new version.
 3. The [conda-forge package](https://anaconda.org/conda-forge/era5cli) is updated, and can be installed using conda.
 4. Wait a few hours, then confirm the addition of a new release on the [RSD](https://www.research-software.nl/software/era5cli).
 
 ??? note "Adding contributors to the Research Software Directory (RSD)"
     If any contributors have been added, or the description of the software has changed, this can be edited (by eScience Center employees) via the [RSD admin interface](https://www.research-software.nl/admin/).
     More information about this process (e.g. how to add a new contributor or new affiliation) can be found in the [RSD documentation](https://github.com/research-software-directory/research-software-directory/blob/master/docs/entering-data.md) or in [this blogpost](https://blog.esciencecenter.nl/the-research-software-directory-and-how-it-promotes-software-citation-4bd2137a6b8).
+
+### Maintaining the conda-forge release
+The new release on pypi will trigger the [conda-forge feedstock](https://github.com/conda-forge/era5cli-feedstock) to be automatically updated.
+
+If nothing changed to the build configuration, the automatic pull request should pass all tests, and can be merged by one of the maintainers.
+
+If the build changed, you can fork the feedstock repository to your own account, re-generate the `recipes/meta.yml` file (for example with [Grayskull](https://github.com/conda/grayskull)), and create a pull request to the feedstock.
```

### Comparing `era5cli-1.4.0/docs/getting_started.md` & `era5cli-1.4.1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/hourly_monthly.md` & `era5cli-1.4.1/docs/hourly_monthly.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/index.md` & `era5cli-1.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/assets/era5cli_favicon.png` & `era5cli-1.4.1/docs/assets/era5cli_favicon.png`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/assets/era5cli_logo_colors.png` & `era5cli-1.4.1/docs/assets/era5cli_logo_colors.png`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/assets/era5cli_logo_colors_border.png` & `era5cli-1.4.1/docs/assets/era5cli_logo_colors_border.png`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/assets/era5cli_logo_white.svg` & `era5cli-1.4.1/docs/assets/era5cli_logo_white.svg`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/reference/cli_usage.md` & `era5cli-1.4.1/docs/reference/cli_usage.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/docs/reference/variables.md` & `era5cli-1.4.1/docs/reference/variables.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/era5cli/__version__.py` & `era5cli-1.4.1/era5cli/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
     "Aytaç Paçal",
     "Stef Smeets",
     "Stefan Verhoeven",
     "Elizaveta Malinina",
     "Bart Schilperoort",
 )
 __email__ = "ewatercycle@esciencecenter.nl"
-__version__ = "1.4.0"
+__version__ = "1.4.1"
```

### Comparing `era5cli-1.4.0/era5cli/_request_size.py` & `era5cli-1.4.1/era5cli/_request_size.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/era5cli/cli.py` & `era5cli-1.4.1/era5cli/cli.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/era5cli/fetch.py` & `era5cli-1.4.1/era5cli/fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Fetch ERA5 variables."""
 
 import itertools
 import logging
 import os
+import sys
 import cdsapi
 from pathos.threading import ThreadPool as Pool
 import era5cli.inputref as ref
 import era5cli.utils
 from era5cli import key_management
 from era5cli._request_size import TooLargeRequestError
 from era5cli._request_size import request_too_large
@@ -541,11 +542,16 @@
                 os.linesep,
                 "Download request is being queued at Copernicus.",
                 os.linesep,
                 "It can take some time before downloading starts, ",
                 "please do not kill this process in the meantime.",
                 os.linesep,
             )
-            connection = cdsapi.Client(url=self.url, key=self.key, verify=True)
+            connection = cdsapi.Client(
+                url=self.url,
+                key=self.key,
+                verify=True,
+                progress=sys.stdin.isatty(),  # only show progress in interactive sesh.
+            )
             print("".join(queueing_message))  # print queueing message
             connection.retrieve(name, request, outputfile)
             era5cli.utils.append_history(name, request, outputfile)
```

### Comparing `era5cli-1.4.0/era5cli/info.py` & `era5cli-1.4.1/era5cli/info.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/era5cli/inputref.py` & `era5cli-1.4.1/era5cli/inputref.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/era5cli/key_management.py` & `era5cli-1.4.1/era5cli/key_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from pathlib import Path
 from typing import Tuple
 import cdsapi
 from requests.exceptions import ConnectionError  # pylint: disable=redefined-builtin
 
 
 ERA5CLI_CONFIG_PATH = Path.home() / ".config" / "era5cli" / "cds_key.txt"
@@ -131,15 +132,15 @@
 
     Returns:
         True if a valid key has been found & written to file. Otherwise False.
     """
     if CDSAPI_CONFIG_PATH.exists():
         url, fullkey = load_cdsapi_config()
         try:
-            if attempt_cds_login(url, fullkey):
+            if sys.stdin.isatty() and attempt_cds_login(url, fullkey):
                 userinput = input(
                     "Valid CDS keys found in the .cdsapirc file. Do you want to use "
                     "these for era5cli? [Y/n]"
                 )
                 if userinput in ["Y", "y", "Yes", "yes"]:
                     set_config(
                         url, uid=fullkey.split(":")[0], key=fullkey.split(":")[1]
@@ -155,15 +156,15 @@
         url = f.readline().replace("url:", "").strip()
         uid = f.readline().replace("uid:", "").strip()
         key = f.readline().replace("key:", "").strip()
     return url, f"{uid}:{key}"
 
 
 def write_era5cli_config(url: str, uid: str, key: str):
-    ERA5CLI_CONFIG_PATH.parent.mkdir(exist_ok=True)
+    ERA5CLI_CONFIG_PATH.parent.mkdir(exist_ok=True, parents=True)
     with open(ERA5CLI_CONFIG_PATH, mode="w", encoding="utf-8") as f:
         f.write(f"url: {url}\n")
         f.write(f"uid: {uid}\n")
         f.write(f"key: {key}\n")
 
 
 def load_cdsapi_config() -> Tuple[str, str]:
```

### Comparing `era5cli-1.4.0/era5cli/utils.py` & `era5cli-1.4.1/era5cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utility functions."""
 
 import datetime
 import shutil
+import sys
 import textwrap
 from pathlib import Path
 from typing import List
 import prettytable
 from netCDF4 import Dataset
 import era5cli
 from era5cli.__version__ import __version__ as era5cliversion
@@ -207,18 +208,21 @@
         f"{trues} and {falses} (case insensitive)."
     )
 
 
 def assert_outputfiles_not_exist(outputfiles: List[str]) -> None:
     """Check if files already exist, and prompt the user if they do."""
     if any(Path(file).exists() for file in outputfiles):
-        answer = input(
-            "\n  Some file(s) that will be downloaded already exist in this folder."
-            "\n  Do you want to overwrite them? (Y/N)"
-            "\n  Tip: to skip this flag, use `--overwrite`."
-            "\n"
-        )
-        if answer.lower() in ["n", "no", "nope"]:
+        answer = "no"  # default answer for non-interactive sessions
+        if sys.stdin.isatty():  # only ask for input if the user can reply.
+            answer = input(
+                "\n  Some file(s) that will be downloaded already exist in this folder."
+                "\n  To always overwrite use `--overwrite` flag."
+                "\n  Do you want to overwrite any existing files? (Y/N)"
+            )
+        if answer.lower() not in ["y", "yes", "yup", "ja"]:
             raise FileExistsError(
                 "\n  One or more files already exist in this folder."
-                "\n  Please remove them, or change to a different folder to continue"
+                "\n  Please remove them, change to a different folder, or use the"
+                "\n  --overwrite flag to always overwrite existing files."
+                "\n"
             )
```

### Comparing `era5cli-1.4.0/era5cli/args/common.py` & `era5cli-1.4.1/era5cli/args/common.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/era5cli/args/config.py` & `era5cli-1.4.1/era5cli/args/config.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/era5cli/args/info.py` & `era5cli-1.4.1/era5cli/args/info.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/era5cli/args/periods.py` & `era5cli-1.4.1/era5cli/args/periods.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/tests/test_cli.py` & `era5cli-1.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/tests/test_config.py` & `era5cli-1.4.1/tests/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import pytest
 import requests.exceptions as rex
 from era5cli import key_management
 
 
 @pytest.fixture(scope="function")
 def empty_path_era5(tmp_path_factory):
-    return tmp_path_factory.mktemp(".config") / "era5cli.txt"
+    return tmp_path_factory.mktemp("usrhome") / ".config" / "era5cli" / "cds_keys.txt"
 
 
 @pytest.fixture(scope="function")
 def valid_path_era5(tmp_path_factory):
-    fn = tmp_path_factory.mktemp(".config") / "era5cli.txt"
+    fn = tmp_path_factory.mktemp(".config") / "era5cli" / "cds_keys.txt"
+    fn.parent.mkdir(parents=True)
     with open(fn, mode="w", encoding="utf-8") as f:
         f.write("url: b\nuid: 123\nkey: abc-def\n")
     return fn
 
 
 @pytest.fixture(scope="function")
 def empty_path_cds(tmp_path_factory):
@@ -27,15 +28,20 @@
     fn = tmp_path_factory.mktemp(".config") / "cdsapirc.txt"
     with open(fn, mode="w", encoding="utf-8") as f:
         f.write("url: a\nkey: 123:abc-def")
     return fn
 
 
 class TestEra5CliConfig:
-    """Test the functionality when the /.config/era5cli.txt file exists."""
+    """Test the functionality for writing and loading the config file."""
+
+    def test_set_config(self, empty_path_era5):
+        with patch("era5cli.key_management.ERA5CLI_CONFIG_PATH", empty_path_era5):
+            key_management.write_era5cli_config(url="b", uid="123", key="abc-def")
+            assert key_management.load_era5cli_config() == ("b", "123:abc-def")
 
     def test_load_era5cli_config(self, valid_path_era5):
         with patch("era5cli.key_management.ERA5CLI_CONFIG_PATH", valid_path_era5):
             assert key_management.load_era5cli_config() == ("b", "123:abc-def")
 
     def test_check_era5cli_config(self, valid_path_era5):
         mp1 = patch("era5cli.key_management.ERA5CLI_CONFIG_PATH", valid_path_era5)
@@ -55,40 +61,43 @@
 
     def test_cdsrcfile_user_says_no(self, empty_path_era5, valid_path_cds):
         """.cdsapirc exists. User says no. Should raise InvalidLoginError"""
         mp1 = patch("builtins.input", return_value="N")
         mp2 = patch("era5cli.key_management.attempt_cds_login", return_value=True)
         mp3 = patch("era5cli.key_management.ERA5CLI_CONFIG_PATH", empty_path_era5)
         mp4 = patch("era5cli.key_management.CDSAPI_CONFIG_PATH", valid_path_cds)
-        with mp1, mp2, mp3, mp4:
+        mp5 = patch("sys.stdin.isatty", return_value=True)
+        with mp1, mp2, mp3, mp4, mp5:
             with pytest.raises(
                 key_management.InvalidLoginError, match="No valid CDS login found"
             ):
                 key_management.check_era5cli_config()
 
     def test_cdsrcfile_user_says_yes(self, empty_path_era5, valid_path_cds):
         """.cdsapirc exists. User says yes. url+key is copied to the era5cli config."""
         mp1 = patch("builtins.input", return_value="Y")
         mp2 = patch("era5cli.key_management.attempt_cds_login", return_value=True)
         mp3 = patch("era5cli.key_management.ERA5CLI_CONFIG_PATH", empty_path_era5)
         mp4 = patch("era5cli.key_management.CDSAPI_CONFIG_PATH", valid_path_cds)
-        with mp1, mp2, mp3, mp4:
+        mp5 = patch("sys.stdin.isatty", return_value=True)
+        with mp1, mp2, mp3, mp4, mp5:
             key_management.check_era5cli_config()
             with open(empty_path_era5, "r", encoding="utf-8") as f:
                 assert f.readlines() == ["url: a\n", "uid: 123\n", "key: abc-def\n"]
 
     def test_cdsrcfile_invalid_keys(self, empty_path_era5, valid_path_cds):
         """.cdsapirc exists. url+key is validated, and is bad."""
         mp1 = patch(
             "era5cli.key_management.attempt_cds_login",
             side_effect=key_management.InvalidLoginError,
         )
         mp2 = patch("era5cli.key_management.ERA5CLI_CONFIG_PATH", empty_path_era5)
         mp3 = patch("era5cli.key_management.CDSAPI_CONFIG_PATH", valid_path_cds)
-        with mp1, mp2, mp3:
+        mp4 = patch("sys.stdin.isatty", return_value=True)
+        with mp1, mp2, mp3, mp4:
             with pytest.raises(
                 key_management.InvalidLoginError, match="No valid CDS login found"
             ):
                 key_management.check_era5cli_config()
 
 
 class TestAttemptCdsLogin:
```

### Comparing `era5cli-1.4.0/tests/test_fetch.py` & `era5cli-1.4.1/tests/test_fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -656,19 +656,26 @@
         era5._build_request("total_precipitation", [2008])
 
 
 def test_file_exists():
     with mock.patch.object(pathlib.Path, "exists", return_value=True):
         era5 = initialize()
 
-        with mock.patch("builtins.input", return_value="Y"):
+        mp_yes = mock.patch("builtins.input", return_value="Y")
+        mp_no = mock.patch("builtins.input", return_value="N")
+        mp_atty = mock.patch("sys.stdin.isatty", return_value=True)
+        with mp_yes, mp_atty:
             era5.fetch(dryrun=True)
 
-        with mock.patch("builtins.input", return_value="N"):
+        with mp_no, mp_atty:
             with pytest.raises(FileExistsError):
                 era5.fetch(dryrun=True)
 
+        # Last one should have isatty->False.
+        with pytest.raises(FileExistsError):
+            era5.fetch(dryrun=True)
+
 
 def test_overwrite():
     with mock.patch.object(pathlib.Path, "exists", return_value=True):
         era5 = initialize(overwrite=True)
         era5.fetch(dryrun=True)
```

### Comparing `era5cli-1.4.0/tests/test_info.py` & `era5cli-1.4.1/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/tests/test_integration.py` & `era5cli-1.4.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/tests/test_utils.py` & `era5cli-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/.gitignore` & `era5cli-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/LICENSE` & `era5cli-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/README.md` & `era5cli-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/pyproject.toml` & `era5cli-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `era5cli-1.4.0/PKG-INFO` & `era5cli-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: era5cli
-Version: 1.4.0
+Version: 1.4.1
 Summary: A command line interface to download ERA5 data from the Copernicus Climate Data Store. https://climate.copernicus.eu/..
 Author: Ronald van Haren, Jaro Camphuijsen, Yifat Dzigan, Niels Drost, Fakhereh Alidoost, Bouwe Andela, Jerom Aerts, Berend Weel, Rolf Hut, Klaus Zimmermann, Peter Kalverla, Aytaç Paçal, Stef Smeets, Stefan Verhoeven, Elizaveta Malinina
 Author-email: Barbara Vreede <b.vreede@esciencecenter.nl>, Bart Schilperoort <b.schilperoort@esciencecenter.nl>
 License: Apache Software License
 License-File: LICENSE
 Keywords: ERA-5,cds api,cds download,climate data
 Classifier: Development Status :: 5 - Production/Stable
```

