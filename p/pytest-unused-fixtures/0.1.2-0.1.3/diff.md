# Comparing `tmp/pytest_unused_fixtures-0.1.2.tar.gz` & `tmp/pytest_unused_fixtures-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_unused_fixtures-0.1.2.tar", max compression
+gzip compressed data, was "pytest_unused_fixtures-0.1.3.tar", max compression
```

## Comparing `pytest_unused_fixtures-0.1.2.tar` & `pytest_unused_fixtures-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-06-13 20:43:22.326631 pytest_unused_fixtures-0.1.2/LICENSE
--rw-r--r--   0        0        0     2165 2023-06-15 09:24:44.910899 pytest_unused_fixtures-0.1.2/README.md
--rw-r--r--   0        0        0     2800 2023-06-15 08:59:11.577729 pytest_unused_fixtures-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      153 2023-06-15 08:59:11.585729 pytest_unused_fixtures-0.1.2/pytest_unused_fixtures/__init__.py
--rw-r--r--   0        0        0       88 2023-06-14 21:25:32.009991 pytest_unused_fixtures-0.1.2/pytest_unused_fixtures/decorators.py
--rw-r--r--   0        0        0     1196 2023-06-14 15:58:39.977422 pytest_unused_fixtures-0.1.2/pytest_unused_fixtures/options.py
--rw-r--r--   0        0        0     4432 2023-06-15 09:23:47.202684 pytest_unused_fixtures-0.1.2/pytest_unused_fixtures/plugin.py
--rw-r--r--   0        0        0     1512 2023-06-14 15:58:39.858423 pytest_unused_fixtures-0.1.2/pytest_unused_fixtures/xdist.py
--rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 pytest_unused_fixtures-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-13 20:43:22.326631 pytest_unused_fixtures-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2233 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/README.md
+-rw-r--r--   0        0        0     2799 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-06-15 08:59:11.585729 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-14 21:25:32.009991 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/decorators.py
+-rw-r--r--   0        0        0     1226 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/options.py
+-rw-r--r--   0        0        0     4543 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/plugin.py
+-rw-r--r--   0        0        0     1529 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/xdist.py
+-rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pytest_unused_fixtures-0.1.3/PKG-INFO
```

### Comparing `pytest_unused_fixtures-0.1.2/LICENSE` & `pytest_unused_fixtures-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.2/README.md` & `pytest_unused_fixtures-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,19 @@
 Many thanks to
 
  - [pytest-deadfixtures](https://github.com/jllorencetti/pytest-deadfixtures) for inspiration for this project
  - [pytest-durations](https://github.com/blake-r/pytest-durations) for inspirations in parts of the implementation
 
 ## Changelog
 
+### 0.1.3 (Jun 30, 2023)
+
+* Print line number
+* Support Python 3.9
+
 ### 0.1.2 (Jun 15, 2023)
 
 * Fix typo, add repository to PyPI
 * Update location handling with respect to showing fixture locations and ignoring paths
 
 ### 0.1.1 (Jun 14, 2023)
```

### Comparing `pytest_unused_fixtures-0.1.2/pyproject.toml` & `pytest_unused_fixtures-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-unused-fixtures"
-version = "0.1.2"
+version = "0.1.3"
 description = "A pytest plugin to list unused fixtures after a test run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_unused_fixtures"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -22,15 +22,15 @@
 repository = "https://github.com/mikicz/pytest-unused-fixtures"
 keywords = ["pytest", "fixtures"]
 
 [tool.poetry.plugins."pytest11"]
 pytest-unused-fixtures = "pytest_unused_fixtures"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 pytest = "^7.3.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.272"
 pytest-xdist = "^3.3.1"
```

### Comparing `pytest_unused_fixtures-0.1.2/pytest_unused_fixtures/options.py` & `pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+from __future__ import annotations
+
 from typing import TYPE_CHECKING, NoReturn
 
 if TYPE_CHECKING:
     from _pytest.config import Config, PytestPluginManager
     from _pytest.config.argparsing import Parser
 
 
-def pytest_addoption(parser: "Parser", pluginmanager: "PytestPluginManager") -> NoReturn:
+def pytest_addoption(parser: Parser, pluginmanager: PytestPluginManager) -> NoReturn:
     group = parser.getgroup("pytest-unused-fixtures")
     group.addoption("--unused-fixtures", action="store_true", default=False, help="Try to identify unused fixtures.")
     group.addoption(
         "--unused-fixtures-ignore-path",
         metavar="PATH",
         type=str,
         default=None,
         action="append",
         help="Ignore fixtures in PATHs from unused fixtures report.",
     )
 
 
-def pytest_configure(config: "Config") -> NoReturn:
+def pytest_configure(config: Config) -> NoReturn:
     if not config.getoption("--unused-fixtures"):
         return
 
     from pytest_unused_fixtures.plugin import PytestUnusedFixturesPlugin
 
     pluginmanager = config.pluginmanager
```

### Comparing `pytest_unused_fixtures-0.1.2/pytest_unused_fixtures/plugin.py` & `pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import dataclasses
 import itertools
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, NoReturn
 
 import pytest
 from _pytest.compat import getlocation
@@ -15,14 +17,15 @@
 
 @dataclasses.dataclass(frozen=True, eq=True)
 class FixtureInfo:
     module: str
     argname: str
     scope: str
     location: str
+    lineno: int
 
     def __lt__(self, other):
         return (self.module, self.location, self.argname) < (other.module, other.location, other.argname)
 
     @property
     def location_path(self):
         return Path(self.location.split(":")[0]).resolve()
@@ -39,37 +42,38 @@
 class PytestUnusedFixturesPlugin:
     def __init__(self, ignore_paths: list[str | Path] | None = None):
         self.ignore_paths: list[Path] = [Path(x).resolve() for x in (ignore_paths or [])]
         self.used_fixtures: set[FixtureInfo] = set()
         self.available_fixtures: None | set[FixtureInfo] = None
         self.curdir = Path().cwd()
 
-    def get_fixture_info(self, fixturedef: "FixtureDef") -> FixtureInfo:
+    def get_fixture_info(self, fixturedef: FixtureDef) -> FixtureInfo:
         return FixtureInfo(
             module=fixturedef.func.__module__,
             argname=fixturedef.argname,
             scope=fixturedef.scope,
             location=getlocation(fixturedef.func, self.curdir),
+            lineno=fixturedef.func.__code__.co_firstlineno,
         )
 
     @pytest.hookimpl(hookwrapper=True)
-    def pytest_fixture_setup(self, fixturedef: "FixtureDef", request: "SubRequest") -> Any | None:
+    def pytest_fixture_setup(self, fixturedef: FixtureDef, request: SubRequest) -> Any | None:
         self.used_fixtures.add(self.get_fixture_info(fixturedef))
 
         yield
 
-    def pytest_collection_finish(self, session: "Session") -> None:
+    def pytest_collection_finish(self, session: Session) -> None:
         self.available_fixtures = {
             self.get_fixture_info(x)
             for x in itertools.chain(*session._fixturemanager._arg2fixturedefs.values())
             # if fixture is not in available fixtures, it won't be marked as unused
             if not hasattr(x.func, "ignore_unused_fixture")
         }
 
-    def _write_fixtures(self, config: "Config", terminalreporter: "TerminalReporter", fixtures: set[FixtureInfo]):
+    def _write_fixtures(self, config: Config, terminalreporter: TerminalReporter, fixtures: set[FixtureInfo]):
         verbose = config.getvalue("verbose")
         tw = terminalreporter
 
         available: list[FixtureInfo] = []
         seen: set[tuple[str, str]] = set()
 
         fixture: FixtureInfo
@@ -86,22 +90,22 @@
                 tw.write_sep("-", f"fixtures defined from {fixture.module}")
                 current_module = fixture.module
             if verbose <= 0 and fixture.argname.startswith("_"):
                 continue
             tw.write(f"{fixture.argname}", green=True)
             if fixture.scope != "function":
                 tw.write(" [%s scope]" % fixture.scope, cyan=True)
-            tw.write(f" -- {fixture.pretty_path}", yellow=True)
+            tw.write(f" -- {fixture.pretty_path}:{fixture.lineno}", yellow=True)
             tw.write("\n")
 
     def pytest_terminal_summary(
         self,
-        terminalreporter: "TerminalReporter",
-        exitstatus: "ExitCode",
-        config: "Config",
+        terminalreporter: TerminalReporter,
+        exitstatus: ExitCode,
+        config: Config,
     ) -> NoReturn:
         """Add the fixture time report."""
         fullwidth = config.get_terminal_writer().fullwidth
 
         # do a simple set operation to get the unused fixtures
         unused_fixtures = self.available_fixtures - self.used_fixtures
```

### Comparing `pytest_unused_fixtures-0.1.2/pytest_unused_fixtures/xdist.py` & `pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/xdist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+from __future__ import annotations
+
 from dataclasses import asdict
-from typing import TYPE_CHECKING, Any, NoReturn, Union
+from typing import TYPE_CHECKING, Any, NoReturn
 
 from pytest_unused_fixtures.plugin import FixtureInfo, PytestUnusedFixturesPlugin
 
 if TYPE_CHECKING:
     from _pytest.config import ExitCode
     from _pytest.main import Session
     from xdist.workermanage import WorkerController
 
 _WORKEROUTPUT_KEY_USED = "pytest_unused_fixtures_used"
 _WORKEROUTPUT_KEY_AVAILABLE = "pytest_unused_fixtures_available"
 
 
 class PytestUnusedFixturesPluginXdist(PytestUnusedFixturesPlugin):
-    def pytest_sessionfinish(self, session: "Session", exitstatus: Union[int, "ExitCode"]) -> None:
+    def pytest_sessionfinish(self, session: Session, exitstatus: int | ExitCode) -> None:
         # send used & available fixtures
         if (workeroutput := getattr(session.config, "workeroutput", None)) is not None:
             workeroutput[_WORKEROUTPUT_KEY_AVAILABLE] = list(map(asdict, self.available_fixtures))
             workeroutput[_WORKEROUTPUT_KEY_USED] = list(map(asdict, self.used_fixtures))
 
-    def pytest_testnodedown(self, node: "WorkerController", error: Any | None) -> NoReturn:
+    def pytest_testnodedown(self, node: WorkerController, error: Any | None) -> NoReturn:
         if (workeroutput := getattr(node, "workeroutput", None)) is not None:
             # add used & available fixtures from nodes
             if self.available_fixtures is None:
                 self.available_fixtures = set()
             self.available_fixtures.update(
                 FixtureInfo(**x) for x in workeroutput.get(_WORKEROUTPUT_KEY_AVAILABLE, set())
             )
```

### Comparing `pytest_unused_fixtures-0.1.2/PKG-INFO` & `pytest_unused_fixtures-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest-unused-fixtures
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pytest plugin to list unused fixtures after a test run.
 Home-page: https://github.com/mikicz/pytest-unused-fixtures
 License: MIT
 Keywords: pytest,fixtures
 Author: Mikuláš Poul
 Author-email: mikulaspoul@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Project-URL: Repository, https://github.com/mikicz/pytest-unused-fixtures
 Description-Content-Type: text/markdown
@@ -71,14 +72,19 @@
 Many thanks to
 
  - [pytest-deadfixtures](https://github.com/jllorencetti/pytest-deadfixtures) for inspiration for this project
  - [pytest-durations](https://github.com/blake-r/pytest-durations) for inspirations in parts of the implementation
 
 ## Changelog
 
+### 0.1.3 (Jun 30, 2023)
+
+* Print line number
+* Support Python 3.9
+
 ### 0.1.2 (Jun 15, 2023)
 
 * Fix typo, add repository to PyPI
 * Update location handling with respect to showing fixture locations and ignoring paths
 
 ### 0.1.1 (Jun 14, 2023)
```

