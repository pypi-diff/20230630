# Comparing `tmp/odd-collector-sdk-0.3.8.tar.gz` & `tmp/odd_collector_sdk-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odd-collector-sdk-0.3.8.tar", max compression
+gzip compressed data, was "odd_collector_sdk-0.3.9.tar", max compression
```

## Comparing `odd-collector-sdk-0.3.8.tar` & `odd_collector_sdk-0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11356 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/LICENSE
--rw-r--r--   0        0        0     5422 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/README.md
--rw-r--r--   0        0        0        1 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/__init__.py
--rw-r--r--   0        0        0        0 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/api/__init__.py
--rw-r--r--   0        0        0     1464 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/api/datasource_api.py
--rw-r--r--   0        0        0      522 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/api/http_client.py
--rw-r--r--   0        0        0     2268 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/collector.py
--rw-r--r--   0        0        0        0 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/domain/__init__.py
--rw-r--r--   0        0        0      514 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/domain/adapter.py
--rw-r--r--   0        0        0     2095 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/domain/adapters_initializer.py
--rw-r--r--   0        0        0      307 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/domain/collector_config.py
--rw-r--r--   0        0        0      635 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/domain/collector_config_loader.py
--rw-r--r--   0        0        0      172 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/domain/plugin.py
--rw-r--r--   0        0        0      214 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/errors.py
--rw-r--r--   0        0        0     3724 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/job.py
--rw-r--r--   0        0        0       64 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/logger.py
--rw-r--r--   0        0        0      123 2022-12-26 18:21:00.000000 odd-collector-sdk-0.3.8/odd_collector_sdk/types/__init__.py
--rw-r--r--   0        0        0      866 2022-12-26 18:21:17.000000 odd-collector-sdk-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6632 2022-12-26 18:22:10.064800 odd-collector-sdk-0.3.8/setup.py
--rw-r--r--   0        0        0     6491 2022-12-26 18:22:10.065499 odd-collector-sdk-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/LICENSE
+-rw-r--r--   0        0        0     5422 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/README.md
+-rw-r--r--   0        0        0        1 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1464 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/api/datasource_api.py
+-rw-r--r--   0        0        0      522 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/api/http_client.py
+-rw-r--r--   0        0        0     2581 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/collector.py
+-rw-r--r--   0        0        0        0 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/domain/__init__.py
+-rw-r--r--   0        0        0      514 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/domain/adapter.py
+-rw-r--r--   0        0        0     2095 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/domain/adapters_initializer.py
+-rw-r--r--   0        0        0      546 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/domain/collector_config.py
+-rw-r--r--   0        0        0      635 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/domain/collector_config_loader.py
+-rw-r--r--   0        0        0      172 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/domain/plugin.py
+-rw-r--r--   0        0        0      214 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/errors.py
+-rw-r--r--   0        0        0     3724 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/job.py
+-rw-r--r--   0        0        0       64 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/logger.py
+-rw-r--r--   0        0        0      123 2023-01-11 09:17:54.000000 odd_collector_sdk-0.3.9/odd_collector_sdk/types/__init__.py
+-rw-r--r--   0        0        0      866 2023-01-11 09:18:11.000000 odd_collector_sdk-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6636 1970-01-01 00:00:00.000000 odd_collector_sdk-0.3.9/setup.py
+-rw-r--r--   0        0        0     6593 1970-01-01 00:00:00.000000 odd_collector_sdk-0.3.9/PKG-INFO
```

### Comparing `odd-collector-sdk-0.3.8/LICENSE` & `odd_collector_sdk-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odd-collector-sdk-0.3.8/README.md` & `odd_collector_sdk-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `odd-collector-sdk-0.3.8/odd_collector_sdk/api/datasource_api.py` & `odd_collector_sdk-0.3.9/odd_collector_sdk/api/datasource_api.py`

 * *Files identical despite different names*

### Comparing `odd-collector-sdk-0.3.8/odd_collector_sdk/api/http_client.py` & `odd_collector_sdk-0.3.9/odd_collector_sdk/api/http_client.py`

 * *Files identical despite different names*

### Comparing `odd-collector-sdk-0.3.8/odd_collector_sdk/collector.py` & `odd_collector_sdk-0.3.9/odd_collector_sdk/collector.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,21 +34,29 @@
                 token=self.config.token,
                 connection_timeout_seconds=self.config.connection_timeout_seconds,
             ),
             platform_url=self.config.platform_host_url,
         )
 
     def start_polling(self):
+        misfire_grace_time = (
+            self.config.misfire_grace_time or self.config.default_pulling_interval * 60
+        )
+
         scheduler = AsyncIOScheduler(timezone=str(tzlocal.get_localzone()))
         for adapter in self._adapters:
             scheduler.add_job(
                 create_job(self._api, adapter, self.config.chunk_size).start,
                 "interval",
                 minutes=self.config.default_pulling_interval,
                 next_run_time=datetime.now(),
+                misfire_grace_time=misfire_grace_time,
+                max_instances=self.config.max_instances,
+                coalesce=True,
+                id=adapter.config.name,
             )
         scheduler.start()
 
     async def register_data_sources(self):
         data_sources: List[DataSource] = [
             DataSource(
                 oddrn=adapter.get_data_source_oddrn(),
```

### Comparing `odd-collector-sdk-0.3.8/odd_collector_sdk/domain/adapter.py` & `odd_collector_sdk-0.3.9/odd_collector_sdk/domain/adapter.py`

 * *Files identical despite different names*

### Comparing `odd-collector-sdk-0.3.8/odd_collector_sdk/domain/adapters_initializer.py` & `odd_collector_sdk-0.3.9/odd_collector_sdk/domain/adapters_initializer.py`

 * *Files identical despite different names*

### Comparing `odd-collector-sdk-0.3.8/odd_collector_sdk/domain/collector_config_loader.py` & `odd_collector_sdk-0.3.9/odd_collector_sdk/domain/collector_config_loader.py`

 * *Files identical despite different names*

### Comparing `odd-collector-sdk-0.3.8/odd_collector_sdk/job.py` & `odd_collector_sdk-0.3.9/odd_collector_sdk/job.py`

 * *Files identical despite different names*

### Comparing `odd-collector-sdk-0.3.8/pyproject.toml` & `odd_collector_sdk-0.3.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odd-collector-sdk"
-version = "0.3.8"
+version = "0.3.9"
 description = "ODD Collector"
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/opendatadiscovery/odd-collector-sdk"
 repository = "https://github.com/opendatadiscovery/odd-collector-sdk"
 keywords = ["odd-collector-sdk", "odd_collector_sdk", "opendatadiscovery"]
 include = ["LICENSE"]
```

### Comparing `odd-collector-sdk-0.3.8/setup.py` & `odd_collector_sdk-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
  'odd-models>=2.0.0,<3.0.0',
  'pyaml-env>=1.1.5,<2.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'odd-collector-sdk',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'ODD Collector',
     'long_description': '[![PyPI version](https://badge.fury.io/py/odd-collector-sdk.svg)](https://badge.fury.io/py/odd-collector-sdk)\n\n# ODD Collector SDK\nRoot project for ODD collectors\n\n### Domain\n* `CollectorConfig`\n\n    _Main config file for collector_\n    ``` python\n    class CollectorConfig(pydantic.BaseSettings):\n        default_pulling_interval: int # pulling interval in minutes\n        token: str                    # token for requests to odd-platform\n        plugins: Any\n        platform_host_url: str\n    ```\n\n* `Collector`\n\n    Args:\n\n    `config_path`: str - path to collector_config.yaml (i.e. `\'/collector_config.yaml\'`)\n\n    `root_package`: str - root package for adapters which will be loaded (i.e. `\'my_collector.adapters\'`)\n\n    `plugins_union_type` - Type variable for pydantic model.\n\n* `Plugin`\n\n  Is a config for adapter\n  ```python\n  class Plugin(pydantic.BaseSettings):\n    name: str\n    description: Optional[str] = None\n    namespace: Optional[str] = None\n  ```\n\n  Plugin class inherited from Pydantic\'s BaseSetting,it means it can take any field, which was skipped in `collector_config.yaml`, from env variables.\n\n  Field `type: Literal["custom_adapter"]`  is obligatory for each plugin, by convention literal **MUST** have same name with adapter package\n\n  Plugins example:\n  ```python\n    # plugins.py\n    class AwsPlugin(Plugin):\n        aws_secret_access_key: str\n        aws_access_key_id: str\n        aws_region: str\n    \n    class S3Plugin(AwsPlugin):\n        type: Literal["s3"]\n        buckets: Optional[List[str]] = []\n\n    class GluePlugin(AwsPlugin):\n        type: Literal["glue"]\n    \n    # For Collector\'s plugins_union_type argument\n    AvailablePlugin = Annotated[\n        Union[\n            GluePlugin,\n            S3Plugin,\n        ],\n        pydantic.Field(discriminator="type"),\n    ]\n  ```\n* AbstractAdapter\n    Abstract adapter which **MUST** be implemented by generic adapters\n\n## Collector example\n\n### Requirenments\nUse the package manager [poetry](https://python-poetry.org/) to install add odd-collector-sdk and asyncio.\n```bash\npoetry add odd-collector-sdk\n```\n\n### A typical top-level collector\'s directory layout (as an example we took poetry project)\n\n    .\n    ├── my_collector            \n    │   ├── adapters            # Adapters\n    │   │   ├── custom_adapter  # Some adapter package\n    │   │   │   ├── adapter.py  # Entry file for adapter\n    │   │   │   └── __init__.py\n    │   │   ├── other_custom_adapter\n    │   │   ├── ...             # Other adapters\n    │   │   └── __init__.py\n    │   ├── domain              # Domain models\n    │   │   ├── ...\n    │   │   ├── plugins.py      # Models for available plugins\n    │   │   └── __init__.py\n    │   ├── __init__.py         \n    │   └── __main__.py         # Entry file for collector\n    ├── ...\n    ├── collector_config.yaml\n    ├── pyproject.toml\n    ├── LICENSE\n    └── README.md\n\n\n\n### Adapters folder\nEach adapter inside adapters folder must have an `adapter.py` file with an `Adapter` class implementing `AbstractAdapter`\n```python\n    # custom_adapter/adapter.py example\n    from odd_collector_sdk.domain.adapter import AbstractAdapter\n    from odd_models.models import DataEntityList\n\n    # \n    class Adapter(AbstractAdapter):\n        def __init__(self, config: any) -> None:\n            super().__init__()\n\n        def get_data_entity_list(self) -> DataEntityList:\n            return DataEntityList(data_source_oddrn="test")\n\n        def get_data_source_oddrn(self) -> str:\n            return "oddrn"\n```\n\n### Plugins\nEach plugin must implement `Plugin` class from sdk\n```python\n    # domain/plugins.py\n    from typing import Literal, Union\n    from typing_extensions import Annotated\n\n    import pydantic\n    from odd_collector_sdk.domain.plugin import Plugin\n\n    class CustomPlugin(Plugin):\n        type: Literal["custom_adapter"]\n\n\n    class OtherCustomPlugin(Plugin):\n        type: Literal["other_custom_adapter"]\n\n    # Needs this type variable for Collector initialization\n    AvailablePlugins = Annotated[\n        Union[CustomPlugin, OtherCustomPlugin],\n        pydantic.Field(discriminator="type"),\n    ]\n```\n\n### collector_config.yaml\n\n```yaml\ndefault_pulling_interval: 10 \ntoken: "" \nplatform_host_url: "http://localhost:8080" \nplugins:\n  - type: custom_adapter\n    name: custom_adapter_name\n  - type: other_custom_adapter\n    name: other_custom_adapter_name\n\n```\n\n## Usage\n```python\n# __main__.py\n\nimport asyncio\nimport logging\nfrom os import path\n\n\nfrom odd_collector_sdk.collector import Collector\n\n# Union type of avalable plugins\nfrom my_collector.domain.plugins import AvailablePlugins\n\nlogging.basicConfig(\n    level=logging.INFO, format="[%(asctime)s] %(levelname)s in %(module)s: %(message)s"\n)\n\ntry:\n    cur_dirname = path.dirname(path.realpath(__file__))\n    config_path = path.join(cur_dirname, "../collector_config.yaml")\n    root_package = "my_collector.adapters"\n\n    loop = asyncio.get_event_loop()\n\n    collector = Collector(config_path, root_package, AvailablePlugin)\n\n    loop.run_until_complete(collector.register_data_sources())\n\n    collector.start_polling()\n    loop.run_forever()\nexcept Exception as e:\n    logging.error(e, exc_info=True)\n    loop.stop()\n```\n\nAnd run\n```bash\npoetry run python -m my_collector\n```\n\n\n',
     'author': 'Open Data Discovery',
     'author_email': 'pypi@opendatadiscovery.org',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/opendatadiscovery/odd-collector-sdk',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `odd-collector-sdk-0.3.8/PKG-INFO` & `odd_collector_sdk-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: odd-collector-sdk
-Version: 0.3.8
+Version: 0.3.9
 Summary: ODD Collector
 Home-page: https://github.com/opendatadiscovery/odd-collector-sdk
 License: Apache-2.0
 Keywords: odd-collector-sdk,odd_collector_sdk,opendatadiscovery
 Author: Open Data Discovery
 Author-email: pypi@opendatadiscovery.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: APScheduler (>=3.8.1,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: black (==22.3.0)
 Requires-Dist: funcy (>=1.17,<2.0)
 Requires-Dist: importlib-metadata (>=5.1.0,<6.0.0)
 Requires-Dist: isort (>=5.11.4,<6.0.0)
 Requires-Dist: odd-models (>=2.0.0,<3.0.0)
```

