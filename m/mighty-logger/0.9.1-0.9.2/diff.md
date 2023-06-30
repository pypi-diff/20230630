# Comparing `tmp/mighty_logger-0.9.1.tar.gz` & `tmp/mighty_logger-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mighty_logger-0.9.1.tar", last modified: Fri Jun 30 17:55:52 2023, max compression
+gzip compressed data, was "mighty_logger-0.9.2.tar", last modified: Fri Jun 30 19:35:28 2023, max compression
```

## Comparing `mighty_logger-0.9.1.tar` & `mighty_logger-0.9.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.539240 mighty_logger-0.9.1/
--rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.9.1/LICENSE
--rw-rw-rw-   0        0        0    10873 2023-06-30 17:55:52.541240 mighty_logger-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     9941 2023-06-30 17:52:14.000000 mighty_logger-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.121204 mighty_logger-0.9.1/mighty_logger/
--rw-rw-rw-   0        0        0      886 2023-06-30 15:04:11.000000 mighty_logger-0.9.1/mighty_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.360227 mighty_logger-0.9.1/mighty_logger/basic/
--rw-rw-rw-   0        0        0      808 2023-06-30 12:57:57.000000 mighty_logger-0.9.1/mighty_logger/basic/__init__.py
--rw-rw-rw-   0        0        0     8869 2023-06-30 13:13:14.000000 mighty_logger-0.9.1/mighty_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1842 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/exceptions.py
--rw-rw-rw-   0        0        0     3379 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/exporter.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.469236 mighty_logger-0.9.1/mighty_logger/basic/lib_types/
--rw-rw-rw-   0        0        0      961 2023-06-30 12:33:00.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/__init__.py
--rw-rw-rw-   0        0        0     1163 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/animation_type.py
--rw-rw-rw-   0        0        0     2079 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/entry_type.py
--rw-rw-rw-   0        0        0     1415 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/environment_type.py
--rw-rw-rw-   0        0        0      891 2023-06-30 13:42:10.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/sorting_key_type.py
--rw-rw-rw-   0        0        0     6706 2023-06-30 13:06:13.000000 mighty_logger-0.9.1/mighty_logger/basic/lib_types/text_buffer_type.py
--rw-rw-rw-   0        0        0     8207 2023-06-30 13:47:39.000000 mighty_logger-0.9.1/mighty_logger/basic/modifier.py
--rw-rw-rw-   0        0        0      842 2023-06-30 13:13:13.000000 mighty_logger-0.9.1/mighty_logger/basic/singleton.py
--rw-rw-rw-   0        0        0    10557 2023-06-30 13:13:13.000000 mighty_logger-0.9.1/mighty_logger/basic/text_buffer.py
--rw-rw-rw-   0        0        0    32357 2023-06-30 17:34:17.000000 mighty_logger-0.9.1/mighty_logger/mighty_logger.py
--rw-rw-rw-   0        0        0     6868 2023-06-30 17:43:48.000000 mighty_logger-0.9.1/mighty_logger/simple_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.512238 mighty_logger-0.9.1/mighty_logger/src/
--rw-rw-rw-   0        0        0      928 2023-06-30 14:44:07.000000 mighty_logger-0.9.1/mighty_logger/src/__init__.py
--rw-rw-rw-   0        0        0     9983 2023-06-30 14:44:07.000000 mighty_logger-0.9.1/mighty_logger/src/animations.py
--rw-rw-rw-   0        0        0     4664 2023-06-30 14:44:07.000000 mighty_logger-0.9.1/mighty_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     9688 2023-06-30 14:46:54.000000 mighty_logger-0.9.1/mighty_logger/src/color_picker.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.529240 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/
--rw-rw-rw-   0        0        0      865 2023-06-30 14:14:17.000000 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/__init__.py
--rw-rw-rw-   0        0        0    47441 2023-06-30 14:22:00.000000 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/entry_types.py
--rw-rw-rw-   0        0        0     1030 2023-06-30 14:14:17.000000 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/environments.py
--rw-rw-rw-   0        0        0      975 2023-06-30 14:14:17.000000 mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/sorting_keys.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:55:52.137204 mighty_logger-0.9.1/mighty_logger.egg-info/
--rw-rw-rw-   0        0        0    10873 2023-06-30 17:55:52.000000 mighty_logger-0.9.1/mighty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2023-06-30 17:55:52.000000 mighty_logger-0.9.1/mighty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 17:55:52.000000 mighty_logger-0.9.1/mighty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 17:55:52.000000 mighty_logger-0.9.1/mighty_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1869 2023-06-29 15:07:42.000000 mighty_logger-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 17:55:52.543240 mighty_logger-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.903619 mighty_logger-0.9.2/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0    10873 2023-06-30 19:35:28.904619 mighty_logger-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9941 2023-06-30 19:23:51.000000 mighty_logger-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.723312 mighty_logger-0.9.2/mighty_logger/
+-rw-rw-rw-   0        0        0      846 2023-06-30 19:00:03.000000 mighty_logger-0.9.2/mighty_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.802614 mighty_logger-0.9.2/mighty_logger/basic/
+-rw-rw-rw-   0        0        0      808 2023-06-30 12:57:57.000000 mighty_logger-0.9.2/mighty_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     8659 2023-06-30 18:38:56.000000 mighty_logger-0.9.2/mighty_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1805 2023-06-30 18:18:43.000000 mighty_logger-0.9.2/mighty_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0     3379 2023-06-30 13:42:10.000000 mighty_logger-0.9.2/mighty_logger/basic/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.863621 mighty_logger-0.9.2/mighty_logger/basic/lib_types/
+-rw-rw-rw-   0        0        0      961 2023-06-30 12:33:00.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/__init__.py
+-rw-rw-rw-   0        0        0     1163 2023-06-30 13:42:10.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/animation_type.py
+-rw-rw-rw-   0        0        0     2079 2023-06-30 13:42:10.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/entry_type.py
+-rw-rw-rw-   0        0        0     1415 2023-06-30 13:42:10.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/environment_type.py
+-rw-rw-rw-   0        0        0      891 2023-06-30 18:04:36.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/sorting_key_type.py
+-rw-rw-rw-   0        0        0     6706 2023-06-30 13:06:13.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/text_buffer_type.py
+-rw-rw-rw-   0        0        0     8207 2023-06-30 13:47:39.000000 mighty_logger-0.9.2/mighty_logger/basic/modifier.py
+-rw-rw-rw-   0        0        0      842 2023-06-30 13:13:13.000000 mighty_logger-0.9.2/mighty_logger/basic/singleton.py
+-rw-rw-rw-   0        0        0    10557 2023-06-30 13:13:13.000000 mighty_logger-0.9.2/mighty_logger/basic/text_buffer.py
+-rw-rw-rw-   0        0        0    31663 2023-06-30 19:11:51.000000 mighty_logger-0.9.2/mighty_logger/mighty_logger.py
+-rw-rw-rw-   0        0        0     7446 2023-06-30 19:10:22.000000 mighty_logger-0.9.2/mighty_logger/simple_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.870619 mighty_logger-0.9.2/mighty_logger/src/
+-rw-rw-rw-   0        0        0      928 2023-06-30 14:44:07.000000 mighty_logger-0.9.2/mighty_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     9983 2023-06-30 14:44:07.000000 mighty_logger-0.9.2/mighty_logger/src/animations.py
+-rw-rw-rw-   0        0        0     4664 2023-06-30 14:44:07.000000 mighty_logger-0.9.2/mighty_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     9688 2023-06-30 14:46:54.000000 mighty_logger-0.9.2/mighty_logger/src/color_picker.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.875620 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/
+-rw-rw-rw-   0        0        0      865 2023-06-30 14:14:17.000000 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/__init__.py
+-rw-rw-rw-   0        0        0    47441 2023-06-30 14:22:00.000000 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/entry_types.py
+-rw-rw-rw-   0        0        0     1030 2023-06-30 14:14:17.000000 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/environments.py
+-rw-rw-rw-   0        0        0      956 2023-06-30 18:04:36.000000 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/sorting_keys.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.756613 mighty_logger-0.9.2/mighty_logger.egg-info/
+-rw-rw-rw-   0        0        0    10873 2023-06-30 19:35:28.000000 mighty_logger-0.9.2/mighty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2023-06-30 19:35:28.000000 mighty_logger-0.9.2/mighty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 19:35:28.000000 mighty_logger-0.9.2/mighty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 19:35:28.000000 mighty_logger-0.9.2/mighty_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1869 2023-06-30 19:23:51.000000 mighty_logger-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 19:35:28.905620 mighty_logger-0.9.2/setup.cfg
```

### Comparing `mighty_logger-0.9.1/LICENSE` & `mighty_logger-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/PKG-INFO` & `mighty_logger-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mighty_logger
-Version: 0.9.1
+Version: 0.9.2
 Summary: Powerful functional logger
 Author-email: Kalynovsky 'Nakamura Akira' Valentin <nakama3942@gmail.com>
 License: Apache License Version 2.0
 Project-URL: Repository, https://github.com/Nakama3942/mighty_logger
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -108,15 +108,15 @@
 - [x] v0.6.1 - Animation update (added animations in processes)
 - [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
 - [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [x] v0.9.1 - Documenting update (documented library)
-- [ ] v0.9.2 - Feature update (made optimizations)
+- [x] v0.9.2 - Feature update (made optimizations)
 - [ ] v0.9.3 - Web docs update (added generation of web docs)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
```

### Comparing `mighty_logger-0.9.1/README.md` & `mighty_logger-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 - [x] v0.6.1 - Animation update (added animations in processes)
 - [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
 - [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [x] v0.9.1 - Documenting update (documented library)
-- [ ] v0.9.2 - Feature update (made optimizations)
+- [x] v0.9.2 - Feature update (made optimizations)
 - [ ] v0.9.3 - Web docs update (added generation of web docs)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
```

### Comparing `mighty_logger-0.9.1/mighty_logger/__init__.py` & `mighty_logger-0.9.2/mighty_logger/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,13 +14,12 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .mighty_logger import MightyLogger
 from .simple_logger import Logger
 
 __authot__ = "Kalynovsky 'Nakamura Akira' Valentin"
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/__init__.py` & `mighty_logger-0.9.2/mighty_logger/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/basic_logger.py` & `mighty_logger-0.9.2/mighty_logger/basic/basic_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 
 		:param colors: Color string list of initialized data
 		:type colors: list[str, str]
 		:return: A string with initialized data
 		:rtype: str
 		"""
 		match self._environment.environment_name:
-			# todo оптимизировать
 			case LogEnvironments.CONSOLE.environment_name:
 				return (
 					f"{colors[1]}" +
 					f"{colors[0]}-{self._program_name}?entry> " +
 					f"${platform.node()}:{getlogin()}" +
 					f":{platform.system()}" +
 					f":{platform.version()}" +
@@ -115,15 +114,14 @@
 
 	def _assemble_entry(
 		self,
 		entry_type: EntryType,
 		icon_set: int,
 		animation: str,
 		message_text: str,
-		entry_background: bool,
 		local_settings: dict
 	) -> str:
 		"""
 		A method that assemble an entry into a string and returns it.
 
 		.. versionadded:: 0.0.0
 
@@ -131,43 +129,41 @@
 		:type entry_type: EntryType
 		:param icon_set: Icon set number
 		:type icon_set: int
 		:param animation: Animation frame of entry
 		:type animation: str
 		:param message_text: Message of entry
 		:type message_text: str
-		:param entry_background: Flag indicating setting the background of the entry string
-		:type entry_background: bool
 		:param local_settings: Settings for the string of the current entry
 		:type local_settings: dict
 		:return: The formed entry string
 		:rtype: str
 		:raises MessageException: Message is too short (less than 10 characters)
 		"""
 		if len(message_text) < 10:
 			raise MessageException("Message is too short (less than 10 characters)")
 
 		bold = local_settings['bold'] if 'bold' in local_settings else self._settings['global_bold_font']
 		italic = local_settings['italic'] if 'italic' in local_settings else self._settings['global_italic_font']
 		invert = local_settings['invert'] if 'invert' in local_settings else self._settings['global_invert_font']
+		background = local_settings['background'] if 'background' in local_settings else self._settings['global_background']
 
 		match self._environment.environment_name:
-			# todo оптимизировать
 			case LogEnvironments.CONSOLE.environment_name:
 				return (
 					(f"{GetAnsiFormat('bold/on')}" if bold else "") +
 					(f"{GetAnsiFormat('italic/on')}" if italic else "") +
 					(f"{GetAnsiFormat('invert/on')}" if invert else "") +
-					f"{entry_type.background_color[self._environment.environment_code][entry_background]}" +
-					f"{entry_type.message_color[self._environment.environment_code][entry_background]}-?entry> {animation} " +
-					f"{entry_type.time_color[self._environment.environment_code][entry_background]}*{datetime.now()} " +
+					f"{entry_type.background_color[self._environment.environment_code][background]}" +
+					f"{entry_type.message_color[self._environment.environment_code][background]}-?entry> {animation} " +
+					f"{entry_type.time_color[self._environment.environment_code][background]}*{datetime.now()} " +
 					f"{entry_type.icon[icon_set]} " +
-					f"{entry_type.status_color[self._environment.environment_code][entry_background]}#STATUS: " +
-					f"{entry_type.type_color[self._environment.environment_code][entry_background]}{entry_type.type_category}{entry_type.type_name} - " +
-					f"{entry_type.message_color[self._environment.environment_code][entry_background]}{message_text}" +
+					f"{entry_type.status_color[self._environment.environment_code][background]}#STATUS: " +
+					f"{entry_type.type_color[self._environment.environment_code][background]}{entry_type.type_category}{entry_type.type_name} - " +
+					f"{entry_type.message_color[self._environment.environment_code][background]}{message_text}" +
 					f"{GetAnsiFormat('reset/on')}"
 				)
 			case LogEnvironments.PLAIN_CONSOLE.environment_name:
 				return (
 					f"-?entry> {animation} " +
 					f"*{datetime.now()} " +
 					f"{entry_type.icon[icon_set]} " +
@@ -175,35 +171,35 @@
 					f"{entry_type.type_category}{entry_type.type_name} - " +
 					f"{message_text}"
 				)
 			case LogEnvironments.HTML.environment_name:
 				return (
 					(f"<b>" if bold else "") +
 					(f"<i>" if italic else "") +
-					f"<span style='background-color: #{entry_type.background_color[self._environment.environment_code][entry_background]};'>" +
-					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>-?entry> {animation} </span>" +
-					f"<span style='color: #{entry_type.time_color[self._environment.environment_code][entry_background]};'>*{datetime.now()} </span>" +
+					f"<span style='background-color: #{entry_type.background_color[self._environment.environment_code][background]};'>" +
+					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][background]};'>-?entry> {animation} </span>" +
+					f"<span style='color: #{entry_type.time_color[self._environment.environment_code][background]};'>*{datetime.now()} </span>" +
 					f"{entry_type.icon[icon_set]} " +
-					f"<span style='color: #{entry_type.status_color[self._environment.environment_code][entry_background]};'>#STATUS: </span>" +
-					f"<span style='color: #{entry_type.type_color[self._environment.environment_code][entry_background]};'>{entry_type.type_category}{entry_type.type_name} - </span>" +
-					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>{message_text}</span></span>" +
+					f"<span style='color: #{entry_type.status_color[self._environment.environment_code][background]};'>#STATUS: </span>" +
+					f"<span style='color: #{entry_type.type_color[self._environment.environment_code][background]};'>{entry_type.type_category}{entry_type.type_name} - </span>" +
+					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][background]};'>{message_text}</span></span>" +
 					(f"</i>" if italic else "") +
 					(f"</b>" if bold else "")
 				)
 			case LogEnvironments.MARKDOWN.environment_name:
 				return (
 					(f"<b>" if bold else "") +
 					(f"<i>" if italic else "") +
-					f"<span style='background-color: #{entry_type.background_color[self._environment.environment_code][entry_background]};'>" +
-					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>-?entry> {animation} </span>" +
-					f"<span style='color: #{entry_type.time_color[self._environment.environment_code][entry_background]};'>*{datetime.now()} </span>" +
+					f"<span style='background-color: #{entry_type.background_color[self._environment.environment_code][background]};'>" +
+					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][background]};'>-?entry> {animation} </span>" +
+					f"<span style='color: #{entry_type.time_color[self._environment.environment_code][background]};'>*{datetime.now()} </span>" +
 					f"{entry_type.icon[icon_set]} " +
-					f"<span style='color: #{entry_type.status_color[self._environment.environment_code][entry_background]};'>#STATUS: </span>" +
-					f"<span style='color: #{entry_type.type_color[self._environment.environment_code][entry_background]};'>{entry_type.type_category}{entry_type.type_name} - </span>" +
-					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>{message_text}</span></span>" +
+					f"<span style='color: #{entry_type.status_color[self._environment.environment_code][background]};'>#STATUS: </span>" +
+					f"<span style='color: #{entry_type.type_color[self._environment.environment_code][background]};'>{entry_type.type_category}{entry_type.type_name} - </span>" +
+					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][background]};'>{message_text}</span></span>" +
 					(f"</i>" if italic else "") +
 					(f"</b>" if bold else "")
 				)
 			case LogEnvironments.PLAIN.environment_name:
 				return (
 					f"-?entry> {animation} " +
 					f"*{datetime.now()} " +
```

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/exceptions.py` & `mighty_logger-0.9.2/mighty_logger/basic/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-# todo разбить в пакет
-
 class ColorException(BaseException):
 	"""
 	The exception that is thrown when there is no color in any palette.
 
 	.. versionadded:: 0.0.0
 	"""
```

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/exporter.py` & `mighty_logger-0.9.2/mighty_logger/basic/exporter.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/lib_types/__init__.py` & `mighty_logger-0.9.2/mighty_logger/basic/lib_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/lib_types/animation_type.py` & `mighty_logger-0.9.2/mighty_logger/basic/lib_types/animation_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/lib_types/entry_type.py` & `mighty_logger-0.9.2/mighty_logger/basic/lib_types/entry_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/lib_types/environment_type.py` & `mighty_logger-0.9.2/mighty_logger/basic/lib_types/environment_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/lib_types/sorting_key_type.py` & `mighty_logger-0.9.2/mighty_logger/basic/lib_types/sorting_key_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 class SortingKeyType:
 	"""
 	A data type that characterizes the sort keys for entries.
 
 	.. versionadded:: 0.0.0
 	"""
 
-	def __init__(self, sorting_key: int):
-		self.__sorting_key: int = sorting_key
+	def __init__(self, sorting_key: str):
+		self.__sorting_key: str = sorting_key
 
 	@property
-	def sorting_key(self) -> int:
+	def sorting_key(self) -> str:
 		return self.__sorting_key
```

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/lib_types/text_buffer_type.py` & `mighty_logger-0.9.2/mighty_logger/basic/lib_types/text_buffer_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/modifier.py` & `mighty_logger-0.9.2/mighty_logger/basic/modifier.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/singleton.py` & `mighty_logger-0.9.2/mighty_logger/basic/singleton.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/basic/text_buffer.py` & `mighty_logger-0.9.2/mighty_logger/basic/text_buffer.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/mighty_logger.py` & `mighty_logger-0.9.2/mighty_logger/mighty_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,29 +62,29 @@
 		program_name: str = "Unknown",
 		log_environment: EnvironmentType = LogEnvironments.PLAIN,
 		console_width: int = 60,
 		icon_set: int = 1,
 		global_bold_font: bool = False,
 		global_italic_font: bool = False,
 		global_invert_font: bool = False,
-		global_background: bool = False,
+		global_background: bool = False
 	) -> None:
 		if not hasattr(self, "_environment"):
 			super().__init__(program_name, log_environment)
 			self._animation: BasicAnimationType = BasicAnimationType([])
 			self._icon_set = icon_set if 0 < icon_set < 5 else 1
 			self._settings["global_bold_font"] = global_bold_font
 			self._settings["global_italic_font"] = global_italic_font
 			self._settings["global_invert_font"] = global_invert_font
+			self._settings["global_background"] = global_background
 			self._progress_rise = 0
 			self._progress_start: datetime | None = None
 			self._progress_time: str = "        "
 			self._progress_interrupt = False
 			self._start_timer_value: datetime | None = None
-			self._global_background = global_background
 			self._buffer: TextBufferType = TextBufferType(log_environment)
 			self._init_buffer(console_width)
 			self._initial_log()
 		else:
 			raise ReCreationException("Logger class object already created")
 
 	def _init_buffer(self, console_width: int) -> None:
@@ -124,16 +124,16 @@
 
 		.. versionadded:: 0.0.0
 		"""
 		if self._environment.weak_environment:
 			self._buffer << "<body style='background-color: #000000; color: #ffffff;'>"
 		self._buffer << self._initialized_data(
 			[
-				ServiceLogger.initial[0][self._environment.environment_code][self._global_background],
-				ServiceLogger.initial[1][self._environment.environment_code][self._global_background]
+				ServiceLogger.initial[0][self._environment.environment_code][self._settings["global_background"]],
+				ServiceLogger.initial[1][self._environment.environment_code][self._settings["global_background"]]
 			]
 		)
 		if self._environment.updatable:
 			self._buffer.update_console()
 
 	def set_icons(self, icon_set: int) -> None:
 		"""
@@ -142,15 +142,55 @@
 		.. versionadded:: 0.0.0
 
 		:param icon_set: Icon set to use
 		:type icon_set: int
 		"""
 		self._icon_set = icon_set if 0 < icon_set < 5 else 1
 
-	# todo добавить методы-настройки и скрыть из __init__
+	def set_settings(
+		self,
+		*,
+		global_bold_font: bool = None,
+		global_italic_font: bool = None,
+		global_invert_font: bool = None,
+		global_background: bool = None
+	) -> None:
+		"""
+		Method that sets new Logger settings.
+
+		.. versionadded:: 0.9.2
+
+		:param global_bold_font: Sets the global setting "bold font"
+		:type global_bold_font: bool
+		:param global_italic_font: Sets the global setting "italic font"
+		:type global_italic_font: bool
+		:param global_invert_font: Sets the global setting "invert font"
+		:type global_invert_font: bool
+		:param global_background: Sets the global setting "background"
+		:type global_background: bool
+		"""
+		if global_bold_font is not None:
+			self._settings['global_bold_font'] = global_bold_font
+		if global_italic_font is not None:
+			self._settings['global_italic_font'] = global_italic_font
+		if global_invert_font is not None:
+			self._settings['global_invert_font'] = global_invert_font
+		if global_background is not None:
+			self._settings['global_background'] = global_background
+
+	def get_settings(self) -> dict:
+		"""
+		Returns a dictionary of settings.
+
+		.. versionadded:: 0.9.2
+
+		:return: A dictionary of settings
+		:rtype: dict
+		"""
+		return self._settings
 
 	# ######################################################################################## #
 	#                                                                                          #
 	#                                        Publishers                                        #
 	#                                                                                          #
 	# ######################################################################################## #
 
@@ -184,14 +224,15 @@
 
 		.. versionadded:: 0.0.0
 		"""
 		self.empty("Global settings:")
 		self.empty(f"    Bold font is set to {str(self._settings['global_bold_font'])};")
 		self.empty(f"    Italic font is set to {str(self._settings['global_italic_font'])};")
 		self.empty(f"    Invert font is set to {str(self._settings['global_invert_font'])};")
+		self.empty(f"    Background is set to {str(self._settings['global_background'])};")
 
 	def publish_author(self) -> None:
 		"""
 		A method that publishes information about the Author of the library to the Logger Buffer.
 
 		.. versionadded:: 0.0.0
 		"""
@@ -504,56 +545,50 @@
 	#                                                                                          #
 	# ######################################################################################## #
 
 	def entry(
 		self,
 		entry_type: EntryType,
 		message_text: str,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		A method that generates and adds an entry to the Logger.
 
 		.. versionadded:: 0.0.0
 
 		:param entry_type: Entry type
 		:type entry_type: EntryType
 		:param message_text: Log entry message
 		:type message_text: str
-		:param local_background: Display entry with background?
-		:type local_background: bool
 		:param local_settings: Dictionary of local entering settings
 		:type local_settings: dict
 		"""
 		if local_settings is None:
 			local_settings = {}
-		background = local_background if local_background is not None else self._global_background
 		self.empty(
 			self._assemble_entry(
 				entry_type,
 				self._icon_set,
 				self._progress_time,
 				message_text,
-				background,
 				local_settings
 			)
 		)
 
 	# ######################################################################################## #
 	#                                                                                          #
 	#                                  Entering to Processes                                   #
 	#                                                                                          #
 	# ######################################################################################## #
 
 	def start_indefinite_process(
 		self,
 		message_text: str,
 		animation: IndefiniteAnimationType = IndefiniteAnimations.Line,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		A method that starts the whole process of indefinite logging. While the process
 		is running, you cannot start other processes in the Logger and call the entering
 		methods directly. While the process is running - the last entry will play
 		the animation of the process. Before starting a process, you can specify that
@@ -561,38 +596,33 @@
 
 		.. versionadded:: 0.6.0
 
 		:param message_text: Log entry message
 		:type message_text: str
 		:param animation: The name of the animation that will play in the Progress entry
 		:type animation: IndefiniteAnimationType
-		:param local_background: Display entry with background?
-		:type local_background: bool
 		:param local_settings: Dictionary of local entering settings
 		:type local_settings: dict
 		"""
 		self._animation = animation
 
 		self._progress_start = datetime.now()
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		args = {'message_text': message_text}
-		if local_background is not None:
-			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(ServiceProcessEntryTypes.initiation, **args)
 
 		thread = Thread(target=self._indefinite_progress, kwargs=args)
 		thread.start()
 
 	def _indefinite_progress(
 		self,
 		message_text: str,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		A method that creates an animation entry. Only works on the last string.
 		You need to run in a thread. Terminates when the process stop flag
 		is set by the Logger.stop_process() method.
 
@@ -609,35 +639,32 @@
 			local_settings = {}
 		animation_index = 0
 		self._buffer << "."
 		if self._environment.updatable:
 			self._buffer.update_console()
 		while not self._progress_interrupt:
 			animation_item = self._animation.animation[animation_index]
-			background = local_background if local_background is not None else self._global_background
 			self._buffer.get_data()[-1] = self._assemble_entry(
 				ServiceProcessEntryTypes.process,
 				self._icon_set,
 				animation_item,
 				message_text,
-				background,
 				local_settings
 			)
 			animation_index = (animation_index + 1) % len(self._animation.animation)
 			if self._environment.updatable:
 				self._buffer.update_entry()
 			sleep(0.1)
 		if self._environment.updatable:
 			self._buffer.update_console()
 
 	def start_definite_process(
 		self,
 		message_text: str,
 		progress_bar: DefiniteAnimationType = DefiniteAnimations.Line,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		A method that starts the whole process of a definite logging. While the process
 		is running, you cannot start other processes in the Logger and call the entering
 		methods directly. While the process is running - the last entry will display
 		the progress of the process. Before starting a process, you can specify that
@@ -645,38 +672,33 @@
 
 		.. versionadded:: 0.6.0
 
 		:param message_text: Log entry message
 		:type message_text: str
 		:param progress_bar: The name of the progress bar that will play in the Progress entry
 		:type progress_bar: DefiniteAnimationType
-		:param local_background: Display entry with background?
-		:type local_background: bool
 		:param local_settings: Dictionary of local entering settings
 		:type local_settings: dict
 		"""
 		self._animation = progress_bar
 
 		self._progress_start = datetime.now()
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		args = {'message_text': message_text}
-		if local_background is not None:
-			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(ServiceProcessEntryTypes.initiation, **args)
 
 		thread = Thread(target=self._definite_progress, kwargs=args)
 		thread.start()
 
 	def _definite_progress(
 		self,
 		message_text: str,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		A method that creates a progress bar entry. Only works on the last string.
 		You need to run in a thread. Terminates when the process stop flag
 		is set by the Logger.stop_process() method.
 
@@ -697,21 +719,19 @@
 			self._buffer.update_console()
 		while not self._progress_interrupt:
 			if old_progress_rise == self._progress_rise:
 				continue
 			else:
 				old_progress_rise = self._progress_rise
 				animation_item = f"{self._animation.animation[(self._progress_rise // 15) + (2 if self._progress_rise == 100 else 1)]} - {self._progress_rise} %"
-				background = local_background if local_background is not None else self._global_background
 				self._buffer.get_data()[-1] = self._assemble_entry(
 					ServiceProcessEntryTypes.process,
 					self._icon_set,
 					animation_item,
 					message_text,
-					background,
 					local_settings
 				)
 				if self._environment.updatable:
 					self._buffer.update_entry()
 			sleep(0.1)
 		if self._environment.updatable:
 			self._buffer.update_console()
@@ -730,15 +750,14 @@
 		"""
 		self._progress_rise = percent
 
 	def note_process(
 		self,
 		entry_type: EntryType,
 		message_text: str,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		An important method that allows you to add standard non-process entry types
 		while a process is running. It's important to note that this entry will still be
 		associated with the process, so it's best to use this entry when you want to describe
 		intermediate process execution entries beyond process initiation, progress, and
@@ -750,63 +769,54 @@
 
 		.. versionadded:: 0.6.0
 
 		:param entry_type: The type of entry to be entered in the progress history
 		:type entry_type: EntryType
 		:param message_text: Log entry message
 		:type message_text: str
-		:param local_background: Display entry with background?
-		:type local_background: bool
 		:param local_settings: Dictionary of local entering settings
 		:type local_settings: dict
 		"""
 		sleep(0.001)
 		last = self._buffer.pop()
 
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		args = {'message_text': message_text}
-		if local_background is not None:
-			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(entry_type, **args)
 
 		self.empty(last)
 
 	def stop_process(
 		self,
 		message_text: str,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		The method that terminates the process. If before the end of the process
 		its execution has reached 100% - the process was completed successfully,
 		otherwise - failed. After calling this method, the Progress entry will be replaced
 		by the entry with the result of the process execution.
 
 		.. versionadded:: 0.6.0
 
 		:param message_text: Log entry message
 		:type message_text: str
-		:param local_background: Display entry with background?
-		:type local_background: bool
 		:param local_settings: Dictionary of local entering settings
 		:type local_settings: dict
 		"""
 		self._progress_interrupt = True
 		sleep(0.11)
 		self._buffer.remove()
 
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		args = {'message_text': message_text}
-		if local_background is not None:
-			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(
 			ServiceProcessEntryTypes.success if self._progress_rise == 100 else ServiceProcessEntryTypes.fail,
 			**args
 		)
 
@@ -820,100 +830,85 @@
 	#                                     Entering to Timer                                    #
 	#                                                                                          #
 	# ######################################################################################## #
 
 	def start_timer(
 		self,
 		message_text: str,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		Stores the current time as the start time and write entry about the current time.
 
 		.. versionadded:: 0.6.1
 		?
 
 		:param message_text: Log entry message
 		:type message_text: str
-		:param local_background: Display entry with background?
-		:type local_background: bool
 		:param local_settings: Dictionary of local entering settings
 		:type local_settings: dict
 		"""
 		self._start_timer_value = datetime.now()
 		stop_timer_value = datetime.now()
 		self._progress_time = "^" + str(stop_timer_value - self._start_timer_value).split(".")[0]
 
 		args = {'message_text': message_text}
-		if local_background is not None:
-			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(ServiceTimerEntryTypes.start_timer, **args)
 
 		self._progress_time = "        "
 
 	def timer_mark(
 		self,
 		message_text: str,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		Calculates the difference between current and start time
 		and write entry about the difference.
 
 		.. versionadded:: 0.6.1
 		?
 
 		:param message_text: Log entry message
 		:type message_text: str
-		:param local_background: Display entry with background?
-		:type local_background: bool
 		:param local_settings: Dictionary of local entering settings
 		:type local_settings: dict
 		"""
 		mark_timer_value = datetime.now()
 		self._progress_time = "^" + str(mark_timer_value - self._start_timer_value).split(".")[0]
 
 		args = {'message_text': message_text}
-		if local_background is not None:
-			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(ServiceTimerEntryTypes.timer_mark, **args)
 
 		self._progress_time = "        "
 
 	def stop_timer(
 		self,
 		message_text: str,
-		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		Calculates the difference between the current and start time,
 		write entry about the difference, and resets the start time.
 
 		.. versionadded:: 0.6.1
 		?
 
 		:param message_text: Log entry message
 		:type message_text: str
-		:param local_background: Display entry with background?
-		:type local_background: bool
 		:param local_settings: Dictionary of local entering settings
 		:type local_settings: dict
 		"""
 		stop_timer_value = datetime.now()
 		self._progress_time = "^" + str(stop_timer_value - self._start_timer_value).split(".")[0]
 
 		args = {'message_text': message_text}
-		if local_background is not None:
-			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(ServiceTimerEntryTypes.stop_timer, **args)
 
 		self._start_timer_value = None
 		self._progress_time = "        "
```

### Comparing `mighty_logger-0.9.1/mighty_logger/simple_logger.py` & `mighty_logger-0.9.2/mighty_logger/simple_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,42 +11,61 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
+from mighty_logger.basic.singleton import Singleton
 from mighty_logger.src.lib_types_collection.entry_types import LoggerEntryTypes, ServiceProcessEntryTypes
 from mighty_logger.src.lib_types_collection.environments import LogEnvironments
 from mighty_logger.mighty_logger import MightyLogger
 
-class Logger:
+class Logger(Singleton):
 	"""
 	Lightweight Logger automates work with entry types.
 
 	.. versionadded:: 0.0.0
 	"""
 
 	def __init__(
 		self,
 		program_name: str = "Unknown",
-		environment: EnvironmentType = LogEnvironments.PLAIN,
-		console_width: int = 60
+		log_environment: EnvironmentType = LogEnvironments.PLAIN,
+		console_width: int = 60,
+		icon_set: int = 1,
+		global_bold_font: bool = False,
+		global_italic_font: bool = False,
+		global_invert_font: bool = False,
+		global_background: bool = False
 	) -> None:
 		if MightyLogger._instance is not None:
 			self.__logger = MightyLogger._instance
 			self.notice("An existing logger was taken into use")
 		else:
 			self.__logger = MightyLogger(
 				program_name=program_name,
-				log_environment=environment,
+				log_environment=log_environment,
 				console_width=console_width,
+				icon_set=icon_set,
+				global_bold_font=global_bold_font,
+				global_italic_font=global_italic_font,
+				global_invert_font=global_invert_font,
+				global_background=global_background
 			)
 
 	def might(self) -> MightyLogger:
+		"""
+		Provides access to "mighty" Logger methods.
+
+		.. versionadded:: 0.0.0
+
+		:return: A "mighty" Logger
+		:rtype: MightyLogger
+		"""
 		return self.__logger
 
 	def debug(self, message_text: str) -> None:
 		"""
 		Debugging information logging:
 		Can be used to log entry any information while debugging an application.
```

### Comparing `mighty_logger-0.9.1/mighty_logger/src/__init__.py` & `mighty_logger-0.9.2/mighty_logger/src/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/src/animations.py` & `mighty_logger-0.9.2/mighty_logger/src/animations.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/src/ansi_format.py` & `mighty_logger-0.9.2/mighty_logger/src/ansi_format.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/src/color_picker.py` & `mighty_logger-0.9.2/mighty_logger/src/color_picker.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/__init__.py` & `mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/entry_types.py` & `mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/entry_types.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/environments.py` & `mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/environments.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/mighty_logger/src/lib_types_collection/sorting_keys.py` & `mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/sorting_keys.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from mighty_logger.basic.lib_types.sorting_key_type import SortingKeyType
 
-# todo заменить числа на строки
-
 class SortingKeys:
 	"""
 	Sort keys.
 
 	.. versionadded:: 0.0.0
 	"""
 
-	SORT_ON_TIME = SortingKeyType(0)
-	SORT_ON_TIME_WITH_REVERSE = SortingKeyType(1)
-	SORT_ON_CATEGORY = SortingKeyType(2)
-	SORT_ON_TYPE = SortingKeyType(3)
+	SORT_ON_TIME = SortingKeyType("time")
+	SORT_ON_TIME_WITH_REVERSE = SortingKeyType("time_with_reverse")
+	SORT_ON_CATEGORY = SortingKeyType("category")
+	SORT_ON_TYPE = SortingKeyType("type")
```

### Comparing `mighty_logger-0.9.1/mighty_logger.egg-info/PKG-INFO` & `mighty_logger-0.9.2/mighty_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mighty-logger
-Version: 0.9.1
+Version: 0.9.2
 Summary: Powerful functional logger
 Author-email: Kalynovsky 'Nakamura Akira' Valentin <nakama3942@gmail.com>
 License: Apache License Version 2.0
 Project-URL: Repository, https://github.com/Nakama3942/mighty_logger
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -108,15 +108,15 @@
 - [x] v0.6.1 - Animation update (added animations in processes)
 - [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
 - [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [x] v0.9.1 - Documenting update (documented library)
-- [ ] v0.9.2 - Feature update (made optimizations)
+- [x] v0.9.2 - Feature update (made optimizations)
 - [ ] v0.9.3 - Web docs update (added generation of web docs)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
```

### Comparing `mighty_logger-0.9.1/mighty_logger.egg-info/SOURCES.txt` & `mighty_logger-0.9.2/mighty_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.1/pyproject.toml` & `mighty_logger-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mighty_logger"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
 	{name = "Kalynovsky 'Nakamura Akira' Valentin", email = "nakama3942@gmail.com"},
 ]
 description = "Powerful functional logger"
 readme = "README.md"
 license = {text = "Apache License Version 2.0"}
 classifiers = [
```

