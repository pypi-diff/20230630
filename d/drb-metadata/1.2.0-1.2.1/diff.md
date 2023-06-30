# Comparing `tmp/drb-metadata-1.2.0.tar.gz` & `tmp/drb-metadata-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-metadata-1.2.0.tar", last modified: Tue May 16 14:07:26 2023, max compression
+gzip compressed data, was "drb-metadata-1.2.1.tar", last modified: Fri Jun 30 07:30:51 2023, max compression
```

## Comparing `drb-metadata-1.2.0.tar` & `drb-metadata-1.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1818 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1400 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.685710 drb-metadata-1.2.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.705710 drb-metadata-1.2.0/drb/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/drb/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-16 14:07:26.705710 drb-metadata-1.2.0/drb/metadata/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5308 2023-05-16 13:19:20.000000 drb-metadata-1.2.0/drb/metadata/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/drb/metadata/schema.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/drb_metadata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1818 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/tests/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    81180 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 07:30:50.993131 drb-metadata-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-06-30 07:30:50.993131 drb-metadata-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 07:30:50.989130 drb-metadata-1.2.1/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 07:30:50.997130 drb-metadata-1.2.1/drb/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/drb/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-30 07:30:50.997130 drb-metadata-1.2.1/drb/metadata/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5408 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/drb/metadata/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/drb/metadata/schema.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 07:30:50.993131 drb-metadata-1.2.1/drb_metadata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-06-30 07:30:50.000000 drb-metadata-1.2.1/drb_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-30 07:30:50.000000 drb-metadata-1.2.1/drb_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 07:30:50.000000 drb-metadata-1.2.1/drb_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 07:30:50.000000 drb-metadata-1.2.1/drb_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-30 07:30:50.000000 drb-metadata-1.2.1/drb_metadata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-30 07:30:50.000000 drb-metadata-1.2.1/drb_metadata.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-30 07:30:50.997130 drb-metadata-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 07:30:50.993131 drb-metadata-1.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/tests/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    81180 2023-06-28 15:25:59.000000 drb-metadata-1.2.1/versioneer.py
```

### Comparing `drb-metadata-1.2.0/LICENCE.txt` & `drb-metadata-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-metadata-1.2.0/PKG-INFO` & `drb-metadata-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-metadata
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB Metadata Extractor
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -20,16 +20,17 @@
 ### How to extract metadata ?
 ```python
 from drb.metadata import DrbMetadataResolver
 import drb.topics.resolver as resolver
 
 
 if __name__ == '__main__':
-    node = resolver.create('<my_resource_url>')
-    metadata = DrbMetadataResolver().get_metadata(node)
+    topic, node = resolver.resolve('<my_resource_url>')
+    # topic keyword argument is not mandatory
+    metadata = DrbMetadataResolver().get_metadata(node, topic=topic)
     for md_name, md in metadata.items():
         print(md_name, ' -- ', md.extract(node))
 
 ```
 
 ### How to define metadata ?
 Metadata are defined in a `cortex.yaml` file following the template:
```

### Comparing `drb-metadata-1.2.0/README.md` & `drb-metadata-1.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 ### How to extract metadata ?
 ```python
 from drb.metadata import DrbMetadataResolver
 import drb.topics.resolver as resolver
 
 
 if __name__ == '__main__':
-    node = resolver.create('<my_resource_url>')
-    metadata = DrbMetadataResolver().get_metadata(node)
+    topic, node = resolver.resolve('<my_resource_url>')
+    # topic keyword argument is not mandatory
+    metadata = DrbMetadataResolver().get_metadata(node, topic=topic)
     for md_name, md in metadata.items():
         print(md_name, ' -- ', md.extract(node))
 
 ```
 
 ### How to define metadata ?
 Metadata are defined in a `cortex.yaml` file following the template:
```

### Comparing `drb-metadata-1.2.0/drb/metadata/metadata.py` & `drb-metadata-1.2.1/drb/metadata/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -161,10 +161,12 @@
         # add specific metadata of the given class (override if necessary)
         if ic.id in self.__metadata.keys():
             for md in self.__metadata[ic.id]:
                 metadata[md.name] = md
 
         return metadata
 
-    def get_metadata(self, node: DrbNode) -> Dict[str, DrbMetadata]:
+    def get_metadata(self, node: DrbNode, **kwargs) -> Dict[str, DrbMetadata]:
+        if 'topic' in kwargs:
+            return self._retrieve_metadata(kwargs['topic'])
         ic, base_node = resolver.resolve(node)
         return self._retrieve_metadata(ic)
```

### Comparing `drb-metadata-1.2.0/drb/metadata/schema.yml` & `drb-metadata-1.2.1/drb/metadata/schema.yml`

 * *Files identical despite different names*

### Comparing `drb-metadata-1.2.0/drb_metadata.egg-info/PKG-INFO` & `drb-metadata-1.2.1/drb_metadata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-metadata
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB Metadata Extractor
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -20,16 +20,17 @@
 ### How to extract metadata ?
 ```python
 from drb.metadata import DrbMetadataResolver
 import drb.topics.resolver as resolver
 
 
 if __name__ == '__main__':
-    node = resolver.create('<my_resource_url>')
-    metadata = DrbMetadataResolver().get_metadata(node)
+    topic, node = resolver.resolve('<my_resource_url>')
+    # topic keyword argument is not mandatory
+    metadata = DrbMetadataResolver().get_metadata(node, topic=topic)
     for md_name, md in metadata.items():
         print(md_name, ' -- ', md.extract(node))
 
 ```
 
 ### How to define metadata ?
 Metadata are defined in a `cortex.yaml` file following the template:
```

### Comparing `drb-metadata-1.2.0/setup.cfg` & `drb-metadata-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-metadata-1.2.0/versioneer.py` & `drb-metadata-1.2.1/versioneer.py`

 * *Files identical despite different names*

