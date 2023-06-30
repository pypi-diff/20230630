# Comparing `tmp/mkdoxy-1.0.6.tar.gz` & `tmp/mkdoxy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.0.6.tar", last modified: Sat Apr  1 12:27:31 2023, max compression
+gzip compressed data, was "mkdoxy-1.1.0.tar", last modified: Fri Jun 30 11:39:37 2023, max compression
```

## Comparing `mkdoxy-1.0.6.tar` & `mkdoxy-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-04-01 12:27:31.417200 mkdoxy-1.0.6/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.0.6/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     9049 2023-04-01 12:27:31.417001 mkdoxy-1.0.6/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     8271 2023-04-01 12:26:56.000000 mkdoxy-1.0.6/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-04-01 12:27:31.412835 mkdoxy-1.0.6/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.0.6/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.0.6/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     2779 2023-01-25 07:25:08.000000 mkdoxy-1.0.6/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     3928 2023-01-25 07:25:08.000000 mkdoxy-1.0.6/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     2861 2023-03-21 12:31:35.000000 mkdoxy-1.0.6/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)     2228 2023-01-25 07:15:22.000000 mkdoxy-1.0.6/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)     9200 2023-03-21 15:23:09.000000 mkdoxy-1.0.6/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    10415 2023-04-01 09:31:21.000000 mkdoxy-1.0.6/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)     9275 2023-01-25 07:25:08.000000 mkdoxy-1.0.6/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.0.6/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    19592 2023-01-25 07:25:08.000000 mkdoxy-1.0.6/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     6286 2023-04-01 12:05:27.000000 mkdoxy-1.0.6/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)     8794 2023-01-25 07:25:08.000000 mkdoxy-1.0.6/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-04-01 12:27:31.416773 mkdoxy-1.0.6/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      346 2023-04-01 09:20:46.000000 mkdoxy-1.0.6/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      278 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      411 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      152 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      333 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      424 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      280 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      649 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1624 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4248 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      266 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      339 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)       34 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      157 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/pages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      384 2023-01-24 19:46:00.000000 mkdoxy-1.0.6/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     2665 2023-01-25 07:25:08.000000 mkdoxy-1.0.6/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     7369 2023-01-25 07:25:08.000000 mkdoxy-1.0.6/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-04-01 12:27:31.413732 mkdoxy-1.0.6/mkdoxy.egg-info/
--rwxr-xr-x   0 kuba       (501) staff       (20)     9049 2023-04-01 12:27:31.000000 mkdoxy-1.0.6/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)      976 2023-04-01 12:27:31.000000 mkdoxy-1.0.6/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-04-01 12:27:31.000000 mkdoxy-1.0.6/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-04-01 12:27:31.000000 mkdoxy-1.0.6/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       49 2023-04-01 12:27:31.000000 mkdoxy-1.0.6/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-04-01 12:27:31.000000 mkdoxy-1.0.6/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       38 2023-04-01 12:27:31.417236 mkdoxy-1.0.6/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1342 2023-04-01 12:27:16.000000 mkdoxy-1.0.6/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 11:39:37.976269 mkdoxy-1.1.0/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-04-15 21:27:30.000000 mkdoxy-1.1.0/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5072 2023-06-30 11:39:37.976089 mkdoxy-1.1.0/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4344 2023-06-14 11:27:54.000000 mkdoxy-1.1.0/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 11:39:37.971078 mkdoxy-1.1.0/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-05-29 07:50:23.000000 mkdoxy-1.1.0/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-04-15 21:27:30.000000 mkdoxy-1.1.0/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      252 2023-04-15 21:27:30.000000 mkdoxy-1.1.0/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2841 2023-04-15 21:27:30.000000 mkdoxy-1.1.0/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4415 2023-06-14 12:31:16.000000 mkdoxy-1.1.0/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4241 2023-06-14 11:26:23.000000 mkdoxy-1.1.0/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-14 12:43:51.000000 mkdoxy-1.1.0/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:09:09.000000 mkdoxy-1.1.0/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-06-14 12:31:18.000000 mkdoxy-1.1.0/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    12065 2023-06-14 12:32:26.000000 mkdoxy-1.1.0/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-04-15 21:27:30.000000 mkdoxy-1.1.0/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    20867 2023-06-14 12:31:22.000000 mkdoxy-1.1.0/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7543 2023-06-30 11:12:43.000000 mkdoxy-1.1.0/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-06-14 12:31:23.000000 mkdoxy-1.1.0/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 11:39:37.975798 mkdoxy-1.1.0/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-06 13:14:28.000000 mkdoxy-1.1.0/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      351 2023-05-03 22:30:18.000000 mkdoxy-1.1.0/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-08 09:34:40.000000 mkdoxy-1.1.0/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      164 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      581 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      407 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      498 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      437 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      741 2023-05-03 22:39:48.000000 mkdoxy-1.1.0/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-05-03 22:41:26.000000 mkdoxy-1.1.0/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4480 2023-06-30 11:06:00.000000 mkdoxy-1.1.0/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      444 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      413 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:05:44.000000 mkdoxy-1.1.0/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-05-03 22:35:42.000000 mkdoxy-1.1.0/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:08:10.000000 mkdoxy-1.1.0/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-06-14 12:31:25.000000 mkdoxy-1.1.0/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 11:39:37.972175 mkdoxy-1.1.0/mkdoxy.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     5072 2023-06-30 11:39:37.000000 mkdoxy-1.1.0/mkdoxy.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     1072 2023-06-30 11:39:37.000000 mkdoxy-1.1.0/mkdoxy.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2023-06-30 11:39:37.000000 mkdoxy-1.1.0/mkdoxy.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       47 2023-06-30 11:39:37.000000 mkdoxy-1.1.0/mkdoxy.egg-info/entry_points.txt
+-rw-r--r--   0 kuba       (501) staff       (20)      107 2023-06-30 11:39:37.000000 mkdoxy-1.1.0/mkdoxy.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        7 2023-06-30 11:39:37.000000 mkdoxy-1.1.0/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2023-06-30 11:39:37.976317 mkdoxy-1.1.0/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1293 2023-06-14 12:54:06.000000 mkdoxy-1.1.0/setup.py
```

### Comparing `mkdoxy-1.0.6/LICENSE` & `mkdoxy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.0.6/mkdoxy/constants.py` & `mkdoxy-1.1.0/mkdoxy/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,17 @@
 
 	def is_dir(self) -> bool:
 		return self == Kind.DIR
 
 	def is_page(self) -> bool:
 		return self == Kind.PAGE
 
+	def is_example(self) -> bool:
+		return self == Kind.EXAMPLE
+
 	def is_language(self) -> bool:
 		LANGUAGE = [
 			Kind.FUNCTION,
 			Kind.VARIABLE,
 			Kind.NAMESPACE,
 			Kind.DEFINE,
 			Kind.CLASS,
```

### Comparing `mkdoxy-1.0.6/mkdoxy/doxygen.py` & `mkdoxy-1.1.0/mkdoxy/doxygen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+import logging
 import os
 from xml.etree import ElementTree
-from mkdoxy.node import Node
-from mkdoxy.constants import Kind, Visibility
+
+import path as path
+
 from mkdoxy.cache import Cache
+from mkdoxy.constants import Kind, Visibility
+from mkdoxy.node import Node
 from mkdoxy.xml_parser import XmlParser
-import logging
 
-log = logging.getLogger("mkdocs")
+log: logging.Logger = logging.getLogger("mkdocs")
 
 
 
 class Doxygen:
-	def __init__(self, index_path: str, parser: XmlParser, cache: Cache, debug: bool = False):
-		self.debug = debug
-		path = os.path.join(index_path, 'index.xml')
+	def __init__(self, index_path: path, parser: XmlParser, cache: Cache):
+		self.debug = parser.debug
+		path_xml = os.path.join(index_path, 'index.xml')
 		if self.debug:
-			log.info(f'Loading XML from: {path}')
-		xml = ElementTree.parse(path).getroot()
+			log.info(f'Loading XML from: {path_xml}')
+		xml = ElementTree.parse(path_xml).getroot()
 
 		self.parser = parser
 		self.cache = cache
 
 		self.root = Node('root', None, self.cache, self.parser, None)
 		self.groups = Node('root', None, self.cache, self.parser, None)
 		self.files = Node('root', None, self.cache, self.parser, None)
 		self.pages = Node('root', None, self.cache, self.parser, None)
+		self.examples = Node('root', None, self.cache, self.parser, None)
 
 		for compound in xml.findall('compound'):
 			kind = Kind.from_str(compound.get('kind'))
 			refid = compound.get('refid')
 			if kind.is_language():
 				node = Node(
 					os.path.join(index_path, f'{refid}.xml'),
@@ -65,34 +69,48 @@
 					None,
 					self.cache,
 					self.parser,
 					self.root,
 				)
 				node._visibility = Visibility.PUBLIC
 				self.pages.add_child(node)
+			if kind == Kind.EXAMPLE:
+				node = Node(
+					os.path.join(index_path, f'{refid}.xml'),
+					None,
+					self.cache,
+					self.parser,
+					self.root,
+				)
+				node._visibility = Visibility.PUBLIC
+				self.examples.add_child(node)
 
 		if self.debug:
 			log.info('Deduplicating data... (may take a minute!)')
 		for child in self.root.children.copy():
 			self._fix_duplicates(child, self.root, [])
 
 		for child in self.groups.children.copy():
 			self._fix_duplicates(child, self.groups, [Kind.GROUP])
 
 		for child in self.files.children.copy():
 			self._fix_duplicates(child, self.files, [Kind.FILE, Kind.DIR])
 
+		for child in self.examples.children.copy():
+			self._fix_duplicates(child, self.examples, [Kind.EXAMPLE])
+
 		self._fix_parents(self.files)
 
 		if self.debug:
 			log.info('Sorting...')
 		self._recursive_sort(self.root)
 		self._recursive_sort(self.groups)
 		self._recursive_sort(self.files)
 		self._recursive_sort(self.pages)
+		self._recursive_sort(self.examples)
 
 	def _fix_parents(self, node: Node):
 		if node.is_dir or node.is_root:
 			for child in node.children:
 				if child.is_file:
 					child._parent = node
 				if child.is_dir:
```

### Comparing `mkdoxy-1.0.6/mkdoxy/finder.py` & `mkdoxy-1.1.0/mkdoxy/finder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,14 @@
-import os
-import re
-import string
-import traceback
-from typing import TextIO
-from jinja2 import Template
-from jinja2.exceptions import TemplateSyntaxError, TemplateError
-from jinja2 import StrictUndefined, Undefined
-from mkdoxy.node import Node, DummyNode
-from mkdoxy.doxygen import Doxygen
 from mkdoxy.constants import Kind
+from mkdoxy.doxygen import Doxygen
 from mkdoxy.utils import recursive_find, recursive_find_with_parent
-from pprint import pprint
-
+from typing import Dict
 
 class Finder:
-	def __init__(self, doxygen: Doxygen, debug: bool = False):
+	def __init__(self, doxygen: Dict[str, Doxygen], debug: bool = False):
 		self.doxygen = doxygen
 		self.debug = debug
 
 	def _normalize(self, name: str) -> str:
 		return name.replace(" ", "")
 
 	def listToNames(self, list):
```

### Comparing `mkdoxy-1.0.6/mkdoxy/generatorAuto.py` & `mkdoxy-1.1.0/mkdoxy/generatorAuto.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,18 @@
+import logging
 import os
-import re
-import string
-import traceback
+
 from mkdocs.structure import files
-from io import StringIO
-from typing import TextIO
-from jinja2 import Template
-from jinja2.exceptions import TemplateSyntaxError, TemplateError
-from jinja2 import StrictUndefined, Undefined
-from mkdoxy.node import Node, DummyNode
-from mkdoxy.doxygen import Doxygen
+
 from mkdoxy.constants import Kind
+from mkdoxy.doxygen import Doxygen
 from mkdoxy.generatorBase import GeneratorBase
-from mkdoxy.utils import recursive_find, recursive_find_with_parent
-from pprint import *
-from pathlib import Path, PurePath
-import logging
+from mkdoxy.node import Node
 
-log = logging.getLogger("mkdocs")
+log: logging.Logger = logging.getLogger("mkdocs")
 
 ADDITIONAL_FILES = {
 	'Namespace ListNamespace List': 'namespaces.md',
 	'Namespace Members': 'namespace_members.md',
 	'Namespace Member Functions': 'namespace_member_functions.md',
 	'Namespace Member Variables': 'namespace_member_variables.md',
 	'Namespace Member Typedefs': 'namespace_member_typedefs.md',
@@ -31,230 +22,268 @@
 	'Class Members': 'class_members.md',
 	'Class Member Functions': 'class_member_functions.md',
 	'Class Member Variables': 'class_member_variables.md',
 	'Class Member Typedefs': 'class_member_typedefs.md',
 	'Class Member Enumerations': 'class_member_enums.md',
 }
 
-def generate_link(name, url) -> str:
-	return f'* [{name}]({url}' + ')\n'
+def generate_link(name, url, end="\n") -> str:
+	def normalize(name):
+		return "\\" + name if name.startswith("__") else name
+
+	return f'- [{normalize(name)}]({url}){end}'
 
 # def generate_link(name, url) -> str:
 # 	return f"\t\t- '{name}': '{url}'\n"
 
 class GeneratorAuto:
 	def __init__(self,
 	             generatorBase: GeneratorBase,
 	             tempDoxyDir: str,
 	             siteDir: str,
 	             apiPath: str,
 				 doxygen: Doxygen,
-	             useDirectoryUrls: bool,
-	             debug: bool = False):
+	             useDirectoryUrls: bool
+				 ):
 		self.generatorBase = generatorBase
 		self.tempDoxyDir = tempDoxyDir
 		self.siteDir = siteDir
 		self.apiPath = apiPath
 		self.doxygen = doxygen
 		self.useDirectoryUrls = useDirectoryUrls
 		self.fullDocFiles = []
-		self.debug = debug
-		self.outputSumm = ""
+		self.debug = generatorBase.debug
 		os.makedirs(os.path.join(self.tempDoxyDir, self.apiPath), exist_ok=True)
 
 	def save(self, path: str, output: str):
 		pathRel = os.path.join(self.apiPath, path)
 		self.fullDocFiles.append(files.File(pathRel, self.tempDoxyDir, self.siteDir, self.useDirectoryUrls))
 		with open(os.path.join(self.tempDoxyDir, pathRel), 'w', encoding='utf-8') as file:
 			file.write(output)
 
-	def fullDoc(self):
-		self.annotated(self.doxygen.root.children)
-		self.fileindex(self.doxygen.files.children)
-		self.members(self.doxygen.root.children)
-		self.members(self.doxygen.groups.children)
-		self.files(self.doxygen.files.children)
-		self.namespaces(self.doxygen.root.children)
-		self.classes(self.doxygen.root.children)
-		self.hierarchy(self.doxygen.root.children)
-		self.modules(self.doxygen.groups.children)
-		self.pages(self.doxygen.pages.children)
+	def fullDoc(self, defaultTemplateConfig: dict):
+		self.annotated(self.doxygen.root.children, defaultTemplateConfig)
+		self.fileindex(self.doxygen.files.children, defaultTemplateConfig)
+		self.members(self.doxygen.root.children, defaultTemplateConfig)
+		self.members(self.doxygen.groups.children, defaultTemplateConfig)
+		self.files(self.doxygen.files.children, defaultTemplateConfig)
+		self.namespaces(self.doxygen.root.children, defaultTemplateConfig)
+		self.classes(self.doxygen.root.children, defaultTemplateConfig)
+		self.hierarchy(self.doxygen.root.children, defaultTemplateConfig)
+		self.modules(self.doxygen.groups.children, defaultTemplateConfig)
+		self.pages(self.doxygen.pages.children, defaultTemplateConfig)
+		# self.examples(self.doxygen.examples.children) # TODO examples
 		self.relatedpages(self.doxygen.pages.children)
 		self.index(self.doxygen.root.children, [Kind.FUNCTION, Kind.VARIABLE, Kind.TYPEDEF, Kind.ENUM],
-		           [Kind.CLASS, Kind.STRUCT, Kind.INTERFACE], 'Class Members')
+		           [Kind.CLASS, Kind.STRUCT, Kind.INTERFACE], 'Class Members', defaultTemplateConfig)
 		self.index(self.doxygen.root.children, [Kind.FUNCTION], [Kind.CLASS, Kind.STRUCT, Kind.INTERFACE],
-		           'Class Member Functions')
+		           'Class Member Functions', defaultTemplateConfig)
 		self.index(self.doxygen.root.children, [Kind.VARIABLE], [Kind.CLASS, Kind.STRUCT, Kind.INTERFACE],
-		           'Class Member Variables')
+		           'Class Member Variables', defaultTemplateConfig)
 		self.index(self.doxygen.root.children, [Kind.TYPEDEF], [Kind.CLASS, Kind.STRUCT, Kind.INTERFACE],
-		           'Class Member Typedefs')
+		           'Class Member Typedefs', defaultTemplateConfig)
 		self.index(self.doxygen.root.children, [Kind.ENUM], [Kind.CLASS, Kind.STRUCT, Kind.INTERFACE],
-		           'Class Member Enums')
+		           'Class Member Enums', defaultTemplateConfig)
 		self.index(self.doxygen.root.children, [Kind.FUNCTION, Kind.VARIABLE, Kind.TYPEDEF, Kind.ENUM],
-		           [Kind.NAMESPACE], 'Namespace Members')
-		self.index(self.doxygen.root.children, [Kind.FUNCTION], [Kind.NAMESPACE], 'Namespace Member Functions')
-		self.index(self.doxygen.root.children, [Kind.VARIABLE], [Kind.NAMESPACE], 'Namespace Member Variables')
-		self.index(self.doxygen.root.children, [Kind.TYPEDEF], [Kind.NAMESPACE], 'Namespace Member Typedefs')
-		self.index(self.doxygen.root.children, [Kind.ENUM], [Kind.NAMESPACE], 'Namespace Member Enums')
-		self.index(self.doxygen.files.children, [Kind.FUNCTION], [Kind.FILE], 'Functions')
-		self.index(self.doxygen.files.children, [Kind.DEFINE], [Kind.FILE], 'Macros')
+		           [Kind.NAMESPACE], 'Namespace Members', defaultTemplateConfig)
+		self.index(self.doxygen.root.children, [Kind.FUNCTION], [Kind.NAMESPACE], 'Namespace Member Functions', defaultTemplateConfig)
+		self.index(self.doxygen.root.children, [Kind.VARIABLE], [Kind.NAMESPACE], 'Namespace Member Variables', defaultTemplateConfig)
+		self.index(self.doxygen.root.children, [Kind.TYPEDEF], [Kind.NAMESPACE], 'Namespace Member Typedefs', defaultTemplateConfig)
+		self.index(self.doxygen.root.children, [Kind.ENUM], [Kind.NAMESPACE], 'Namespace Member Enums', defaultTemplateConfig)
+		self.index(self.doxygen.files.children, [Kind.FUNCTION], [Kind.FILE], 'Functions', defaultTemplateConfig)
+		self.index(self.doxygen.files.children, [Kind.DEFINE], [Kind.FILE], 'Macros', defaultTemplateConfig)
 		self.index(self.doxygen.files.children, [Kind.VARIABLE, Kind.UNION, Kind.TYPEDEF, Kind.ENUM], [Kind.FILE],
-		           'Variables')
+		           'Variables', defaultTemplateConfig)
 
-	def annotated(self, nodes: [Node]):
+	def annotated(self, nodes: [Node], config: dict = None):
 		path = 'annotated.md'
-		output = self.generatorBase.annotated(nodes)
+		output = self.generatorBase.annotated(nodes, config)
 		self.save(path, output)
 
-	def programlisting(self, node: [Node]):
+	def programlisting(self, node: [Node], config: dict = None):
 		path = f'{node.refid}_source.md'
 
-		output = self.generatorBase.programlisting(node)
+		output = self.generatorBase.programlisting(node, config)
 		self.save(path, output)
 
-	def fileindex(self, nodes: [Node]):
+	def fileindex(self, nodes: [Node], config: dict = None):
 		path = 'files.md'
 
-		output = self.generatorBase.fileindex(nodes)
+		output = self.generatorBase.fileindex(nodes, config)
 		self.save(path, output)
 
-	def namespaces(self, nodes: [Node]):
+	def namespaces(self, nodes: [Node], config: dict = None):
 		path = 'namespaces.md'
 
-		output = self.generatorBase.namespaces(nodes)
+		output = self.generatorBase.namespaces(nodes, config)
 		self.save(path, output)
 
-	def page(self, node: Node):
+	def page(self, node: Node, config: dict = None):
 		path = f'{node.name}.md'
 
-		output = self.generatorBase.page(node)
+		output = self.generatorBase.page(node, config)
 		self.save(path, output)
 
-	def pages(self, nodes: [Node]):
+	def pages(self, nodes: [Node], config: dict = None):
 		for node in nodes:
-			self.page(node)
+			self.page(node, config)
 
-	def relatedpages(self, nodes: [Node]):
+	def relatedpages(self, nodes: [Node], config: dict = None):
 		path = 'pages.md'
 
-		output = self.generatorBase.annotated(nodes)
+		output = self.generatorBase.relatedpages(nodes)
+		self.save(path, output)
+
+	def example(self, node: Node, config: dict = None):
+		path = f'{node.refid}.md'
+
+		output = self.generatorBase.example(node, config)
 		self.save(path, output)
 
-	def classes(self, nodes: [Node]):
+	def examples(self, nodes: [Node], config: dict = None):
+		for node in nodes:
+			if node.is_example:
+				if node.has_programlisting:
+					print(f'Generating example {node.name}...')
+				self.example(node, config)
+
+		path = 'examples.md'
+
+		output = self.generatorBase.examples(nodes, config)
+		self.save(path, output)
+
+	def classes(self, nodes: [Node], config: dict = None):
 		path = 'classes.md'
 
-		output = self.generatorBase.classes(nodes)
+		output = self.generatorBase.classes(nodes, config)
 		self.save(path, output)
 
-	def modules(self, nodes: [Node]):
+	def modules(self, nodes: [Node], config: dict = None):
 		path = 'modules.md'
 
-		output = self.generatorBase.modules(nodes)
+		output = self.generatorBase.modules(nodes, config)
 		self.save(path, output)
 
-	def hierarchy(self, nodes: [Node]):
+	def hierarchy(self, nodes: [Node], config: dict = None):
 		path = 'hierarchy.md'
 
-		output = self.generatorBase.hierarchy(nodes)
+		output = self.generatorBase.hierarchy(nodes, config)
 		self.save(path, output)
 
-	def member(self, node: Node):
+	def member(self, node: Node, config: dict = None):
 		path = node.filename
 
-		output = self.generatorBase.member(node)
+		output = self.generatorBase.member(node, config)
 		self.save(path, output)
 
 		if node.is_language or node.is_group or node.is_file or node.is_dir:
-			self.members(node.children)
+			self.members(node.children, config)
 
-	def file(self, node: Node):
+	def file(self, node: Node, config: dict = None):
 		path = node.filename
 
-		output = self.generatorBase.file(node)
+		output = self.generatorBase.file(node, config)
 		self.save(path, output)
 
 		if node.is_file and node.has_programlisting:
-			self.programlisting(node)
+			self.programlisting(node, config)
 
 		if node.is_file or node.is_dir:
-			self.files(node.children)
+			self.files(node.children, config)
 
-	def members(self, nodes: [Node]):
+	def members(self, nodes: [Node], config: dict = None):
 		for node in nodes:
 			if node.is_parent or node.is_group or node.is_file or node.is_dir:
-				self.member(node)
+				self.member(node, config)
 
-	def files(self, nodes: [Node]):
+	def files(self, nodes: [Node], config: dict = None):
 		for node in nodes:
 			if node.is_file or node.is_dir:
-				self.file(node)
+				self.file(node, config)
 
-	def index(self, nodes: [Node], kind_filters: Kind, kind_parents: [Kind], title: str):
+	def index(self, nodes: [Node], kind_filters: Kind, kind_parents: [Kind], title: str, config: dict = None):
 		path = title.lower().replace(' ', '_') + '.md'
 
-		output = self.generatorBase.index(nodes, kind_filters, kind_parents, title)
+		output = self.generatorBase.index(nodes, kind_filters, kind_parents, title, config)
 		self.save(path, output)
 
-	def _generate_recursive(self, node: Node, level: int):
+	def _generate_recursive(self, output_summary: str, node: Node, level: int):
 		if node.kind.is_parent():
-			self.outputSumm += str(
+			output_summary += str(
 				' ' * level
 				+ generate_link(f'{node.kind.value} {node.name}', f'{node.refid}.md')
 			)
 			for child in node.children:
-				self._generate_recursive(child, level + 2)
+				self._generate_recursive(output_summary, child, level + 2)
 
-	def _generate_recursive_files(self, node: Node, level: int):
+	def _generate_recursive_files(self, output_summary: str, node: Node, level: int, config: dict = None):
+		if config is None:
+			config = []
 		if node.kind.is_file() or node.kind.is_dir():
-			self.outputSumm += str(
-				' ' * level + generate_link(node.name, f'{node.refid}.md')
+			output_summary += str(
+				' ' * int(level +2 ) +generate_link(node.name, f'{node.refid}.md', end='')
 			)
+
 			if node.kind.is_file():
-				self.outputSumm += str(
-					' ' * level
-					+ generate_link(f'{node.name} source', f'{node.refid}_source.md')
-				)
+				output_summary += f" [[source code]]({node.refid}_source.md) \n"
+			else:
+				output_summary += "\n"
+
 			for child in node.children:
-				self._generate_recursive_files(child, level + 2)
+				self._generate_recursive_files(output_summary, child, level + 2, config)
 
-	def _generate_recursive_groups(self, node: Node, level: int):
+	def _generate_recursive_examples(self, output_summary: str, node: Node, level: int):
+		if node.kind.is_example():
+			output_summary += str(
+				' ' * level + generate_link(node.name, f'{node.refid}.md')
+			)
+			for child in node.children:
+				self._generate_recursive_examples(output_summary, child, level + 2)
+
+	def _generate_recursive_groups(self, output_summary: str, node: Node, level: int):
 		if node.kind.is_group():
-			self.outputSumm += str(
+			output_summary += str(
 				' ' * level + generate_link(node.title, f'{node.refid}.md')
 			)
 			for child in node.children:
-				self._generate_recursive_groups(child, level + 2)
+				self._generate_recursive_groups(output_summary, child, level + 2)
 
-	def _generate_recursive_pages(self, node: Node, level: int):
+	def _generate_recursive_pages(self, output_summary: str, node: Node, level: int):
 		if node.kind.is_page():
-			self.outputSumm += str(
+			output_summary += str(
 				' ' * level + generate_link(node.title, f'{node.refid}.md')
 			)
 			for child in node.children:
-				self._generate_recursive_pages(child, level + 2)
+				self._generate_recursive_pages(output_summary, child, level + 2)
 
-	def summary(self):
+	def summary(self, defaultTemplateConfig: dict):
 		offset = 0
-		self.outputSumm += str(' ' * (offset + 2) + generate_link('Related Pages',  'pages.md'))
+		output_summary = "" + str(
+			' ' * (offset + 2) + generate_link('Related Pages', 'pages.md')
+		)
 		for node in self.doxygen.pages.children:
-			self._generate_recursive_pages(node, offset + 4)
+			self._generate_recursive_pages(output_summary, node, offset + 4)
 
-		self.outputSumm += str(' ' * (offset + 2) + generate_link('Modules', 'modules.md'))
+		output_summary += str(' ' * (offset + 2) + generate_link('Modules', 'modules.md'))
 		for node in self.doxygen.groups.children:
-			self._generate_recursive_groups(node, offset + 4)
+			self._generate_recursive_groups(output_summary, node, offset + 4)
 
-		self.outputSumm += str(' ' * (offset + 2) + generate_link('Class List', 'annotated.md'))
+		output_summary += str(' ' * (offset + 2) + generate_link('Class List', 'annotated.md'))
 		for node in self.doxygen.root.children:
-			self._generate_recursive(node, offset + 4)
+			self._generate_recursive(output_summary, node, offset + 4)
 
 		for key, val in ADDITIONAL_FILES.items():
-			self.outputSumm += str(' ' * (offset + 2) + generate_link(key, val))
+			output_summary += str(' ' * (offset + 2) + generate_link(key, val))
 
-		self.outputSumm += str(' ' * (offset + 2) + generate_link('Files', 'files.md'))
+		output_summary += str(' ' * (offset + 2) + generate_link('Files', 'files.md', end='\n'))
 		for node in self.doxygen.files.children:
-			self._generate_recursive_files(node, offset + 4)
+			self._generate_recursive_files(output_summary, node, offset + 4, defaultTemplateConfig)
+
+		# output_summary += str(' ' * (offset + 2) + generate_link('Examples', 'examples.md'))
+		# for node in self.doxygen.examples.children:
+		# 	self._generate_recursive_examples(node, offset + 4)
 
-		self.outputSumm += str(' ' * (offset + 2) + generate_link('File Variables', 'variables.md'))
-		self.outputSumm += str(' ' * (offset + 2) + generate_link('File Functions', 'functions.md'))
-		self.outputSumm += str(' ' * (offset + 2) + generate_link('File Macros', 'macros.md'))
+		output_summary += str(' ' * (offset + 2) + generate_link('File Variables', 'variables.md'))
+		output_summary += str(' ' * (offset + 2) + generate_link('File Functions', 'functions.md'))
+		output_summary += str(' ' * (offset + 2) + generate_link('File Macros', 'macros.md'))
 
-		self.save("links.md", self.outputSumm)
+		self.save("links.md", output_summary)
```

### Comparing `mkdoxy-1.0.6/mkdoxy/markdown.py` & `mkdoxy-1.1.0/mkdoxy/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.0.6/mkdoxy/node.py` & `mkdoxy-1.1.0/mkdoxy/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+import logging
 import os
-import re
-import traceback
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element as Element
-from mkdoxy.constants import Kind, Visibility, OVERLOAD_OPERATORS
+
 from mkdoxy.cache import Cache
-from mkdoxy.xml_parser import XmlParser
+from mkdoxy.constants import Kind, Visibility, OVERLOAD_OPERATORS
 from mkdoxy.markdown import escape
-from mkdoxy.utils import split_safe
 from mkdoxy.property import Property
-import logging
+from mkdoxy.utils import split_safe
+from mkdoxy.xml_parser import XmlParser
 
-log = logging.getLogger("mkdocs")
+log: logging.Logger = logging.getLogger("mkdocs")
 
 
 class Node:
 	def __init__(self, xml_file: str, xml: Element, cache: Cache, parser: XmlParser, parent: 'Node', refid: str = None, debug: bool = False):
 		self._children: ['Node'] = []
 		self._cache: Cache = cache
 		self._parser: XmlParser = parser
@@ -141,15 +140,15 @@
 		for innerfile in self._xml.findall('innerfile'):
 			refid = innerfile.get('refid')
 			if self._kind == Kind.DIR:
 				try:
 					child = self._cache.get(refid)
 					self.add_child(child)
 					continue
-				except:
+				except Exception:
 					pass
 
 			child = Node(
 				os.path.join(self._dirname, f'{refid}.xml'),
 				None,
 				self._cache,
 				self._parser,
@@ -161,15 +160,15 @@
 		for innerdir in self._xml.findall('innerdir'):
 			refid = innerdir.get('refid')
 			if self._kind == Kind.DIR:
 				try:
 					child = self._cache.get(refid)
 					self.add_child(child)
 					continue
-				except:
+				except Exception:
 					pass
 
 			child = Node(
 				os.path.join(self._dirname, f'{refid}.xml'),
 				None,
 				self._cache,
 				self._parser,
@@ -182,15 +181,15 @@
 			refid = innernamespace.get('refid')
 
 			if self._kind in [Kind.GROUP, Kind.DIR, Kind.FILE]:
 				try:
 					child = self._cache.get(refid)
 					self.add_child(child)
 					continue
-				except:
+				except Exception:
 					pass
 
 			child = Node(
 				os.path.join(self._dirname, f'{refid}.xml'),
 				None,
 				self._cache,
 				self._parser,
@@ -210,14 +209,28 @@
 							self.add_child(child)
 							continue
 						except:
 							pass
 					child = Node(None, memberdef, self._cache, self._parser, self)
 					self.add_child(child)
 
+		# for detaileddescription in self._xml.findall('detaileddescription'):
+		# 	for para in detaileddescription.findall('para'):
+		# 		for programlisting in para.findall('programlisting'):
+		# 			pass
+
+
+
+			# # kind = Kind.from_str(memberdef.get('kind'))
+			# # 	if kind.is_language():
+			# if self._kind in [Kind.EXAMPLE]:
+			# 	log.info(f'programlisting: {para.text}')
+			# if para.find('programlisting') is not None:
+			# 	self._programlisting = Property.Programlisting(para, self._parser, self._kind)
+
 	def _check_attrs(self):
 		prot = self._xml.get('prot')
 		self._visibility = Visibility(prot) if prot is not None else Visibility.PUBLIC
 
 		static = self._xml.get('static')
 		self._static = static == 'yes'
 
@@ -367,14 +380,18 @@
 		return self._kind.is_dir()
 
 	@property
 	def is_page(self) -> bool:
 		return self._kind.is_page()
 
 	@property
+	def is_example(self) -> bool:
+		return self._kind.is_example()
+
+	@property
 	def name(self) -> str:
 		return self._name
 
 	@property
 	def name_params(self) -> str:
 		name = self._name
 		type = self._type.plain()
@@ -714,14 +731,22 @@
 		return self._location.has()
 
 	@property
 	def location(self) -> str:
 		return self._location.plain()
 
 	@property
+	def location_bodystart(self) -> int:
+		return self._location.bodystart()
+
+	@property
+	def location_bodyend(self) -> int:
+		return self._location.bodyend()
+
+	@property
 	def has_params(self) -> bool:
 		return self._params.has()
 
 	@property
 	def params(self) -> str:
 		if self._params.has():
 			return f'({self._params.md()})'
@@ -783,14 +808,29 @@
 		return True
 
 	@property
 	def reimplements(self) -> 'Node':
 		reimp = self._xml.find('reimplements')
 		return self._cache.get(reimp.get('refid')) if reimp is not None else None
 
+	@property
+	def print_node_recursive(self) -> str:
+		# code_block = f'```md\n{self._print_node_recursive_md(self._xml, 0)}```'
+		# return code_block
+		return self._print_node_recursive_md(self._xml, 0)
+
+	def _print_node_recursive_md(self, node: Element, depth: int) -> str:
+		# print as Markdown code block
+		indent = "	" * depth
+		ret = f'{indent} * {node.tag} {node.attrib} -> Text: {node.text}\n'
+		for child in node.findall('*'):
+			ret += self._print_node_recursive_md(child, depth + 1)
+
+		return ret
+
 
 class DummyNode:
 	def __init__(self, name_long: str, derived_classes: [Node], kind: Kind):
 		self.name_long = name_long
 		self.derived_classes = derived_classes
 		self.kind = kind
```

### Comparing `mkdoxy-1.0.6/mkdoxy/plugin.py` & `mkdoxy-1.1.0/mkdoxy/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,169 +1,195 @@
-import sys
-from os import path, makedirs
+"""@package mkdoxy.plugin
+MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
+
+MkDoxy is a MkDocs plugin for generating documentation from Doxygen XML files.
+"""
+
+import logging
 from pathlib import Path, PurePath
-from mkdocs import utils as mkdocs_utils
-from mkdocs.plugins import BasePlugin
+
+from mkdocs import exceptions
 from mkdocs.config import base, config_options, Config
+from mkdocs.plugins import BasePlugin
 from mkdocs.structure import files, pages
-from mkdocs.commands import serve
-from mkdocs import exceptions
 
-from mkdoxy.doxyrun import DoxygenRun
+from mkdoxy.cache import Cache
 from mkdoxy.doxygen import Doxygen
-from mkdoxy.generatorBase import GeneratorBase
+from mkdoxy.doxyrun import DoxygenRun
 from mkdoxy.generatorAuto import GeneratorAuto
-from mkdoxy.xml_parser import XmlParser
-from mkdoxy.cache import Cache
-from mkdoxy.constants import Kind
+from mkdoxy.generatorBase import GeneratorBase
 from mkdoxy.generatorSnippets import GeneratorSnippets
-from mkdoxy.finder import Finder
-
-from pprint import *
-import logging
+from mkdoxy.utils import check_enabled_markdown_extensions
+from mkdoxy.xml_parser import XmlParser
 
-log = logging.getLogger("mkdocs")
-pluginName = "MkDoxy"
+log: logging.Logger = logging.getLogger("mkdocs")
+pluginName: str = "MkDoxy"
 
 
 class MkDoxy(BasePlugin):
-	"""
-	plugins:
-	- search
-	- mkdoxy
+	"""! MkDocs plugin for generating documentation from Doxygen XML files.
 	"""
 
+	# Config options for the plugin
 	config_scheme = (
 		('projects', config_options.Type(dict, default={})),
 		('full-doc', config_options.Type(bool, default=True)),
 		('debug', config_options.Type(bool, default=False)),
 		('ignore-errors', config_options.Type(bool, default=False)),
 		('save-api', config_options.Type(str, default="")),
 		("enabled", config_options.Type(bool, default=True)),
 	)
 
+	# Config options for each project
 	config_project = (
 		('src-dirs', config_options.Type(str)),
 		('full-doc', config_options.Type(bool, default=True)),
 		('debug', config_options.Type(bool, default=False)),
 		# ('ignore-errors', config_options.Type(bool, default=False)),
 		('doxy-cfg', config_options.Type(dict, default={}, required=False)),
 		('template-dir', config_options.Type(str, default="", required=False)),
 	)
 
-	def is_enabled(self):
+	def is_enabled(self) -> bool:
+		"""! Checks if the plugin is enabled
+		@details
+		@return: (bool) True if the plugin is enabled.
+		"""
 		return self.config.get("enabled")
 
-	def on_files(self, files: files.Files, config):
-
+	def on_files(self, files: files.Files, config: base.Config) -> files.Files:
+		"""! Called after files have been gathered by MkDocs.
+		@details
+
+		@param files: (Files) The files gathered by MkDocs.
+		@param config: (Config) The global configuration object.
+		@return: (Files) The files gathered by MkDocs.
+		"""
 		if not self.is_enabled():
 			return files
 		def checkConfig(config_project, proData, strict: bool):
 			cfg = Config(config_project, '')
 			cfg.load_dict(proData)
 			errors, warnings = cfg.validate()
 			for config_name, warning in warnings:
-				log.warning(f"  -> Config value: '{config_name}' in project '{projectName}'. Warning: {warning}")
+				log.warning(f"  -> Config value: '{config_name}' in project '{project_name}'. Warning: {warning}")
 			for config_name, error in errors:
-				log.error(f"  -> Config value: '{config_name}' in project '{projectName}'. Error: {error}")
+				log.error(f"  -> Config value: '{config_name}' in project '{project_name}'. Error: {error}")
 
 			if len(errors) > 0:
 				raise exceptions.Abort(f"Aborted with {len(errors)} Configuration Errors!")
 			elif strict and len(warnings) > 0:
 				raise exceptions.Abort(f"Aborted with {len(warnings)} Configuration Warnings in 'strict' mode!")
 
 		def tempDir(siteDir: str, tempDir:str, projectName: str) ->str:
 			tempDoxyDir = PurePath.joinpath(Path(siteDir), Path(tempDir), Path(projectName))
 			tempDoxyDir.mkdir(parents=True, exist_ok=True)
 			return str(tempDoxyDir)
 
 		self.doxygen = {}
 		self.generatorBase = {}
-		self.projects = self.config["projects"]
+		self.projects_config:dict[str, dict[str, any]] = self.config["projects"]
+		self.debug = self.config.get('debug', False)
+
+		# generate automatic documentation and append files in the list of files to be processed by mkdocs
+		self.defaultTemplateConfig: dict = {
+			"indent_level": 0,
+		}
 
 		log.info(f"Start plugin {pluginName}")
 
-		for projectName in self.projects:
-			self.proData = self.projects.get(projectName)
-			log.info(f"-> Start project '{projectName}'")
+
+		for project_name, project_data in self.projects_config.items():
+			log.info(f"-> Start project '{project_name}'")
 
 			# Check project config -> raise exceptions
-			checkConfig(self.config_project, self.proData, config['strict'])
+			checkConfig(self.config_project, project_data, config['strict'])
 
 			if self.config.get("save-api"):
-				tempDirApi = tempDir("", self.config.get("save-api"), projectName)
+				tempDirApi = tempDir("", self.config.get("save-api"), project_name)
 			else:
-				tempDirApi = tempDir(config['site_dir'], "assets/.doxy/", projectName)
+				tempDirApi = tempDir(config['site_dir'], "assets/.doxy/", project_name)
 
 			# Check scr changes -> run Doxygen
-			doxygenRun = DoxygenRun(self.proData.get('src-dirs'), tempDirApi, self.proData.get('doxy-cfg', {}))
+			doxygenRun = DoxygenRun(project_data.get('src-dirs'), tempDirApi, project_data.get('doxy-cfg', {}))
 			if doxygenRun.checkAndRun():
 				log.info("  -> generating Doxygen filese")
 			else:
 				log.info("  -> skip generating Doxygen files (nothing changes)")
 
-			self.debug = self.config.get('debug', False)
-
-			# Parse XML to bacic structure
+			# Parse XML to basic structure
 			cache = Cache()
 			parser = XmlParser(cache=cache, debug=self.debug)
 
-			# Parse bacic structure to recursive Nodes
-			self.doxygen[projectName] = Doxygen(doxygenRun.path, parser=parser, cache=cache, debug=self.debug)
+			# Parse basic structure to recursive Nodes
+			self.doxygen[project_name] = Doxygen(doxygenRun.getOutputFolder(), parser=parser, cache=cache)
 
 			# Print parsed files
 			if self.debug:
-				self.doxygen[projectName].printStructure()
+				self.doxygen[project_name].printStructure()
 
 			# Prepare generator for future use (GeneratorAuto, SnippetGenerator)
-			self.generatorBase[projectName] = GeneratorBase(self.proData.get('template-dir',""), ignore_errors=self.config["ignore-errors"], debug=self.debug)
+			self.generatorBase[project_name] = GeneratorBase(project_data.get('template-dir',""), ignore_errors=self.config["ignore-errors"], debug=self.debug)
 
-			if self.config["full-doc"] and self.proData.get("full-doc", True):
+			if self.config["full-doc"] and project_data.get("full-doc", True):
 				generatorAuto = GeneratorAuto(
-					generatorBase=self.generatorBase[projectName],
+					generatorBase=self.generatorBase[project_name],
 					tempDoxyDir=tempDirApi,
 					siteDir=config['site_dir'],
-					apiPath=projectName,
-					doxygen=self.doxygen[projectName],
+					apiPath=project_name,
+					doxygen=self.doxygen[project_name],
 					useDirectoryUrls=config['use_directory_urls'],
-					debug=self.debug
 				)
 
-				# generate automatic documentation and append files into files
-				generatorAuto.fullDoc()
+				project_config = self.defaultTemplateConfig.copy()
+				project_config.update(project_data)
+				generatorAuto.fullDoc(project_config)
 
-				generatorAuto.summary()
+				generatorAuto.summary(project_config)
 
 				for file in generatorAuto.fullDocFiles:
 					files.append(file)
 		return files
 
 	def on_page_markdown(
 			self,
 			markdown: str,
 			page: pages.Page,
 			config: base.Config,
 			files: files.Files,
 	) -> str:
+		"""! Generate snippets and append them to the markdown.
+		@details
+
+		@param markdown (str): The markdown.
+		@param page (Page): The MkDocs page.
+		@param config (Config): The MkDocs config.
+		@param files (Files): The MkDocs files.
+		@return: (str) The markdown.
+		"""
 		if not self.is_enabled():
 			return markdown
 
+		# update default template config with page meta
+		page_config = self.defaultTemplateConfig.copy()
+		page_config.update(page.meta)
+
 		generatorSnippets = GeneratorSnippets(
 			markdown=markdown,
 			generatorBase=self.generatorBase,
 			doxygen=self.doxygen,
+			projects=self.projects_config,
 			useDirectoryUrls=config['use_directory_urls'],
 			page = page,
-		debug=self.debug
+			config = page_config,
+			debug=self.debug
 		)
 
 		return generatorSnippets.generate()
 
-# def on_pre_build(self, config):
-
 # def on_serve(self, server):
 #     return server
 #
 # def on_files(self, files: files.Files, config):
 #     return files
 
 # def on_nav(self, nav, config, files):
@@ -171,14 +197,16 @@
 #
 # def on_env(self, env, config, files):
 #     return env
 #
 # def on_config(self, config):
 #     return config
 #
+# def on_pre_build(self, config: base.Config):
+#     return
 # def on_post_build(self, config):
 #     return
 #
 # def on_pre_template(self, template, template_name, config):
 #     return template
 #
 # def on_template_context(self, context, template_name, config):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkdoxy-1.0.6/mkdoxy/property.py` & `mkdoxy-1.1.0/mkdoxy/property.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from xml.etree.ElementTree import Element as Element
-from mkdoxy.xml_parser import XmlParser
+
 from mkdoxy.constants import Kind
 from mkdoxy.markdown import escape
+from mkdoxy.xml_parser import XmlParser
 
 
 class Property:
 	class Details:
 		def __init__(self, xml: Element, parser: XmlParser, kind: Kind):
 			self.xml = xml
 			self.parser = parser
@@ -106,17 +107,34 @@
 		def md(self, plain: bool = False) -> str:
 			return self.plain()
 
 		def plain(self) -> str:
 			loc = self.xml.find('location')
 			return loc.get('file') if loc is not None else ''
 
+		def line(self) -> int:
+			loc = self.xml.find('location')
+			return int(loc.get('line')) if loc is not None else 0
+
+		def column(self) -> int:
+			loc = self.xml.find('location')
+			return int(loc.get('column')) if loc is not None else 0
+
+		def bodystart(self) -> int:
+			loc = self.xml.find('location')
+			return int(loc.get('bodystart')) if loc is not None else 0
+
+		def bodyend(self) -> int:
+			loc = self.xml.find('location')
+			return int(loc.get('bodyend')) if loc is not None else 0
+
 		def has(self) -> bool:
 			return self.xml.find('location') is not None
 
+
 	class Params:
 		def __init__(self, xml: Element, parser: XmlParser, kind: Kind):
 			self.xml = xml
 			self.parser = parser
 			self.kind = kind
 
 		def md(self, plain: bool = False) -> str:
```

### Comparing `mkdoxy-1.0.6/mkdoxy/templates/memDef.jinja2` & `mkdoxy-1.1.0/mkdoxy/templates/memDef.jinja2`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 ---
 brief: True
 details: True
 implements: True
+url_source: True
 ---
+
 {# This template is used inside of member.py #}
+{% filter indent(config.get('indent_level', 0), True) %}
 
 ### {{node.kind.value}} {{node.name_long if node.is_group else node.name_short}} {{node.overload_suffix}}
 
 {% if configMemDef.get('brief') -%}
 {% if node.has_brief -%}
 {{node.brief + "\n"}}
 {%- endif -%}
@@ -25,7 +28,9 @@
 {%- endif -%}
 
 {% if configMemDef.get('implements') -%}
 {% if node.reimplements %}
 Implements [*{{node.reimplements.name_long}}*]({{node.reimplements.url}})
 {% endif %}
 {%- endif -%}
+
+{% endfilter %}
```

### Comparing `mkdoxy-1.0.6/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.1.0/mkdoxy/templates/memTab.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% filter indent(config.get('indent_level', 0), True) %}
 {# This template is used inside of member.py #}
 
 {%- if node.has(visibility, kinds, static) -%}
 {%- if parent is none -%}
 ## {{title}}
 {%- else -%}
 ## {{title}} inherited from {{node.name}}
@@ -26,7 +27,9 @@
 | {{member.prefix}} {{member.type}} | [**{{member.name_long if node.is_group else member.name_short}}**](#{{member.anchor}}) {{member.params}} {{member.suffix}}<br>{{member.brief}} |
 {%- else -%}
 | {{member.prefix}} {{member.type}} | [**{{member.name_long if node.is_group else member.name_short}}**]({{member.url}}) {{member.params}} {{member.suffix}}<br>{{member.brief}} |
 {%- endif %}
 {% endfor -%}
 
 {%- endif -%}
+
+{% endfilter %}
```

### Comparing `mkdoxy-1.0.6/mkdoxy/templates/member.jinja2` & `mkdoxy-1.1.0/mkdoxy/templates/member.jinja2`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 ---
 brief: True
 details: True
 implements: True
 ---
+{% filter indent(config.get('indent_level', 0), True) %}
 
 # {{node.kind.value|title}} {{node.name_long}}
 {% if node.has_templateparams %}
 **template &lt;{{node.templateparams}}&gt;**
 {% endif %}
 
 
 [**{{node.base_name}}**]({{node.base_url}})
 {%- for parent in node.parents -%}
 {{'**>**'|indent(1, true)}} [**{{parent.name_long if node.is_group else parent.name_short}}**]({{parent.url}})
 {%- endfor %}
 
 {% if node.is_file and node.has_programlisting -%}
-[Go to the source code of this file.]({{node.url_source}})
+[Go to the source code of this file]({{node.url_source}})
 {%- endif %}
 
 {{node.brief}}
 {%- if node.has_details -%}
 [More...](#detailed-description)
 {%- endif %}
 
@@ -42,66 +43,68 @@
 Inherited by the following classes:
 {%- for derived in node.derived_classes -%}
 {%- if derived is string %} {{derived}}{%- else %} [{{derived.name_long}}]({{derived.url}}){%- endif -%}
 {{ ', ' if not loop.last else '' }}
 {%- endfor -%}
 {%- endif %}
 
-{{ templateMemTab.render({'node': node, 'parent': None, 'title': 'Files', 'visibility': 'public', 'kinds': ['file'], 'static': False}) }}
-{{ templateMemTab.render({'node': node, 'parent': None, 'title': 'Directories', 'visibility': 'public', 'kinds': ['dir'], 'static': False}) }}
-{{ templateMemTab.render({'node': node, 'parent': None, 'title': 'Modules', 'visibility': 'public', 'kinds': ['group'], 'static': False}) }}
-{{ templateMemTab.render({'node': node, 'parent': None, 'title': 'Namespaces', 'visibility': 'public', 'kinds': ['namespace'], 'static': False}) }}
-{{ templateMemTab.render({'node': node, 'parent': None, 'title': 'Classes', 'visibility': 'public', 'kinds': ['class', 'struct', 'interface'], 'static': False}) }}
+{{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Files', 'visibility': 'public', 'kinds': ['file'], 'static': False}) }}
+{{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Directories', 'visibility': 'public', 'kinds': ['dir'], 'static': False}) }}
+{{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Modules', 'visibility': 'public', 'kinds': ['group'], 'static': False}) }}
+{{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Namespaces', 'visibility': 'public', 'kinds': ['namespace'], 'static': False}) }}
+{{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Classes', 'visibility': 'public', 'kinds': ['class', 'struct', 'interface'], 'static': False}) }}
 
 {%- for visibility in ['public', 'protected'] -%}
 {%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['functions', ['function']]] -%}
 {%- for static in [['', False], ['static ', True]] %}
-{{ templateMemTab.render({'node': node, 'parent': None, 'title': visibility|title + ' ' + static[0]|title + query[0]|title, 'visibility': visibility, 'kinds': query[1], 'static': static[1]}) }}
+{{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': visibility|title + ' ' + static[0]|title + query[0]|title, 'visibility': visibility, 'kinds': query[1], 'static': static[1]}) }}
 {%- for child in node.base_classes recursive -%}{%- if child is not string %}
-{{ templateMemTab.render({'node': child, 'parent': node, 'title': visibility|title + ' ' + static[0]|title + query[0]|title, 'visibility': visibility, 'kinds': query[1], 'static': static[1]}) }}
+{{ templateMemTab.render({'config': {}, 'node': child, 'parent': node, 'title': visibility|title + ' ' + static[0]|title + query[0]|title, 'visibility': visibility, 'kinds': query[1], 'static': static[1]}) }}
 {{- loop(child.base_classes)}}
 {%- endif -%}{%- endfor -%}
 {%- endfor -%}
 {%- endfor -%}
 {%- endfor -%}
 
-{{ templateMemTab.render({'node': node, 'parent': None, 'title': 'Macros', 'visibility': 'public', 'kinds': ['define'], 'static': False}) }}
+{{ templateMemTab.render({'config': {"":""}, 'node': node, 'parent': None, 'title': 'Macros', 'visibility': 'public', 'kinds': ['define'], 'static': False}) }}
 
 {%- if node.has_details %}
 # Detailed Description
 
 {{node.details}}
 {%- endif %}
 
 {%- for visibility in ['public', 'protected'] -%}
 {%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['functions', ['function']]] -%}
 {%- for static in [['', False], ['static ', True]] %}
 {%- if node.has(visibility, query[1], static[1]) %}
 ## {{visibility|title}} {{static[0]|title}}{{query[0]|title}} Documentation
 {% for member in node.query(visibility, query[1], static[1]) -%}
-{{ templateMemDef.render({'node': member, 'configMemDef': configMemDef}) }}
+{{ templateMemDef.render({'config': {}, 'node': member, 'configMemDef': configMemDef}) }}
 {%- endfor %}
 {%- endif -%}
 {%- endfor -%}
 {%- endfor -%}
 {%- endfor -%}
 
 {%- if node.has('public', ['define'], False) %}
 ## Macro Definition Documentation
 
 {% for member in node.query('public', ['define'], False) -%}
-{{ templateMemDef.render({'node': member, 'configMemDef': configMemDef}) }}
+{{ templateMemDef.render({'config': {}, 'node': member, 'configMemDef': configMemDef}) }}
 {%- endfor -%}
 {%- endif %}
 
 {%- if node.has('public', ['friend'], False) -%}
 ## Friends Documentation
 
 {% for member in node.query('public', ['friend'], False) -%}
-{{ templateMemDef.render({'node': member, 'configMemDef': configMemDef}) }}
+{{ templateMemDef.render({'config': {}, 'node': member, 'configMemDef': configMemDef}) }}
 {%- endfor %}
 {%- endif %}
 
 ------------------------------
 {% if node.has_location -%}
 The documentation for this class was generated from the following file `{{node.location}}`
-{%- endif %}
+{%- endif %}
+
+{% endfilter %}
```

### Comparing `mkdoxy-1.0.6/mkdoxy/xml_parser.py` & `mkdoxy-1.1.0/mkdoxy/xml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from xml.etree.ElementTree import Element as Element
-from mkdoxy.markdown import Md, MdRenderer, MdParagraph, MdTable, Code, MdTableRow, MdCodeBlock, MdTableCell, \
-	MdHeader, MdImage, MdList, MdBlockQuote, MdLink, MdBold, MdItalic, MdHint, Text, Br
+
 from mkdoxy.cache import Cache
+from mkdoxy.markdown import Md, MdRenderer, MdParagraph, MdTable, Code, MdTableRow, MdCodeBlock, MdTableCell, \
+    MdHeader, MdImage, MdList, MdBlockQuote, MdLink, MdBold, MdItalic, Text, Br
 from mkdoxy.utils import lookahead
 
 SIMPLE_SECTIONS = {
 	'see': 'See also:',
 	'note': 'Note:',
 	'bug': 'Bug:',
 	'warning': 'Warning:',
@@ -21,15 +22,16 @@
 	'remark': 'Remark:',
 	'copyright': 'Copyright:',
 	'post': 'Postcondition:',
 	'rcs': 'Rcs:',
 	'attention': 'Attention:',
 	'invariant': 'Invariant:',
 	'exception': 'Exception:',
-	'date': 'Date:'
+	'date': 'Date:',
+	'version': 'Version:',
 }
 
 class XmlParser:
 	def __init__(self, cache: Cache, debug: bool = False):
 		self.cache = cache
 		self.debug = debug
```

### Comparing `mkdoxy-1.0.6/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.1.0/mkdoxy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+mkdoxy/DoxyTagParser.py
 mkdoxy/__init__.py
 mkdoxy/cache.py
 mkdoxy/constants.py
 mkdoxy/doxygen.py
 mkdoxy/doxyrun.py
 mkdoxy/finder.py
 mkdoxy/generatorAuto.py
@@ -22,18 +23,20 @@
 mkdoxy.egg-info/entry_points.txt
 mkdoxy.egg-info/requires.txt
 mkdoxy.egg-info/top_level.txt
 mkdoxy/templates/annotated.jinja2
 mkdoxy/templates/classes.jinja2
 mkdoxy/templates/code.jinja2
 mkdoxy/templates/error.jinja2
+mkdoxy/templates/example.jinja2
+mkdoxy/templates/examples.jinja2
 mkdoxy/templates/files.jinja2
 mkdoxy/templates/hierarchy.jinja2
 mkdoxy/templates/index.jinja2
 mkdoxy/templates/memDef.jinja2
 mkdoxy/templates/memTab.jinja2
 mkdoxy/templates/member.jinja2
 mkdoxy/templates/modules.jinja2
 mkdoxy/templates/namespaces.jinja2
 mkdoxy/templates/page.jinja2
-mkdoxy/templates/pages.jinja2
-mkdoxy/templates/programlisting.jinja2
+mkdoxy/templates/programlisting.jinja2
+mkdoxy/templates/relatedPages.jinja2
```

### Comparing `mkdoxy-1.0.6/setup.py` & `mkdoxy-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 def requirements():
     with open('requirements.txt') as f:
         return f.read().splitlines()
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name='mkdoxy',
-    version='1.0.6',
+    version='1.1.0',
     description='MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator',
     url='https://github.com/JakubAndrysek/MkDoxy',
     author='Jakub Andrýsek',
     author_email='email@kubaandrysek.cz',
     license='MIT',
-    python_requires='>=3.8',
+    python_requires='>=3.9',
     install_requires=requirements(),
     classifiers=[
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
     ],
     packages=find_packages(),
     package_data={'mkdoxy': ['templates/*.jinja2']},
```

