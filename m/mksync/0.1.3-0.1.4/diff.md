# Comparing `tmp/mksync-0.1.3.tar.gz` & `tmp/mksync-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mksync-0.1.3.tar", max compression
+gzip compressed data, was "mksync-0.1.4.tar", max compression
```

## Comparing `mksync-0.1.3.tar` & `mksync-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      998 2023-06-29 20:35:59.711226 mksync-0.1.3/LICENSE
--rw-r--r--   0        0        0     2117 2023-06-29 21:39:04.444606 mksync-0.1.3/README.md
--rw-r--r--   0        0        0     1731 2023-06-29 21:39:03.804624 mksync-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      781 2023-06-29 21:39:03.820623 mksync-0.1.3/src/mksync/__init__.py
--rw-r--r--   0        0        0     1123 2023-06-29 20:56:11.733080 mksync-0.1.3/src/mksync/__main__.py
--rw-r--r--   0        0        0      427 2023-06-29 16:54:45.263854 mksync-0.1.3/src/mksync/context.py
--rw-r--r--   0        0        0        5 2023-06-29 16:54:45.263854 mksync-0.1.3/src/mksync/directives/__init__.py
--rw-r--r--   0        0        0      984 2023-06-29 16:54:45.263854 mksync-0.1.3/src/mksync/directives/generic.py
--rw-r--r--   0        0        0     2359 2023-06-29 21:27:26.756219 mksync-0.1.3/src/mksync/directives/include.py
--rw-r--r--   0        0        0     2705 2023-06-29 21:06:40.479346 mksync-0.1.3/src/mksync/directives/parser.py
--rw-r--r--   0        0        0     1931 2023-06-29 21:04:20.275312 mksync-0.1.3/src/mksync/directives/runcmd.py
--rw-r--r--   0        0        0     1946 2023-06-29 21:06:40.471346 mksync-0.1.3/src/mksync/directives/toc.py
--rw-r--r--   0        0        0        0 2023-06-29 20:35:59.711226 mksync-0.1.3/src/mksync/py.typed
--rw-r--r--   0        0        0      330 2023-06-29 16:54:45.263854 mksync-0.1.3/src/mksync/readfile.py
--rw-r--r--   0        0        0     1063 2023-06-29 16:54:45.263854 mksync-0.1.3/src/mksync/targets.py
--rw-r--r--   0        0        0     2724 1970-01-01 00:00:00.000000 mksync-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-06-29 20:35:59.711226 mksync-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2660 2023-06-29 22:13:46.049607 mksync-0.1.4/README.md
+-rw-r--r--   0        0        0     1754 2023-06-29 22:13:44.833642 mksync-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      781 2023-06-29 22:13:44.845641 mksync-0.1.4/src/mksync/__init__.py
+-rw-r--r--   0        0        0     1123 2023-06-29 20:56:11.733080 mksync-0.1.4/src/mksync/__main__.py
+-rw-r--r--   0        0        0      427 2023-06-29 16:54:45.263854 mksync-0.1.4/src/mksync/context.py
+-rw-r--r--   0        0        0        5 2023-06-29 16:54:45.263854 mksync-0.1.4/src/mksync/directives/__init__.py
+-rw-r--r--   0        0        0      984 2023-06-29 16:54:45.263854 mksync-0.1.4/src/mksync/directives/generic.py
+-rw-r--r--   0        0        0     2359 2023-06-29 22:12:12.400262 mksync-0.1.4/src/mksync/directives/include.py
+-rw-r--r--   0        0        0     2744 2023-06-29 22:11:41.465139 mksync-0.1.4/src/mksync/directives/parser.py
+-rw-r--r--   0        0        0     1931 2023-06-29 21:04:20.275312 mksync-0.1.4/src/mksync/directives/runcmd.py
+-rw-r--r--   0        0        0     1982 2023-06-29 22:11:54.344774 mksync-0.1.4/src/mksync/directives/toc.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:35:59.711226 mksync-0.1.4/src/mksync/py.typed
+-rw-r--r--   0        0        0      330 2023-06-29 16:54:45.263854 mksync-0.1.4/src/mksync/readfile.py
+-rw-r--r--   0        0        0     1063 2023-06-29 16:54:45.263854 mksync-0.1.4/src/mksync/targets.py
+-rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 mksync-0.1.4/PKG-INFO
```

### Comparing `mksync-0.1.3/LICENSE` & `mksync-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mksync-0.1.3/README.md` & `mksync-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 features to your project's `README.md` file, such as a table of contents, without the manual upkeep.
 
 <!-- table of contents -->
   * [Example](#example)
   * [Available Directives](#available-directives)
   * [Synopsis](#synopsis)
 * [Changelog](#changelog)
-  * [Unreleased](#unreleased)
+  * [0.1.4 (2023-06-29)](#014-2023-06-29)
+  * [0.1.3 (2023-06-29)](#013-2023-06-29)
 <!-- end table of contents -->
 
 ## Example
 
 Say this is your `README.md`:
 
 ```md
@@ -68,14 +69,25 @@
 <!-- end runcmd -->
 
 ---
 
 # Changelog
 
 <!-- runcmd slap changelog format --all --markdown -->
+## 0.1.4 (2023-06-29)
+
+<table><tr><th>Type</th><th>Description</th><th>PR</th><th>Issues</th><th>Author</th></tr>
+  <tr><td>Fix</td><td>
+
+Fix placement of code block when rendering `include` directive back into the Markdown file.</td><td></td><td></td><td>@NiklasRosenstein</td></tr>
+  <tr><td>Improvement</td><td>
+
+Keep the same keyword that was used for the TOC directive, which can be one of `toc` and `table of contents`</td><td></td><td></td><td>@NiklasRosenstein</td></tr>
+</table>
+
 ## 0.1.3 (2023-06-29)
 
 <table><tr><th>Type</th><th>Description</th><th>PR</th><th>Issues</th><th>Author</th></tr>
   <tr><td>Fix</td><td>
 
 Fix parsing of `include` directives</td><td></td><td></td><td>@NiklasRosenstein</td></tr>
 </table>
```

#### html2text {}

```diff
@@ -1,24 +1,33 @@
 # mksync MkSync replaces directives in a Markdown file with corresponding
 content. It's a useful tool to add nice features to your project's `README.md`
 file, such as a table of contents, without the manual upkeep.  * [Example]
 (#example) * [Available Directives](#available-directives) * [Synopsis]
-(#synopsis) * [Changelog](#changelog) * [Unreleased](#unreleased)  ## Example
-Say this is your `README.md`: ```md # My Project  ## Installation ##
-Documentation ``` Then running `mksync README.md` will update the file in-place
-to: ```md # My Project  * [Installation](#installation) * [Documentation]
-(#documentation)  ## Installation ## Documentation ``` ## Available Directives
-* `toc` or `table of contents`: Produce an unordered list of links to all
-headers in the document after the directive. * `include `: Include the contents
-of the file at the given path. You can optionally specify a language name to
-wrap the content in a code block, e.g. `include code:python `. * `runcmd `: Run
-the given command and include the output in the document. You can optionally
-specify a language name to wrap the output in a code block, e.g. `runcmd code:
-python `. ## Synopsis  ``` usage: mksync [-h] [--inplace] [--verbose] file
-MkSync is a utility to update Markdown files in-place to automate some common
-upkeep tasks, such as inling example code and updating table of contents.
-positional arguments: file the file to process options: -h, --help show this
-help message and exit --inplace, -i update the file in-place --verbose, -
-v enable verbose logging ```  --- # Changelog  ## 0.1.3 (2023-06-29)
+(#synopsis) * [Changelog](#changelog) * [0.1.4 (2023-06-29)](#014-2023-06-29) *
+[0.1.3 (2023-06-29)](#013-2023-06-29)  ## Example Say this is your `README.md`:
+```md # My Project  ## Installation ## Documentation ``` Then running `mksync
+README.md` will update the file in-place to: ```md # My Project  *
+[Installation](#installation) * [Documentation](#documentation)  ##
+Installation ## Documentation ``` ## Available Directives * `toc` or `table of
+contents`: Produce an unordered list of links to all headers in the document
+after the directive. * `include `: Include the contents of the file at the
+given path. You can optionally specify a language name to wrap the content in a
+code block, e.g. `include code:python `. * `runcmd `: Run the given command and
+include the output in the document. You can optionally specify a language name
+to wrap the output in a code block, e.g. `runcmd code:python `. ## Synopsis
+``` usage: mksync [-h] [--inplace] [--verbose] file MkSync is a utility to
+update Markdown files in-place to automate some common upkeep tasks, such as
+inling example code and updating table of contents. positional arguments: file
+the file to process options: -h, --help show this help message and exit --
+inplace, -i update the file in-place --verbose, -v enable verbose logging ```
+--- # Changelog  ## 0.1.4 (2023-06-29)
+Type        Description                             PR Issues Author
+            Fix placement of code block when
+Fix         rendering `include` directive back into           @NiklasRosenstein
+            the Markdown file.
+            Keep the same keyword that was used for
+Improvement the TOC directive, which can be one of            @NiklasRosenstein
+            `toc` and `table of contents`
+## 0.1.3 (2023-06-29)
 Type Description                         PR Issues Author
 Fix  Fix parsing of `include` directives           @NiklasRosenstein
```

### Comparing `mksync-0.1.3/pyproject.toml` & `mksync-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mksync"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 packages = [{ include = "mksync", from = "src" }]
 classifiers = []
 keywords = []
 readme = "README.md"
@@ -40,15 +40,15 @@
 [tool.poetry.scripts]
 mksync = "mksync.__main__:main"
 
 [tool.slap]
 typed = true
 
 [tool.slap.release]
-pre-commit = "mksync README.md -i && git add README.md"
+pre-commit = "mksync README.md -i && mksync README.md -i && git add README.md"
 
 [tool.slap.test]
 check  = "slap check"
 black  = "black --check src/ tests/"
 flake8 = "flake8 src/ tests/"
 isort  = "isort --check-only src/ tests/"
 mypy   = "dmypy run src/"
```

### Comparing `mksync-0.1.3/src/mksync/__init__.py` & `mksync-0.1.4/src/mksync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from pathlib import Path
 
 from adjudicator import Params, RuleEngine
 
 from mksync.targets import PreprocessFileResult, PreprocessFileTarget
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __all__ = ["mksync_file"]
 logger = logging.getLogger(__name__)
 modules = [
     "mksync." + x
     for x in [
         "readfile",
         "targets",
```

### Comparing `mksync-0.1.3/src/mksync/__main__.py` & `mksync-0.1.4/src/mksync/__main__.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.3/src/mksync/directives/generic.py` & `mksync-0.1.4/src/mksync/directives/generic.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.3/src/mksync/directives/include.py` & `mksync-0.1.4/src/mksync/directives/include.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 def _get_include_file_directives(request: PreprocessFileTarget) -> IncludeFileDirectives:
     content = get(ReadFile, ReadFileRequest(request.path)).content
     return IncludeFileDirectives(IncludeFileDirective.parse(content))
 
 
 @rule()
 def _include_file_request(request: IncludeFileDirective) -> RenderedDirective:
-    code = f" code:{request.code}" if request.code else ""
+    code = f"code:{request.code} " if request.code else ""
     begin_marker = f"```{request.code}\n" if request.code else ""
     end_marker = "```\n" if request.code else ""
     return RenderedDirective(
-        f"<!-- include {request.filename}{code} -->\n{begin_marker}"
+        f"<!-- include {code}{request.filename} -->\n{begin_marker}"
         + Path(request.filename).read_text().strip()
         + f"\n{end_marker}<!-- end include -->"
     )
```

### Comparing `mksync-0.1.3/src/mksync/directives/parser.py` & `mksync-0.1.4/src/mksync/directives/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 @dataclass(frozen=True)
 class ParsedDirective:
     begin: int
     end: int
     opts: str
+    keyword: str
 
 
 def parse_directives(text: str, *keywords: str) -> Iterator[ParsedDirective]:
     codeblocks = get_codeblock_positions(text)
     begin_regex = re.compile(r"<!--\s*(" + "|".join(map(re.escape, keywords)) + r")(.*)?\s*-->")
     end_regex = re.compile(r"<!--\s*end\s*(" + "|".join(map(re.escape, keywords)) + r")\s*-->")
     offset = 0
@@ -53,15 +54,15 @@
             end = begin_match.end()
             offset = begin_match.end()
         else:
             end = end_match.end()
             offset = end_match.end()
 
         logger.debug("Found directive %r in [%d, %d]", begin_match.group(1), begin, end)
-        yield ParsedDirective(begin, end, opts)
+        yield ParsedDirective(begin, end, opts, begin_match.group(1))
 
         begin_match = next_begin_match
 
 
 def get_codeblock_positions(text: str) -> list[tuple[int, int]]:
     """
     Returns a list of pairs of indices marking the beginning and end of Markdown code blocks in *text*.
```

### Comparing `mksync-0.1.3/src/mksync/directives/runcmd.py` & `mksync-0.1.4/src/mksync/directives/runcmd.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.3/src/mksync/directives/toc.py` & `mksync-0.1.4/src/mksync/directives/toc.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 from .parser import get_codeblock_positions, is_position_inside_codeblock, parse_directives
 
 
 @dataclass(frozen=True)
 @union_rule()
 class TocDirective(PreprocessorDirective):
     path: Path
+    keyword: str
 
     @classmethod
     def parse(cls, path: Path, text: str) -> Iterator[TocDirective]:
         for directive in parse_directives(text, "table of contents", "toc"):
-            yield cls(directive.begin, directive.end, path)
+            yield cls(directive.begin, directive.end, path, directive.keyword)
 
 
 @union_rule(PreprocessorDirectives)
 class TocDirectives(GenericPreprocessorDirectives["TocDirective"]):
     ...
 
 
@@ -47,8 +48,8 @@
     toc = []
     for match in matches:
         depth = len(match.group(1)) - min_depth
         anchor = re.sub(r"[^a-zA-Z0-9-]", "", match.group(2).lower().replace(" ", "-"))
         toc.append("  " * depth + f"* [{match.group(2)}](#{anchor})")
 
     toc_string = "\n".join(toc)
-    return RenderedDirective(f"<!-- table of contents -->\n{toc_string}\n<!-- end table of contents -->")
+    return RenderedDirective(f"<!-- {request.keyword} -->\n{toc_string}\n<!-- end {request.keyword} -->")
```

### Comparing `mksync-0.1.3/src/mksync/targets.py` & `mksync-0.1.4/src/mksync/targets.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.3/PKG-INFO` & `mksync-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mksync
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,16 @@
 features to your project's `README.md` file, such as a table of contents, without the manual upkeep.
 
 <!-- table of contents -->
   * [Example](#example)
   * [Available Directives](#available-directives)
   * [Synopsis](#synopsis)
 * [Changelog](#changelog)
-  * [Unreleased](#unreleased)
+  * [0.1.4 (2023-06-29)](#014-2023-06-29)
+  * [0.1.3 (2023-06-29)](#013-2023-06-29)
 <!-- end table of contents -->
 
 ## Example
 
 Say this is your `README.md`:
 
 ```md
@@ -85,14 +86,25 @@
 <!-- end runcmd -->
 
 ---
 
 # Changelog
 
 <!-- runcmd slap changelog format --all --markdown -->
+## 0.1.4 (2023-06-29)
+
+<table><tr><th>Type</th><th>Description</th><th>PR</th><th>Issues</th><th>Author</th></tr>
+  <tr><td>Fix</td><td>
+
+Fix placement of code block when rendering `include` directive back into the Markdown file.</td><td></td><td></td><td>@NiklasRosenstein</td></tr>
+  <tr><td>Improvement</td><td>
+
+Keep the same keyword that was used for the TOC directive, which can be one of `toc` and `table of contents`</td><td></td><td></td><td>@NiklasRosenstein</td></tr>
+</table>
+
 ## 0.1.3 (2023-06-29)
 
 <table><tr><th>Type</th><th>Description</th><th>PR</th><th>Issues</th><th>Author</th></tr>
   <tr><td>Fix</td><td>
 
 Fix parsing of `include` directives</td><td></td><td></td><td>@NiklasRosenstein</td></tr>
 </table>
```

#### html2text {}

```diff
@@ -1,32 +1,41 @@
-Metadata-Version: 2.1 Name: mksync Version: 0.1.3 Summary: License: MIT Author:
+Metadata-Version: 2.1 Name: mksync Version: 0.1.4 Summary: License: MIT Author:
 Niklas Rosenstein Author-email: rosensteinniklas@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 python-adjudicator (>=0.3.1,<0.4.0) Project-URL: Bug Tracker, https://
 github.com/NiklasRosenstein/mksync/issues Project-URL: Repository, https://
 github.com/NiklasRosenstein/mksync Description-Content-Type: text/markdown #
 mksync MkSync replaces directives in a Markdown file with corresponding
 content. It's a useful tool to add nice features to your project's `README.md`
 file, such as a table of contents, without the manual upkeep.  * [Example]
 (#example) * [Available Directives](#available-directives) * [Synopsis]
-(#synopsis) * [Changelog](#changelog) * [Unreleased](#unreleased)  ## Example
-Say this is your `README.md`: ```md # My Project  ## Installation ##
-Documentation ``` Then running `mksync README.md` will update the file in-place
-to: ```md # My Project  * [Installation](#installation) * [Documentation]
-(#documentation)  ## Installation ## Documentation ``` ## Available Directives
-* `toc` or `table of contents`: Produce an unordered list of links to all
-headers in the document after the directive. * `include `: Include the contents
-of the file at the given path. You can optionally specify a language name to
-wrap the content in a code block, e.g. `include code:python `. * `runcmd `: Run
-the given command and include the output in the document. You can optionally
-specify a language name to wrap the output in a code block, e.g. `runcmd code:
-python `. ## Synopsis  ``` usage: mksync [-h] [--inplace] [--verbose] file
-MkSync is a utility to update Markdown files in-place to automate some common
-upkeep tasks, such as inling example code and updating table of contents.
-positional arguments: file the file to process options: -h, --help show this
-help message and exit --inplace, -i update the file in-place --verbose, -
-v enable verbose logging ```  --- # Changelog  ## 0.1.3 (2023-06-29)
+(#synopsis) * [Changelog](#changelog) * [0.1.4 (2023-06-29)](#014-2023-06-29) *
+[0.1.3 (2023-06-29)](#013-2023-06-29)  ## Example Say this is your `README.md`:
+```md # My Project  ## Installation ## Documentation ``` Then running `mksync
+README.md` will update the file in-place to: ```md # My Project  *
+[Installation](#installation) * [Documentation](#documentation)  ##
+Installation ## Documentation ``` ## Available Directives * `toc` or `table of
+contents`: Produce an unordered list of links to all headers in the document
+after the directive. * `include `: Include the contents of the file at the
+given path. You can optionally specify a language name to wrap the content in a
+code block, e.g. `include code:python `. * `runcmd `: Run the given command and
+include the output in the document. You can optionally specify a language name
+to wrap the output in a code block, e.g. `runcmd code:python `. ## Synopsis
+``` usage: mksync [-h] [--inplace] [--verbose] file MkSync is a utility to
+update Markdown files in-place to automate some common upkeep tasks, such as
+inling example code and updating table of contents. positional arguments: file
+the file to process options: -h, --help show this help message and exit --
+inplace, -i update the file in-place --verbose, -v enable verbose logging ```
+--- # Changelog  ## 0.1.4 (2023-06-29)
+Type        Description                             PR Issues Author
+            Fix placement of code block when
+Fix         rendering `include` directive back into           @NiklasRosenstein
+            the Markdown file.
+            Keep the same keyword that was used for
+Improvement the TOC directive, which can be one of            @NiklasRosenstein
+            `toc` and `table of contents`
+## 0.1.3 (2023-06-29)
 Type Description                         PR Issues Author
 Fix  Fix parsing of `include` directives           @NiklasRosenstein
```

