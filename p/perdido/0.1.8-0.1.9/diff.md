# Comparing `tmp/perdido-0.1.8.tar.gz` & `tmp/perdido-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perdido-0.1.8.tar", last modified: Sat Jun 11 09:58:46 2022, max compression
+gzip compressed data, was "perdido-0.1.9.tar", last modified: Sun Jun 12 16:22:30 2022, max compression
```

## Comparing `perdido-0.1.8.tar` & `perdido-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-11 09:58:46.970830 perdido-0.1.8/
--rw-r--r--   0 lmoncla    (501) staff       (20)     1324 2022-06-01 11:36:37.000000 perdido-0.1.8/LICENSE
--rw-r--r--   0 lmoncla    (501) staff       (20)       64 2022-06-01 15:21:47.000000 perdido-0.1.8/MANIFEST.in
--rw-r--r--   0 lmoncla    (501) staff       (20)     4466 2022-06-11 09:58:46.969140 perdido-0.1.8/PKG-INFO
--rw-r--r--   0 lmoncla    (501) staff       (20)     3824 2022-06-10 07:41:22.000000 perdido-0.1.8/README.md
-drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-11 09:58:46.961948 perdido-0.1.8/perdido/
--rw-r--r--   0 lmoncla    (501) staff       (20)      112 2022-06-03 20:29:45.000000 perdido-0.1.8/perdido/__init__.py
--rw-r--r--   0 lmoncla    (501) staff       (20)     1972 2022-06-08 12:19:34.000000 perdido-0.1.8/perdido/geocoder.py
--rw-r--r--   0 lmoncla    (501) staff       (20)     2158 2022-06-07 13:00:13.000000 perdido-0.1.8/perdido/geoparser.py
--rw-r--r--   0 lmoncla    (501) staff       (20)     2084 2022-06-09 15:48:12.000000 perdido-0.1.8/perdido/perdido.py
-drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-11 09:58:46.968333 perdido-0.1.8/perdido/utils/
--rw-r--r--   0 lmoncla    (501) staff       (20)        0 2022-06-01 11:52:44.000000 perdido-0.1.8/perdido/utils/__init__.py
--rw-r--r--   0 lmoncla    (501) staff       (20)     1488 2022-06-07 04:54:32.000000 perdido-0.1.8/perdido/utils/map.py
--rw-r--r--   0 lmoncla    (501) staff       (20)     1651 2022-06-08 11:38:20.000000 perdido-0.1.8/perdido/utils/webservices.py
--rw-r--r--   0 lmoncla    (501) staff       (20)     7440 2022-06-11 09:58:29.000000 perdido-0.1.8/perdido/utils/xml.py
-drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-11 09:58:46.964572 perdido-0.1.8/perdido.egg-info/
--rw-r--r--   0 lmoncla    (501) staff       (20)     4466 2022-06-11 09:58:46.000000 perdido-0.1.8/perdido.egg-info/PKG-INFO
--rw-r--r--   0 lmoncla    (501) staff       (20)      369 2022-06-11 09:58:46.000000 perdido-0.1.8/perdido.egg-info/SOURCES.txt
--rw-r--r--   0 lmoncla    (501) staff       (20)        1 2022-06-11 09:58:46.000000 perdido-0.1.8/perdido.egg-info/dependency_links.txt
--rw-r--r--   0 lmoncla    (501) staff       (20)       35 2022-06-11 09:58:46.000000 perdido-0.1.8/perdido.egg-info/requires.txt
--rw-r--r--   0 lmoncla    (501) staff       (20)        8 2022-06-11 09:58:46.000000 perdido-0.1.8/perdido.egg-info/top_level.txt
--rw-r--r--   0 lmoncla    (501) staff       (20)       38 2022-06-11 09:58:46.971187 perdido-0.1.8/setup.cfg
--rw-r--r--   0 lmoncla    (501) staff       (20)     2104 2022-06-11 09:58:42.000000 perdido-0.1.8/setup.py
+drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-12 16:22:30.228742 perdido-0.1.9/
+-rw-r--r--   0 lmoncla    (501) staff       (20)     1324 2022-06-01 11:36:37.000000 perdido-0.1.9/LICENSE
+-rw-r--r--   0 lmoncla    (501) staff       (20)       64 2022-06-01 15:21:47.000000 perdido-0.1.9/MANIFEST.in
+-rw-r--r--   0 lmoncla    (501) staff       (20)     4466 2022-06-12 16:22:30.228375 perdido-0.1.9/PKG-INFO
+-rw-r--r--   0 lmoncla    (501) staff       (20)     3824 2022-06-10 07:41:22.000000 perdido-0.1.9/README.md
+drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-12 16:22:30.221120 perdido-0.1.9/perdido/
+-rw-r--r--   0 lmoncla    (501) staff       (20)      112 2022-06-03 20:29:45.000000 perdido-0.1.9/perdido/__init__.py
+drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-12 16:22:30.215295 perdido-0.1.9/perdido/datasets/
+drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-12 16:22:30.223595 perdido-0.1.9/perdido/datasets/edda_artfl/
+-rw-r--r--   0 lmoncla    (501) staff       (20)   203607 2022-06-12 06:48:55.000000 perdido-0.1.9/perdido/datasets/edda_artfl/edda_artf_dataset.csv
+-rw-r--r--   0 lmoncla    (501) staff       (20)     1937 2022-06-12 10:51:53.000000 perdido-0.1.9/perdido/datasets.py
+-rw-r--r--   0 lmoncla    (501) staff       (20)     1972 2022-06-08 12:19:34.000000 perdido-0.1.9/perdido/geocoder.py
+-rw-r--r--   0 lmoncla    (501) staff       (20)     2158 2022-06-07 13:00:13.000000 perdido-0.1.9/perdido/geoparser.py
+-rw-r--r--   0 lmoncla    (501) staff       (20)     2701 2022-06-12 16:21:42.000000 perdido-0.1.9/perdido/perdido.py
+drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-12 16:22:30.227837 perdido-0.1.9/perdido/utils/
+-rw-r--r--   0 lmoncla    (501) staff       (20)        0 2022-06-01 11:52:44.000000 perdido-0.1.9/perdido/utils/__init__.py
+-rw-r--r--   0 lmoncla    (501) staff       (20)     1488 2022-06-07 04:54:32.000000 perdido-0.1.9/perdido/utils/map.py
+-rw-r--r--   0 lmoncla    (501) staff       (20)     1651 2022-06-08 11:38:20.000000 perdido-0.1.9/perdido/utils/webservices.py
+-rw-r--r--   0 lmoncla    (501) staff       (20)     7481 2022-06-12 11:44:40.000000 perdido-0.1.9/perdido/utils/xml.py
+drwxr-xr-x   0 lmoncla    (501) staff       (20)        0 2022-06-12 16:22:30.223144 perdido-0.1.9/perdido.egg-info/
+-rw-r--r--   0 lmoncla    (501) staff       (20)     4466 2022-06-12 16:22:29.000000 perdido-0.1.9/perdido.egg-info/PKG-INFO
+-rw-r--r--   0 lmoncla    (501) staff       (20)      439 2022-06-12 16:22:30.000000 perdido-0.1.9/perdido.egg-info/SOURCES.txt
+-rw-r--r--   0 lmoncla    (501) staff       (20)        1 2022-06-12 16:22:29.000000 perdido-0.1.9/perdido.egg-info/dependency_links.txt
+-rw-r--r--   0 lmoncla    (501) staff       (20)       41 2022-06-12 16:22:29.000000 perdido-0.1.9/perdido.egg-info/requires.txt
+-rw-r--r--   0 lmoncla    (501) staff       (20)        8 2022-06-12 16:22:30.000000 perdido-0.1.9/perdido.egg-info/top_level.txt
+-rw-r--r--   0 lmoncla    (501) staff       (20)       38 2022-06-12 16:22:30.228877 perdido-0.1.9/setup.cfg
+-rw-r--r--   0 lmoncla    (501) staff       (20)     2180 2022-06-12 16:22:23.000000 perdido-0.1.9/setup.py
```

### Comparing `perdido-0.1.8/LICENSE` & `perdido-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `perdido-0.1.8/PKG-INFO` & `perdido-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perdido
-Version: 0.1.8
+Version: 0.1.9
 Summary: PERDIDO Geoparser python library
 Home-page: https://github.com/ludovicmoncla/perdido
 Author: Ludovic Moncla
 Author-email: moncla.ludovic@gmail.com
 License: BSD-Clause-2
 Keywords: geoparsing named-entity-recognition geographic-information-retrieval toponym-resolution toponym-disambiguation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `perdido-0.1.8/README.md` & `perdido-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `perdido-0.1.8/perdido/geocoder.py` & `perdido-0.1.9/perdido/geocoder.py`

 * *Files identical despite different names*

### Comparing `perdido-0.1.8/perdido/geoparser.py` & `perdido-0.1.9/perdido/geoparser.py`

 * *Files identical despite different names*

### Comparing `perdido-0.1.8/perdido/perdido.py` & `perdido-0.1.9/perdido/perdido.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from typing import Iterator, List, Union
 
 import lxml.etree as etree
 import folium
 import geojson
 
 from perdido.utils.xml import Token
-from perdido.utils.xml import get_tokens_from_tei, get_entities_from_tei, get_toponyms_from_tei, get_nested_entities_from_tei, get_toponyms_from_geojson
+from perdido.utils.xml import get_tokens_from_tei, get_entities_from_tei, get_toponyms_from_tei, get_nested_entities_from_tei, get_toponyms_from_geojson, parent_exists
 from perdido.utils.map import overlay_gpx, get_bounding_box
 
+from spacy.tokens import Span
+from spacy.tokens import Doc
+from spacy.vocab import Vocab
+
 
 class Perdido:
 
 
     def __init__(self) -> None:
 
         self.text = None
@@ -46,15 +50,15 @@
 
     def parse_geojson(self) -> None:
         if self.geojson is not None:
            
             self.toponyms = get_toponyms_from_geojson(self.geojson)  
            
 
-    def get_folium_map(self, properties: Union[List[str], None] = None, gpx: Union[str , None] = None) -> Union[folium.Map,None]:
+    def get_folium_map(self, properties: Union[List[str], None] = ['name', 'source'], gpx: Union[str , None] = None) -> Union[folium.Map,None]:
         m = folium.Map()
         if gpx is not None:
             overlay_gpx(m, gpx)
 
         if self.geojson is not None:
             coords = list(geojson.utils.coords(self.geojson))
             if len(coords) > 0:
@@ -63,8 +67,26 @@
                     folium.GeoJson(self.geojson, name='Toponyms', tooltip=folium.features.GeoJsonTooltip(fields=properties, localize=True)).add_to(m)
                 else:
                     folium.GeoJson(self.geojson, name='Toponyms').add_to(m)
                 return m    
         return None
 
 
+    def to_displacy(self) -> Doc:
+        vocab = Vocab()
+        
+        words = [t.text for t in self.tokens]
+        spaces = [True] * len(words)
+        
+        doc = Doc(vocab, words = words, spaces = spaces)
+        ents = [] 
+
+        for e in self.ne:
+            if e.start is not None and e.end is not None:
+                print(e.text, e.tag, e.start, e.end)
+                ents.append(Span(doc, int(e.start), int(e.end), label=e.tag))
+
+        doc.ents = ents
+        return doc 
+
+
```

### Comparing `perdido-0.1.8/perdido/utils/map.py` & `perdido-0.1.9/perdido/utils/map.py`

 * *Files identical despite different names*

### Comparing `perdido-0.1.8/perdido/utils/webservices.py` & `perdido-0.1.9/perdido/utils/webservices.py`

 * *Files identical despite different names*

### Comparing `perdido-0.1.8/perdido/utils/xml.py` & `perdido-0.1.9/perdido/utils/xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,24 +158,25 @@
 
 
 def get_entity(elt: Element) -> Entity:
     text = get_w_content(elt)
     tag = elt.get('type') if 'type' in elt.attrib else  ""
     tokens = get_tokens_from_tei(elt)
     parent = elt.getparent()
+    start = None
+    end = None
 
     if elt.tag == 'name':
-
-        start = elt.get('startT') if 'startT' in elt.attrib else  ""
-        end = elt.get('endT') if 'endT' in elt.attrib else  ""
+        start = elt.get('startT') if 'startT' in elt.attrib else  None
+        end = elt.get('endT') if 'endT' in elt.attrib else  None
     elif elt.tag == 'rs':
-        subtype = elt.get('subtype') if 'subtype' in elt.attrib else  ""
+        subtype = elt.get('subtype') if 'subtype' in elt.attrib else  None
         if subtype == 'ene':
-            start = elt.get('startT') if 'startT' in elt.attrib else  ""
-            end = elt.get('endT') if 'endT' in elt.attrib else  ""
+            start = elt.get('startT') if 'startT' in elt.attrib else  None
+            end = elt.get('endT') if 'endT' in elt.attrib else  None
         
     #TODO get and return lat/lng if it is a place
     return Entity(text = text, tokens = tokens, start = start, end = end, tag = tag, parent = parent)
 
 
 def get_toponyms_from_tei(elt: Element) -> List[Toponym]:
     toponyms = []
```

### Comparing `perdido-0.1.8/perdido.egg-info/PKG-INFO` & `perdido-0.1.9/perdido.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perdido
-Version: 0.1.8
+Version: 0.1.9
 Summary: PERDIDO Geoparser python library
 Home-page: https://github.com/ludovicmoncla/perdido
 Author: Ludovic Moncla
 Author-email: moncla.ludovic@gmail.com
 License: BSD-Clause-2
 Keywords: geoparsing named-entity-recognition geographic-information-retrieval toponym-resolution toponym-disambiguation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `perdido-0.1.8/setup.py` & `perdido-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='perdido',
-    version='0.1.8',
+    version='0.1.9',
     license='BSD-Clause-2',
     author='Ludovic Moncla',
     author_email='moncla.ludovic@gmail.com',
     description="PERDIDO Geoparser python library",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ludovicmoncla/perdido',
@@ -55,8 +55,10 @@
          'Operating System :: POSIX :: Other',
          'Operating System :: MacOS',
 
          'Programming Language :: Python :: 3',
     ],
     keywords='geoparsing named-entity-recognition geographic-information-retrieval toponym-resolution toponym-disambiguation',
     install_requires=get_requirements(),
+    include_package_data=True,
+    package_data={'': ['datasets/*/*.csv']},
 )
```

