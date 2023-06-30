# Comparing `tmp/pydantic_settings-2.0b1.tar.gz` & `tmp/pydantic_settings-2.0b2.tar.gz`

## Comparing `pydantic_settings-2.0b1.tar` & `pydantic_settings-2.0b2.tar`

### file list

```diff
@@ -1,26 +1,32 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/Makefile
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/.github/FUNDING.yml
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/.github/workflows/ci.yml
--rw-r--r--   0        0        0    18908 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/docs/index.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/__init__.py
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/py.typed
--rw-r--r--   0        0        0    20920 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/sources.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/utils.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/version.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/all.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/linting.in
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/linting.txt
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/pyproject.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/testing.in
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/testing.txt
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/tests/conftest.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/tests/example_test_config.json
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/tests/test_docs.py
--rw-r--r--   0        0        0    46791 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/tests/test_settings.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/LICENSE
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/README.md
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pyproject.toml
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/PKG-INFO
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/Makefile
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/mkdocs.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/docs/favicon.png
+-rw-r--r--   0        0        0    20932 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/docs/index.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/docs/logo-white.svg
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/docs/extra/terminal.css
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/docs/extra/tweaks.css
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/docs/theme/main.html
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/pydantic_settings/__init__.py
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/pydantic_settings/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/pydantic_settings/py.typed
+-rw-r--r--   0        0        0    23767 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/pydantic_settings/sources.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/pydantic_settings/utils.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/pydantic_settings/version.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/requirements/all.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/requirements/linting.in
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/requirements/linting.txt
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/requirements/pyproject.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/requirements/testing.in
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/requirements/testing.txt
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/tests/conftest.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/tests/example_test_config.json
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/tests/test_docs.py
+-rw-r--r--   0        0        0    48656 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/tests/test_settings.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/LICENSE
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/README.md
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 pydantic_settings-2.0b2/PKG-INFO
```

### Comparing `pydantic_settings-2.0b1/.pre-commit-config.yaml` & `pydantic_settings-2.0b2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.3.0
   hooks:
   - id: check-yaml
+    args: ['--unsafe']
   - id: check-toml
   - id: end-of-file-fixer
   - id: trailing-whitespace
 
 - repo: local
   hooks:
   - id: lint
```

### Comparing `pydantic_settings-2.0b1/Makefile` & `pydantic_settings-2.0b2/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0b1/.github/workflows/ci.yml` & `pydantic_settings-2.0b2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0b1/docs/index.md` & `pydantic_settings-2.0b2/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,164 +14,229 @@
 ```py
 from typing import Any, Callable, Set
 
 from pydantic import (
     AliasChoices,
     AmqpDsn,
     BaseModel,
-    ConfigDict,
     Field,
     ImportString,
     PostgresDsn,
     RedisDsn,
 )
 
-from pydantic_settings import BaseSettings
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
 class SubModel(BaseModel):
     foo: str = 'bar'
     apple: int = 1
 
 
 class Settings(BaseSettings):
-    auth_key: str = Field(validation_alias='my_auth_key')
-    api_key: str = Field(validation_alias='my_api_key')
+    auth_key: str = Field(validation_alias='my_auth_key')  # (1)!
 
     redis_dsn: RedisDsn = Field(
         'redis://user:pass@localhost:6379/1',
-        validation_alias=AliasChoices('service_redis_dsn', 'redis_url'),
+        validation_alias=AliasChoices('service_redis_dsn', 'redis_url'),  # (2)!
     )
     pg_dsn: PostgresDsn = 'postgres://user:pass@localhost:5432/foobar'
     amqp_dsn: AmqpDsn = 'amqp://user:pass@localhost:5672/'
 
-    special_function: ImportString[Callable[[Any], Any]] = 'math.cos'
+    special_function: ImportString[Callable[[Any], Any]] = 'math.cos'  # (3)!
 
     # to override domains:
     # export my_prefix_domains='["foo.com", "bar.com"]'
     domains: Set[str] = set()
 
     # to override more_settings:
     # export my_prefix_more_settings='{"foo": "x", "apple": 1}'
     more_settings: SubModel = SubModel()
 
-    model_config = ConfigDict(env_prefix='my_prefix_')  # defaults to no prefix, i.e. ""
+    model_config = SettingsConfigDict(env_prefix='my_prefix_')  # (4)!
 
 
 print(Settings().model_dump())
 """
 {
     'auth_key': 'xxx',
-    'api_key': 'xxx',
     'redis_dsn': Url('redis://user:pass@localhost:6379/1'),
     'pg_dsn': Url('postgres://user:pass@localhost:5432/foobar'),
     'amqp_dsn': Url('amqp://user:pass@localhost:5672/'),
     'special_function': math.cos,
     'domains': set(),
     'more_settings': {'foo': 'bar', 'apple': 1},
 }
 """
 ```
 
-## Environment variable names
+1. The environment variable name is overridden using `validation_alias`. In this case, the environment variable
+   `my_auth_key` will be read instead of `auth_key`.
+
+    Check the [`Field` documentation](/usage/fields/) for more information.
+
+2. The `AliasChoices` class allows to have multiple environment variable names for a single field.
+   The first environment variable that is found will be used.
 
-The following rules are used to determine which environment variable(s) are read for a given field:
+    Check the [`AliasChoices`](/usage/fields/#aliaspath-and-aliaschoices) for more information.
 
-* By default, the environment variable name is built by concatenating the prefix and field name.
-  * For example, to override `special_function` above, you could use:
+3. The `ImportString` class allows to import an object from a string.
+   In this case, the environment variable `special_function` will be read and the function `math.cos` will be imported.
 
-          export my_prefix_special_function='foo.bar'
+4. The `env_prefix` config setting allows to set a prefix for all environment variables.
 
-  * Note : The default prefix is an empty string.
+    Check the [Environment variable names documentation](#environment-variable-names) for more information.
+
+## Environment variable names
 
-* Custom environment variable names can be set like:
-  * `Field(validation_alias=...)` (see `api_key` and `redis_dsn` above)
-* When specifying custom environment variable names, either a string, `AliasChoices`, `AliasPath` my be provided.
-  * `env_prefix` is not considered.
-  * When specifying a `AliasChoices`, order matters: the first detected value is used.
-  * For example, for `redis_dsn` above, `service_redis_dsn` would take precedence over `redis_url`.
+By default, the environment variable name is the same as the field name.
 
-Case-sensitivity can be turned on through the `model_config`:
+You can change the prefix for all environment variables by setting the `env_prefix` config setting,
+or via the `_env_prefix` keyword argument on instantiation:
 
 ```py
-from pydantic import ConfigDict
+from pydantic_settings import BaseSettings, SettingsConfigDict
+
+
+class Settings(BaseSettings):
+    model_config = SettingsConfigDict(env_prefix='my_prefix_')
+
+    auth_key: str = 'xxx'  # will be read from `my_prefix_auth_key`
+```
+
+!!! note
+    The default `env_prefix` is `''` (empty string).
+
+If you want to change the environment variable name for a single field, you can use an alias.
+
+There are two ways to do this:
+
+* Using `Field(alias=...)` (see `api_key` above)
+* Using `Field(validation_alias=...)` (see `auth_key` above)
+
+Check the [`Field` aliases documentation](/usage/fields#field-aliases) for more information about aliases.
+
+### Case-sensitivity
 
-from pydantic_settings import BaseSettings
+By default, environment variable names are case-insensitive.
+
+If you want to make environment variable names case-sensitive, you can set the `case_sensitive` config setting:
+
+```py
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
 class Settings(BaseSettings):
-    redis_host: str = 'localhost'
+    model_config = SettingsConfigDict(case_sensitive=True)
 
-    model_config = ConfigDict(case_sensitive=True)
+    redis_host: str = 'localhost'
 ```
 
 When `case_sensitive` is `True`, the environment variable names must match field names (optionally with a prefix),
-so in this example
-`redis_host` could only be modified via `export redis_host`. If you want to name environment variables
+so in this example `redis_host` could only be modified via `export redis_host`. If you want to name environment variables
 all upper-case, you should name attribute all upper-case too. You can still name environment variables anything
 you like through `Field(validation_alias=...)`.
 
-In Pydantic **v1** `case_sensitive` is `False` by default and all variable names are converted to lower-case internally.
-If you want to define upper-case variable names on nested models like `SubModel` you have to
-set `case_sensitive=True` to disable this behaviour.
+Case-sensitivity can also be set via the `_case_sensitive` keyword argument on instantiation.
+
+In case of nested models, the `case_sensitive` setting will be applied to all nested models.
+
+```py
+import os
+
+from pydantic import ValidationError
+
+from pydantic_settings import BaseSettings, SettingsConfigDict
+
+
+class RedisSettings(BaseSettings):
+    host: str
+    port: int
+
+
+class Settings(BaseSettings):
+    model_config = SettingsConfigDict(case_sensitive=True)
+
+    redis: RedisSettings
+
+
+os.environ['redis'] = '{"host": "localhost", "port": 6379}'
+print(Settings().model_dump())
+#> {'redis': {'host': 'localhost', 'port': 6379}}
+os.environ['redis'] = '{"HOST": "localhost", "port": 6379}'  # (1)!
+try:
+    Settings()
+except ValidationError as e:
+    print(e)
+    """
+    2 validation errors for RedisSettings
+    host
+      Field required [type=missing, input_value={'HOST': 'localhost', 'port': 6379}, input_type=dict]
+        For further information visit https://errors.pydantic.dev/2/v/missing
+    HOST
+      Extra inputs are not permitted [type=extra_forbidden, input_value='localhost', input_type=str]
+        For further information visit https://errors.pydantic.dev/2/v/extra_forbidden
+    """
+```
+
+1. Note that the `host` field is not found because the environment variable name is `HOST` (all upper-case).
 
 !!! note
     On Windows, Python's `os` module always treats environment variables as case-insensitive, so the
     `case_sensitive` config setting will have no effect - settings will always be updated ignoring case.
 
 ## Parsing environment variable values
 
-For most simple field types (such as `int`, `float`, `str`, etc.),
-the environment variable value is parsed the same way it would
-be if passed directly to the initialiser (as a string).
+For most simple field types (such as `int`, `float`, `str`, etc.), the environment variable value is parsed
+the same way it would be if passed directly to the initialiser (as a string).
 
-Complex types like `list`, `set`, `dict`, and sub-models are populated from the environment
-by treating the environment variable's value as a JSON-encoded string.
+Complex types like `list`, `set`, `dict`, and sub-models are populated from the environment by treating the
+environment variable's value as a JSON-encoded string.
 
 Another way to populate nested complex variables is to configure your model with the `env_nested_delimiter`
-config setting, then use an env variable with a name pointing to the nested module fields.
+config setting, then use an environment variable with a name pointing to the nested module fields.
 What it does is simply explodes your variable into nested models or dicts.
 So if you define a variable `FOO__BAR__BAZ=123` it will convert it into `FOO={'BAR': {'BAZ': 123}}`
 If you have multiple variables with the same structure they will be merged.
 
-With the following environment variables:
+As an example, given the following environment variables:
 ```bash
 # your environment
 export V0=0
 export SUB_MODEL='{"v1": "json-1", "v2": "json-2"}'
 export SUB_MODEL__V2=nested-2
 export SUB_MODEL__V3=3
 export SUB_MODEL__DEEP__V4=v4
 ```
 
-You could load a settings module thus:
+You could load them into the following settings model:
 
 ```py
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel
 
-from pydantic_settings import BaseSettings
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
 class DeepSubModel(BaseModel):
     v4: str
 
 
 class SubModel(BaseModel):
     v1: str
     v2: bytes
     v3: int
     deep: DeepSubModel
 
 
 class Settings(BaseSettings):
+    model_config = SettingsConfigDict(env_nested_delimiter='__')
+
     v0: str
     sub_model: SubModel
 
-    model_config = ConfigDict(env_nested_delimiter='__')
-
 
 print(Settings().model_dump())
 """
 {
     'v0': '0',
     'sub_model': {'v1': 'json-1', 'v2': b'nested-2', 'v3': 3, 'deep': {'v4': 'v4'}},
 }
@@ -230,45 +295,38 @@
 os.environ['numbers'] = '1,2,3'
 print(Settings().model_dump())
 #> {'numbers': [1, 2, 3]}
 ```
 
 ## Dotenv (.env) support
 
-!!! note
-    dotenv file parsing requires [python-dotenv](https://pypi.org/project/python-dotenv/) to be installed.
-    This can be done with either `pip install python-dotenv` or `pip install pydantic[dotenv]`.
-
 Dotenv files (generally named `.env`) are a common pattern that make it easy to use environment variables in a
 platform-independent manner.
 
-A dotenv file follows the same general principles of all environment variables,
-and looks something like:
+A dotenv file follows the same general principles of all environment variables, and it looks like this:
 
-```bash
+```bash title=".env"
 # ignore comment
 ENVIRONMENT="production"
 REDIS_ADDRESS=localhost:6379
 MEANING_OF_LIFE=42
 MY_VAR='Hello world'
 ```
 
 Once you have your `.env` file filled with variables, *pydantic* supports loading it in two ways:
 
-**1.** setting `env_file` (and `env_file_encoding` if you don't want the default encoding of your OS) on `model_config`
-in a `BaseSettings` class:
+1. Setting the `env_file` (and `env_file_encoding` if you don't want the default encoding of your OS) on `model_config`
+in the `BaseSettings` class:
 
 ```py test="skip" lint="skip"
 class Settings(BaseSettings):
-    ...
-
-    model_config = ConfigDict(env_file='.env', env_file_encoding = 'utf-8')
+    model_config = SettingsConfigDict(env_file='.env', env_file_encoding='utf-8')
 ```
 
-**2.** instantiating a `BaseSettings` derived class with the `_env_file` keyword argument
+2. Instantiating the `BaseSettings` derived class with the `_env_file` keyword argument
 (and the `_env_file_encoding` if needed):
 
 ```py test="skip" lint="skip"
 settings = Settings(_env_file='prod.env', _env_file_encoding='utf-8')
 ```
 
 In either case, the value of the passed argument can be any valid path or filename, either absolute or relative to the
@@ -282,28 +340,20 @@
 Even when using a dotenv file, *pydantic* will still read environment variables as well as the dotenv file,
 **environment variables will always take priority over values loaded from a dotenv file**.
 
 Passing a file path via the `_env_file` keyword argument on instantiation (method 2) will override
 the value (if any) set on the `model_config` class. If the above snippets were used in conjunction, `prod.env` would be loaded
 while `.env` would be ignored.
 
-If you need to load multiple dotenv files, you can pass the file paths as a `list` or `tuple`.
-
-Later files in the list/tuple will take priority over earlier files.
-
-```py
-from pydantic import ConfigDict
-
-from pydantic_settings import BaseSettings
-
+If you need to load multiple dotenv files, you can pass multiple file paths as a tuple or list. The files will be
+loaded in order, with each file overriding the previous one.
 
+```py test="skip" lint="skip"
 class Settings(BaseSettings):
-    ...
-
-    model_config = ConfigDict(
+    model_config = SettingsConfigDict(
         # `.env.prod` takes priority over `.env`
         env_file=('.env', '.env.prod')
     )
 ```
 
 You can also use the keyword argument override to tell Pydantic not to load any file at all (even if one is set in
 the `model_config` class) by passing `None` as the instantiation keyword argument, e.g. `settings = Settings(_env_file=None)`.
@@ -312,39 +362,37 @@
 (depending on your OS and environment) may allow your dotenv file to also be used with `source`,
 see [python-dotenv's documentation](https://saurabh-kumar.com/python-dotenv/#usages) for more details.
 
 Pydantic settings consider `extra` config in case of dotenv file. It means if you set the `extra=forbid`
 on `model_config` and your dotenv file contains an entry for a field that is not defined in settings model,
 it will raise `ValidationError` in settings construction.
 
-## Secret Support
+## Secrets
 
 Placing secret values in files is a common pattern to provide sensitive configuration to an application.
 
 A secret file follows the same principal as a dotenv file except it only contains a single value and the file name
 is used as the key. A secret file will look like the following:
 
-`/var/run/database_password`:
-```
+``` title="/var/run/database_password"
 super_secret_database_password
 ```
 
 Once you have your secret files, *pydantic* supports loading it in two ways:
 
-**1.** setting `secrets_dir` on `model_config` in a `BaseSettings` class to the directory where your secret files are stored:
+1. Setting the `secrets_dir` on `model_config` in a `BaseSettings` class to the directory where your secret files are stored.
 
 ```py test="skip" lint="skip"
 class Settings(BaseSettings):
-    ...
-    database_password: str
+    model_config = SettingsConfigDict(secrets_dir='/var/run')
 
-    model_config = ConfigDict(secrets_dir='/var/run')
+    database_password: str
 ```
 
-**2.** instantiating a `BaseSettings` derived class with the `_secrets_dir` keyword argument:
+2. Instantiating the `BaseSettings` derived class with the `_secrets_dir` keyword argument:
 
 ```py test="skip" lint="skip"
 settings = Settings(_secrets_dir='/var/run')
 ```
 
 In either case, the value of the passed argument can be any valid directory, either absolute or relative to the
 current working directory. **Note that a non existent directory will only generate a warning**.
@@ -359,24 +407,26 @@
 ### Use Case: Docker Secrets
 
 Docker Secrets can be used to provide sensitive configuration to an application running in a Docker container.
 To use these secrets in a *pydantic* application the process is simple. More information regarding creating, managing
 and using secrets in Docker see the official
 [Docker documentation](https://docs.docker.com/engine/reference/commandline/secret/).
 
-First, define your Settings
+First, define your `Settings` class with a `SettingsConfigDict` that specifies the secrets directory.
+
 ```py test="skip" lint="skip"
 class Settings(BaseSettings):
-    my_secret_data: str
+    model_config = SettingsConfigDict(secrets_dir='/run/secrets')
 
-    model_config = ConfigDict(secrets_dir='/run/secrets')
+    my_secret_data: str
 ```
+
 !!! note
-    By default Docker uses `/run/secrets` as the target mount point. If you want to use a different location, change
-    `Config.secrets_dir` accordingly.
+    By default [Docker uses `/run/secrets`](https://docs.docker.com/engine/swarm/secrets/#how-docker-manages-secrets)
+    as the target mount point. If you want to use a different location, change `Config.secrets_dir` accordingly.
 
 Then, create your secret via the Docker CLI
 ```bash
 printf "This is a secret" | docker secret create my_secret_data -
 ```
 
 Last, run your application inside a Docker container and supply your newly created secret
@@ -444,18 +494,21 @@
 need to add your own custom sources, `settings_customise_sources` makes this very easy:
 
 ```py
 import json
 from pathlib import Path
 from typing import Any, Dict, Tuple, Type
 
-from pydantic import ConfigDict
 from pydantic.fields import FieldInfo
 
-from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
+from pydantic_settings import (
+    BaseSettings,
+    PydanticBaseSettingsSource,
+    SettingsConfigDict,
+)
 
 
 class JsonConfigSettingsSource(PydanticBaseSettingsSource):
     """
     A simple settings source class that loads variables from a JSON file
     at the project's root.
 
@@ -491,17 +544,17 @@
             if field_value is not None:
                 d[field_key] = field_value
 
         return d
 
 
 class Settings(BaseSettings):
-    foobar: str
+    model_config = SettingsConfigDict(env_file_encoding='utf-8')
 
-    model_config = ConfigDict(env_file_encoding='utf-8')
+    foobar: str
 
     @classmethod
     def settings_customise_sources(
         cls,
         settings_cls: Type[BaseSettings],
         init_settings: PydanticBaseSettingsSource,
         env_settings: PydanticBaseSettingsSource,
```

### Comparing `pydantic_settings-2.0b1/pydantic_settings/sources.py` & `pydantic_settings-2.0b2/pydantic_settings/sources.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,33 @@
 import warnings
 from abc import ABC, abstractmethod
 from collections import deque
 from dataclasses import is_dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, List, Mapping, Sequence, Tuple, Union, cast
 
-from pydantic import AliasChoices, AliasPath, BaseModel
+from pydantic import AliasChoices, AliasPath, BaseModel, Json
 from pydantic._internal._typing_extra import origin_is_union
 from pydantic._internal._utils import deep_update, lenient_issubclass
 from pydantic.fields import FieldInfo
 from typing_extensions import get_origin
 
 from pydantic_settings.utils import path_type_label
 
 if TYPE_CHECKING:
     from pydantic_settings.main import BaseSettings
 
 
 DotenvType = Union[Path, List[Path], Tuple[Path, ...]]
 
+# This is used as default value for `_env_file` in the `BaseSettings` class and
+# `env_file` in `DotEnvSettingsSource` so the default can be distinguished from `None`.
+# See the docstring of `BaseSettings` for more details.
+ENV_FILE_SENTINEL: DotenvType = Path('')
+
 
 class SettingsError(ValueError):
     pass
 
 
 class PydanticBaseSettingsSource(ABC):
     """
@@ -41,57 +46,61 @@
     def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
         """
         Gets the value, the key for model creation, and a flag to determine whether value is complex.
 
         This is an abstract method that should be overrided in every settings source classes.
 
         Args:
-            field (FieldInfo): The field.
-            field_name (str): The field name.
+            field: The field.
+            field_name: The field name.
 
         Returns:
-            tuple[str, Any, bool]: The key, value and a flag to determine whether value is complex.
+            A tuple contains the key, value and a flag to determine whether value is complex.
         """
         pass
 
     def field_is_complex(self, field: FieldInfo) -> bool:
         """
         Checks whether a field is complex, in which case it will attempt to be parsed as JSON.
 
         Args:
-            field (FieldInfo): The field.
+            field: The field.
 
         Returns:
-            bool: Whether the field is complex.
+            Whether the field is complex.
         """
-        return _annotation_is_complex(field.annotation)
+        return _annotation_is_complex(field.annotation, field.metadata)
 
     def prepare_field_value(self, field_name: str, field: FieldInfo, value: Any, value_is_complex: bool) -> Any:
         """
         Prepares the value of a field.
 
         Args:
-            field_name (str): The field name.
-            field (FieldInfo): The field.
-            value (Any): The value of the field that has to be prepared.
+            field_name: The field name.
+            field: The field.
+            value: The value of the field that has to be prepared.
             value_is_complex: A flag to determine whether value is complex.
 
         Returns:
-            Any: The prepared value.
+            The prepared value.
         """
         if self.field_is_complex(field) or value_is_complex:
             return json.loads(value)
         return value
 
     @abstractmethod
     def __call__(self) -> dict[str, Any]:
         pass
 
 
 class InitSettingsSource(PydanticBaseSettingsSource):
+    """
+    Source class for loading values provided during settings class initialization.
+    """
+
     def __init__(self, settings_cls: type[BaseSettings], init_kwargs: dict[str, Any]):
         self.init_kwargs = init_kwargs
         super().__init__(settings_cls)
 
     def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
         # Nothing to do here. Only implement the return statement to make mypy happy
         return None, '', False
@@ -100,16 +109,23 @@
         return self.init_kwargs
 
     def __repr__(self) -> str:
         return f'InitSettingsSource(init_kwargs={self.init_kwargs!r})'
 
 
 class PydanticBaseEnvSettingsSource(PydanticBaseSettingsSource):
+    def __init__(
+        self, settings_cls: type[BaseSettings], case_sensitive: bool | None = None, env_prefix: str | None = None
+    ) -> None:
+        super().__init__(settings_cls)
+        self.case_sensitive = case_sensitive if case_sensitive is not None else False
+        self.env_prefix = env_prefix if env_prefix is not None else ''
+
     def _apply_case_sensitive(self, value: str) -> str:
-        return value.lower() if not self.config.get('case_sensitive') else value
+        return value.lower() if not self.case_sensitive else value
 
     def _extract_field_info(self, field: FieldInfo, field_name: str) -> list[tuple[str, str, bool]]:
         """
         Extracts field info. This info is used to get the value of field from environment variables.
 
         It returns a list of tuples, each tuple contains:
             * field_key: The key of field that has to be used in model creation.
@@ -139,17 +155,15 @@
                         first_arg = cast(str, alias[0])  # first item of an AliasChoices must be a str
                         field_info.append(
                             (first_arg, self._apply_case_sensitive(first_arg), True if len(alias) > 1 else False)
                         )
             else:  # string validation alias
                 field_info.append((v_alias, self._apply_case_sensitive(v_alias), False))
         else:
-            field_info.append(
-                (field_name, self._apply_case_sensitive(self.config.get('env_prefix', '') + field_name), False)
-            )
+            field_info.append((field_name, self._apply_case_sensitive(self.env_prefix + field_name), False))
 
         return field_info
 
     def _replace_field_names_case_insensitively(self, field: FieldInfo, field_values: dict[str, Any]) -> dict[str, Any]:
         """
         Replace field names in values dict by looking in models fields insensitively.
 
@@ -223,26 +237,36 @@
                 field_value = self.prepare_field_value(field_name, field, field_value, value_is_complex)
             except ValueError as e:
                 raise SettingsError(
                     f'error parsing value for field "{field_name}" from source "{self.__class__.__name__}"'
                 ) from e
 
             if field_value is not None:
-                if not self.config.get('case_sensitive', False) and lenient_issubclass(field.annotation, BaseModel):
+                if not self.case_sensitive and lenient_issubclass(field.annotation, BaseModel):
                     data[field_key] = self._replace_field_names_case_insensitively(field, field_value)
                 else:
                     data[field_key] = field_value
 
         return data
 
 
 class SecretsSettingsSource(PydanticBaseEnvSettingsSource):
-    def __init__(self, settings_cls: type[BaseSettings], secrets_dir: str | Path | None):
-        self.secrets_dir = secrets_dir
-        super().__init__(settings_cls)
+    """
+    Source class for loading settings values from secret files.
+    """
+
+    def __init__(
+        self,
+        settings_cls: type[BaseSettings],
+        secrets_dir: str | Path | None = None,
+        case_sensitive: bool | None = None,
+        env_prefix: str | None = None,
+    ) -> None:
+        super().__init__(settings_cls, case_sensitive, env_prefix)
+        self.secrets_dir = secrets_dir if secrets_dir is not None else self.config.get('secrets_dir')
 
     def __call__(self) -> dict[str, Any]:
         """
         Build fields from "secrets" files.
         """
         secrets: dict[str, str | None] = {}
 
@@ -260,27 +284,45 @@
 
         return super().__call__()
 
     @classmethod
     def find_case_path(cls, dir_path: Path, file_name: str, case_sensitive: bool) -> Path | None:
         """
         Find a file within path's directory matching filename, optionally ignoring case.
+
+        Args:
+            dir_path: Directory path.
+            file_name: File name.
+            case_sensitive: Whether to search for file name case sensitively.
+
+        Returns:
+            Whether file path or `None` if file does not exist in directory.
         """
         for f in dir_path.iterdir():
             if f.name == file_name:
                 return f
             elif not case_sensitive and f.name.lower() == file_name.lower():
                 return f
         return None
 
     def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
+        """
+        Gets the value for field from secret file and a flag to determine whether value is complex.
+
+        Args:
+            field: The field.
+            field_name: The field name.
+
+        Returns:
+            A tuple contains the key, value if the file exists otherwise `None`, and
+                a flag to determine whether value is complex.
+        """
+
         for field_key, env_name, value_is_complex in self._extract_field_info(field, field_name):
-            path = self.find_case_path(
-                self.secrets_path, env_name, self.settings_cls.model_config.get('case_sensitive', False)
-            )
+            path = self.find_case_path(self.secrets_path, env_name, self.case_sensitive)
             if not path:
                 # path does not exist, we curently don't return a warning for this
                 continue
 
             if path.is_file():
                 return path.read_text().strip(), field_key, value_is_complex
             else:
@@ -292,42 +334,76 @@
         return None, field_key, value_is_complex
 
     def __repr__(self) -> str:
         return f'SecretsSettingsSource(secrets_dir={self.secrets_dir!r})'
 
 
 class EnvSettingsSource(PydanticBaseEnvSettingsSource):
+    """
+    Source class for loading settings values from environment variables.
+    """
+
     def __init__(
         self,
         settings_cls: type[BaseSettings],
+        case_sensitive: bool | None = None,
+        env_prefix: str | None = None,
         env_nested_delimiter: str | None = None,
-        env_prefix_len: int = 0,
-    ):
-        super().__init__(settings_cls)
-
-        self.env_nested_delimiter: str | None = env_nested_delimiter
-        self.env_prefix_len: int = env_prefix_len
+    ) -> None:
+        super().__init__(settings_cls, case_sensitive, env_prefix)
+        self.env_nested_delimiter = (
+            env_nested_delimiter if env_nested_delimiter is not None else self.config.get('env_nested_delimiter')
+        )
+        self.env_prefix_len = len(self.env_prefix)
 
-        self.env_vars: Mapping[str, str | None] = self._load_env_vars()
+        self.env_vars = self._load_env_vars()
 
     def _load_env_vars(self) -> Mapping[str, str | None]:
-        if self.settings_cls.model_config.get('case_sensitive'):
+        if self.case_sensitive:
             return os.environ
         return {k.lower(): v for k, v in os.environ.items()}
 
     def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
+        """
+        Gets the value for field from environment variables and a flag to determine whether value is complex.
+
+        Args:
+            field: The field.
+            field_name: The field name.
+
+        Returns:
+            A tuple contains the key, value if the file exists otherwise `None`, and
+                a flag to determine whether value is complex.
+        """
+
         env_val: str | None = None
         for field_key, env_name, value_is_complex in self._extract_field_info(field, field_name):
             env_val = self.env_vars.get(env_name)
             if env_val is not None:
                 break
 
         return env_val, field_key, value_is_complex
 
     def prepare_field_value(self, field_name: str, field: FieldInfo, value: Any, value_is_complex: bool) -> Any:
+        """
+        Prepare value for the field.
+
+        * Extract value for nested field.
+        * Deserialize value to python object for complex field.
+
+        Args:
+            field: The field.
+            field_name: The field name.
+
+        Returns:
+            A tuple contains prepared value for the field.
+
+        Raises:
+            ValuesError: When There is an error in deserializing value for complex field.
+        """
         is_complex, allow_parse_failure = self._field_is_complex(field)
         if is_complex or value_is_complex:
             if value is None:
                 # field is complex but no value found so far, try explode_env_vars
                 env_val_built = self.explode_env_vars(field_name, field, self.env_vars)
                 if env_val_built:
                     return env_val_built
@@ -378,28 +454,43 @@
             class Cfg(BaseSettings):
                 sub_model: SubModel
             ```
 
         Then:
             next_field(sub_model, 'vals') Returns the `vals` field of `SubModel` class
             next_field(sub_model, 'sub_sub_model') Returns `sub_sub_model` field of `SubModel` class
+
+        Args:
+            field: The field.
+            key: The key (env name).
+
+        Returns:
+            Field if it finds the next field otherwise `None`.
         """
         if not field or origin_is_union(get_origin(field.annotation)):
             # no support for Unions of complex BaseSettings fields
             return None
         elif field.annotation and hasattr(field.annotation, 'model_fields') and field.annotation.model_fields.get(key):
             return field.annotation.model_fields[key]
 
         return None
 
     def explode_env_vars(self, field_name: str, field: FieldInfo, env_vars: Mapping[str, str | None]) -> dict[str, Any]:
         """
         Process env_vars and extract the values of keys containing env_nested_delimiter into nested dictionaries.
 
         This is applied to a single field, hence filtering by env_var prefix.
+
+        Args:
+            field_name: The field name.
+            field: The field.
+            env_vars: Environment variables.
+
+        Returns:
+            A dictionaty contains extracted values from nested env values.
         """
         prefixes = [
             f'{env_name}{self.env_nested_delimiter}' for _, env_name, _ in self._extract_field_info(field, field_name)
         ]
         result: dict[str, Any] = {}
         for env_name, env_val in env_vars.items():
             if not any(env_name.startswith(prefix) for prefix in prefixes):
@@ -433,29 +524,35 @@
         return (
             f'EnvSettingsSource(env_nested_delimiter={self.env_nested_delimiter!r}, '
             f'env_prefix_len={self.env_prefix_len!r})'
         )
 
 
 class DotEnvSettingsSource(EnvSettingsSource):
+    """
+    Source class for loading settings values from env files.
+    """
+
     def __init__(
         self,
         settings_cls: type[BaseSettings],
-        env_file: DotenvType | None,
-        env_file_encoding: str | None,
+        env_file: DotenvType | None = ENV_FILE_SENTINEL,
+        env_file_encoding: str | None = None,
+        case_sensitive: bool | None = None,
+        env_prefix: str | None = None,
         env_nested_delimiter: str | None = None,
-        env_prefix_len: int = 0,
-    ):
-        self.env_file: DotenvType | None = env_file
-        self.env_file_encoding: str | None = env_file_encoding
-
-        super().__init__(settings_cls, env_nested_delimiter, env_prefix_len)
+    ) -> None:
+        self.env_file = env_file if env_file != ENV_FILE_SENTINEL else settings_cls.model_config.get('env_file')
+        self.env_file_encoding = (
+            env_file_encoding if env_file_encoding is not None else settings_cls.model_config.get('env_file_encoding')
+        )
+        super().__init__(settings_cls, case_sensitive, env_prefix, env_nested_delimiter)
 
     def _load_env_vars(self) -> Mapping[str, str | None]:
-        return self._read_env_files(self.settings_cls.model_config.get('case_sensitive', False))
+        return self._read_env_files(self.case_sensitive)
 
     def _read_env_files(self, case_sensitive: bool) -> Mapping[str, str | None]:
         env_files = self.env_file
         if env_files is None:
             return {}
 
         if isinstance(env_files, (str, os.PathLike)):
@@ -471,15 +568,15 @@
 
         return dotenv_vars
 
     def __call__(self) -> dict[str, Any]:
         data: dict[str, Any] = super().__call__()
 
         data_lower_keys: list[str] = []
-        if not self.settings_cls.model_config.get('case_sensitive', False):
+        if not self.case_sensitive:
             data_lower_keys = [x.lower() for x in data.keys()]
 
         # As `extra` config is allowed in dotenv settings source, We have to
         # update data with extra env variabels from dotenv file.
         for env_name, env_value in self.env_vars.items():
             if env_value is not None:
                 env_name_without_prefix = env_name[self.env_prefix_len :]
@@ -510,27 +607,17 @@
     file_vars: dict[str, str | None] = dotenv_values(file_path, encoding=encoding or 'utf8')
     if not case_sensitive:
         return {k.lower(): v for k, v in file_vars.items()}
     else:
         return file_vars
 
 
-def find_case_path(dir_path: Path, file_name: str, case_sensitive: bool) -> Path | None:
-    """
-    Find a file within path's directory matching filename, optionally ignoring case.
-    """
-    for f in dir_path.iterdir():
-        if f.name == file_name:
-            return f
-        elif not case_sensitive and f.name.lower() == file_name.lower():
-            return f
-    return None
-
-
-def _annotation_is_complex(annotation: type[Any] | None) -> bool:
+def _annotation_is_complex(annotation: type[Any] | None, metadata: list[Any]) -> bool:
+    if any(isinstance(md, Json) for md in metadata):  # type: ignore[misc]
+        return False
     origin = get_origin(annotation)
     return (
         _annotation_is_complex_inner(annotation)
         or _annotation_is_complex_inner(origin)
         or hasattr(origin, '__pydantic_core_schema__')
         or hasattr(origin, '__get_pydantic_core_schema__')
     )
```

### Comparing `pydantic_settings-2.0b1/pydantic_settings/utils.py` & `pydantic_settings-2.0b2/pydantic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0b1/requirements/linting.txt` & `pydantic_settings-2.0b2/requirements/linting.txt`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0b1/requirements/testing.txt` & `pydantic_settings-2.0b2/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0b1/tests/conftest.py` & `pydantic_settings-2.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0b1/tests/test_docs.py` & `pydantic_settings-2.0b2/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0b1/tests/test_settings.py` & `pydantic_settings-2.0b2/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pydantic import (
     AliasChoices,
     AliasPath,
     BaseModel,
     ConfigDict,
     Field,
     HttpUrl,
+    Json,
     SecretStr,
     ValidationError,
 )
 from pydantic import (
     dataclasses as pydantic_dataclasses,
 )
 from pydantic.fields import FieldInfo
@@ -1626,7 +1627,74 @@
     # pydantic-settings default
     with pytest.raises(
         NameError, match='Field "settings_prefixed_field" has conflict with protected namespace "settings_"'
     ):
 
         class Model1(BaseSettings):
             settings_prefixed_field: str
+
+
+def test_case_sensitive_from_args(monkeypatch):
+    class Settings(BaseSettings):
+        foo: str
+
+    # Need to patch os.environ to get build to work on Windows, where os.environ is case insensitive
+    monkeypatch.setattr(os, 'environ', value={'Foo': 'foo'})
+    with pytest.raises(ValidationError) as exc_info:
+        Settings(_case_sensitive=True)
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'missing', 'loc': ('foo',), 'msg': 'Field required', 'input': {}}
+    ]
+
+
+def test_env_prefix_from_args(env):
+    class Settings(BaseSettings):
+        apple: str
+
+    env.set('foobar_apple', 'has_prefix')
+    s = Settings(_env_prefix='foobar_')
+    assert s.apple == 'has_prefix'
+
+
+def test_env_json_field(env):
+    class Settings(BaseSettings):
+        x: Json
+
+    env.set('x', '{"foo": "bar"}')
+
+    s = Settings()
+    assert s.x == {'foo': 'bar'}
+
+    env.set('x', 'test')
+    with pytest.raises(ValidationError) as exc_info:
+        Settings()
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'json_invalid',
+            'loc': ('x',),
+            'msg': 'Invalid JSON: expected ident at line 1 column 2',
+            'input': 'test',
+            'ctx': {'error': 'expected ident at line 1 column 2'},
+        }
+    ]
+
+
+def test_env_json_field_dict(env):
+    class Settings(BaseSettings):
+        x: Json[Dict[str, int]]
+
+    env.set('x', '{"foo": 1}')
+
+    s = Settings()
+    assert s.x == {'foo': 1}
+
+    env.set('x', '{"foo": "bar"}')
+    with pytest.raises(ValidationError) as exc_info:
+        Settings()
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'int_parsing',
+            'loc': ('x', 'foo'),
+            'msg': 'Input should be a valid integer, unable to parse string as an integer',
+            'input': 'bar',
+        }
+    ]
```

### Comparing `pydantic_settings-2.0b1/LICENSE` & `pydantic_settings-2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0b1/README.md` & `pydantic_settings-2.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0b1/pyproject.toml` & `pydantic_settings-2.0b2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -36,25 +36,25 @@
     'Environment :: Console',
     'Environment :: MacOS X',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 requires-python = '>=3.7'
 dependencies = [
-    'pydantic>=2.0b1',
+    'pydantic>=2.0b3',
     'python-dotenv>=0.21.0',
 ]
 dynamic = ['version']
 
 [project.urls]
 Homepage = 'https://github.com/pydantic/pydantic-settings'
 Funding = 'https://github.com/sponsors/samuelcolvin'
 Source = 'https://github.com/pydantic/pydantic-settings'
 Changelog = 'https://github.com/pydantic/pydantic-settings/releases'
-# TODO: Documentation
+Documentation = 'https://docs.pydantic.dev/dev-v2/usage/pydantic_settings/'
 
 [tool.pytest.ini_options]
 testpaths = 'tests'
 filterwarnings = [
     'error',
     'ignore:This is a placeholder until pydantic-settings.*:UserWarning',
 ]
@@ -119,7 +119,12 @@
 # ansi2html and devtools are required to avoid the need to install these packages when running linting,
 # they're used in the docs build script
 [[tool.mypy.overrides]]
 module = [
     'dotenv.*',
 ]
 ignore_missing_imports = true
+
+# configuring https://github.com/pydantic/hooky
+[tool.hooky]
+reviewers = ['samuelcolvin', 'dmontagu', 'hramezani']
+require_change_file = false
```

### Comparing `pydantic_settings-2.0b1/PKG-INFO` & `pydantic_settings-2.0b2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pydantic-settings
-Version: 2.0b1
+Version: 2.0b2
 Summary: Settings management using Pydantic
 Project-URL: Homepage, https://github.com/pydantic/pydantic-settings
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic-settings
 Project-URL: Changelog, https://github.com/pydantic/pydantic-settings/releases
+Project-URL: Documentation, https://docs.pydantic.dev/dev-v2/usage/pydantic_settings/
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Framework :: Pydantic
@@ -27,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: pydantic>=2.0b1
+Requires-Dist: pydantic>=2.0b3
 Requires-Dist: python-dotenv>=0.21.0
 Description-Content-Type: text/markdown
 
 # pydantic-settings
 
 [![CI](https://github.com/pydantic/pydantic-settings/workflows/CI/badge.svg?event=push)](https://github.com/pydantic/pydantic-settings/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![Coverage](https://codecov.io/gh/pydantic/pydantic-settings/branch/main/graph/badge.svg)](https://codecov.io/gh/pydantic/pydantic-settings)
```

