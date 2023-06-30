# Comparing `tmp/arclet-alconna-1.7.7.tar.gz` & `tmp/arclet-alconna-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.7.tar", last modified: Thu May 25 17:54:03 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.8.tar", last modified: Fri Jun 30 14:54:00 2023, max compression
```

## Comparing `arclet-alconna-1.7.7.tar` & `arclet-alconna-1.7.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.7/LICENSE
--rw-r--r--   0        0        0     2810 2023-05-25 16:57:28.459958 arclet-alconna-1.7.7/pyproject.toml
--rw-r--r--   0        0        0     6702 2023-05-25 16:37:15.089363 arclet-alconna-1.7.7/README-EN.md
--rw-r--r--   0        0        0     1084 2023-05-25 16:37:15.105359 arclet-alconna-1.7.7/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 16:37:15.106361 arclet-alconna-1.7.7/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    17705 2023-05-25 17:31:34.682918 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0     8476 2023-05-25 16:37:15.107359 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    23280 2023-05-25 17:07:20.959020 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0    10053 2023-05-25 17:28:18.129401 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0     1333 2023-05-25 17:53:21.656271 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1543 2023-05-25 16:37:15.110384 arclet-alconna-1.7.7/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    14323 2023-05-25 17:43:52.094619 arclet-alconna-1.7.7/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1499 2023-05-25 16:37:15.112359 arclet-alconna-1.7.7/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    15488 2023-05-25 17:37:16.116622 arclet-alconna-1.7.7/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    13248 2023-05-25 16:37:15.114361 arclet-alconna-1.7.7/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     2715 2023-05-25 17:37:16.076621 arclet-alconna-1.7.7/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     4867 2023-05-25 16:37:15.116360 arclet-alconna-1.7.7/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4465 2023-05-25 16:37:15.117360 arclet-alconna-1.7.7/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14061 2023-05-25 16:37:15.117360 arclet-alconna-1.7.7/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2014 2023-05-25 17:41:01.475077 arclet-alconna-1.7.7/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-05-25 16:37:15.119359 arclet-alconna-1.7.7/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11287 2023-05-25 16:37:15.120361 arclet-alconna-1.7.7/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       99 2023-05-21 05:43:33.502836 arclet-alconna-1.7.7/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3638 2023-05-21 05:43:33.503837 arclet-alconna-1.7.7/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3687 2023-05-21 05:43:33.504836 arclet-alconna-1.7.7/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    17039 2023-05-25 17:37:16.096623 arclet-alconna-1.7.7/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1484 2023-05-25 16:37:15.122358 arclet-alconna-1.7.7/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1943 2023-05-25 16:37:15.123407 arclet-alconna-1.7.7/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3940 2023-05-25 16:37:15.124599 arclet-alconna-1.7.7/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-05-21 05:43:33.513926 arclet-alconna-1.7.7/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5815 2023-05-25 16:37:15.125359 arclet-alconna-1.7.7/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     3586 2023-05-25 16:37:15.125704 arclet-alconna-1.7.7/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3246 2023-05-25 16:37:15.127191 arclet-alconna-1.7.7/tests/analyser_test.py
--rw-r--r--   0        0        0     7583 2023-05-25 16:37:15.127710 arclet-alconna-1.7.7/tests/args_test.py
--rw-r--r--   0        0        0     2167 2023-05-25 16:37:15.128711 arclet-alconna-1.7.7/tests/base_test.py
--rw-r--r--   0        0        0     3119 2023-05-25 17:37:16.085622 arclet-alconna-1.7.7/tests/components_test.py
--rw-r--r--   0        0        0     1199 2023-05-25 16:37:15.130711 arclet-alconna-1.7.7/tests/config_test.py
--rw-r--r--   0        0        0    24318 2023-05-25 17:21:11.641086 arclet-alconna-1.7.7/tests/core_test.py
--rw-r--r--   0        0        0      505 2023-05-25 16:37:15.132710 arclet-alconna-1.7.7/tests/util_test.py
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.8/LICENSE
+-rw-r--r--   0        0        0     2810 2023-06-08 08:47:20.882466 arclet-alconna-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0     6644 2023-06-30 14:51:14.232836 arclet-alconna-1.7.8/README-EN.md
+-rw-r--r--   0        0        0     1084 2023-06-30 14:50:29.541004 arclet-alconna-1.7.8/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:37:15.106361 arclet-alconna-1.7.8/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    17705 2023-06-08 08:47:20.884468 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8476 2023-05-25 16:37:15.107359 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    23280 2023-06-08 08:47:20.884468 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0    10053 2023-06-08 08:48:46.609460 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0     1333 2023-06-08 08:47:20.886467 arclet-alconna-1.7.8/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1543 2023-05-25 16:37:15.110384 arclet-alconna-1.7.8/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14606 2023-06-30 14:47:51.057920 arclet-alconna-1.7.8/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1499 2023-05-25 16:37:15.112359 arclet-alconna-1.7.8/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15488 2023-06-08 08:47:20.888469 arclet-alconna-1.7.8/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    13248 2023-05-25 16:37:15.114361 arclet-alconna-1.7.8/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     2715 2023-06-08 08:47:20.889467 arclet-alconna-1.7.8/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4867 2023-05-25 16:37:15.116360 arclet-alconna-1.7.8/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4465 2023-05-25 16:37:15.117360 arclet-alconna-1.7.8/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14029 2023-06-25 08:21:06.237281 arclet-alconna-1.7.8/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2014 2023-06-08 08:47:20.890468 arclet-alconna-1.7.8/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-05-25 16:37:15.119359 arclet-alconna-1.7.8/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11287 2023-05-25 16:37:15.120361 arclet-alconna-1.7.8/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-21 05:43:33.502836 arclet-alconna-1.7.8/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3638 2023-05-21 05:43:33.503837 arclet-alconna-1.7.8/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3687 2023-05-21 05:43:33.504836 arclet-alconna-1.7.8/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    17039 2023-06-08 08:47:20.891468 arclet-alconna-1.7.8/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1484 2023-05-25 16:37:15.122358 arclet-alconna-1.7.8/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-25 16:37:15.123407 arclet-alconna-1.7.8/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-25 16:37:15.124599 arclet-alconna-1.7.8/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-21 05:43:33.513926 arclet-alconna-1.7.8/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5815 2023-05-25 16:37:15.125359 arclet-alconna-1.7.8/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3586 2023-05-25 16:37:15.125704 arclet-alconna-1.7.8/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3246 2023-05-25 16:37:15.127191 arclet-alconna-1.7.8/tests/analyser_test.py
+-rw-r--r--   0        0        0     7583 2023-05-25 16:37:15.127710 arclet-alconna-1.7.8/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-25 16:37:15.128711 arclet-alconna-1.7.8/tests/base_test.py
+-rw-r--r--   0        0        0     3119 2023-06-08 08:47:20.892467 arclet-alconna-1.7.8/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-25 16:37:15.130711 arclet-alconna-1.7.8/tests/config_test.py
+-rw-r--r--   0        0        0    24318 2023-06-12 11:16:57.189124 arclet-alconna-1.7.8/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-25 16:37:15.132710 arclet-alconna-1.7.8/tests/util_test.py
+-rw-r--r--   0        0        0     7306 1970-01-01 00:00:00.000000 arclet-alconna-1.7.8/PKG-INFO
```

### Comparing `arclet-alconna-1.7.7/LICENSE` & `arclet-alconna-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/pyproject.toml` & `arclet-alconna-1.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.7"
+version = "1.7.8"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.7/README-EN.md` & `arclet-alconna-1.7.8/README-EN.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,19 @@
 
 ## Installation
 
 pip
 ```shell
 $ pip install --upgrade arclet-alconna
 $ pip install --upgrade arclet-alconna[full]
-$ pip install --upgrade arclet-alconna[all]
 ```
 
 ## Documentation
 
-Official Document : [👉Link](https://arcletproject.github.io/docs/alconna/tutorial)
+Official Document : [👉Link](https://arclet.top/docs/tutorial/alconna)
 
 Relevant Document : [📚Docs](https://graiax.cn/guide/message_parser/alconna.html)
 
 ## A Simple Example
 
 ```python
 from arclet.alconna import Alconna, Option, Subcommand, Args
```

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.8/src/arclet/alconna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 from .builtin import set_default
 from .model import OptionResult, SubcommandResult, HeadResult
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.7"
+__version__ = "1.7.8"
 
 # backward compatibility
 Arpamar = Arparma
 DataCollectionContainer = Argv
```

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/_internal/_analyser.py` & `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_analyser.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/_internal/_argv.py` & `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/_internal/_handlers.py` & `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_handlers.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/_internal/_header.py` & `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_header.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/_internal/_util.py` & `arclet-alconna-1.7.8/src/arclet/alconna/_internal/_util.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/action.py` & `arclet-alconna-1.7.8/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/args.py` & `arclet-alconna-1.7.8/src/arclet/alconna/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 from copy import deepcopy
 from enum import Enum
 from functools import partial
 from typing import Any, Callable, Generic, Iterable, Sequence, TypeVar, Union
 
 from nepattern import AllParam, AnyOne, BasePattern, RawStr, UnionPattern, all_patterns, type_parser
 from tarina import Empty, get_signature, lang
-from typing_extensions import Self
+from typing_extensions import Self, TypeAlias
 
 from .exceptions import InvalidParam
 from .typing import KeyWordVar, MultiVar
 
 
 def safe_dcls_kw(**kwargs):
     if sys.version_info < (3, 10):  # pragma: no cover
         kwargs.pop('slots')
     return kwargs
 
 
 _T = TypeVar("_T")
-TAValue = Union[BasePattern, AllParam.__class__, type, str]
+TAValue: TypeAlias = Union[BasePattern[_T], type[_T], str]
 STRING = all_patterns()[str]
 
 
 class ArgFlag(str, Enum):
     """标识参数单元的特殊属性"""
     OPTIONAL = '?'
     HIDDEN = "/"
@@ -49,47 +49,47 @@
     @property
     def display(self):
         """返回参数单元的显示值"""
         return self.alias or self.default
 
 
 @dc.dataclass(**safe_dcls_kw(init=False, eq=True, unsafe_hash=True, slots=True))
-class Arg:
+class Arg(Generic[_T]):
     """参数单元"""
 
     name: str = dc.field(compare=True, hash=True)
     """参数单元的名称"""
-    value: BasePattern = dc.field(compare=False, hash=True)
+    value: BasePattern[_T] = dc.field(compare=False, hash=True)
     """参数单元的值"""
-    field: Field[Any] = dc.field(compare=False, hash=False)
+    field: Field[_T] = dc.field(compare=False, hash=False)
     """参数单元的字段"""
     notice: str | None = dc.field(compare=False, hash=False)
     """参数单元的注释"""
     flag: set[ArgFlag] = dc.field(compare=False, hash=False)
     """参数单元的标识"""
     separators: tuple[str, ...] = dc.field(compare=False, hash=False)
     """参数单元使用的分隔符"""
     optional: bool = dc.field(compare=False, hash=False)
     hidden: bool = dc.field(compare=False, hash=False)
     anonymous: bool = dc.field(compare=False, hash=False)
 
     def __init__(
         self,
         name: str,
-        value: TAValue | None = None,
+        value: TAValue[_T] | None = None,
         field: Field[_T] | _T | None = None,
         seps: str | Iterable[str] = " ",
         notice: str | None = None,
         flags: list[ArgFlag] | None = None,
     ):
         """构造参数单元
 
         Args:
             name (str): 参数单元的名称
-            value (TAValue, optional): 参数单元的值. Defaults to None.
+            value (TAValue[_T], optional): 参数单元的值. Defaults to None.
             field (Field[_T], optional): 参数单元的字段. Defaults to None.
             seps (str | Iterable[str], optional): 参数单元使用的分隔符. Defaults to " ".
             notice (str, optional): 参数单元的注释. Defaults to None.
             flags (list[ArgFlag], optional): 参数单元的标识. Defaults to None.
         """
         if not isinstance(name, str) or name.startswith('$'):
             raise InvalidParam(lang.require("args", "name_error"))
@@ -122,14 +122,20 @@
         if ArgFlag.ANTI in self.flag and self.value not in (AnyOne, AllParam):
             self.value = deepcopy(self.value).reverse()
 
     def __repr__(self):
         n, v = f"'{self.name}'", str(self.value)
         return (n if n == v else f"{n}: {v}") + (f" = '{self.field.display}'" if self.field.display is not None else "")
 
+    def __add__(self, other) -> "Args":
+        if isinstance(other, Arg):
+            return Args(self, other)
+        raise TypeError(f"unsupported operand type(s) for +: 'Arg' and '{other.__class__.__name__}'")
+    
+
 
 class ArgsMeta(type):
     """`Args` 类的元类"""
 
     def __getattr__(self, name: str):
         return type("_S", (), {"__getitem__": partial(self.__class__.__getitem__, self, key=name), "__call__": None})()
 
@@ -160,15 +166,15 @@
         Args('name': str, 'age': int)
 
     也可以使用特殊方法 `__getattr__` 来构造参数集合, 例如:
 
         >>> Args.name[str]
         Args('name': str)
     """
-    argument: list[Arg]
+    argument: list[Arg[Any]]
     """参数单元组"""
     var_positional: MultiVar | None
     """可变参数"""
     var_keyword: MultiVar | None
     """可变关键字参数"""
     keyword_only: list[str]
     """仅关键字参数的名称"""
@@ -207,15 +213,15 @@
             if param.kind == param.VAR_POSITIONAL:
                 anno = MultiVar(anno, "*")
             if param.kind == param.VAR_KEYWORD:
                 anno = MultiVar(KeyWordVar(anno), "*")
             _args.add(name, value=anno, default=de)
         return _args, method
 
-    def __init__(self, *args: Arg, separators: str | Iterable[str] | None = None, **kwargs: TAValue):
+    def __init__(self, *args: Arg[Any], separators: str | Iterable[str] | None = None, **kwargs: TAValue[Any]):
         """
         构造一个 `Args`
 
         Args:
             *args (Arg): 参数单元
             separators (str | Iterable[str] | None, optional): 可选的为所有参数单元指定分隔符
             **kwargs (TAValue): 剩余的参数单元值
@@ -229,15 +235,15 @@
         self.argument.extend(Arg(k, type_parser(v), Field()) for k, v in kwargs.items())
         self.__check_vars__()
         if separators is not None:
             self.separate(*((separators,) if isinstance(separators, str) else tuple(separators)))
 
     __slots__ = "var_positional", "var_keyword", "argument", "optional_count", "keyword_only", "_visit"
 
-    def add(self, name: str, *, value: TAValue, default: Any = None, flags: list[ArgFlag] | None = None) -> Self:
+    def add(self, name: str, *, value: TAValue[Any], default: Any = None, flags: list[ArgFlag] | None = None) -> Self:
         """添加一个参数
 
         Args:
             name (str): 参数名称
             value (TAValue): 参数值
             default (Any, optional): 参数默认值.
             flags (list[ArgFlag] | None, optional): 参数标记.
@@ -307,15 +313,15 @@
                 else:
                     self.var_positional = arg.value
             if isinstance(arg.value, KeyWordVar):
                 if self.var_keyword or self.var_positional:
                     raise InvalidParam(lang.require("args", "exclude_mutable_args"))
                 self.keyword_only.append(arg.name)
                 if arg.value.sep in arg.separators:
-                    _tmp.insert(-1, Arg(f"_key_{arg.name}", value=f"-*{arg.name}"))
+                    _tmp.insert(-1, Arg(f"_key_{arg.name}", value=f"re:-*{arg.name}"))
                     _tmp[-1].value = arg.value.base
             if arg.optional:
                 if self.var_keyword or self.var_positional:
                     raise InvalidParam(lang.require("args", "exclude_mutable_args"))
                 self.optional_count += 1
         self.argument.clear()
         self.argument.extend(_tmp)
```

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/argv.py` & `arclet-alconna-1.7.8/src/arclet/alconna/argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.8/src/arclet/alconna/arparma.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/base.py` & `arclet-alconna-1.7.8/src/arclet/alconna/base.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.8/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.8/src/arclet/alconna/completion.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/config.py` & `arclet-alconna-1.7.8/src/arclet/alconna/config.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/core.py` & `arclet-alconna-1.7.8/src/arclet/alconna/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,34 +140,32 @@
         """
         if not namespace:
             ns_config = config.default_namespace
         elif isinstance(namespace, str):
             ns_config = config.namespaces.setdefault(namespace, Namespace(namespace))
         else:
             ns_config = namespace
-        self.prefixes = next(filter(lambda x: isinstance(x, list), args), ns_config.prefixes.copy())  # type: ignore
+        self.prefixes = next((i for i in args if isinstance(i, list)), ns_config.prefixes.copy())  # type: ignore
         try:
-            self.command = next(filter(lambda x: not isinstance(x, (list, Option, Subcommand, Args, Arg)), args))
+            self.command = next(i for i in args if not isinstance(i, (list, Option, Subcommand, Args, Arg)))
         except StopIteration:
             self.command = "" if self.prefixes else handle_argv()
         self.namespace = ns_config.name
         self.formatter = (formatter_type or ns_config.formatter_type or TextFormatter)()
         self.meta = meta or CommandMeta()
         if self.meta.example:
             self.meta.example = self.meta.example.replace("$", str(self.prefixes[0]) if self.prefixes else "")
         self.meta.fuzzy_match = self.meta.fuzzy_match or ns_config.fuzzy_match
         self.meta.raise_exception = self.meta.raise_exception or ns_config.raise_exception
         self.meta.compact = self.meta.compact or ns_config.compact
         options = [i for i in args if isinstance(i, (Option, Subcommand))]
         add_builtin_options(options, ns_config)
         name = f"{self.command or self.prefixes[0]}"  # type: ignore
         self.path = f"{self.namespace}::{name}"
-        _args = Args()
-        for i in filter(lambda x: isinstance(x, (Args, Arg)), args):
-            _args << i
+        _args = sum((i for i in args if isinstance(i, (Args, Arg))), Args())
         super().__init__(
             "ALCONNA::",
             _args, *options, dest=name, separators=separators or ns_config.separators, help_text=self.meta.description
         )
         self.name = name
         self.behaviors = []
         for behavior in behaviors or []:
@@ -226,15 +224,15 @@
                 return lang.require("shortcut", "delete_success").format(shortcut=key, target=self.path)
             if args:
                 command_manager.add_shortcut(self, key, args)
                 return lang.require("shortcut", "add_success").format(shortcut=key, target=self.path)
             elif cmd := command_manager.recent_message:
                 alc = command_manager.last_using
                 if alc and alc == self:
-                    command_manager.add_shortcut(self, key, {"command": cmd})
+                    command_manager.add_shortcut(self, key, {"command": cmd})  # type: ignore
                     return lang.require("shortcut", "add_success").format(shortcut=key, target=self.path)
                 raise ValueError(
                     lang.require("shortcut", "recent_command_error")
                     .format(target=self.path, source=getattr(alc, "path", "Unknown"))
                 )
             else:
                 raise ValueError(lang.require("shortcut", "no_recent_command"))
```

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.8/src/arclet/alconna/duplication.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.8/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.8/src/arclet/alconna/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.8/src/arclet/alconna/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.8/src/arclet/alconna/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.8/src/arclet/alconna/manager.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/model.py` & `arclet-alconna-1.7.8/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.8/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/output.py` & `arclet-alconna-1.7.8/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.8/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.8/src/arclet/alconna/typing.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/tests/analyser_test.py` & `arclet-alconna-1.7.8/tests/analyser_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/tests/args_test.py` & `arclet-alconna-1.7.8/tests/args_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/tests/base_test.py` & `arclet-alconna-1.7.8/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/tests/components_test.py` & `arclet-alconna-1.7.8/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/tests/config_test.py` & `arclet-alconna-1.7.8/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/tests/core_test.py` & `arclet-alconna-1.7.8/tests/core_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.7/PKG-INFO` & `arclet-alconna-1.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.7
+Version: 1.7.8
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -43,20 +43,19 @@
 
 ## Installation
 
 pip
 ```shell
 $ pip install --upgrade arclet-alconna
 $ pip install --upgrade arclet-alconna[full]
-$ pip install --upgrade arclet-alconna[all]
 ```
 
 ## Documentation
 
-Official Document : [👉Link](https://arcletproject.github.io/docs/alconna/tutorial)
+Official Document : [👉Link](https://arclet.top/docs/tutorial/alconna)
 
 Relevant Document : [📚Docs](https://graiax.cn/guide/message_parser/alconna.html)
 
 ## A Simple Example
 
 ```python
 from arclet.alconna import Alconna, Option, Subcommand, Args
```

