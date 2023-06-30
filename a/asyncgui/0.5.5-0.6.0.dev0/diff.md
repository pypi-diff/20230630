# Comparing `tmp/asyncgui-0.5.5.tar.gz` & `tmp/asyncgui-0.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncgui-0.5.5.tar", max compression
+gzip compressed data, was "asyncgui-0.6.0.dev0.tar", max compression
```

## Comparing `asyncgui-0.5.5.tar` & `asyncgui-0.6.0.dev0.tar`

### file list

```diff
@@ -1,12 +1,5 @@
--rw-r--r--   0        0        0     1055 2022-08-15 00:42:01.490120 asyncgui-0.5.5/LICENSE
--rw-r--r--   0        0        0     4251 2022-08-17 13:02:13.508361 asyncgui-0.5.5/README.md
--rw-r--r--   0        0        0       47 2022-08-15 00:42:01.490120 asyncgui-0.5.5/asyncgui/__init__.py
--rw-r--r--   0        0        0     9222 2022-08-17 00:57:40.674534 asyncgui-0.5.5/asyncgui/_core.py
--rw-r--r--   0        0        0     2082 2022-08-17 13:02:13.500361 asyncgui-0.5.5/asyncgui/_multierror.py
--rw-r--r--   0        0        0      314 2022-08-17 11:19:54.159182 asyncgui-0.5.5/asyncgui/exceptions.py
--rw-r--r--   0        0        0     9777 2022-08-17 13:02:13.496361 asyncgui-0.5.5/asyncgui/structured_concurrency.py
--rw-r--r--   0        0        0       26 2022-08-15 00:42:01.490120 asyncgui-0.5.5/asyncgui/testing/__init__.py
--rw-r--r--   0        0        0      318 2022-08-15 00:42:01.490120 asyncgui-0.5.5/asyncgui/testing/_scheduler.py
--rw-r--r--   0        0        0      989 2022-08-17 13:02:13.516361 asyncgui-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     4995 2022-08-17 13:04:14.265717 asyncgui-0.5.5/setup.py
--rw-r--r--   0        0        0     5177 2022-08-17 13:04:14.266407 asyncgui-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-28 01:11:59.000000 asyncgui-0.6.0.dev0/LICENSE
+-rw-r--r--   0        0        0     4268 2023-06-30 01:07:19.587907 asyncgui-0.6.0.dev0/README.md
+-rw-r--r--   0        0        0     1213 2023-06-30 01:07:19.587907 asyncgui-0.6.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    21326 2023-06-30 01:07:19.587907 asyncgui-0.6.0.dev0/src/asyncgui.py
+-rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 asyncgui-0.6.0.dev0/PKG-INFO
```

### Comparing `asyncgui-0.5.5/LICENSE` & `asyncgui-0.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncgui-0.5.5/README.md` & `asyncgui-0.6.0.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # AsyncGui
 
-A thin layer that helps to build an async/await-based api using a callback-based api.
+A thin layer that helps to build async/await-based apis using callback-based apis.
 
 ## How to use
 
-Despite its name, `asyncgui` has nothing to do with gui.
-You can wrap any kind of callback-based api in it.
+Despite its name, the application of `asyncgui` is **not** limited to gui programs.
+You can wrap any kind of callback-based apis in it.
 The simplest example of it would be [sched](https://docs.python.org/3/library/sched.html),
 whose the whole feature is a timer.
 All you need is just few lines of code:
 
 ```python
 import types
 import sched
 import asyncgui
 
 s = sched.scheduler()
 
-# wrapping 'scheduler.enter()' takes only three lines
+# Wrapping 'scheduler.enter()' only takes three lines of code
 @types.coroutine
-def sleep(duration):
-    yield lambda step_coro: s.enter(duration, 10, step_coro)
+def sleep(duration, *, priority=10):
+    yield lambda task: s.enter(duration, priority, task._step)
 
 
 async def main():
     print('A')
     await sleep(1)  # Now you can sleep in an async-manner
     print('B')
     await sleep(1)
@@ -46,19 +46,18 @@
 async def print_letters():
     for c in "ABCDE":
         await sleep(.1)
         print(c)
 
 
 async def main():
-    from asyncgui.structured_concurrency import or_
     # Let print_letters() and print_numbers() race.
-    # As soon as one of them finishes, the other one gets cancelled.
-    tasks = await or_(print_letters(), print_numbers())
-    if tasks[0].done:
+    # As soon as any of them finishes, the other one gets cancelled.
+    tasks = await asyncgui.wait_any(print_letters(), print_numbers())
+    if tasks[0].finished:
         print("print_letters() won")
     else:
         print("print_numbers() won")
     print('main end')
 ```
 
 ```
@@ -74,37 +73,37 @@
 print_letters() won
 main end
 ```
 
 ## Why not asyncio ?
 
 The above example may not attract you because you can just replace `sched` with [asyncio](https://docs.python.org/3/library/asyncio.html) or [Trio](https://trio.readthedocs.io/en/stable/),
-and can use thier sleep function (`asyncio.sleep` and `trio.sleep`).
+and can use thier respective sleep function (`asyncio.sleep` and `trio.sleep`).
 But in a read-world situation, that might not be an option:
 Kivy required [massive changes](https://github.com/kivy/kivy/pull/6368) in order to adapt to `asyncio` and `Trio`,
 [asyncio-tkinter](https://github.com/fluentpython/asyncio-tkinter)'s codebase is quite big as well.
 
 The reason they needed lots of work is that they had to merge two event-loops into one.
 One is from the gui libraries. The other one is from async libraries.
 You cannot just simply run multiple event-loops simultaneously in one thread.
 
 On the other hand, `asyncgui` doesn't require a lot of work as shown above **because it doesn't have an event-loop**.
-`asyncgui` and a library who has an event-loop can live in the same thread seemlessly because of it.
+`asyncgui` and a library that has an event-loop can live in the same thread seamlessly because of it.
 
 ## So, is asyncgui superior to asyncio ?
 
 No, it is not.
 For `asyncgui`, many features that exist in `asyncio` are either impossible or hard to implement because of the lack of event-loop.
-The implementation of those features needs to be specific to the event-loop you are using.
+The implementation of those features needs to be specific to each event-loop.
 You've already witnessed one, the `sleep`.
 
 ## asyncgui is not usefull then.
 
 There is at least one situation that `asyncgui` shines.
-When you are creating a gui app, you probably want the app to quickly react to the gui events, like pressing a button.
+When you are creating a gui app, you probably want the app to quickly react to its gui events, like pressing a button.
 This is problematic for `asyncio` because it cannot immediately start/resume a task.
 It can schedule a task to *eventually* start/resume but not *immediate*,
 which causes to [spill gui events](https://github.com/gottadiveintopython/asynckivy/blob/main/examples/misc/why_asyncio_is_not_suitable_for_handling_touch_events.py).
 As a result, you need to use callback-based apis for that, and thus you cannot fully receive the benefits of async/await.
 
 If you use `asyncgui`, that never happens because:
 
@@ -121,16 +120,16 @@
 ```text
 poetry add asyncgui@~0.5
 pip install "asyncgui>=0.5,<0.6"
 ```
 
 ## Tested on
 
-- CPython 3.7
 - CPython 3.8
 - CPython 3.9
 - CPython 3.10
+- CPython 3.11
 
 ## Async-libraries who relies on this
 
 - [asynckivy](https://github.com/gottadiveintopython/asynckivy)
 - [asynctkinter](https://github.com/gottadiveintopython/asynctkinter)
```

### Comparing `asyncgui-0.5.5/pyproject.toml` & `asyncgui-0.6.0.dev0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 [tool.poetry]
 name = "asyncgui"
-version = "0.5.5"
+version = "0.6.0.dev0"
 description = "async/await without event-loop"
 authors = ["Nattōsai Mitō <flow4re2c@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/gottadiveintopython/asyncgui'
 homepage = 'https://github.com/gottadiveintopython/asyncgui'
 keywords = ['async', ]
 classifiers=[
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: MIT License',
     'Intended Audience :: Developers',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Software Development :: Libraries',
     'Operating System :: OS Independent',
 ]
+packages = [
+    { include = "asyncgui.py", from = "src" },
+]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
+exceptiongroup = {version = "^1.0.4", python = "<3.11"}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.0.1"
 flake8 = "^4.0.1"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+xfail_strict = true
+addopts = "--maxfail=4 --strict-markers"
```

### Comparing `asyncgui-0.5.5/PKG-INFO` & `asyncgui-0.6.0.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 Metadata-Version: 2.1
 Name: asyncgui
-Version: 0.5.5
+Version: 0.6.0.dev0
 Summary: async/await without event-loop
 Home-page: https://github.com/gottadiveintopython/asyncgui
 License: MIT
 Keywords: async
 Author: Nattōsai Mitō
 Author-email: flow4re2c@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: exceptiongroup (>=1.0.4,<2.0.0) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/gottadiveintopython/asyncgui
 Description-Content-Type: text/markdown
 
 # AsyncGui
 
-A thin layer that helps to build an async/await-based api using a callback-based api.
+A thin layer that helps to build async/await-based apis using callback-based apis.
 
 ## How to use
 
-Despite its name, `asyncgui` has nothing to do with gui.
-You can wrap any kind of callback-based api in it.
+Despite its name, the application of `asyncgui` is **not** limited to gui programs.
+You can wrap any kind of callback-based apis in it.
 The simplest example of it would be [sched](https://docs.python.org/3/library/sched.html),
 whose the whole feature is a timer.
 All you need is just few lines of code:
 
 ```python
 import types
 import sched
 import asyncgui
 
 s = sched.scheduler()
 
-# wrapping 'scheduler.enter()' takes only three lines
+# Wrapping 'scheduler.enter()' only takes three lines of code
 @types.coroutine
-def sleep(duration):
-    yield lambda step_coro: s.enter(duration, 10, step_coro)
+def sleep(duration, *, priority=10):
+    yield lambda task: s.enter(duration, priority, task._step)
 
 
 async def main():
     print('A')
     await sleep(1)  # Now you can sleep in an async-manner
     print('B')
     await sleep(1)
@@ -70,19 +71,18 @@
 async def print_letters():
     for c in "ABCDE":
         await sleep(.1)
         print(c)
 
 
 async def main():
-    from asyncgui.structured_concurrency import or_
     # Let print_letters() and print_numbers() race.
-    # As soon as one of them finishes, the other one gets cancelled.
-    tasks = await or_(print_letters(), print_numbers())
-    if tasks[0].done:
+    # As soon as any of them finishes, the other one gets cancelled.
+    tasks = await asyncgui.wait_any(print_letters(), print_numbers())
+    if tasks[0].finished:
         print("print_letters() won")
     else:
         print("print_numbers() won")
     print('main end')
 ```
 
 ```
@@ -98,37 +98,37 @@
 print_letters() won
 main end
 ```
 
 ## Why not asyncio ?
 
 The above example may not attract you because you can just replace `sched` with [asyncio](https://docs.python.org/3/library/asyncio.html) or [Trio](https://trio.readthedocs.io/en/stable/),
-and can use thier sleep function (`asyncio.sleep` and `trio.sleep`).
+and can use thier respective sleep function (`asyncio.sleep` and `trio.sleep`).
 But in a read-world situation, that might not be an option:
 Kivy required [massive changes](https://github.com/kivy/kivy/pull/6368) in order to adapt to `asyncio` and `Trio`,
 [asyncio-tkinter](https://github.com/fluentpython/asyncio-tkinter)'s codebase is quite big as well.
 
 The reason they needed lots of work is that they had to merge two event-loops into one.
 One is from the gui libraries. The other one is from async libraries.
 You cannot just simply run multiple event-loops simultaneously in one thread.
 
 On the other hand, `asyncgui` doesn't require a lot of work as shown above **because it doesn't have an event-loop**.
-`asyncgui` and a library who has an event-loop can live in the same thread seemlessly because of it.
+`asyncgui` and a library that has an event-loop can live in the same thread seamlessly because of it.
 
 ## So, is asyncgui superior to asyncio ?
 
 No, it is not.
 For `asyncgui`, many features that exist in `asyncio` are either impossible or hard to implement because of the lack of event-loop.
-The implementation of those features needs to be specific to the event-loop you are using.
+The implementation of those features needs to be specific to each event-loop.
 You've already witnessed one, the `sleep`.
 
 ## asyncgui is not usefull then.
 
 There is at least one situation that `asyncgui` shines.
-When you are creating a gui app, you probably want the app to quickly react to the gui events, like pressing a button.
+When you are creating a gui app, you probably want the app to quickly react to its gui events, like pressing a button.
 This is problematic for `asyncio` because it cannot immediately start/resume a task.
 It can schedule a task to *eventually* start/resume but not *immediate*,
 which causes to [spill gui events](https://github.com/gottadiveintopython/asynckivy/blob/main/examples/misc/why_asyncio_is_not_suitable_for_handling_touch_events.py).
 As a result, you need to use callback-based apis for that, and thus you cannot fully receive the benefits of async/await.
 
 If you use `asyncgui`, that never happens because:
 
@@ -145,17 +145,17 @@
 ```text
 poetry add asyncgui@~0.5
 pip install "asyncgui>=0.5,<0.6"
 ```
 
 ## Tested on
 
-- CPython 3.7
 - CPython 3.8
 - CPython 3.9
 - CPython 3.10
+- CPython 3.11
 
 ## Async-libraries who relies on this
 
 - [asynckivy](https://github.com/gottadiveintopython/asynckivy)
 - [asynctkinter](https://github.com/gottadiveintopython/asynctkinter)
```

