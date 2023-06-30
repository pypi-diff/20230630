# Comparing `tmp/dbt-core-1.6.0b7.tar.gz` & `tmp/dbt-core-1.6.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.6.0b7.tar", last modified: Wed Jun 28 16:06:25 2023, max compression
+gzip compressed data, was "dbt-core-1.6.0b8.tar", last modified: Fri Jun 30 19:21:38 2023, max compression
```

## Comparing `dbt-core-1.6.0b7.tar` & `dbt-core-1.6.0b8.tar`

### file list

```diff
@@ -1,339 +1,343 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.930106 dbt-core-1.6.0b7/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-28 16:06:25.930106 dbt-core-1.6.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.898106 dbt-core-1.6.0b7/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.898106 dbt-core-1.6.0b7/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.898106 dbt-core-1.6.0b7/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    56679 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.898106 dbt-core-1.6.0b7/dbt/adapters/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/relation_configs/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/relation_configs/config_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/relation_configs/config_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.898106 dbt-core-1.6.0b7/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.902106 dbt-core-1.6.0b7/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.902106 dbt-core-1.6.0b7/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.902106 dbt-core-1.6.0b7/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    27182 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.902106 dbt-core-1.6.0b7/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    59722 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.906106 dbt-core-1.6.0b7/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.906106 dbt-core-1.6.0b7/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53414 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/node_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    53340 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/semantic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22434 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.906106 dbt-core-1.6.0b7/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.890106 dbt-core-1.6.0b7/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.906106 dbt-core-1.6.0b7/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.906106 dbt-core-1.6.0b7/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.910106 dbt-core-1.6.0b7/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    62526 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   115121 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    79375 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.910106 dbt-core-1.6.0b7/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.910106 dbt-core-1.6.0b7/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.910106 dbt-core-1.6.0b7/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.914106 dbt-core-1.6.0b7/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.890106 dbt-core-1.6.0b7/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.914106 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/drop_relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.914106 dbt-core-1.6.0b7/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.914106 dbt-core-1.6.0b7/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.914106 dbt-core-1.6.0b7/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.914106 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.890106 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.914106 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.914106 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.914106 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.918106 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.918106 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.918106 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.918106 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.918106 dbt-core-1.6.0b7/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.922106 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.890106 dbt-core-1.6.0b7/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.922106 dbt-core-1.6.0b7/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497953 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.922106 dbt-core-1.6.0b7/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.922106 dbt-core-1.6.0b7/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.922106 dbt-core-1.6.0b7/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.894106 dbt-core-1.6.0b7/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.922106 dbt-core-1.6.0b7/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.922106 dbt-core-1.6.0b7/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.922106 dbt-core-1.6.0b7/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.922106 dbt-core-1.6.0b7/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.926106 dbt-core-1.6.0b7/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    66330 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    48426 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/parser/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.926106 dbt-core-1.6.0b7/dbt/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/plugins/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/plugins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/plugins/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.926106 dbt-core-1.6.0b7/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.926106 dbt-core-1.6.0b7/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.930106 dbt-core-1.6.0b7/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:06:25.930106 dbt-core-1.6.0b7/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-28 16:06:25.000000 dbt-core-1.6.0b7/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-06-28 16:06:25.000000 dbt-core-1.6.0b7/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 16:06:25.000000 dbt-core-1.6.0b7/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-28 16:06:25.000000 dbt-core-1.6.0b7/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 16:06:25.000000 dbt-core-1.6.0b7/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-28 16:06:25.000000 dbt-core-1.6.0b7/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-28 16:06:25.000000 dbt-core-1.6.0b7/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 16:06:25.930106 dbt-core-1.6.0b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-28 16:06:13.000000 dbt-core-1.6.0b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.491028 dbt-core-1.6.0b8/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56679 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/adapters/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.499029 dbt-core-1.6.0b8/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.499029 dbt-core-1.6.0b8/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27182 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.499029 dbt-core-1.6.0b8/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60992 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55058 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/node_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53205 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/semantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22434 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62526 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115121 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79375 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30457 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/drop_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/clone/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/clone/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497953 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.523029 dbt-core-1.6.0b8/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68817 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48426 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.523029 dbt-core-1.6.0b8/dbt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/setup.py
```

### Comparing `dbt-core-1.6.0b7/PKG-INFO` & `dbt-core-1.6.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b7
+Version: 1.6.0b8
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b7 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b8 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b7/README.md` & `dbt-core-1.6.0b8/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/base/__init__.py` & `dbt-core-1.6.0b8/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/base/column.py` & `dbt-core-1.6.0b8/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/base/connections.py` & `dbt-core-1.6.0b8/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/base/impl.py` & `dbt-core-1.6.0b8/dbt/adapters/base/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/base/meta.py` & `dbt-core-1.6.0b8/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/base/plugin.py` & `dbt-core-1.6.0b8/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/base/query_headers.py` & `dbt-core-1.6.0b8/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/base/relation.py` & `dbt-core-1.6.0b8/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/cache.py` & `dbt-core-1.6.0b8/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/factory.py` & `dbt-core-1.6.0b8/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/protocol.py` & `dbt-core-1.6.0b8/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/reference_keys.py` & `dbt-core-1.6.0b8/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/relation_configs/config_base.py` & `dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/relation_configs/config_change.py` & `dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_change.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/relation_configs/config_validation.py` & `dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_validation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/sql/connections.py` & `dbt-core-1.6.0b8/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/adapters/sql/impl.py` & `dbt-core-1.6.0b8/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/cli/exceptions.py` & `dbt-core-1.6.0b8/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/cli/flags.py` & `dbt-core-1.6.0b8/dbt/cli/flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,15 @@
     e.g. fn("run") -> ["defer", "favor_state", "exclude", ...]
     """
     import dbt.cli.main as cli
 
     CMD_DICT: Dict[CliCommand, ClickCommand] = {
         CliCommand.BUILD: cli.build,
         CliCommand.CLEAN: cli.clean,
+        CliCommand.CLONE: cli.clone,
         CliCommand.COMPILE: cli.compile,
         CliCommand.DOCS_GENERATE: cli.docs_generate,
         CliCommand.DOCS_SERVE: cli.docs_serve,
         CliCommand.DEBUG: cli.debug,
         CliCommand.DEPS: cli.deps,
         CliCommand.INIT: cli.init,
         CliCommand.LIST: cli.list,
```

### Comparing `dbt-core-1.6.0b7/dbt/cli/main.py` & `dbt-core-1.6.0b8/dbt/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from dbt.contracts.results import (
     CatalogArtifact,
     RunExecutionResult,
 )
 from dbt.events.base_types import EventMsg
 from dbt.task.build import BuildTask
 from dbt.task.clean import CleanTask
+from dbt.task.clone import CloneTask
 from dbt.task.compile import CompileTask
 from dbt.task.debug import DebugTask
 from dbt.task.deps import DepsTask
 from dbt.task.freshness import FreshnessTask
 from dbt.task.generate import GenerateTask
 from dbt.task.init import InitTask
 from dbt.task.list import ListTask
@@ -600,14 +601,51 @@
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
     success = task.interpret_results(results)
+    return results, success
+
+
+# dbt clone
+@cli.command("clone")
+@click.pass_context
+@p.defer_state
+@p.exclude
+@p.full_refresh
+@p.profile
+@p.profiles_dir
+@p.project_dir
+@p.resource_type
+@p.select
+@p.selector
+@p.state  # required
+@p.target
+@p.target_path
+@p.threads
+@p.vars
+@p.version_check
+@requires.preflight
+@requires.profile
+@requires.project
+@requires.runtime_config
+@requires.manifest
+@requires.postflight
+def clone(ctx, **kwargs):
+    """Create clones of selected nodes based on their location in the manifest provided to --state."""
+    task = CloneTask(
+        ctx.obj["flags"],
+        ctx.obj["runtime_config"],
+        ctx.obj["manifest"],
+    )
+
+    results = task.run()
+    success = task.interpret_results(results)
     return results, success
 
 
 # dbt run operation
 @cli.command("run-operation")
 @click.pass_context
 @click.argument("macro")
```

### Comparing `dbt-core-1.6.0b7/dbt/cli/option_types.py` & `dbt-core-1.6.0b8/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/cli/options.py` & `dbt-core-1.6.0b8/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/cli/params.py` & `dbt-core-1.6.0b8/dbt/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/cli/requires.py` & `dbt-core-1.6.0b8/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/cli/resolvers.py` & `dbt-core-1.6.0b8/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/cli/types.py` & `dbt-core-1.6.0b8/dbt/cli/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dbt.exceptions import DbtInternalError
 
 
 class Command(Enum):
     BUILD = "build"
     CLEAN = "clean"
     COMPILE = "compile"
+    CLONE = "clone"
     DOCS_GENERATE = "generate"
     DOCS_SERVE = "serve"
     DEBUG = "debug"
     DEPS = "deps"
     INIT = "init"
     LIST = "list"
     PARSE = "parse"
```

### Comparing `dbt-core-1.6.0b7/dbt/clients/_jinja_blocks.py` & `dbt-core-1.6.0b8/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/clients/agate_helper.py` & `dbt-core-1.6.0b8/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/clients/git.py` & `dbt-core-1.6.0b8/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/clients/jinja.py` & `dbt-core-1.6.0b8/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/clients/jinja_static.py` & `dbt-core-1.6.0b8/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/clients/registry.py` & `dbt-core-1.6.0b8/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/clients/system.py` & `dbt-core-1.6.0b8/dbt/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/clients/yaml_helper.py` & `dbt-core-1.6.0b8/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/compilation.py` & `dbt-core-1.6.0b8/dbt/compilation.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,15 +177,14 @@
                 raise GraphDependencyNotFoundError(node, dependency)
 
     def link_graph(self, manifest: Manifest):
         for source in manifest.sources.values():
             self.add_node(source.unique_id)
         for semantic_model in manifest.semantic_models.values():
             self.add_node(semantic_model.unique_id)
-
         for node in manifest.nodes.values():
             self.link_node(node, manifest)
         for exposure in manifest.exposures.values():
             self.link_node(exposure, manifest)
         for metric in manifest.metrics.values():
             self.link_node(metric, manifest)
 
@@ -297,70 +296,14 @@
         return context
 
     def add_ephemeral_prefix(self, name: str):
         adapter = get_adapter(self.config)
         relation_cls = adapter.Relation
         return relation_cls.add_ephemeral_prefix(name)
 
-    def _inject_ctes_into_sql(self, sql: str, ctes: List[InjectedCTE]) -> str:
-        """
-        `ctes` is a list of InjectedCTEs like:
-
-            [
-                InjectedCTE(
-                    id="cte_id_1",
-                    sql="__dbt__cte__ephemeral as (select * from table)",
-                ),
-                InjectedCTE(
-                    id="cte_id_2",
-                    sql="__dbt__cte__events as (select id, type from events)",
-                ),
-            ]
-
-        Given `sql` like:
-
-          "with internal_cte as (select * from sessions)
-           select * from internal_cte"
-
-        This will spit out:
-
-          "with __dbt__cte__ephemeral as (select * from table),
-                __dbt__cte__events as (select id, type from events),
-                with internal_cte as (select * from sessions)
-           select * from internal_cte"
-
-        (Whitespace enhanced for readability.)
-        """
-        if len(ctes) == 0:
-            return sql
-
-        parsed_stmts = sqlparse.parse(sql)
-        parsed = parsed_stmts[0]
-
-        with_stmt = None
-        for token in parsed.tokens:
-            if token.is_keyword and token.normalized == "WITH":
-                with_stmt = token
-                break
-
-        if with_stmt is None:
-            # no with stmt, add one, and inject CTEs right at the beginning
-            first_token = parsed.token_first()
-            with_stmt = sqlparse.sql.Token(sqlparse.tokens.Keyword, "with")
-            parsed.insert_before(first_token, with_stmt)
-        else:
-            # stmt exists, add a comma (which will come after injected CTEs)
-            trailing_comma = sqlparse.sql.Token(sqlparse.tokens.Punctuation, ",")
-            parsed.insert_after(with_stmt, trailing_comma)
-
-        token = sqlparse.sql.Token(sqlparse.tokens.Keyword, ", ".join(c.sql for c in ctes))
-        parsed.insert_after(with_stmt, token)
-
-        return str(parsed)
-
     def _recursively_prepend_ctes(
         self,
         model: ManifestSQLNode,
         manifest: Manifest,
         extra_context: Optional[Dict[str, Any]],
     ) -> Tuple[ManifestSQLNode, List[InjectedCTE]]:
         """This method is called by the 'compile_node' method. Starting
@@ -427,15 +370,15 @@
 
             new_cte_name = self.add_ephemeral_prefix(cte_model.name)
             rendered_sql = cte_model._pre_injected_sql or cte_model.compiled_code
             sql = f" {new_cte_name} as (\n{rendered_sql}\n)"
 
             _add_prepended_cte(prepended_ctes, InjectedCTE(id=cte.id, sql=sql))
 
-        injected_sql = self._inject_ctes_into_sql(
+        injected_sql = inject_ctes_into_sql(
             model.compiled_code,
             prepended_ctes,
         )
         # Check again before updating for multi-threading
         if not model.extra_ctes_injected:
             model._pre_injected_sql = model.compiled_code
             model.compiled_code = injected_sql
@@ -578,7 +521,78 @@
         """
         node = self._compile_code(node, manifest, extra_context)
 
         node, _ = self._recursively_prepend_ctes(node, manifest, extra_context)
         if write:
             self._write_node(node)
         return node
+
+
+def inject_ctes_into_sql(sql: str, ctes: List[InjectedCTE]) -> str:
+    """
+    `ctes` is a list of InjectedCTEs like:
+
+        [
+            InjectedCTE(
+                id="cte_id_1",
+                sql="__dbt__cte__ephemeral as (select * from table)",
+            ),
+            InjectedCTE(
+                id="cte_id_2",
+                sql="__dbt__cte__events as (select id, type from events)",
+            ),
+        ]
+
+    Given `sql` like:
+
+      "with internal_cte as (select * from sessions)
+       select * from internal_cte"
+
+    This will spit out:
+
+      "with __dbt__cte__ephemeral as (select * from table),
+            __dbt__cte__events as (select id, type from events),
+            internal_cte as (select * from sessions)
+       select * from internal_cte"
+
+    (Whitespace enhanced for readability.)
+    """
+    if len(ctes) == 0:
+        return sql
+
+    parsed_stmts = sqlparse.parse(sql)
+    parsed = parsed_stmts[0]
+
+    with_stmt = None
+    for token in parsed.tokens:
+        if token.is_keyword and token.normalized == "WITH":
+            with_stmt = token
+        elif token.is_keyword and token.normalized == "RECURSIVE" and with_stmt is not None:
+            with_stmt = token
+            break
+        elif not token.is_whitespace and with_stmt is not None:
+            break
+
+    if with_stmt is None:
+        # no with stmt, add one, and inject CTEs right at the beginning
+        # [original_sql]
+        first_token = parsed.token_first()
+        with_token = sqlparse.sql.Token(sqlparse.tokens.Keyword, "with")
+        parsed.insert_before(first_token, with_token)
+        # [with][original_sql]
+        injected_ctes = ", ".join(c.sql for c in ctes) + " "
+        injected_ctes_token = sqlparse.sql.Token(sqlparse.tokens.Keyword, injected_ctes)
+        parsed.insert_after(with_token, injected_ctes_token)
+        # [with][joined_ctes][original_sql]
+    else:
+        # with stmt exists so we don't need to add one, but we do need to add a comma
+        # between the injected ctes and the original sql
+        # [with][original_sql]
+        injected_ctes = ", ".join(c.sql for c in ctes)
+        injected_ctes_token = sqlparse.sql.Token(sqlparse.tokens.Keyword, injected_ctes)
+        parsed.insert_after(with_stmt, injected_ctes_token)
+        # [with][joined_ctes][original_sql]
+        comma_token = sqlparse.sql.Token(sqlparse.tokens.Punctuation, ", ")
+        parsed.insert_after(injected_ctes_token, comma_token)
+        # [with][joined_ctes][, ][original_sql]
+
+    return str(parsed)
```

### Comparing `dbt-core-1.6.0b7/dbt/config/profile.py` & `dbt-core-1.6.0b8/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/config/project.py` & `dbt-core-1.6.0b8/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/config/renderer.py` & `dbt-core-1.6.0b8/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/config/runtime.py` & `dbt-core-1.6.0b8/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/config/selectors.py` & `dbt-core-1.6.0b8/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/config/utils.py` & `dbt-core-1.6.0b8/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/constants.py` & `dbt-core-1.6.0b8/dbt/constants.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/base.py` & `dbt-core-1.6.0b8/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/configured.py` & `dbt-core-1.6.0b8/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/context_config.py` & `dbt-core-1.6.0b8/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/docs.py` & `dbt-core-1.6.0b8/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/exceptions_jinja.py` & `dbt-core-1.6.0b8/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/macro_resolver.py` & `dbt-core-1.6.0b8/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/macros.py` & `dbt-core-1.6.0b8/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/manifest.py` & `dbt-core-1.6.0b8/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/providers.py` & `dbt-core-1.6.0b8/dbt/context/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1374,28 +1374,38 @@
         return [
             h.to_dict(omit_none=True) for h in self.model.config.post_hook  # type: ignore[union-attr] # noqa
         ]
 
     @contextproperty
     def sql(self) -> Optional[str]:
         # only doing this in sql model for backward compatible
-        if (
-            getattr(self.model, "extra_ctes_injected", None)
-            and self.model.language == ModelLanguage.sql  # type: ignore[union-attr]
-        ):
-            # TODO CT-211
-            return self.model.compiled_code  # type: ignore[union-attr]
-        return None
+        if self.model.language == ModelLanguage.sql:  # type: ignore[union-attr]
+            # If the model is deferred and the adapter doesn't support zero-copy cloning, then select * from the prod
+            # relation
+            if getattr(self.model, "defer_relation", None):
+                # TODO https://github.com/dbt-labs/dbt-core/issues/7976
+                return f"select * from {self.model.defer_relation.relation_name or str(self.defer_relation)}"  # type: ignore[union-attr]
+            elif getattr(self.model, "extra_ctes_injected", None):
+                # TODO CT-211
+                return self.model.compiled_code  # type: ignore[union-attr]
+            else:
+                return None
+        else:
+            return None
 
     @contextproperty
     def compiled_code(self) -> Optional[str]:
-        if getattr(self.model, "extra_ctes_injected", None):
+        if getattr(self.model, "defer_relation", None):
+            # TODO https://github.com/dbt-labs/dbt-core/issues/7976
+            return f"select * from {self.model.defer_relation.relation_name or str(self.defer_relation)}"  # type: ignore[union-attr]
+        elif getattr(self.model, "extra_ctes_injected", None):
             # TODO CT-211
             return self.model.compiled_code  # type: ignore[union-attr]
-        return None
+        else:
+            return None
 
     @contextproperty
     def database(self) -> str:
         return getattr(self.model, "database", self.config.credentials.database)
 
     @contextproperty
     def schema(self) -> str:
@@ -1432,14 +1442,28 @@
                 post-hook:
                   - "grant select on {{ this }} to db_reader"
         """
         if self.model.resource_type == NodeType.Operation:
             return None
         return self.db_wrapper.Relation.create_from(self.config, self.model)
 
+    @contextproperty
+    def defer_relation(self) -> Optional[RelationProxy]:
+        """
+        For commands which add information about this node's corresponding
+        production version (via a --state artifact), access the Relation
+        object for that stateful other
+        """
+        if getattr(self.model, "defer_relation", None):
+            return self.db_wrapper.Relation.create_from_node(
+                self.config, self.model.defer_relation  # type: ignore
+            )
+        else:
+            return None
+
 
 # This is called by '_context_for', used in 'render_with_context'
 def generate_parser_model_context(
     model: ManifestNode,
     config: RuntimeConfig,
     manifest: Manifest,
     context_config: ContextConfig,
```

### Comparing `dbt-core-1.6.0b7/dbt/context/secret.py` & `dbt-core-1.6.0b8/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/context/target.py` & `dbt-core-1.6.0b8/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/connection.py` & `dbt-core-1.6.0b8/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/files.py` & `dbt-core-1.6.0b8/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/graph/manifest.py` & `dbt-core-1.6.0b8/dbt/contracts/graph/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     GenericTestNode,
     GraphMemberNode,
     Group,
     Macro,
     ManifestNode,
     Metric,
     ModelNode,
-    RelationalNode,
+    DeferRelation,
     ResultNode,
     SemanticModel,
     SourceDefinition,
     UnpatchedSourceDefinition,
 )
 from dbt.contracts.graph.unparsed import SourcePatch, NodeVersion, UnparsedVersion
 from dbt.contracts.graph.manifest_upgrade import upgrade_manifest_json
@@ -46,26 +46,34 @@
 from dbt.dataclass_schema import dbtClassMixin
 from dbt.exceptions import (
     CompilationError,
     DuplicateResourceNameError,
     DuplicateMacroInPackageError,
     DuplicateMaterializationNameError,
     AmbiguousResourceNameRefError,
+    ParsingError,
 )
 from dbt.helper_types import PathSet
 from dbt.events.functions import fire_event
 from dbt.events.types import MergedFromState, UnpinnedRefNewVersionAvailable
 from dbt.events.contextvars import get_node_info
 from dbt.node_types import NodeType, AccessType
 from dbt.flags import get_flags, MP_CONTEXT
 from dbt import tracking
 import dbt.utils
 from dbt_semantic_interfaces.implementations.metric import PydanticMetric
 from dbt_semantic_interfaces.implementations.semantic_manifest import PydanticSemanticManifest
 from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
+from dbt_semantic_interfaces.implementations.project_configuration import (
+    PydanticProjectConfiguration,
+)
+from dbt_semantic_interfaces.implementations.time_spine_table_configuration import (
+    PydanticTimeSpineTableConfiguration,
+)
+from dbt_semantic_interfaces.type_enums import TimeGranularity
 
 NodeEdgeMap = Dict[str, List[str]]
 PackageName = str
 DocName = str
 RefName = str
 UniqueID = str
 
@@ -978,24 +986,48 @@
     def analysis_lookup(self) -> AnalysisLookup:
         if self._analysis_lookup is None:
             self._analysis_lookup = AnalysisLookup(self)
         return self._analysis_lookup
 
     @property
     def pydantic_semantic_manifest(self) -> PydanticSemanticManifest:
-        pydantic_semantic_manifest = PydanticSemanticManifest(metrics=[], semantic_models=[])
+        project_config = PydanticProjectConfiguration(
+            time_spine_table_configurations=[],
+        )
+        pydantic_semantic_manifest = PydanticSemanticManifest(
+            metrics=[], semantic_models=[], project_configuration=project_config
+        )
 
         for semantic_model in self.semantic_models.values():
             pydantic_semantic_manifest.semantic_models.append(
                 PydanticSemanticModel.parse_obj(semantic_model.to_dict())
             )
 
         for metric in self.metrics.values():
             pydantic_semantic_manifest.metrics.append(PydanticMetric.parse_obj(metric.to_dict()))
 
+        # Look for time-spine table model and create time spine table configuration
+        if self.semantic_models:
+            # Get model for time_spine_table
+            time_spine_model_name = "metricflow_time_spine"
+            model = self.ref_lookup.find(time_spine_model_name, None, None, self)
+            if not model:
+                raise ParsingError(
+                    "The semantic layer requires a 'metricflow_time_spine' model in the project, but none was found. Guidance on creating this model can be found on our docs site (https://docs.getdbt.com/docs/build/metricflow-time-spine)"
+                )
+            # Create time_spine_table_config, set it in project_config, and add to semantic manifest
+            time_spine_table_config = PydanticTimeSpineTableConfiguration(
+                location=model.relation_name,
+                column_name="date_day",
+                grain=TimeGranularity.DAY,
+            )
+            pydantic_semantic_manifest.project_configuration.time_spine_table_configurations = [
+                time_spine_table_config
+            ]
+
         return pydantic_semantic_manifest
 
     @property
     def external_node_unique_ids(self):
         return [node.unique_id for node in self.nodes.values() if node.is_external_node]
 
     def resolve_refs(
@@ -1214,16 +1246,18 @@
 
         Only non-ephemeral refable nodes are examined.
         """
         refables = set(NodeType.refable())
         for unique_id, node in other.nodes.items():
             current = self.nodes.get(unique_id)
             if current and (node.resource_type in refables and not node.is_ephemeral):
-                state_relation = RelationalNode(node.database, node.schema, node.alias)
-                self.nodes[unique_id] = current.replace(state_relation=state_relation)
+                defer_relation = DeferRelation(
+                    node.database, node.schema, node.alias, node.relation_name
+                )
+                self.nodes[unique_id] = current.replace(defer_relation=defer_relation)
 
     # Methods that were formerly in ParseResult
 
     def add_macro(self, source_file: SourceFile, macro: Macro):
         if macro.unique_id in self.macros:
             # detect that the macro exists and emit an error
             raise DuplicateMacroInPackageError(macro=macro, macro_mapping=self.macros)
@@ -1436,16 +1470,16 @@
             data = upgrade_manifest_json(data, manifest_schema_version)
         return cls.from_dict(data)
 
     def __post_serialize__(self, dct):
         for unique_id, node in dct["nodes"].items():
             if "config_call_dict" in node:
                 del node["config_call_dict"]
-            if "state_relation" in node:
-                del node["state_relation"]
+            if "defer_relation" in node:
+                del node["defer_relation"]
         return dct
 
 
 def get_manifest_schema_version(dct: dict) -> int:
     schema_version = dct.get("metadata", {}).get("dbt_schema_version", None)
     if not schema_version:
         raise ValueError("Manifest doesn't have schema version")
```

### Comparing `dbt-core-1.6.0b7/dbt/contracts/graph/manifest_upgrade.py` & `dbt-core-1.6.0b8/dbt/contracts/graph/manifest_upgrade.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/graph/metrics.py` & `dbt-core-1.6.0b8/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/graph/model_config.py` & `dbt-core-1.6.0b8/dbt/contracts/graph/model_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,20 +491,20 @@
                     f"Invalid color name for docs.node_color: {node_color}. "
                     "It is neither a valid HTML color name nor a valid HEX code."
                 )
 
         if (
             self.contract.enforced
             and self.materialized == "incremental"
-            and self.on_schema_change != "append_new_columns"
+            and self.on_schema_change not in ("append_new_columns", "fail")
         ):
             raise ValidationError(
                 f"Invalid value for on_schema_change: {self.on_schema_change}. Models "
                 "materialized as incremental with contracts enabled must set "
-                "on_schema_change to 'append_new_columns'"
+                "on_schema_change to 'append_new_columns' or 'fail'"
             )
 
     @classmethod
     def __pre_deserialize__(cls, data):
         data = super().__pre_deserialize__(data)
         field_map = {"post-hook": "post_hook", "pre-hook": "pre_hook"}
         # create a new dict because otherwise it gets overwritten in
```

### Comparing `dbt-core-1.6.0b7/dbt/contracts/graph/node_args.py` & `dbt-core-1.6.0b8/dbt/contracts/graph/node_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,13 +19,13 @@
     deprecation_date: Optional[datetime] = None
     access: Optional[str] = AccessType.Protected.value
     generated_at: datetime = field(default_factory=datetime.utcnow)
     depends_on_nodes: List[str] = field(default_factory=list)
     enabled: bool = True
 
     @property
-    def unique_id(self):
+    def unique_id(self) -> str:
         unique_id = f"{NodeType.Model}.{self.package_name}.{self.name}"
         if self.version:
-            unique_id = f"{unique_id}.{self.verison}"
+            unique_id = f"{unique_id}.{self.version}"
 
         return unique_id
```

### Comparing `dbt-core-1.6.0b7/dbt/contracts/graph/nodes.py` & `dbt-core-1.6.0b8/dbt/contracts/graph/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from dbt.exceptions import ParsingError, ContractBreakingChangeError
 from dbt.events.types import (
     SeedIncreased,
     SeedExceedsLimitSamePath,
     SeedExceedsLimitAndPathChanged,
     SeedExceedsLimitChecksumChanged,
 )
-from dbt.events.contextvars import set_contextvars
+from dbt.events.contextvars import set_log_contextvars
 from dbt.flags import get_flags
 from dbt.node_types import ModelLanguage, NodeType, AccessType
 from dbt_semantic_interfaces.references import (
     MeasureReference,
     LinkableElementReference,
     SemanticModelReference,
 )
@@ -254,16 +254,17 @@
     # 'in' on lists is O(n) so this is O(n^2) for # of macros
     def add_macro(self, value: str):
         if value not in self.macros:
             self.macros.append(value)
 
 
 @dataclass
-class RelationalNode(HasRelationMetadata):
+class DeferRelation(HasRelationMetadata):
     alias: str
+    relation_name: Optional[str]
 
     @property
     def identifier(self):
         return self.alias
 
 
 @dataclass
@@ -272,25 +273,14 @@
 
     def add_node(self, value: str):
         if value not in self.nodes:
             self.nodes.append(value)
 
 
 @dataclass
-class StateRelation(dbtClassMixin):
-    alias: str
-    database: Optional[str]
-    schema: str
-
-    @property
-    def identifier(self):
-        return self.alias
-
-
-@dataclass
 class ParsedNodeMandatory(GraphNode, HasRelationMetadata, Replaceable):
     alias: str
     checksum: FileHash
     config: NodeConfig = field(default_factory=NodeConfig)
 
     @property
     def identifier(self):
@@ -323,15 +313,15 @@
             },
         }
         return node_info
 
     def update_event_status(self, **kwargs):
         for k, v in kwargs.items():
             self._event_status[k] = v
-        set_contextvars(node_info=self.node_info)
+        set_log_contextvars(node_info=self.node_info)
 
     def clear_event_status(self):
         self._event_status = dict()
 
 
 @dataclass
 class ParsedNode(NodeInfoMixin, ParsedNodeMandatory, SerializableType):
@@ -573,15 +563,15 @@
 class ModelNode(CompiledNode):
     resource_type: NodeType = field(metadata={"restrict": [NodeType.Model]})
     access: AccessType = AccessType.Protected
     constraints: List[ModelLevelConstraint] = field(default_factory=list)
     version: Optional[NodeVersion] = None
     latest_version: Optional[NodeVersion] = None
     deprecation_date: Optional[datetime] = None
-    state_relation: Optional[StateRelation] = None
+    defer_relation: Optional[DeferRelation] = None
 
     @classmethod
     def from_args(cls, args: ModelNodeArgs) -> "ModelNode":
         unique_id = args.unique_id
 
         # build unrendered config -- for usage in ParsedNode.same_contents
         unrendered_config = {}
@@ -792,15 +782,15 @@
 class SeedNode(ParsedNode):  # No SQLDefaults!
     resource_type: NodeType = field(metadata={"restrict": [NodeType.Seed]})
     config: SeedConfig = field(default_factory=SeedConfig)
     # seeds need the root_path because the contents are not loaded initially
     # and we need the root_path to load the seed later
     root_path: Optional[str] = None
     depends_on: MacroDependsOn = field(default_factory=MacroDependsOn)
-    state_relation: Optional[StateRelation] = None
+    defer_relation: Optional[DeferRelation] = None
 
     def same_seeds(self, other: "SeedNode") -> bool:
         # for seeds, we check the hashes. If the hashes are different types,
         # no match. If the hashes are both the same 'path', log a warning and
         # assume they are the same
         # if the current checksum is a path, we want to log a warning.
         result = self.checksum == other.checksum
@@ -987,15 +977,15 @@
     config: EmptySnapshotConfig = field(default_factory=EmptySnapshotConfig)
 
 
 @dataclass
 class SnapshotNode(CompiledNode):
     resource_type: NodeType = field(metadata={"restrict": [NodeType.Snapshot]})
     config: SnapshotConfig
-    state_relation: Optional[StateRelation] = None
+    defer_relation: Optional[DeferRelation] = None
 
 
 # ====================================
 # Macro
 # ====================================
```

### Comparing `dbt-core-1.6.0b7/dbt/contracts/graph/semantic_models.py` & `dbt-core-1.6.0b8/dbt/contracts/graph/semantic_models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/graph/unparsed.py` & `dbt-core-1.6.0b8/dbt/contracts/graph/unparsed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/graph/utils.py` & `dbt-core-1.6.0b8/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/project.py` & `dbt-core-1.6.0b8/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/relation.py` & `dbt-core-1.6.0b8/dbt/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/results.py` & `dbt-core-1.6.0b8/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/selection.py` & `dbt-core-1.6.0b8/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/sql.py` & `dbt-core-1.6.0b8/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/state.py` & `dbt-core-1.6.0b8/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/contracts/util.py` & `dbt-core-1.6.0b8/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/dataclass_schema.py` & `dbt-core-1.6.0b8/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/deprecations.py` & `dbt-core-1.6.0b8/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/deps/base.py` & `dbt-core-1.6.0b8/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/deps/git.py` & `dbt-core-1.6.0b8/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/deps/local.py` & `dbt-core-1.6.0b8/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/deps/registry.py` & `dbt-core-1.6.0b8/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/deps/resolver.py` & `dbt-core-1.6.0b8/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/deps/tarball.py` & `dbt-core-1.6.0b8/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.6.0b8/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/docs/source/conf.py` & `dbt-core-1.6.0b8/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/events/adapter_endpoint.py` & `dbt-core-1.6.0b8/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/events/base_types.py` & `dbt-core-1.6.0b8/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/events/contextvars.py` & `dbt-core-1.6.0b8/dbt/events/contextvars.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,114 @@
 import contextlib
 import contextvars
 
 from typing import Any, Generator, Mapping, Dict
 
 
 LOG_PREFIX = "log_"
-LOG_PREFIX_LEN = len(LOG_PREFIX)
+TASK_PREFIX = "task_"
 
-_log_context_vars: Dict[str, contextvars.ContextVar] = {}
+_context_vars: Dict[str, contextvars.ContextVar] = {}
 
 
-def get_contextvars() -> Dict[str, Any]:
+def get_contextvars(prefix: str) -> Dict[str, Any]:
     rv = {}
     ctx = contextvars.copy_context()
 
+    prefix_len = len(prefix)
     for k in ctx:
-        if k.name.startswith(LOG_PREFIX) and ctx[k] is not Ellipsis:
-            rv[k.name[LOG_PREFIX_LEN:]] = ctx[k]
+        if k.name.startswith(prefix) and ctx[k] is not Ellipsis:
+            rv[k.name[prefix_len:]] = ctx[k]
 
     return rv
 
 
 def get_node_info():
-    cvars = get_contextvars()
+    cvars = get_contextvars(LOG_PREFIX)
     if "node_info" in cvars:
         return cvars["node_info"]
     else:
         return {}
 
 
-def clear_contextvars() -> None:
+def get_project_root():
+    cvars = get_contextvars(TASK_PREFIX)
+    if "project_root" in cvars:
+        return cvars["project_root"]
+    else:
+        return None
+
+
+def clear_contextvars(prefix: str) -> None:
     ctx = contextvars.copy_context()
     for k in ctx:
-        if k.name.startswith(LOG_PREFIX):
+        if k.name.startswith(prefix):
             k.set(Ellipsis)
 
 
+def set_log_contextvars(**kwargs: Any) -> Mapping[str, contextvars.Token]:
+    return set_contextvars(LOG_PREFIX, **kwargs)
+
+
+def set_task_contextvars(**kwargs: Any) -> Mapping[str, contextvars.Token]:
+    return set_contextvars(TASK_PREFIX, **kwargs)
+
+
 # put keys and values into context. Returns the contextvar.Token mapping
 # Save and pass to reset_contextvars
-def set_contextvars(**kwargs: Any) -> Mapping[str, contextvars.Token]:
+def set_contextvars(prefix: str, **kwargs: Any) -> Mapping[str, contextvars.Token]:
     cvar_tokens = {}
     for k, v in kwargs.items():
-        log_key = f"{LOG_PREFIX}{k}"
+        log_key = f"{prefix}{k}"
         try:
-            var = _log_context_vars[log_key]
+            var = _context_vars[log_key]
         except KeyError:
             var = contextvars.ContextVar(log_key, default=Ellipsis)
-            _log_context_vars[log_key] = var
+            _context_vars[log_key] = var
 
         cvar_tokens[k] = var.set(v)
 
     return cvar_tokens
 
 
 # reset by Tokens
-def reset_contextvars(**kwargs: contextvars.Token) -> None:
+def reset_contextvars(prefix: str, **kwargs: contextvars.Token) -> None:
     for k, v in kwargs.items():
-        log_key = f"{LOG_PREFIX}{k}"
-        var = _log_context_vars[log_key]
+        log_key = f"{prefix}{k}"
+        var = _context_vars[log_key]
         var.reset(v)
 
 
 # remove from contextvars
-def unset_contextvars(*keys: str) -> None:
+def unset_contextvars(prefix: str, *keys: str) -> None:
     for k in keys:
-        if k in _log_context_vars:
-            log_key = f"{LOG_PREFIX}{k}"
-            _log_context_vars[log_key].set(Ellipsis)
+        if k in _context_vars:
+            log_key = f"{prefix}{k}"
+            _context_vars[log_key].set(Ellipsis)
 
 
 # Context manager or decorator to set and unset the context vars
 @contextlib.contextmanager
 def log_contextvars(**kwargs: Any) -> Generator[None, None, None]:
-    context = get_contextvars()
+    context = get_contextvars(LOG_PREFIX)
+    saved = {k: context[k] for k in context.keys() & kwargs.keys()}
+
+    set_contextvars(LOG_PREFIX, **kwargs)
+    try:
+        yield
+    finally:
+        unset_contextvars(LOG_PREFIX, *kwargs.keys())
+        set_contextvars(LOG_PREFIX, **saved)
+
+
+# Context manager for earlier in task.run
+@contextlib.contextmanager
+def task_contextvars(**kwargs: Any) -> Generator[None, None, None]:
+    context = get_contextvars(TASK_PREFIX)
     saved = {k: context[k] for k in context.keys() & kwargs.keys()}
 
-    set_contextvars(**kwargs)
+    set_contextvars(TASK_PREFIX, **kwargs)
     try:
         yield
     finally:
-        unset_contextvars(*kwargs.keys())
-        set_contextvars(**saved)
+        unset_contextvars(TASK_PREFIX, *kwargs.keys())
+        set_contextvars(TASK_PREFIX, **saved)
```

### Comparing `dbt-core-1.6.0b7/dbt/events/eventmgr.py` & `dbt-core-1.6.0b8/dbt/events/eventmgr.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/events/format.py` & `dbt-core-1.6.0b8/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/events/functions.py` & `dbt-core-1.6.0b8/dbt/events/functions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/events/helpers.py` & `dbt-core-1.6.0b8/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/events/types.py` & `dbt-core-1.6.0b8/dbt/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/events/types_pb2.py` & `dbt-core-1.6.0b8/dbt/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/exceptions.py` & `dbt-core-1.6.0b8/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/flags.py` & `dbt-core-1.6.0b8/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/graph/cli.py` & `dbt-core-1.6.0b8/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/graph/graph.py` & `dbt-core-1.6.0b8/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/graph/queue.py` & `dbt-core-1.6.0b8/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/graph/selector.py` & `dbt-core-1.6.0b8/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/graph/selector_methods.py` & `dbt-core-1.6.0b8/dbt/graph/selector_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from dbt.contracts.graph.unparsed import UnparsedVersion
 from dbt.contracts.state import PreviousState
 from dbt.exceptions import (
     DbtInternalError,
     DbtRuntimeError,
 )
 from dbt.node_types import NodeType
-from dbt.task.contextvars import cv_project_root
+from dbt.events.contextvars import get_project_root
 
 
 SELECTOR_GLOB = "*"
 SELECTOR_DELIMITER = ":"
 
 
 class MethodName(StrEnum):
@@ -57,16 +57,16 @@
 
 def is_selected_node(fqn: List[str], node_selector: str, is_versioned: bool) -> bool:
     # If qualified_name exactly matches model name (fqn's leaf), return True
     if is_versioned:
         flat_node_selector = node_selector.split(".")
         if fqn[-2] == node_selector:
             return True
-        # If this is a versioned model, then the last two segments should be allowed to exactly match
-        elif fqn[-2:] == flat_node_selector[-2:]:
+        # If this is a versioned model, then the last two segments should be allowed to exactly match on either the '.' or '_' delimiter
+        elif "_".join(fqn[-2:]) == "_".join(flat_node_selector[-2:]):
             return True
     else:
         if fqn[-1] == node_selector:
             return True
     # Flatten node parts. Dots in model names act as namespace separators
     flat_fqn = [item for segment in fqn for item in segment.split(".")]
     # Selector components cannot be more than fqn's
@@ -322,15 +322,19 @@
             yield node
 
 
 class PathSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """Yields nodes from included that match the given path."""
         # get project root from contextvar
-        root = Path(cv_project_root.get())
+        project_root = get_project_root()
+        if project_root:
+            root = Path(project_root)
+        else:
+            root = Path.cwd()
         paths = set(p.relative_to(root) for p in root.glob(selector))
         for node, real_node in self.all_nodes(included_nodes):
             ofp = Path(real_node.original_file_path)
             if ofp in paths:
                 yield node
             if hasattr(real_node, "patch_path") and real_node.patch_path:  # type: ignore
                 pfp = real_node.patch_path.split("://")[1]  # type: ignore
@@ -343,14 +347,16 @@
 
 class FileSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """Yields nodes from included that match the given file name."""
         for node, real_node in self.all_nodes(included_nodes):
             if fnmatch(Path(real_node.original_file_path).name, selector):
                 yield node
+            elif fnmatch(Path(real_node.original_file_path).stem, selector):
+                yield node
 
 
 class PackageSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """Yields nodes from included that have the specified package"""
         for node, real_node in self.all_nodes(included_nodes):
             if fnmatch(real_node.package_name, selector):
@@ -534,14 +540,19 @@
             different_contents = not new.same_contents(old)  # type: ignore
         else:
             different_contents = not new.same_contents(old, adapter_type)  # type: ignore
 
         upstream_macro_change = self.check_macros_modified(new)
         return different_contents or upstream_macro_change
 
+    def check_unmodified_content(
+        self, old: Optional[SelectorTarget], new: SelectorTarget, adapter_type: str
+    ) -> bool:
+        return not self.check_modified_content(old, new, adapter_type)
+
     def check_modified_macros(self, old, new: SelectorTarget) -> bool:
         return self.check_macros_modified(new)
 
     @staticmethod
     def check_modified_factory(
         compare_method: str,
     ) -> Callable[[Optional[SelectorTarget], SelectorTarget], bool]:
@@ -578,16 +589,18 @@
             raise DbtRuntimeError("Got a state selector method, but no comparison manifest")
 
         adapter_type = self.manifest.metadata.adapter_type
 
         state_checks = {
             # it's new if there is no old version
             "new": lambda old, new: old is None,
+            "old": lambda old, new: old is not None,
             # use methods defined above to compare properties of old + new
             "modified": self.check_modified_content,
+            "unmodified": self.check_unmodified_content,
             "modified.body": self.check_modified_factory("same_body"),
             "modified.configs": self.check_modified_factory("same_config"),
             "modified.persisted_descriptions": self.check_modified_factory(
                 "same_persisted_description"
             ),
             "modified.relation": self.check_modified_factory("same_database_representation"),
             "modified.macros": self.check_modified_macros,
@@ -611,15 +624,19 @@
                 previous_node = manifest.sources[node]
             elif node in manifest.exposures:
                 previous_node = manifest.exposures[node]
             elif node in manifest.metrics:
                 previous_node = manifest.metrics[node]
 
             keyword_args = {}
-            if checker.__name__ in ["same_contract", "check_modified_content"]:
+            if checker.__name__ in [
+                "same_contract",
+                "check_modified_content",
+                "check_unmodified_content",
+            ]:
                 keyword_args["adapter_type"] = adapter_type  # type: ignore
 
             if checker(previous_node, real_node, **keyword_args):  # type: ignore
                 yield node
 
 
 class ResultSelectorMethod(SelectorMethod):
```

### Comparing `dbt-core-1.6.0b7/dbt/graph/selector_spec.py` & `dbt-core-1.6.0b8/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/helper_types.py` & `dbt-core-1.6.0b8/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/README.md` & `dbt-core-1.6.0b8/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/docs/overview.md` & `dbt-core-1.6.0b8/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/columns.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/drop_relation.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/drop_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/relation.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/schema.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/etc/datetime.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/etc/statement.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/configs.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/table/table.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/models/view/view.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/python_model/python.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/data_types.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/listagg.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/macros/utils/split_part.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/global_project/tests/generic/builtin.sql` & `dbt-core-1.6.0b8/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/index.html` & `dbt-core-1.6.0b8/dbt/include/index.html`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/starter_project/README.md` & `dbt-core-1.6.0b8/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.6.0b8/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/internal_deprecations.py` & `dbt-core-1.6.0b8/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/logger.py` & `dbt-core-1.6.0b8/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/node_types.py` & `dbt-core-1.6.0b8/dbt/node_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     Analysis = "analysis"
     Test = "test"
     Snapshot = "snapshot"
     Operation = "operation"
     Seed = "seed"
     # TODO: rm?
     RPCCall = "rpc"
-    SqlOperation = "sqloperation"
+    SqlOperation = "sql_operation"
     Documentation = "doc"
     Source = "source"
     Macro = "macro"
     Exposure = "exposure"
     Metric = "metric"
     Group = "group"
-    SemanticModel = "semanticmodel"
+    SemanticModel = "semantic_model"
 
     @classmethod
     def executable(cls) -> List["NodeType"]:
         return [
             cls.Model,
             cls.Test,
             cls.Snapshot,
```

### Comparing `dbt-core-1.6.0b7/dbt/parser/__init__.py` & `dbt-core-1.6.0b8/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/analysis.py` & `dbt-core-1.6.0b8/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/base.py` & `dbt-core-1.6.0b8/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/common.py` & `dbt-core-1.6.0b8/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/docs.py` & `dbt-core-1.6.0b8/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/generic_test.py` & `dbt-core-1.6.0b8/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/generic_test_builders.py` & `dbt-core-1.6.0b8/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/hooks.py` & `dbt-core-1.6.0b8/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/macros.py` & `dbt-core-1.6.0b8/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/manifest.py` & `dbt-core-1.6.0b8/dbt/parser/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,14 +118,16 @@
 from dbt.parser.snapshots import SnapshotParser
 from dbt.parser.sources import SourcePatcher
 from dbt.version import __version__
 
 from dbt.dataclass_schema import StrEnum, dbtClassMixin
 from dbt.plugins import get_plugin_manager
 
+from dbt_semantic_interfaces.enum_extension import assert_values_exhausted
+from dbt_semantic_interfaces.type_enums import MetricType
 
 PARSING_STATE = DbtProcessState("parsing")
 PERF_INFO_FILE_NAME = "perf_info.json"
 
 
 def extended_mashumaro_encoder(data):
     return msgpack.packb(data, default=extended_msgpack_encoder, use_bin_type=True)
@@ -1060,24 +1062,23 @@
             _process_refs(self.manifest, current_project, semantic_model, dependencies)
             self.update_semantic_model(semantic_model)
 
     # Takes references in 'metrics' array of nodes and exposures, finds the target
     # node, and updates 'depends_on.nodes' with the unique id
     def process_metrics(self, config: RuntimeConfig):
         current_project = config.project_name
-        for node in self.manifest.nodes.values():
-            if node.created_at < self.started_at:
-                continue
-            _process_metrics_for_node(self.manifest, current_project, node)
         for metric in self.manifest.metrics.values():
-            # TODO: Can we do this if the metric is derived & depends on
-            # some other metric for its definition? Maybe....
             if metric.created_at < self.started_at:
                 continue
+            _process_metric_node(self.manifest, current_project, metric)
             _process_metrics_for_node(self.manifest, current_project, metric)
+        for node in self.manifest.nodes.values():
+            if node.created_at < self.started_at:
+                continue
+            _process_metrics_for_node(self.manifest, current_project, node)
         for exposure in self.manifest.exposures.values():
             if exposure.created_at < self.started_at:
                 continue
             _process_metrics_for_node(self.manifest, current_project, exposure)
 
     def update_semantic_model(self, semantic_model) -> None:
         # This has to be done at the end of parsing because the referenced model
@@ -1435,14 +1436,71 @@
                 scope=target_model.package_name,
             )
 
         target_model_id = target_model.unique_id
         node.depends_on.add_node(target_model_id)
 
 
+def _process_metric_node(
+    manifest: Manifest,
+    current_project: str,
+    metric: Metric,
+) -> None:
+    """Sets a metric's input_measures"""
+
+    # This ensures that if this metrics input_measures have already been set
+    # we skip the work. This could happen either due to recursion or if multiple
+    # metrics derive from another given metric.
+    # NOTE: This does not protect against infinite loops
+    if len(metric.type_params.input_measures) > 0:
+        return
+
+    if metric.type is MetricType.SIMPLE or metric.type is MetricType.CUMULATIVE:
+        assert (
+            metric.type_params.measure is not None
+        ), f"{metric} should have a measure defined, but it does not."
+        metric.type_params.input_measures.append(metric.type_params.measure)
+
+    elif metric.type is MetricType.DERIVED or metric.type is MetricType.RATIO:
+        input_metrics = metric.input_metrics
+        if metric.type is MetricType.RATIO:
+            if metric.type_params.numerator is None or metric.type_params.denominator is None:
+                raise dbt.exceptions.ParsingError(
+                    "Invalid ratio metric. Both a numerator and denominator must be specified",
+                    node=metric,
+                )
+            input_metrics = [metric.type_params.numerator, metric.type_params.denominator]
+
+        for input_metric in input_metrics:
+            target_metric = manifest.resolve_metric(
+                target_metric_name=input_metric.name,
+                target_metric_package=None,
+                current_project=current_project,
+                node_package=metric.package_name,
+            )
+
+            if target_metric is None:
+                raise dbt.exceptions.ParsingError(
+                    f"The metric `{input_metric.name}` does not exist but was referenced.",
+                    node=metric,
+                )
+            elif isinstance(target_metric, Disabled):
+                raise dbt.exceptions.ParsingError(
+                    f"The metric `{input_metric.name}` is disabled and thus cannot be referenced.",
+                    node=metric,
+                )
+
+            _process_metric_node(
+                manifest=manifest, current_project=current_project, metric=target_metric
+            )
+            metric.type_params.input_measures.extend(target_metric.type_params.input_measures)
+    else:
+        assert_values_exhausted(metric.type)
+
+
 def _process_metrics_for_node(
     manifest: Manifest,
     current_project: str,
     node: Union[ManifestNode, Metric, Exposure],
 ):
     """Given a manifest and a node in that manifest, process its metrics"""
```

### Comparing `dbt-core-1.6.0b7/dbt/parser/models.py` & `dbt-core-1.6.0b8/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/partial.py` & `dbt-core-1.6.0b8/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/read_files.py` & `dbt-core-1.6.0b8/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/schema_generic_tests.py` & `dbt-core-1.6.0b8/dbt/parser/schema_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/schema_renderer.py` & `dbt-core-1.6.0b8/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/schema_yaml_readers.py` & `dbt-core-1.6.0b8/dbt/parser/schema_yaml_readers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/schemas.py` & `dbt-core-1.6.0b8/dbt/parser/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/search.py` & `dbt-core-1.6.0b8/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/seeds.py` & `dbt-core-1.6.0b8/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/singular_test.py` & `dbt-core-1.6.0b8/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/snapshots.py` & `dbt-core-1.6.0b8/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/sources.py` & `dbt-core-1.6.0b8/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/parser/sql.py` & `dbt-core-1.6.0b8/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/plugins/__init__.py` & `dbt-core-1.6.0b8/dbt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/plugins/manager.py` & `dbt-core-1.6.0b8/dbt/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/plugins/manifest.py` & `dbt-core-1.6.0b8/dbt/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/semver.py` & `dbt-core-1.6.0b8/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/base.py` & `dbt-core-1.6.0b8/dbt/task/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     DbtRuntimeError,
     DbtInternalError,
 )
 from dbt.flags import get_flags
 from dbt.graph import Graph
 from dbt.logger import log_manager
 from .printer import print_run_result_error
-from dbt.task.contextvars import cv_project_root
 
 
 class NoneConfig:
     @classmethod
     def from_args(cls, args):
         return None
 
@@ -72,16 +71,14 @@
 class BaseTask(metaclass=ABCMeta):
     ConfigType: Union[Type[NoneConfig], Type[Project]] = NoneConfig
 
     def __init__(self, args, config, project=None):
         self.args = args
         self.config = config
         self.project = config if isinstance(config, Project) else project
-        if self.config:
-            cv_project_root.set(self.config.project_root)
 
     @classmethod
     def pre_init_hook(cls, args):
         """A hook called before the task is initialized."""
         if args.log_format == "json":
             log_manager.format_json()
         else:
```

### Comparing `dbt-core-1.6.0b7/dbt/task/build.py` & `dbt-core-1.6.0b8/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/clean.py` & `dbt-core-1.6.0b8/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/compile.py` & `dbt-core-1.6.0b8/dbt/task/compile.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import AbstractSet, Optional
 
 from dbt.contracts.graph.manifest import WritableManifest
 from dbt.contracts.results import RunStatus, RunResult
 from dbt.events.base_types import EventLevel
 from dbt.events.functions import fire_event
 from dbt.events.types import CompiledNode, Note
-from dbt.exceptions import DbtInternalError, DbtRuntimeError
+from dbt.exceptions import DbtInternalError
 from dbt.graph import ResourceTypeSelector
 from dbt.node_types import NodeType
 from dbt.parser.manifest import write_manifest, process_node
 from dbt.parser.sql import SqlBlockParser
 from dbt.task.base import BaseRunner
 from dbt.task.runnable import GraphRunnableTask
 
@@ -93,26 +93,15 @@
                     is_inline=is_inline,
                     output_format=output_format,
                     unique_id=result.node.unique_id,
                 )
             )
 
     def _get_deferred_manifest(self) -> Optional[WritableManifest]:
-        if not self.args.defer:
-            return None
-
-        state = self.previous_defer_state or self.previous_state
-        if not state:
-            raise DbtRuntimeError(
-                "Received a --defer argument, but no value was provided to --state"
-            )
-
-        if not state.manifest:
-            raise DbtRuntimeError(f'Could not find manifest in --state path: "{state}"')
-        return state.manifest
+        return super()._get_deferred_manifest() if self.args.defer else None
 
     def defer_to_manifest(self, adapter, selected_uids: AbstractSet[str]):
         deferred_manifest = self._get_deferred_manifest()
         if deferred_manifest is None:
             return
         if self.manifest is None:
             raise DbtInternalError(
```

### Comparing `dbt-core-1.6.0b7/dbt/task/debug.py` & `dbt-core-1.6.0b8/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/deps.py` & `dbt-core-1.6.0b8/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/freshness.py` & `dbt-core-1.6.0b8/dbt/task/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/generate.py` & `dbt-core-1.6.0b8/dbt/task/generate.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/init.py` & `dbt-core-1.6.0b8/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/list.py` & `dbt-core-1.6.0b8/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/printer.py` & `dbt-core-1.6.0b8/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/retry.py` & `dbt-core-1.6.0b8/dbt/task/retry.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,38 +5,41 @@
 from dbt.config import RuntimeConfig
 from dbt.contracts.results import NodeStatus
 from dbt.contracts.state import PreviousState
 from dbt.exceptions import DbtRuntimeError
 from dbt.graph import GraphQueue
 from dbt.task.base import ConfiguredTask
 from dbt.task.build import BuildTask
+from dbt.task.clone import CloneTask
 from dbt.task.compile import CompileTask
 from dbt.task.generate import GenerateTask
 from dbt.task.run import RunTask
 from dbt.task.run_operation import RunOperationTask
 from dbt.task.seed import SeedTask
 from dbt.task.snapshot import SnapshotTask
 from dbt.task.test import TestTask
 
 RETRYABLE_STATUSES = {NodeStatus.Error, NodeStatus.Fail, NodeStatus.Skipped, NodeStatus.RuntimeErr}
 
 TASK_DICT = {
     "build": BuildTask,
     "compile": CompileTask,
+    "clone": CloneTask,
     "generate": GenerateTask,
     "seed": SeedTask,
     "snapshot": SnapshotTask,
     "test": TestTask,
     "run": RunTask,
     "run-operation": RunOperationTask,
 }
 
 CMD_DICT = {
     "build": CliCommand.BUILD,
     "compile": CliCommand.COMPILE,
+    "clone": CliCommand.CLONE,
     "generate": CliCommand.DOCS_GENERATE,
     "seed": CliCommand.SEED,
     "snapshot": CliCommand.SNAPSHOT,
     "test": CliCommand.TEST,
     "run": CliCommand.RUN,
     "run-operation": CliCommand.RUN_OPERATION,
 }
```

### Comparing `dbt-core-1.6.0b7/dbt/task/run.py` & `dbt-core-1.6.0b8/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/run_operation.py` & `dbt-core-1.6.0b8/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/runnable.py` & `dbt-core-1.6.0b8/dbt/task/runnable.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     NodeStart,
     NodeFinished,
     QueryCancelationUnsupported,
     ConcurrencyLine,
     EndRunResult,
     NothingToDo,
 )
-from dbt.events.contextvars import log_contextvars
+from dbt.events.contextvars import log_contextvars, task_contextvars
 from dbt.contracts.graph.nodes import ResultNode
 from dbt.contracts.results import NodeStatus, RunExecutionResult, RunningStatus
 from dbt.contracts.state import PreviousState
 from dbt.exceptions import (
     DbtInternalError,
     NotImplementedError,
     DbtRuntimeError,
@@ -50,14 +50,15 @@
 from dbt.graph import GraphQueue, NodeSelector, SelectionSpec, parse_difference
 from dbt.parser.manifest import write_manifest
 import dbt.tracking
 
 import dbt.exceptions
 from dbt.flags import get_flags
 import dbt.utils
+from dbt.contracts.graph.manifest import WritableManifest
 
 RESULT_FILE_NAME = "run_results.json"
 RUNNING_STATE = DbtProcessState("running")
 
 
 class GraphRunnableTask(ConfiguredTask):
     MARK_DEPENDENT_ERRORS_STATUSES = [NodeStatus.Error]
@@ -426,33 +427,38 @@
 
         return result
 
     def run(self):
         """
         Run dbt for the query, based on the graph.
         """
-        self._runtime_initialize()
+        # We set up a context manager here with "task_contextvars" because we
+        # we need the project_root in runtime_initialize.
+        with task_contextvars(project_root=self.config.project_root):
+            self._runtime_initialize()
 
-        if self._flattened_nodes is None:
-            raise DbtInternalError("after _runtime_initialize, _flattened_nodes was still None")
+            if self._flattened_nodes is None:
+                raise DbtInternalError(
+                    "after _runtime_initialize, _flattened_nodes was still None"
+                )
 
-        if len(self._flattened_nodes) == 0:
-            with TextOnly():
-                fire_event(Formatting(""))
-            warn_or_error(NothingToDo())
-            result = self.get_result(
-                results=[],
-                generated_at=datetime.utcnow(),
-                elapsed_time=0.0,
-            )
-        else:
-            with TextOnly():
-                fire_event(Formatting(""))
-            selected_uids = frozenset(n.unique_id for n in self._flattened_nodes)
-            result = self.execute_with_hooks(selected_uids)
+            if len(self._flattened_nodes) == 0:
+                with TextOnly():
+                    fire_event(Formatting(""))
+                warn_or_error(NothingToDo())
+                result = self.get_result(
+                    results=[],
+                    generated_at=datetime.utcnow(),
+                    elapsed_time=0.0,
+                )
+            else:
+                with TextOnly():
+                    fire_event(Formatting(""))
+                selected_uids = frozenset(n.unique_id for n in self._flattened_nodes)
+                result = self.execute_with_hooks(selected_uids)
 
         # We have other result types here too, including FreshnessResult
         if isinstance(result, RunExecutionResult):
             result_msgs = [result.to_msg_dict() for result in result.results]
             fire_event(
                 EndRunResult(
                     results=result_msgs,
@@ -576,7 +582,18 @@
             elapsed_time=elapsed_time,
             generated_at=generated_at,
             args=dbt.utils.args_to_dict(self.args),
         )
 
     def task_end_messages(self, results):
         print_run_end_messages(results)
+
+    def _get_deferred_manifest(self) -> Optional[WritableManifest]:
+        state = self.previous_defer_state or self.previous_state
+        if not state:
+            raise DbtRuntimeError(
+                "--state or --defer-state are required for deferral, but neither was provided"
+            )
+
+        if not state.manifest:
+            raise DbtRuntimeError(f'Could not find manifest in --state path: "{state}"')
+        return state.manifest
```

### Comparing `dbt-core-1.6.0b7/dbt/task/seed.py` & `dbt-core-1.6.0b8/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/serve.py` & `dbt-core-1.6.0b8/dbt/task/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/show.py` & `dbt-core-1.6.0b8/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/snapshot.py` & `dbt-core-1.6.0b8/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/sql.py` & `dbt-core-1.6.0b8/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/task/test.py` & `dbt-core-1.6.0b8/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/tests/fixtures/project.py` & `dbt-core-1.6.0b8/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/tests/util.py` & `dbt-core-1.6.0b8/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/tracking.py` & `dbt-core-1.6.0b8/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/ui.py` & `dbt-core-1.6.0b8/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/utils.py` & `dbt-core-1.6.0b8/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b7/dbt/version.py` & `dbt-core-1.6.0b8/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.6.0b7"
+__version__ = "1.6.0b8"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.6.0b7/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.6.0b8/dbt_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b7
+Version: 1.6.0b8
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b7 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b8 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b7/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.6.0b8/dbt_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,17 @@
 dbt/include/global_project/macros/generic_test_sql/relationships.sql
 dbt/include/global_project/macros/generic_test_sql/unique.sql
 dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
 dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
 dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
 dbt/include/global_project/macros/materializations/configs.sql
 dbt/include/global_project/macros/materializations/hooks.sql
+dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
+dbt/include/global_project/macros/materializations/models/clone/clone.sql
+dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
 dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
 dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
 dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
 dbt/include/global_project/macros/materializations/models/incremental/merge.sql
 dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
 dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
 dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
@@ -248,16 +251,16 @@
 dbt/plugins/exceptions.py
 dbt/plugins/manager.py
 dbt/plugins/manifest.py
 dbt/task/__init__.py
 dbt/task/base.py
 dbt/task/build.py
 dbt/task/clean.py
+dbt/task/clone.py
 dbt/task/compile.py
-dbt/task/contextvars.py
 dbt/task/debug.py
 dbt/task/deps.py
 dbt/task/freshness.py
 dbt/task/generate.py
 dbt/task/init.py
 dbt/task/list.py
 dbt/task/parse.py
```

### Comparing `dbt-core-1.6.0b7/setup.py` & `dbt-core-1.6.0b8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.6.0b7"
+package_version = "1.6.0b8"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -64,25 +64,24 @@
         # ----
         # These packages are major-version-0. Keep upper bounds on upcoming minor versions (which could have breaking changes)
         # and check compatibility / bump in each new minor version of dbt-core.
         "colorama>=0.3.9,<0.5",
         "pathspec>=0.9,<0.12",
         "isodate>=0.6,<0.7",
         # ----
-        # There is a difficult-to-reproduce bug in sqlparse==0.4.4 for ephemeral model compilation
-        # For context: dbt-core#7396 + dbt-core#7515
-        "sqlparse>=0.2.3,<0.4.4",
+        # There was a pin to below 0.4.4 for a while due to a bug in Ubuntu/sqlparse 0.4.4
+        "sqlparse>=0.2.3",
         # ----
         # These are major-version-0 packages also maintained by dbt-labs. Accept patches.
         "dbt-extractor~=0.4.1",
         "hologram~=0.0.16",  # includes transitive dependencies on python-dateutil and jsonschema
         "minimal-snowplow-tracker~=0.0.2",
         # DSI is under active development, so we're pinning to specific dev versions for now.
         # TODO: Before RC/final release, update to use ~= pinning.
-        "dbt-semantic-interfaces==0.1.0.dev7",
+        "dbt-semantic-interfaces==0.1.0.dev8",
         # ----
         # Expect compatibility with all new versions of these packages, so lower bounds only.
         "packaging>20.9",
         "protobuf>=4.0.0",
         "pytz>=2015.7",
         "pyyaml>=6.0",
         "typing-extensions>=3.7.4",
```

