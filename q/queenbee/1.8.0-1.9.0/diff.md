# Comparing `tmp/queenbee-1.8.0.tar.gz` & `tmp/queenbee-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/queenbee-1.8.0.tar", last modified: Thu Jan 23 17:50:34 2020, max compression
+gzip compressed data, was "dist/queenbee-1.9.0.tar", last modified: Sun Feb 23 03:41:33 2020, max compression
```

## Comparing `queenbee-1.8.0.tar` & `queenbee-1.9.0.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      675 2020-01-23 17:49:43.000000 queenbee-1.8.0/docs/index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-23 17:49:43.000000 queenbee-1.8.0/docs/.nojekyll
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-01-23 17:49:43.000000 queenbee-1.8.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       44 2020-01-23 17:49:43.000000 queenbee-1.8.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    18576 2020-01-23 17:50:34.000000 queenbee-1.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-01-23 17:49:43.000000 queenbee-1.8.0/.releaserc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    14577 2020-01-23 17:49:43.000000 queenbee-1.8.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2020-01-23 17:49:43.000000 queenbee-1.8.0/docs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/queenbee.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18576 2020-01-23 17:50:33.000000 queenbee-1.8.0/queenbee.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-23 17:50:33.000000 queenbee-1.8.0/queenbee.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-01-23 17:50:33.000000 queenbee-1.8.0/queenbee.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1978 2020-01-23 17:50:33.000000 queenbee-1.8.0/queenbee.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2020-01-23 17:50:33.000000 queenbee-1.8.0/queenbee.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-01-23 17:50:33.000000 queenbee-1.8.0/queenbee.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      212 2020-01-23 17:49:43.000000 queenbee-1.8.0/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-01-23 17:49:43.000000 queenbee-1.8.0/CONTRIBUTING.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/queenbee/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/queenbee/schema/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3870 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/artifact_location.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8898 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/arguments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4327 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/variable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2915 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14889 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/workflow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5650 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/dag.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1963 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/qutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       39 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      682 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/operator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3183 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4380 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/schema/function.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4410 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2674 2020-01-23 17:49:43.000000 queenbee-1.8.0/queenbee/_openapi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-01-23 17:50:34.000000 queenbee-1.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2020-01-23 17:49:43.000000 queenbee-1.8.0/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1070 2020-01-23 17:49:43.000000 queenbee-1.8.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      229 2020-01-23 17:49:43.000000 queenbee-1.8.0/dev-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1153 2020-01-23 17:49:43.000000 queenbee-1.8.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-01-23 17:49:43.000000 queenbee-1.8.0/deploy.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/tests/schema/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3314 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/schema/artifact_location_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2094 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/schema/arguments_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/schema/dag_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/schema/import_from_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      880 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/schema/function_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1235 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/schema/parameters_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4787 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/schema/workflow_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/schema/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      917 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/schema/operator_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/tests/assets/
--rw-rw-r--   0 travis    (2000) travis    (2000)      472 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/function_illegal_input.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/arguments_dup_name.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      251 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/arguments.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/flow_invalid_loop.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      491 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/function_workflow_reference.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/function.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      540 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/function_referenced_input.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/tests/assets/import_from/
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/import_from/radiance_app.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/import_from/radiance_operator.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      118 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/import_from/base.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      661 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/flow_with_wrong_target.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/parameters.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/operator.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/function_int_input.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-23 17:50:34.000000 queenbee-1.8.0/tests/assets/workflow_example/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/workflow_example/daylightfactor.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     6428 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/workflow_example/double_run_folder.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/workflow_example/radiance_app.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/workflow_example/radiance_operator.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     5094 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/workflow_example/daylightfactor_invalid_location.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/workflow_example/honeybee_radiance_operator.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      641 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/flow.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/assets/artifact_locations.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2020-01-23 17:49:43.000000 queenbee-1.8.0/tests/conftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      675 2020-02-23 03:40:39.000000 queenbee-1.9.0/docs/index.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-23 03:40:39.000000 queenbee-1.9.0/docs/.nojekyll
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-02-23 03:40:39.000000 queenbee-1.9.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       44 2020-02-23 03:40:39.000000 queenbee-1.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18576 2020-02-23 03:41:33.000000 queenbee-1.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-02-23 03:40:39.000000 queenbee-1.9.0/.releaserc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14577 2020-02-23 03:40:39.000000 queenbee-1.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      239 2020-02-23 03:40:39.000000 queenbee-1.9.0/docs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/queenbee.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18576 2020-02-23 03:41:33.000000 queenbee-1.9.0/queenbee.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-23 03:41:33.000000 queenbee-1.9.0/queenbee.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-02-23 03:41:33.000000 queenbee-1.9.0/queenbee.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2031 2020-02-23 03:41:33.000000 queenbee-1.9.0/queenbee.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2020-02-23 03:41:33.000000 queenbee-1.9.0/queenbee.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-02-23 03:41:33.000000 queenbee-1.9.0/queenbee.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      212 2020-02-23 03:40:39.000000 queenbee-1.9.0/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-02-23 03:40:39.000000 queenbee-1.9.0/CONTRIBUTING.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/queenbee/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/queenbee/schema/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3870 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/artifact_location.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9302 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/arguments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4327 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/variable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2915 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1501 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15151 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/workflow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5650 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/dag.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1963 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/qutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       39 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      682 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/operator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3183 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4380 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/schema/function.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4410 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2674 2020-02-23 03:40:39.000000 queenbee-1.9.0/queenbee/_openapi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-02-23 03:41:33.000000 queenbee-1.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2020-02-23 03:40:39.000000 queenbee-1.9.0/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1070 2020-02-23 03:40:39.000000 queenbee-1.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      229 2020-02-23 03:40:39.000000 queenbee-1.9.0/dev-requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1153 2020-02-23 03:40:39.000000 queenbee-1.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-02-23 03:40:39.000000 queenbee-1.9.0/deploy.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/tests/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/tests/schema/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3314 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/artifact_location_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2094 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/arguments_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      565 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/dag_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      469 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/import_from_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      528 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      880 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/function_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1235 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/parameters_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4787 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/workflow_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      917 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/schema/operator_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/tests/assets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      472 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/function_illegal_input.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/arguments_dup_name.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      251 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/arguments.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      565 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/flow_invalid_loop.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      491 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/function_workflow_reference.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      495 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/function.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      540 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/function_referenced_input.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/tests/assets/import_from/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      140 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/import_from/radiance_app.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/import_from/radiance_operator.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      118 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/import_from/base.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      661 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/flow_with_wrong_target.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      164 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/parameters.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/operator.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/function_int_input.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-23 03:41:33.000000 queenbee-1.9.0/tests/assets/workflow_example/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/workflow_example/daylightfactor.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6428 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/workflow_example/double_run_folder.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       78 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/workflow_example/radiance_app.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/workflow_example/radiance_operator.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5094 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/workflow_example/daylightfactor_invalid_location.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       92 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/workflow_example/honeybee_radiance_operator.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      641 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/flow.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/assets/artifact_locations.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2020-02-23 03:40:39.000000 queenbee-1.9.0/tests/conftest.py
```

### Comparing `queenbee-1.8.0/docs/index.html` & `queenbee-1.9.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/PKG-INFO` & `queenbee-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee
-Version: 1.8.0
+Version: 1.9.0
 Summary: Queenbee is a workflow language for creating DAG workflows which empowers all workflow libraries in Ladybug Tools!
 Home-page: https://github.com/ladybug-tools/queenbee
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: # queenbee
```

### Comparing `queenbee-1.8.0/README.md` & `queenbee-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee.egg-info/PKG-INFO` & `queenbee-1.9.0/queenbee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee
-Version: 1.8.0
+Version: 1.9.0
 Summary: Queenbee is a workflow language for creating DAG workflows which empowers all workflow libraries in Ladybug Tools!
 Home-page: https://github.com/ladybug-tools/queenbee
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: # queenbee
```

### Comparing `queenbee-1.8.0/queenbee.egg-info/SOURCES.txt` & `queenbee-1.9.0/queenbee.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 queenbee.egg-info/requires.txt
 queenbee.egg-info/top_level.txt
 queenbee/schema/__init__.py
 queenbee/schema/arguments.py
 queenbee/schema/artifact_location.py
 queenbee/schema/dag.py
 queenbee/schema/function.py
+queenbee/schema/metadata.py
 queenbee/schema/operator.py
 queenbee/schema/parser.py
 queenbee/schema/qutil.py
 queenbee/schema/status.py
 queenbee/schema/variable.py
 queenbee/schema/workflow.py
 tests/__init__.py
@@ -59,10 +60,11 @@
 tests/assets/workflow_example/radiance_operator.yaml
 tests/schema/__init__.py
 tests/schema/arguments_test.py
 tests/schema/artifact_location_test.py
 tests/schema/dag_test.py
 tests/schema/function_test.py
 tests/schema/import_from_test.py
+tests/schema/metadata.py
 tests/schema/operator_test.py
 tests/schema/parameters_test.py
 tests/schema/workflow_test.py
```

### Comparing `queenbee-1.8.0/queenbee/schema/artifact_location.py` & `queenbee-1.9.0/queenbee/schema/artifact_location.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee/schema/arguments.py` & `queenbee-1.9.0/queenbee/schema/arguments.py`

 * *Files 5% similar despite different names*

```diff
@@ -280,7 +280,20 @@
         if self.parameters:
             ref_values['parameters'] = [
                 {par.name: par.referenced_values} for par in self.parameters
                 if par.referenced_values
             ]
 
         return ref_values
+
+
+class WorkflowArguments(Arguments):
+    """A workflow arguments object.
+
+    The difference between the workflow argument and a standard argument is the extra
+    field for user_data.
+    """
+    user_data: Dict = Field(
+        None,
+        description='Optional user data as a dictionary. User data is for user reference'
+        ' only and will not be used in the execution of the workflow.'
+    )
```

### Comparing `queenbee-1.8.0/queenbee/schema/variable.py` & `queenbee-1.9.0/queenbee/schema/variable.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee/schema/parser.py` & `queenbee-1.9.0/queenbee/schema/parser.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee/schema/workflow.py` & `queenbee-1.9.0/queenbee/schema/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,39 +3,46 @@
 Workflow is a collection of operators and inter-related tasks that describes an end to
 end steps for the workflow.
 """
 from uuid import uuid4
 import collections
 import re
 from graphviz import Digraph
-from pydantic import Field, validator, constr, root_validator
+from pydantic import Field, validator, constr
 from typing import List, Union
 from queenbee.schema.qutil import BaseModel
 from queenbee.schema.dag import DAG
-from queenbee.schema.arguments import Arguments
+from queenbee.schema.arguments import Arguments, WorkflowArguments
 from queenbee.schema.operator import Operator
 from queenbee.schema.function import Function
 from queenbee.schema.artifact_location import RunFolderLocation, InputFolderLocation, \
     HTTPLocation, S3Location
 from queenbee.schema.parser import parse_double_quote_workflow_vars, \
     replace_double_quote_vars
+from queenbee.schema.metadata import MetaData
 import queenbee.schema.variable as qbvar
 
 
 class Workflow(BaseModel):
     """A DAG Workflow."""
 
     type: constr(regex='^workflow$')
 
     name: str
 
     id: str = str(uuid4())
 
-    inputs: Arguments = Field(
-        None
+    metadata: MetaData = Field(
+        None,
+        description='Workflow metadata information.'
+    )
+
+    inputs: WorkflowArguments = Field(
+        None,
+        description='Workflow input arguments.'
     )
 
     operators: List[Operator]
 
     templates: List[Union[Function, DAG, 'Workflow']] = Field(
         ...,
         description='A list of templates. Templates can be Function, DAG or a Workflow.'
@@ -43,15 +50,16 @@
 
     flow: DAG = Field(
         ...,
         description='A list of tasks to create a DAG workflow.'
     )
 
     outputs: Arguments = Field(
-        None
+        None,
+        description='Workflow output arguments.'
     )
 
     artifact_locations: List[
         Union[RunFolderLocation, InputFolderLocation, HTTPLocation, S3Location]
     ] = Field(
         None,
         description='A list of artifact locations which can be used by flow objects.'
```

### Comparing `queenbee-1.8.0/queenbee/schema/dag.py` & `queenbee-1.9.0/queenbee/schema/dag.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee/schema/qutil.py` & `queenbee-1.9.0/queenbee/schema/qutil.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee/schema/operator.py` & `queenbee-1.9.0/queenbee/schema/operator.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee/schema/status.py` & `queenbee-1.9.0/queenbee/schema/status.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee/schema/function.py` & `queenbee-1.9.0/queenbee/schema/function.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee/cli.py` & `queenbee-1.9.0/queenbee/cli.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/queenbee/_openapi.py` & `queenbee-1.9.0/queenbee/_openapi.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/.travis.yml` & `queenbee-1.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/LICENSE` & `queenbee-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/setup.py` & `queenbee-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/schema/artifact_location_test.py` & `queenbee-1.9.0/tests/schema/artifact_location_test.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/schema/arguments_test.py` & `queenbee-1.9.0/tests/schema/arguments_test.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/schema/dag_test.py` & `queenbee-1.9.0/tests/schema/dag_test.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/schema/function_test.py` & `queenbee-1.9.0/tests/schema/function_test.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/schema/parameters_test.py` & `queenbee-1.9.0/tests/schema/parameters_test.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/schema/workflow_test.py` & `queenbee-1.9.0/tests/schema/workflow_test.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/schema/operator_test.py` & `queenbee-1.9.0/tests/schema/operator_test.py`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/assets/flow_invalid_loop.yaml` & `queenbee-1.9.0/tests/assets/flow_invalid_loop.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/assets/function_referenced_input.yaml` & `queenbee-1.9.0/tests/assets/function_referenced_input.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/assets/flow_with_wrong_target.yaml` & `queenbee-1.9.0/tests/assets/flow_with_wrong_target.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/assets/function_int_input.yaml` & `queenbee-1.9.0/tests/assets/function_int_input.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/assets/workflow_example/daylightfactor.yaml` & `queenbee-1.9.0/tests/assets/workflow_example/daylightfactor.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/assets/workflow_example/double_run_folder.yaml` & `queenbee-1.9.0/tests/assets/workflow_example/double_run_folder.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/assets/workflow_example/daylightfactor_invalid_location.yaml` & `queenbee-1.9.0/tests/assets/workflow_example/daylightfactor_invalid_location.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-1.8.0/tests/assets/flow.yaml` & `queenbee-1.9.0/tests/assets/flow.yaml`

 * *Files identical despite different names*

