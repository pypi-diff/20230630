# Comparing `tmp/voicemeeter-compact-1.8.1.tar.gz` & `tmp/voicemeeter_compact-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter-compact-1.8.1.tar", max compression
+gzip compressed data, was "voicemeeter_compact-1.8.2.tar", max compression
```

## Comparing `voicemeeter-compact-1.8.1.tar` & `voicemeeter_compact-1.8.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter-compact-1.8.1/LICENSE
--rw-r--r--   0        0        0      730 2023-06-29 18:09:21.736138 voicemeeter-compact-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter-compact-1.8.1/README.md
--rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter-compact-1.8.1/vmcompact/__init__.py
--rw-r--r--   0        0        0     4644 2023-06-29 17:12:44.240157 voicemeeter-compact-1.8.1/vmcompact/app.py
--rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter-compact-1.8.1/vmcompact/banner.py
--rw-r--r--   0        0        0    23309 2023-06-29 11:15:56.815136 voicemeeter-compact-1.8.1/vmcompact/builders.py
--rw-r--r--   0        0        0    10867 2023-06-29 10:15:56.869547 voicemeeter-compact-1.8.1/vmcompact/channels.py
--rw-r--r--   0        0        0     9634 2023-06-26 08:40:26.219945 voicemeeter-compact-1.8.1/vmcompact/config.py
--rw-r--r--   0        0        0     2661 2023-06-29 18:10:03.397989 voicemeeter-compact-1.8.1/vmcompact/configurations.py
--rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter-compact-1.8.1/vmcompact/data.py
--rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter-compact-1.8.1/vmcompact/errors.py
--rw-r--r--   0        0        0     8960 2023-06-29 10:16:01.341472 voicemeeter-compact-1.8.1/vmcompact/gainlayer.py
--rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter-compact-1.8.1/vmcompact/img/cat.ico
--rw-r--r--   0        0        0    17472 2023-06-29 11:09:26.649143 voicemeeter-compact-1.8.1/vmcompact/menu.py
--rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter-compact-1.8.1/vmcompact/navigation.py
--rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter-compact-1.8.1/vmcompact/subject.py
--rw-r--r--   0        0        0     7183 2023-06-29 18:13:16.117955 voicemeeter-compact-1.8.1/setup.py
--rw-r--r--   0        0        0     6857 2023-06-29 18:13:16.118955 voicemeeter-compact-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-04-27 02:09:14.944574 voicemeeter_compact-1.8.2/LICENSE
+-rw-r--r--   0        0        0      730 2023-06-30 03:26:36.376204 voicemeeter_compact-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     6287 2022-09-15 02:49:35.375182 voicemeeter_compact-1.8.2/README.md
+-rw-r--r--   0        0        0       51 2022-04-27 02:09:14.959298 voicemeeter_compact-1.8.2/vmcompact/__init__.py
+-rw-r--r--   0        0        0     4672 2023-06-30 03:20:03.642634 voicemeeter_compact-1.8.2/vmcompact/app.py
+-rw-r--r--   0        0        0     1123 2023-06-30 02:12:19.037717 voicemeeter_compact-1.8.2/vmcompact/banner.py
+-rw-r--r--   0        0        0    23309 2023-06-30 02:12:19.039884 voicemeeter_compact-1.8.2/vmcompact/builders.py
+-rw-r--r--   0        0        0    10867 2023-06-30 02:12:19.040693 voicemeeter_compact-1.8.2/vmcompact/channels.py
+-rw-r--r--   0        0        0     9634 2023-06-30 02:12:19.042695 voicemeeter_compact-1.8.2/vmcompact/config.py
+-rw-r--r--   0        0        0     2661 2023-06-30 02:12:19.043695 voicemeeter_compact-1.8.2/vmcompact/configurations.py
+-rw-r--r--   0        0        0     2124 2023-06-30 02:12:19.045865 voicemeeter_compact-1.8.2/vmcompact/data.py
+-rw-r--r--   0        0        0       88 2023-06-30 02:12:19.046924 voicemeeter_compact-1.8.2/vmcompact/errors.py
+-rw-r--r--   0        0        0     8960 2023-06-30 02:12:19.049103 voicemeeter_compact-1.8.2/vmcompact/gainlayer.py
+-rw-r--r--   0        0        0   112922 2022-04-27 02:09:14.966281 voicemeeter_compact-1.8.2/vmcompact/img/cat.ico
+-rw-r--r--   0        0        0    17472 2023-06-30 02:12:19.050808 voicemeeter_compact-1.8.2/vmcompact/menu.py
+-rw-r--r--   0        0        0     3785 2023-06-30 02:12:19.051694 voicemeeter_compact-1.8.2/vmcompact/navigation.py
+-rw-r--r--   0        0        0      854 2022-09-15 02:49:35.423185 voicemeeter_compact-1.8.2/vmcompact/subject.py
+-rw-r--r--   0        0        0     7187 1970-01-01 00:00:00.000000 voicemeeter_compact-1.8.2/setup.py
+-rw-r--r--   0        0        0     6908 1970-01-01 00:00:00.000000 voicemeeter_compact-1.8.2/PKG-INFO
```

### Comparing `voicemeeter-compact-1.8.1/LICENSE` & `voicemeeter_compact-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/pyproject.toml` & `voicemeeter_compact-1.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-compact"
-version = "1.8.1"
+version = "1.8.2"
 description = "A Compact Voicemeeter Remote App"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-compact"
 
 packages = [{ include = "vmcompact" }]
```

### Comparing `voicemeeter-compact-1.8.1/README.md` & `voicemeeter_compact-1.8.2/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-[![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![OS: Windows](https://img.shields.io/badge/os-windows-red)
-
-![Image of app/potato size comparison](./doc_imgs/potatocomparisonsmaller.png)
-
-# Voicemeeter Compact
-
-A compact Voicemeeter remote app, works locally and over LAN.
-
-For an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)
-
-## Prerequisites
-
--   [Voicemeeter](https://voicemeeter.com/) (Basic v1.0.8.4), (Banana v2.0.6.4) or (Potato v3.0.2.4)
--   Python 3.10 or greater
-
-## Installation
-
-For a step-by-step guide [click here](INSTALLATION.md)
-
-```
-pip install voicemeeter-compact
-```
-
-## Usage
-
-Example `__main__.py` file:
-
-```python
-import voicemeeterlib
-import vmcompact
-
-
-def main():
-    # pass the kind_id and the vm object to the app
-    with voicemeeterlib.api(kind_id) as vm:
-        app = vmcompact.connect(kind_id, vm)
-        app.mainloop()
-
-
-if __name__ == "__main__":
-    # choose the kind of Voicemeeter (Local connection)
-    kind_id = "banana"
-
-    main()
-```
-
-It's important to know that only labelled strips and buses will appear in the Channel frames. Removing a Channels label will cause the GUI to grow/shrink in real time.
-
-![Image of unlabelled app](./doc_imgs/nolabels.png)
-
-If the GUI looks like the above when you first load it, then no channels are labelled. From the menu, `Configs->Load config` you may load an example config. Save your current Voicemeeter settings first :).
-
-### kind_id
-
-Set the kind of Voicemeeter, kind_id may be:
-
--   `basic`
--   `banana`
--   `potato`
-
-## TOML Files
-
-This is how your files should be organised. Wherever your `__main__.py` file is located (after install this can be any location), `configs` should be in the same location.
-Directly inside of configs directory you may place an app.toml, vban.toml and a directory for each kind.
-Inside each kind directory you may place as many custom toml configurations as you wish.
-
-.
-
-├── `__main__.py`
-
-├── configs
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── app.toml
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── vban.toml
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── basic
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other_config.toml
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── streaming_config.toml
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── banana
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other.toml
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── potato
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml
-
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...
-
-## Configs
-
-### app.toml
-
-Configure certain startup states for the app.
-
--   `configs`
-    Configure a user config to load on app startup. Don't include the .toml extension in the config name.
-
--   `theme`
-    By default the app loads up the [Sun Valley light or dark theme](https://github.com/rdbende/Sun-Valley-ttk-theme) by @rdbende. You have the option to load up the app without any theme loaded. Simply set `enabled` to false and `mode` will take no effect.
-
--   `extends`
-    Extending the app will show both strips and buses. In reduced mode only one or the other. This app will extend both horizontally and vertically, simply set `extends_horizontal` true or false accordingly.
-
--   `channel`
-    For each channel labelframe the width and height may be adjusted which effects the spacing between widgets and the length of the scales and progressbars respectively.
-
--   `mwscroll_step`
-    Sets the amount (in db) the gain slider moves with a single mousewheel step. Default 3.
-
--   `submixes`
-    Select the default submix bus when Submix frame is shown. For example, a dedicated bus for OBS.
-
-### vban.toml
-
-Configure as many vban connections as you wish. This allows the app to work over a LAN connection as well as with a local Voicemeeter installation.
-
-For vban connections to work correctly VBAN TEXT incoming stream MUST be configured correctly on the remote machine. Both pcs ought to be connected to a local private network and should be able to ping one another.
-
-A valid `vban.toml` might look like this:
-
-```toml
-[connection-1]
-kind = 'banana'
-ip = '192.168.1.2'
-streamname = 'worklaptop'
-port = 6980
-
-[connection-2]
-kind = 'potato'
-ip = '192.168.1.3'
-streamname = 'streampc'
-port = 6990
-```
-
-### basic/ banana/ potato/
-
-Three example user configs are included with the package, one for each kind of Voicemeeter. Use these to configure parameter startup states. Any parameter supported by the underlying interfaces may be used. Check the 'multiple-parameters' section for more info:
-
-[Python Interface for Voicemeeter API](https://github.com/onyx-and-iris/voicemeeter-api-python#multiple-parameters)
-
-[Python Interface for VBAN CMD](https://github.com/onyx-and-iris/vban-cmd-python#multiple-parameters)
-
-User configs may be loaded at any time via the menu.
-
-## Special Thanks
-
-[Vincent Burel](https://github.com/vburel2018) for creating Voicemeeter, its SDK, the C Remote API, the RT Packet service and Streamer View app!
-
-[Rdbende](https://github.com/rdbende) for creating the beautiful Sun Valley Tkinter theme and adding it to Pypi!
+[![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![OS: Windows](https://img.shields.io/badge/os-windows-red)
+
+![Image of app/potato size comparison](./doc_imgs/potatocomparisonsmaller.png)
+
+# Voicemeeter Compact
+
+A compact Voicemeeter remote app, works locally and over LAN.
+
+For an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)
+
+## Prerequisites
+
+-   [Voicemeeter](https://voicemeeter.com/) (Basic v1.0.8.4), (Banana v2.0.6.4) or (Potato v3.0.2.4)
+-   Python 3.10 or greater
+
+## Installation
+
+For a step-by-step guide [click here](INSTALLATION.md)
+
+```
+pip install voicemeeter-compact
+```
+
+## Usage
+
+Example `__main__.py` file:
+
+```python
+import voicemeeterlib
+import vmcompact
+
+
+def main():
+    # pass the kind_id and the vm object to the app
+    with voicemeeterlib.api(kind_id) as vm:
+        app = vmcompact.connect(kind_id, vm)
+        app.mainloop()
+
+
+if __name__ == "__main__":
+    # choose the kind of Voicemeeter (Local connection)
+    kind_id = "banana"
+
+    main()
+```
+
+It's important to know that only labelled strips and buses will appear in the Channel frames. Removing a Channels label will cause the GUI to grow/shrink in real time.
+
+![Image of unlabelled app](./doc_imgs/nolabels.png)
+
+If the GUI looks like the above when you first load it, then no channels are labelled. From the menu, `Configs->Load config` you may load an example config. Save your current Voicemeeter settings first :).
+
+### kind_id
+
+Set the kind of Voicemeeter, kind_id may be:
+
+-   `basic`
+-   `banana`
+-   `potato`
+
+## TOML Files
+
+This is how your files should be organised. Wherever your `__main__.py` file is located (after install this can be any location), `configs` should be in the same location.
+Directly inside of configs directory you may place an app.toml, vban.toml and a directory for each kind.
+Inside each kind directory you may place as many custom toml configurations as you wish.
+
+.
+
+├── `__main__.py`
+
+├── configs
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── app.toml
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── vban.toml
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── basic
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other_config.toml
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── streaming_config.toml
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── banana
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other.toml
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── potato
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml
+
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...
+
+## Configs
+
+### app.toml
+
+Configure certain startup states for the app.
+
+-   `configs`
+    Configure a user config to load on app startup. Don't include the .toml extension in the config name.
+
+-   `theme`
+    By default the app loads up the [Sun Valley light or dark theme](https://github.com/rdbende/Sun-Valley-ttk-theme) by @rdbende. You have the option to load up the app without any theme loaded. Simply set `enabled` to false and `mode` will take no effect.
+
+-   `extends`
+    Extending the app will show both strips and buses. In reduced mode only one or the other. This app will extend both horizontally and vertically, simply set `extends_horizontal` true or false accordingly.
+
+-   `channel`
+    For each channel labelframe the width and height may be adjusted which effects the spacing between widgets and the length of the scales and progressbars respectively.
+
+-   `mwscroll_step`
+    Sets the amount (in db) the gain slider moves with a single mousewheel step. Default 3.
+
+-   `submixes`
+    Select the default submix bus when Submix frame is shown. For example, a dedicated bus for OBS.
+
+### vban.toml
+
+Configure as many vban connections as you wish. This allows the app to work over a LAN connection as well as with a local Voicemeeter installation.
+
+For vban connections to work correctly VBAN TEXT incoming stream MUST be configured correctly on the remote machine. Both pcs ought to be connected to a local private network and should be able to ping one another.
+
+A valid `vban.toml` might look like this:
+
+```toml
+[connection-1]
+kind = 'banana'
+ip = '192.168.1.2'
+streamname = 'worklaptop'
+port = 6980
+
+[connection-2]
+kind = 'potato'
+ip = '192.168.1.3'
+streamname = 'streampc'
+port = 6990
+```
+
+### basic/ banana/ potato/
+
+Three example user configs are included with the package, one for each kind of Voicemeeter. Use these to configure parameter startup states. Any parameter supported by the underlying interfaces may be used. Check the 'multiple-parameters' section for more info:
+
+[Python Interface for Voicemeeter API](https://github.com/onyx-and-iris/voicemeeter-api-python#multiple-parameters)
+
+[Python Interface for VBAN CMD](https://github.com/onyx-and-iris/vban-cmd-python#multiple-parameters)
+
+User configs may be loaded at any time via the menu.
+
+## Special Thanks
+
+[Vincent Burel](https://github.com/vburel2018) for creating Voicemeeter, its SDK, the C Remote API, the RT Packet service and Streamer View app!
+
+[Rdbende](https://github.com/rdbende) for creating the beautiful Sun Valley Tkinter theme and adding it to Pypi!
```

### Comparing `voicemeeter-compact-1.8.1/vmcompact/app.py` & `voicemeeter_compact-1.8.2/vmcompact/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         """
         Clear observables.
 
         Deregister app as observer.
 
         Destroy all top level frames.
         """
-        self.target.subject.remove(self)
+        self.target.subject.remove([self.on_pdirty, self.on_ldirty])
         self.subject.clear()
         [
             frame.destroy()
             for frame in self.winfo_children()
             if isinstance(frame, ttk.Frame)
         ]
```

### Comparing `voicemeeter-compact-1.8.1/vmcompact/banner.py` & `voicemeeter_compact-1.8.2/vmcompact/banner.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/builders.py` & `voicemeeter_compact-1.8.2/vmcompact/builders.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/channels.py` & `voicemeeter_compact-1.8.2/vmcompact/channels.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/config.py` & `voicemeeter_compact-1.8.2/vmcompact/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/configurations.py` & `voicemeeter_compact-1.8.2/vmcompact/configurations.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/data.py` & `voicemeeter_compact-1.8.2/vmcompact/data.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/gainlayer.py` & `voicemeeter_compact-1.8.2/vmcompact/gainlayer.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/img/cat.ico` & `voicemeeter_compact-1.8.2/vmcompact/img/cat.ico`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/menu.py` & `voicemeeter_compact-1.8.2/vmcompact/menu.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/navigation.py` & `voicemeeter_compact-1.8.2/vmcompact/navigation.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/vmcompact/subject.py` & `voicemeeter_compact-1.8.2/vmcompact/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.8.1/setup.py` & `voicemeeter_compact-1.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
  'voicemeeter-api>=2.0.2,<3.0.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'voicemeeter-compact',
-    'version': '1.8.1',
+    'version': '1.8.2',
     'description': 'A Compact Voicemeeter Remote App',
     'long_description': '[![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![OS: Windows](https://img.shields.io/badge/os-windows-red)\n\n![Image of app/potato size comparison](./doc_imgs/potatocomparisonsmaller.png)\n\n# Voicemeeter Compact\n\nA compact Voicemeeter remote app, works locally and over LAN.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Prerequisites\n\n-   [Voicemeeter](https://voicemeeter.com/) (Basic v1.0.8.4), (Banana v2.0.6.4) or (Potato v3.0.2.4)\n-   Python 3.10 or greater\n\n## Installation\n\nFor a step-by-step guide [click here](INSTALLATION.md)\n\n```\npip install voicemeeter-compact\n```\n\n## Usage\n\nExample `__main__.py` file:\n\n```python\nimport voicemeeterlib\nimport vmcompact\n\n\ndef main():\n    # pass the kind_id and the vm object to the app\n    with voicemeeterlib.api(kind_id) as vm:\n        app = vmcompact.connect(kind_id, vm)\n        app.mainloop()\n\n\nif __name__ == "__main__":\n    # choose the kind of Voicemeeter (Local connection)\n    kind_id = "banana"\n\n    main()\n```\n\nIt\'s important to know that only labelled strips and buses will appear in the Channel frames. Removing a Channels label will cause the GUI to grow/shrink in real time.\n\n![Image of unlabelled app](./doc_imgs/nolabels.png)\n\nIf the GUI looks like the above when you first load it, then no channels are labelled. From the menu, `Configs->Load config` you may load an example config. Save your current Voicemeeter settings first :).\n\n### kind_id\n\nSet the kind of Voicemeeter, kind_id may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## TOML Files\n\nThis is how your files should be organised. Wherever your `__main__.py` file is located (after install this can be any location), `configs` should be in the same location.\nDirectly inside of configs directory you may place an app.toml, vban.toml and a directory for each kind.\nInside each kind directory you may place as many custom toml configurations as you wish.\n\n.\n\n├── `__main__.py`\n\n├── configs\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── app.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── vban.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── basic\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── streaming_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── banana\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── potato\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n## Configs\n\n### app.toml\n\nConfigure certain startup states for the app.\n\n-   `configs`\n    Configure a user config to load on app startup. Don\'t include the .toml extension in the config name.\n\n-   `theme`\n    By default the app loads up the [Sun Valley light or dark theme](https://github.com/rdbende/Sun-Valley-ttk-theme) by @rdbende. You have the option to load up the app without any theme loaded. Simply set `enabled` to false and `mode` will take no effect.\n\n-   `extends`\n    Extending the app will show both strips and buses. In reduced mode only one or the other. This app will extend both horizontally and vertically, simply set `extends_horizontal` true or false accordingly.\n\n-   `channel`\n    For each channel labelframe the width and height may be adjusted which effects the spacing between widgets and the length of the scales and progressbars respectively.\n\n-   `mwscroll_step`\n    Sets the amount (in db) the gain slider moves with a single mousewheel step. Default 3.\n\n-   `submixes`\n    Select the default submix bus when Submix frame is shown. For example, a dedicated bus for OBS.\n\n### vban.toml\n\nConfigure as many vban connections as you wish. This allows the app to work over a LAN connection as well as with a local Voicemeeter installation.\n\nFor vban connections to work correctly VBAN TEXT incoming stream MUST be configured correctly on the remote machine. Both pcs ought to be connected to a local private network and should be able to ping one another.\n\nA valid `vban.toml` might look like this:\n\n```toml\n[connection-1]\nkind = \'banana\'\nip = \'192.168.1.2\'\nstreamname = \'worklaptop\'\nport = 6980\n\n[connection-2]\nkind = \'potato\'\nip = \'192.168.1.3\'\nstreamname = \'streampc\'\nport = 6990\n```\n\n### basic/ banana/ potato/\n\nThree example user configs are included with the package, one for each kind of Voicemeeter. Use these to configure parameter startup states. Any parameter supported by the underlying interfaces may be used. Check the \'multiple-parameters\' section for more info:\n\n[Python Interface for Voicemeeter API](https://github.com/onyx-and-iris/voicemeeter-api-python#multiple-parameters)\n\n[Python Interface for VBAN CMD](https://github.com/onyx-and-iris/vban-cmd-python#multiple-parameters)\n\nUser configs may be loaded at any time via the menu.\n\n## Special Thanks\n\n[Vincent Burel](https://github.com/vburel2018) for creating Voicemeeter, its SDK, the C Remote API, the RT Packet service and Streamer View app!\n\n[Rdbende](https://github.com/rdbende) for creating the beautiful Sun Valley Tkinter theme and adding it to Pypi!\n',
     'author': 'onyx-and-iris',
     'author_email': 'code@onyxandiris.online',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/onyx-and-iris/voicemeeter-compact',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `voicemeeter-compact-1.8.1/PKG-INFO` & `voicemeeter_compact-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: voicemeeter-compact
-Version: 1.8.1
+Version: 1.8.2
 Summary: A Compact Voicemeeter Remote App
 Home-page: https://github.com/onyx-and-iris/voicemeeter-compact
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sv-ttk (>=2.5.1,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11"
 Requires-Dist: vban-cmd (>=2.0.0,<3.0.0)
 Requires-Dist: voicemeeter-api (>=2.0.2,<3.0.0)
 Project-URL: Repository, https://github.com/onyx-and-iris/voicemeeter-compact
 Description-Content-Type: text/markdown
```

