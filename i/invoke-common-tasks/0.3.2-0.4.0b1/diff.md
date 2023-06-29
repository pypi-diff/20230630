# Comparing `tmp/invoke-common-tasks-0.3.2.tar.gz` & `tmp/invoke_common_tasks-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoke-common-tasks-0.3.2.tar", max compression
+gzip compressed data, was "invoke_common_tasks-0.4.0b1.tar", max compression
```

## Comparing `invoke-common-tasks-0.3.2.tar` & `invoke_common_tasks-0.4.0b1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1066 2022-04-19 04:33:06.776827 invoke-common-tasks-0.3.2/LICENSE
--rw-r--r--   0        0        0     7151 2022-04-19 04:33:06.776827 invoke-common-tasks-0.3.2/README.md
--rw-r--r--   0        0        0       70 2022-04-19 04:33:06.776827 invoke-common-tasks-0.3.2/invoke_common_tasks/__init__.py
--rw-r--r--   0        0        0     2060 2022-04-19 04:33:06.776827 invoke-common-tasks-0.3.2/invoke_common_tasks/tasks.py
--rw-r--r--   0        0        0        0 2022-04-19 04:33:06.776827 invoke-common-tasks-0.3.2/invoke_common_tasks/utils/__init__.py
--rw-r--r--   0        0        0     2831 2022-04-19 04:33:06.776827 invoke-common-tasks-0.3.2/invoke_common_tasks/utils/config.py
--rw-r--r--   0        0        0     1076 2022-04-19 04:33:06.776827 invoke-common-tasks-0.3.2/invoke_common_tasks/utils/git.py
--rw-r--r--   0        0        0     3107 2022-04-19 04:33:06.776827 invoke-common-tasks-0.3.2/invoke_common_tasks/utils/poetry.py
--rw-r--r--   0        0        0     1885 2022-04-19 04:33:06.776827 invoke-common-tasks-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8882 2022-04-19 04:33:31.298002 invoke-common-tasks-0.3.2/setup.py
--rw-r--r--   0        0        0     8693 2022-04-19 04:33:31.298592 invoke-common-tasks-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-29 23:50:27.240476 invoke_common_tasks-0.4.0b1/LICENSE
+-rw-r--r--   0        0        0     8041 2023-06-29 23:50:27.240476 invoke_common_tasks-0.4.0b1/README.md
+-rw-r--r--   0        0        0       70 2023-06-29 23:50:27.240476 invoke_common_tasks-0.4.0b1/invoke_common_tasks/__init__.py
+-rw-r--r--   0        0        0     2040 2023-06-29 23:50:27.240476 invoke_common_tasks-0.4.0b1/invoke_common_tasks/tasks.py
+-rw-r--r--   0        0        0        0 2023-06-29 23:50:27.240476 invoke_common_tasks-0.4.0b1/invoke_common_tasks/utils/__init__.py
+-rw-r--r--   0        0        0     2891 2023-06-29 23:50:27.240476 invoke_common_tasks-0.4.0b1/invoke_common_tasks/utils/config.py
+-rw-r--r--   0        0        0     1073 2023-06-29 23:50:27.240476 invoke_common_tasks-0.4.0b1/invoke_common_tasks/utils/git.py
+-rw-r--r--   0        0        0     3460 2023-06-29 23:50:27.240476 invoke_common_tasks-0.4.0b1/invoke_common_tasks/utils/poetry.py
+-rw-r--r--   0        0        0     1982 2023-06-29 23:50:27.240476 invoke_common_tasks-0.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0     9685 1970-01-01 00:00:00.000000 invoke_common_tasks-0.4.0b1/PKG-INFO
```

### Comparing `invoke-common-tasks-0.3.2/LICENSE` & `invoke_common_tasks-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `invoke-common-tasks-0.3.2/README.md` & `invoke_common_tasks-0.4.0b1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,45 @@
 # Invoke Common Tasks
 
 Some common tasks for PyInvoke to bootstrap your code quality and testing workflows.
 
+<!--TOC-->
+
+- [Invoke Common Tasks](#invoke-common-tasks)
+  - [Getting Started](#getting-started)
+    - [Invoke Setup](#invoke-setup)
+  - [The Tasks](#the-tasks)
+    - [build](#build)
+    - [format](#format)
+    - [lint](#lint)
+    - [typecheck](#typecheck)
+    - [test (and coverage)](#test-and-coverage)
+    - [ci](#ci)
+    - [init-config](#init-config)
+  - [TODO](#todo)
+  - [Roadmap](#roadmap)
+  - [All Together](#all-together)
+- [Contributing](#contributing)
+- [Development](#development)
+- [Resources](#resources)
+- [Prior Art](#prior-art)
+
+<!--TOC-->
 
 ## Getting Started
 
 ```sh
 pip install invoke-common-tasks
 # Or
 poetry add -D invoke-common-tasks
 
 # With Extras
 pip install invoke-common-tasks[all]
 # Or
-poetry add -D invoke-common-tasks[all]
+poetry add --group dev invoke-common-tasks[all]
 ```
 
 `invoke-common-tasks` defines a few _extras_, where you can also install the tooling to go with each task.
 By default we **do not** install the tools that these tasks call, since you could have different pinned versions than what we specify.
 
 However, you can install `all` of them or distinct subsets:
 
@@ -199,18 +221,20 @@
 Options:
   -a, --all
   -f, --format
   -l, --lint
   -t, --test
   -y, --typecheck
 ```
+
 ## TODO
 
- - Auto-initialisations of some default config. 
-    - eg `invoke format --init` should set config if not present
+ - Add task for auto generation of Sphinx Docs.
+ - Add typechecking support to root `tasks.py` file now that Invoke v2+ is released.
+
 
 
 ## Roadmap
 
 This project will get marked as a stable v1.0 once the above TODO features are ticked off and this has seen at least 6 months in the wild in production.
 
 
@@ -249,14 +273,24 @@
 
 However if you would like to contribute your changes back, then open a Pull Request "across forks".
 
 Once your changes are merged and published you can revert to the canonical version of `pip install`ing this package.
 
 If you're not sure how to make changes or if you should sink the time and effort, then open an Issue instead and we can have a chat to triage the issue.
 
+# Development
+
+```sh
+git clone https://github.com/neozenith/invoke-common-tasks
+cd invoke-common-tasks
+poetry shell
+# This will not install the dev dependencies which are optional when a consumer uses the project but are actually needed for development of this library
+poetry install --all-extras
+```
+
 
 # Resources
 
  - [`pyinvoke`](https://pyinvoke.org)
 
 # Prior Art
```

### Comparing `invoke-common-tasks-0.3.2/invoke_common_tasks/tasks.py` & `invoke_common_tasks-0.4.0b1/invoke_common_tasks/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .utils.config import (
     add_format_config,
     add_test_config,
     add_typecheck_config,
     write_lint_config,
 )
-from .utils.poetry import poetry_project
+from .utils.poetry import poetry_pyprojecttoml
 
 # NOTE: Invoke tasks files don't support mypy typechecking for the forseeable future
 # They were looking at addressing it after Python2 EOL 01-01-2020 but there was a global pandemic.
 # https://github.com/pyinvoke/invoke/issues/357
 
 
 @task
@@ -68,16 +68,15 @@
 
     print("Initialise config options selected:")
     print(f"format:    {format}")
     print(f"lint:      {lint}")
     print(f"typecheck: {typecheck}")
     print(f"test:      {test}")
 
-    project = poetry_project()
-    pyproject = project.pyproject
+    pyproject = poetry_pyprojecttoml()
 
     if format:
         print("Adding format config...")
         add_format_config(pyproject)
 
     if lint:
         print("Adding linting config...")
```

### Comparing `invoke-common-tasks-0.3.2/invoke_common_tasks/utils/config.py` & `invoke_common_tasks-0.4.0b1/invoke_common_tasks/utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Third Party
-from poetry.core._vendor.tomlkit import table
-from poetry.core.pyproject.toml import PyProjectTOML
+from poetry.pyproject.toml import PyProjectTOML
+from tomlkit.api import table
+from tomlkit.items import Table
 
 FLAKE8 = """[flake8]
 exclude =
     venv,
     dist,
     .venv
 select = ANN,B,B9,BLK,C,D,DAR,E,F,I,S,W
@@ -24,34 +25,34 @@
         f.write(FLAKE8)
 
 
 def add_format_config(pyproject: PyProjectTOML) -> None:
     """Augment pyproject.toml in memory with default formatting config."""
     tools = pyproject.data["tool"]
     if "black" not in tools:
-        black_table = table()
+        black_table: Table = table()
         black_table["line-length"] = 120
         tools["black"] = black_table
 
     if "isort" not in tools:
-        isort_table = table()
+        isort_table: Table = table()
         isort_table["profile"] = "black"
         isort_table["multi_line_output"] = 3
         isort_table["import_heading_stdlib"] = "Standard Library"
         isort_table["import_heading_firstparty"] = "Our Libraries"
         isort_table["import_heading_thirdparty"] = "Third Party"
         tools["isort"] = isort_table
 
 
 def add_typecheck_config(pyproject: PyProjectTOML) -> None:
     """Augment pyproject.toml in memory with default typechecking config."""
     tools = pyproject.data["tool"]
 
     if "mypy" not in tools:
-        mypy_table = table()
+        mypy_table: Table = table()
         mypy_table["exclude"] = ["tests/", "tasks\.py"]  # noqa
         mypy_table["pretty"] = True
         mypy_table["show_error_codes"] = True
         mypy_table["show_column_numbers"] = True
         mypy_table["show_error_context"] = True
         mypy_table["ignore_missing_imports"] = True
         mypy_table["follow_imports"] = "silent"
@@ -61,24 +62,24 @@
         tools["mypy"] = mypy_table
 
 
 def add_test_config(pyproject: PyProjectTOML) -> None:
     """Augment pyproject.toml in memory with default test config."""
     tools = pyproject.data["tool"]
     if "pytest" not in tools:
-        ini_options = table()
+        ini_options: Table = table()
         ini_options["minversion"] = "6.0"
         ini_options["addopts"] = "-s -vvv --color=yes --cov=. --no-cov-on-fail"
 
-        pytest_table = table()
+        pytest_table: Table = table()
         # TODO: For some reason nested tables are adding the intermediate table heading
         pytest_table["ini_options"] = ini_options
         tools["pytest"] = pytest_table
 
     if "coverage" not in tools:
-        run_table = table()
+        run_table: Table = table()
         run_table["branch"] = True
         run_table["omit"] = ["tests/*", "**/__init__.py", "tasks.py"]
 
-        coverage_table = table()
+        coverage_table: Table = table()
         coverage_table["run"] = run_table
         tools["coverage"] = coverage_table
```

### Comparing `invoke-common-tasks-0.3.2/invoke_common_tasks/utils/git.py` & `invoke_common_tasks-0.4.0b1/invoke_common_tasks/utils/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
     # When using Jenkins or other CI systems, if they checkout a commit hash it is in a detached HEAD state
     # So no branch name will resolve even if there is a branch name associated with that commit hash.
     # So if the above returns the default "HEAD", then we resort to the short hash as a meaningful pointer.
     # https://stackoverflow.com/questions/6245570/how-to-get-the-current-branch-name-in-git#comment50696859_11868440
     if branch_name == "HEAD":
         branch_name = run("git rev-parse --short HEAD", hide=True).stdout.strip()
-    
-    return branch_name
+
+    return branch_name
```

### Comparing `invoke-common-tasks-0.3.2/invoke_common_tasks/utils/poetry.py` & `invoke_common_tasks-0.4.0b1/invoke_common_tasks/utils/poetry.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,35 @@
 from subprocess import run
 from typing import List, Optional
 
 # Third Party
 from poetry.core.factory import Factory
 from poetry.core.masonry.builders.wheel import WheelBuilder
 from poetry.core.poetry import Poetry
+from poetry.pyproject.toml import PyProjectTOML
 
 
 @lru_cache(maxsize=None)
 def poetry_project(path: str = ".") -> Poetry:
     """Get an instance of the current Poetry project.
 
     This is cached so that subsequent calls in the same invoke session reduce interactions with disk.
     """
     poetry = Factory().create_poetry(Path(path).resolve())
     return poetry
 
 
 @lru_cache(maxsize=None)
+def poetry_pyprojecttoml(path: str = ".") -> PyProjectTOML:
+    """Create a writable instance of a PyProjectTOML since the poetry.core API treats it as read-only."""
+    pyproject_toml_filepath = poetry_project().pyproject_path
+    return PyProjectTOML(pyproject_toml_filepath)
+
+
+@lru_cache(maxsize=None)
 def poetry_project_name(path: str = ".") -> str:
     """Get the name of the current Poerty project."""
     return str(poetry_project(path).pyproject.poetry_config["name"])
 
 
 @lru_cache(maxsize=None)
 def poetry_project_version(path: str = ".") -> str:
```

### Comparing `invoke-common-tasks-0.3.2/pyproject.toml` & `invoke_common_tasks-0.4.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 [tool.poetry]
 name = "invoke-common-tasks"
-version = "0.3.2"
+version = "0.4.0-b1"
 description = "Some common tasks for PyInvoke to bootstrap your code quality and testing workflows."
 authors = ["Josh Peak <neozenith.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/neozenith/invoke-common-tasks"
 repository = "https://github.com/neozenith/invoke-common-tasks"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-invoke = "^1.6.0"
-types-invoke = "^1.6.2"
-poetry-core = "^1.0.8"
+invoke = ">=2.0.0,<=3.0.0"
+types-invoke = ">=2.0.0,<=3.0.0"
+poetry-core = "^1.6.0"
 black = {version = "^22.1.0", optional = true}
 isort = {version = "^5.10.1", optional = true}
 flake8 = {version = "^4.0.1", optional = true}
 flake8-docstrings = {version = "^1.6.0", optional = true}
 mypy = {version = "^0.942", optional = true}
 pytest = {version = "^7.1.1", optional = true}
 pytest-cov = {version = "^3.0.0", optional = true}
 coverage = {extras = ["toml"], version = "^6.3.2", optional = true}
+poetry = "^1.5.1"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 format = ["black", "isort"]
 lint = ["flake8", "flake8-docstrings"]
 typecheck = ["mypy"]
 test = ["pytest", "pytest-cov", "coverage"]
 all = ["black", "isort", "flake8", "flake8-docstrings", "mypy", "pytest", "pytest-cov", "coverage"]
 
+
+
+
+[tool.poetry.group.dev.dependencies]
+md-toc = "^8.1.9"
+
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 import_heading_stdlib = "Standard Library"
@@ -55,12 +62,11 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-s -vvv --color=yes --cov=. --no-cov-on-fail"
 
 [tool.coverage.run]
 branch = true
 omit = ["tests/*", "**/__init__.py", "tasks.py"]
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `invoke-common-tasks-0.3.2/setup.py` & `invoke_common_tasks-0.4.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,336 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: invoke-common-tasks
+Version: 0.4.0b1
+Summary: Some common tasks for PyInvoke to bootstrap your code quality and testing workflows.
+Home-page: https://github.com/neozenith/invoke-common-tasks
+License: MIT
+Author: Josh Peak
+Author-email: neozenith.dev@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: format
+Provides-Extra: lint
+Provides-Extra: test
+Provides-Extra: typecheck
+Requires-Dist: black (>=22.1.0,<23.0.0) ; extra == "format" or extra == "all"
+Requires-Dist: coverage[toml] (>=6.3.2,<7.0.0) ; extra == "test" or extra == "all"
+Requires-Dist: flake8 (>=4.0.1,<5.0.0) ; extra == "lint" or extra == "all"
+Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "lint" or extra == "all"
+Requires-Dist: invoke (>=2.0.0,<=3.0.0)
+Requires-Dist: isort (>=5.10.1,<6.0.0) ; extra == "format" or extra == "all"
+Requires-Dist: mypy (>=0.942,<0.943) ; extra == "typecheck" or extra == "all"
+Requires-Dist: poetry (>=1.5.1,<2.0.0)
+Requires-Dist: poetry-core (>=1.6.0,<2.0.0)
+Requires-Dist: pytest (>=7.1.1,<8.0.0) ; extra == "test" or extra == "all"
+Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test" or extra == "all"
+Requires-Dist: types-invoke (>=2.0.0,<=3.0.0)
+Project-URL: Repository, https://github.com/neozenith/invoke-common-tasks
+Description-Content-Type: text/markdown
 
-packages = \
-['invoke_common_tasks', 'invoke_common_tasks.utils']
+# Invoke Common Tasks
 
-package_data = \
-{'': ['*']}
+Some common tasks for PyInvoke to bootstrap your code quality and testing workflows.
 
-install_requires = \
-['invoke>=1.6.0,<2.0.0',
- 'poetry-core>=1.0.8,<2.0.0',
- 'types-invoke>=1.6.2,<2.0.0']
-
-extras_require = \
-{'all': ['black>=22.1.0,<23.0.0',
-         'isort>=5.10.1,<6.0.0',
-         'flake8>=4.0.1,<5.0.0',
-         'flake8-docstrings>=1.6.0,<2.0.0',
-         'mypy>=0.942,<0.943',
-         'pytest>=7.1.1,<8.0.0',
-         'pytest-cov>=3.0.0,<4.0.0',
-         'coverage[toml]>=6.3.2,<7.0.0'],
- 'format': ['black>=22.1.0,<23.0.0', 'isort>=5.10.1,<6.0.0'],
- 'lint': ['flake8>=4.0.1,<5.0.0', 'flake8-docstrings>=1.6.0,<2.0.0'],
- 'test': ['pytest>=7.1.1,<8.0.0',
-          'pytest-cov>=3.0.0,<4.0.0',
-          'coverage[toml]>=6.3.2,<7.0.0'],
- 'typecheck': ['mypy>=0.942,<0.943']}
-
-setup_kwargs = {
-    'name': 'invoke-common-tasks',
-    'version': '0.3.2',
-    'description': 'Some common tasks for PyInvoke to bootstrap your code quality and testing workflows.',
-    'long_description': '# Invoke Common Tasks\n\nSome common tasks for PyInvoke to bootstrap your code quality and testing workflows.\n\n\n## Getting Started\n\n```sh\npip install invoke-common-tasks\n# Or\npoetry add -D invoke-common-tasks\n\n# With Extras\npip install invoke-common-tasks[all]\n# Or\npoetry add -D invoke-common-tasks[all]\n```\n\n`invoke-common-tasks` defines a few _extras_, where you can also install the tooling to go with each task.\nBy default we **do not** install the tools that these tasks call, since you could have different pinned versions than what we specify.\n\nHowever, you can install `all` of them or distinct subsets:\n\n - **format** -> `black`, `isort`\n - **lint** -> `flake8`, `flake8-docstrings`\n - **typecheck** -> `mypy`\n - **test** -> `pytest`, `pytest-cov`, `coverage[toml]`\n\nSo you can specify the following if you only want `format` and `test`:\n\n```sh\npip install invoke-common-tasks[format,test]\n```\n\nAll _tasks_ will still be available but we won\'t install associated tooling.\n\n### Invoke Setup\n\n`tasks.py`\n\n```python\nfrom invoke_common_tasks import * # noqa\n```\n\nOnce your `tasks.py` is setup like this `invoke` will have the extra commands:\n\n```sh\nλ invoke --list\nAvailable tasks:\n\n  build         Build wheel.\n  ci            Run linting and test suite for Continuous Integration.\n  format        Autoformat code for code style.\n  init-config   Setup default configuration for development tooling.\n  lint          Linting and style checking.\n  test          Run test suite.\n  typecheck     Run typechecking tooling.\n```\n\nYou can also initialise default configuration for each tool by running the following:\n\n```sh\ninvoke init-config --all\n```\n\nMore details in the [init-config](#init-config) section.\n\n## The Tasks\n\n### build\n\nAssuming you are using `poetry` this will build a wheel (and only a wheel).\n\n### format\n\nThis will apply code formatting tools `black` and `isort`.\n\nThese are only triggers for these commands, the specifics of configuration are up to you.\n\nRecommended configuration in your `pyproject.toml`:\n\n```toml\n[tool.black]\nline-length = 120\n\n[tool.isort]\nprofile = "black"\nmulti_line_output = 3\nimport_heading_stdlib = "Standard Library"\nimport_heading_firstparty = "Our Libraries"\nimport_heading_thirdparty = "Third Party"\n```\n\n### lint\n\nThis will run checks for `black`, `isort` and `flake8`.\n\nUp to you to specify your preferences of plugins for `flake8` and its configuration.\n\nRecommended configuration in `.flake8`:\n\n```ini\n[flake8]\nexclude = \n    venv,\n    dist,\n    .venv\nselect = ANN,B,B9,BLK,C,D,DAR,E,F,I,S,W\nignore = E203,E501,W503,D100,D104\nper-file-ignores =\n    tests/*: D103,S101\nmax-line-length = 120\nmax-complexity = 10\nimport-order-style = google\ndocstring-convention = google\n```\n\nRecommended `flake8` plugins:\n - [`flake8-docstrings`](https://pypi.org/project/flake8-docstrings/)\n\nMore `flake8` plugins:\n\nhttps://github.com/DmytroLitvinov/awesome-flake8-extensions\n\n### typecheck\n\nSimply runs `mypy .`.\n\nRecommended configuration to add to your `pyproject.toml`\n\n```toml\n[tool.mypy]\npretty = true\nshow_error_codes = true\nshow_column_numbers = true\nshow_error_context = true\nexclude = [\n  \'tests/\',\n  \'tasks\\.py\'\n]\nfollow_imports = \'silent\'\nignore_missing_imports = true\n\n# Work your way up to these:\ndisallow_incomplete_defs = true\n# disallow_untyped_defs = true \n# disallow-untyped-calls = true\n# strict = true\n```\n\n### test (and coverage)\n\nThis will simply run `python3 -m pytest`. This is important to run as a module instead of `pytest` since it resolves\na lot of import issues.\n\nYou can simply not import this task if you prefer something else. But all config and plugins are left flexible for your own desires, this simply triggers the entrypoint.\n\nRecommended configuration in `pyproject.toml`:\n\n```toml\n[tool.pytest.ini_options]\nminversion = "6.0"\naddopts = "-s -vvv --color=yes --cov=. --no-cov-on-fail"\n\n[tool.coverage.run]\nomit = ["tests/*", "**/__init__.py", "tasks.py"]\nbranch = true\n```\n\nAssuming you also install `pytest-cov` and `coverage[toml]`.\n\nRecommended `pytest` plugins:\n - [`pytest-xdist`](https://pypi.org/project/pytest-xdist/) - Run tests in parallel using maximum cpu cores \n - [`pytest-randomly`](https://pypi.org/project/pytest-randomly/) - Run tests in random order each time to detect tests with unintentional dependencies to each other that should be isolated. Each run prints out the seed if you need to reproduce an exact seeded run.\n - [`pytest-cov`](https://pypi.org/project/pytest-cov/) - It is recommended to run coverage from the `pytest` plugin.\n \nList of other `pytest` plugins:\n\nhttps://docs.pytest.org/en/latest/reference/plugin_list.html\n\n### ci\n\nThis is a task with no commands but chains together `lint`, `typecheck` and `test`. \n\n### init-config\n\n> Experimental: This feature is still in a pre-release state.\n\nEach of the above commands came with some recommended configuration.\nThis command attempts to automate setting up even that part in your `pyproject.toml` and `.flake8` files.\n\n```sh\nλ invoke init-config --help\nUsage: inv[oke] [--core-opts] init-config [--options] [other tasks here ...]\n\nDocstring:\n  Setup default configuration for development tooling.\n\nOptions:\n  -a, --all\n  -f, --format\n  -l, --lint\n  -t, --test\n  -y, --typecheck\n```\n## TODO\n\n - Auto-initialisations of some default config. \n    - eg `invoke format --init` should set config if not present\n\n\n## Roadmap\n\nThis project will get marked as a stable v1.0 once the above TODO features are ticked off and this has seen at least 6 months in the wild in production.\n\n\n## All Together\n\nOnce all the tasks are imported, you can create a custom task as your default task with runs a few tasks chained together.\n\n```python\nfrom invoke import task\nfrom invoke_common_tasks import *\n\n@task(pre=[format, lint, typecheck, test], default=True)\ndef all(c):\n  """Default development loop."""\n  ...\n```\n\nYou will notice a few things here:\n\n1. The method has no implementation `...`\n1. We are chaining a series of `@task`s in the `pre=[...]` argument\n1. The `default=True` on this root tasks means we could run either `invoke all` or simply `invoke`.\n\nHow cool is that?\n\n# Contributing\n\nAt all times, you have the power to fork this project, make changes as you see fit and then:\n\n```sh\npip install https://github.com/user/repository/archive/branch.zip\n```\n[Stackoverflow: pip install from github branch](https://stackoverflow.com/a/24811490/622276)\n\nThat way you can run from your own custom fork in the interim or even in-house your work and simply use this project as a starting point. That is totally ok.\n\nHowever if you would like to contribute your changes back, then open a Pull Request "across forks".\n\nOnce your changes are merged and published you can revert to the canonical version of `pip install`ing this package.\n\nIf you\'re not sure how to make changes or if you should sink the time and effort, then open an Issue instead and we can have a chat to triage the issue.\n\n\n# Resources\n\n - [`pyinvoke`](https://pyinvoke.org)\n\n# Prior Art\n\n - https://github.com/Smile-SA/invoke-sphinx\n - https://github.com/Dashlane/dbt-invoke\n - https://invocations.readthedocs.io/en/latest/index.html\n\n',
-    'author': 'Josh Peak',
-    'author_email': 'neozenith.dev@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/neozenith/invoke-common-tasks',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
+<!--TOC-->
+
+- [Invoke Common Tasks](#invoke-common-tasks)
+  - [Getting Started](#getting-started)
+    - [Invoke Setup](#invoke-setup)
+  - [The Tasks](#the-tasks)
+    - [build](#build)
+    - [format](#format)
+    - [lint](#lint)
+    - [typecheck](#typecheck)
+    - [test (and coverage)](#test-and-coverage)
+    - [ci](#ci)
+    - [init-config](#init-config)
+  - [TODO](#todo)
+  - [Roadmap](#roadmap)
+  - [All Together](#all-together)
+- [Contributing](#contributing)
+- [Development](#development)
+- [Resources](#resources)
+- [Prior Art](#prior-art)
+
+<!--TOC-->
+
+## Getting Started
+
+```sh
+pip install invoke-common-tasks
+# Or
+poetry add -D invoke-common-tasks
+
+# With Extras
+pip install invoke-common-tasks[all]
+# Or
+poetry add --group dev invoke-common-tasks[all]
+```
+
+`invoke-common-tasks` defines a few _extras_, where you can also install the tooling to go with each task.
+By default we **do not** install the tools that these tasks call, since you could have different pinned versions than what we specify.
+
+However, you can install `all` of them or distinct subsets:
+
+ - **format** -> `black`, `isort`
+ - **lint** -> `flake8`, `flake8-docstrings`
+ - **typecheck** -> `mypy`
+ - **test** -> `pytest`, `pytest-cov`, `coverage[toml]`
+
+So you can specify the following if you only want `format` and `test`:
+
+```sh
+pip install invoke-common-tasks[format,test]
+```
+
+All _tasks_ will still be available but we won't install associated tooling.
+
+### Invoke Setup
+
+`tasks.py`
+
+```python
+from invoke_common_tasks import * # noqa
+```
+
+Once your `tasks.py` is setup like this `invoke` will have the extra commands:
+
+```sh
+λ invoke --list
+Available tasks:
+
+  build         Build wheel.
+  ci            Run linting and test suite for Continuous Integration.
+  format        Autoformat code for code style.
+  init-config   Setup default configuration for development tooling.
+  lint          Linting and style checking.
+  test          Run test suite.
+  typecheck     Run typechecking tooling.
+```
+
+You can also initialise default configuration for each tool by running the following:
+
+```sh
+invoke init-config --all
+```
+
+More details in the [init-config](#init-config) section.
+
+## The Tasks
+
+### build
+
+Assuming you are using `poetry` this will build a wheel (and only a wheel).
+
+### format
+
+This will apply code formatting tools `black` and `isort`.
+
+These are only triggers for these commands, the specifics of configuration are up to you.
+
+Recommended configuration in your `pyproject.toml`:
+
+```toml
+[tool.black]
+line-length = 120
+
+[tool.isort]
+profile = "black"
+multi_line_output = 3
+import_heading_stdlib = "Standard Library"
+import_heading_firstparty = "Our Libraries"
+import_heading_thirdparty = "Third Party"
+```
+
+### lint
+
+This will run checks for `black`, `isort` and `flake8`.
+
+Up to you to specify your preferences of plugins for `flake8` and its configuration.
+
+Recommended configuration in `.flake8`:
+
+```ini
+[flake8]
+exclude = 
+    venv,
+    dist,
+    .venv
+select = ANN,B,B9,BLK,C,D,DAR,E,F,I,S,W
+ignore = E203,E501,W503,D100,D104
+per-file-ignores =
+    tests/*: D103,S101
+max-line-length = 120
+max-complexity = 10
+import-order-style = google
+docstring-convention = google
+```
+
+Recommended `flake8` plugins:
+ - [`flake8-docstrings`](https://pypi.org/project/flake8-docstrings/)
+
+More `flake8` plugins:
+
+https://github.com/DmytroLitvinov/awesome-flake8-extensions
+
+### typecheck
+
+Simply runs `mypy .`.
+
+Recommended configuration to add to your `pyproject.toml`
+
+```toml
+[tool.mypy]
+pretty = true
+show_error_codes = true
+show_column_numbers = true
+show_error_context = true
+exclude = [
+  'tests/',
+  'tasks\.py'
+]
+follow_imports = 'silent'
+ignore_missing_imports = true
+
+# Work your way up to these:
+disallow_incomplete_defs = true
+# disallow_untyped_defs = true 
+# disallow-untyped-calls = true
+# strict = true
+```
+
+### test (and coverage)
+
+This will simply run `python3 -m pytest`. This is important to run as a module instead of `pytest` since it resolves
+a lot of import issues.
+
+You can simply not import this task if you prefer something else. But all config and plugins are left flexible for your own desires, this simply triggers the entrypoint.
+
+Recommended configuration in `pyproject.toml`:
+
+```toml
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-s -vvv --color=yes --cov=. --no-cov-on-fail"
+
+[tool.coverage.run]
+omit = ["tests/*", "**/__init__.py", "tasks.py"]
+branch = true
+```
+
+Assuming you also install `pytest-cov` and `coverage[toml]`.
+
+Recommended `pytest` plugins:
+ - [`pytest-xdist`](https://pypi.org/project/pytest-xdist/) - Run tests in parallel using maximum cpu cores 
+ - [`pytest-randomly`](https://pypi.org/project/pytest-randomly/) - Run tests in random order each time to detect tests with unintentional dependencies to each other that should be isolated. Each run prints out the seed if you need to reproduce an exact seeded run.
+ - [`pytest-cov`](https://pypi.org/project/pytest-cov/) - It is recommended to run coverage from the `pytest` plugin.
+ 
+List of other `pytest` plugins:
+
+https://docs.pytest.org/en/latest/reference/plugin_list.html
+
+### ci
+
+This is a task with no commands but chains together `lint`, `typecheck` and `test`. 
+
+### init-config
+
+> Experimental: This feature is still in a pre-release state.
+
+Each of the above commands came with some recommended configuration.
+This command attempts to automate setting up even that part in your `pyproject.toml` and `.flake8` files.
+
+```sh
+λ invoke init-config --help
+Usage: inv[oke] [--core-opts] init-config [--options] [other tasks here ...]
+
+Docstring:
+  Setup default configuration for development tooling.
+
+Options:
+  -a, --all
+  -f, --format
+  -l, --lint
+  -t, --test
+  -y, --typecheck
+```
+
+## TODO
+
+ - Add task for auto generation of Sphinx Docs.
+ - Add typechecking support to root `tasks.py` file now that Invoke v2+ is released.
+
+
+
+## Roadmap
+
+This project will get marked as a stable v1.0 once the above TODO features are ticked off and this has seen at least 6 months in the wild in production.
+
+
+## All Together
+
+Once all the tasks are imported, you can create a custom task as your default task with runs a few tasks chained together.
+
+```python
+from invoke import task
+from invoke_common_tasks import *
+
+@task(pre=[format, lint, typecheck, test], default=True)
+def all(c):
+  """Default development loop."""
+  ...
+```
+
+You will notice a few things here:
+
+1. The method has no implementation `...`
+1. We are chaining a series of `@task`s in the `pre=[...]` argument
+1. The `default=True` on this root tasks means we could run either `invoke all` or simply `invoke`.
+
+How cool is that?
+
+# Contributing
+
+At all times, you have the power to fork this project, make changes as you see fit and then:
+
+```sh
+pip install https://github.com/user/repository/archive/branch.zip
+```
+[Stackoverflow: pip install from github branch](https://stackoverflow.com/a/24811490/622276)
+
+That way you can run from your own custom fork in the interim or even in-house your work and simply use this project as a starting point. That is totally ok.
+
+However if you would like to contribute your changes back, then open a Pull Request "across forks".
+
+Once your changes are merged and published you can revert to the canonical version of `pip install`ing this package.
+
+If you're not sure how to make changes or if you should sink the time and effort, then open an Issue instead and we can have a chat to triage the issue.
+
+# Development
+
+```sh
+git clone https://github.com/neozenith/invoke-common-tasks
+cd invoke-common-tasks
+poetry shell
+# This will not install the dev dependencies which are optional when a consumer uses the project but are actually needed for development of this library
+poetry install --all-extras
+```
+
+
+# Resources
+
+ - [`pyinvoke`](https://pyinvoke.org)
+
+# Prior Art
+
+ - https://github.com/Smile-SA/invoke-sphinx
+ - https://github.com/Dashlane/dbt-invoke
+ - https://invocations.readthedocs.io/en/latest/index.html
 
 
-setup(**setup_kwargs)
```

