# Comparing `tmp/benimang-0.2.2.tar.gz` & `tmp/benimang-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.2.2.tar", last modified: Sun Apr 23 11:00:56 2023, max compression
+gzip compressed data, was "benimang-0.3.5.tar", last modified: Fri Jun 30 02:16:19 2023, max compression
```

## Comparing `benimang-0.2.2.tar` & `benimang-0.3.5.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 11:00:56.717546 benimang-0.2.2/
--rw-rw-rw-   0        0        0       29 2022-09-20 03:37:30.000000 benimang-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      258 2023-04-23 11:00:56.717546 benimang-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-09-20 03:37:30.000000 benimang-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 11:00:56.710546 benimang-0.2.2/beni/
--rw-rw-rw-   0        0        0        0 2022-09-20 06:33:04.000000 benimang-0.2.2/beni/__init__.py
--rw-rw-rw-   0        0        0     6223 2022-09-20 06:33:43.000000 benimang-0.2.2/beni/bbyte.py
--rw-rw-rw-   0        0        0     6312 2023-04-20 08:42:14.000000 benimang-0.2.2/beni/bcache.py
--rw-rw-rw-   0        0        0    10207 2023-04-23 09:51:57.000000 benimang-0.2.2/beni/bcmd.py
--rw-rw-rw-   0        0        0     1906 2022-09-20 03:37:31.000000 benimang-0.2.2/beni/bcolor.py
--rw-rw-rw-   0        0        0     2460 2023-04-20 08:42:43.000000 benimang-0.2.2/beni/bexecute.py
--rw-rw-rw-   0        0        0     2139 2023-04-21 01:32:03.000000 benimang-0.2.2/beni/bfile.py
--rw-rw-rw-   0        0        0     5009 2023-04-23 08:32:41.000000 benimang-0.2.2/beni/bfunc.py
--rw-rw-rw-   0        0        0     5855 2023-04-21 01:32:29.000000 benimang-0.2.2/beni/bhttp.py
--rw-rw-rw-   0        0        0     2310 2023-04-23 08:04:15.000000 benimang-0.2.2/beni/binput.py
--rw-rw-rw-   0        0        0     5653 2023-04-20 09:28:08.000000 benimang-0.2.2/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-04-21 01:58:47.000000 benimang-0.2.2/beni/blog.py
--rw-rw-rw-   0        0        0     5664 2023-04-23 10:53:28.000000 benimang-0.2.2/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2023-04-21 01:24:20.000000 benimang-0.2.2/beni/bplaywright.py
--rw-rw-rw-   0        0        0      841 2023-02-27 04:00:30.000000 benimang-0.2.2/beni/bprogress.py
--rw-rw-rw-   0        0        0     3845 2023-04-23 09:28:40.000000 benimang-0.2.2/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10553 2023-04-21 01:31:13.000000 benimang-0.2.2/beni/bsqlite.py
--rw-rw-rw-   0        0        0      859 2023-04-21 02:20:59.000000 benimang-0.2.2/beni/bstorage.py
--rw-rw-rw-   0        0        0     1974 2022-11-09 09:34:30.000000 benimang-0.2.2/beni/btable.py
--rw-rw-rw-   0        0        0     2941 2023-04-20 08:53:07.000000 benimang-0.2.2/beni/btask.py
--rw-rw-rw-   0        0        0     1574 2023-02-28 02:25:16.000000 benimang-0.2.2/beni/btime.py
--rw-rw-rw-   0        0        0     2397 2023-04-23 07:11:54.000000 benimang-0.2.2/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-04-23 11:00:56.715548 benimang-0.2.2/benimang.egg-info/
--rw-rw-rw-   0        0        0      258 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       93 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 11:00:56.000000 benimang-0.2.2/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-04-23 10:55:35.000000 benimang-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 11:00:56.717546 benimang-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 11:00:56.716546 benimang-0.2.2/test/
--rw-rw-rw-   0        0        0      638 2023-02-24 01:48:48.000000 benimang-0.2.2/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:16:19.860579 benimang-0.3.5/
+-rw-rw-rw-   0        0        0       29 2023-05-30 09:18:28.000000 benimang-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      258 2023-06-30 02:16:19.859580 benimang-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 02:16:19.852579 benimang-0.3.5/beni/
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.5/beni/__init__.py
+-rw-rw-rw-   0        0        0     6350 2023-06-29 02:15:26.000000 benimang-0.3.5/beni/bbyte.py
+-rw-rw-rw-   0        0        0     5783 2023-06-29 07:11:14.000000 benimang-0.3.5/beni/bcache.py
+-rw-rw-rw-   0        0        0    11460 2023-06-29 07:06:28.000000 benimang-0.3.5/beni/bcmd.py
+-rw-rw-rw-   0        0        0     1941 2023-06-09 08:30:18.000000 benimang-0.3.5/beni/bcolor.py
+-rw-rw-rw-   0        0        0      436 2023-06-29 07:09:07.000000 benimang-0.3.5/beni/bdefine.py
+-rw-rw-rw-   0        0        0     2423 2023-06-26 06:18:37.000000 benimang-0.3.5/beni/bexecute.py
+-rw-rw-rw-   0        0        0     1908 2023-06-29 01:45:33.000000 benimang-0.3.5/beni/bfile.py
+-rw-rw-rw-   0        0        0     4482 2023-06-30 02:05:52.000000 benimang-0.3.5/beni/bfunc.py
+-rw-rw-rw-   0        0        0     1029 2023-06-28 03:38:59.000000 benimang-0.3.5/beni/bhash.py
+-rw-rw-rw-   0        0        0     5745 2023-06-26 09:08:25.000000 benimang-0.3.5/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2583 2023-06-13 01:57:12.000000 benimang-0.3.5/beni/binput.py
+-rw-rw-rw-   0        0        0     5708 2023-06-30 02:08:08.000000 benimang-0.3.5/beni/block.py
+-rw-rw-rw-   0        0        0     3989 2023-06-29 01:25:39.000000 benimang-0.3.5/beni/blog.py
+-rw-rw-rw-   0        0        0     5790 2023-06-29 01:32:58.000000 benimang-0.3.5/beni/bpath.py
+-rw-rw-rw-   0        0        0     2450 2023-06-29 01:26:10.000000 benimang-0.3.5/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1058 2023-06-27 03:17:47.000000 benimang-0.3.5/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3373 2023-06-29 01:32:58.000000 benimang-0.3.5/beni/bqiniu.py
+-rw-rw-rw-   0        0        0     9866 2023-06-29 01:31:14.000000 benimang-0.3.5/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      759 2023-06-29 01:45:35.000000 benimang-0.3.5/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1981 2023-06-26 02:57:46.000000 benimang-0.3.5/beni/btable.py
+-rw-rw-rw-   0        0        0     4987 2023-06-29 01:28:43.000000 benimang-0.3.5/beni/btask.py
+-rw-rw-rw-   0        0        0     1378 2023-06-29 07:10:32.000000 benimang-0.3.5/beni/btime.py
+-rw-rw-rw-   0        0        0      324 2023-06-30 02:01:04.000000 benimang-0.3.5/beni/btype.py
+-rw-rw-rw-   0        0        0     2392 2023-06-29 02:21:02.000000 benimang-0.3.5/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:16:19.857581 benimang-0.3.5/benimang.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-06-30 02:09:09.000000 benimang-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 02:16:19.860579 benimang-0.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 02:16:19.858580 benimang-0.3.5/test/
+-rw-rw-rw-   0        0        0      638 2023-05-30 09:18:28.000000 benimang-0.3.5/test/test_sample.py
```

### Comparing `benimang-0.2.2/beni/bcmd.py` & `benimang-0.3.5/beni/bcmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import nest_asyncio
 import pyperclip
 import typer
 from colorama import Fore
 
 from beni import bcolor, bexecute, bfile, binput, bpath
+from beni.btype import Null
 
 _app = typer.Typer()
 
 
 def main():
     nest_asyncio.apply()
     _app()
@@ -31,61 +32,55 @@
 
 
 # ------------------------------------------------------------------------
 
 
 @_app.command('time')
 def showtime(
-    value: str = typer.Argument('', help='时间戳（支持整形和浮点型）或日期（格式: 2021-11-23）', show_default=False, metavar='[Timestamp or Date]'),
+    value1: str = typer.Argument('', help='时间戳（整形或浮点型）或日期（格式: 2021-11-23）', show_default=False, metavar='[Timestamp or Date]'),
     value2: str = typer.Argument('', help='时间（格式: 09:20:20），只有第一个参数为日期才有意义', show_default=False, metavar='[Time]')
 ):
     '''
-    格式化时间戳
-
-    beni showtime
-
-    beni showtime 1632412740
-
-    beni showtime 1632412740.1234
-
-    beni showtime 2021-9-23
-
-    beni showtime 2021-9-23 09:47:00
+    格式化时间戳\n
+    beni time\n
+    beni time 1632412740\n
+    beni time 1632412740.1234\n
+    beni time 2021-9-23\n
+    beni time 2021-9-23 09:47:00\n
     '''
-
-    timestamp: float | None = None
-    if not value:
+    timestamp: float = Null
+    if not value1:
         timestamp = time.time()
     else:
         try:
-            timestamp = float(value)
+            timestamp = float(value1)
         except:
             try:
                 if value2:
-                    timestamp = Datetime.strptime(f'{value} {value2}', '%Y-%m-%d %H:%M:%S').timestamp()
+                    timestamp = Datetime.strptime(f'{value1} {value2}', '%Y-%m-%d %H:%M:%S').timestamp()
                 else:
-                    timestamp = Datetime.strptime(f'{value}', '%Y-%m-%d').timestamp()
+                    timestamp = Datetime.strptime(f'{value1}', '%Y-%m-%d').timestamp()
             except:
                 pass
 
     if timestamp is None:
         color = typer.colors.BRIGHT_RED
         typer.secho('参数无效', fg=color)
         typer.secho('\n可使用格式: ', fg=color)
-        msgAry = str(showtime.__doc__).strip().replace('\n\n', '\n').split('\n')[1:]
-        msgAry = [x.strip() for x in msgAry]
-        typer.secho('\n'.join(msgAry), fg=color)
+        msg_ary = str(showtime.__doc__).strip().replace('\n\n', '\n').split('\n')[1:]
+        msg_ary = [x.strip() for x in msg_ary]
+        typer.secho('\n'.join(msg_ary), fg=color)
         raise typer.Abort()
 
     print()
     print(timestamp)
     print()
     localtime = time.localtime(timestamp)
     tzname = time.tzname[(time.daylight and localtime.tm_isdst) and 1 or 0]
-    bcolor.printx(time.strftime('%Y-%m-%d %H:%M:%S %z', localtime), tzname, colorList=[Fore.YELLOW])
+    bcolor.printx(time.strftime('%Y-%m-%d %H:%M:%S %z', localtime), tzname, colors=[Fore.YELLOW])
     print()
 
     # pytz版本，留作参考别删除
     # tzNameList = [
     #     'Asia/Tokyo',
     #     'Asia/Kolkata',
     #     'Europe/London',
@@ -118,64 +113,76 @@
         print(f'{datetime_tz} {tzname} {dstStr}')
 
     print()
 
 # ------------------------------------------------------------------------
 
 
-@_app.command()
-def format_json_file(file_path: str, encoding: str = 'utf8'):
-    '''格式化 JSON 文件'''
-    file = bpath.get(file_path)
-    content = file.read_text(encoding=encoding)
-    data = json.loads(content)
-    file.write_text(json.dumps(data, indent=4, ensure_ascii=False, sort_keys=True), encoding=encoding)
+@_app.command('json')
+def format_json():
+    '''格式化 JSON （使用复制文本）'''
+    import pyperclip
+    content = pyperclip.paste()
+    try:
+        data = json.loads(content)
+        print(
+            json.dumps(data, indent=4, ensure_ascii=False, sort_keys=True)
+        )
+    except:
+        bcolor.print_red('无效的 JSON')
+        bcolor.print_red(content)
 
 
 # ------------------------------------------------------------------------
 
-class MirrorType(str, Enum):
+class _MirrorType(str, Enum):
     pip = 'pip'
     npm = 'npm'
     all = 'all'
 
 
+_mirror_files = {
+    _MirrorType.pip: (
+        bpath.user('pip/pip.ini'),
+        [
+            '[global]',
+            'index-url = https://mirrors.aliyun.com/pypi/simple',
+        ],
+    ),
+    _MirrorType.npm: (
+        bpath.user('.bashrc'),
+        [
+            'registry=https://registry.npm.taobao.org/',
+            'electron_mirror=https://npm.taobao.org/mirrors/electron/',
+        ],
+    ),
+}
+
+
 @_app.command()
 def mirror(
-    type: MirrorType = typer.Option(MirrorType.all, help="设置镜像的类型，支持pip/npm/all"),
+    type: _MirrorType = typer.Option(_MirrorType.all, help="设置镜像的类型，支持pip/npm/all"),
     enabled: bool = typer.Option(True, help="是否使用镜像"),
 ):
     '''设置镜像地址'''
     async def _():
-        if type in (MirrorType.pip, MirrorType.all):
-            file = bpath.getUser('pip/pip.ini')
-            if enabled:
-                content = '\n'.join([
-                    '[global]',
-                    'index-url = https://mirrors.aliyun.com/pypi/simple',
-                ])
-                await bfile.writeText(file, content)
-                bcolor.printYellow('写入文件', file)
-                print(content)
-            else:
-                await bpath.remove(file)
-                bcolor.printRed('删除文件', file)
-        if type in (MirrorType.npm, MirrorType.all):
-            file = bpath.getUser('.bashrc')
+        if type is _MirrorType.all:
+            type_ary = [_MirrorType.pip, _MirrorType.npm]
+        else:
+            type_ary = [type]
+        for target_type in type_ary:
+            file, msg_ary = _mirror_files[target_type]
             if enabled:
-                content = '\n'.join([
-                    'registry=https://registry.npm.taobao.org/',
-                    'electron_mirror=https://npm.taobao.org/mirrors/electron/',
-                ])
-                await bfile.writeText(file, content)
-                bcolor.printYellow('写入文件', file)
-                print(content)
+                msg = '\n'.join(msg_ary)
+                await bfile.write_text(file, msg)
+                bcolor.print_green('写入文件', file)
+                bcolor.print_magenta(msg)
             else:
                 await bpath.remove(file)
-                bcolor.printRed('删除文件', file)
+                bcolor.print_red('删除文件', file)
     asyncio.run(_())
 
 
 # ------------------------------------------------------------------------
 
 @_app.command()
 def venv(
@@ -185,69 +192,67 @@
     clear_all: bool = typer.Option(False, help='删除venv.lock文件和venv目录后重新安装，可以保证环境干净的情况下将包更新'),
 ):
     '''python 虚拟环境配置'''
     path = path or Path(os.getcwd())
     clear = clear or clear_all
 
     async def _():
-        venvDir = bpath.get(path, 'venv')
-        _assertDirOrNotExists(venvDir)
-        if not venvDir.exists():
+        venv_dir = bpath.get(path, 'venv')
+        assert_dir(venv_dir)
+        if not venv_dir.exists():
             await binput.confirm('指定目录为非venv目录，是否确认新创建？')
         if clear:
-            await bpath.remove(venvDir)
-        if not venvDir.exists():
-            await bexecute.run(f'python.exe -m venv {venvDir}')
-        vevnListFile = bpath.get(path, 'venv.list')
-        _assertFileOrNotExists(vevnListFile)
-        if not vevnListFile.exists():
-            await bfile.writeText(vevnListFile, '')
-        await tidyVenvFile(vevnListFile, packages)
-        venvLockFile = bpath.get(path, 'venv.lock')
-        _assertFileOrNotExists(venvLockFile)
+            await bpath.remove(venv_dir)
+        if not venv_dir.exists():
+            await bexecute.run(f'python.exe -m venv {venv_dir}')
+        venv_list_file = bpath.get(path, 'venv.list')
+        assert_file(venv_list_file)
+        if not venv_list_file.exists():
+            await bfile.write_text(venv_list_file, '')
+        await tidy_venv_file(venv_list_file, packages)
+        venv_lock_file = bpath.get(path, 'venv.lock')
+        assert_file(venv_lock_file)
         if clear_all:
-            await bpath.remove(venvLockFile)
-        elif venvLockFile.exists():
-            await tidyVenvFile(venvLockFile, packages)
-        targetFile = venvLockFile if venvLockFile.exists() else vevnListFile
-        pip = bpath.get(venvDir, 'Scripts/pip.exe')
-        await pipInstall(pip, targetFile)
-        await bexecute.run(f'{pip} freeze > {venvLockFile}')
+            await bpath.remove(venv_lock_file)
+        elif venv_lock_file.exists():
+            await tidy_venv_file(venv_lock_file, packages)
+        target_file = venv_lock_file if venv_lock_file.exists() else venv_list_file
+        pip = bpath.get(venv_dir, 'Scripts/pip.exe')
+        await pip_install(pip, target_file)
+        await bexecute.run(f'{pip} freeze > {venv_lock_file}')
 
-    async def pipInstall(pip: Path, file: Path):
+    async def pip_install(pip: Path, file: Path):
         python = pip.with_name('python.exe')
         assert python.is_file()
-        assert not await bexecute.run(f'{python} -m pip install --upgrade pip'), '更新 pip 失败'
         assert pip.is_file()
+        assert not await bexecute.run(f'{python} -m pip install --upgrade pip'), '更新 pip 失败'
         assert not await bexecute.run(f'{pip} install -r {file}'), '执行失败'
 
-    async def tidyVenvFile(file: Path, packages: list[str]):
-        addPackageNames = [getPackageName(x) for x in packages]
-        ary = (await bfile.readText(file)).strip().replace('\r\n', '\n').replace('\r\n', '\n').split('\n')
-        ary = list(filter(lambda x: getPackageName(x) not in addPackageNames, ary))
+    async def tidy_venv_file(file: Path, packages: list[str]):
+        packages_names = [get_package_name(x) for x in packages]
+        ary = (await bfile.read_text(file)).strip().replace('\r\n', '\n').replace('\r\n', '\n').split('\n')
+        ary = list(filter(lambda x: get_package_name(x) not in packages_names, ary))
         ary.extend(packages)
         ary.sort()
-        await bfile.writeText(file, '\n'.join(ary).strip())
+        await bfile.write_text(file, '\n'.join(ary).strip())
 
-    def getPackageName(value: str):
-        sepList = ['>', '<', '=']
-        for sep in sepList:
+    def get_package_name(value: str):
+        sep_ary = ['>', '<', '=']
+        for sep in sep_ary:
             if sep in value:
                 return value.split(sep)[0]
         return value
 
-    asyncio.run(_())
-
+    def assert_file(file: Path):
+        assert file.is_file() or not file.exists(), f'必须是文件 {file=}'
 
-def _assertFileOrNotExists(file: Path):
-    assert file.is_file() or not file.exists(), f'必须是文件 {file=}'
+    def assert_dir(folder: Path):
+        assert folder.is_dir() or not folder.exists(), f'必须是目录 {folder=}'
 
-
-def _assertDirOrNotExists(folder: Path):
-    assert folder.is_dir() or not folder.exists(), f'必须是文件 {folder=}'
+    asyncio.run(_())
 
 
 # ------------------------------------------------------------------------
 
 
 @_app.command()
 def bin(
@@ -266,26 +271,26 @@
             bucketName = 'pytask'
             bucketUrl = 'http://qiniu-cdn.pytask.com'
             if output is None:
                 output = Path(os.curdir)
             bucket = QiniuBucket(bucketName, bucketUrl, ak, sk)
             targetList: list[str] = []
             if is_file:
-                content = await bfile.readText(Path(name))
+                content = await bfile.read_text(Path(name))
                 targetList.extend(content.replace('\r\n', '\n').split('\n'))
             else:
                 targetList.extend(name.strip().split(','))
             for target in targetList:
                 file = output.joinpath(target).resolve()
                 if file.exists():
                     print(f'exists {file}')
                 else:
                     key = f'bin/{target}.zip'
-                    await bucket.downloadPrivateFileUnzip(key, output)
-                    bcolor.printGreen(f'added  {file}')
+                    await bucket.download_unzip(key, output)
+                    bcolor.print_green(f'added  {file}')
         except Exception as e:
             print(e)
 
     asyncio.run(_())
 
 
 # ------------------------------------------------------------------------
@@ -298,10 +303,70 @@
     '''生成终端设置代理服务器的命令'''
     msg = '\r\n'.join([
         f'set http_proxy=http://localhost:{port}',
         f'set https_proxy=http://localhost:{port}',
         f'set all_proxy=http://localhost:{port}',
         '',
     ])
-    print('\r\n' + msg)
+    bcolor.print_magenta('\r\n' + msg)
     pyperclip.copy(msg)
-    print('已复制')
+    bcolor.print_yellow('已复制，可直接粘贴使用')
+
+
+# ------------------------------------------------------------------------
+
+@_app.command()
+def btask(path: str = typer.Option(None, help="项目路径")):
+    '''生成 btask 项目'''
+
+    content_dict = {
+        # ------------------------------------
+        'main.py':
+        '''
+from beni import btask
+
+btask.main()
+        ''',
+        # ------------------------------------
+        'dev.py':
+        '''
+from beni import btask
+
+btask.dev('hello.chicken')
+# btask.dev('hello.duck')
+        ''',
+        # ------------------------------------
+        'tasks/__init__.py':
+        '''
+        ''',
+        # ------------------------------------
+        'tasks/hello.py':
+        '''
+from typer import Typer
+from beni import bfunc
+
+app = Typer(help='这里是帮助信息')
+
+
+@app.command()
+@bfunc.sync_call
+async def chicken():
+    \'''chicken函数\'''
+    print('我是小鸡')
+
+
+@app.command()
+@bfunc.sync_call
+async def duck():
+    \'''duck函数\'''
+    print('我是小鸭')
+        ''',
+    }
+
+    async def func():
+        file_dir = bpath.get(path or os.getcwd())
+        for key in sorted(content_dict.keys()):
+            file = file_dir.joinpath(key)
+            content = content_dict[key]
+            await bfile.write_text(file, content)
+
+    asyncio.run(func())
```

### Comparing `benimang-0.2.2/beni/bcolor.py` & `benimang-0.3.5/beni/bcolor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 import sys
 from typing import IO, Any
 
 from colorama import Fore, Style, init
 
-_isInited = False
+_inited = False
 
-if not _isInited:
-    _isInited = True
+if not _inited:
+    _inited = True
     init()
 
 
-def printx(*values: Any, sep: str = ' ', end: str = '\n', file: IO[str] = sys.stdout, flush: bool = False, colorList: list[Any] | None):
+def printx(*values: Any, sep: str = ' ', end: str = '\n', file: IO[str] = sys.stdout, flush: bool = False, colors: list[Any] | None):
     '''color 数组参数 colorama.Fore / colorama.Back / colorama.Style 的常量'''
-    if colorList:
-        set(*colorList)
+    if colors:
+        set_colors(*colors)
     print(*values, sep=sep, end=end, file=file, flush=flush)
-    clear()
+    reset_colors()
 
 
-def getStr(value: Any, *colorList: Any):
-    if colorList:
-        value = ''.join(colorList) + str(value) + Style.RESET_ALL
+def get_str(value: Any, *colors: Any):
+    if colors:
+        value = ''.join(colors) + str(value) + Style.RESET_ALL
     return value
 
 
-def set(*colorList: Any):
-    content = ''.join(colorList)
+def set_colors(*colors: Any):
+    content = ''.join(colors)
     if content:
         sys.stdout.write(content)
         sys.stderr.write(content)
 
 
-def clear():
+def reset_colors():
     sys.stdout.write(Style.RESET_ALL)
     sys.stderr.write(Style.RESET_ALL)
 
 
-def red(msg: str):
-    return getStr(msg, Fore.LIGHTRED_EX)
+def get_red(msg: str):
+    return get_str(msg, Fore.LIGHTRED_EX)
 
 
-def yellow(msg: str):
-    return getStr(msg, Fore.YELLOW)
+def get_yellow(msg: str):
+    return get_str(msg, Fore.YELLOW)
 
 
-def green(msg: str):
-    return getStr(msg, Fore.LIGHTGREEN_EX)
+def get_green(msg: str):
+    return get_str(msg, Fore.LIGHTGREEN_EX)
 
 
-def cyan(msg: str):
+def get_cyan(msg: str):
     '蓝色'
-    return getStr(msg, Fore.LIGHTCYAN_EX)
+    return get_str(msg, Fore.LIGHTCYAN_EX)
 
 
-def magenta(msg: str):
+def get_magenta(msg: str):
     '紫色'
-    return getStr(msg, Fore.LIGHTMAGENTA_EX)
+    return get_str(msg, Fore.LIGHTMAGENTA_EX)
 
 
-def white(msg: str):
-    return getStr(msg, Fore.LIGHTWHITE_EX)
+def get_white(msg: str):
+    return get_str(msg, Fore.LIGHTWHITE_EX)
 
 
-def printRed(*values: Any):
-    print(red(' '.join([str(x) for x in values])))
+def print_red(*msgs: Any):
+    print(get_red(' '.join([str(x) for x in msgs])))
 
 
-def printYellow(*values: Any):
-    print(yellow(' '.join([str(x) for x in values])))
+def print_yellow(*msgs: Any):
+    print(get_yellow(' '.join([str(x) for x in msgs])))
 
 
-def printGreen(*values: Any):
-    print(green(' '.join([str(x) for x in values])))
+def print_green(*msgs: Any):
+    print(get_green(' '.join([str(x) for x in msgs])))
 
 
-def printCyan(*values: Any):
+def print_cyan(*msgs: Any):
     '蓝色'
-    print(cyan(' '.join([str(x) for x in values])))
+    print(get_cyan(' '.join([str(x) for x in msgs])))
 
 
-def printMagenta(*values: Any):
+def print_magenta(*msgs: Any):
     '紫色'
-    print(magenta(' '.join([str(x) for x in values])))
+    print(get_magenta(' '.join([str(x) for x in msgs])))
 
 
-def printWhite(*values: Any):
-    print(white(' '.join([str(x) for x in values])))
+def print_white(*msgs: Any):
+    print(get_white(' '.join([str(x) for x in msgs])))
```

### Comparing `benimang-0.2.2/beni/bexecute.py` & `benimang-0.3.5/beni/bexecute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import asyncio
 from pathlib import Path
 from typing import Any
 
 from beni import bbyte, bpath
 
 
-async def winscp(winscp_exe: Path | str, key_file: str, server: str, cmd_list: list[str], show_cmd: bool = True):
-    logFile = bpath.getUser('executeWinScp.log')
-    await bpath.remove(logFile)
+async def winscp(winscp_exe: Path | str, key_file: str, server: str, cmds: list[str], show_cmd: bool = True):
+    log_file = bpath.user('executeWinScp.log')
+    await bpath.remove(log_file)
     ary = [
-        'option batch abort',
-        'option transfer binary',
+        f'option batch abort',
+        f'option transfer binary',
         f'open sftp://{server} -privatekey={key_file} -hostkey=*',
-    ]
-    ary += cmd_list
-    ary += [
-        'close',
-        'exit',
+        *cmds,
+        f'close',
+        f'exit',
     ]
     # /console
-    cmd = f'{winscp_exe} /log={logFile} /loglevel=0 /command ' + ' '.join("%s" % x for x in ary)
+    cmd = f'{winscp_exe} /log={log_file} /loglevel=0 /command ' + ' '.join(ary)
     if show_cmd:
         print(cmd)
     return await run(cmd)
 
 
-async def runTry(*args: Any, output: str = '', error: str = ''):
-    outputBytes, errorBytes, _ = await runQuiet(*args)
-    if output and output not in bbyte.decode(outputBytes):
+async def run_try(*args: Any, output: str = '', error: str = ''):
+    output_bytes, error_bytes, _ = await run_quiet(*args)
+    if output and output not in bbyte.decode(output_bytes):
         raise Exception(f'命令执行失败: {" ".join([str(x) for x in args])}')
-    if error and error not in bbyte.decode(errorBytes):
+    if error and error not in bbyte.decode(error_bytes):
         raise Exception(f'命令执行失败: {" ".join([str(x) for x in args])}')
 
 
-async def runQuiet(*args: Any):
+async def run_quiet(*args: Any):
     proc = await asyncio.create_subprocess_shell(
         ' '.join([str(x) for x in args]),
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
     return await proc.communicate() + (proc.returncode or 0,)
```

### Comparing `benimang-0.2.2/beni/bfile.py` & `benimang-0.3.5/beni/bfile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,73 @@
 from pathlib import Path
 from typing import Any
 
 import aiofiles
 
-from beni import bfunc, block, bpath
+from beni import bhash, block, bpath
 
 _limit = 50
 
 
-@block.useLimit(_limit)
-async def writeText(file: Path | str, content: str, encoding: str = 'utf8', newline: str = '\n'):
+@block.limit(_limit)
+async def write_text(file: Path | str, content: str, encoding: str = 'utf8', newline: str = '\n'):
     file = bpath.get(file)
     await bpath.make(file.parent)
     async with aiofiles.open(file, 'w', encoding=encoding, newline=newline) as f:
         return await f.write(content)
 
 
-@block.useLimit(_limit)
-async def writeBytes(file: Path | str, data: bytes):
+@block.limit(_limit)
+async def write_bytes(file: Path | str, data: bytes):
     file = bpath.get(file)
     await bpath.make(file.parent)
     async with aiofiles.open(file, 'wb') as f:
         return await f.write(data)
 
 
-@block.useLimit(_limit)
-async def writeYaml(file: Path | str, data: Any):
+@block.limit(_limit)
+async def write_yaml(file: Path | str, data: Any):
     import yaml
-    await writeText(file, yaml.safe_dump(data))
+    await write_text(file, yaml.safe_dump(data))
 
 
-@block.useLimit(_limit)
-async def writeJson(file: Path | str, data: Any, mini: bool = True):
+@block.limit(_limit)
+async def write_json(file: Path | str, data: Any, mini: bool = True):
     if mini:
-        await writeText(file, bfunc.jsonDumpsMini(data))
+        await write_text(file, bhash.json_dumps(data))
     else:
         import json
-        await writeText(file, json.dumps(data, ensure_ascii=False, sort_keys=True, indent=4))
+        await write_text(file, json.dumps(data, ensure_ascii=False, sort_keys=True, indent=4))
 
 
-@block.useLimit(_limit)
-async def readText(file: Path | str, encoding: str = 'utf8', newline: str = '\n'):
+@block.limit(_limit)
+async def read_text(file: Path | str, encoding: str = 'utf8', newline: str = '\n'):
     async with aiofiles.open(file, 'r', encoding=encoding, newline=newline) as f:
         return await f.read()
 
 
-@block.useLimit(_limit)
-async def readBytes(file: Path | str):
+@block.limit(_limit)
+async def read_bytes(file: Path | str):
     async with aiofiles.open(file, 'rb') as f:
         return await f.read()
 
 
-@block.useLimit(_limit)
-async def readYaml(file: Path | str):
+@block.limit(_limit)
+async def read_yaml(file: Path | str):
     import yaml
     return yaml.safe_load(
-        await readText(file)
+        await read_text(file)
     )
 
 
-@block.useLimit(_limit)
-async def readJson(file: Path | str):
+@block.limit(_limit)
+async def read_json(file: Path | str):
     import orjson
-    return orjson.loads(await readBytes(file))
+    return orjson.loads(await read_bytes(file))
 
 
-@block.useLimit(_limit)
-async def readToml(file: Path | str):
+@block.limit(_limit)
+async def read_toml(file: Path | str):
     import tomllib
     return tomllib.loads(
-        await readText(file)
-    )
-
-
-async def md5File(file: Path | str):
-    return bfunc.md5Bytes(
-        await readBytes(file)
-    )
-
-
-async def crcFile(file: Path | str):
-    return bfunc.crcBytes(
-        await readBytes(file)
+        await read_text(file)
     )
```

### Comparing `benimang-0.2.2/beni/bfunc.py` & `benimang-0.3.5/beni/bfunc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,157 +1,132 @@
 import asyncio
-import binascii
-import hashlib
-import json
 import os
 import random
 import sys
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import asynccontextmanager
 from functools import wraps
 from pathlib import Path
-from typing import Any, Callable, Coroutine, TypeVar, cast
+from typing import Any, Callable, Coroutine, cast
 
 import async_timeout
 
-Fun = TypeVar("Fun", bound=Callable[..., object])
-AsyncFun = TypeVar("AsyncFun", bound=Callable[..., Coroutine[Any, Any, object]])
-AnyType = TypeVar("AnyType")
+from beni.btype import AnyType, AsyncFunc, IntFloatStr, Null
 
 
-def jsonDumpsMini(value: Any):
-    return json.dumps(value, ensure_ascii=False, sort_keys=True, separators=(',', ':'))
-
-
-def md5Bytes(data: bytes):
-
-    return hashlib.md5(data).hexdigest()
-
-
-def md5Str(content: str):
-    return md5Bytes(content.encode())
-
-
-def md5Data(data: Any):
-    return md5Str(
-        jsonDumpsMini(data)
-    )
-
-
-def crcBytes(data: bytes):
-
-    return hex(binascii.crc32(data))[2:].zfill(8)
-
-
-def crcStr(content: str):
-    return crcBytes(content.encode())
-
-
-def crcData(data: Any):
-    return crcStr(
-        jsonDumpsMini(data)
-    )
-
-
-def setWinUtf8():
+def sys_utf8():
     if sys.platform == 'win32':
         os.system('chcp 65001')
 
 
-def addEnvPath(p: Path | str):
+def add_env_dir(p: Path | str):
     value = os.getenv('path') or ''
     value = ';'.join([value, str(p)])
     os.putenv('path', value)
 
 
-def makeValidateCode(length: int):
+def make_verify_code(length: int):
     minValue = 10 ** (length - 1)
     maxValue = int('9' * length)
     return str(random.randrange(minValue, maxValue))
 
 
-IntFloatStr = TypeVar("IntFloatStr", int, float, str)
-
-
-def getValueInside(value: IntFloatStr, minValue: IntFloatStr, maxValue: IntFloatStr):
+def get_inside(value: IntFloatStr, min_value: IntFloatStr, max_value: IntFloatStr):
     '包括最小值和最大值'
-    value = min(value, maxValue)
-    value = max(value, minValue)
+    value = min(value, max_value)
+    value = max(value, min_value)
     return value
 
 
-def getPercentValue(targetValue: float, minValue: float, maxValue: float, minResult: float, maxResult: float):
-    '''
-    根据百分之计算指定数值
-    '''
-    if targetValue >= maxValue:
-        return maxResult
-    elif targetValue <= minValue:
-        return minResult
+def get_value(value: float, min_value: float, max_value: float, min_result: float, max_result: float):
+    '根据百分之计算指定数值'
+    if value >= max_value:
+        return max_result
+    elif value <= min_value:
+        return min_result
     else:
-        percent = (targetValue - minValue) / (maxValue - minValue)
-        return minResult + (maxResult - minResult) * percent
+        percent = (value - min_value) / (max_value - min_value)
+        return min_result + (max_result - min_result) * percent
 
 
-def getIncrease(fromValue: float, toValue: float):
+def get_increase(fromValue: float, toValue: float):
     return toValue / fromValue - 1
 
 
-def toFloat(value: IntFloatStr, default: float = 0):
+def to_float(value: IntFloatStr, default: float = 0):
     result = default
     try:
         result = float(value)
     except:
         pass
     return result
 
 
-def toInt(value: IntFloatStr, default: int = 0):
+def to_int(value: IntFloatStr, default: int = 0):
     result = default
     try:
         result = int(value)
     except:
         pass
     return result
 
 
-def getSqlPlacement(ary: list[Any] | set[Any]):
+def get_sql_placement(ary: list[Any] | set[Any]):
     return '(' + ','.join(['?' for _ in range(len(ary))]) + ')'
 
 
-def getWrapped(data: Any):
+def get_wrapped(data: Any):
     result = data
     while hasattr(result, '__wrapped__'):
         result = getattr(result, '__wrapped__')
     return result
 
 
 def retry(times: int):
-    def fun(func: AsyncFun) -> AsyncFun:
+    def fun(func: AsyncFunc) -> AsyncFunc:
         @wraps(func)
         async def wrapper(*args: Any, **kwargs: Any):
             current = 0
             while True:
                 try:
                     return await func(*args, **kwargs)
                 except:
                     current += 1
                     if current >= times:
                         raise
-        return cast(AsyncFun, wrapper)
+        return cast(AsyncFunc, wrapper)
     return fun
 
 
 @asynccontextmanager
 async def timeout(timeout: float):
     async with async_timeout.timeout(timeout):
         yield
 
 
-def initErrorFormat():
+def sync_call(func: Callable[..., Coroutine[Any, Any, AnyType]]) -> Callable[..., AnyType]:
+    @wraps(func)
+    def wraper(*args: Any, **kwargs: Any):
+        return asyncio.run(func(*args, **kwargs))
+    return cast(Any, wraper)
+
+
+_once_call_set: set[int] = set()
+
+
+def once_call(func: Callable[..., AnyType]) -> Callable[..., AnyType]:
+    @wraps(func)
+    def wraper(*args: Any, **kwargs: Any):
+        assert id(func) not in _once_call_set, f'函数 {func.__module__}.{func.__name__} 只能调用一次'
+        _once_call_set.add(id(func))
+        return func(*args, **kwargs)
+    return cast(Any, wraper)
+
+
+def init_pretty_errors():
     import pretty_errors
     pretty_errors.configure(
         separator_character='*',
         filename_display=pretty_errors.FILENAME_COMPACT,
         # line_number_first   = True,
         display_link=True,
         lines_before=5,
@@ -168,40 +143,24 @@
     def _(v: int = 1):
         nonlocal value
         value += v
         return value
     return _
 
 
-_threadPoolExector: ThreadPoolExecutor | None = None
-_threadMaxNum: int = 4
+_thread_pool_exector: ThreadPoolExecutor = Null
+_thread_max_workers: int = 4
 
 
-def setThreadMaxNum(value: int):
-    global _threadPoolExector, _threadMaxNum
-    if not _threadPoolExector:
-        _threadMaxNum = value
+def set_run_thread_max(value: int):
+    global _thread_pool_exector, _thread_max_workers
+    if not _thread_pool_exector:
+        _thread_max_workers = value
     else:
-        raise Exception('ThreadPoolExector实例化之后不能再设置maxWorkers')
-
-
-async def runInThread(lambdaFunc: Callable[..., AnyType]) -> AnyType:
-    global _threadPoolExector
-    if _threadPoolExector is None:
-        _threadPoolExector = ThreadPoolExecutor(max_workers=_threadMaxNum)
-    return await asyncio.get_running_loop().run_in_executor(_threadPoolExector, lambdaFunc)
-
-
-class TaskList():
-
-    def __init__(self):
-        self._enabled = True
-        self._list: list[Coroutine[Any, Any, Any]] = []
+        raise Exception('ThreadPoolExecutor 实例化之后不允许调用 set_thread_max_workers')
 
-    async def add(self, task: Coroutine[Any, Any, Any]):
-        assert self._enabled
-        asyncio.create_task(task)
-        self._list.append(task)
 
-    async def waitAll(self):
-        self._enabled = False
-        await asyncio.gather(*self._list)
+async def run_thread(func: Callable[..., AnyType]) -> AnyType:
+    global _thread_pool_exector
+    if not _thread_pool_exector:
+        _thread_pool_exector = ThreadPoolExecutor(max_workers=_thread_max_workers)
+    return await asyncio.get_running_loop().run_in_executor(_thread_pool_exector, func)
```

### Comparing `benimang-0.2.2/beni/bhttp.py` & `benimang-0.3.5/beni/bhttp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import asyncio
 from http.cookiejar import CookieJar
 from pathlib import Path
-from typing import Any, Final
+from typing import Any
 from urllib.parse import urlencode
 from urllib.request import HTTPCookieProcessor, build_opener, install_opener
 
 import aiofiles
 import aiohttp
 import orjson
 
 from beni import block, bpath
 
-_limit: Final = 5
-_defaultRetry = 3
+_LIMIT = 5
+_retry = 3
 
-_httpHeaders = {
+_headers = {
     'Connection': 'keep-alive',
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/76.0.3809.100 Safari/537.36',
     'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
     'Accept-Encoding': 'gzip',
     'Accept-Language': 'zh-CN,zh;q=0.8',
 }
 
 
-def _makeHttpHeaders(headers: dict[str, Any] | None = None):
+def _make_headers(headers: dict[str, Any] | None = None):
     if headers:
-        return _httpHeaders | headers
+        return _headers | headers
     else:
-        return dict(_httpHeaders)
+        return dict(_headers)
 
 
-@block.useLimit(_limit)
+@block.limit(_LIMIT)
 async def get(
     url: str,
     *,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
 ):
-    retry = retry or _defaultRetry
+    retry = retry or _retry
     while True:
         retry -= 1
         try:
             async with aiohttp.ClientSession() as session:
-                async with session.get(url, headers=_makeHttpHeaders(headers), timeout=timeout) as response:
+                async with session.get(url, headers=_make_headers(headers), timeout=timeout) as response:
                     result = await response.read()
                     if not result:
                         await asyncio.sleep(0.5)
                         raise Exception('http get result is empty')
                     return result, response
         except:
             if retry <= 0:
                 raise
 
 
-async def getBytes(
+async def get_bytes(
     url: str,
     *,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
 ):
     resultBytes, _ = await get(
@@ -66,65 +66,64 @@
         headers=headers,
         timeout=timeout,
         retry=retry,
     )
     return resultBytes
 
 
-async def getStr(
+async def get_str(
     url: str,
     *,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
 ):
-    result = await getBytes(url, headers=headers, timeout=timeout, retry=retry)
+    result = await get_bytes(url, headers=headers, timeout=timeout, retry=retry)
     return result.decode()
 
 
-async def getJson(
+async def get_json(
     url: str,
     *,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
 ):
-    result = await getBytes(url, headers=headers, timeout=timeout, retry=retry)
+    result = await get_bytes(url, headers=headers, timeout=timeout, retry=retry)
     return orjson.loads(result)
 
 
-@block.useLimit(_limit)
+@block.limit(_LIMIT)
 async def post(
     url: str,
     *,
     data: bytes | dict[str, Any] | None = None,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
 ):
-    retry = retry or _defaultRetry
+    retry = retry or _retry
     while True:
         retry -= 1
         try:
-            postData = data
             if type(data) is dict:
-                postData = urlencode(data).encode()
+                data = urlencode(data).encode()
             async with aiohttp.ClientSession() as session:
-                async with session.post(url, data=postData, headers=_makeHttpHeaders(headers), timeout=timeout) as response:
+                async with session.post(url, data=data, headers=_make_headers(headers), timeout=timeout) as response:
                     result = await response.read()
                     if not result:
                         await asyncio.sleep(0.5)
                         raise Exception('http get result is empty')
                     return result, response
         except:
             if retry <= 0:
                 raise
 
 
-async def postBytes(
+async def post_bytes(
     url: str,
     *,
     data: bytes | dict[str, Any] | None = None,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
 ):
@@ -134,58 +133,58 @@
         headers=headers,
         timeout=timeout,
         retry=retry,
     )
     return resultBytes
 
 
-async def postStr(
+async def post_str(
     url: str,
     *,
     data: bytes | dict[str, Any] | None = None,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
 ):
-    return (await postBytes(
+    return (await post_bytes(
         url,
         data=data,
         headers=headers,
         timeout=timeout,
         retry=retry,
     )).decode()
 
 
-async def postJson(
+async def post_json(
     url: str,
     *,
     data: bytes | dict[str, Any] | None = None,
     headers: dict[str, Any] | None = None,
     timeout: int = 10,
     retry: int | None = None,
 ):
     return orjson.loads(
-        await postBytes(
+        await post_bytes(
             url,
             data=data,
             headers=headers,
             timeout=timeout,
             retry=retry,
         )
     )
 
 
-@block.useLimit(_limit)
+@block.limit(_LIMIT)
 async def download(url: str, file: Path | str, timeout: int = 300):
     # total_size: int = 0
     # download_size: int = 0
     try:
         file = bpath.get(file)
         async with aiohttp.ClientSession() as session:
-            async with session.get(url, headers=_httpHeaders, timeout=timeout) as response:
+            async with session.get(url, headers=_headers, timeout=timeout) as response:
                 await bpath.make(file.parent)
                 assert response.content_length, '下载内容为空'
                 # total_size = response.content_length
                 async with aiofiles.open(file, 'wb') as f:
                     while True:
                         data = await response.content.read(1024 * 1024)
                         if data:
@@ -197,16 +196,16 @@
         # assert total_size and total_size == download_size, '下载为文件不完整'
     except:
         await bpath.remove(file)
         raise
 
 
 def setDefaultRetry(value: int):
-    global _defaultRetry
-    _defaultRetry = value
+    global _retry
+    _retry = value
 
 
 # Cookie
 _cookie = CookieJar()
 _cookieProc = HTTPCookieProcessor(_cookie)
 _opener = build_opener(_cookieProc)
 install_opener(_opener)
```

### Comparing `benimang-0.2.2/beni/binput.py` & `benimang-0.3.5/beni/binput.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,89 @@
 import getpass
 import random
+from dataclasses import dataclass
+from types import FunctionType
 from typing import Any, Callable, Coroutine, cast
 
 from beni import bcolor
 
 
-async def hold(msg: str | None = None, password: bool = False, *exitvalue_list: str):
+async def hold(msg: str | None = None, password: bool = False, *exits: str):
     msg = msg or '测试暂停，输入exit可以退出'
     msg = f'{msg}: '
-    exitvalue_list = exitvalue_list or ('exit',)
+    exits = exits or ('exit',)
     while True:
         if password:
-            inputValue = getpass.getpass(msg)
+            value = getpass.getpass(msg)
         else:
             import aioconsole
-            inputValue = cast(str, await aioconsole.ainput(msg))
-        if (inputValue in exitvalue_list) or ('*' in exitvalue_list):
-            return inputValue
+            value = cast(str, await aioconsole.ainput(msg))
+        if (value in exits) or ('*' in exits):
+            return value
 
 
-async def confirm(msg: str = '确认'):
+async def confirm(msg: str = '确认', show_input: bool = False):
+    '输入验证码继续（随机3位数字的验证码）'
     code = f'{random.randint(1, 999):03}'
-    await hold(f'{msg} [ {_getRemindMsg(code)} ]', False, code)
+    await hold(f'{msg} [ {bcolor.get_yellow(code)} ]', not show_input, code)
+
+
+@dataclass
+class Selections:
+    msg: str
+    desc: str | None = None
+    confirm: str | Callable[[str], Any] | None = None
+    handler: Callable[[str], Coroutine[Any, Any, Any]] | None = None
 
 
-async def select(*data: tuple[str, str, str | Callable[[str], Any] | None, Callable[[str], Coroutine[Any, Any, Any]] | None]):
+async def select(*data_ary: Selections):
     '''
-    value = goSelect(
-        ('descA', 'confirmDescA', 'quanbuqueren', __handlerA),
-        ('descB', 'confirmDescB', lambda x: ..., __handlerB),
-    )
+    async def main():
+        value = await binput.select(
+            binput.Selections('msgA', 'descA', 'confirmTextA', __handlerA),
+            binput.Selections('msgB', 'descB', 'confirmTextB', __handlerB),
+        )
+        print(value)
+
+    async def __handlerA(value: str):
+        print('run __handlerA')
+
+    async def __handlerB(value: str):
+        print('run __handlerB')
     '''
     print()
     print('-' * 30)
     print()
-    for msg, inputDisplay, _, _ in data:
-        if inputDisplay:
-            msg += f' [ {_getRemindMsg(inputDisplay)} ]'
-        print(msg)
+    for item in data_ary:
+        if item.desc:
+            print(f'{item.msg} [ {bcolor.get_yellow(item.desc)} ]')
+        else:
+            print(item.msg)
     print()
     import aioconsole
     while True:
         value = cast(str, await aioconsole.ainput('输入选择：'))
         isMatch = False
-        result = None
-        for msg, inputDisplay, inputValue, handler in data:
-            inputValue = inputValue or inputDisplay or msg
-            if type(inputValue) is str:
-                isMatch = value == inputValue
-            else:
+        for item in data_ary:
+            check = item.confirm or item.desc or item.msg
+            if type(check) is str:
+                isMatch = value == check
+            elif type(check) is FunctionType:
                 try:
-                    isMatch = cast(Callable[[str], bool], inputValue)(value)
+                    isMatch = check(value)
                 except:
                     pass
             if isMatch:
-                if handler:
-                    result = await handler(value)
-                    break
-        if isMatch and result is not False:
-            return value
+                if item.handler:
+                    await item.handler(value)
+                return value
 
 
-async def inputCheck(msg: str, check: Callable[[str], Any]):
+async def input_check(msg: str, check_func: Callable[[str], Any]):
     import aioconsole
     while True:
         try:
             value = cast(str, await aioconsole.ainput(f'{msg}：'))
-            if check(value):
+            if check_func(value):
                 return value
         except:
             pass
-
-
-def _getRemindMsg(msg: str):
-    return bcolor.yellow(msg)
```

### Comparing `benimang-0.2.2/beni/block.py` & `benimang-0.3.5/beni/bcache.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,187 +1,181 @@
 from __future__ import annotations
 
 import asyncio
-import inspect
-from contextlib import asynccontextmanager
+import pickle
+from datetime import datetime, timedelta
 from functools import wraps
 from pathlib import Path
-from typing import Any, Callable, cast
+from typing import Any, Callable, Coroutine, cast
 
-from beni import bfunc, binput, bpath
+from beni import bfile, bfunc, bhash, bpath, btime
+from beni.bdefine import END_DATETIME
 
 
-@asynccontextmanager
-async def useFileLock(*keys: str, timeout: float = 0, quite: bool = False):
-    import portalocker
-    lock_list: list[portalocker.Lock] = []
-    keyfile_list: list[Path] = []
-    for key in keys:
-        lock, keyfile = await _lock_acquire(key, timeout, quite)
-        lock_list.append(lock)
-        keyfile_list.append(keyfile)
-    try:
-        yield
-    finally:
-        for lock in lock_list:
-            lock.release()
-        for keyfile in keyfile_list:
-            try:
-                await bpath.remove(keyfile)
-            except:
-                pass
-
-
-async def _lock_acquire(key: str, timeout: float = 0, quite: bool = False):
-    '''不对外部提供，只提供给 async_keylock 方法使用'''
-    keyfile = bpath.getWorkspace(f'.lock/{bfunc.crcStr(key)}.lock')
-    await bpath.make(keyfile.parent)
-    import portalocker
-    while True:
+class Store:
+
+    def __init__(self, cache_dir: Path) -> None:
+        self._CACHE_DIR = cache_dir
+        self._DEADLINE = _StoreDeadline(cache_dir)
+
+    async def put(self, key: str, data: Any, *, duration: timedelta | None = None, deadline: datetime | None = None):
+        assert not (duration and deadline), 'BCacheStore.put 不允许同时指定 duration 和 deadline'
+        file = self._get_file(key)
         try:
-            lock = portalocker.Lock(keyfile, timeout=timeout, fail_when_locked=timeout == 0)
-            f = lock.acquire()
-            f.write(key)
-            f.flush()
-            break
+            await bfile.write_bytes(
+                file,
+                pickle.dumps(data),
+            )
+            if not deadline:
+                if duration:
+                    deadline = btime.datetime() + duration
+                else:
+                    deadline = END_DATETIME
+            self._DEADLINE.update(key, deadline)
+            return True
         except:
-            if quite:
-                raise Exception(f'资源被锁定无法继续操作 key={key} keyfile={keyfile}')
+            await bpath.remove(file)
+            self._DEADLINE.clear(key)
+            return False
+
+    async def get(self, key: str):
+        file = self._get_file(key)
+        if file.is_file():
+            if self._DEADLINE.valid(key):
+                return pickle.loads(await bfile.read_bytes(file))
             else:
-                async def __retry(_):
-                    print('正在重试...')
-
-                async def __exit(_):
-                    raise Exception(f'资源被锁定无法继续操作 - {key}')
-
-                asyncio.run(
-                    binput.select(
-                        ('重试', 'retry', None, __retry),
-                        ('退出', 'exit', None, __exit),
-                    )
-                )
-    return lock, keyfile
-
-
-# ------------------------------------------------------------------------------------------------------------------------
-
-
-def useLimit(limit: int = 1):
-    def wraperfun(func: bfunc.AsyncFun) -> bfunc.AsyncFun:
-        @wraps(func)
-        async def wraper(*args: Any, **kwargs: Any):
-            funid = id(inspect.unwrap(func))
-            if funid not in _limit_dict:
-                _limit_dict[funid] = _Limit(limit)
-            try:
-                await _limit_dict[funid].wait()
-                return await func(*args, **kwargs)
-            finally:
-                await _limit_dict[funid].release()
-        return cast(Any, wraper)
-    return wraperfun
-
-
-async def setLimit(func: Callable[..., Any], limit: int):
-    funid = id(inspect.unwrap(func))
-    if funid not in _limit_dict:
-        _limit_dict[funid] = _Limit(limit)
-    await _limit_dict[funid].set_limit(limit)
-
-
-_limit_dict: dict[int, _Limit] = {}
-
-
-class _Limit():
-
-    _queue: asyncio.Queue[Any]
-    _running: int
-
-    def __init__(self, limit: int):
-        self._limit = limit
-        self._queue = asyncio.Queue()
-        self._running = 0
-        while self._queue.qsize() < self._limit:
-            self._queue.put_nowait(True)
-
-    async def wait(self):
-        await self._queue.get()
-        self._running += 1
-
-    async def release(self):
-        if self._queue.qsize() < self._limit:
-            await self._queue.put(True)
-        self._running -= 1
-
-    async def set_limit(self, limit: int):
-        self._limit = limit
-        while self._running + self._queue.qsize() < self._limit:
-            await self._queue.put(True)
-        while self._running + self._queue.qsize() > self._limit:
-            if self._queue.empty():
-                break
-            await self._queue.get()
-
-
-# ------------------------------------------------------------------------------------------------------------------------
-
-
-class RWLock():
-
-    def __init__(self, maxNum: int) -> None:
-        self._maxNum = maxNum
-        self._readNum = 0
-        self._writeNum = 0
-        self._onReadFinished = asyncio.Event()
-        self._onWriteFinished = asyncio.Event()
-
-    def _getNum(self):
-        return self._readNum + self._writeNum
+                await bpath.remove(file)
+        else:
+            self._DEADLINE.clear(key)
+
+    async def clear(self, key: str):
+        await bpath.remove(self._get_file(key))
+
+    def cache_func(self, key: str, *, duration: timedelta | None = None, deadline: datetime | None = None):
+        def fun(func: bfunc.AsyncFunc) -> bfunc.AsyncFunc:
+            @wraps(func)
+            async def wrapper(*args: Any, **kwargs: Any):
+                try:
+                    result = await self.get(key)
+                    if result is None:
+                        result = await func(*args, **kwargs)
+                        await self.put(key, result, duration=duration, deadline=deadline)
+                    return result
+                except:
+                    await self.clear(key)
+                    raise
+            return cast(Any, wrapper)
+        return fun
+
+    def _get_file(self, key: str):
+        return bpath.get(self._CACHE_DIR, bhash.crc_str(key))
+
+
+class _StoreDeadline:
+
+    def __init__(self, cache_dir: Path) -> None:
+        self._file = cache_dir.joinpath('deadline.dat')
+        self._writing = False
+        try:
+            self._data: dict[str, datetime] = pickle.loads(
+                asyncio.run(bfile.read_bytes(self._file))
+            )
+        except:
+            self._data: dict[str, datetime] = {}
 
-    async def getRead(self):
-        while True:
-            if self._writeNum:
-                self._onWriteFinished.clear()
-                await self._onWriteFinished.wait()
-            elif self._getNum() >= self._maxNum:
-                self._onReadFinished.clear()
-                await self._onReadFinished.wait()
+    async def valid(self, key: str):
+        if key in self._data:
+            if self._data[key] > btime.datetime():
+                return True
             else:
-                self._readNum += 1
-                break
+                self.clear(key)
+        return False
 
-    def releaseRead(self):
-        self._readNum -= 1
-        if not self._readNum:
-            self._onReadFinished.set()
-
-    @asynccontextmanager
-    async def useRead(self):
-        await self.getRead()
+    def update(self, key: str, deadline: datetime):
+        self._data[key] = deadline
+        self._flush()
+
+    def clear(self, key: str):
+        if key in self._data:
+            del self._data[key]
+            self._flush()
+
+    def _flush(self):
+        if not self._writing:
+            self._writing = True
+            asyncio.create_task(self._write())
+
+    async def _write(self):
+        await asyncio.sleep(2)
+        self._writing = False
         try:
-            yield
-        finally:
-            self.releaseRead()
+            await bfile.write_bytes(
+                self._file,
+                pickle.dumps(self._data),
+            )
+        except:
+            pass
 
-    async def getWrite(self):
+# ---------------------------------------------------------------------------------------------------------
+
+
+def cache_func(func: bfunc.AsyncFunc) -> bfunc.AsyncFunc:
+    @wraps(func)
+    async def wraper(*args: Any, **kwargs: Any):
+        base_func = bfunc.get_wrapped(func)
+        data = _cache_dict.get(base_func)
+        if not data:
+            data = _CacheFuncData()
+            _cache_dict[base_func] = data
+        key = (args, kwargs)
         while True:
-            if self._readNum:
-                self._onReadFinished.clear()
-                await self._onReadFinished.wait()
-            elif self._writeNum:
-                self._onWriteFinished.clear()
-                await self._onWriteFinished.wait()
+            result = data.get(key)
+            if result is not None:
+                return result
+            elif data.running:
+                await data.event.wait()
+                continue
             else:
-                self._writeNum += 1
-                break
-
-    def releaseWrite(self):
-        self._writeNum -= 1
-        self._onWriteFinished.set()
-
-    @asynccontextmanager
-    async def useWrite(self):
-        await self.getWrite()
-        try:
-            yield
-        finally:
-            self.releaseWrite()
+                data.running = True
+                try:
+                    result = await func(*args, **kwargs)
+                    data.set(key, result)
+                    return result
+                except:
+                    return None
+                finally:
+                    data.running = False
+                    data.event.set()
+                    data.event.clear()
+    return cast(Any, wraper)
+
+
+def cache_func_clear(func: Callable[..., _AsyncFunc]):
+    base_func = bfunc.get_wrapped(func)
+    data = _cache_dict.get(base_func)
+    if data:
+        data.clear()
+
+
+class _CacheFuncData:
+
+    def __init__(self) -> None:
+        self.event = asyncio.Event()
+        self.running = False
+        self._result_ary: list[tuple[_FuncArgs, Any]] = []
+
+    def get(self, key: _FuncArgs):
+        for xx in self._result_ary:
+            if xx[0] == key:
+                return xx[1]
+
+    def set(self, key: _FuncArgs, result: Any):
+        self._result_ary = list(filter(lambda x: x[0] != key, self._result_ary))
+        self._result_ary.append((key, result))
+
+    def clear(self):
+        self._result_ary.clear()
+
+
+_AsyncFunc = Coroutine[Any, Any, object]
+_FuncArgs = tuple[tuple[Any, ...], dict[str, Any]]  # (*args, **kwargs)
+_cache_dict: dict[Callable[..., _AsyncFunc], _CacheFuncData] = {}
```

### Comparing `benimang-0.2.2/beni/blog.py` & `benimang-0.3.5/beni/blog.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,76 +4,75 @@
 from pathlib import Path
 from typing import Any
 
 from colorama import Fore
 
 from beni import bcolor, bpath
 
-_loggerName = 'beni'
+_name = 'beni'
 
-_countWarning: int = 0
-_countError: int = 0
-_countCritical: int = 0
+_warning_count = 0
+_error_count = 0
+_critical_count = 0
 
 
-def init(loggerName: str = '', loggerLevel: int = logging.INFO, logFile: Path | None = None):
-    LOGGER_FORMAT = '%(asctime)s %(levelname)-1s %(message)s', '%Y-%m-%d %H:%M:%S'
-    LOGGER_LEVEL_NAME = {
+def init(name: str = '', level: int = logging.INFO, file: Path | None = None):
+    FORMAT = '%(asctime)s %(levelname)-1s %(message)s', '%Y-%m-%d %H:%M:%S'
+    LEVEL_NAME = {
         logging.DEBUG: 'D',
         logging.INFO: '',
         logging.WARNING: 'W',
         logging.ERROR: 'E',
         logging.CRITICAL: 'C',
     }
 
-    if loggerName:
-        global _loggerName
-        _loggerName = loggerName
-
-    logger = logging.getLogger(_loggerName)
-    logger.setLevel(loggerLevel)
-    for loggingLevel, value in LOGGER_LEVEL_NAME.items():
-        logging.addLevelName(loggingLevel, value)
+    if name:
+        global _name
+        _name = name
+
+    logger = logging.getLogger(_name)
+    logger.setLevel(level)
+    for k, v in LEVEL_NAME.items():
+        logging.addLevelName(k, v)
 
-    loggerFormatter = logging.Formatter(*LOGGER_FORMAT)
+    formatter = logging.Formatter(*FORMAT)
 
     class CustomStreamHandler(logging.StreamHandler):  # type: ignore
 
         def emit(self, record: logging.LogRecord):
             try:
                 msg = self.format(record) + self.terminator
                 # issue 35046: merged two stream.writes into one.
                 func = self.stream.write
                 if record.levelno == logging.WARNING:
-                    global _countWarning
-                    _countWarning += 1
-                    bcolor.set(Fore.YELLOW)
-
+                    global _warning_count
+                    _warning_count += 1
+                    bcolor.set_colors(Fore.YELLOW)
                 elif record.levelno == logging.ERROR:
-                    global _countError
-                    _countError += 1
-                    bcolor.set(Fore.LIGHTRED_EX)
+                    global _error_count
+                    _error_count += 1
+                    bcolor.set_colors(Fore.LIGHTRED_EX)
                 elif record.levelno == logging.CRITICAL:
-                    global _countCritical
-                    _countCritical += 1
-                    bcolor.set(Fore.LIGHTMAGENTA_EX)
+                    global _critical_count
+                    _critical_count += 1
+                    bcolor.set_colors(Fore.LIGHTMAGENTA_EX)
                 func(msg)
-                bcolor.clear()
+                bcolor.reset_colors()
                 self.flush()
             except RecursionError:  # See issue 36272
                 raise
             except Exception:
                 self.handleError(record)
 
-    loggerHandler = CustomStreamHandler()
-    loggerHandler.setFormatter(loggerFormatter)
-    loggerHandler.setLevel(loggerLevel)
-    logger.addHandler(loggerHandler)
+    handler = CustomStreamHandler()
+    handler.setFormatter(formatter)
+    handler.setLevel(level)
+    logger.addHandler(handler)
 
-    if logFile:
+    if file:
 
         class CustomFileHandler(logging.FileHandler):
 
             _write_func: Any
             _xx = re.compile(r'\x1b\[\d+m')
 
             def _open(self):
@@ -82,66 +81,66 @@
                 setattr(result, 'write', self._write)
                 return result
 
             def _write(self, msg: str):
                 msg = self._xx.sub('', msg)
                 self._write_func(msg)
 
-        asyncio.run(bpath.make(logFile.parent))
-        fileLoggerHandler = CustomFileHandler(logFile, delay=True)
-        fileLoggerHandler.setFormatter(loggerFormatter)
-        fileLoggerHandler.setLevel(loggerLevel)
-        logger.addHandler(fileLoggerHandler)
+        asyncio.run(bpath.make(file.parent))
+        file_handler = CustomFileHandler(file, delay=True)
+        file_handler.setFormatter(formatter)
+        file_handler.setLevel(level)
+        logger.addHandler(file_handler)
 
 
 def debug(msg: Any, wrap: bool = False, *args: Any, **kwargs: Any):
-    logging.getLogger(_loggerName).debug(_format(msg, wrap), *args, **kwargs)
+    logging.getLogger(_name).debug(_format(msg, wrap), *args, **kwargs)
 
 
 def info(msg: Any, wrap: bool = False, *args: Any, **kwargs: Any):
-    logging.getLogger(_loggerName).info(_format(msg, wrap), *args, **kwargs)
+    logging.getLogger(_name).info(_format(msg, wrap), *args, **kwargs)
 
 
 def warning(msg: Any, wrap: bool = False, *args: Any, **kwargs: Any):
-    logging.getLogger(_loggerName).warning(_format(msg, wrap), *args, **kwargs)
+    logging.getLogger(_name).warning(_format(msg, wrap), *args, **kwargs)
 
 
 def error(msg: Any, wrap: bool = False, *args: Any, **kwargs: Any):
-    logging.getLogger(_loggerName).error(_format(msg, wrap), *args, **kwargs)
+    logging.getLogger(_name).error(_format(msg, wrap), *args, **kwargs)
 
 
 def critical(msg: Any, wrap: bool = False, *args: Any, **kwargs: Any):
-    logging.getLogger(_loggerName).critical(_format(msg, wrap), *args, **kwargs)
+    logging.getLogger(_name).critical(_format(msg, wrap), *args, **kwargs)
 
 
 def _format(msg: Any, wrap: bool):
     if wrap:
         return '\n\n' + msg + '\n'
     else:
         return msg
 
 
-def getCountWarning():
-    return _countWarning
+def get_warning_count():
+    return _warning_count
 
 
-def setCountWarning(value: int):
-    global _countWarning
-    _countWarning = value
+def set_warning_count(value: int):
+    global _warning_count
+    _warning_count = value
 
 
-def getCountError():
-    return _countError
+def get_error_count():
+    return _error_count
 
 
-def setCountError(value: int):
-    global _countError
-    _countError = value
+def set_error_count(value: int):
+    global _error_count
+    _error_count = value
 
 
-def getCountCritical():
-    return _countCritical
+def get_critical_count():
+    return _critical_count
 
 
-def setCountCritical(value: int):
-    global _countCritical
-    _countCritical = value
+def set_critical_count(value: int):
+    global _critical_count
+    _critical_count = value
```

### Comparing `benimang-0.2.2/beni/bpath.py` & `benimang-0.3.5/beni/bpath.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,84 +10,85 @@
 
 def get(path: str | Path, expand: str = ''):
     if type(path) is not Path:
         path = Path(path)
     return path.joinpath(expand).resolve()
 
 
-def getUser(expand: str = ''):
+def user(expand: str = ''):
     return get(Path('~').expanduser(), expand)
 
 
-def getDesktop(expand: str = ''):
-    return getUser(f'Desktop/{expand}')
+def desktop(expand: str = ''):
+    return user(f'Desktop/{expand}')
 
 
-def getWorkspace(expand: str = ''):
+def workspace(expand: str = ''):
+    DIR = 'beni-workspace'
     if sys.platform == 'win32':
-        return get(f'C:/beni-workspace/{expand}')
+        return get(f'C:/{DIR}/{expand}')
     else:
-        return get(f'/data/beni-workspace/{expand}')
+        return get(f'/data/{DIR}/{expand}')
 
 
-def getTempFile():
-    return getWorkspace(f'temp/{uuid.uuid4()}.tmp')
+def temp_file():
+    return workspace(f'temp/{uuid.uuid4()}.tmp')
 
 
-def getTempDir():
-    return getWorkspace(f'temp/{uuid.uuid4()}')
+def temp_dir():
+    return workspace(f'temp/{uuid.uuid4()}')
 
 
-def changeRelative(target: Path | str, fromRelative: Path | str, toRelative: Path | str):
+def change_relative(target: Path | str, from_relative: Path | str, to_relative: Path | str):
     target = get(target)
-    fromRelative = get(fromRelative)
-    toRelative = get(toRelative)
-    assert target.is_relative_to(fromRelative)
-    return toRelative.joinpath(target.relative_to(fromRelative))
+    from_relative = get(from_relative)
+    to_relative = get(to_relative)
+    assert target.is_relative_to(from_relative)
+    return to_relative.joinpath(target.relative_to(from_relative))
 
 
-def openDir(dir: Path | str):
+def open_dir(dir: Path | str):
     os.system(f'start explorer {dir}')
 
 
-def _remove(*pathList: Path | str):
-    for path in pathList:
+def _remove(*ary: Path | str):
+    for path in ary:
         path = get(path)
         if path.is_file():
             path.unlink(True)
         elif path.is_dir():
             shutil.rmtree(path)
 
 
-async def remove(*pathList: Path | str):
-    return await bfunc.runInThread(
-        lambda: _remove(*pathList)
+async def remove(*ary: Path | str):
+    return await bfunc.run_thread(
+        lambda: _remove(*ary)
     )
 
 
-def _make(*pathList: Path | str):
-    for path in pathList:
+def _make(*ary: Path | str):
+    for path in ary:
         path = get(path)
         path.mkdir(parents=True, exist_ok=True)
 
 
-async def make(*pathList: Path | str):
-    return await bfunc.runInThread(
-        lambda: _make(*pathList)
+async def make(*ary: Path | str):
+    return await bfunc.run_thread(
+        lambda: _make(*ary)
     )
 
 
-def _clearDir(*dirList: Path | str):
-    for dir in dirList:
+def _clear_dir(*ary: Path | str):
+    for dir in ary:
         _remove(*[x for x in get(dir).iterdir()])
 
 
-async def clearDir(*dirList: Path | str):
-    return await bfunc.runInThread(
-        lambda: _clearDir(*dirList)
+async def clear_dir(*ary: Path | str):
+    return await bfunc.run_thread(
+        lambda: _clear_dir(*ary)
     )
 
 
 def _copy(src: Path | str, dst: Path | str):
     src = get(src)
     dst = get(dst)
     _make(dst.parent)
@@ -99,27 +100,27 @@
         if not src.exists():
             raise Exception(f'copy error: src not exists {src}')
         else:
             raise Exception(f'copy error: src not support {src}')
 
 
 async def copy(src: Path | str, dst: Path | str):
-    return await bfunc.runInThread(
+    return await bfunc.run_thread(
         lambda: _copy(src, dst)
     )
 
 
-def _copyMany(dataDict: dict[Path | str, Path | str]):
-    for src, dst in dataDict.items():
+def _copy_many(data: dict[Path | str, Path | str]):
+    for src, dst in data.items():
         _copy(src, dst)
 
 
-async def copyMany(dataDict: dict[Path | str, Path | str]):
-    return await bfunc.runInThread(
-        lambda: _copyMany(dataDict)
+async def copy_many(data: dict[Path | str, Path | str]):
+    return await bfunc.run_thread(
+        lambda: _copy_many(data)
     )
 
 
 def _move(src: Path | str, dst: Path | str, force: bool = False):
     src = get(src)
     dst = get(dst)
     if dst.exists():
@@ -128,112 +129,118 @@
         else:
             raise Exception(f'move error: dst exists {dst}')
     _make(dst.parent)
     os.rename(src, dst)
 
 
 async def move(src: Path | str, dst: Path | str, force: bool = False):
-    return await bfunc.runInThread(
+    return await bfunc.run_thread(
         lambda: _move(src, dst, force)
     )
 
 
-def _moveMany(dataDict: dict[Path | str, Path | str], force: bool = False):
-    for src, dst in dataDict.items():
+def _move_many(data: dict[Path | str, Path | str], force: bool = False):
+    for src, dst in data.items():
         _move(src, dst, force)
 
 
-async def moveMany(dataDict: dict[Path | str, Path | str], force: bool = False):
-    return await bfunc.runInThread(
-        lambda: _moveMany(dataDict, force)
+async def move_many(data: dict[Path | str, Path | str], force: bool = False):
+    return await bfunc.run_thread(
+        lambda: _move_many(data, force)
     )
 
 
-def renameName(src: Path | str, name: str):
+async def move_children(src: Path | str, dst: Path | str, force: bool = False):
+    for from_file in await list_path(src, True):
+        to_file = change_relative(from_file, src, dst)
+        await move(from_file, to_file, force)
+
+
+def rename_name(src: Path | str, name: str):
     src = get(src)
     src.rename(src.with_name(name))
 
 
-def renameStem(src: Path | str, stemName: str):
+def rename_stem(src: Path | str, stemName: str):
     src = get(src)
     src.rename(src.with_stem(stemName))
 
 
-def renameSuffix(src: Path | str, suffixName: str):
+def rename_suffix(src: Path | str, suffixName: str):
     src = get(src)
     src.rename(src.with_suffix(suffixName))
 
 
-def _listPath(path: Path | str, recursive: bool = False):
-    '''获取指定路径下文件以及目录列表'''
+def _list_path(path: Path | str, recursive: bool = False):
     path = get(path)
     if recursive:
         return list(path.glob('**/*'))
     else:
         return list(path.glob("*"))
 
 
-async def listPath(path: Path | str, recursive: bool = False):
-    return await bfunc.runInThread(
-        lambda: _listPath(path, recursive)
+async def list_path(path: Path | str, recursive: bool = False):
+    '''获取指定路径下文件以及目录列表'''
+    return await bfunc.run_thread(
+        lambda: _list_path(path, recursive)
     )
 
 
-def _listFile(path: Path | str, recursive: bool = False):
-    '''获取指定路径下文件列表'''
+def _list_file(path: Path | str, recursive: bool = False):
     path = get(path)
     if recursive:
         return list(filter(lambda x: x.is_file(), path.glob('**/*')))
     else:
         return list(filter(lambda x: x.is_file(), path.glob('*')))
 
 
-async def listFile(path: Path | str, recursive: bool = False):
-    return await bfunc.runInThread(
-        lambda: _listFile(path, recursive)
+async def list_file(path: Path | str, recursive: bool = False):
+    '''获取指定路径下文件列表'''
+    return await bfunc.run_thread(
+        lambda: _list_file(path, recursive)
     )
 
 
-def _listDir(path: Path | str, recursive: bool = False):
-    '''获取指定路径下目录列表'''
+def _list_dir(path: Path | str, recursive: bool = False):
     path = get(path)
     if recursive:
         return list(filter(lambda x: x.is_dir(), path.glob('**/*')))
     else:
         return list(filter(lambda x: x.is_dir(), path.glob('*')))
 
 
-async def listDir(path: Path | str, recursive: bool = False):
-    return await bfunc.runInThread(
-        lambda: _listDir(path, recursive)
+async def list_dir(path: Path | str, recursive: bool = False):
+    '''获取指定路径下目录列表'''
+    return await bfunc.run_thread(
+        lambda: _list_dir(path, recursive)
     )
 
 
 @asynccontextmanager
-async def useTempFile():
-    tempFile = getTempFile()
+async def use_temp_file():
+    file = temp_file()
     try:
-        yield tempFile
+        yield file
     finally:
-        await remove(tempFile)
+        await remove(file)
 
 
 @asynccontextmanager
-async def useTempDir(isMakeDir: bool = False):
-    tempDir = getTempDir()
-    if isMakeDir:
-        await make(tempDir)
+async def use_temp_dir(is_make: bool = False):
+    path = temp_dir()
+    if is_make:
+        await make(path)
     try:
-        yield tempDir
+        yield path
     finally:
-        await remove(tempDir)
+        await remove(path)
 
 
 @asynccontextmanager
-async def useDir(path: str | Path):
+async def use_dir(path: str | Path):
     path = Path(path)
     currentPath = os.getcwd()
     try:
         os.chdir(str(path))
         yield
     finally:
         os.chdir(currentPath)
```

### Comparing `benimang-0.2.2/beni/bplaywright.py` & `benimang-0.3.5/beni/bplaywright.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,96 +1,92 @@
 import os
 from contextlib import asynccontextmanager
-from typing import Any, cast
+from pathlib import Path
+from typing import Any
 
 from playwright.async_api import async_playwright
 from playwright.sync_api import BrowserContext, sync_playwright
 
 from beni import bpath
+from beni.btype import Null
 
-_testContext: BrowserContext | None = None
+_context: BrowserContext = Null
 
 
-def test(*, url: str = '', storage_state: str | None = None):
-    global _testContext
-    if not _testContext:
+def run(*, url: str = '', storage_state: str | Path | None = None):
+    global _context
+    if not _context:
         import nest_asyncio
         nest_asyncio.apply()
         os.environ['PWDEBUG'] = 'console'
         playwright = sync_playwright().start()
         browser = playwright.chromium.launch(headless=False, channel='chrome')
-        _testContext = browser.new_context(storage_state=cast(str, storage_state))
-    page = _testContext.new_page()
+        _context = browser.new_context(storage_state=storage_state)
+    page = _context.new_page()
     if url:
         page.goto(url)
     return page
 
 
-def testStorageState():
-    if _testContext:
-        _testContext.storage_state(path=bpath.getDesktop('storage_state.dat'))
+def save_storage_state(storage_state: str | Path | None = None):
+    if _context:
+        _context.storage_state(path=storage_state or bpath.desktop('storage_state.dat'))
 
 
 @asynccontextmanager
 async def page(
     *,
     browser: dict[str, Any] = {},
     context: dict[str, Any] = {},
     page: dict[str, Any] = {},
 ):
-    '''
-    ```py
+    '''```py
     browser={
         'headless': False,    # 显示浏览器UI
         'channel': 'chrome',  # 使用系统 Chrome 浏览器
     },
     context={
-        'storage_state': FILE_STATE,
+        'storage_state': STATE_FILE,
     },
-    ```
-    '''
+    ```'''
     async with async_playwright() as p:
         async with await p.chromium.launch(**browser) as b:
             async with await b.new_context(**context) as c:
                 async with await c.new_page(**page) as p:
                     yield p
 
 
 @asynccontextmanager
 async def context(
     *,
     browser: dict[str, Any] = {},
     context: dict[str, Any] = {},
 ):
-    '''
-    ```py
+    '''```py
     browser={
         'headless': False,    # 显示浏览器UI
         'channel': 'chrome',  # 使用系统 Chrome 浏览器
     },
     context={
-        'storage_state': FILE_STATE,
+        'storage_state': STATE_FILE,
     },
-    ```
-    '''
+    ```'''
     async with async_playwright() as p:
         async with await p.chromium.launch(**browser) as b:
             async with await b.new_context(**context) as c:
                 yield c
 
 
 @asynccontextmanager
 async def browser(
     *,
     browser: dict[str, Any] = {},
 ):
-    '''
-    ```py
+    '''```py
     browser={
         'headless': False,    # 显示浏览器UI
         'channel': 'chrome',  # 使用系统 Chrome 浏览器
     }
-    ```
-    '''
+    ```'''
     async with async_playwright() as p:
         async with await p.chromium.launch(**browser) as b:
             yield b
```

### Comparing `benimang-0.2.2/beni/bqiniu.py` & `benimang-0.3.5/beni/bqiniu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 from contextlib import asynccontextmanager
 from pathlib import Path
-from typing import Any, NamedTuple, Tuple, cast
+from typing import Any, Tuple, cast
 
 from qiniu import Auth, BucketManager, build_batch_delete, etag, put_file
 from qiniu.http import ResponseInfo
 
 from beni import bfunc, bhttp, bpath, bzip
 
 
-class QiniuItem(NamedTuple):
-    key: str
-    size: int
-    qetag: str
-    time: int
+class QiniuItem:
+    def __init__(self, data: Any) -> None:
+        self.key = data['key']
+        self.size = data['fsize']
+        self.qetag = data['hash']
+        self.time = data['putTime']
 
 
-_FileListResult = tuple[dict[str, Any], Any, Any]
+_ListResult = tuple[
+    dict[str, Any],
+    Any,
+    Any,
+]
 
 
 class QiniuBucket():
 
-    def __init__(self, bucket: str, baseUrl: str, ak: str, sk: str) -> None:
+    def __init__(self, bucket: str, url: str, ak: str, sk: str) -> None:
         self.q = Auth(ak, sk)
         self.bucket = bucket
-        self.baseUrl = baseUrl
+        self.url = url
 
-    async def uploadFile(self, key: str, localFile: Path | str):
+    async def upload(self, key: str, file: Path | str):
         token = self.q.upload_token(self.bucket, key)
-        _, info = await bfunc.runInThread(
-            lambda: cast(Tuple[Any, ResponseInfo], put_file(token, key, localFile, version='v2'))
+        _, info = await bfunc.run_thread(
+            lambda: cast(Tuple[Any, ResponseInfo], put_file(token, key, file, version='v2'))
         )
         assert info.exception is None
         assert info.status_code == 200
 
-    def getPrivateFileUrl(self, key: str):
-        return self.q.private_download_url(f'{self.baseUrl}/{key}')
+    def get_url(self, key: str):
+        return self.q.private_download_url(f'{self.url}/{key}')
 
     @asynccontextmanager
-    async def _downloadPrivateFile(self, key: str):
-        url = self.getPrivateFileUrl(key)
-        async with bpath.useTempFile() as tempFile:
-            tempFile = bpath.getTempFile()
-            await bhttp.download(url, tempFile)
-            assert tempFile.exists()
-            yield tempFile
-
-    async def downloadPrivateFile(self, key: str, localFile: Path | str):
-        async with self._downloadPrivateFile(key) as tempFile:
-            await bpath.move(tempFile, localFile, True)
-
-    async def downloadPrivateFileUnzip(self, key: str, outputDir: Path | str):
-        async with self._downloadPrivateFile(key) as tempFile:
-            async with bpath.useTempDir() as tempDir:
-                await bzip.unzip(tempFile, tempDir)
-                for file in await bpath.listFile(tempDir, True):
-                    toFile = bpath.changeRelative(file, tempDir, outputDir)
-                    await bpath.move(file, toFile, True)
-
-    async def downloadPrivateFileSevenUnzip(self, key: str, outputDir: Path | str):
-        async with self._downloadPrivateFile(key) as tempFile:
-            async with bpath.useTempDir() as tempDir:
-                await bzip.sevenUnzip(tempFile, tempDir)
-                for file in await bpath.listFile(tempDir, True):
-                    toFile = bpath.changeRelative(file, tempDir, outputDir)
-                    await bpath.move(file, toFile, True)
+    async def _download(self, key: str):
+        url = self.get_url(key)
+        async with bpath.use_temp_file() as tempfile:
+            await bhttp.download(url, tempfile)
+            assert tempfile.exists()
+            yield tempfile
+
+    async def download(self, key: str, file: Path | str, force: bool = False):
+        async with self._download(key) as tempfile:
+            await bpath.move(tempfile, file, force)
+
+    async def download_unzip(self, key: str, output: Path | str):
+        async with self._download(key) as tempfile:
+            async with bpath.use_temp_dir() as tempdir:
+                await bzip.unzip(tempfile, tempdir)
+                await bpath.move_children(tempdir, output, True)
+
+    async def download_seven_unzip(self, key: str, output: Path | str):
+        async with self._download(key) as tempfile:
+            async with bpath.use_temp_dir() as tempdir:
+                await bzip.seven_unzip(tempfile, tempdir)
+                await bpath.move_children(tempdir, output, True)
 
-    async def getFileList(self, prefix: str, limit: int = 100) -> tuple[list[QiniuItem], str | None]:
+    async def get_list(self, prefix: str, limit: int = 100):
         bucket = BucketManager(self.q)
-        result, _, _ = await bfunc.runInThread(
-            lambda: cast(_FileListResult, bucket.list(self.bucket, prefix, None, limit))
+        result, _, _ = await bfunc.run_thread(
+            lambda: cast(_ListResult, bucket.list(self.bucket, prefix, None, limit))
         )
         assert type(result) is dict
-        fileList = [QiniuItem(x['key'], x['fsize'], x['hash'], x['putTime']) for x in result['items']]
-        return fileList, cast(str | None, result.get('marker', None))
+        ary = [QiniuItem(x) for x in result['items']]
+        return ary, cast(str | None, result.get('marker', None))
 
-    async def getFileListByMarker(self, marker: str, limit: int = 100):
+    async def get_list_by_marker(self, marker: str, limit: int = 100):
         bucket = BucketManager(self.q)
-        result, _, _ = await bfunc.runInThread(
-            lambda: cast(_FileListResult, bucket.list(self.bucket, None, marker, limit))
+        result, _, _ = await bfunc.run_thread(
+            lambda: cast(_ListResult, bucket.list(self.bucket, None, marker, limit))
         )
         assert type(result) is dict
-        fileList = [QiniuItem(x['key'], x['fsize'], x['hash'], x['putTime']) for x in result['items']]
-        return fileList, cast(str | None, result.get('marker', None))
+        ary = [QiniuItem(x) for x in result['items']]
+        return ary, cast(str | None, result.get('marker', None))
 
-    async def deleteFiles(self, *keyList: str):
+    async def delete_files(self, *keyList: str):
         bucket = BucketManager(self.q)
-        result, _ = await bfunc.runInThread(
+        result, _ = await bfunc.run_thread(
             lambda: cast(tuple[Any, Any], bucket.batch(build_batch_delete(self.bucket, keyList)))
         )
         assert result
 
-    async def hashFile(self, file: Path | str):
-        return await bfunc.runInThread(
+    async def hash_file(self, file: Path | str):
+        return await bfunc.run_thread(
             lambda: etag(file)
         )
```

### Comparing `benimang-0.2.2/beni/bsqlite.py` & `benimang-0.3.5/beni/bsqlite.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,347 +2,342 @@
 
 import asyncio
 import re
 import sqlite3
 import time
 from contextlib import asynccontextmanager
 from pathlib import Path
-from typing import Any, Final, Sequence, cast
+from typing import Any, Sequence, cast
 
 import aiosqlite
 import orjson
 from pydantic import BaseModel
 
-from beni import block, bpath
-from beni.bfunc import getSqlPlacement
+from beni import bfunc, block, bpath
+from beni.btype import Null
 
 sqlite3.register_converter(
     "bool",
     lambda x: x not in (
         b'',
         b'0',
         # None, # 如果是None根本就不会进来，这里判断也没有意义
     )
 )
 
-_ALIVE: Final = 5 * 60  # 数据库链接至少存活时间（因为清除不是实时执行）
+_ALIVE = 5 * 60  # 数据库链接至少存活时间（因为清除不是实时执行）
 
 
-class SqliteDbPool:
+class SqliteDb:
 
-    _isRunningClean = False
-
-    def __init__(self, dbFile: str | Path, maxConnections: int = 10):
-        self._avaliableList: asyncio.Queue[_SqliteDbWrite] = asyncio.Queue()
-        self.lock = block.RWLock(maxConnections)
-        if type(dbFile) is Path:
-            self._dbFile = dbFile
-        else:
-            self._dbFile = bpath.get(dbFile)
+    def __init__(self, file: str | Path, max_num: int = 10):
+        self._ary: asyncio.Queue[_SqliteDbWrite] = asyncio.Queue()
+        self.lock = block.RWLock(max_num)
+        self._file = bpath.get(file)
+        self._rtime_dict: dict[int, float] = {}  # rtime = release time
+        asyncio.create_task(self._clean())
 
     def exists(self):
-        return self._dbFile.exists()
+        return self._file.exists()
 
     async def _clean(self):
         while True:
             await asyncio.sleep(_ALIVE)
             now = time.monotonic()
-            dbList: list[_SqliteDbWrite] = []
-            while not self._avaliableList.empty():
-                db = self._avaliableList.get_nowait()
-                if now - db._releaseTime > _ALIVE:  # type: ignore
+            ary: list[_SqliteDbWrite] = []
+            while not self._ary.empty():
+                db = self._ary.get_nowait()
+                db_key = id(db)
+                release_time = self._rtime_dict[db_key]
+                if now - release_time > _ALIVE:
+                    del self._rtime_dict[db_key]
                     await db.close()
                 else:
-                    dbList.append(db)
-            for db in dbList:
-                self._avaliableList.put_nowait(db)
-
-    async def close(self, isWriteLock: bool = True):
-        if isWriteLock:
-            await self.lock.getWrite()
-        while not self._avaliableList.empty():
-            db = self._avaliableList.get_nowait()
+                    ary.append(db)
+            for db in ary:
+                self._ary.put_nowait(db)
+
+    async def close(self, write_lock: bool = True):
+        if write_lock:
+            await self.lock.get_write()
+        while not self._ary.empty():
+            db = self._ary.get_nowait()
             await db.close()
-        if isWriteLock:
-            self.lock.releaseWrite()
+        if write_lock:
+            self.lock.release_write()
 
-    async def _getDb(self):
-        if self._avaliableList.empty():
+    async def _get_db(self):
+        if self._ary.empty():
             db = _SqliteDbWrite()
-            await db.connect(self._dbFile)
-            #
-            if not self._isRunningClean:
-                self._isRunningClean = True
-                asyncio.create_task(self._clean())
+            await db.connect(self._file)
         else:
-            db = self._avaliableList.get_nowait()
+            db = self._ary.get_nowait()
         return db
 
-    def _releaseDb(self, db: _SqliteDbWrite):
-        db._releaseTime = time.monotonic()  # type: ignore 访问私有变量
-        self._avaliableList.put_nowait(db)
+    def _release_db(self, db: _SqliteDbWrite):
+        self._rtime_dict[id(db)] = time.monotonic()
+        self._ary.put_nowait(db)
 
     @asynccontextmanager
-    async def _useDb(self):
-        db = await self._getDb()
+    async def _use_db(self):
+        db = await self._get_db()
         try:
             yield db
         finally:
-            self._releaseDb(db)
+            self._release_db(db)
 
     @asynccontextmanager
     async def read(self):
-        async with self.lock.useRead():
-            async with self._useDb() as db:
+        async with self.lock.use_read():
+            async with self._use_db() as db:
                 yield cast(_SqliteDbRead, db)
 
     @asynccontextmanager
     async def write(self):
-        async with self.lock.useWrite():
-            async with self._useDb() as db:
+        async with self.lock.use_write():
+            async with self._use_db() as db:
                 try:
                     yield db
                     await db.commit()
                 except:
                     await db.rollback()
                     raise
 
     async def add(self, table: str, data: dict[str, Any]):
         async with self.write() as db:
             return await db.add(table, data)
 
-    async def addList(self, table: str, dataList: list[dict[str, Any]]):
+    async def add_ary(self, table: str, ary: list[dict[str, Any]]):
         async with self.write() as db:
-            return await db.addList(table, dataList)
+            return await db.add_ary(table, ary)
 
-    async def update(self, table: str, data: dict[str, Any], statement: str = '', *whereValues: Any):
+    async def update(self, table: str, data: dict[str, Any], statement: str = '', *args: Any):
         async with self.write() as db:
-            return await db.update(table, data, statement, *whereValues)
+            return await db.update(table, data, statement, *args)
 
-    async def get(self, sql: str, *parameters: Any):
+    async def get(self, sql: str, *args: Any):
         async with self.read() as db:
-            return await db.get(sql, *parameters)
+            return await db.get(sql, *args)
 
-    async def getList(self, sql: str, *parameters: Any):
+    async def getList(self, sql: str, *args: Any):
         async with self.read() as db:
-            return await db.getList(sql, *parameters)
+            return await db.get_ary(sql, *args)
 
-    async def value(self, sql: str, *parameters: Any):
+    async def value(self, sql: str, *args: Any):
         async with self.read() as db:
-            return await db.value(sql, *parameters)
+            return await db.value(sql, *args)
 
-    async def execute(self, sql: str, *parameters: Any):
+    async def execute(self, sql: str, *args: Any):
         async with self.write() as db:
-            return await db.execute(sql, *parameters)
+            return await db.execute(sql, *args)
 
 
 class _SqliteDbRead:
 
-    _db: aiosqlite.Connection
-    _releaseTime = 0.0
+    _db: aiosqlite.Connection = Null
 
-    async def connect(self, db_file: Path | str):
-        self._db = await aiosqlite.connect(db_file, detect_types=sqlite3.PARSE_DECLTYPES)
+    async def connect(self, file: Path | str):
+        self._db = await aiosqlite.connect(file, detect_types=sqlite3.PARSE_DECLTYPES)
         self._db.row_factory = sqlite3.Row
 
     async def close(self):
         await self._db.close()
 
-    async def get(self, sql: str, *parameters: Any):
-        async with self._db.execute(sql, parameters) as cursor:
+    async def get(self, sql: str, *args: Any):
+        async with self._db.execute(sql, args) as cursor:
             return await cursor.fetchone()
 
-    async def getList(self, sql: str, *parameters: Any):
-        async with self._db.execute(sql, parameters) as cursor:
+    async def get_ary(self, sql: str, *args: Any):
+        async with self._db.execute(sql, args) as cursor:
             return cast(list[sqlite3.Row], await cursor.fetchall())
 
-    async def value(self, sql: str, *parameters: Any):
-        row = await self.get(sql, *parameters)
+    async def value(self, sql: str, *args: Any):
+        row = await self.get(sql, *args)
         assert row
         return row[0]
 
 
 class _SqliteDbWrite(_SqliteDbRead):
 
     async def add(self, table: str, data: dict[str, Any]):
-        keylist = sorted(data.keys())
-        fieldname_list = ','.join([f'"{x}"' for x in keylist])
-        fieldvalue_list = [data[x] for x in keylist]
+        keys = sorted(data.keys())
+        names = ','.join([f'"{x}"' for x in keys])
+        values = [data[x] for x in keys]
         async with self._db.execute(
             f'''
-            INSERT INTO `{table}` ({fieldname_list})
+            INSERT INTO `{table}` ({names})
             VALUES
-                {getSqlPlacement(keylist)}
+                {bfunc.get_sql_placement(keys)}
             ''',
-            fieldvalue_list,
+            values,
         ) as cursor:
             return cursor.lastrowid
 
-    async def addList(self, table: str, dataList: list[dict[str, Any]]):
+    async def add_ary(self, table: str, ary: list[dict[str, Any]]):
         keyset: set[str] = set()
-        for data in dataList:
+        for data in ary:
             keyset.update(data.keys())
-        keylist = sorted(keyset)
-        fieldname_list = ','.join([f'`{x}`' for x in keylist])
-        fieldvalue_list = [[data.get(key) for key in keylist] for data in dataList]
+        keys = sorted(keyset)
+        names = ','.join([f'`{x}`' for x in keys])
+        values = [[data.get(key) for key in keys] for data in ary]
         async with self._db.executemany(
             f'''
-            INSERT INTO `{table}` ({fieldname_list})
+            INSERT INTO `{table}` ({names})
             VALUES
-                {getSqlPlacement(keylist)}
+                {bfunc.get_sql_placement(keys)}
             ''',
-            fieldvalue_list
+            values
         ) as cursor:
             return cursor.rowcount
 
-    async def update(self, table: str, data: dict[str, Any], statement: str = '', *whereValues: Any):
-        keylist = sorted(data.keys())
-        fieldname_list = ','.join([f'`{x}`=?' for x in keylist])
-        fieldvalue_list = [data[x] for x in keylist] + list(whereValues)
+    async def update(self, table: str, data: dict[str, Any], statement: str = '', *args: Any):
+        keys = sorted(data.keys())
+        names = ','.join([f'`{x}`=?' for x in keys])
+        values = [data[x] for x in keys] + list(args)
         async with self._db.execute(
             f'''
             UPDATE `{table}`
-            SET {fieldname_list}
+            SET {names}
             {statement}
             ''',
-            fieldvalue_list,
+            values,
         ) as cursor:
             return cursor.rowcount
 
-    async def execute(self, sql: str, *parameters: Any):
-        async with self._db.execute(sql, parameters) as cursor:
+    async def execute(self, sql: str, *args: Any):
+        async with self._db.execute(sql, args) as cursor:
             return cursor.rowcount
 
     async def commit(self):
         return await self._db.commit()
 
     async def rollback(self):
         return await self._db.rollback()
 
 
-_RE_TABLE_NAME: Final = re.compile(r'(.*?)Model$')
+_RE_TABLE = re.compile(r'(.*?)Model$')
 
 
 class SqliteDbModel(BaseModel):
 
-    __tableName__ = ''
+    __table__ = ''
 
-    _db: SqliteDbPool = cast(SqliteDbPool, None)
+    _db: SqliteDb = Null
 
     class Config:
         json_loads = orjson.loads
         json_dumps = orjson.dumps
 
     @classmethod
-    def setDb(cls, data: SqliteDbPool):
-        cls._db = data
+    def set_db(cls, db: SqliteDb):
+        cls._db = db
 
     @classmethod
-    def getDb(cls):
+    def get_db(cls):
         return cls._db
 
     @classmethod
     @property
-    def TableName(cls):
-        if not cls.__tableName__:
-            name: str = _RE_TABLE_NAME.findall(cls.__name__)[0]
-            nameList = list(name)
-            nameList[0] = nameList[0].lower()
-            for i in range(len(nameList)):
-                v = nameList[i]
+    def TABLE(cls):
+        if not cls.__table__:
+            name: str = _RE_TABLE.findall(cls.__name__)[0]
+            name_ary = list(name)
+            name_ary[0] = name_ary[0].lower()
+            for i in range(len(name_ary)):
+                v = name_ary[i]
                 if v.isupper():
-                    nameList[i] = f'_{v.lower()}'
-            result = ''.join(nameList)
-            cls.__tableName__ = result
-        return cls.__tableName__
+                    name_ary[i] = f'_{v.lower()}'
+            result = ''.join(name_ary)
+            cls.__table__ = result
+        return cls.__table__
 
     async def add(self):
         return await self._add()
 
     async def _add(self, exclude: set[str] | None = None, include: set[str] | None = None):
         return await self._db.add(
-            self.TableName,
+            self.TABLE,
             self.dict(
                 exclude=cast(Any, exclude),
                 include=cast(Any, include),
             )
         )
 
     @classmethod
-    async def addList(cls, modelList: Sequence[SqliteDbModel]):
-        return await cls._addList(modelList)
+    async def add_ary(cls, ary: Sequence[SqliteDbModel]):
+        return await cls._add_ary(ary)
 
     @classmethod
-    async def _addList(cls, modelList: Sequence[SqliteDbModel], exclude: set[str] | None = None):
-        if not modelList:
+    async def _add_ary(cls, ary: Sequence[SqliteDbModel], exclude: set[str] | None = None):
+        if not ary:
             return 0
-        return await cls._db.addList(
-            cls.TableName,
-            [x.dict(exclude=cast(Any, exclude)) for x in modelList],
+        return await cls._db.add_ary(
+            cls.TABLE,
+            [x.dict(exclude=exclude) for x in ary],
         )
 
-    async def _update(self, statement: str = '', *parList: Any, exclude: set[str] | None = None, include: set[str] | None = None):
+    async def _update(self, statement: str = '', *args: Any, exclude: set[str] | None = None, include: set[str] | None = None):
         return await self._db.update(
-            self.TableName,
+            self.TABLE,
             self.dict(
-                exclude=cast(Any, exclude),
-                include=cast(Any, include),
+                exclude=exclude,
+                include=include,
             ),
             statement,
-            *parList,
+            *args,
         )
 
     @classmethod
-    async def removeAll(cls):
+    async def remove_all(cls):
         return await cls._db.execute(
-            f'DELETE FROM {cls.TableName}',
+            f'DELETE FROM {cls.TABLE}',
         )
 
     @classmethod
-    async def _remove(cls, statement: str = '', *parList: Any):
+    async def _remove(cls, statement: str = '', *args: Any):
         return await cls._db.execute(
-            f'DELETE FROM {cls.TableName} {statement}',
-            *parList,
+            f'DELETE FROM {cls.TABLE} {statement}',
+            *args,
         )
 
     @classmethod
-    async def _get(cls, statement: str = '', *parList: Any, fields: set[str] | None = None):
+    async def _get(cls, statement: str = '', *args: Any, fields: set[str] | None = None):
         row = await cls._db.get(
             f'''
             SELECT
                 {fields and ', '.join(fields) or '*'}
             FROM
-                `{cls.TableName}`
+                `{cls.TABLE}`
             {statement}
             LIMIT 1
             ''',
-            *parList,
+            *args,
         )
         if row:
             return cls(**dict(row))
 
     @classmethod
-    async def _getList(cls, statement: str = '', *parList: Any, fields: set[str] | None = None):
-        rowList = await cls._db.getList(
+    async def _get_ary(cls, statement: str = '', *args: Any, fields: set[str] | None = None):
+        rows = await cls._db.getList(
             f'''
             SELECT
                 {fields and ', '.join(fields) or '*'}
             FROM
-                `{cls.TableName}`
+                `{cls.TABLE}`
             {statement}
             ''',
-            *parList,
+            *args,
         )
-        return [cls(**dict(x)) for x in rowList]
+        return [cls(**dict(x)) for x in rows]
 
     @classmethod
-    async def _count(cls, statement: str = '', *parList: Any) -> int:
+    async def _count(cls, statement: str = '', *args: Any) -> int:
         return await cls._db.value(
             f'''
             SELECT
                 COUNT( * )
             FROM
-                `{cls.TableName}`
+                `{cls.TABLE}`
             {statement}
             ''',
-            *parList,
+            *args,
         )
```

### Comparing `benimang-0.2.2/beni/bstorage.py` & `benimang-0.3.5/beni/bstorage.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import Any, Final
+from typing import Any
 
 from beni import bfile, bpath
 
 
 async def get(key: str, default: Any = None):
-    storageFile = _getStorageFile(key)
-    if storageFile.is_file():
-        return await bfile.readYaml(storageFile)
+    file = _get_file(key)
+    if file.is_file():
+        return await bfile.read_yaml(file)
     else:
         return default
 
 
 async def set(key: str, value: Any):
-    storageFile = _getStorageFile(key)
-    await bfile.writeYaml(storageFile, value)
+    file = _get_file(key)
+    await bfile.write_yaml(file, value)
 
 
-async def clear(*keyList: str):
-    await bpath.remove(*[_getStorageFile(key) for key in keyList])
+async def remove(*args: str):
+    await bpath.remove(*[_get_file(key) for key in args])
 
 
-async def clearAll():
-    fileList = await bpath.listFile(_storagePath)
-    await bpath.remove(*fileList)
+async def remove_all():
+    file_ary = await bpath.list_file(_DIR)
+    await bpath.remove(*file_ary)
 
 
 # ------------------------------------------------------------------------------------------
 
-_storagePath: Final = bpath.getWorkspace('.storage')
+_DIR = bpath.workspace('.storage')
 
 
-def _getStorageFile(key: str):
-    return bpath.get(_storagePath, f'{key}.yaml')
+def _get_file(key: str):
+    return bpath.get(_DIR, f'{key}.yaml')
```

### Comparing `benimang-0.2.2/beni/btable.py` & `benimang-0.3.5/beni/btable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-from typing import Any, Callable, Final, Sequence, Tuple, TypeVar
+from typing import Any, Callable, Sequence, Tuple
 
 import colorama
 
 from beni import bcolor
-
-_T = TypeVar('_T')
+from beni.btype import AnyType
 
 
 def get(
-    data_list: Sequence[_T],
+    data_list: Sequence[AnyType],
     *,
     title: str | None = None,
-    fields: Sequence[Tuple[str, Callable[[_T], Any]]],
+    fields: Sequence[Tuple[str, Callable[[AnyType], Any]]],
     rowcolor: Callable[[list[Any]], Any] | None = None,
     extend: list[list[Any]] | None = None,
     isPrint: bool = False,
 ):
-    header_color: Final = colorama.Fore.YELLOW
+    HEADER_COLOR = colorama.Fore.YELLOW
     from prettytable import PrettyTable
     table = PrettyTable()
     if title:
-        table.title = bcolor.getStr(title, header_color)
-    field_funclist: list[Callable[[_T], Any]] = []
+        table.title = bcolor.get_str(title, HEADER_COLOR)
+    field_funclist: list[Callable[[AnyType], Any]] = []
     field_namelist: list[str] = []
     align_dict: dict[str, str] = {}
     for i in range(len(fields)):
         item = fields[i]
         field_funclist.append(item[1])
         field_name = item[0]
         if field_name.endswith('>'):
             field_name = field_name[:-1]
             align_dict[field_name] = 'r'
         elif field_name.endswith('<'):
             field_name = field_name[:-1]
             align_dict[field_name] = 'l'
         field_namelist.append(field_name)
-    table.field_names = [bcolor.getStr(x, header_color) for x in field_namelist]
+    table.field_names = [bcolor.get_str(x, HEADER_COLOR) for x in field_namelist]
     for k, v in align_dict.items():
-        table.align[bcolor.getStr(k, header_color)] = v
+        table.align[bcolor.get_str(k, HEADER_COLOR)] = v
     row_list: list[list[Any]] = []
     for data in data_list:
         row = [func(data) for func in field_funclist]
         row_list.append(row)
     if extend:
         for row in extend:
             newRow = row[:]
@@ -49,13 +48,13 @@
                 newRow.extend([''] * (len(fields) - len(newRow)))
             row_list.append(newRow)
     if rowcolor:
         for row in row_list:
             color = rowcolor(row)
             if color:
                 for i in range(len(row)):
-                    row[i] = bcolor.getStr(row[i], color)
+                    row[i] = bcolor.get_str(row[i], color)
     table.add_rows(row_list)
     tableStr = str(table.get_string())
     if isPrint:
         print(f'\n{tableStr}\n')
     return tableStr
```

### Comparing `benimang-0.2.2/beni/btime.py` & `benimang-0.3.5/beni/btime.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import datetime as xdatetime
 import time as xtime
 
 from beni import bhttp
 
-_serverTime: float = xtime.time()
-_initTime: float = xtime.monotonic()
+_server_time: float = xtime.time()
+_init_time: float = xtime.monotonic()
 
 
-async def networkTime():
+async def network():
     _, response = await bhttp.get('https://www.baidu.com')
     date_str = response.headers['Date']
     return xdatetime.datetime.strptime(date_str, '%a, %d %b %Y %H:%M:%S GMT') + xdatetime.timedelta(hours=8)
 
 
-async def initServerDatetime():
-    global _serverTime, _initTime
-    _serverTime = (await networkTime()).timestamp()
-    _initTime = xtime.monotonic()
+async def init_server_time():
+    global _server_time, _init_time
+    _server_time = (await network()).timestamp()
+    _init_time = xtime.monotonic()
 
 
 def timestamp():
-    return _serverTime + xtime.monotonic() - _initTime
+    return _server_time + xtime.monotonic() - _init_time
 
 
-def timestampSecond():
+def timestamp_sec():
     return int(timestamp())
 
 
-def timestampMillisecond():
+def timestamp_millsec():
     return int(timestamp() * 1000)
 
 
 def datetime():
     return xdatetime.datetime.fromtimestamp(timestamp())
 
 
@@ -39,36 +39,25 @@
     return xdatetime.date.fromtimestamp(timestamp())
 
 
 def time():
     return datetime().time()
 
 
-def datetimeStr(fmt: str = r'%Y-%m-%d %H:%M:%S'):
+def datetime_str(fmt: str = r'%Y-%m-%d %H:%M:%S'):
     return datetime().strftime(fmt)
 
 
-def dateStr(fmt: str = r'%Y-%m-%d'):
+def date_str(fmt: str = r'%Y-%m-%d'):
     return date().strftime(fmt)
 
 
-def timeStr(fmt: str = r'%H:%M:%S'):
+def time_str(fmt: str = r'%H:%M:%S'):
     return time().strftime(fmt)
 
 
-def makeDatetime(date_str: str, fmt: str = r'%Y-%m-%d %H:%M:%S'):
+def make_datetime(date_str: str, fmt: str = r'%Y-%m-%d %H:%M:%S'):
     return xdatetime.datetime.strptime(date_str, fmt)
 
 
-def makeDate(date_str: str, fmt: str = r'%Y-%m-%d'):
+def make_date(date_str: str, fmt: str = r'%Y-%m-%d'):
     return xdatetime.datetime.strptime(date_str, fmt).date()
-
-
-# def tomorrowDatetime():
-#     return datetime.datetime.combine(
-#         nowDate(),
-#         datetime.time(),
-#     )
-
-
-# def foreverDatetime():
-#     return datetime.datetime(9999, 1, 1)
```

### Comparing `benimang-0.2.2/benimang.egg-info/SOURCES.txt` & `benimang-0.3.5/benimang.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 README.md
 pyproject.toml
 beni/__init__.py
 beni/bbyte.py
 beni/bcache.py
 beni/bcmd.py
 beni/bcolor.py
+beni/bdefine.py
 beni/bexecute.py
 beni/bfile.py
 beni/bfunc.py
+beni/bhash.py
 beni/bhttp.py
 beni/binput.py
 beni/block.py
 beni/blog.py
 beni/bpath.py
 beni/bplaywright.py
 beni/bprogress.py
 beni/bqiniu.py
 beni/bsqlite.py
 beni/bstorage.py
 beni/btable.py
 beni/btask.py
 beni/btime.py
+beni/btype.py
 beni/bzip.py
 benimang.egg-info/PKG-INFO
 benimang.egg-info/SOURCES.txt
 benimang.egg-info/dependency_links.txt
 benimang.egg-info/entry_points.txt
 benimang.egg-info/requires.txt
 benimang.egg-info/top_level.txt
```

### Comparing `benimang-0.2.2/pyproject.toml` & `benimang-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "benimang"
-version = "0.2.2"
+version = "0.3.5"
 description = "utils library for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni"]
 authors = [
   {email = "benimang@126.com"},
   {name = "Beni Mang"}
 ]
```

### Comparing `benimang-0.2.2/test/test_sample.py` & `benimang-0.3.5/test/test_sample.py`

 * *Files identical despite different names*

