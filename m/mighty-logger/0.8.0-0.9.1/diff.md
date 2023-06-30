# Comparing `tmp/mighty_logger-0.8.0.tar.gz` & `tmp/mighty_logger-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mighty_logger-0.8.0.tar", last modified: Thu Jun 29 13:38:37 2023, max compression
+gzip compressed data, was "mighty_logger-0.9.1.tar", last modified: Fri Jun 30 17:55:52 2023, max compression
```

## Comparing `mighty_logger-0.8.0.tar` & `mighty_logger-0.9.1.tar`

### file list

```diff
@@ -1,43 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.645940 mighty_logger-0.8.0/
--rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.8.0/LICENSE
--rw-rw-rw-   0        0        0    10856 2023-06-29 13:38:37.645940 mighty_logger-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     9913 2023-06-29 12:46:55.000000 mighty_logger-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.535905 mighty_logger-0.8.0/mighty_logger/
--rw-rw-rw-   0        0        0      861 2023-06-29 12:46:55.000000 mighty_logger-0.8.0/mighty_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.572906 mighty_logger-0.8.0/mighty_logger/basic/
--rw-rw-rw-   0        0        0      783 2023-06-29 12:11:16.000000 mighty_logger-0.8.0/mighty_logger/basic/__init__.py
--rw-rw-rw-   0        0        0     8311 2023-06-29 12:34:25.000000 mighty_logger-0.8.0/mighty_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1712 2023-06-29 12:11:16.000000 mighty_logger-0.8.0/mighty_logger/basic/exceptions.py
--rw-rw-rw-   0        0        0     2606 2023-06-29 12:34:25.000000 mighty_logger-0.8.0/mighty_logger/basic/exporter.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.620938 mighty_logger-0.8.0/mighty_logger/basic/lib_types/
--rw-rw-rw-   0        0        0      869 2023-06-28 14:21:52.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/__init__.py
--rw-rw-rw-   0        0        0     1086 2023-06-25 13:07:43.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/animation_type.py
--rw-rw-rw-   0        0        0     2030 2023-06-28 10:45:25.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/entry_type.py
--rw-rw-rw-   0        0        0     1297 2023-06-26 11:32:43.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/environment_type.py
--rw-rw-rw-   0        0        0      798 2023-06-27 12:43:22.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/sorting_key_type.py
--rw-rw-rw-   0        0        0     4317 2023-06-26 11:33:46.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/text_buffer_type.py
--rw-rw-rw-   0        0        0     7061 2023-06-29 12:34:25.000000 mighty_logger-0.8.0/mighty_logger/basic/modifier.py
--rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.8.0/mighty_logger/basic/singleton.py
--rw-rw-rw-   0        0        0    10554 2023-06-29 12:34:25.000000 mighty_logger-0.8.0/mighty_logger/basic/text_buffer.py
--rw-rw-rw-   0        0        0    25499 2023-06-29 09:55:09.000000 mighty_logger-0.8.0/mighty_logger/mighty_logger.py
--rw-rw-rw-   0        0        0     5953 2023-06-29 12:15:54.000000 mighty_logger-0.8.0/mighty_logger/simple_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.631752 mighty_logger-0.8.0/mighty_logger/src/
--rw-rw-rw-   0        0        0      903 2023-06-29 08:51:20.000000 mighty_logger-0.8.0/mighty_logger/src/__init__.py
--rw-rw-rw-   0        0        0     9975 2023-06-25 13:20:13.000000 mighty_logger-0.8.0/mighty_logger/src/animations.py
--rw-rw-rw-   0        0        0     4572 2023-06-11 16:58:31.000000 mighty_logger-0.8.0/mighty_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     8659 2023-06-11 16:58:31.000000 mighty_logger-0.8.0/mighty_logger/src/color_picker.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.642941 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/
--rw-rw-rw-   0        0        0      779 2023-06-28 14:22:30.000000 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/__init__.py
--rw-rw-rw-   0        0        0    40877 2023-06-28 11:04:00.000000 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/entry_types.py
--rw-rw-rw-   0        0        0     1140 2023-06-25 13:20:13.000000 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/environments.py
--rw-rw-rw-   0        0        0      873 2023-06-27 12:43:22.000000 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/sorting_keys.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.544905 mighty_logger-0.8.0/mighty_logger.egg-info/
--rw-rw-rw-   0        0        0    10856 2023-06-29 13:38:37.000000 mighty_logger-0.8.0/mighty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-06-29 13:38:37.000000 mighty_logger-0.8.0/mighty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:38:37.000000 mighty_logger-0.8.0/mighty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-29 13:38:37.000000 mighty_logger-0.8.0/mighty_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 13:38:37.646940 mighty_logger-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1757 2023-06-29 12:46:55.000000 mighty_logger-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.644940 mighty_logger-0.8.0/test/
--rw-rw-rw-   0        0        0     3078 2023-06-29 09:02:18.000000 mighty_logger-0.8.0/test/test.py
--rw-rw-rw-   0        0        0      924 2023-06-28 09:53:14.000000 mighty_logger-0.8.0/test/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.539240 mighty_logger-0.9.1/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0    10873 2023-06-30 17:55:52.541240 mighty_logger-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9941 2023-06-30 17:52:14.000000 mighty_logger-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.121204 mighty_logger-0.9.1/mighty_logger/
+-rw-rw-rw-   0        0        0      886 2023-06-30 15:04:11.000000 mighty_logger-0.9.1/mighty_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.360227 mighty_logger-0.9.1/mighty_logger/basic/
+-rw-rw-rw-   0        0        0      808 2023-06-30 12:57:57.000000 mighty_logger-0.9.1/mighty_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     8869 2023-06-30 13:13:14.000000 mighty_logger-0.9.1/mighty_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1842 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0     3379 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.469236 mighty_logger-0.9.1/mighty_logger/basic/lib_types/
+-rw-rw-rw-   0        0        0      961 2023-06-30 12:33:00.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/__init__.py
+-rw-rw-rw-   0        0        0     1163 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/animation_type.py
+-rw-rw-rw-   0        0        0     2079 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/entry_type.py
+-rw-rw-rw-   0        0        0     1415 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/environment_type.py
+-rw-rw-rw-   0        0        0      891 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/sorting_key_type.py
+-rw-rw-rw-   0        0        0     6706 2023-06-30 13:06:13.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/text_buffer_type.py
+-rw-rw-rw-   0        0        0     8207 2023-06-30 13:47:39.000000 mighty_logger-0.9.1/mighty_logger/basic/modifier.py
+-rw-rw-rw-   0        0        0      842 2023-06-30 13:13:13.000000 mighty_logger-0.9.1/mighty_logger/basic/singleton.py
+-rw-rw-rw-   0        0        0    10557 2023-06-30 13:13:13.000000 mighty_logger-0.9.1/mighty_logger/basic/text_buffer.py
+-rw-rw-rw-   0        0        0    32357 2023-06-30 17:34:17.000000 mighty_logger-0.9.1/mighty_logger/mighty_logger.py
+-rw-rw-rw-   0        0        0     6868 2023-06-30 17:43:48.000000 mighty_logger-0.9.1/mighty_logger/simple_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.512238 mighty_logger-0.9.1/mighty_logger/src/
+-rw-rw-rw-   0        0        0      928 2023-06-30 14:44:07.000000 mighty_logger-0.9.1/mighty_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     9983 2023-06-30 14:44:07.000000 mighty_logger-0.9.1/mighty_logger/src/animations.py
+-rw-rw-rw-   0        0        0     4664 2023-06-30 14:44:07.000000 mighty_logger-0.9.1/mighty_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     9688 2023-06-30 14:46:54.000000 mighty_logger-0.9.1/mighty_logger/src/color_picker.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.529240 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/
+-rw-rw-rw-   0        0        0      865 2023-06-30 14:14:17.000000 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/__init__.py
+-rw-rw-rw-   0        0        0    47441 2023-06-30 14:22:00.000000 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/entry_types.py
+-rw-rw-rw-   0        0        0     1030 2023-06-30 14:14:17.000000 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/environments.py
+-rw-rw-rw-   0        0        0      975 2023-06-30 14:14:17.000000 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/sorting_keys.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.137204 mighty_logger-0.9.1/mighty_logger.egg-info/
+-rw-rw-rw-   0        0        0    10873 2023-06-30 17:55:52.000000 mighty_logger-0.9.1/mighty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2023-06-30 17:55:52.000000 mighty_logger-0.9.1/mighty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 17:55:52.000000 mighty_logger-0.9.1/mighty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 17:55:52.000000 mighty_logger-0.9.1/mighty_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1869 2023-06-29 15:07:42.000000 mighty_logger-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 17:55:52.543240 mighty_logger-0.9.1/setup.cfg
```

### Comparing `mighty_logger-0.8.0/LICENSE` & `mighty_logger-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.8.0/PKG-INFO` & `mighty_logger-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mighty_logger
-Version: 0.8.0
+Version: 0.9.1
 Summary: Powerful functional logger
-Home-page: https://github.com/Nakama3942/mighty_logger
-Author: Kalynovsky 'Nakamura Akira' Valentin
-Author-email: nakama3942@gmail.com
-License: Apache License, Version 2.0, see LICENSE file
+Author-email: Kalynovsky 'Nakamura Akira' Valentin <nakama3942@gmail.com>
+License: Apache License Version 2.0
+Project-URL: Repository, https://github.com/Nakama3942/mighty_logger
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -107,16 +106,18 @@
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [x] v0.6.1 - Animation update (added animations in processes)
 - [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
-- [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
-- [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
+- [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
+- [x] v0.9.1 - Documenting update (documented library)
+- [ ] v0.9.2 - Feature update (made optimizations)
+- [ ] v0.9.3 - Web docs update (added generation of web docs)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
```

### Comparing `mighty_logger-0.8.0/README.md` & `mighty_logger-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,18 @@
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [x] v0.6.1 - Animation update (added animations in processes)
 - [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
-- [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
-- [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
+- [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
+- [x] v0.9.1 - Documenting update (documented library)
+- [ ] v0.9.2 - Feature update (made optimizations)
+- [ ] v0.9.3 - Web docs update (added generation of web docs)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
```

### Comparing `mighty_logger-0.8.0/mighty_logger/__init__.py` & `mighty_logger-0.9.1/mighty_logger/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
 A root package that provides access to a implementation of the powerful logger.
+
+.. versionadded:: 0.0.0
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -16,9 +18,9 @@
 limitations under the License.
 """
 
 from .mighty_logger import MightyLogger
 from .simple_logger import Logger
 
 __authot__ = "Kalynovsky 'Nakamura Akira' Valentin"
-__version__ = "0.8.0"
+__version__ = "0.9.1"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/__init__.py` & `mighty_logger-0.9.1/mighty_logger/basic/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
 A package with base classes intended for use within a library.
+
+.. versionadded:: 0.0.0
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/basic_logger.py` & `mighty_logger-0.9.1/mighty_logger/basic/basic_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-A module with an implementation of the base (parent) logger class.
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -25,14 +23,21 @@
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 from mighty_logger.basic.exceptions import MessageException
 from mighty_logger.basic.singleton import Singleton
 from mighty_logger.src.lib_types_collection.environments import LogEnvironments
 from mighty_logger.src.ansi_format import GetAnsiFormat
 
 class BasicLogger(Singleton):
+	"""
+	The base class of the Logger, which stores the main attributes and implements
+	the most important functionality - the formation of the Logger entry string.
+
+	.. versionadded:: 0.0.0
+	"""
+
 	def __init__(
 		self,
 		program_name: str,
 		env: EnvironmentType
 	) -> None:
 		self._ID: int = randint(1000000, 9999999)
 		self._program_name: str = program_name
@@ -42,18 +47,23 @@
 	def _initialized_data(
 		self,
 		colors: list[str, str],
 	) -> str:
 		"""
 		A method that assemble an entry of system initialized data.
 
+		.. versionadded:: 0.0.0
+
 		:param colors: Color string list of initialized data
-		:return: a string with initialized data
+		:type colors: list[str, str]
+		:return: A string with initialized data
+		:rtype: str
 		"""
 		match self._environment.environment_name:
+			# todo оптимизировать
 			case LogEnvironments.CONSOLE.environment_name:
 				return (
 					f"{colors[1]}" +
 					f"{colors[0]}-{self._program_name}?entry> " +
 					f"${platform.node()}:{getlogin()}" +
 					f":{platform.system()}" +
 					f":{platform.version()}" +
@@ -111,31 +121,41 @@
 		message_text: str,
 		entry_background: bool,
 		local_settings: dict
 	) -> str:
 		"""
 		A method that assemble an entry into a string and returns it.
 
-		:param colors: 6 colors that the method uses to assemble the string
-		:param animation: Animation of entry
-		:param icon: Type icon
-		:param status_message_text: Status message
-		:param message_type: Entry type
-		:param message_text: Entry message
+		.. versionadded:: 0.0.0
+
+		:param entry_type: Type of entry to be generated
+		:type entry_type: EntryType
+		:param icon_set: Icon set number
+		:type icon_set: int
+		:param animation: Animation frame of entry
+		:type animation: str
+		:param message_text: Message of entry
+		:type message_text: str
+		:param entry_background: Flag indicating setting the background of the entry string
+		:type entry_background: bool
 		:param local_settings: Settings for the string of the current entry
-		:return: the formed entry string
+		:type local_settings: dict
+		:return: The formed entry string
+		:rtype: str
+		:raises MessageException: Message is too short (less than 10 characters)
 		"""
 		if len(message_text) < 10:
 			raise MessageException("Message is too short (less than 10 characters)")
 
 		bold = local_settings['bold'] if 'bold' in local_settings else self._settings['global_bold_font']
 		italic = local_settings['italic'] if 'italic' in local_settings else self._settings['global_italic_font']
 		invert = local_settings['invert'] if 'invert' in local_settings else self._settings['global_invert_font']
 
 		match self._environment.environment_name:
+			# todo оптимизировать
 			case LogEnvironments.CONSOLE.environment_name:
 				return (
 					(f"{GetAnsiFormat('bold/on')}" if bold else "") +
 					(f"{GetAnsiFormat('italic/on')}" if italic else "") +
 					(f"{GetAnsiFormat('invert/on')}" if invert else "") +
 					f"{entry_type.background_color[self._environment.environment_code][entry_background]}" +
 					f"{entry_type.message_color[self._environment.environment_code][entry_background]}-?entry> {animation} " +
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/exceptions.py` & `mighty_logger-0.9.1/mighty_logger/basic/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-A module with a collection of exceptions.
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,56 +10,73 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+# todo разбить в пакет
+
 class ColorException(BaseException):
 	"""
 	The exception that is thrown when there is no color in any palette.
+
+	.. versionadded:: 0.0.0
 	"""
+
 	def __init__(self, message):
 		self.message = message
 
 	def __str__(self):
 		return self.message
 
 class ReCreationException(BaseException):
 	"""
-	The exception that is thrown when an object of the Singleton class is re-created.
+	The exception that is thrown when an object of the Singleton category is re-created.
+
+	.. versionadded:: 0.0.0
 	"""
+
 	def __init__(self, message):
 		self.message = message
 
 	def __str__(self):
 		return self.message
 
 class EnvironmentException(BaseException):
 	"""
 	The exception that is thrown when on environmental errors.
+
+	.. versionadded:: 0.0.0
 	"""
+
 	def __init__(self, message):
 		self.message = message
 
 	def __str__(self):
 		return self.message
 
 class InitException(BaseException):
 	"""
 	The exception thrown on errors during initialization.
+
+	.. versionadded:: 0.0.0
 	"""
+
 	def __init__(self, message):
 		self.message = message
 
 	def __str__(self):
 		return self.message
 
 class MessageException(BaseException):
 	"""
 	The exception that is thrown when a write message is too short.
+
+	.. versionadded:: 0.0.0
 	"""
+
 	def __init__(self, message):
 		self.message = message
 
 	def __str__(self):
 		return self.message
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/lib_types/__init__.py` & `mighty_logger-0.9.1/mighty_logger/basic/lib_types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-...
+A package that contains the data types that are used in the library.
+
+.. versionadded:: 0.0.0
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/lib_types/animation_type.py` & `mighty_logger-0.9.1/mighty_logger/basic/lib_types/animation_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-...
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,26 +13,33 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class BasicAnimationType:
 	"""
 	Basic wrapper class for animations type.
+
+	.. versionadded:: 0.0.0
 	"""
+
 	def __init__(self, animation: list):
 		self.__animation: list = animation
 
 	@property
 	def animation(self) -> list:
 		return self.__animation
 
 class IndefiniteAnimationType(BasicAnimationType):
 	"""
 	Wrapper class for indefinite animations type.
+
+	.. versionadded:: 0.0.0
 	"""
 	...
 
 class DefiniteAnimationType(BasicAnimationType):
 	"""
 	Wrapper class for definite animations type.
+
+	.. versionadded:: 0.0.0
 	"""
 	...
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/lib_types/entry_type.py` & `mighty_logger-0.9.1/mighty_logger/basic/lib_types/entry_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-...
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,26 +11,32 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class EntryType:
+	"""
+	The data type that characterizes the entry type.
+
+	.. versionadded:: 0.0.0
+	"""
+
 	def __init__(
 		self,
 		*,
 		type_category: str,
 		type_name: str,
-		time_color: tuple = (),
-		status_color: tuple = (),
-		status_message_color: tuple = (),
-		type_color: tuple = (),
-		message_color: tuple = (),
-		background_color: tuple = (),
-		icon: tuple = ()
+		time_color: tuple,
+		status_color: tuple,
+		status_message_color: tuple,
+		type_color: tuple,
+		message_color: tuple,
+		background_color: tuple,
+		icon: tuple
 	) -> None:
 		self.__type_category: str = type_category
 		self.__type_name: str = type_name
 		self.__time_color: tuple = time_color
 		self.__status_color: tuple = status_color
 		self.__status_message_color: tuple = status_message_color
 		self.__type_color: tuple = type_color
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/lib_types/environment_type.py` & `mighty_logger-0.9.1/mighty_logger/basic/lib_types/environment_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-...
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,14 +11,20 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class EnvironmentType:
+	"""
+	A data type that characterizes the environments in which the Logger can operate.
+
+	.. versionadded:: 0.0.0
+	"""
+
 	def __init__(
 		self,
 		environment_name: str,
 		environment_code: int,
 		updatable: bool,
 		weak_environment: bool
 	) -> None:
@@ -34,13 +38,13 @@
 		return self.__environment_name
 
 	@property
 	def environment_code(self) -> int:
 		return self.__environment_code
 
 	@property
-	def updatable(self) -> int:
+	def updatable(self) -> bool:
 		return self.__updatable
 
 	@property
-	def weak_environment(self) -> int:
+	def weak_environment(self) -> bool:
 		return self.__weak_environment
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/lib_types/sorting_key_type.py` & `mighty_logger-0.9.1/mighty_logger/basic/lib_types/sorting_key_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-...
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,13 +11,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class SortingKeyType:
+	"""
+	A data type that characterizes the sort keys for entries.
+
+	.. versionadded:: 0.0.0
+	"""
+
 	def __init__(self, sorting_key: int):
 		self.__sorting_key: int = sorting_key
 
 	@property
 	def sorting_key(self) -> int:
 		return self.__sorting_key
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/singleton.py` & `mighty_logger-0.9.1/mighty_logger/basic/singleton.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-This module is a collection of Patterns. Available: Singleton.
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,13 +11,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class Singleton:
+	"""
+	A class that implements the Singleton pattern.
+
+	.. versionadded:: 0.0.0
+	"""
+
 	_instance = None
 
 	def __new__(cls, *args, **kwargs):
 		if cls._instance is None:
 			cls._instance = super().__new__(cls)
 		return cls._instance
```

### Comparing `mighty_logger-0.8.0/mighty_logger/basic/text_buffer.py` & `mighty_logger-0.9.1/mighty_logger/basic/text_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-A module with implementation of text buffers.
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -23,16 +21,18 @@
 from mighty_logger.basic.lib_types.text_buffer_type import TextBufferType
 from mighty_logger.basic.exceptions import ReCreationException, EnvironmentException
 from mighty_logger.basic.singleton import Singleton
 from mighty_logger.src.lib_types_collection.environments import LogEnvironments
 
 class BasicTextBuffer(Singleton, TextBufferType):
 	"""
-	A class with a basic implementation of a simple text buffer. It is intended
+	A class with a basic implementation of a simple Text Buffer. It is intended
 	to be used in conjunction with HTML, but this is optional.
+
+	.. versionadded:: 0.0.0
 	"""
 
 	def __init__(self, env: EnvironmentType) -> None:
 		if not hasattr(self, "_text_buffer"):
 			super().__init__(env)
 		else:
 			raise ReCreationException("BasicTextBuffer class object already created")
@@ -123,18 +123,20 @@
 		super().update_console()
 
 	def update_entry(self) -> None:
 		super().update_console()
 
 class TextBuffer(Singleton, TextBufferType):
 	"""
-	A class with an advanced implementation of the console text buffer. It is not necessary to use it
+	A class with an advanced implementation of the console Text Buffer. It is not necessary to use it
 	only in the console, but almost all methods are reimplemented for more complex algorithms, taking
 	into account the width of the console (number of characters per line) and use ANSI escape codes
 	that are only found in the console.
+
+	.. versionadded:: 0.0.0
 	"""
 
 	def __init__(self, env: EnvironmentType, console_width: int = 60) -> None:
 		if not hasattr(self, "_text_buffer"):
 			super().__init__(env)
 			self._cursor_string: int = 0
 			self._buffer_size: int = 0
```

### Comparing `mighty_logger-0.8.0/mighty_logger/simple_logger.py` & `mighty_logger-0.9.1/mighty_logger/simple_logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-...
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -19,23 +17,25 @@
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 from mighty_logger.src.lib_types_collection.entry_types import LoggerEntryTypes, ServiceProcessEntryTypes
 from mighty_logger.src.lib_types_collection.environments import LogEnvironments
 from mighty_logger.mighty_logger import MightyLogger
 
 class Logger:
 	"""
-	...
+	Lightweight Logger automates work with entry types.
+
+	.. versionadded:: 0.0.0
 	"""
 
 	def __init__(
 		self,
 		program_name: str = "Unknown",
 		environment: EnvironmentType = LogEnvironments.PLAIN,
 		console_width: int = 60
-	):
+	) -> None:
 		if MightyLogger._instance is not None:
 			self.__logger = MightyLogger._instance
 			self.notice("An existing logger was taken into use")
 		else:
 			self.__logger = MightyLogger(
 				program_name=program_name,
 				log_environment=environment,
@@ -46,141 +46,186 @@
 		return self.__logger
 
 	def debug(self, message_text: str) -> None:
 		"""
 		Debugging information logging:
 		Can be used to log entry any information while debugging an application.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.debug, message_text)
 
 	def debug_performance(self, message_text: str) -> None:
 		"""
 		Performance debugging information logging:
 		Can be used to log entry the execution time of operations or other
 		performance information while the application is being debugged.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.debug_performance, message_text)
 
 	def performance(self, message_text: str) -> None:
 		"""
 		Performance information logging:
 		Can be used to log entry the execution time of operations or
 		other application performance information.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.performance, message_text)
 
 	def event(self, message_text: str) -> None:
 		"""
 		Event information logging:
 		Can be used to log entry specific events in the application,
 		such as button presses or mouse cursor movements.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.event, message_text)
 
 	def audit(self, message_text: str) -> None:
 		"""
 		Audit information logging:
 		Can be used to log entry changes in the system, such as creating or
 		deleting users, as well as changes in security settings.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.audit, message_text)
 
 	def metrics(self, message_text: str) -> None:
 		"""
 		Metrics information logging:
 		Can be used to log entry metrics to track application performance and identify issues.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.metrics, message_text)
 
 	def user(self, message_text: str) -> None:
 		"""
 		User information logging:
 		Can be used to log entry custom logs to store additional information
 		that may be useful for diagnosing problems.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.user, message_text)
 
 	def message(self, message_text: str) -> None:
 		"""
 		Message information logging:
 		Can be used for the usual output of ordinary messages about the program's operation.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.message, message_text)
 
 	def info(self, message_text: str) -> None:
 		"""
 		Default information logging:
 		Can be used to log entry messages with specific content about the operation of the program.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.info, message_text)
 
 	def notice(self, message_text: str) -> None:
 		"""
 		Notice information logging:
 		Can be used to flag important events that might be missed with a normal logging level.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.notice, message_text)
 
 	def warning(self, message_text: str) -> None:
 		"""
 		Warning information logging:
 		Can be used to log entry warnings that the program may work with unpredictable results.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.warning, message_text)
 
 	def error(self, message_text: str) -> None:
 		"""
 		Error information logging:
 		Used to log entry errors and crashes in the program.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.error, message_text)
 
 	def critical(self, message_text: str) -> None:
 		"""
 		Critical error information logging:
 		Used to log entry for critical and unpredictable program failures.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.critical, message_text)
 
 	def success(self, message_text: str) -> None:
 		"""
 		Success information logging:
 		Used to log entry a message about the success of the process.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(ServiceProcessEntryTypes.success, message_text)
 
 	def fail(self, message_text: str) -> None:
 		"""
 		Fail information logging:
 		Used to log entry a message about the failed execution of the process.
 
+		.. versionadded:: 0.0.0
+
 		:param message_text: Log entry message
+		:type message_text: str
 		"""
 		self.__logger.entry(ServiceProcessEntryTypes.fail, message_text)
```

### Comparing `mighty_logger-0.8.0/mighty_logger/src/__init__.py` & `mighty_logger-0.9.1/mighty_logger/src/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
 A package with the implementation of various data (ANSI, colors, etc.).
+
+.. versionadded:: 0.0.0
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `mighty_logger-0.8.0/mighty_logger/src/animations.py` & `mighty_logger-0.9.1/mighty_logger/src/animations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-A module with realisation of animations.
-\n
 The source of IndefiniteAnimation:
 https://github.com/kopensource/colored_logs/blob/develop/colored_logs/models/animation_type.py
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
@@ -20,14 +18,16 @@
 """
 
 from mighty_logger.basic.lib_types.animation_type import IndefiniteAnimationType, DefiniteAnimationType
 
 class IndefiniteAnimations:
 	"""
 	The class with sets indefinite animations.
+
+	.. versionadded:: 0.0.0
 	"""
 	Dots = IndefiniteAnimationType([
 		'.       ',
 		'..      ',
 		'...     ',
 		'....    ',
 		'.....   ',
@@ -434,14 +434,16 @@
 		'........',
 		'........'
 	])
 
 class DefiniteAnimations:
 	"""
 	The class with sets definite animations.
+
+	.. versionadded:: 0.0.0
 	"""
 	Dots = DefiniteAnimationType([
 		'        ',
 		'.       ',
 		'..      ',
 		'...     ',
 		'....    ',
```

### Comparing `mighty_logger-0.8.0/mighty_logger/src/ansi_format.py` & `mighty_logger-0.9.1/mighty_logger/src/ansi_format.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-A module with implementation of ANSI escape codes.
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -151,17 +149,22 @@
 	},
 }
 
 def _RecursiveGetAnsiFormat(ansi_address: str, ansi: dict) -> str:
 	"""
 	Recursively extracts a string with an ANSI escape code from a heavily nested dictionary.
 
+	.. versionadded:: 0.0.0
+
 	:param ansi_address: Path to ANSI escape code value
+	:type ansi_address: str
 	:param ansi: External/nested dictionary
+	:type ansi: dict
 	:return: value - ANSI escape code
+	:rtype: str
 	"""
 	split_address = ansi_address.split("/")
 	# print(split_address)
 	if type(ansi[split_address[0]]) == dict:
 		return _RecursiveGetAnsiFormat("/".join(split_address[1:]), ansi[split_address[0]])
 	else:
 		if len(split_address) == 2:
@@ -178,11 +181,15 @@
 	print(f"{GetAnsiFormat('blink/slow')}Test string")\n
 	print(f"{GetAnsiFormat('invert/off')}Test string")\n
 	print(f"{GetAnsiFormat('font/3th alternative')}Test string")\n
 	print(f"{GetAnsiFormat('color/foreground/green')}Test string")\n
 	print(f"{GetAnsiFormat('color/set/background/255;255;255')}Test string")\n
 	print(f"{GetAnsiFormat('reset/on')}Test string")\n
 
+	.. versionadded:: 0.0.0
+
 	:param ansi_address: Path to ANSI escape code value
+	:type ansi_address: str
 	:return: ANSI escape code
+	:rtype: str
 	"""
 	return _RecursiveGetAnsiFormat(ansi_address, AnsiFormat)
```

### Comparing `mighty_logger-0.8.0/mighty_logger/src/color_picker.py` & `mighty_logger-0.9.1/mighty_logger/src/color_picker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-A module with implementation of colors and their formatter functions.
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -175,86 +173,126 @@
 	'GAINSBORO': [220, 220, 220],
 }
 
 def DecColor(color_name: str) -> list[int, int, int]:
 	"""
 	Returns a decimal color value.
 
+	.. versionadded:: 0.0.0
+
 	:param color_name: Color name
+	:type color_name: str
 	:return: Decimal color value
+	:rtype: list[int, int, int]
+	:raises ColorException: This color is not in the dictionary
 	"""
 	if color_name in ColorPicker:
 		return ColorPicker[color_name]
 	else:
 		raise ColorException("This color is not in the dictionary")
 
 def HexColor(color_name: str) -> str:
 	"""
 	Returns a hexadecimal color value.
 
+	.. versionadded:: 0.0.0
+
 	:param color_name: Color name
+	:type color_name: str
 	:return: Hexadecimal color value
+	:rtype: str
+	:raises ColorException: This color is not in the dictionary
 	"""
-	return '{:02x}{:02x}{:02x}'.format(*DecColor(color_name))
+	if color_name in ColorPicker:
+		return '{:02x}{:02x}{:02x}'.format(*ColorPicker[color_name])
+	else:
+		raise ColorException("This color is not in the dictionary")
 
 def AnsiColor(color_name: str, color_ground: str) -> str:
 	"""
 	Returns an ANSI color value.\n
 	In AnsiFormat, the following levels are available under the "color/set/..." path:\n
 	- foreground
 	- background
 	- bright foreground
 	- bright background
 	- underline
 
+	.. versionadded:: 0.0.0
+
 	:param color_name: Color name
+	:type color_name: str
 	:param color_ground: Color level
+	:type color_ground: str
 	:return: ANSI color value
+	:rtype: str
+	:raises ColorException: This color is not in the dictionary
 	"""
-	return GetAnsiFormat("color/set/{}/{};{};{}".format(color_ground, *DecColor(color_name)))
+	if color_name in ColorPicker:
+		return GetAnsiFormat("color/set/{}/{};{};{}".format(color_ground, *ColorPicker[color_name]))
+	else:
+		raise ColorException("This color is not in the dictionary")
 
 def Dec2Hex(dec_colors: list[int, int, int]) -> str:
 	"""
 	Converts a decimal color value to a hexadecimal.
 
+	.. versionadded:: 0.0.0
+
 	:param dec_colors: Decimal color value
+	:type dec_colors: list[int, int, int]
 	:return: Hexadecimal color value
+	:rtype: str
 	"""
 	return '{:02x}{:02x}{:02x}'.format(*dec_colors)
 
 def Dec2Ansi(dec_colors: list[int, int, int], color_ground: str) -> str:
 	"""
 	Converts a decimal color value to an ANSI escape code.
 
+	.. versionadded:: 0.0.0
+
 	:param dec_colors: Decimal color value
+	:type dec_colors: list[int, int, int]
 	:param color_ground: Color level (read AnsiColor() function documentation)
+	:type color_ground: str
 	:return: ANSI escape code color value
+	:rtype: str
 	"""
 	return GetAnsiFormat("color/set/{}/{};{};{}".format(color_ground, *dec_colors))
 
 def Hex2Dec(hex_color: str) -> list[int, int, int]:
 	"""
 	Converts a hexadecimal color value to a decimal.
 
+	.. versionadded:: 0.0.0
+
 	:param hex_color: Hexadecimal color value
+	:type hex_color: str
 	:return: Decimal color value
+	:rtype: list[int, int, int]
 	"""
 	return [
 		int(hex_color[:2], base=16),
 		int(hex_color[2:4], base=16),
 		int(hex_color[4:], base=16)
 	]
 
 def Hex2Ansi(hex_color: str, color_ground: str) -> str:
 	"""
 	Converts a hexadecimal color value to an ANSI escape code.
 
+	.. versionadded:: 0.0.0
+
 	:param hex_color: Hexadecimal color value
+	:type hex_color: str
 	:param color_ground: Color level (read AnsiColor() function documentation)
+	:type color_ground: str
 	:return: ANSI escape code color value
+	:rtype: str
 	"""
 	return GetAnsiFormat("color/set/{}/{};{};{}".format(
 		color_ground,
 		int(hex_color[:2], base=16),
 		int(hex_color[2:4], base=16),
 		int(hex_color[4:], base=16)
 	))
@@ -262,31 +300,39 @@
 def Ansi2Dec(ansi_color: str) -> list[int, int, int]:
 	"""
 	Converts an ANSI escape code color value to a decimal.
 	When converting to ANSI escape code, you need to know which level the color is applied
 	to, and when from ANSI escape code, you don’t need to, because in other formats the levels
 	are defined differently and are not included in the command along with the color.
 
+	.. versionadded:: 0.0.0
+
 	:param ansi_color: ANSI escape code color value
+	:type ansi_color: str
 	:return: Decimal color value
+	:rtype: list[int, int, int]
 	"""
 	return [
 		int(ansi_color.split(';')[2]),
 		int(ansi_color.split(';')[3]),
 		int(ansi_color.split(';')[4][:-1])
 	]
 
 def Ansi2Hex(ansi_color: str) -> str:
 	"""
 	Converts an ANSI escape code color value to a hexadecimal.
 	When converting to ANSI escape code, you need to know which level the color is applied
 	to, and when from ANSI escape code, you don’t need to, because in other formats the levels
 	are defined differently and are not included in the command along with the color.
 
+	.. versionadded:: 0.0.0
+
 	:param ansi_color: ANSI escape code color value
+	:type ansi_color: str
 	:return: Hexadecimal color value
+	:rtype: str
 	"""
 	return '{:02x}{:02x}{:02x}'.format(
 		int(ansi_color.split(';')[2]),
 		int(ansi_color.split(';')[3]),
 		int(ansi_color.split(';')[4][:-1])
 	)
```

### Comparing `mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/__init__.py` & `mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-...
+A package containing lists of prebuilt objects of library types.
+
+.. versionadded:: 0.0.0
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/environments.py` & `mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/environments.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """
-A module with a list of environment options in which the modules work
-and entry types that can be passed to an entry in Progress bar.
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -18,13 +15,16 @@
 """
 
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 
 class LogEnvironments:
 	"""
 	Environments of Logger.
+
+	.. versionadded:: 0.0.0
 	"""
+
 	CONSOLE = EnvironmentType("CONSOLE", 0, True, False)
 	PLAIN_CONSOLE = EnvironmentType("PLAIN_CONSOLE", 1, True, False)
 	HTML = EnvironmentType("HTML", 2, False, True)
 	MARKDOWN = EnvironmentType("MARKDOWN", 3, False, True)
 	PLAIN = EnvironmentType("PLAIN", 4, False, False)
```

### Comparing `mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/sorting_keys.py` & `mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/sorting_keys.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-...
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,12 +12,20 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from mighty_logger.basic.lib_types.sorting_key_type import SortingKeyType
 
+# todo заменить числа на строки
+
 class SortingKeys:
+	"""
+	Sort keys.
+
+	.. versionadded:: 0.0.0
+	"""
+
 	SORT_ON_TIME = SortingKeyType(0)
 	SORT_ON_TIME_WITH_REVERSE = SortingKeyType(1)
 	SORT_ON_CATEGORY = SortingKeyType(2)
 	SORT_ON_TYPE = SortingKeyType(3)
```

### Comparing `mighty_logger-0.8.0/mighty_logger.egg-info/PKG-INFO` & `mighty_logger-0.9.1/mighty_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mighty-logger
-Version: 0.8.0
+Version: 0.9.1
 Summary: Powerful functional logger
-Home-page: https://github.com/Nakama3942/mighty_logger
-Author: Kalynovsky 'Nakamura Akira' Valentin
-Author-email: nakama3942@gmail.com
-License: Apache License, Version 2.0, see LICENSE file
+Author-email: Kalynovsky 'Nakamura Akira' Valentin <nakama3942@gmail.com>
+License: Apache License Version 2.0
+Project-URL: Repository, https://github.com/Nakama3942/mighty_logger
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -107,16 +106,18 @@
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [x] v0.6.1 - Animation update (added animations in processes)
 - [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
-- [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
-- [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
+- [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
+- [x] v0.9.1 - Documenting update (documented library)
+- [ ] v0.9.2 - Feature update (made optimizations)
+- [ ] v0.9.3 - Web docs update (added generation of web docs)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
```

### Comparing `mighty_logger-0.8.0/mighty_logger.egg-info/SOURCES.txt` & `mighty_logger-0.9.1/mighty_logger.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
-setup.py
 mighty_logger/__init__.py
 mighty_logger/mighty_logger.py
 mighty_logger/simple_logger.py
 mighty_logger.egg-info/PKG-INFO
 mighty_logger.egg-info/SOURCES.txt
 mighty_logger.egg-info/dependency_links.txt
 mighty_logger.egg-info/top_level.txt
@@ -25,10 +25,8 @@
 mighty_logger/src/__init__.py
 mighty_logger/src/animations.py
 mighty_logger/src/ansi_format.py
 mighty_logger/src/color_picker.py
 mighty_logger/src/lib_types_collection/__init__.py
 mighty_logger/src/lib_types_collection/entry_types.py
 mighty_logger/src/lib_types_collection/environments.py
-mighty_logger/src/lib_types_collection/sorting_keys.py
-test/test.py
-test/test_simple.py
+mighty_logger/src/lib_types_collection/sorting_keys.py
```

