# Comparing `tmp/pyproject_examples-2022.5.3.tar.gz` & `tmp/pyproject_examples-2023.6.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_examples-2022.5.3.tar", last modified: Tue May  3 10:38:04 2022, max compression
+gzip compressed data, was "pyproject_examples-2023.6.30.tar", last modified: Fri Jun 30 09:36:47 2023, max compression
```

## Comparing `pyproject_examples-2022.5.3.tar` & `pyproject_examples-2023.6.30.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0 runner    (1001) docker     (121)     8684 2022-05-03 10:38:04.840873 pyproject_examples-2022.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-05-03 10:38:04.840873 pyproject_examples-2022.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     7714 2022-05-03 10:38:04.840873 pyproject_examples-2022.5.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-05-03 10:38:04.836873 pyproject_examples-2022.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-03 10:38:04.840873 pyproject_examples-2022.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9274 2022-05-03 10:37:26.754195 pyproject_examples-2022.5.3/pyproject_examples/example_configs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-05-03 10:37:26.754195 pyproject_examples-2022.5.3/pyproject_examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8576 2022-05-03 10:37:26.754195 pyproject_examples-2022.5.3/pyproject_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 10:37:26.754195 pyproject_examples-2022.5.3/pyproject_examples/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-06-30 09:36:47.358292 pyproject_examples-2023.6.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     8719 2023-06-30 09:36:47.362292 pyproject_examples-2023.6.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-30 09:36:47.358292 pyproject_examples-2023.6.30/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-06-30 09:36:47.354292 pyproject_examples-2023.6.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7717 2023-06-30 09:36:47.358292 pyproject_examples-2023.6.30/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:36:10.070021 pyproject_examples-2023.6.30/pyproject_examples/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    10051 2023-06-30 09:36:10.070021 pyproject_examples-2023.6.30/pyproject_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1616 2023-06-30 09:36:10.070021 pyproject_examples-2023.6.30/pyproject_examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9274 2023-06-30 09:36:10.070021 pyproject_examples-2023.6.30/pyproject_examples/example_configs.py
```

### Comparing `pyproject_examples-2022.5.3/PKG-INFO` & `pyproject_examples-2023.6.30/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pyproject-examples
-Version: 2022.5.3
+Version: 2023.6.30
 Summary: Example pyproject.toml configs for testing.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Home-page: https://github.com/repo-helper/pyproject-examples
 Project-URL: Issue Tracker, https://github.com/repo-helper/pyproject-examples/issues
 Project-URL: Source Code, https://github.com/repo-helper/pyproject-examples
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: coincidence>=0.4.0
 Requires-Dist: dom-toml>=0.4.0
+Requires-Dist: packaging>=21.3
 Requires-Dist: pytest>=6.2.3
 Description-Content-Type: text/x-rst
 
 
 ###################
 pyproject-examples
 ###################
@@ -72,16 +73,16 @@
 	:target: https://github.com/repo-helper/pyproject-examples/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/pyproject-examples/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/pyproject-examples/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-examples/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-examples/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-examples/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-examples/
 	:alt: Requirements Status
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/pyproject-examples?logo=codefactor
 	:target: https://www.codefactor.io/repository/github/repo-helper/pyproject-examples
 	:alt: CodeFactor Grade
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/pyproject-examples
@@ -103,23 +104,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-examples
 	:target: https://github.com/repo-helper/pyproject-examples/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-examples
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-examples/v2022.5.3
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-examples/v2023.6.30
 	:target: https://github.com/repo-helper/pyproject-examples/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-examples
 	:target: https://github.com/repo-helper/pyproject-examples/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pyproject-examples
 	:target: https://pypi.org/project/pyproject-examples/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `pyproject_examples-2022.5.3/pyproject.toml` & `pyproject_examples-2023.6.30/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "pyproject-examples"
-version = "2022.5.3"
+version = "2023.6.30"
 description = "Example pyproject.toml configs for testing."
 readme = "README.rst"
+requires-python = ">=3.6"
 keywords = []
 dynamic = []
-dependencies = [ "coincidence>=0.4.0", "dom-toml>=0.4.0", "pytest>=6.2.3",]
+dependencies = [ "coincidence>=0.4.0", "dom-toml>=0.4.0", "packaging>=21.3", "pytest>=6.2.3",]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Typed",
 ]
-requires-python = ">=3.6"
 
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
 
 [project.license]
@@ -35,22 +35,22 @@
 "Source Code" = "https://github.com/repo-helper/pyproject-examples"
 
 [tool.importcheck]
 always = [ "pyproject_examples.example_configs", "pyproject_examples", "pyproject_examples.utils",]
 
 [tool.whey]
 base-classifiers = [ "Typing :: Typed",]
-python-versions = [ "3.6",]
+python-versions = [ "3.8",]
 python-implementations = [ "CPython",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "pyproject_examples"
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
```

### Comparing `pyproject_examples-2022.5.3/README.rst` & `pyproject_examples-2023.6.30/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 	:target: https://github.com/repo-helper/pyproject-examples/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/pyproject-examples/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/pyproject-examples/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-examples/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-examples/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-examples/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-examples/
 	:alt: Requirements Status
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/pyproject-examples?logo=codefactor
 	:target: https://www.codefactor.io/repository/github/repo-helper/pyproject-examples
 	:alt: CodeFactor Grade
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/pyproject-examples
@@ -77,23 +77,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-examples
 	:target: https://github.com/repo-helper/pyproject-examples/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-examples
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-examples/v2022.5.3
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-examples/v2023.6.30
 	:target: https://github.com/repo-helper/pyproject-examples/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-examples
 	:target: https://github.com/repo-helper/pyproject-examples/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pyproject-examples
 	:target: https://pypi.org/project/pyproject-examples/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `pyproject_examples-2022.5.3/LICENSE` & `pyproject_examples-2023.6.30/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_examples-2022.5.3/pyproject_examples/example_configs.py` & `pyproject_examples-2023.6.30/pyproject_examples/example_configs.py`

 * *Files identical despite different names*

### Comparing `pyproject_examples-2022.5.3/pyproject_examples/utils.py` & `pyproject_examples-2023.6.30/pyproject_examples/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_examples-2022.5.3/pyproject_examples/__init__.py` & `pyproject_examples-2023.6.30/pyproject_examples/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,19 +23,23 @@
 #  MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 import re
+import sys
 
 # 3rd party
 import pytest as pytest
 from coincidence.selectors import not_windows, only_windows
 from dom_toml.parser import BadConfigError
+from packaging.requirements import InvalidRequirement
+from packaging.specifiers import InvalidSpecifier
+from packaging.version import InvalidVersion
 
 # this package
 from pyproject_examples.example_configs import (
 		AUTHORS,
 		CLASSIFIERS,
 		COMPLETE_A,
 		COMPLETE_B,
@@ -51,15 +55,15 @@
 		URLS
 		)
 from pyproject_examples.utils import file_not_found_regex
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "2022.5.3"
+__version__: str = "2023.6.30"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = [
 		"valid_pep621_config",
 		"bad_pep621_config",
 		"valid_buildsystem_config",
 		"bad_buildsystem_config",
@@ -103,26 +107,26 @@
 				BadConfigError,
 				"The 'project.name' field may not be dynamic.",
 				id="dynamic_name"
 				),
 		pytest.param(
 				'[project]\nname = "???????12345=============☃"\nversion = "2020.0.0"',
 				BadConfigError,
-				"The value for 'project.name' is invalid.",
+				re.escape("The value '???????12345=============☃' for 'project.name' is invalid."),
 				id="bad_name"
 				),
 		pytest.param(
 				'[project]\nname = "spam"\nversion = "???????12345=============☃"',
-				BadConfigError,
+				InvalidVersion,
 				re.escape("Invalid version: '???????12345=============☃'"),
 				id="bad_version"
 				),
 		pytest.param(
 				f'{MINIMAL_CONFIG}\nrequires-python = "???????12345=============☃"',
-				BadConfigError,
+				InvalidSpecifier,
 				re.escape("Invalid specifier: '???????12345=============☃'"),
 				id="bad_requires_python"
 				),
 		pytest.param(
 				f'{MINIMAL_CONFIG}\nauthors = [{{name = "Bob, Alice"}}]',
 				BadConfigError,
 				r"The 'project.authors\[0\].name' key cannot contain commas.",
@@ -149,14 +153,28 @@
 		pytest.param(
 				f'{MINIMAL_CONFIG}\ndependencies = [1, 2, 3, 4, 5]',
 				TypeError,
 				r"Invalid type for 'project.dependencies\[0\]': expected <class 'str'>, got <class 'int'>",
 				id="dependencies_wrong_type"
 				),
 		pytest.param(
+				f'{MINIMAL_CONFIG}\ndependencies = ["foo]]]"]',
+				InvalidRequirement,
+				r"'foo]]]'\n    Expected end or semicolon \(after name and no valid version specifier\)\n    foo]]]\n       \^",
+				id="dependencies_invalid_requirement",
+				marks=pytest.mark.skipif(sys.version_info < (3, 7), reason="Error differs on 3.6"),
+				),
+		pytest.param(
+				f'{MINIMAL_CONFIG}\ndependencies = ["foo]]]"]',
+				InvalidRequirement,
+				r"'foo]]]'\n    Parse error at \"']]]'\": Expected string_end",
+				id="dependencies_invalid_requirement",
+				marks=pytest.mark.skipif(sys.version_info >= (3, 7), reason="Error differs on 3.6"),
+				),
+		pytest.param(
 				f'{MINIMAL_CONFIG}\nreadme = "README.rst"',
 				FileNotFoundError,
 				r"No such file or directory: ((Windows|Posix)Path(Plus)?\('README.rst'\)|'README.rst')",
 				id="missing_readme_file",
 				marks=not_windows("Message differs on Windows.")
 				),
 		pytest.param(
@@ -219,14 +237,28 @@
 		pytest.param(
 				'[build-system]\nrequires = "whey"',
 				TypeError,
 				"Invalid type for 'build-system.requires': expected <class 'collections.abc.Sequence'>, got <class 'str'>",
 				id="requires_str"
 				),
 		pytest.param(
+				'[build-system]\nrequires = ["foo]]]"]',
+				InvalidRequirement,
+				r"'foo]]]'\n    Expected end or semicolon \(after name and no valid version specifier\)\n    foo]]]\n       \^",
+				id="requires_invalid_requirement",
+				marks=pytest.mark.skipif(sys.version_info < (3, 7), reason="Error differs on 3.6"),
+				),
+		pytest.param(
+				'[build-system]\nrequires = ["foo]]]"]',
+				InvalidRequirement,
+				r"'foo]]]'\n    Parse error at \"']]]'\": Expected string_end",
+				id="requires_invalid_requirement",
+				marks=pytest.mark.skipif(sys.version_info >= (3, 7), reason="Error differs on 3.6"),
+				),
+		pytest.param(
 				'[build-system]\nrequires = ["whey"]\nbackend-path = [1234]',
 				TypeError,
 				r"Invalid type for 'build-system.backend-path\[0\]': expected <class 'str'>, got <class 'int'>",
 				id="backend_path_list_int"
 				),
 		pytest.param(
 				'[build-system]\nrequires = ["whey"]\nbackend-path = "whey"',
```

