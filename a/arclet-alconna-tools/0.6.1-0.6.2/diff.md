# Comparing `tmp/arclet-alconna-tools-0.6.1.tar.gz` & `tmp/arclet-alconna-tools-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-tools-0.6.1.tar", last modified: Sun May 28 14:06:35 2023, max compression
+gzip compressed data, was "arclet-alconna-tools-0.6.2.tar", last modified: Fri Jun 30 15:23:55 2023, max compression
```

## Comparing `arclet-alconna-tools-0.6.1.tar` & `arclet-alconna-tools-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.1/LICENSE
--rw-r--r--   0        0        0     1075 2023-05-28 13:57:51.253672 arclet-alconna-tools-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      749 2023-05-10 16:28:11.249182 arclet-alconna-tools-0.6.1/README.md
--rw-r--r--   0        0        0      387 2023-05-10 14:13:40.054086 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/actions.py
--rw-r--r--   0        0        0      866 2023-05-07 05:15:13.324038 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/checker.py
--rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/config.py
--rw-r--r--   0        0        0    30725 2023-05-28 13:55:54.267542 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/construct.py
--rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/debug.py
--rw-r--r--   0        0        0    17620 2023-05-10 14:36:13.901208 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/formatter.py
--rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/.config.json
--rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/en-US.json
--rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/zh-CN.json
--rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/pattern.py
--rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1075 2023-06-30 14:54:04.331377 arclet-alconna-tools-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      749 2023-05-10 16:28:11.249182 arclet-alconna-tools-0.6.2/README.md
+-rw-r--r--   0        0        0      387 2023-05-10 14:13:40.054086 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/actions.py
+-rw-r--r--   0        0        0      866 2023-05-07 05:15:13.324038 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/checker.py
+-rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/config.py
+-rw-r--r--   0        0        0    32763 2023-06-30 15:22:56.421449 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/construct.py
+-rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/debug.py
+-rw-r--r--   0        0        0    17620 2023-05-10 14:36:13.901208 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/formatter.py
+-rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/.config.json
+-rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/en-US.json
+-rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/zh-CN.json
+-rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/pattern.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.2/PKG-INFO
```

### Comparing `arclet-alconna-tools-0.6.1/LICENSE` & `arclet-alconna-tools-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.1/pyproject.toml` & `arclet-alconna-tools-0.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "arclet-alconna-tools"
-version = "0.6.1"
+version = "0.6.2"
 description = "Builtin Tools for Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nepattern<0.6.0, >=0.5.8",
-    "arclet-alconna>=1.7.7",
+    "arclet-alconna>=1.7.8",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `arclet-alconna-tools-0.6.1/README.md` & `arclet-alconna-tools-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/actions.py` & `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/actions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/checker.py` & `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/checker.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/construct.py` & `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/construct.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,20 @@
     Any,
     Callable,
     Dict,
     Generic,
     List,
     Optional,
     Type,
+    Tuple,
     TypeVar,
     Union,
     cast,
     TypedDict,
+    overload
 )
 
 
 from arclet.alconna.args import ArgFlag, Args, TAValue, Arg
 from arclet.alconna.action import Action
 from arclet.alconna.arparma import Arparma, ArparmaBehavior
 from arclet.alconna.base import Option, Subcommand
@@ -505,16 +507,16 @@
     description: NotRequired[str]
     # get_subcommand: NotRequired[bool]
     namespace: NotRequired[str]
     command: NotRequired[str]
 
 config_keys = ("prefixes", "raise_exception", "description", "namespace", "command")
 
-def visit_config(obj: Any):
-    result = {}
+def visit_config(obj: Any, base: Optional[MountConfig] = None) -> MountConfig:
+    result: MountConfig = base or {}
     if isinstance(obj, (FunctionType, MethodType)):
         codes, _ = inspect.getsourcelines(obj)
         _get_config = False
         _start_indent = 0
         for line in codes:
             indent = len(line) - len(line.lstrip())
             if line.lstrip().startswith("class") and line.lstrip().rstrip(
@@ -526,34 +528,39 @@
             if _get_config:
                 if indent == _start_indent:
                     break
                 if line.lstrip().startswith("def"):
                     continue
                 _contents = re.split(r"\s*=\s*", line.strip())
                 if len(_contents) == 2 and _contents[0] in config_keys:
-                    result[_contents[0]] = eval(_contents[1])
-    elif config := inspect.getmembers(
+                    result[_contents[0]] = eval(_contents[1])  # type: ignore
+    elif kss := inspect.getmembers(
         obj, lambda x: inspect.isclass(x) and x.__name__.endswith("Config")
     ):
-        config = config[0][1]
-        result = {k: getattr(config, k) for k in config_keys if k in dir(config)}
+        ks = kss[0][1]
+        result.update({k: getattr(ks, k) for k in config_keys if k in dir(ks)})
     return result
 
 
 @dataclass(unsafe_hash=True)
 class CallbackHandler(ArparmaBehavior):
     main_call: Optional[Callable] = field(default=None)
     options: Dict[str, Callable] = field(default_factory=dict, hash=False)
+    results: Dict[str, Any] = field(default_factory=dict, hash=False)
+
+    def before_operate(self, interface: Arparma):
+        super().before_operate(interface)
+        self.results.clear()
 
     def operate(self, interface: Arparma):
         if call := self.main_call:
             call(**interface.main_args)
         for path, action in self.options.items():
             if (d := interface.query(path, None)) is not None:
-                action(**d)
+                self.results[action.__qualname__] = action(**d)
 
 
 class SubClassMounter(Subcommand):
 
     def _get_instance(self):
         return self.instance
 
@@ -609,97 +616,117 @@
             config.get("command", mount_cls.__name__),
             main_args,
             *_options,
             help_text=config.get("description", main_help_text),
         )
 
 
-class FuncMounter(Alconna):
+class FuncMounter(Alconna[TDC], Generic[T, TDC]):
+    target: Callable[..., T]
+
     def __init__(
-        self, func: Union[FunctionType, MethodType], config: Optional[MountConfig] = None
+        self, func: Callable[..., T], config: Optional[MountConfig] = None
     ):
-        config = config or visit_config(func)
+        config = visit_config(func, config)
         func_name = func.__name__
         if func_name.startswith("_"):
             raise ValueError(lang.require("tools", "construct.func_name_error"))
         _args, method = Args.from_callable(func)
         if method and isinstance(func, MethodType):
             self.instance = func.__self__
             func = cast(FunctionType, partial(func, self.instance))
         super(FuncMounter, self).__init__(
-            config.get("headers", []),
+            config.get("prefixes", []),
             config.get("command", func_name),
             _args,
             meta=CommandMeta(
                 description=config.get("description", func.__doc__ or func_name),
                 raise_exception=config.get("raise_exception", True),
             ),
             namespace=config.get("namespace", None),
         )
+        self.target = func
         self.bind()(func)
 
+    def exec(self, message: TDC) -> Tuple[Arparma[TDC], Optional[T]]:
+        try:
+            arp = self._parse(message)
+        except NullMessage as e:
+            if self.meta.raise_exception:
+                raise e
+            return Arparma(self.path, message, False, error_info=e), None
+        if arp.matched:
+            arp = arp.execute(self.behaviors)
+            return arp, arp.call(self.target)
+        return arp, None
+
 class ModuleMounter(Alconna):
-    def __init__(self, module: ModuleType, config: Optional[dict] = None):
+    def __init__(self, module: ModuleType, config: Optional[MountConfig] = None):
         self.mount_cls = module.__class__
         self.instance = module
-        config = config or visit_config(module)
+        config = config or visit_config(module, config)
         _options = []
         members = inspect.getmembers(
             module, lambda x: inspect.isfunction(x) or inspect.ismethod(x)
         )
-        behavior = CallbackHandler()
+        self.cb_behavior = CallbackHandler()
         for name, func in members:
             if name.startswith("_") or func.__name__.startswith("_"):
                 continue
             help_text = func.__doc__ or name
             _opt_args, method = Args.from_callable(func)
             if method:
                 func = partial(func, func.__self__)
             _options.append(
                 Option(
                     name, args=_opt_args, help_text=help_text
                 )
             )
-            behavior.options[f"options.{name}.args"] = func
+            self.cb_behavior.options[f"options.{name}.args"] = func
         _options.extend(
-            SubClassMounter(cls, behavior, "")
+            SubClassMounter(cls, self.cb_behavior, "")
             for name, cls in inspect.getmembers(module, inspect.isclass)
             if not name.startswith("_") and not name.endswith("Config")
         )
         super().__init__(
             config.get("command", module.__name__),
-            config.get("headers", []),
+            config.get("prefixes", []),
             *_options,
             namespace=config.get("namespace", None),
             meta=CommandMeta(
                 description=config.get(
                     "description", module.__doc__ or module.__name__
                 ),
                 raise_exception=config.get("raise_exception", True),
             ),
-            behaviors=[behavior],
+            behaviors=[self.cb_behavior],
         )
 
+    def get_result(self, func: Callable):
+        return self.cb_behavior.results.get(func.__qualname__)
 
-class ClassMounter(Alconna):
 
-    def _get_instance(self):
+class ClassMounter(Alconna[TDC], Generic[T, TDC]):
+    mount_cls: Type[T]
+    instance: T
+
+    def _get_instance(self) -> T:
         return self.instance
 
     def _inject_instance(self, target: Callable):
         @wraps(target)
         def wrapper(*args, **kwargs):
             return target(self._get_instance(), *args, **kwargs)
 
         return wrapper
 
-    def __init__(self, mount_cls: Type, config: Optional[MountConfig] = None):
+    def __init__(self, mount_cls: Type[T], config: Optional[MountConfig] = None):
         self.mount_cls = mount_cls
         self.instance: mount_cls = None
-        config = config or visit_config(mount_cls)
+        config = config or visit_config(mount_cls, config)
         members = inspect.getmembers(
             mount_cls, lambda x: inspect.isfunction(x) or inspect.ismethod(x)
         )
 
         _options = []
         main_help_text = (
             mount_cls.__doc__ or mount_cls.__init__.__doc__ or mount_cls.__name__
@@ -713,99 +740,130 @@
                 for key, value in kwargs.items():
                     self.args[key].field.default = value
             else:
                 for k, v in kwargs.items():
                     setattr(self.instance, k, v)
 
 
-        behavior = CallbackHandler(main_call=_main_func)
+        self.cb_behavior = CallbackHandler(main_call=_main_func)
         for name, func in filter(lambda x: not x[0].startswith("_"), members):
             help_text = func.__doc__ or name
             _opt_args, method = Args.from_callable(func)
             if method:
                 func = self._inject_instance(func)
             _options.append(
                 Option(name, _opt_args, help_text=help_text)
             )
-            behavior.options[f"options.{name}.args"] = func
+            self.cb_behavior.options[f"options.{name}.args"] = func
 
         _options.extend(
-            SubClassMounter(cls, behavior, "")
+            SubClassMounter(cls, self.cb_behavior, "")
             for name, cls in inspect.getmembers(mount_cls, inspect.isclass)
             if not name.startswith("_") and not name.endswith("Config")
         )
         super().__init__(
             config.get("command", mount_cls.__name__),
             main_args,
-            config.get("headers", []),
+            config.get("prefixes", []),
             *_options,
             namespace=config.get("namespace", None),
             meta=CommandMeta(
                 description=config.get("description", main_help_text),
                 raise_exception=config.get("raise_exception", True),
             ),
-            behaviors=[behavior],
+            behaviors=[self.cb_behavior],
         )
 
+    def get_result(self, func: Callable):
+        return self.cb_behavior.results.get(func.__qualname__)
+
+class ObjectMounter(Alconna[TDC], Generic[T, TDC]):
+    mount_cls: Type[T]
+    instance: T
 
-class ObjectMounter(Alconna):
-    def __init__(self, obj: object, config: Optional[dict] = None):
+    def __init__(self, obj: T, config: Optional[dict] = None):
         self.mount_cls = type(obj)
         self.instance = obj
         config = config or visit_config(obj)
         obj_name = obj.__class__.__name__
         members = inspect.getmembers(
             obj, lambda x: inspect.isfunction(x) or inspect.ismethod(x)
         )
         _options = []
         main_help_text = obj.__doc__ or obj.__init__.__doc__ or obj_name
 
         def _main_func(**kwargs):
             for k, v in kwargs.items():
                 setattr(self.instance, k, v)
 
-        behavior = CallbackHandler(main_call=_main_func)
+        self.cb_behavior = CallbackHandler(main_call=_main_func)
 
         for name, func in filter(lambda x: not x[0].startswith("_"), members):
             help_text = func.__doc__ or name
             _opt_args, _ = Args.from_callable(func)
             _options.append(
                 Option(
                     name, args=_opt_args, help_text=help_text
                 )
             )
-            behavior.options[f"options.{name}.args"] = func
+            self.cb_behavior.options[f"options.{name}.args"] = func
 
         _options.extend(
-            SubClassMounter(cls, behavior, "")
+            SubClassMounter(cls, self.cb_behavior, "")
             for name, cls in inspect.getmembers(obj, inspect.isclass)
             if not name.startswith("_")
         )
         main_args = Args.from_callable(obj.__init__)[0]
         for arg in main_args.argument:
             if hasattr(self.instance, arg.name):
                 arg.field.default = getattr(self.instance, arg.name)
 
         super().__init__(
             config.get("command", obj_name),
             main_args,
-            config.get("headers", []),
+            config.get("prefixes", []),
             *_options,
             meta=CommandMeta(
                 description=config.get("description", main_help_text),
                 raise_exception=config.get("raise_exception", True),
             ),
-            behaviors=[behavior],
+            behaviors=[self.cb_behavior],
             namespace=config.get("namespace", None),
         )
 
+    def get_result(self, func: Callable):
+        return self.cb_behavior.results.get(func.__qualname__)
+
+@overload
+def _from_object(
+    *, command: Optional[TDC] = None, config: Optional[MountConfig] = None,
+) -> ModuleMounter:
+    ...
+
+@overload
+def _from_object(
+    target: Type[T], command: Optional[TDC] = None, config: Optional[MountConfig] = None,
+) -> ClassMounter[T, TDC]:
+    ...
+
+@overload
+def _from_object(
+    target: T, command: Optional[TDC] = None, config: Optional[MountConfig] = None,
+) -> ObjectMounter[T, TDC]:
+    ...
+
+@overload
+def _from_object(
+    target: Callable[..., T], command: Optional[TDC] = None, config: Optional[MountConfig] = None,
+) -> FuncMounter[T, TDC]:
+    ...
 
 def _from_object(
-    target: Optional[Union[Type, object, FunctionType, MethodType, ModuleType]] = None,
-    command: Optional[str] = None,
+    target: Optional[Union[Type[T], T, Callable[..., T], ModuleType]] = None,
+    command: Optional[TDC] = None,
     config: Optional[MountConfig] = None,
 ):
     """
     通过解析传入的对象，生成 Alconna 实例的方法, 或者说是Fire-like的方式
 
     Examples:
```

### Comparing `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/debug.py` & `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/debug.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/formatter.py` & `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/en-US.json` & `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/zh-CN.json` & `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/pattern.py` & `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.1/PKG-INFO` & `arclet-alconna-tools-0.6.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: Builtin Tools for Alconna
 License: MIT
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Alconna Tools
```

