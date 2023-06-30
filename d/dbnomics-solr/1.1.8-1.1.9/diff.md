# Comparing `tmp/dbnomics-solr-1.1.8.tar.gz` & `tmp/dbnomics-solr-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnomics-solr-1.1.8.tar", max compression
+gzip compressed data, was "dbnomics-solr-1.1.9.tar", max compression
```

## Comparing `dbnomics-solr-1.1.8.tar` & `dbnomics-solr-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34452 2022-04-04 11:13:02.240011 dbnomics-solr-1.1.8/LICENSE
--rw-r--r--   0        0        0     1634 2022-04-04 13:53:11.921594 dbnomics-solr-1.1.8/README.md
--rw-r--r--   0        0        0       36 2022-04-08 13:01:15.515087 dbnomics-solr-1.1.8/dbnomics_solr/__init__.py
--rwxr-xr-x   0        0        0     9284 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/cli.py
--rw-r--r--   0        0        0    21622 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/dbnomics_solr_client.py
--rw-r--r--   0        0        0     1233 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/errors.py
--rw-r--r--   0        0        0      308 2022-04-04 11:13:02.244011 dbnomics-solr-1.1.8/dbnomics_solr/hash_utils.py
--rw-r--r--   0        0        0        0 2022-04-04 11:13:02.244011 dbnomics-solr-1.1.8/dbnomics_solr/py.typed
--rw-r--r--   0        0        0      215 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/services/__init__.py
--rw-r--r--   0        0        0     1199 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/services/delete_dataset_docs.py
--rw-r--r--   0        0        0     1181 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/services/delete_extra_datasets.py
--rw-r--r--   0        0        0     2238 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/services/delete_provider_docs.py
--rw-r--r--   0        0        0     5656 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/services/index_provider.py
--rw-r--r--   0        0        0     1259 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/services/search_extra_datasets.py
--rw-r--r--   0        0        0      903 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/services/search_provider_datasets.py
--rw-r--r--   0        0        0      161 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/types.py
--rw-r--r--   0        0        0      274 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/dbnomics_solr/utils.py
--rw-r--r--   0        0        0     1619 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 dbnomics-solr-1.1.8/setup.py
--rw-r--r--   0        0        0     2860 1970-01-01 00:00:00.000000 dbnomics-solr-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    34452 2022-04-04 11:13:02.240011 dbnomics-solr-1.1.9/LICENSE
+-rw-r--r--   0        0        0     1634 2022-04-04 13:53:11.921594 dbnomics-solr-1.1.9/README.md
+-rw-r--r--   0        0        0       36 2022-04-08 13:01:15.515087 dbnomics-solr-1.1.9/dbnomics_solr/__init__.py
+-rwxr-xr-x   0        0        0     9284 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/cli.py
+-rw-r--r--   0        0        0    21622 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/dbnomics_solr_client.py
+-rw-r--r--   0        0        0     1233 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/errors.py
+-rw-r--r--   0        0        0      308 2022-04-04 11:13:02.244011 dbnomics-solr-1.1.9/dbnomics_solr/hash_utils.py
+-rw-r--r--   0        0        0        0 2022-04-04 11:13:02.244011 dbnomics-solr-1.1.9/dbnomics_solr/py.typed
+-rw-r--r--   0        0        0      215 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/services/__init__.py
+-rw-r--r--   0        0        0     1199 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/services/delete_dataset_docs.py
+-rw-r--r--   0        0        0     1215 2022-06-28 12:23:44.209258 dbnomics-solr-1.1.9/dbnomics_solr/services/delete_extra_datasets.py
+-rw-r--r--   0        0        0     2238 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/services/delete_provider_docs.py
+-rw-r--r--   0        0        0     5656 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/services/index_provider.py
+-rw-r--r--   0        0        0     1259 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/services/search_extra_datasets.py
+-rw-r--r--   0        0        0      903 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/services/search_provider_datasets.py
+-rw-r--r--   0        0        0      161 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/types.py
+-rw-r--r--   0        0        0      274 2022-06-28 11:50:21.306161 dbnomics-solr-1.1.9/dbnomics_solr/utils.py
+-rw-r--r--   0        0        0     1619 2022-06-28 12:23:44.209258 dbnomics-solr-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 dbnomics-solr-1.1.9/setup.py
+-rw-r--r--   0        0        0     2860 1970-01-01 00:00:00.000000 dbnomics-solr-1.1.9/PKG-INFO
```

### Comparing `dbnomics-solr-1.1.8/LICENSE` & `dbnomics-solr-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/README.md` & `dbnomics-solr-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/dbnomics_solr/cli.py` & `dbnomics-solr-1.1.9/dbnomics_solr/cli.py`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/dbnomics_solr/dbnomics_solr_client.py` & `dbnomics-solr-1.1.9/dbnomics_solr/dbnomics_solr_client.py`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/dbnomics_solr/errors.py` & `dbnomics-solr-1.1.9/dbnomics_solr/errors.py`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/dbnomics_solr/services/delete_dataset_docs.py` & `dbnomics-solr-1.1.9/dbnomics_solr/services/delete_dataset_docs.py`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/dbnomics_solr/services/delete_extra_datasets.py` & `dbnomics-solr-1.1.9/dbnomics_solr/services/delete_extra_datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,7 +29,8 @@
         storage=storage,
         storage_dataset_codes=storage_dataset_codes,
     )
     for dataset_code in extra_dataset_codes:
         dataset_id = f"{provider_code}/{dataset_code}"
         logger.info("Deleting the extra dataset", dataset_id=dataset_id)
         dbnomics_solr_client.delete_dataset_docs(provider_code, dataset_code)
+    dbnomics_solr_client.commit()
```

### Comparing `dbnomics-solr-1.1.8/dbnomics_solr/services/delete_provider_docs.py` & `dbnomics-solr-1.1.9/dbnomics_solr/services/delete_provider_docs.py`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/dbnomics_solr/services/index_provider.py` & `dbnomics-solr-1.1.9/dbnomics_solr/services/index_provider.py`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/dbnomics_solr/services/search_extra_datasets.py` & `dbnomics-solr-1.1.9/dbnomics_solr/services/search_extra_datasets.py`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/dbnomics_solr/services/search_provider_datasets.py` & `dbnomics-solr-1.1.9/dbnomics_solr/services/search_provider_datasets.py`

 * *Files identical despite different names*

### Comparing `dbnomics-solr-1.1.8/pyproject.toml` & `dbnomics-solr-1.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbnomics-solr"
-version = "1.1.8"
+version = "1.1.9"
 description = "Index DBnomics data with Apache Solr for full-text and faceted search"
 authors = ["Christophe Benz <christophe.benz@nomics.world>"]
 license = "AGPLv3+"
 readme = "README.md"
 repository = "https://git.nomics.world/dbnomics/dbnomics-solr"
 
 [tool.poetry.dependencies]
```

### Comparing `dbnomics-solr-1.1.8/setup.py` & `dbnomics-solr-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'typer>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['dbnomics-solr = dbnomics_solr.cli:app']}
 
 setup_kwargs = {
     'name': 'dbnomics-solr',
-    'version': '1.1.8',
+    'version': '1.1.9',
     'description': 'Index DBnomics data with Apache Solr for full-text and faceted search',
     'long_description': '# DBnomics Solr\n\nIndex DBnomics data into Apache Solr for full-text and faceted search.\n\nRequirements:\n\n- a running instance of [Apache Solr](http://lucene.apache.org/solr/); at the time this documentation is written, we use the version 7.3.\n\nSee [dbnomics-docker](https://git.nomics.world/dbnomics/dbnomics-docker) to run a local DBnomics instance with Docker that includes a service for Apache Solr.\n\n## Configuration\n\nEnvironment variables:\n\n- `DEBUG_PYSOLR`: display pysolr DEBUG logging messages (cf <https://github.com/django-haystack/pysolr>)\n\n## Index a provider\n\nReplace `wto` by the real provider slug in the following command:\n\n```bash\ndbnomics-solr index-provider /path/to/wto-json-data\n```\n\n### Full mode vs incremental mode\n\nWhen data is stored in a regular directory, the script always indexes all datasets and series of a provider. This is called _full mode_.\n\nWhen data is stored in a Git repository, the script runs by default in _incremental mode_: it indexes only the datasets modified since the last indexation.\n\nIt is possible to force the _full mode_ with the `--full` option.\n\n### Bare repositories\n\nThe script has an option `--bare-repo-fallback` which tries to add `.git` at the end of the storage dir name, if not found.\n\n## Remove all data from a provider\n\nTo remove all the documents related to a provider (`type:provider`, `type:dataset` and `type:series`):\n\n```bash\ndbnomics-solr --debug delete-provider --code <provider_code>\ndbnomics-solr --debug delete-provider --slug <provider_slug>\n\n# Examples:\ndbnomics-solr --debug delete-provider --code WTO\ndbnomics-solr --debug delete-provider --slug wto\n```\n',
     'author': 'Christophe Benz',
     'author_email': 'christophe.benz@nomics.world',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.nomics.world/dbnomics/dbnomics-solr',
```

### Comparing `dbnomics-solr-1.1.8/PKG-INFO` & `dbnomics-solr-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnomics-solr
-Version: 1.1.8
+Version: 1.1.9
 Summary: Index DBnomics data with Apache Solr for full-text and faceted search
 Home-page: https://git.nomics.world/dbnomics/dbnomics-solr
 License: AGPLv3+
 Author: Christophe Benz
 Author-email: christophe.benz@nomics.world
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

