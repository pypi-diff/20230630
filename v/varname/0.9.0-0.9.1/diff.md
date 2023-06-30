# Comparing `tmp/varname-0.9.0.tar.gz` & `tmp/varname-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varname-0.9.0.tar", max compression
+gzip compressed data, was "varname-0.9.1.tar", max compression
```

## Comparing `varname-0.9.0.tar` & `varname-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2022-07-26 01:54:18.264960 varname-0.9.0/LICENSE
--rw-r--r--   0        0        0    10961 2022-07-26 01:54:18.264960 varname-0.9.0/README.md
--rw-r--r--   0        0        0     1155 2022-07-26 01:54:18.264960 varname-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      368 2022-07-26 01:54:18.268960 varname-0.9.0/varname/__init__.py
--rw-r--r--   0        0        0    18319 2022-07-26 01:54:18.268960 varname-0.9.0/varname/core.py
--rw-r--r--   0        0        0     5871 2022-07-26 01:54:18.268960 varname-0.9.0/varname/helpers.py
--rw-r--r--   0        0        0    14400 2022-07-26 01:54:18.268960 varname-0.9.0/varname/ignore.py
--rw-r--r--   0        0        0    18508 2022-07-26 01:54:18.268960 varname-0.9.0/varname/utils.py
--rw-r--r--   0        0        0    12290 2022-07-26 01:54:29.794807 varname-0.9.0/setup.py
--rw-r--r--   0        0        0    11830 2022-07-26 01:54:29.795723 varname-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-09-19 18:07:22.908952 varname-0.9.1/LICENSE
+-rw-r--r--   0        0        0    10961 2022-09-19 18:07:22.908952 varname-0.9.1/README.md
+-rw-r--r--   0        0        0     1155 2022-09-19 18:07:22.912952 varname-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      368 2022-09-19 18:07:22.912952 varname-0.9.1/varname/__init__.py
+-rw-r--r--   0        0        0    18319 2022-09-19 18:07:22.912952 varname-0.9.1/varname/core.py
+-rw-r--r--   0        0        0     5871 2022-09-19 18:07:22.912952 varname-0.9.1/varname/helpers.py
+-rw-r--r--   0        0        0    14400 2022-09-19 18:07:22.912952 varname-0.9.1/varname/ignore.py
+-rw-r--r--   0        0        0    18508 2022-09-19 18:07:22.912952 varname-0.9.1/varname/utils.py
+-rw-r--r--   0        0        0    12293 1970-01-01 00:00:00.000000 varname-0.9.1/setup.py
+-rw-r--r--   0        0        0    11829 1970-01-01 00:00:00.000000 varname-0.9.1/PKG-INFO
```

### Comparing `varname-0.9.0/LICENSE` & `varname-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `varname-0.9.0/README.md` & `varname-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `varname-0.9.0/pyproject.toml` & `varname-0.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "varname"
-version = "0.9.0"
+version = "0.9.1"
 description = "Dark magics about variable names in python."
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/python-varname"
 repository = "https://github.com/pwwang/python-varname"
 
 [tool.poetry.dependencies]
 python = "^3.6"
-executing = "^0.9"
+executing = "^1.0"
 asttokens = { version = "2.*", optional = true }
 pure_eval = { version = "0.*", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^3"
```

### Comparing `varname-0.9.0/varname/core.py` & `varname-0.9.1/varname/core.py`

 * *Files identical despite different names*

### Comparing `varname-0.9.0/varname/helpers.py` & `varname-0.9.1/varname/helpers.py`

 * *Files identical despite different names*

### Comparing `varname-0.9.0/varname/ignore.py` & `varname-0.9.1/varname/ignore.py`

 * *Files identical despite different names*

### Comparing `varname-0.9.0/varname/utils.py` & `varname-0.9.1/varname/utils.py`

 * *Files identical despite different names*

### Comparing `varname-0.9.0/setup.py` & `varname-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 packages = \
 ['varname']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['executing>=0.9,<0.10']
+['executing>=1.0,<2.0']
 
 extras_require = \
 {'all': ['asttokens>=2.0.0,<3.0.0', 'pure_eval<1.0.0']}
 
 setup_kwargs = {
     'name': 'varname',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Dark magics about variable names in python.',
     'long_description': '![varname][7]\n\n[![Pypi][3]][4] [![Github][5]][6] [![PythonVers][8]][4] ![Building][10]\n[![Docs and API][9]][15] [![Codacy][12]][13] [![Codacy coverage][14]][13]\n[![Chat on gitter][17]][18]\n\nDark magics about variable names in python\n\n[CHANGELOG][16] | [API][15] | [Playground][11] | :fire: [StackOverflow answer][20]\n\n## Installation\n```shell\npip install -U varname\n```\n\n## Features\n\n- Core features:\n\n  - Retrieving names of variables a function/class call is assigned to from inside it, using `varname`.\n  - Retrieving variable names directly, using `nameof`\n  - Detecting next immediate attribute name, using `will`\n  - Fetching argument names/sources passed to a function using `argname`\n\n- Other helper APIs (built based on core features):\n\n  - A value wrapper to store the variable name that a value is assigned to, using `Wrapper`\n  - A decorator to register `__varname__` to functions/classes, using `register`\n  - A `debug` function to print variables with their names and values\n\n## Credits\n\nThanks goes to these awesome people/projects:\n\n<table>\n  <tr>\n    <td align="center" style="min-width: 75px">\n      <a href="https://github.com/alexmojaki/executing">\n        <img src="https://ui-avatars.com/api/?color=3333ff&background=ffffff&bold=true&name=e&size=400" width="50px;" alt=""/>\n        <br /><sub><b>executing</b></sub>\n      </a>\n    </td>\n    <td align="center" style="min-width: 75px">\n      <a href="https://github.com/alexmojaki">\n        <img src="https://avatars0.githubusercontent.com/u/3627481?s=400&v=4" width="50px;" alt=""/>\n        <br /><sub><b>@alexmojaki</b></sub>\n      </a>\n    </td>\n    <td align="center" style="min-width: 75px">\n      <a href="https://github.com/breuleux">\n        <img src="https://avatars.githubusercontent.com/u/599820?s=400&v=4" width="50px;" alt=""/>\n        <br /><sub><b>@breuleux</b></sub>\n      </a>\n    </td>\n    <td align="center" style="min-width: 75px">\n      <a href="https://github.com/ElCuboNegro">\n        <img src="https://avatars.githubusercontent.com/u/5524219?s=400&v=4" width="50px;" alt=""/>\n        <br /><sub><b>@ElCuboNegro</b></sub>\n      </a>\n    </td>\n    <td align="center" style="min-width: 75px">\n      <a href="https://github.com/thewchan">\n        <img src="https://avatars.githubusercontent.com/u/49702524?s=400&v=4" width="50px;" alt=""/>\n        <br /><sub><b>@thewchan</b></sub>\n      </a>\n    </td>\n    <td align="center" style="min-width: 75px">\n      <a href="https://github.com/LawsOfSympathy">\n        <img src="https://avatars.githubusercontent.com/u/96355982?s=400&v=4" width="50px;" alt=""/>\n        <br /><sub><b>@LawsOfSympathy</b></sub>\n      </a>\n    </td>\n  </tr>\n</table>\n\nSpecial thanks to [@HanyuuLu][2] to give up the name `varname` in pypi for this project.\n\n## Usage\n\n### Retrieving the variable names using `varname(...)`\n\n- From inside a function\n\n    ```python\n    from varname import varname\n    def function():\n        return varname()\n\n    func = function()  # func == \'func\'\n    ```\n\n    When there are intermediate frames:\n    ```python\n    def wrapped():\n        return function()\n\n    def function():\n        # retrieve the variable name at the 2nd frame from this one\n        return varname(frame=2)\n\n    func = wrapped() # func == \'func\'\n    ```\n\n    Or use `ignore` to ignore the wrapped frame:\n    ```python\n    def wrapped():\n        return function()\n\n    def function():\n        return varname(ignore=wrapped)\n\n    func = wrapped() # func == \'func\'\n    ```\n\n    Calls from standard libraries are ignored by default:\n    ```python\n    import asyncio\n\n    async def function():\n        return varname()\n\n    func = asyncio.run(function()) # func == \'func\'\n    ```\n\n    Use `strict` to control whether the call should be assigned to\n    the variable directly:\n    ```python\n    def function(strict):\n        return varname(strict=strict)\n\n    func = function(True)     # OK, direct assignment, func == \'func\'\n\n    func = [function(True)]   # Not a direct assignment, raises ImproperUseError\n    func = [function(False)]  # OK, func == [\'func\']\n\n    func = function(False), function(False)   # OK, func = (\'func\', \'func\')\n    ```\n\n- Retrieving name of a class instance\n\n    ```python\n    class Foo:\n        def __init__(self):\n            self.id = varname()\n\n        def copy(self):\n            # also able to fetch inside a method call\n            copied = Foo() # copied.id == \'copied\'\n            copied.id = varname() # assign id to whatever variable name\n            return copied\n\n    foo = Foo()   # foo.id == \'foo\'\n\n    foo2 = foo.copy() # foo2.id == \'foo2\'\n    ```\n\n- Multiple variables on Left-hand side\n\n    ```python\n    # since v0.5.4\n    def func():\n        return varname(multi_vars=True)\n\n    a = func() # a == (\'a\',)\n    a, b = func() # (a, b) == (\'a\', \'b\')\n    [a, b] = func() # (a, b) == (\'a\', \'b\')\n\n    # hierarchy is also possible\n    a, (b, c) = func() # (a, b, c) == (\'a\', \'b\', \'c\')\n    ```\n\n- Some unusual use\n\n    ```python\n    def function(**kwargs):\n        return varname(strict=False)\n\n    func = func1 = function()  # func == func1 == \'func1\'\n    # if varname < 0.8: func == func1 == \'func\'\n    # a warning will be shown\n    # since you may not want func to be \'func1\'\n\n    x = function(y = function())  # x == \'x\'\n\n    # get part of the name\n    func_abc = function()[-3:]  # func_abc == \'abc\'\n\n    # function alias supported now\n    function2 = function\n    func = function2()  # func == \'func\'\n\n    a = lambda: 0\n    a.b = function() # a.b == \'b\'\n    ```\n\n### The decorator way to register `__varname__` to functions/classes\n\n- Registering `__varname__` to functions\n\n    ```python\n    from varname.helpers import register\n\n    @register\n    def function():\n        return __varname__\n\n    func = function() # func == \'func\'\n    ```\n\n    ```python\n    # arguments also allowed (frame, ignore and raise_exc)\n    @register(frame=2)\n    def function():\n        return __varname__\n\n    def wrapped():\n        return function()\n\n    func = wrapped() # func == \'func\'\n    ```\n\n- Registering `__varname__` as a class property\n\n    ```python\n    @register\n    class Foo:\n        ...\n\n    foo = Foo()\n    # foo.__varname__ == \'foo\'\n    ```\n\n### Getting variable names directly using `nameof`\n\n```python\nfrom varname import varname, nameof\n\na = 1\nnameof(a) # \'a\'\n\nb = 2\nnameof(a, b) # (\'a\', \'b\')\n\ndef func():\n    return varname() + \'_suffix\'\n\nf = func() # f == \'f_suffix\'\nnameof(f)  # \'f\'\n\n# get full names of (chained) attribute calls\nfunc.a = func\nnameof(func.a, vars_only=False) # \'func.a\'\n\nfunc.a.b = 1\nnameof(func.a.b, vars_only=False) # \'func.a.b\'\n```\n\n### Detecting next immediate attribute name\n```python\nfrom varname import will\nclass AwesomeClass:\n    def __init__(self):\n        self.will = None\n\n    def permit(self):\n        self.will = will(raise_exc=False)\n        if self.will == \'do\':\n            # let self handle do\n            return self\n        raise AttributeError(\'Should do something with AwesomeClass object\')\n\n    def do(self):\n        if self.will != \'do\':\n            raise AttributeError("You don\'t have permission to do")\n        return \'I am doing!\'\n\nawesome = AwesomeClass()\nawesome.do() # AttributeError: You don\'t have permission to do\nawesome.permit() # AttributeError: Should do something with AwesomeClass object\nawesome.permit().do() == \'I am doing!\'\n```\n\n### Fetching argument names/sources using `argname`\n```python\nfrom varname import argname\n\ndef func(a, b=1):\n    print(argname(\'a\'))\n\nx = y = z = 2\nfunc(x) # prints: x\n\n\ndef func2(a, b=1):\n    print(argname(\'a\', \'b\'))\nfunc2(y, b=x) # prints: (\'y\', \'x\')\n\n\n# allow expressions\ndef func3(a, b=1):\n    print(argname(\'a\', \'b\', vars_only=False))\nfunc3(x+y, y+x) # prints: (\'x+y\', \'y+x\')\n\n\n# positional and keyword arguments\ndef func4(*args, **kwargs):\n    print(argname(\'args[1]\', \'kwargs[c]\'))\nfunc4(y, x, c=z) # prints: (\'x\', \'z\')\n\n\n# As of 0.9.0 (see: https://pwwang.github.io/python-varname/CHANGELOG/#v090)\n# Can also fetch the source of the argument for\n# __getattr__/__getitem__/__setattr/__setitem__/__add__/__lt__, etc.\nclass Foo:\n    def __setattr__(self, name, value):\n        print(argname("name", "value"))\n\nFoo().a = 1 # prints: ("\'a\'", \'1\')\n\n```\n\n### Value wrapper\n\n```python\nfrom varname.helpers import Wrapper\n\nfoo = Wrapper(True)\n# foo.name == \'foo\'\n# foo.value == True\nbar = Wrapper(False)\n# bar.name == \'bar\'\n# bar.value == False\n\ndef values_to_dict(*args):\n    return {val.name: val.value for val in args}\n\nmydict = values_to_dict(foo, bar)\n# {\'foo\': True, \'bar\': False}\n```\n\n### Debugging with `debug`\n```python\nfrom varname.helpers import debug\n\na = \'value\'\nb = [\'val\']\ndebug(a)\n# "DEBUG: a=\'value\'\\n"\ndebug(b)\n# "DEBUG: b=[\'val\']\\n"\ndebug(a, b)\n# "DEBUG: a=\'value\'\\nDEBUG: b=[\'val\']\\n"\ndebug(a, b, merge=True)\n# "DEBUG: a=\'value\', b=[\'val\']\\n"\ndebug(a, repr=False, prefix=\'\')\n# \'a=value\\n\'\n# also debug an expression\ndebug(a+a)\n# "DEBUG: a+a=\'valuevalue\'\\n"\n# If you want to disable it:\ndebug(a+a, vars_only=True) # ImproperUseError\n```\n\n## Reliability and limitations\n`varname` is all depending on `executing` package to look for the node.\nThe node `executing` detects is ensured to be the correct one (see [this][19]).\n\nIt partially works with environments where other AST magics apply, including\n`pytest`, `ipython`, `macropy`, `birdseye`, `reticulate` with `R`, etc. Neither\n`executing` nor `varname` is 100% working with those environments. Use\nit at your own risk.\n\nFor example:\n\n- This will not work with `pytest`:\n  ```python\n  a = 1\n  assert nameof(a) == \'a\' # pytest manipulated the ast here\n\n  # do this instead\n  name_a = nameof(a)\n  assert name_a == \'a\'\n  ```\n\n[1]: https://github.com/pwwang/python-varname\n[2]: https://github.com/HanyuuLu\n[3]: https://img.shields.io/pypi/v/varname?style=flat-square\n[4]: https://pypi.org/project/varname/\n[5]: https://img.shields.io/github/tag/pwwang/python-varname?style=flat-square\n[6]: https://github.com/pwwang/python-varname\n[7]: logo.png\n[8]: https://img.shields.io/pypi/pyversions/varname?style=flat-square\n[9]: https://img.shields.io/github/workflow/status/pwwang/python-varname/Build%20Docs?label=docs&style=flat-square\n[10]: https://img.shields.io/github/workflow/status/pwwang/python-varname/Build%20and%20Deploy?style=flat-square\n[11]: https://mybinder.org/v2/gh/pwwang/python-varname/dev?filepath=playground%2Fplayground.ipynb\n[12]: https://img.shields.io/codacy/grade/6fdb19c845f74c5c92056e88d44154f7?style=flat-square\n[13]: https://app.codacy.com/gh/pwwang/python-varname/dashboard\n[14]: https://img.shields.io/codacy/coverage/6fdb19c845f74c5c92056e88d44154f7?style=flat-square\n[15]: https://pwwang.github.io/python-varname/api/varname\n[16]: https://pwwang.github.io/python-varname/CHANGELOG/\n[17]: https://img.shields.io/gitter/room/pwwang/python-varname?style=flat-square\n[18]: https://gitter.im/python-varname/community\n[19]: https://github.com/alexmojaki/executing#is-it-reliable\n[20]: https://stackoverflow.com/a/59364138/5088165\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/python-varname',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `varname-0.9.0/PKG-INFO` & `varname-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: varname
-Version: 0.9.0
+Version: 0.9.1
 Summary: Dark magics about variable names in python.
 Home-page: https://github.com/pwwang/python-varname
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: all
 Requires-Dist: asttokens (>=2.0.0,<3.0.0); extra == "all"
-Requires-Dist: executing (>=0.9,<0.10)
+Requires-Dist: executing (>=1.0,<2.0)
 Requires-Dist: pure_eval (<1.0.0); extra == "all"
 Project-URL: Repository, https://github.com/pwwang/python-varname
 Description-Content-Type: text/markdown
 
 ![varname][7]
 
 [![Pypi][3]][4] [![Github][5]][6] [![PythonVers][8]][4] ![Building][10]
```

