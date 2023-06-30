# Comparing `tmp/boaviztapi-1.0.0a3.tar.gz` & `tmp/boaviztapi-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boaviztapi-1.0.0a3.tar", max compression
+gzip compressed data, was "boaviztapi-1.0.0a4.tar", max compression
```

## Comparing `boaviztapi-1.0.0a3.tar` & `boaviztapi-1.0.0a4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    34523 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/LICENSE
--rw-r--r--   0        0        0     4494 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/README.md
--rw-r--r--   0        0        0      365 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/__init__.py
--rw-r--r--   0        0        0   114581 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/cloud/aws.csv
--rw-r--r--   0        0        0      559 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/cloud/gcp.csv
--rw-r--r--   0        0        0       58 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/cloud/providers.csv
--rw-r--r--   0        0        0      116 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/components/case.csv
--rw-r--r--   0        0        0      268 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/components/cpu.csv
--rw-r--r--   0        0        0       95 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/components/hdd.csv
--rw-r--r--   0        0        0       97 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/components/power_supply.csv
--rw-r--r--   0        0        0      162 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/components/ram.csv
--rw-r--r--   0        0        0      130 2023-06-05 09:59:36.977544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/components/ssd.csv
--rw-r--r--   0        0        0     1242 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/server.csv
--rw-r--r--   0        0        0      921 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/archetypes/user_terminal.csv
--rw-r--r--   0        0        0      819 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/config.yml
--rw-r--r--   0        0        0      314 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/consumption_profile/cpu/cpu_profile.csv
--rw-r--r--   0        0        0     3404 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/ademe_base_impacts_negaoctet.csv
--rw-r--r--   0        0        0     4553 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/cpu_manufacture.csv
--rw-r--r--   0        0        0   515038 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/cpu_specs.csv
--rw-r--r--   0        0        0    26045 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/electrical_mix.csv
--rw-r--r--   0        0        0      113 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/missing_cpu_manufacture.csv
--rw-r--r--   0        0        0      214 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/ram_manufacture.csv
--rw-r--r--   0        0        0     2274 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/ssd_manufacture.csv
--rw-r--r--   0        0        0   425401 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/factors.yml
--rw-r--r--   0        0        0     2259 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/data/utils/jsonifyer.py
--rw-r--r--   0        0        0       30 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/dto/__init__.py
--rw-r--r--   0        0        0      123 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/dto/base_dto.py
--rw-r--r--   0        0        0      154 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/dto/component/__init__.py
--rw-r--r--   0        0        0      205 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/dto/component/component_dto.py
--rw-r--r--   0        0        0     2199 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/dto/component/cpu.py
--rw-r--r--   0        0        0     1814 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/dto/component/disk.py
--rw-r--r--   0        0        0     1994 2023-06-05 09:59:36.981544 boaviztapi-1.0.0a3/boaviztapi/dto/component/other.py
--rw-r--r--   0        0        0     1440 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/dto/component/ram.py
--rw-r--r--   0        0        0       55 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/dto/consumption_profile/__init__.py
--rw-r--r--   0        0        0     1633 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/dto/consumption_profile/consumption_profile.py
--rw-r--r--   0        0        0       45 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/dto/device/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/dto/device/device.py
--rw-r--r--   0        0        0     2629 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/dto/device/user_terminal.py
--rw-r--r--   0        0        0       50 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/dto/usage/__init__.py
--rw-r--r--   0        0        0     6577 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/dto/usage/usage.py
--rw-r--r--   0        0        0     3329 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/main.py
--rw-r--r--   0        0        0      143 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/__init__.py
--rw-r--r--   0        0        0     3866 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/boattribute.py
--rw-r--r--   0        0        0      318 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/__init__.py
--rw-r--r--   0        0        0     1106 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/assembly.py
--rw-r--r--   0        0        0     5052 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/case.py
--rw-r--r--   0        0        0     2150 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/component.py
--rw-r--r--   0        0        0    14232 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/cpu.py
--rw-r--r--   0        0        0     1460 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/hdd.py
--rw-r--r--   0        0        0      941 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/motherboard.py
--rw-r--r--   0        0        0     2004 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/power_supply.py
--rw-r--r--   0        0        0     7197 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/ram.py
--rw-r--r--   0        0        0     4960 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/component/ssd.py
--rw-r--r--   0        0        0       88 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/consumption_profile/__init__.py
--rw-r--r--   0        0        0     7244 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/consumption_profile/consumption_profile.py
--rw-r--r--   0        0        0       81 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/device/__init__.py
--rw-r--r--   0        0        0     1134 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/device/device.py
--rw-r--r--   0        0        0     8965 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/device/server.py
--rw-r--r--   0        0        0     7261 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/device/userTerminal.py
--rw-r--r--   0        0        0     3983 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/impact.py
--rw-r--r--   0        0        0       65 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/usage/__init__.py
--rw-r--r--   0        0        0     8503 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/model/usage/usage.py
--rw-r--r--   0        0        0        0 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/__init__.py
--rw-r--r--   0        0        0     4052 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/cloud_router.py
--rw-r--r--   0        0        0    17594 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/component_router.py
--rw-r--r--   0        0        0      958 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/consumption_profile_router.py
--rw-r--r--   0        0        0        0 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/openapi_doc/__init__.py
--rw-r--r--   0        0        0     9638 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/openapi_doc/descriptions.py
--rw-r--r--   0        0        0     2624 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/openapi_doc/examples.py
--rw-r--r--   0        0        0     2207 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/openapi_doc/intro_openapi.md
--rw-r--r--   0        0        0     8625 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/peripheral_router.py
--rw-r--r--   0        0        0     3612 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/server_router.py
--rw-r--r--   0        0        0    13529 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/terminal_router.py
--rw-r--r--   0        0        0     2864 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/routers/utils_router.py
--rw-r--r--   0        0        0        0 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/service/__init__.py
--rw-r--r--   0        0        0      602 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/service/allocation.py
--rw-r--r--   0        0        0     4276 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/service/archetype.py
--rw-r--r--   0        0        0     2199 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/service/bottom_up.py
--rw-r--r--   0        0        0     3280 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/service/factor_provider.py
--rw-r--r--   0        0        0     2646 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/service/verbose.py
--rw-r--r--   0        0        0        0 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/utils/__init__.py
--rw-r--r--   0        0        0     1405 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/utils/fuzzymatch.py
--rw-r--r--   0        0        0     3257 2023-06-05 09:59:36.985544 boaviztapi-1.0.0a3/boaviztapi/utils/roundit.py
--rw-r--r--   0        0        0      695 2023-06-05 09:59:37.005544 boaviztapi-1.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 boaviztapi-1.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-30 14:28:51.753469 boaviztapi-1.0.0a4/LICENSE
+-rw-r--r--   0        0        0     4657 2023-06-30 14:28:51.753469 boaviztapi-1.0.0a4/README.md
+-rw-r--r--   0        0        0      336 2023-06-30 14:28:51.753469 boaviztapi-1.0.0a4/boaviztapi/__init__.py
+-rw-r--r--   0        0        0   114581 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/cloud/aws.csv
+-rw-r--r--   0        0        0      559 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/cloud/gcp.csv
+-rw-r--r--   0        0        0       58 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/cloud/providers.csv
+-rw-r--r--   0        0        0      116 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/components/case.csv
+-rw-r--r--   0        0        0      268 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/components/cpu.csv
+-rw-r--r--   0        0        0       95 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/components/hdd.csv
+-rw-r--r--   0        0        0       97 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/components/power_supply.csv
+-rw-r--r--   0        0        0      162 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/components/ram.csv
+-rw-r--r--   0        0        0      130 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/components/ssd.csv
+-rw-r--r--   0        0        0     1242 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/server.csv
+-rw-r--r--   0        0        0      921 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/archetypes/user_terminal.csv
+-rw-r--r--   0        0        0      819 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/config.yml
+-rw-r--r--   0        0        0      314 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/consumption_profile/cpu/cpu_profile.csv
+-rw-r--r--   0        0        0     3404 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/ademe_base_impacts_negaoctet.csv
+-rw-r--r--   0        0        0     4553 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/cpu_manufacture.csv
+-rw-r--r--   0        0        0   515038 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/cpu_specs.csv
+-rw-r--r--   0        0        0    26045 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/electrical_mix.csv
+-rw-r--r--   0        0        0      113 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/missing_cpu_manufacture.csv
+-rw-r--r--   0        0        0      214 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/ram_manufacture.csv
+-rw-r--r--   0        0        0     2274 2023-06-30 14:28:51.757469 boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/ssd_manufacture.csv
+-rw-r--r--   0        0        0   425401 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/data/factors.yml
+-rw-r--r--   0        0        0     2259 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/data/utils/jsonifyer.py
+-rw-r--r--   0        0        0       30 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/__init__.py
+-rw-r--r--   0        0        0      123 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/base_dto.py
+-rw-r--r--   0        0        0      154 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/component/__init__.py
+-rw-r--r--   0        0        0      205 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/component/component_dto.py
+-rw-r--r--   0        0        0     2199 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/component/cpu.py
+-rw-r--r--   0        0        0     1814 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/component/disk.py
+-rw-r--r--   0        0        0     1994 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/component/other.py
+-rw-r--r--   0        0        0     1440 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/component/ram.py
+-rw-r--r--   0        0        0       55 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/consumption_profile/__init__.py
+-rw-r--r--   0        0        0     1633 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/consumption_profile/consumption_profile.py
+-rw-r--r--   0        0        0       45 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/device/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/device/device.py
+-rw-r--r--   0        0        0     2629 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/device/user_terminal.py
+-rw-r--r--   0        0        0       50 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/usage/__init__.py
+-rw-r--r--   0        0        0     6577 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/dto/usage/usage.py
+-rw-r--r--   0        0        0     3529 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/main.py
+-rw-r--r--   0        0        0      143 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/__init__.py
+-rw-r--r--   0        0        0     3866 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/boattribute.py
+-rw-r--r--   0        0        0      318 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/__init__.py
+-rw-r--r--   0        0        0     1106 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/assembly.py
+-rw-r--r--   0        0        0     5052 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/case.py
+-rw-r--r--   0        0        0     2150 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/component.py
+-rw-r--r--   0        0        0    14284 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/cpu.py
+-rw-r--r--   0        0        0     1460 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/hdd.py
+-rw-r--r--   0        0        0      941 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/motherboard.py
+-rw-r--r--   0        0        0     2004 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/power_supply.py
+-rw-r--r--   0        0        0     7197 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/ram.py
+-rw-r--r--   0        0        0     4960 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/component/ssd.py
+-rw-r--r--   0        0        0       88 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/consumption_profile/__init__.py
+-rw-r--r--   0        0        0     7244 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/consumption_profile/consumption_profile.py
+-rw-r--r--   0        0        0       81 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/device/__init__.py
+-rw-r--r--   0        0        0     1134 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/device/device.py
+-rw-r--r--   0        0        0     8965 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/device/server.py
+-rw-r--r--   0        0        0     7261 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/device/userTerminal.py
+-rw-r--r--   0        0        0     3983 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/impact.py
+-rw-r--r--   0        0        0       65 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/usage/__init__.py
+-rw-r--r--   0        0        0     8503 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/model/usage/usage.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/__init__.py
+-rw-r--r--   0        0        0     4052 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/cloud_router.py
+-rw-r--r--   0        0        0    17594 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/component_router.py
+-rw-r--r--   0        0        0      958 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/consumption_profile_router.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/openapi_doc/__init__.py
+-rw-r--r--   0        0        0     9638 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/openapi_doc/descriptions.py
+-rw-r--r--   0        0        0     2624 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/openapi_doc/examples.py
+-rw-r--r--   0        0        0     2207 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/openapi_doc/intro_openapi.md
+-rw-r--r--   0        0        0     8625 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/peripheral_router.py
+-rw-r--r--   0        0        0     3612 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/server_router.py
+-rw-r--r--   0        0        0    13529 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/terminal_router.py
+-rw-r--r--   0        0        0     2864 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/routers/utils_router.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/service/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/service/allocation.py
+-rw-r--r--   0        0        0     4276 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/service/archetype.py
+-rw-r--r--   0        0        0     2199 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/service/bottom_up.py
+-rw-r--r--   0        0        0     3280 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/service/factor_provider.py
+-rw-r--r--   0        0        0     2646 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/service/verbose.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/utils/__init__.py
+-rw-r--r--   0        0        0     1405 2023-06-30 14:28:51.761469 boaviztapi-1.0.0a4/boaviztapi/utils/fuzzymatch.py
+-rw-r--r--   0        0        0     3257 2023-06-30 14:28:51.765469 boaviztapi-1.0.0a4/boaviztapi/utils/roundit.py
+-rw-r--r--   0        0        0      728 2023-06-30 14:28:51.781470 boaviztapi-1.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     5604 1970-01-01 00:00:00.000000 boaviztapi-1.0.0a4/PKG-INFO
```

### Comparing `boaviztapi-1.0.0a3/LICENSE` & `boaviztapi-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/README.md` & `boaviztapi-1.0.0a4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-    <img src="https://raw.githubusercontent.com/Boavizta/boaviztapi/dev/boavizta-logo-4.png" width="100">
+    <img src="https://github.com/Boavizta/boaviztapi/blob/af7ca450518a2108f907736222a540908a258368/boavizta-logo-4.png" width="100">
 </p>
 <h1 align="center">
   Boavizta API
 </h1>
 
 ---
 
@@ -87,25 +87,35 @@
 ```
 
 You can run the tests with `pytest`.
 
 ### Create your own docker image and run it
 
 Build application package
+
 ```sh
 make install
 ```
+
 Build docker image
+
 ```sh
-$ make docker-build
+# using the makefile (recommended)
+make docker-build
+
+# manual build (requires to set version)
+docker build --build-arg VERSION=`poetry version -s` .
 ```
+
 Run docker image
+
 ```sh
 docker run -p 5000:5000/tcp boavizta/boaviztapi:0.2.0
 ```
+
 ### Deploy to AWS as serverless application
 
 Api can be self hosted to your own AWS account using the serverless framework.
 
 ```sh
 # Install the serverless framework and plugins
 npm install -g serverless
```

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/archetypes/cloud/aws.csv` & `boaviztapi-1.0.0a4/boaviztapi/data/archetypes/cloud/aws.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/archetypes/cloud/gcp.csv` & `boaviztapi-1.0.0a4/boaviztapi/data/archetypes/cloud/gcp.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/archetypes/server.csv` & `boaviztapi-1.0.0a4/boaviztapi/data/archetypes/server.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/archetypes/user_terminal.csv` & `boaviztapi-1.0.0a4/boaviztapi/data/archetypes/user_terminal.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/config.yml` & `boaviztapi-1.0.0a4/boaviztapi/data/config.yml`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/ademe_base_impacts_negaoctet.csv` & `boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/ademe_base_impacts_negaoctet.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/cpu_manufacture.csv` & `boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/cpu_manufacture.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/cpu_specs.csv` & `boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/cpu_specs.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/electrical_mix.csv` & `boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/electrical_mix.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/crowdsourcing/ssd_manufacture.csv` & `boaviztapi-1.0.0a4/boaviztapi/data/crowdsourcing/ssd_manufacture.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/factors.yml` & `boaviztapi-1.0.0a4/boaviztapi/data/factors.yml`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/data/utils/jsonifyer.py` & `boaviztapi-1.0.0a4/boaviztapi/data/utils/jsonifyer.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/dto/component/cpu.py` & `boaviztapi-1.0.0a4/boaviztapi/dto/component/cpu.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/dto/component/disk.py` & `boaviztapi-1.0.0a4/boaviztapi/dto/component/disk.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/dto/component/other.py` & `boaviztapi-1.0.0a4/boaviztapi/dto/component/other.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/dto/component/ram.py` & `boaviztapi-1.0.0a4/boaviztapi/dto/component/ram.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/dto/consumption_profile/consumption_profile.py` & `boaviztapi-1.0.0a4/boaviztapi/dto/consumption_profile/consumption_profile.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/dto/device/device.py` & `boaviztapi-1.0.0a4/boaviztapi/dto/device/device.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/dto/device/user_terminal.py` & `boaviztapi-1.0.0a4/boaviztapi/dto/device/user_terminal.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/dto/usage/usage.py` & `boaviztapi-1.0.0a4/boaviztapi/dto/usage/usage.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/main.py` & `boaviztapi-1.0.0a4/boaviztapi/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
+import subprocess
 
 import markdown
+import toml
 from fastapi.middleware.cors import CORSMiddleware
 import os
-import pkg_resources
 from fastapi import FastAPI
 from fastapi.openapi.utils import get_openapi
 from mangum import Mangum
 
 from boaviztapi.routers.component_router import component_router
 from boaviztapi.routers.consumption_profile_router import consumption_profile
 from boaviztapi.routers.peripheral_router import peripheral_router
@@ -19,15 +20,16 @@
 from fastapi.responses import HTMLResponse
 
 # Serverless frameworks adds a 'stage' prefix to the route used to serve applications
 # We have to manage it to expose openapi doc on aws and generate proper links.
 stage = os.environ.get('STAGE', None)
 openapi_prefix = f"/{stage}" if stage else "/"
 app = FastAPI(root_path=openapi_prefix)  # Here is the magic
-version = pkg_resources.get_distribution('boaviztapi').version
+version = toml.loads(open(os.path.join(os.path.dirname(__file__), '../pyproject.toml'), 'r').read())['tool']['poetry']['version']
+
 
 origins = json.loads(os.getenv("ALLOWED_ORIGINS", '["*"]'))
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
     allow_methods=["*"],
@@ -65,18 +67,23 @@
 
 # Wrapper for aws/lambda serverless app
 handler = Mangum(app)
 
 
 @app.get("/", response_class=HTMLResponse)
 async def welcome_page():
-    html_content = f"""
+    html_content = """
     <html>
         <head>
             <title>BOAVIZTAPI</title>
+            <style>
+                * {
+                    font-family: sans-serif;
+                }
+            </style>
         </head>
         <body>
             <p align="center">
                 <img src="https://boavizta.org/media/site/d84925bc94-1642413712/boavizta-logo-4.png" width="100">
             </p>
             <h1 align="center">
               Welcome to BOAVIZTAPI
```

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/boattribute.py` & `boaviztapi-1.0.0a4/boaviztapi/model/boattribute.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/component/assembly.py` & `boaviztapi-1.0.0a4/boaviztapi/model/component/assembly.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/component/case.py` & `boaviztapi-1.0.0a4/boaviztapi/model/component/case.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/component/component.py` & `boaviztapi-1.0.0a4/boaviztapi/model/component/component.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/component/cpu.py` & `boaviztapi-1.0.0a4/boaviztapi/model/component/cpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from boaviztapi.model.component.component import Component
 from boaviztapi.model.consumption_profile import CPUConsumptionProfileModel
 from boaviztapi.model.impact import ImpactFactor
 from boaviztapi.service.archetype import get_component_archetype, get_arch_value
 from boaviztapi.service.factor_provider import get_impact_factor
 from boaviztapi.utils.fuzzymatch import fuzzymatch_attr_from_pdf, fuzzymatch_attr_from_cpu_name
 
-
 _cpu_specs = pd.read_csv(os.path.join(data_dir, 'crowdsourcing/cpu_specs.csv'))
 _family_df = pd.read_csv(os.path.join(data_dir, 'crowdsourcing/cpu_manufacture.csv'))
 
 
 def attributes_from_cpu_name(cpu_name: str):
     return fuzzymatch_attr_from_cpu_name(cpu_name, _cpu_specs)
 
@@ -246,9 +245,10 @@
             if model_range is not None:
                 self.model_range.set_completed(model_range, min=model_range_min, max=model_range_max, source=f"Completed from name name based on {source}.")
             if tdp is not None:
                 self.tdp.set_completed(tdp, min=tdp_min, max=tdp_max, source=f"Completed from name name based on {source}.")
             if cores is not None:
                 self.core_units.set_completed(cores, min=cores_min, max=cores_max, source=f"Completed from name name based on {source}.")
             if die_size is not None:
-                self.die_size.set_completed(die_size/1000, min=die_size_min/1000, max=die_size_max/1000, source=f"{die_size_source} : Completed from name name based on {source}.")
+                # divide by 100 to convert mm2 into cm2
+                self.die_size.set_completed(die_size/100, min=die_size_min/100, max=die_size_max/100, source=f"{die_size_source} : Completed from name name based on {source}.")
             self.name_completion = True
```

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/component/hdd.py` & `boaviztapi-1.0.0a4/boaviztapi/model/component/hdd.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/component/motherboard.py` & `boaviztapi-1.0.0a4/boaviztapi/model/component/motherboard.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/component/power_supply.py` & `boaviztapi-1.0.0a4/boaviztapi/model/component/power_supply.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/component/ram.py` & `boaviztapi-1.0.0a4/boaviztapi/model/component/ram.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/component/ssd.py` & `boaviztapi-1.0.0a4/boaviztapi/model/component/ssd.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/consumption_profile/consumption_profile.py` & `boaviztapi-1.0.0a4/boaviztapi/model/consumption_profile/consumption_profile.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/device/device.py` & `boaviztapi-1.0.0a4/boaviztapi/model/device/device.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/device/server.py` & `boaviztapi-1.0.0a4/boaviztapi/model/device/server.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/device/userTerminal.py` & `boaviztapi-1.0.0a4/boaviztapi/model/device/userTerminal.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/impact.py` & `boaviztapi-1.0.0a4/boaviztapi/model/impact.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/model/usage/usage.py` & `boaviztapi-1.0.0a4/boaviztapi/model/usage/usage.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/cloud_router.py` & `boaviztapi-1.0.0a4/boaviztapi/routers/cloud_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/component_router.py` & `boaviztapi-1.0.0a4/boaviztapi/routers/component_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                        description=cpu_description)
 async def cpu_all_archetype_name():
     archetype_lst = get_all_archetype_name("cpu")
     return archetype_lst
 
 @component_router.get('/cpu/archetype_config',
                        description=cpu_description)
-async def cpu_archetype_config(archetype: str = Query(Exemple=config["default_cpu"])):
+async def cpu_archetype_config(archetype: str = Query(example=config["default_cpu"])):
     archetype_config = get_archetype_config(archetype,"cpu")
     return archetype_config
 
 @component_router.post('/cpu',
                        description=cpu_description)
 async def cpu_impact_bottom_up(cpu: CPU = Body(None, example=components_examples["cpu"]),
                                verbose: bool = True,
@@ -91,15 +91,15 @@
                        description=ram_description)
 async def ram_all_archetype_name():
     archetype_lst = get_all_archetype_name("ram")
     return archetype_lst
 
 @component_router.get('/ram/archetype_config',
                        description=ram_description)
-async def ram_archetype_config(archetype: str = Query(Exemple=config["default_ram"])):
+async def ram_archetype_config(archetype: str = Query(example=config["default_ram"])):
     archetype_config = get_archetype_config(archetype,"ram")
     return archetype_config
 
 @component_router.post('/ram',
                        description=ram_description)
 async def ram_impact_bottom_up(ram: RAM = Body(None, example=components_examples["ram"]),
                                verbose: bool = True,
@@ -144,15 +144,15 @@
                        description=ssd_description)
 async def ssd_all_archetype_name():
     archetype_lst = get_all_archetype_name("ssd")
     return archetype_lst
 
 @component_router.get('/ssd/archetype_config',
                        description=ssd_description)
-async def ssd_archetype_config(archetype: str = Query(Exemple=config["default_ssd"])):
+async def ssd_archetype_config(archetype: str = Query(example=config["default_ssd"])):
     archetype_config = get_archetype_config(archetype,"ssd")
     return archetype_config
 
 @component_router.post('/ssd',
                        description=ssd_description)
 async def disk_impact_bottom_up(disk: Disk = Body(None, example=components_examples["ssd"]),
                                 verbose: bool = True,
@@ -200,15 +200,15 @@
                        description=hdd_description)
 async def hdd_all_archetype_name():
     archetype_lst = get_all_archetype_name("hdd")
     return archetype_lst
 
 @component_router.get('/hdd/archetype_config',
                        description=hdd_description)
-async def hdd_archetype_config(archetype: str = Query(Exemple=config["default_hdd"])):
+async def hdd_archetype_config(archetype: str = Query(example=config["default_hdd"])):
     archetype_config = get_archetype_config(archetype,"hdd")
     return archetype_config
 
 @component_router.post('/hdd',
                        description=hdd_description)
 async def disk_impact_bottom_up(disk: Disk = Body(None, example=components_examples["hdd"]),
                                 verbose: bool = True,
@@ -256,15 +256,15 @@
                        description=motherboard_description)
 async def motherboard_all_archetype_name():
     archetype_lst = get_all_archetype_name("motherboard")
     return archetype_lst
 
 @component_router.get('/motherboard/archetype_config',
                        description=motherboard_description)
-async def motherboard_archetype_config(archetype: str = Query(Exemple=config["default_motherboard"])):
+async def motherboard_archetype_config(archetype: str = Query(example=config["default_motherboard"])):
     archetype_config = get_archetype_config(archetype,"motherboard")
     return archetype_config
 
 
 @component_router.post('/motherboard',
                        description=motherboard_description)
 async def motherboard_impact_bottom_up(motherboard: Motherboard = Body(None, example=components_examples["motherboard"]),
@@ -300,15 +300,15 @@
                        description=power_supply_description)
 async def power_supply_all_archetype_name():
     archetype_lst = get_all_archetype_name("power_supply")
     return archetype_lst
 
 @component_router.get('/power_supply/archetype_config',
                        description=power_supply_description)
-async def power_supply_archetype_config(archetype: str = Query(Exemple=config["default_power_supply"])):
+async def power_supply_archetype_config(archetype: str = Query(example=config["default_power_supply"])):
     archetype_config = get_archetype_config(archetype,"power_supply")
     return archetype_config
 
 
 @component_router.post('/power_supply',
                        description=power_supply_description)
 async def power_supply_impact_bottom_up(power_supply: PowerSupply = Body(None, example=components_examples["power_supply"]),
@@ -356,15 +356,15 @@
                        description=case_description)
 async def case_all_archetype_name():
     archetype_lst = get_all_archetype_name("case")
     return archetype_lst
 
 @component_router.get('/case/archetype_config',
                        description=case_description)
-async def case_archetype_config(archetype: str = Query(Exemple=config["default_case"])):
+async def case_archetype_config(archetype: str = Query(example=config["default_case"])):
     archetype_config = get_archetype_config(archetype,"case")
     return archetype_config
 
 @component_router.post('/case',
                        description=case_description)
 async def case_impact_bottom_up(case: Case = Body(None, example=components_examples["case"]),
                                 verbose: bool = True,
```

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/consumption_profile_router.py` & `boaviztapi-1.0.0a4/boaviztapi/routers/consumption_profile_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/openapi_doc/descriptions.py` & `boaviztapi-1.0.0a4/boaviztapi/routers/openapi_doc/descriptions.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/openapi_doc/examples.py` & `boaviztapi-1.0.0a4/boaviztapi/routers/openapi_doc/examples.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/openapi_doc/intro_openapi.md` & `boaviztapi-1.0.0a4/boaviztapi/routers/openapi_doc/intro_openapi.md`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/peripheral_router.py` & `boaviztapi-1.0.0a4/boaviztapi/routers/peripheral_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/server_router.py` & `boaviztapi-1.0.0a4/boaviztapi/routers/server_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 @server_router.get('/archetypes',
                    description=all_archetype_servers)
 async def server_get_all_archetype_name():
     return get_device_archetype_lst(os.path.join(data_dir, 'archetypes/server.csv'))
 
 @server_router.get('/archetype_config',
                    description=get_archetype_config_desc)
-async def get_archetype_config(archetype: str = Query(exemple=config["default_server"])):
+async def get_archetype_config(archetype: str = Query(example=config["default_server"])):
     result = get_server_archetype(archetype)
     if not result:
         raise HTTPException(status_code=404, detail=f"{archetype} not found")
     return result
 
 @server_router.get('/',
                    description=server_impact_by_model_description)
```

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/terminal_router.py` & `boaviztapi-1.0.0a4/boaviztapi/routers/terminal_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/routers/utils_router.py` & `boaviztapi-1.0.0a4/boaviztapi/routers/utils_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/service/allocation.py` & `boaviztapi-1.0.0a4/boaviztapi/service/allocation.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/service/archetype.py` & `boaviztapi-1.0.0a4/boaviztapi/service/archetype.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/service/bottom_up.py` & `boaviztapi-1.0.0a4/boaviztapi/service/bottom_up.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/service/factor_provider.py` & `boaviztapi-1.0.0a4/boaviztapi/service/factor_provider.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/service/verbose.py` & `boaviztapi-1.0.0a4/boaviztapi/service/verbose.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/utils/fuzzymatch.py` & `boaviztapi-1.0.0a4/boaviztapi/utils/fuzzymatch.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/boaviztapi/utils/roundit.py` & `boaviztapi-1.0.0a4/boaviztapi/utils/roundit.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a3/pyproject.toml` & `boaviztapi-1.0.0a4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boaviztapi"
-version = "1.0.0a3"
+version = "1.0.0a4"
 description = "An API to access Boavizta's methodologies and footprint reference data"
 authors = []
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = '^1.10'
@@ -14,14 +14,16 @@
 aiofile = '^3.8'
 numpy = "^1.24"
 scipy = "^1.9"
 rapidfuzz = "^3.0"
 markdown = "^3.4"
 mangum = "^0.17"
 importlib-metadata = "^6.6.0"
+pyyaml = "^6.0"
+toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = '*'
 pytest = '*'
 atomicwrites = "*"
 mkdocs-material = "*"
 httpx = '*'
```

### Comparing `boaviztapi-1.0.0a3/PKG-INFO` & `boaviztapi-1.0.0a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boaviztapi
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: An API to access Boavizta's methodologies and footprint reference data
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,21 +12,23 @@
 Requires-Dist: fastapi (>=0.95,<0.96)
 Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
 Requires-Dist: mangum (>=0.17,<0.18)
 Requires-Dist: markdown (>=3.4,<4.0)
 Requires-Dist: numpy (>=1.24,<2.0)
 Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rapidfuzz (>=3.0,<4.0)
 Requires-Dist: scipy (>=1.9,<2.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: uvicorn (>=0.22,<0.23)
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/Boavizta/boaviztapi/dev/boavizta-logo-4.png" width="100">
+    <img src="https://github.com/Boavizta/boaviztapi/blob/af7ca450518a2108f907736222a540908a258368/boavizta-logo-4.png" width="100">
 </p>
 <h1 align="center">
   Boavizta API
 </h1>
 
 ---
 
@@ -110,25 +112,35 @@
 ```
 
 You can run the tests with `pytest`.
 
 ### Create your own docker image and run it
 
 Build application package
+
 ```sh
 make install
 ```
+
 Build docker image
+
 ```sh
-$ make docker-build
+# using the makefile (recommended)
+make docker-build
+
+# manual build (requires to set version)
+docker build --build-arg VERSION=`poetry version -s` .
 ```
+
 Run docker image
+
 ```sh
 docker run -p 5000:5000/tcp boavizta/boaviztapi:0.2.0
 ```
+
 ### Deploy to AWS as serverless application
 
 Api can be self hosted to your own AWS account using the serverless framework.
 
 ```sh
 # Install the serverless framework and plugins
 npm install -g serverless
```

