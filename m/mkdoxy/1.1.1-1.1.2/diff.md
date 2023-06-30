# Comparing `tmp/mkdoxy-1.1.1.tar.gz` & `tmp/mkdoxy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.1.1.tar", last modified: Fri Jun 30 12:12:18 2023, max compression
+gzip compressed data, was "mkdoxy-1.1.2.tar", last modified: Fri Jun 30 13:15:30 2023, max compression
```

## Comparing `mkdoxy-1.1.1.tar` & `mkdoxy-1.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 12:12:18.187363 mkdoxy-1.1.1/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.1/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     5072 2023-06-30 12:12:18.187138 mkdoxy-1.1.1/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     4344 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 12:12:18.182875 mkdoxy-1.1.1/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/DoxyTagParser.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.1/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.1/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     2841 2023-04-07 16:49:36.000000 mkdoxy-1.1.1/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     4415 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     4369 2023-06-30 12:01:41.000000 mkdoxy-1.1.1/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)    12065 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.1.1/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    20867 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     7661 2023-06-30 11:59:11.000000 mkdoxy-1.1.1/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 12:12:18.186875 mkdoxy-1.1.1/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      351 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/example.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/examples.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4480 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      444 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/templates/relatedPages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-06-30 11:43:03.000000 mkdoxy-1.1.1/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 12:12:18.183917 mkdoxy-1.1.1/mkdoxy.egg-info/
--rwxr-xr-x   0 kuba       (501) staff       (20)     5072 2023-06-30 12:12:18.000000 mkdoxy-1.1.1/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-06-30 12:12:18.000000 mkdoxy-1.1.1/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-06-30 12:12:18.000000 mkdoxy-1.1.1/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-06-30 12:12:18.000000 mkdoxy-1.1.1/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)      107 2023-06-30 12:12:18.000000 mkdoxy-1.1.1/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-06-30 12:12:18.000000 mkdoxy-1.1.1/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       38 2023-06-30 12:12:18.187414 mkdoxy-1.1.1/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1293 2023-06-30 12:02:05.000000 mkdoxy-1.1.1/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 13:15:30.227069 mkdoxy-1.1.2/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.2/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5072 2023-06-30 13:15:30.226925 mkdoxy-1.1.2/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4344 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 13:15:30.223655 mkdoxy-1.1.2/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.2/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.2/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2841 2023-04-07 16:49:36.000000 mkdoxy-1.1.2/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4415 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4326 2023-06-30 13:10:28.000000 mkdoxy-1.1.2/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    12065 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.1.2/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    20935 2023-06-30 12:40:39.000000 mkdoxy-1.1.2/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7661 2023-06-30 13:09:49.000000 mkdoxy-1.1.2/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 13:15:30.226701 mkdoxy-1.1.2/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      351 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4480 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      444 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 13:15:30.224305 mkdoxy-1.1.2/mkdoxy.egg-info/
+-rwxr-xr-x   0 kuba       (501) staff       (20)     5072 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/entry_points.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)      107 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/requires.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2023-06-30 13:15:30.227110 mkdoxy-1.1.2/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1293 2023-06-30 13:12:18.000000 mkdoxy-1.1.2/setup.py
```

### Comparing `mkdoxy-1.1.1/LICENSE` & `mkdoxy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/PKG-INFO` & `mkdoxy-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.1
+Version: 1.1.2
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Keywords: mkdoxy,python,open-source,documentation,mkdocs,doxygen,multilanguage,code-snippets,code,snippets,documentation-generator
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.1 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.2 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Keywords: mkdoxy,python,open-
 source,documentation,mkdocs,doxygen,multilanguage,code-
 snippets,code,snippets,documentation-generator Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `mkdoxy-1.1.1/README.md` & `mkdoxy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/DoxyTagParser.py` & `mkdoxy-1.1.2/mkdoxy/DoxyTagParser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/constants.py` & `mkdoxy-1.1.2/mkdoxy/constants.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/doxygen.py` & `mkdoxy-1.1.2/mkdoxy/doxygen.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/doxyrun.py` & `mkdoxy-1.1.2/mkdoxy/doxyrun.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,14 @@
 			"GENERATE_HTML": "NO",
 			"GENERATE_LATEX": "NO",
 		}
 
 		self.doxyCfg.update(self.doxyCfgNew)
 		self.doxyCfgStr: str = self.dox_dict2str(self.doxyCfg)
 
-		new_file, filename = tempfile.mkstemp()
-
 	# Source of dox_dict2str: https://xdress-fabio.readthedocs.io/en/latest/_modules/xdress/doxygen.html#XDressPlugin
 	def dox_dict2str(self, dox_dict: dict) -> str:
 		"""! Convert a dictionary to a string that can be written to a doxygen config file.
 		@details
 		@param dox_dict: (dict) Dictionary to convert.
 		@return: (str) String that can be written to a doxygen config file.
 		"""
```

### Comparing `mkdoxy-1.1.1/mkdoxy/finder.py` & `mkdoxy-1.1.2/mkdoxy/finder.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/generatorAuto.py` & `mkdoxy-1.1.2/mkdoxy/generatorAuto.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/generatorBase.py` & `mkdoxy-1.1.2/mkdoxy/generatorBase.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/generatorSnippets.py` & `mkdoxy-1.1.2/mkdoxy/generatorSnippets.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/markdown.py` & `mkdoxy-1.1.2/mkdoxy/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/node.py` & `mkdoxy-1.1.2/mkdoxy/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 			self._dirname = os.path.dirname(xml_file)
 			self._xml = ElementTree.parse(xml_file).getroot().find('compounddef')
 			if self._xml is None:
 				raise Exception(f'File {xml_file} has no <compounddef>')
 			self._kind = Kind.from_str(self._xml.get('kind'))
 			self._refid = self._xml.get('id')
 			self._language = self._xml.get('language')
-			self._name = self._xml.find('compoundname').text
+			self._name = self._xml.find('compoundname').text if self._xml.find('compoundname').text is not None else self._refid
 			self._cache.add(self._refid, self)
 			self._static = False
 
 			if self.debug:
 				log.info(f'Parsing: {self._refid}')
 			self._check_for_children()
```

### Comparing `mkdoxy-1.1.1/mkdoxy/plugin.py` & `mkdoxy-1.1.2/mkdoxy/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/property.py` & `mkdoxy-1.1.2/mkdoxy/property.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/templates/annotated.jinja2` & `mkdoxy-1.1.2/mkdoxy/templates/annotated.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/templates/code.jinja2` & `mkdoxy-1.1.2/mkdoxy/templates/code.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/templates/error.jinja2` & `mkdoxy-1.1.2/mkdoxy/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/templates/examples.jinja2` & `mkdoxy-1.1.2/mkdoxy/templates/examples.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/templates/memDef.jinja2` & `mkdoxy-1.1.2/mkdoxy/templates/memDef.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.1.2/mkdoxy/templates/memTab.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/templates/member.jinja2` & `mkdoxy-1.1.2/mkdoxy/templates/member.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/utils.py` & `mkdoxy-1.1.2/mkdoxy/utils.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy/xml_parser.py` & `mkdoxy-1.1.2/mkdoxy/xml_parser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/mkdoxy.egg-info/PKG-INFO` & `mkdoxy-1.1.2/mkdoxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.1
+Version: 1.1.2
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Keywords: mkdoxy,python,open-source,documentation,mkdocs,doxygen,multilanguage,code-snippets,code,snippets,documentation-generator
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.1 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.2 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Keywords: mkdoxy,python,open-
 source,documentation,mkdocs,doxygen,multilanguage,code-
 snippets,code,snippets,documentation-generator Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `mkdoxy-1.1.1/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.1.2/mkdoxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.1/setup.py` & `mkdoxy-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def requirements():
     with open('requirements.txt') as f:
         return f.read().splitlines()
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name='mkdoxy',
-    version='1.1.1',
+    version='1.1.2',
     description='MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator',
     url='https://github.com/JakubAndrysek/MkDoxy',
     author='Jakub Andrýsek',
     author_email='email@kubaandrysek.cz',
```

