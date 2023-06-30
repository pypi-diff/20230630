# Comparing `tmp/nf-core-2.8.tar.gz` & `tmp/nf-core-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nf-core-2.8.tar", last modified: Fri Apr 28 14:12:19 2023, max compression
+gzip compressed data, was "nf-core-2.9.tar", last modified: Fri Jun 30 16:12:27 2023, max compression
```

## Comparing `nf-core-2.8.tar` & `nf-core-2.9.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.062879 nf-core-2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-28 14:11:53.000000 nf-core-2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-28 14:11:53.000000 nf-core-2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    65673 2023-04-28 14:12:19.062879 nf-core-2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    65246 2023-04-28 14:11:53.000000 nf-core-2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.026879 nf-core-2.8/nf_core/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/.pre-commit-prettier-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53727 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/bump_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.030879 nf-core-2.8/nf_core/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/components_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/components_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/components_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/create.py
--rw-r--r--   0 runner    (1001) docker     (123)    13859 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    23874 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/create.py
--rw-r--r--   0 runner    (1001) docker     (123)    37152 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    31865 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/licences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.034879 nf-core-2.8/nf_core/lint/
--rw-r--r--   0 runner    (1001) docker     (123)    23357 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/actions_awsfulltest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/actions_awstest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/actions_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/actions_schema_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/files_exist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/files_unchanged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/merge_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/modules_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/modules_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/multiqc_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/nextflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/pipeline_name_conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/pipeline_todos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/schema_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/schema_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/schema_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/system_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/template_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/version_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/module-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.034879 nf-core-2.8/nf_core/module-template/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/modules/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/modules/meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.034879 nf-core-2.8/nf_core/module-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/tests/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/tests/nextflow.config
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/tests/test.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.038879 nf-core-2.8/nf_core/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/bump_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/modules/lint/
--rw-r--r--   0 runner    (1001) docker     (123)    17255 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24400 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/main_nf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/meta_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_todos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18275 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)    54053 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/nfcore_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    15466 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/test_yml_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/pipeline-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/pipeline-template/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/pipeline-template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/.dockstore.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/awsfulltest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/awstest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/branch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/clean-up.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/fix-linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/linting_comment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.gitpod.yml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.nf-core.yml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/CITATIONS.md
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/adaptivecard.json
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/email_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/email_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/methods_description_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/multiqc_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/samplesheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/schema_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/sendmail_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/slackreport.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9429 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/bin/check_samplesheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/base.config
--rw-r--r--   0 runner    (1001) docker     (123)    35656 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/igenomes.config
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/modules.config
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/test.config
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/test_full.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/docs/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23458 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_adapter.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    33918 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_counts.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    55769 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_quality.png
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/output.md
--rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22038 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/NfcoreSchema.groovy
--rwxr-xr-x   0 runner    (1001) docker     (123)    16592 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/NfcoreTemplate.groovy
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/Utils.groovy
--rwxr-xr-x   0 runner    (1001) docker     (123)     3876 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/WorkflowMain.groovy
--rwxr-xr-x   0 runner    (1001) docker     (123)     3625 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/WorkflowPipeline.groovy
--rw-r--r--   0 runner    (1001) docker     (123)  2291171 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/nfcore_external_java_deps.jar
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/main.nf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/pipeline-template/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/local/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/local/samplesheet_check.nf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/dumpsoftwareversions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules.json
--rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/nextflow.config
--rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/nextflow_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/pipeline-template/subworkflows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/subworkflows/local/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/subworkflows/local/input_check.nf
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/tower.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/workflows/pipeline.nf
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/refgenie.py
--rw-r--r--   0 runner    (1001) docker     (123)    37926 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/subworkflow-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/subworkflow-template/subworkflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/subworkflows/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/subworkflows/meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/subworkflow-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/tests/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/tests/nextflow.config
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/tests/test.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.058879 nf-core-2.8/nf_core/subworkflows/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/subworkflows_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/test_yml_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    41429 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.026879 nf-core-2.8/nf_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    65673 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-04-28 14:12:19.000000 nf-core-2.8/nf_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:12:00.000000 nf-core-2.8/nf_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 14:11:53.000000 nf-core-2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 14:11:53.000000 nf-core-2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 14:12:19.062879 nf-core-2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-28 14:11:53.000000 nf-core-2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.058879 nf-core-2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.058879 nf-core-2.8/tests/lint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/actions_awsfulltest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/actions_awstest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/actions_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/actions_schema_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/files_exist.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/files_unchanged.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/merge_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/modules_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/nextflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/version_consistency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.062879 nf-core-2.8/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/bump_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/create_test_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/modules_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/modules_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    16521 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.062879 nf-core-2.8/tests/subworkflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/create_test_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/subworkflows_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_bump_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)    25709 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_lint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_refgenie.py
--rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_subworkflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    17732 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-28 14:11:53.000000 nf-core-2.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.045479 nf-core-2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-30 16:11:50.000000 nf-core-2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-30 16:11:50.000000 nf-core-2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    68425 2023-06-30 16:12:27.045479 nf-core-2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    67998 2023-06-30 16:11:50.000000 nf-core-2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:26.993474 nf-core-2.9/nf_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/.pre-commit-prettier-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55003 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/bump_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:26.997475 nf-core-2.9/nf_core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/components_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/components_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/components_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13859 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46254 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/components/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82431 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31865 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/licences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.001475 nf-core-2.9/nf_core/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)    23357 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/actions_awsfulltest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/actions_awstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/actions_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/actions_schema_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/files_exist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/files_unchanged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/merge_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/modules_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/modules_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/multiqc_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/nextflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/pipeline_name_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/pipeline_todos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/schema_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/schema_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/schema_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/system_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/template_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint/version_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/lint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:26.985474 nf-core-2.9/nf_core/module-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.001475 nf-core-2.9/nf_core/module-template/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/module-template/modules/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/module-template/modules/meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.005475 nf-core-2.9/nf_core/module-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/module-template/tests/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/module-template/tests/nextflow.config
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/module-template/tests/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.005475 nf-core-2.9/nf_core/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/bump_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.009476 nf-core-2.9/nf_core/modules/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25701 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/lint/main_nf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/lint/meta_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/lint/module_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/lint/module_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/lint/module_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/lint/module_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/lint/module_todos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/lint/module_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18275 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/modules_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54053 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/modules_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/modules_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/modules_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/modules_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/nfcore_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15466 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/test_yml_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/modules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.013476 nf-core-2.9/nf_core/pipeline-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.013476 nf-core-2.9/nf_core/pipeline-template/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.013476 nf-core-2.9/nf_core/pipeline-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/.dockstore.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.013476 nf-core-2.9/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.013476 nf-core-2.9/nf_core/pipeline-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/workflows/awsfulltest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/workflows/awstest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/workflows/branch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/workflows/clean-up.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/workflows/fix-linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.github/workflows/linting_comment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.gitpod.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.nf-core.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/CITATIONS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.017476 nf-core-2.9/nf_core/pipeline-template/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/assets/adaptivecard.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/assets/email_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/assets/email_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/assets/methods_description_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/assets/multiqc_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/assets/samplesheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/assets/schema_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/assets/sendmail_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/assets/slackreport.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.017476 nf-core-2.9/nf_core/pipeline-template/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9429 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/bin/check_samplesheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.021477 nf-core-2.9/nf_core/pipeline-template/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/conf/base.config
+-rw-r--r--   0 runner    (1001) docker     (123)    35656 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/conf/igenomes.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/conf/modules.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/conf/test.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/conf/test_full.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.021477 nf-core-2.9/nf_core/pipeline-template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.025477 nf-core-2.9/nf_core/pipeline-template/docs/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23458 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/docs/images/mqc_fastqc_adapter.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33918 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/docs/images/mqc_fastqc_counts.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55769 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/docs/images/mqc_fastqc_quality.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/docs/output.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.025477 nf-core-2.9/nf_core/pipeline-template/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16645 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/lib/NfcoreTemplate.groovy
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/lib/Utils.groovy
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2245 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/lib/WorkflowMain.groovy
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5563 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/lib/WorkflowPipeline.groovy
+-rw-r--r--   0 runner    (1001) docker     (123)  2291171 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/lib/nfcore_external_java_deps.jar
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/main.nf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:26.989474 nf-core-2.9/nf_core/pipeline-template/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.029477 nf-core-2.9/nf_core/pipeline-template/modules/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/modules/local/samplesheet_check.nf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:26.989474 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:26.989474 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/custom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.029477 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.029477 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/dumpsoftwareversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.029477 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/fastqc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/fastqc/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/fastqc/meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.029477 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/multiqc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/multiqc/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/modules/nf-core/multiqc/meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/modules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9578 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/nextflow.config
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/nextflow_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:26.989474 nf-core-2.9/nf_core/pipeline-template/subworkflows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.029477 nf-core-2.9/nf_core/pipeline-template/subworkflows/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/subworkflows/local/input_check.nf
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/tower.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.029477 nf-core-2.9/nf_core/pipeline-template/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/pipeline-template/workflows/pipeline.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/refgenie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:26.989474 nf-core-2.9/nf_core/subworkflow-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.029477 nf-core-2.9/nf_core/subworkflow-template/subworkflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflow-template/subworkflows/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflow-template/subworkflows/meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.029477 nf-core-2.9/nf_core/subworkflow-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflow-template/tests/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflow-template/tests/nextflow.config
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflow-template/tests/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.033478 nf-core-2.9/nf_core/subworkflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflows/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflows/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflows/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflows/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflows/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflows/subworkflows_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflows/test_yml_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/subworkflows/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/synced_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42968 2023-06-30 16:11:50.000000 nf-core-2.9/nf_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:26.997475 nf-core-2.9/nf_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    68425 2023-06-30 16:12:26.000000 nf-core-2.9/nf_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-06-30 16:12:26.000000 nf-core-2.9/nf_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:12:26.000000 nf-core-2.9/nf_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-30 16:12:26.000000 nf-core-2.9/nf_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:11:58.000000 nf-core-2.9/nf_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-30 16:12:26.000000 nf-core-2.9/nf_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 16:12:26.000000 nf-core-2.9/nf_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-30 16:11:50.000000 nf-core-2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-30 16:11:50.000000 nf-core-2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:12:27.045479 nf-core-2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-30 16:11:50.000000 nf-core-2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.037478 nf-core-2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:50.000000 nf-core-2.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.037478 nf-core-2.9/tests/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/actions_awsfulltest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/actions_awstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/actions_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/actions_schema_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/files_exist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/files_unchanged.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/merge_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/modules_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/nextflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-30 16:11:50.000000 nf-core-2.9/tests/lint/version_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.041478 nf-core-2.9/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/bump_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/create_test_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/modules_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/modules_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16521 2023-06-30 16:11:50.000000 nf-core-2.9/tests/modules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:12:27.045479 nf-core-2.9/tests/subworkflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:11:50.000000 nf-core-2.9/tests/subworkflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-30 16:11:50.000000 nf-core-2.9/tests/subworkflows/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-30 16:11:50.000000 nf-core-2.9/tests/subworkflows/create_test_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-30 16:11:50.000000 nf-core-2.9/tests/subworkflows/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-06-30 16:11:50.000000 nf-core-2.9/tests/subworkflows/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-30 16:11:50.000000 nf-core-2.9/tests/subworkflows/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-30 16:11:50.000000 nf-core-2.9/tests/subworkflows/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-30 16:11:50.000000 nf-core-2.9/tests/subworkflows/subworkflows_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-06-30 16:11:50.000000 nf-core-2.9/tests/subworkflows/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25709 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_lint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_refgenie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_subworkflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17732 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-30 16:11:50.000000 nf-core-2.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-30 16:11:50.000000 nf-core-2.9/tests/utils.py
```

### Comparing `nf-core-2.8/LICENSE` & `nf-core-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/PKG-INFO` & `nf-core-2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nf-core
-Version: 2.8
+Version: 2.9
 Summary: Helper tools for use with nf-core Nextflow pipelines.
 Home-page: https://github.com/nf-core/tools
 Author: Phil Ewels
 Author-email: phil.ewels@scilifelab.se
 License: MIT
 Keywords: nf-core,nextflow,bioinformatics,workflow,pipeline,biology,sequencing,NGS,next generation sequencing
 Requires-Python: >=3.8, <4
@@ -29,15 +29,15 @@
 
 ## Table of contents <!-- omit in toc -->
 
 - [`nf-core` tools installation](#installation)
 - [`nf-core` tools update](#update-tools)
 - [`nf-core list` - List available pipelines](#listing-pipelines)
 - [`nf-core launch` - Run a pipeline with interactive parameter prompts](#launch-a-pipeline)
-- [`nf-core download` - Download pipeline for offline use](#downloading-pipelines-for-offline-use)
+- [`nf-core download` - Download a pipeline for offline use](#downloading-pipelines-for-offline-use)
 - [`nf-core licences` - List software licences in a pipeline](#pipeline-software-licences)
 - [`nf-core create` - Create a new pipeline with the nf-core template](#creating-a-new-pipeline)
 - [`nf-core lint` - Check pipeline code against nf-core guidelines](#linting-a-workflow)
 - [`nf-core schema` - Work with pipeline schema files](#pipeline-schema)
 - [`nf-core bump-version` - Update nf-core pipeline version number](#bumping-a-pipeline-version-number)
 - [`nf-core sync` - Synchronise pipeline TEMPLATE branches](#sync-a-pipeline-with-the-template)
 - [`nf-core modules` - commands for dealing with DSL2 modules](#modules)
@@ -336,15 +336,15 @@
 If run without any arguments, the download tool will interactively prompt you for the required information.
 Each option has a flag, if all are supplied then it will run without any user input needed.
 
 <!-- RICH-CODEX
 working_dir: tmp
 -->
 
-![`nf-core download rnaseq -r 3.8 --outdir nf-core-rnaseq -x none -c none`](docs/images/nf-core-download.svg)
+![`nf-core download rnaseq -r 3.8 --outdir nf-core-rnaseq -x none -s none -d`](docs/images/nf-core-download.svg)
 
 Once downloaded, you will see something like the following file structure for the downloaded pipeline:
 
 <!-- RICH-CODEX
 working_dir: tmp
 -->
 
@@ -352,26 +352,28 @@
 
 You can run the pipeline by simply providing the directory path for the `workflow` folder to your `nextflow run` command:
 
 ```bash
 nextflow run /path/to/download/nf-core-rnaseq-dev/workflow/ --input mydata.csv --outdir results  # usual parameters here
 ```
 
-> Note that if you downloaded singularity images, you will need to use `-profile singularity` or have it enabled in your config file.
+> Note that if you downloaded Singularity container images, you will need to use `-profile singularity` or have it enabled in your config file.
 
 ### Downloaded nf-core configs
 
 The pipeline files are automatically updated (`params.custom_config_base` is set to `../configs`), so that the local copy of institutional configs are available when running the pipeline.
 So using `-profile <NAME>` should work if available within [nf-core/configs](https://github.com/nf-core/configs).
 
-### Downloading singularity containers
+> ⚠️ This option is not available when downloading a pipeline for use with [Nextflow Tower](#adapting-downloads-to-nextflow-tower) because the application manages all configurations separately.
 
-If you're using Singularity, the `nf-core download` command can also fetch the required Singularity container images for you.
-To do this, select `singularity` in the prompt or specify `--container singularity` in the command.
-Your archive / target output directory will then include three folders: `workflow`, `configs` and also `singularity-containers`.
+### Downloading Apptainer containers
+
+If you're using [Singularity](https://apptainer.org) (Apptainer), the `nf-core download` command can also fetch the required container images for you.
+To do this, select `singularity` in the prompt or specify `--container-system singularity` in the command.
+Your archive / target output directory will then also include a separate folder `singularity-containers`.
 
 The downloaded workflow files are again edited to add the following line to the end of the pipeline's `nextflow.config` file:
 
 ```nextflow
 singularity.cacheDir = "${projectDir}/../singularity-images/"
 ```
 
@@ -381,43 +383,50 @@
 #### Singularity cache directory
 
 We highly recommend setting the `$NXF_SINGULARITY_CACHEDIR` environment variable on your system, even if that is a different system to where you will be running Nextflow.
 
 If found, the tool will fetch the Singularity images to this directory first before copying to the target output archive / directory.
 Any images previously fetched will be found there and copied directly - this includes images that may be shared with other pipelines or previous pipeline version downloads or download attempts.
 
-If you are running the download on the same system where you will be running the pipeline (eg. a shared filesystem where Nextflow won't have an internet connection at a later date), you can choose to _only_ use the cache via a prompt or cli options `--singularity-cache-only` / `--singularity-cache-copy`.
+If you are running the download on the same system where you will be running the pipeline (eg. a shared filesystem where Nextflow won't have an internet connection at a later date), you can choose to _only_ use the cache via a prompt or cli options `--container-cache-utilisation amend`. This instructs `nf-core download` to fetch all Singularity images to the `$NXF_SINGULARITY_CACHEDIR` directory but does _not_ copy them to the workflow archive / directory. The workflow config file is _not_ edited. This means that when you later run the workflow, Nextflow will just use the cache folder directly.
 
-This instructs `nf-core download` to fetch all Singularity images to the `$NXF_SINGULARITY_CACHEDIR` directory but does _not_ copy them to the workflow archive / directory.
-The workflow config file is _not_ edited. This means that when you later run the workflow, Nextflow will just use the cache folder directly.
+If you are downloading a workflow for a different system, you can provide information about the contents of its image cache to `nf-core download`. To avoid unnecessary container image downloads, choose `--container-cache-utilisation remote` and provide a list of already available images as plain text file to `--container-cache-index my_list_of_remotely_available_images.txt`. To generate this list on the remote system, run `find $NXF_SINGULARITY_CACHEDIR -name "*.img" > my_list_of_remotely_available_images.txt`. The tool will then only download and copy images into your output directory, which are missing on the remote system.
 
 #### How the Singularity image downloads work
 
 The Singularity image download finds containers using two methods:
 
 1. It runs `nextflow config` on the downloaded workflow to look for a `process.container` statement for the whole pipeline.
    This is the typical method used for DSL1 pipelines.
 2. It scrapes any files it finds with a `.nf` file extension in the workflow `modules` directory for lines
    that look like `container = "xxx"`. This is the typical method for DSL2 pipelines, which have one container per process.
 
-Some DSL2 modules have container addresses for docker (eg. `biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity continaer (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
+Some DSL2 modules have container addresses for docker (eg. `biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity container (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
 Where both are found, the download URL is preferred.
 
 Once a full list of containers is found, they are processed in the following order:
 
-1. If the target image already exists, nothing is done (eg. with `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` specified)
-2. If found in `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` is _not_ specified, they are copied to the output directory
+1. If the target image already exists, nothing is done (eg. with `$NXF_SINGULARITY_CACHEDIR` and `--container-cache-utilisation amend` specified)
+2. If found in `$NXF_SINGULARITY_CACHEDIR` and `--container-cache-utilisation copy` is specified, they are copied to the output directory
 3. If they start with `http` they are downloaded directly within Python (default 4 at a time, you can customise this with `--parallel-downloads`)
-4. If they look like a Docker image name, they are fetched using a `singularity pull` command
-   - This requires Singularity to be installed on the system and is substantially slower
+4. If they look like a Docker image name, they are fetched using a `singularity pull` command. Choose the container libraries (registries) queried by providing one or multiple `--container-library` parameter(s). For example, if you call `nf-core download` with `-l quay.io -l ghcr.io -l docker.io`, every image will be pulled from `quay.io` unless an error is encountered. Subsequently, `ghcr.io` and then `docker.io` will be queried for any image that has failed before.
+   - This requires Singularity/Apptainer to be installed on the system and is substantially slower
 
-Note that compressing many GBs of binary files can be slow, so specifying `--compress none` is recommended when downloading Singularity images.
+Note that compressing many GBs of binary files can be slow, so specifying `--compress none` is recommended when downloading Singularity images that are copied to the output directory.
 
 If the download speeds are much slower than your internet connection is capable of, you can set `--parallel-downloads` to a large number to download loads of images at once.
 
+### Adapting downloads to Nextflow Tower
+
+[seqeralabs® Nextflow Tower](https://cloud.tower.nf/) provides a graphical user interface to oversee pipeline runs, gather statistics and configure compute resources. While pipelines added to _Tower_ are preferably hosted at a Git service, providing them as disconnected, self-reliant repositories is also possible for premises with restricted network access. Choosing the `--tower` flag will download the pipeline in an appropriate form.
+
+Subsequently, the `*.git` folder can be moved to it's final destination and linked with a pipeline in _Tower_ using the `file:/` prefix.
+
+> 💡 Also without access to Tower, pipelines downloaded with the `--tower` flag can be run: `nextflow run -r 2.5 file:/path/to/pipelinedownload.git`. Downloads in this format allow you to include multiple revisions of a pipeline in a single file, but require that the revision (e.g. `-r 2.5`) is always explicitly specified.
+
 ## Pipeline software licences
 
 Sometimes it's useful to see the software licences of the tools used in a pipeline.
 You can use the `licences` subcommand to fetch and print the software licence from each conda / PyPI package used in an nf-core pipeline.
 
 > ⚠️ This command does not currently work for newer DSL2 pipelines. This will hopefully be addressed [soon](https://github.com/nf-core/tools/issues/1155).
 
@@ -571,15 +580,15 @@
 <!-- RICH-CODEX
 working_dir: tmp
 before_command: 'echo "{input: myfiles.csv, outdir: results}" > nf-params.json'
 timeout: 10
 after_command: rm nf-params.json
 -->
 
-![`nf-core schema validate nf-core-rnaseq/workflow nf-params.json`](docs/images/nf-core-schema-validate.svg)
+![`nf-core schema validate nf-core-rnaseq/3_8 nf-params.json`](docs/images/nf-core-schema-validate.svg)
 
 The `pipeline` option can be a directory containing a pipeline, a path to a schema file or the name of an nf-core pipeline (which will be downloaded using `nextflow pull`).
 
 ### Build a pipeline schema
 
 Manually building JSONSchema documents is not trivial and can be very error prone.
 Instead, the `nf-core schema build` command collects your pipeline parameters and gives interactive prompts about any missing or unexpected params.
@@ -908,14 +917,15 @@
 The command will automatically look through parent directories for this file to set the root path, so that you can run the command in a subdirectory.
 It will start in the current working directory, or whatever is specified with `--dir <directory>`.
 
 The `nf-core modules create` command will prompt you with the relevant questions in order to create all of the necessary module files.
 
 <!-- RICH-CODEX
 working_dir: tmp
+timeout: 10
 before_command: git clone https://github.com/nf-core/modules.git && cd modules
 fake_command: nf-core modules create fastqc --author @nf-core-bot  --label process_low --meta --force
 -->
 
 ![`cd modules && nf-core modules create fastqc --author @nf-core-bot  --label process_low --meta --force`](docs/images/nf-core-modules-create.svg)
 
 ### Create a module test config file
@@ -945,14 +955,16 @@
 
 ![`nf-core modules lint multiqc`](docs/images/nf-core-modules-lint.svg)
 
 ### Run the tests for a module using pytest
 
 To run unit tests of a module that you have installed or the test created by the command [`nf-core modules create-test-yml`](#create-a-module-test-config-file), you can use `nf-core modules test` command. This command runs the tests specified in `modules/tests/software/<tool>/<subtool>/test.yml` file using [pytest](https://pytest-workflow.readthedocs.io/en/stable/).
 
+> This command uses the pytest argument `--git-aware` to avoid copying the whole `.git` directory and files ignored by `git`. This means that it will only include files listed by `git ls-files`. Remember to **commit your changes** after adding a new module to add the new files to your git index.
+
 You can specify the module name in the form TOOL/SUBTOOL in command line or provide it later by prompts.
 
 <!-- RICH-CODEX
 working_dir: tmp/modules
 timeout: 30
 extra_env:
   PROFILE: 'conda'
@@ -1178,20 +1190,19 @@
 set to either `pipeline` or `modules`.
 The command will automatically look through parent directories for this file to set the root path, so that you can run the command in a subdirectory.
 It will start in the current working directory, or whatever is specified with `--dir <directory>`.
 
 The `nf-core subworkflows create` command will prompt you with the relevant questions in order to create all of the necessary subworkflow files.
 
 <!-- RICH-CODEX
-working_dir: tmp
-before_command: git clone https://github.com/nf-core/modules.git && cd modules
+working_dir: tmp/modules
 fake_command: nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force
 -->
 
-![`cd modules && nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force`](docs/images/nf-core-subworkflows-create.svg)
+![`nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force`](docs/images/nf-core-subworkflows-create.svg)
 
 ### Create a subworkflow test config file
 
 All subworkflows on [nf-core/modules](https://github.com/nf-core/modules) have a strict requirement of being unit tested using minimal test data.
 To help developers build new subworkflows, the `nf-core subworkflows create-test-yml` command automates the creation of the yaml file required to document the output file `md5sum` and other information generated by the testing.
 After you have written a minimal Nextflow script to test your subworkflow in `/tests/subworkflow/<subworkflow_name>/main.nf`, this command will run the tests for you and create the `/tests/subworkflow/<tool>/<subtool>/test.yml` file.
 
@@ -1203,14 +1214,16 @@
 
 ![`nf-core subworkflows create-test-yml bam_stats_samtools --no-prompts --force`](docs/images/nf-core-subworkflows-create-test.svg)
 
 ### Run the tests for a subworkflow using pytest
 
 To run unit tests of a subworkflow that you have installed or the test created by the command [`nf-core subworkflow create-test-yml`](#create-a-subworkflow-test-config-file), you can use `nf-core subworkflows test` command. This command runs the tests specified in `tests/subworkflows/<subworkflow_name>/test.yml` file using [pytest](https://pytest-workflow.readthedocs.io/en/stable/).
 
+> This command uses the pytest argument `--git-aware` to avoid copying the whole `.git` directory and files ignored by `git`. This means that it will only include files listed by `git ls-files`. Remember to **commit your changes** after adding a new subworkflow to add the new files to your git index.
+
 You can specify the subworkflow name in the form TOOL/SUBTOOL in command line or provide it later by prompts.
 
 <!-- RICH-CODEX
 working_dir: tmp/modules
 timeout: 30
 extra_env:
   PROFILE: 'conda'
```

### Comparing `nf-core-2.8/README.md` & `nf-core-2.9/nf_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: nf-core
+Version: 2.9
+Summary: Helper tools for use with nf-core Nextflow pipelines.
+Home-page: https://github.com/nf-core/tools
+Author: Phil Ewels
+Author-email: phil.ewels@scilifelab.se
+License: MIT
+Keywords: nf-core,nextflow,bioinformatics,workflow,pipeline,biology,sequencing,NGS,next generation sequencing
+Requires-Python: >=3.8, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ![nf-core/tools](docs/images/nfcore-tools_logo_light.png#gh-light-mode-only) ![nf-core/tools](docs/images/nfcore-tools_logo_dark.png#gh-dark-mode-only) <!-- omit in toc -->
 
 [![Python tests](https://github.com/nf-core/tools/workflows/Python%20tests/badge.svg?branch=master&event=push)](https://github.com/nf-core/tools/actions?query=workflow%3A%22Python+tests%22+branch%3Amaster)
 [![codecov](https://codecov.io/gh/nf-core/tools/branch/master/graph/badge.svg)](https://codecov.io/gh/nf-core/tools)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![code style: prettier](https://img.shields.io/badge/code%20style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -16,15 +29,15 @@
 
 ## Table of contents <!-- omit in toc -->
 
 - [`nf-core` tools installation](#installation)
 - [`nf-core` tools update](#update-tools)
 - [`nf-core list` - List available pipelines](#listing-pipelines)
 - [`nf-core launch` - Run a pipeline with interactive parameter prompts](#launch-a-pipeline)
-- [`nf-core download` - Download pipeline for offline use](#downloading-pipelines-for-offline-use)
+- [`nf-core download` - Download a pipeline for offline use](#downloading-pipelines-for-offline-use)
 - [`nf-core licences` - List software licences in a pipeline](#pipeline-software-licences)
 - [`nf-core create` - Create a new pipeline with the nf-core template](#creating-a-new-pipeline)
 - [`nf-core lint` - Check pipeline code against nf-core guidelines](#linting-a-workflow)
 - [`nf-core schema` - Work with pipeline schema files](#pipeline-schema)
 - [`nf-core bump-version` - Update nf-core pipeline version number](#bumping-a-pipeline-version-number)
 - [`nf-core sync` - Synchronise pipeline TEMPLATE branches](#sync-a-pipeline-with-the-template)
 - [`nf-core modules` - commands for dealing with DSL2 modules](#modules)
@@ -323,15 +336,15 @@
 If run without any arguments, the download tool will interactively prompt you for the required information.
 Each option has a flag, if all are supplied then it will run without any user input needed.
 
 <!-- RICH-CODEX
 working_dir: tmp
 -->
 
-![`nf-core download rnaseq -r 3.8 --outdir nf-core-rnaseq -x none -c none`](docs/images/nf-core-download.svg)
+![`nf-core download rnaseq -r 3.8 --outdir nf-core-rnaseq -x none -s none -d`](docs/images/nf-core-download.svg)
 
 Once downloaded, you will see something like the following file structure for the downloaded pipeline:
 
 <!-- RICH-CODEX
 working_dir: tmp
 -->
 
@@ -339,26 +352,28 @@
 
 You can run the pipeline by simply providing the directory path for the `workflow` folder to your `nextflow run` command:
 
 ```bash
 nextflow run /path/to/download/nf-core-rnaseq-dev/workflow/ --input mydata.csv --outdir results  # usual parameters here
 ```
 
-> Note that if you downloaded singularity images, you will need to use `-profile singularity` or have it enabled in your config file.
+> Note that if you downloaded Singularity container images, you will need to use `-profile singularity` or have it enabled in your config file.
 
 ### Downloaded nf-core configs
 
 The pipeline files are automatically updated (`params.custom_config_base` is set to `../configs`), so that the local copy of institutional configs are available when running the pipeline.
 So using `-profile <NAME>` should work if available within [nf-core/configs](https://github.com/nf-core/configs).
 
-### Downloading singularity containers
+> ⚠️ This option is not available when downloading a pipeline for use with [Nextflow Tower](#adapting-downloads-to-nextflow-tower) because the application manages all configurations separately.
+
+### Downloading Apptainer containers
 
-If you're using Singularity, the `nf-core download` command can also fetch the required Singularity container images for you.
-To do this, select `singularity` in the prompt or specify `--container singularity` in the command.
-Your archive / target output directory will then include three folders: `workflow`, `configs` and also `singularity-containers`.
+If you're using [Singularity](https://apptainer.org) (Apptainer), the `nf-core download` command can also fetch the required container images for you.
+To do this, select `singularity` in the prompt or specify `--container-system singularity` in the command.
+Your archive / target output directory will then also include a separate folder `singularity-containers`.
 
 The downloaded workflow files are again edited to add the following line to the end of the pipeline's `nextflow.config` file:
 
 ```nextflow
 singularity.cacheDir = "${projectDir}/../singularity-images/"
 ```
 
@@ -368,43 +383,50 @@
 #### Singularity cache directory
 
 We highly recommend setting the `$NXF_SINGULARITY_CACHEDIR` environment variable on your system, even if that is a different system to where you will be running Nextflow.
 
 If found, the tool will fetch the Singularity images to this directory first before copying to the target output archive / directory.
 Any images previously fetched will be found there and copied directly - this includes images that may be shared with other pipelines or previous pipeline version downloads or download attempts.
 
-If you are running the download on the same system where you will be running the pipeline (eg. a shared filesystem where Nextflow won't have an internet connection at a later date), you can choose to _only_ use the cache via a prompt or cli options `--singularity-cache-only` / `--singularity-cache-copy`.
+If you are running the download on the same system where you will be running the pipeline (eg. a shared filesystem where Nextflow won't have an internet connection at a later date), you can choose to _only_ use the cache via a prompt or cli options `--container-cache-utilisation amend`. This instructs `nf-core download` to fetch all Singularity images to the `$NXF_SINGULARITY_CACHEDIR` directory but does _not_ copy them to the workflow archive / directory. The workflow config file is _not_ edited. This means that when you later run the workflow, Nextflow will just use the cache folder directly.
 
-This instructs `nf-core download` to fetch all Singularity images to the `$NXF_SINGULARITY_CACHEDIR` directory but does _not_ copy them to the workflow archive / directory.
-The workflow config file is _not_ edited. This means that when you later run the workflow, Nextflow will just use the cache folder directly.
+If you are downloading a workflow for a different system, you can provide information about the contents of its image cache to `nf-core download`. To avoid unnecessary container image downloads, choose `--container-cache-utilisation remote` and provide a list of already available images as plain text file to `--container-cache-index my_list_of_remotely_available_images.txt`. To generate this list on the remote system, run `find $NXF_SINGULARITY_CACHEDIR -name "*.img" > my_list_of_remotely_available_images.txt`. The tool will then only download and copy images into your output directory, which are missing on the remote system.
 
 #### How the Singularity image downloads work
 
 The Singularity image download finds containers using two methods:
 
 1. It runs `nextflow config` on the downloaded workflow to look for a `process.container` statement for the whole pipeline.
    This is the typical method used for DSL1 pipelines.
 2. It scrapes any files it finds with a `.nf` file extension in the workflow `modules` directory for lines
    that look like `container = "xxx"`. This is the typical method for DSL2 pipelines, which have one container per process.
 
-Some DSL2 modules have container addresses for docker (eg. `biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity continaer (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
+Some DSL2 modules have container addresses for docker (eg. `biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity container (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
 Where both are found, the download URL is preferred.
 
 Once a full list of containers is found, they are processed in the following order:
 
-1. If the target image already exists, nothing is done (eg. with `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` specified)
-2. If found in `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` is _not_ specified, they are copied to the output directory
+1. If the target image already exists, nothing is done (eg. with `$NXF_SINGULARITY_CACHEDIR` and `--container-cache-utilisation amend` specified)
+2. If found in `$NXF_SINGULARITY_CACHEDIR` and `--container-cache-utilisation copy` is specified, they are copied to the output directory
 3. If they start with `http` they are downloaded directly within Python (default 4 at a time, you can customise this with `--parallel-downloads`)
-4. If they look like a Docker image name, they are fetched using a `singularity pull` command
-   - This requires Singularity to be installed on the system and is substantially slower
+4. If they look like a Docker image name, they are fetched using a `singularity pull` command. Choose the container libraries (registries) queried by providing one or multiple `--container-library` parameter(s). For example, if you call `nf-core download` with `-l quay.io -l ghcr.io -l docker.io`, every image will be pulled from `quay.io` unless an error is encountered. Subsequently, `ghcr.io` and then `docker.io` will be queried for any image that has failed before.
+   - This requires Singularity/Apptainer to be installed on the system and is substantially slower
 
-Note that compressing many GBs of binary files can be slow, so specifying `--compress none` is recommended when downloading Singularity images.
+Note that compressing many GBs of binary files can be slow, so specifying `--compress none` is recommended when downloading Singularity images that are copied to the output directory.
 
 If the download speeds are much slower than your internet connection is capable of, you can set `--parallel-downloads` to a large number to download loads of images at once.
 
+### Adapting downloads to Nextflow Tower
+
+[seqeralabs® Nextflow Tower](https://cloud.tower.nf/) provides a graphical user interface to oversee pipeline runs, gather statistics and configure compute resources. While pipelines added to _Tower_ are preferably hosted at a Git service, providing them as disconnected, self-reliant repositories is also possible for premises with restricted network access. Choosing the `--tower` flag will download the pipeline in an appropriate form.
+
+Subsequently, the `*.git` folder can be moved to it's final destination and linked with a pipeline in _Tower_ using the `file:/` prefix.
+
+> 💡 Also without access to Tower, pipelines downloaded with the `--tower` flag can be run: `nextflow run -r 2.5 file:/path/to/pipelinedownload.git`. Downloads in this format allow you to include multiple revisions of a pipeline in a single file, but require that the revision (e.g. `-r 2.5`) is always explicitly specified.
+
 ## Pipeline software licences
 
 Sometimes it's useful to see the software licences of the tools used in a pipeline.
 You can use the `licences` subcommand to fetch and print the software licence from each conda / PyPI package used in an nf-core pipeline.
 
 > ⚠️ This command does not currently work for newer DSL2 pipelines. This will hopefully be addressed [soon](https://github.com/nf-core/tools/issues/1155).
 
@@ -558,15 +580,15 @@
 <!-- RICH-CODEX
 working_dir: tmp
 before_command: 'echo "{input: myfiles.csv, outdir: results}" > nf-params.json'
 timeout: 10
 after_command: rm nf-params.json
 -->
 
-![`nf-core schema validate nf-core-rnaseq/workflow nf-params.json`](docs/images/nf-core-schema-validate.svg)
+![`nf-core schema validate nf-core-rnaseq/3_8 nf-params.json`](docs/images/nf-core-schema-validate.svg)
 
 The `pipeline` option can be a directory containing a pipeline, a path to a schema file or the name of an nf-core pipeline (which will be downloaded using `nextflow pull`).
 
 ### Build a pipeline schema
 
 Manually building JSONSchema documents is not trivial and can be very error prone.
 Instead, the `nf-core schema build` command collects your pipeline parameters and gives interactive prompts about any missing or unexpected params.
@@ -895,14 +917,15 @@
 The command will automatically look through parent directories for this file to set the root path, so that you can run the command in a subdirectory.
 It will start in the current working directory, or whatever is specified with `--dir <directory>`.
 
 The `nf-core modules create` command will prompt you with the relevant questions in order to create all of the necessary module files.
 
 <!-- RICH-CODEX
 working_dir: tmp
+timeout: 10
 before_command: git clone https://github.com/nf-core/modules.git && cd modules
 fake_command: nf-core modules create fastqc --author @nf-core-bot  --label process_low --meta --force
 -->
 
 ![`cd modules && nf-core modules create fastqc --author @nf-core-bot  --label process_low --meta --force`](docs/images/nf-core-modules-create.svg)
 
 ### Create a module test config file
@@ -932,14 +955,16 @@
 
 ![`nf-core modules lint multiqc`](docs/images/nf-core-modules-lint.svg)
 
 ### Run the tests for a module using pytest
 
 To run unit tests of a module that you have installed or the test created by the command [`nf-core modules create-test-yml`](#create-a-module-test-config-file), you can use `nf-core modules test` command. This command runs the tests specified in `modules/tests/software/<tool>/<subtool>/test.yml` file using [pytest](https://pytest-workflow.readthedocs.io/en/stable/).
 
+> This command uses the pytest argument `--git-aware` to avoid copying the whole `.git` directory and files ignored by `git`. This means that it will only include files listed by `git ls-files`. Remember to **commit your changes** after adding a new module to add the new files to your git index.
+
 You can specify the module name in the form TOOL/SUBTOOL in command line or provide it later by prompts.
 
 <!-- RICH-CODEX
 working_dir: tmp/modules
 timeout: 30
 extra_env:
   PROFILE: 'conda'
@@ -1165,20 +1190,19 @@
 set to either `pipeline` or `modules`.
 The command will automatically look through parent directories for this file to set the root path, so that you can run the command in a subdirectory.
 It will start in the current working directory, or whatever is specified with `--dir <directory>`.
 
 The `nf-core subworkflows create` command will prompt you with the relevant questions in order to create all of the necessary subworkflow files.
 
 <!-- RICH-CODEX
-working_dir: tmp
-before_command: git clone https://github.com/nf-core/modules.git && cd modules
+working_dir: tmp/modules
 fake_command: nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force
 -->
 
-![`cd modules && nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force`](docs/images/nf-core-subworkflows-create.svg)
+![`nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force`](docs/images/nf-core-subworkflows-create.svg)
 
 ### Create a subworkflow test config file
 
 All subworkflows on [nf-core/modules](https://github.com/nf-core/modules) have a strict requirement of being unit tested using minimal test data.
 To help developers build new subworkflows, the `nf-core subworkflows create-test-yml` command automates the creation of the yaml file required to document the output file `md5sum` and other information generated by the testing.
 After you have written a minimal Nextflow script to test your subworkflow in `/tests/subworkflow/<subworkflow_name>/main.nf`, this command will run the tests for you and create the `/tests/subworkflow/<tool>/<subtool>/test.yml` file.
 
@@ -1190,14 +1214,16 @@
 
 ![`nf-core subworkflows create-test-yml bam_stats_samtools --no-prompts --force`](docs/images/nf-core-subworkflows-create-test.svg)
 
 ### Run the tests for a subworkflow using pytest
 
 To run unit tests of a subworkflow that you have installed or the test created by the command [`nf-core subworkflow create-test-yml`](#create-a-subworkflow-test-config-file), you can use `nf-core subworkflows test` command. This command runs the tests specified in `tests/subworkflows/<subworkflow_name>/test.yml` file using [pytest](https://pytest-workflow.readthedocs.io/en/stable/).
 
+> This command uses the pytest argument `--git-aware` to avoid copying the whole `.git` directory and files ignored by `git`. This means that it will only include files listed by `git ls-files`. Remember to **commit your changes** after adding a new subworkflow to add the new files to your git index.
+
 You can specify the subworkflow name in the form TOOL/SUBTOOL in command line or provide it later by prompts.
 
 <!-- RICH-CODEX
 working_dir: tmp/modules
 timeout: 30
 extra_env:
   PROFILE: 'conda'
```

### Comparing `nf-core-2.8/nf_core/__main__.py` & `nf-core-2.9/nf_core/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,34 +6,25 @@
 
 import rich
 import rich.console
 import rich.logging
 import rich.traceback
 import rich_click as click
 
-import nf_core
-import nf_core.bump_version
-import nf_core.create
-import nf_core.download
-import nf_core.launch
-import nf_core.licences
-import nf_core.lint
-import nf_core.list
-import nf_core.modules
-import nf_core.schema
-import nf_core.subworkflows
-import nf_core.sync
-import nf_core.utils
+from nf_core import __version__
+from nf_core.download import DownloadError
+from nf_core.modules.modules_repo import NF_CORE_MODULES_REMOTE
+from nf_core.utils import check_if_outdated, rich_force_colors, setup_nfcore_dir
 
 # Set up logging as the root logger
 # Submodules should all traverse back to this
 log = logging.getLogger()
 
 # Set up .nfcore directory for storing files between sessions
-nf_core.utils.setup_nfcore_dir()
+setup_nfcore_dir()
 
 # Set up nicer formatting of click cli help messages
 click.rich_click.MAX_WIDTH = 100
 click.rich_click.USE_RICH_MARKUP = True
 click.rich_click.COMMAND_GROUPS = {
     "nf-core": [
         {
@@ -67,50 +58,64 @@
     ],
 }
 click.rich_click.OPTION_GROUPS = {
     "nf-core modules list local": [{"options": ["--dir", "--json", "--help"]}],
 }
 
 # Set up rich stderr console
-stderr = rich.console.Console(stderr=True, force_terminal=nf_core.utils.rich_force_colors())
-stdout = rich.console.Console(force_terminal=nf_core.utils.rich_force_colors())
+stderr = rich.console.Console(stderr=True, force_terminal=rich_force_colors())
+stdout = rich.console.Console(force_terminal=rich_force_colors())
 
 # Set up the rich traceback
 rich.traceback.install(console=stderr, width=200, word_wrap=True, extra_lines=1)
 
 
+# Define exceptions for which no traceback should be printed,
+# because they are actually preliminary, but intended program terminations.
+# (Custom exceptions are cleaner than `sys.exit(1)`, which we used before)
+def selective_traceback_hook(exctype, value, traceback):
+    if exctype in {DownloadError}:  # extend set as needed
+        log.error(value)
+    else:
+        # print the colored traceback for all other exceptions with rich as usual
+        stderr.print(rich.traceback.Traceback.from_exception(exctype, value, traceback))
+
+
+sys.excepthook = selective_traceback_hook
+
+
 def run_nf_core():
     # print nf-core header if environment variable is not set
     if os.environ.get("_NF_CORE_COMPLETE") is None:
         # Print nf-core header
         stderr.print(f"\n[green]{' ' * 42},--.[grey39]/[green],-.", highlight=False)
         stderr.print("[blue]          ___     __   __   __   ___     [green]/,-._.--~\\", highlight=False)
         stderr.print(r"[blue]    |\ | |__  __ /  ` /  \ |__) |__      [yellow]   }  {", highlight=False)
         stderr.print(r"[blue]    | \| |       \__, \__/ |  \ |___     [green]\`-._,-`-,", highlight=False)
         stderr.print("[green]                                          `._,._,'\n", highlight=False)
         stderr.print(
-            f"[grey39]    nf-core/tools version {nf_core.__version__} - [link=https://nf-co.re]https://nf-co.re[/]",
+            f"[grey39]    nf-core/tools version {__version__} - [link=https://nf-co.re]https://nf-co.re[/]",
             highlight=False,
         )
         try:
-            is_outdated, _, remote_vers = nf_core.utils.check_if_outdated()
+            is_outdated, _, remote_vers = check_if_outdated()
             if is_outdated:
                 stderr.print(
                     f"[bold bright_yellow]    There is a new version of nf-core/tools available! ({remote_vers})",
                     highlight=False,
                 )
         except Exception as e:
             log.debug(f"Could not check latest version: {e}")
         stderr.print("\n")
     # Launch the click cli
     nf_core_cli(auto_envvar_prefix="NFCORE")
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
-@click.version_option(nf_core.__version__)
+@click.version_option(__version__)
 @click.option("-v", "--verbose", is_flag=True, default=False, help="Print verbose output to the console.")
 @click.option("--hide-progress", is_flag=True, default=False, help="Don't show progress bars.")
 @click.option("-l", "--log-file", help="Save a verbose log to a file.", metavar="<filename>")
 @click.pass_context
 def nf_core_cli(ctx, verbose, hide_progress, log_file):
     """
     nf-core/tools provides a set of helper tools for use with nf-core Nextflow pipelines.
@@ -120,15 +125,15 @@
     # Set the base logger to output DEBUG
     log.setLevel(logging.DEBUG)
 
     # Set up logs to the console
     log.addHandler(
         rich.logging.RichHandler(
             level=logging.DEBUG if verbose else logging.INFO,
-            console=rich.console.Console(stderr=True, force_terminal=nf_core.utils.rich_force_colors()),
+            console=rich.console.Console(stderr=True, force_terminal=rich_force_colors()),
             show_time=False,
             show_path=verbose,  # True if verbose, false otherwise
             markup=True,
         )
     )
 
     # Set up logs to a file if we asked for one
@@ -159,15 +164,17 @@
 def list(keywords, sort, json, show_archived):
     """
     List available nf-core pipelines with local info.
 
     Checks the web for a list of nf-core pipelines with their latest releases.
     Shows which nf-core pipelines you have pulled locally and whether they are up to date.
     """
-    stdout.print(nf_core.list.list_workflows(keywords, sort, json, show_archived))
+    from nf_core.list import list_workflows
+
+    stdout.print(list_workflows(keywords, sort, json, show_archived))
 
 
 # nf-core launch
 @nf_core_cli.command()
 @click.argument("pipeline", required=False, metavar="<pipeline name>")
 @click.option("-r", "--revision", help="Release/branch/SHA of the project to run (if remote)")
 @click.option("-i", "--id", help="ID for web-gui launch parameter set")
@@ -203,47 +210,105 @@
 
     When finished, saves a file with the selected parameters which can be
     passed to Nextflow using the -params-file option.
 
     Run using a remote pipeline name (such as GitHub `user/repo` or a URL),
     a local pipeline directory or an ID from the nf-core web launch tool.
     """
-    launcher = nf_core.launch.Launch(
-        pipeline, revision, command_only, params_in, params_out, save_all, show_hidden, url, id
-    )
+    from nf_core.launch import Launch
+
+    launcher = Launch(pipeline, revision, command_only, params_in, params_out, save_all, show_hidden, url, id)
     if not launcher.launch_pipeline():
         sys.exit(1)
 
 
 # nf-core download
 @nf_core_cli.command()
 @click.argument("pipeline", required=False, metavar="<pipeline name>")
-@click.option("-r", "--revision", type=str, help="Pipeline release")
+@click.option(
+    "-r",
+    "--revision",
+    multiple=True,
+    help="Pipeline release to download. Multiple invocations are possible, e.g. `-r 1.1 -r 1.2`",
+)
 @click.option("-o", "--outdir", type=str, help="Output directory")
 @click.option(
     "-x", "--compress", type=click.Choice(["tar.gz", "tar.bz2", "zip", "none"]), help="Archive compression type"
 )
 @click.option("-f", "--force", is_flag=True, default=False, help="Overwrite existing files")
+@click.option("-t", "--tower", is_flag=True, default=False, help="Download for seqeralabs® Nextflow Tower")
+@click.option(
+    "-d",
+    "--download-configuration",
+    is_flag=True,
+    default=False,
+    help="Include configuration profiles in download. Not available with `--tower`",
+)
+# -c changed to -s for consistency with other --container arguments, where it is always the first letter of the last word.
+# Also -c might be used instead of -d for config in a later release, but reusing params for different options in two subsequent releases might be too error-prone.
 @click.option(
-    "-c", "--container", type=click.Choice(["none", "singularity"]), help="Download software container images"
+    "-s",
+    "--container-system",
+    type=click.Choice(["none", "singularity"]),
+    help="Download container images of required software.",
 )
 @click.option(
-    "--singularity-cache-only/--singularity-cache-copy",
-    help="Don't / do copy images to the output directory and set 'singularity.cacheDir' in workflow",
+    "-l",
+    "--container-library",
+    multiple=True,
+    help="Container registry/library or mirror to pull images from.",
+)
+@click.option(
+    "-u",
+    "--container-cache-utilisation",
+    type=click.Choice(["amend", "copy", "remote"]),
+    help="Utilise a `singularity.cacheDir` in the download process, if applicable.",
+)
+@click.option(
+    "-i",
+    "--container-cache-index",
+    type=str,
+    help="List of images already available in a remote `singularity.cacheDir`.",
 )
 @click.option("-p", "--parallel-downloads", type=int, default=4, help="Number of parallel image downloads")
-def download(pipeline, revision, outdir, compress, force, container, singularity_cache_only, parallel_downloads):
+def download(
+    pipeline,
+    revision,
+    outdir,
+    compress,
+    force,
+    tower,
+    download_configuration,
+    container_system,
+    container_library,
+    container_cache_utilisation,
+    container_cache_index,
+    parallel_downloads,
+):
     """
     Download a pipeline, nf-core/configs and pipeline singularity images.
 
     Collects all files in a single archive and configures the downloaded
     workflow to use relative paths to the configs and singularity images.
     """
-    dl = nf_core.download.DownloadWorkflow(
-        pipeline, revision, outdir, compress, force, container, singularity_cache_only, parallel_downloads
+    from nf_core.download import DownloadWorkflow
+
+    dl = DownloadWorkflow(
+        pipeline,
+        revision,
+        outdir,
+        compress,
+        force,
+        tower,
+        download_configuration,
+        container_system,
+        container_library,
+        container_cache_utilisation,
+        container_cache_index,
+        parallel_downloads,
     )
     dl.download_workflow()
 
 
 # nf-core licences
 @nf_core_cli.command()
 @click.argument("pipeline", required=True, metavar="<pipeline name>")
@@ -252,16 +317,17 @@
     """
     List software licences for a given workflow (DSL1 only).
 
     Checks the pipeline environment.yml file which lists all conda software packages, which is not available for DSL2 workflows. Therefore, this command only supports DSL1 workflows (for now).
     Each of these is queried against the anaconda.org API to find the licence.
     Package name, version and licence is printed to the command line.
     """
+    from nf_core.licences import WorkflowLicences
 
-    lic = nf_core.licences.WorkflowLicences(pipeline)
+    lic = WorkflowLicences(pipeline)
     lic.as_json = json
     try:
         stdout.print(lic.run_licences())
     except LookupError as e:
         log.error(e)
         sys.exit(1)
 
@@ -285,18 +351,18 @@
 def create(name, description, author, version, no_git, force, outdir, template_yaml, plain):
     """
     Create a new pipeline using the nf-core template.
 
     Uses the nf-core template to make a skeleton Nextflow pipeline with all required
     files, boilerplate code and best-practices.
     """
+    from nf_core.create import PipelineCreate
+
     try:
-        create_obj = nf_core.create.PipelineCreate(
-            name, description, author, version, no_git, force, outdir, template_yaml, plain
-        )
+        create_obj = PipelineCreate(name, description, author, version, no_git, force, outdir, template_yaml, plain)
         create_obj.init_pipeline()
     except UserWarning as e:
         log.error(e)
         sys.exit(1)
 
 
 # nf-core lint
@@ -340,25 +406,27 @@
     Runs a large number of automated tests to ensure that the supplied pipeline
     meets the nf-core guidelines. Documentation of all lint tests can be found
     on the nf-core website: [link=https://nf-co.re/tools-docs/]https://nf-co.re/tools-docs/[/]
 
     You can ignore tests using a file called [blue].nf-core.yml[/] [i](if you have a good reason!)[/].
     See the documentation for details.
     """
+    from nf_core.lint import run_linting
+    from nf_core.utils import is_pipeline_directory
 
     # Check if pipeline directory is a pipeline
     try:
-        nf_core.utils.is_pipeline_directory(dir)
+        is_pipeline_directory(dir)
     except UserWarning as e:
         log.error(e)
         sys.exit(1)
 
     # Run the lint tests!
     try:
-        lint_obj, module_lint_obj = nf_core.lint.run_linting(
+        lint_obj, module_lint_obj = run_linting(
             dir,
             release,
             fix,
             key,
             show_passed,
             fail_ignored,
             fail_warned,
@@ -379,15 +447,15 @@
 
 # nf-core modules subcommands
 @nf_core_cli.group()
 @click.option(
     "-g",
     "--git-remote",
     type=str,
-    default=nf_core.modules.modules_repo.NF_CORE_MODULES_REMOTE,
+    default=NF_CORE_MODULES_REMOTE,
     help="Remote git repo to fetch files from",
 )
 @click.option("-b", "--branch", type=str, default=None, help="Branch of git repository hosting modules.")
 @click.option(
     "-N",
     "--no-pull",
     is_flag=True,
@@ -411,15 +479,15 @@
 
 # nf-core subworkflows click command
 @nf_core_cli.group()
 @click.option(
     "-g",
     "--git-remote",
     type=str,
-    default=nf_core.modules.modules_repo.NF_CORE_MODULES_REMOTE,
+    default=NF_CORE_MODULES_REMOTE,
     help="Remote git repo to fetch files from",
 )
 @click.option("-b", "--branch", type=str, default=None, help="Branch of git repository hosting modules.")
 @click.option(
     "-N",
     "--no-pull",
     is_flag=True,
@@ -456,16 +524,18 @@
 @click.pass_context
 @click.argument("keywords", required=False, nargs=-1, metavar="<filter keywords>")
 @click.option("-j", "--json", is_flag=True, help="Print as JSON to stdout")
 def remote(ctx, keywords, json):
     """
     List modules in a remote GitHub repo [dim i](e.g [link=https://github.com/nf-core/modules]nf-core/modules[/])[/].
     """
+    from nf_core.modules import ModuleList
+
     try:
-        module_list = nf_core.modules.ModuleList(
+        module_list = ModuleList(
             None,
             True,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
         stdout.print(module_list.list_components(keywords, json))
@@ -486,16 +556,18 @@
     default=".",
     help=r"Pipeline directory. [dim]\[default: Current working directory][/]",
 )
 def local(ctx, keywords, json, dir):  # pylint: disable=redefined-builtin
     """
     List modules installed locally in a pipeline
     """
+    from nf_core.modules import ModuleList
+
     try:
-        module_list = nf_core.modules.ModuleList(
+        module_list = ModuleList(
             dir,
             False,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
         stdout.print(module_list.list_components(keywords, json))
@@ -520,16 +592,18 @@
 @click.option("-s", "--sha", type=str, metavar="<commit sha>", help="Install module at commit SHA")
 def install(ctx, tool, dir, prompt, force, sha):
     """
     Install DSL2 modules within a pipeline.
 
     Fetches and installs module files from a remote repo e.g. nf-core/modules.
     """
+    from nf_core.modules import ModuleInstall
+
     try:
-        module_install = nf_core.modules.ModuleInstall(
+        module_install = ModuleInstall(
             dir,
             force,
             prompt,
             sha,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
@@ -581,16 +655,18 @@
 )
 def update(ctx, tool, dir, force, prompt, sha, all, preview, save_diff, update_deps):
     """
     Update DSL2 modules within a pipeline.
 
     Fetches and updates module files from a remote repo e.g. nf-core/modules.
     """
+    from nf_core.modules import ModuleUpdate
+
     try:
-        module_install = nf_core.modules.ModuleUpdate(
+        module_install = ModuleUpdate(
             dir,
             force,
             prompt,
             sha,
             all,
             preview,
             save_diff,
@@ -622,16 +698,18 @@
 def patch(ctx, tool, dir, remove):
     """
     Create a patch file for minor changes in a module
 
     Checks if a module has been modified locally and creates a patch file
     describing how the module has changed from the remote version
     """
+    from nf_core.modules import ModulePatch
+
     try:
-        module_patch = nf_core.modules.ModulePatch(
+        module_patch = ModulePatch(
             dir,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
         if remove:
             module_patch.remove(tool)
@@ -653,16 +731,18 @@
     default=".",
     help=r"Pipeline directory. [dim]\[default: current working directory][/]",
 )
 def remove(ctx, dir, tool):
     """
     Remove a module from a pipeline.
     """
+    from nf_core.modules import ModuleRemove
+
     try:
-        module_remove = nf_core.modules.ModuleRemove(
+        module_remove = ModuleRemove(
             dir,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
         module_remove.remove(tool)
     except (UserWarning, LookupError) as e:
@@ -706,17 +786,19 @@
     if meta and no_meta:
         log.critical("Both arguments '--meta' and '--no-meta' given. Please pick one.")
     elif meta:
         has_meta = True
     elif no_meta:
         has_meta = False
 
+    from nf_core.modules import ModuleCreate
+
     # Run function
     try:
-        module_create = nf_core.modules.ModuleCreate(
+        module_create = ModuleCreate(
             dir, tool, author, label, has_meta, force, conda_name, conda_package_version, empty_template
         )
         module_create.create()
     except UserWarning as e:
         log.critical(e)
         sys.exit(1)
     except LookupError as e:
@@ -735,16 +817,18 @@
 def create_test_yml(ctx, tool, run_tests, output, force, no_prompts):
     """
     Auto-generate a test.yml file for a new module.
 
     Given the name of a module, runs the Nextflow test command and automatically generate
     the required `test.yml` file based on the output files.
     """
+    from nf_core.modules import ModulesTestYmlBuilder
+
     try:
-        meta_builder = nf_core.modules.ModulesTestYmlBuilder(
+        meta_builder = ModulesTestYmlBuilder(
             module_name=tool,
             run_tests=run_tests,
             test_yml_output_path=output,
             force_overwrite=force,
             no_prompts=no_prompts,
             remote_url=ctx.obj["modules_repo_url"],
             branch=ctx.obj["modules_repo_branch"],
@@ -756,61 +840,74 @@
 
 
 # nf-core modules lint
 @modules.command()
 @click.pass_context
 @click.argument("tool", type=str, required=False, metavar="<tool> or <tool/subtool>")
 @click.option("-d", "--dir", type=click.Path(exists=True), default=".", metavar="<pipeline/modules directory>")
+@click.option(
+    "-r",
+    "--registry",
+    type=str,
+    metavar="<registry>",
+    default=None,
+    help="Registry to use for containers. If not specified it will use docker.registry value in the nextflow.config file",
+)
 @click.option("-k", "--key", type=str, metavar="<test>", multiple=True, help="Run only these lint tests")
 @click.option("-a", "--all", is_flag=True, help="Run on all modules")
 @click.option("-w", "--fail-warned", is_flag=True, help="Convert warn tests to failures")
 @click.option("--local", is_flag=True, help="Run additional lint tests for local modules")
 @click.option("--passed", is_flag=True, help="Show passed tests")
 @click.option(
     "--sort-by",
     type=click.Choice(["module", "test"]),
     default="test",
     help="Sort lint output by module or test name.",
     show_default=True,
 )
 @click.option("--fix-version", is_flag=True, help="Fix the module version if a newer version is available")
 def lint(
-    ctx, tool, dir, key, all, fail_warned, local, passed, sort_by, fix_version
+    ctx, tool, dir, registry, key, all, fail_warned, local, passed, sort_by, fix_version
 ):  # pylint: disable=redefined-outer-name
     """
     Lint one or more modules in a directory.
 
     Checks DSL2 module code against nf-core guidelines to ensure
     that all modules follow the same standards.
 
     Test modules within a pipeline or a clone of the
     nf-core/modules repository.
     """
+    from nf_core.modules import ModuleLint
+    from nf_core.modules.lint import ModuleLintException
+
     try:
-        module_lint = nf_core.modules.ModuleLint(
+        module_lint = ModuleLint(
             dir,
             fail_warned=fail_warned,
+            registry=ctx.params["registry"],
             remote_url=ctx.obj["modules_repo_url"],
             branch=ctx.obj["modules_repo_branch"],
             no_pull=ctx.obj["modules_repo_no_pull"],
             hide_progress=ctx.obj["hide_progress"],
         )
         module_lint.lint(
             module=tool,
+            registry=registry,
             key=key,
             all_modules=all,
             print_results=True,
             local=local,
             show_passed=passed,
             sort_by=sort_by,
             fix_version=fix_version,
         )
         if len(module_lint.failed) > 0:
             sys.exit(1)
-    except nf_core.modules.lint.ModuleLintException as e:
+    except ModuleLintException as e:
         log.error(e)
         sys.exit(1)
     except (UserWarning, LookupError) as e:
         log.critical(e)
         sys.exit(1)
 
 
@@ -833,16 +930,18 @@
     on the command line. A handy equivalent to searching the
     [link=https://nf-co.re/modules]nf-core website[/].
 
     If run from a pipeline and a local copy of the module is found, the command
     will print this usage info.
     If not, usage from the remote modules repo will be shown.
     """
+    from nf_core.modules import ModuleInfo
+
     try:
-        module_info = nf_core.modules.ModuleInfo(
+        module_info = ModuleInfo(
             dir,
             tool,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
         stdout.print(module_info.get_component_info())
@@ -859,23 +958,26 @@
 @click.option("-a", "--all", is_flag=True, help="Run on all modules")
 @click.option("-s", "--show-all", is_flag=True, help="Show up-to-date modules in results too")
 def bump_versions(ctx, tool, dir, all, show_all):
     """
     Bump versions for one or more modules in a clone of
     the nf-core/modules repo.
     """
+    from nf_core.modules.bump_versions import ModuleVersionBumper
+    from nf_core.modules.modules_utils import ModuleException
+
     try:
-        version_bumper = nf_core.modules.bump_versions.ModuleVersionBumper(
+        version_bumper = ModuleVersionBumper(
             dir,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
         version_bumper.bump_versions(module=tool, all_modules=all, show_uptodate=show_all)
-    except nf_core.modules.modules_utils.ModuleException as e:
+    except ModuleException as e:
         log.error(e)
         sys.exit(1)
     except (UserWarning, LookupError) as e:
         log.critical(e)
         sys.exit(1)
 
 
@@ -887,16 +989,18 @@
 @click.option("-a", "--pytest_args", type=str, required=False, multiple=True, help="Additional pytest arguments")
 def test_module(ctx, tool, no_prompts, pytest_args):
     """
     Run module tests locally.
 
     Given the name of a module, runs the Nextflow test command.
     """
+    from nf_core.modules import ModulesTest
+
     try:
-        meta_builder = nf_core.modules.ModulesTest(tool, no_prompts, pytest_args)
+        meta_builder = ModulesTest(tool, no_prompts, pytest_args)
         meta_builder.run()
     except (UserWarning, LookupError) as e:
         log.critical(e)
         sys.exit(1)
 
 
 # nf-core subworkflows create
@@ -912,18 +1016,19 @@
 
     If the specified directory is a pipeline, this function creates a file called
     'subworkflows/local/<subworkflow_name>.nf'
 
     If the specified directory is a clone of nf-core/modules, it creates or modifies files
     in 'subworkflows/', 'tests/subworkflows' and 'tests/config/pytest_modules.yml'
     """
+    from nf_core.subworkflows import SubworkflowCreate
 
     # Run function
     try:
-        subworkflow_create = nf_core.subworkflows.SubworkflowCreate(dir, subworkflow, author, force)
+        subworkflow_create = SubworkflowCreate(dir, subworkflow, author, force)
         subworkflow_create.create()
     except UserWarning as e:
         log.critical(e)
         sys.exit(1)
     except LookupError as e:
         log.error(e)
         sys.exit(1)
@@ -940,16 +1045,18 @@
 def create_test_yml(ctx, subworkflow, run_tests, output, force, no_prompts):
     """
     Auto-generate a test.yml file for a new subworkflow.
 
     Given the name of a module, runs the Nextflow test command and automatically generate
     the required `test.yml` file based on the output files.
     """
+    from nf_core.subworkflows import SubworkflowTestYmlBuilder
+
     try:
-        meta_builder = nf_core.subworkflows.SubworkflowTestYmlBuilder(
+        meta_builder = SubworkflowTestYmlBuilder(
             subworkflow=subworkflow,
             run_tests=run_tests,
             test_yml_output_path=output,
             force_overwrite=force,
             no_prompts=no_prompts,
             remote_url=ctx.obj["modules_repo_url"],
             branch=ctx.obj["modules_repo_branch"],
@@ -975,23 +1082,26 @@
 @click.pass_context
 @click.argument("keywords", required=False, nargs=-1, metavar="<filter keywords>")
 @click.option("-j", "--json", is_flag=True, help="Print as JSON to stdout")
 def remote(ctx, keywords, json):
     """
     List subworkflows in a remote GitHub repo [dim i](e.g [link=https://github.com/nf-core/modules]nf-core/modules[/])[/].
     """
+    from nf_core.subworkflows import SubworkflowList
+
     try:
-        subworkflows_list = nf_core.subworkflows.SubworkflowList(
+        subworkflow_list = SubworkflowList(
             None,
             True,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
-        stdout.print(subworkflows_list.list_subworkflows(keywords, json))
+
+        stdout.print(subworkflow_list.list_components(keywords, json))
     except (UserWarning, LookupError) as e:
         log.critical(e)
         sys.exit(1)
 
 
 # nf-core subworkflows list local
 @list.command()
@@ -1005,23 +1115,25 @@
     default=".",
     help=r"Pipeline directory. [dim]\[default: Current working directory][/]",
 )
 def local(ctx, keywords, json, dir):  # pylint: disable=redefined-builtin
     """
     List subworkflows installed locally in a pipeline
     """
+    from nf_core.subworkflows import SubworkflowList
+
     try:
-        subworkflows_list = nf_core.subworkflows.SubworkflowList(
+        subworkflow_list = SubworkflowList(
             dir,
             False,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
-        stdout.print(subworkflows_list.list_subworkflows(keywords, json))
+        stdout.print(subworkflow_list.list_components(keywords, json))
     except (UserWarning, LookupError) as e:
         log.error(e)
         sys.exit(1)
 
 
 # nf-core subworkflows info
 @subworkflows.command()
@@ -1042,16 +1154,18 @@
     on the command line. A handy equivalent to searching the
     [link=https://nf-co.re/modules]nf-core website[/].
 
     If run from a pipeline and a local copy of the subworkflow is found, the command
     will print this usage info.
     If not, usage from the remote subworkflows repo will be shown.
     """
+    from nf_core.subworkflows import SubworkflowInfo
+
     try:
-        subworkflow_info = nf_core.subworkflows.SubworkflowInfo(
+        subworkflow_info = SubworkflowInfo(
             dir,
             tool,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
         stdout.print(subworkflow_info.get_component_info())
@@ -1068,16 +1182,18 @@
 @click.option("-a", "--pytest_args", type=str, required=False, multiple=True, help="Additional pytest arguments")
 def test_subworkflow(ctx, subworkflow, no_prompts, pytest_args):
     """
     Run subworkflow tests locally.
 
     Given the name of a subworkflow, runs the Nextflow test command.
     """
+    from nf_core.subworkflows import SubworkflowsTest
+
     try:
-        meta_builder = nf_core.subworkflows.SubworkflowsTest(subworkflow, no_prompts, pytest_args)
+        meta_builder = SubworkflowsTest(subworkflow, no_prompts, pytest_args)
         meta_builder.run()
     except (UserWarning, LookupError) as e:
         log.critical(e)
         sys.exit(1)
 
 
 # nf-core subworkflows install
@@ -1098,16 +1214,18 @@
 @click.option("-s", "--sha", type=str, metavar="<commit sha>", help="Install subworkflow at commit SHA")
 def install(ctx, subworkflow, dir, prompt, force, sha):
     """
     Install DSL2 subworkflow within a pipeline.
 
     Fetches and installs subworkflow files from a remote repo e.g. nf-core/modules.
     """
+    from nf_core.subworkflows import SubworkflowInstall
+
     try:
-        subworkflow_install = nf_core.subworkflows.SubworkflowInstall(
+        subworkflow_install = SubworkflowInstall(
             dir,
             force,
             prompt,
             sha,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
@@ -1117,78 +1235,14 @@
             sys.exit(1)
     except (UserWarning, LookupError) as e:
         log.error(e)
         raise
         sys.exit(1)
 
 
-# nf-core subworkflows list subcommands
-@subworkflows.group()
-@click.pass_context
-def list(ctx):
-    """
-    List modules in a local pipeline or remote repository.
-    """
-    pass
-
-
-# nf-core subworkflows list remote
-@list.command()
-@click.pass_context
-@click.argument("keywords", required=False, nargs=-1, metavar="<filter keywords>")
-@click.option("-j", "--json", is_flag=True, help="Print as JSON to stdout")
-def remote(ctx, keywords, json):
-    """
-    List subworkflows in a remote GitHub repo [dim i](e.g [link=https://github.com/nf-core/modules]nf-core/modules[/])[/].
-    """
-    try:
-        subworkflow_list = nf_core.subworkflows.SubworkflowList(
-            None,
-            True,
-            ctx.obj["modules_repo_url"],
-            ctx.obj["modules_repo_branch"],
-            ctx.obj["modules_repo_no_pull"],
-        )
-
-        stdout.print(subworkflow_list.list_components(keywords, json))
-    except (UserWarning, LookupError) as e:
-        log.critical(e)
-        sys.exit(1)
-
-
-# nf-core subworkflows list local
-@list.command()
-@click.pass_context
-@click.argument("keywords", required=False, nargs=-1, metavar="<filter keywords>")
-@click.option("-j", "--json", is_flag=True, help="Print as JSON to stdout")
-@click.option(
-    "-d",
-    "--dir",
-    type=click.Path(exists=True),
-    default=".",
-    help=r"Pipeline directory. [dim]\[default: Current working directory][/]",
-)
-def local(ctx, keywords, json, dir):  # pylint: disable=redefined-builtin
-    """
-    List subworkflows installed locally in a pipeline
-    """
-    try:
-        subworkflow_list = nf_core.subworkflows.SubworkflowList(
-            dir,
-            False,
-            ctx.obj["modules_repo_url"],
-            ctx.obj["modules_repo_branch"],
-            ctx.obj["modules_repo_no_pull"],
-        )
-        stdout.print(subworkflow_list.list_components(keywords, json))
-    except (UserWarning, LookupError) as e:
-        log.error(e)
-        sys.exit(1)
-
-
 # nf-core subworkflows remove
 @subworkflows.command()
 @click.pass_context
 @click.argument("subworkflow", type=str, required=False, metavar="subworkflow name")
 @click.option(
     "-d",
     "--dir",
@@ -1196,16 +1250,18 @@
     default=".",
     help=r"Pipeline directory. [dim]\[default: current working directory][/]",
 )
 def remove(ctx, dir, subworkflow):
     """
     Remove a subworkflow from a pipeline.
     """
+    from nf_core.subworkflows import SubworkflowRemove
+
     try:
-        module_remove = nf_core.subworkflows.SubworkflowRemove(
+        module_remove = SubworkflowRemove(
             dir,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
         module_remove.remove(subworkflow)
     except (UserWarning, LookupError) as e:
@@ -1252,16 +1308,18 @@
 )
 def update(ctx, subworkflow, dir, force, prompt, sha, all, preview, save_diff, update_deps):
     """
     Update DSL2 subworkflow within a pipeline.
 
     Fetches and updates subworkflow files from a remote repo e.g. nf-core/modules.
     """
+    from nf_core.subworkflows import SubworkflowUpdate
+
     try:
-        subworkflow_install = nf_core.subworkflows.SubworkflowUpdate(
+        subworkflow_install = SubworkflowUpdate(
             dir,
             force,
             prompt,
             sha,
             all,
             preview,
             save_diff,
@@ -1300,15 +1358,17 @@
 
     Nextflow can be run using the -params-file flag, which loads
     script parameters from a JSON file.
 
     This command takes such a file and validates it against the pipeline
     schema, checking whether all schema rules are satisfied.
     """
-    schema_obj = nf_core.schema.PipelineSchema()
+    from nf_core.schema import PipelineSchema
+
+    schema_obj = PipelineSchema()
     try:
         schema_obj.get_schema_path(pipeline)
         # Load and check schema
         schema_obj.load_lint_schema()
     except AssertionError as e:
         log.error(e)
         sys.exit(1)
@@ -1344,16 +1404,18 @@
     compares these to the pipeline schema. Prompts to add or remove parameters
     if the two do not match one another.
 
     Once all parameters are accounted for, can launch a web GUI tool on the
     https://nf-co.re website where you can annotate and organise parameters.
     Listens for this to be completed and saves the updated schema.
     """
+    from nf_core.schema import PipelineSchema
+
     try:
-        schema_obj = nf_core.schema.PipelineSchema()
+        schema_obj = PipelineSchema()
         if schema_obj.build_schema(dir, no_prompts, web_only, url) is False:
             sys.exit(1)
     except (UserWarning, AssertionError) as e:
         log.error(e)
         sys.exit(1)
 
 
@@ -1370,15 +1432,17 @@
     and adheres to the additional nf-core schema requirements.
 
     This function runs as part of the nf-core lint command, this is a convenience
     command that does just the schema linting nice and quickly.
 
     If no schema path is provided, "nextflow_schema.json" will be used (if it exists).
     """
-    schema_obj = nf_core.schema.PipelineSchema()
+    from nf_core.schema import PipelineSchema
+
+    schema_obj = PipelineSchema()
     try:
         schema_obj.get_schema_path(schema_path)
         schema_obj.load_lint_schema()
         # Validate title and description - just warnings as schema should still work fine
         try:
             schema_obj.validate_schema_title_description()
         except AssertionError as e:
@@ -1412,15 +1476,17 @@
     """
     Outputs parameter documentation for a pipeline schema.
     """
     if not os.path.exists(schema_path):
         log.error("Could not find 'nextflow_schema.json' in current directory. Please specify a path.")
         sys.exit(1)
 
-    schema_obj = nf_core.schema.PipelineSchema()
+    from nf_core.schema import PipelineSchema
+
+    schema_obj = PipelineSchema()
     # Assume we're in a pipeline dir root if schema path not set
     schema_obj.get_schema_path(schema_path)
     schema_obj.load_schema()
     schema_obj.print_documentation(output, format, force, columns.split(","))
 
 
 # nf-core bump-version
@@ -1445,27 +1511,30 @@
     so that you don't accidentally miss any.
 
     Should be used for each pipeline release, and again for the next
     development version after release.
 
     As well as the pipeline version, you can also change the required version of Nextflow.
     """
+    from nf_core.bump_version import bump_nextflow_version, bump_pipeline_version
+    from nf_core.utils import Pipeline, is_pipeline_directory
+
     try:
         # Check if pipeline directory contains necessary files
-        nf_core.utils.is_pipeline_directory(dir)
+        is_pipeline_directory(dir)
 
         # Make a pipeline object and load config etc
-        pipeline_obj = nf_core.utils.Pipeline(dir)
+        pipeline_obj = Pipeline(dir)
         pipeline_obj._load()
 
         # Bump the pipeline version number
         if not nextflow:
-            nf_core.bump_version.bump_pipeline_version(pipeline_obj, new_version)
+            bump_pipeline_version(pipeline_obj, new_version)
         else:
-            nf_core.bump_version.bump_nextflow_version(pipeline_obj, new_version)
+            bump_nextflow_version(pipeline_obj, new_version)
     except UserWarning as e:
         log.error(e)
         sys.exit(1)
 
 
 # nf-core sync
 @nf_core_cli.command("sync")
@@ -1490,22 +1559,25 @@
     git branch called [cyan i]TEMPLATE[/].
 
     This command updates the [cyan i]TEMPLATE[/] branch with the latest version of
     the nf-core template, so that these updates can be synchronised with
     the pipeline. It is run automatically for all pipelines when ever a
     new release of [link=https://github.com/nf-core/tools]nf-core/tools[/link] (and the included template) is made.
     """
+    from nf_core.sync import PipelineSync, PullRequestException, SyncException
+    from nf_core.utils import is_pipeline_directory
+
     # Check if pipeline directory contains necessary files
-    nf_core.utils.is_pipeline_directory(dir)
+    is_pipeline_directory(dir)
 
     # Sync the given pipeline dir
-    sync_obj = nf_core.sync.PipelineSync(dir, from_branch, pull_request, github_repository, username, template_yaml)
+    sync_obj = PipelineSync(dir, from_branch, pull_request, github_repository, username, template_yaml)
     try:
         sync_obj.sync()
-    except (nf_core.sync.SyncException, nf_core.sync.PullRequestException) as e:
+    except (SyncException, PullRequestException) as e:
         log.error(e)
         sys.exit(1)
 
 
 # Main script is being run - launch the CLI
 if __name__ == "__main__":
     run_nf_core()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nf-core-2.8/nf_core/bump_version.py` & `nf-core-2.9/nf_core/bump_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Bumps the version number in all appropriate files for
 a nf-core pipeline.
 """
 
 import logging
-import os
 import re
+from pathlib import Path
 
 import rich.console
 
 import nf_core.utils
 
 log = logging.getLogger(__name__)
 stderr = rich.console.Console(stderr=True, force_terminal=nf_core.utils.rich_force_colors())
@@ -40,14 +40,25 @@
         [
             (
                 rf"version\s*=\s*[\'\"]?{re.escape(current_version)}[\'\"]?",
                 f"version = '{new_version}'",
             )
         ],
     )
+    # multiqc_config.yaml
+    update_file_version(
+        Path("assets", "multiqc_config.yml"),
+        pipeline_obj,
+        [
+            (
+                rf"{re.escape(current_version)}",
+                f"{new_version}",
+            )
+        ],
+    )
 
 
 def bump_nextflow_version(pipeline_obj, new_version):
     """Bumps the required Nextflow version number of a pipeline.
 
     Args:
         pipeline_obj (nf_core.utils.Pipeline): A `Pipeline` object that holds information
@@ -73,15 +84,15 @@
                 f"nextflowVersion = '!>={new_version}'",
             )
         ],
     )
 
     # .github/workflows/ci.yml - Nextflow version matrix
     update_file_version(
-        os.path.join(".github", "workflows", "ci.yml"),
+        Path(".github", "workflows", "ci.yml"),
         pipeline_obj,
         [
             (
                 # example:
                 # NXF_VER:
                 #   - "20.04.0"
                 rf"- [\"]{re.escape(current_version)}[\"]",
```

### Comparing `nf-core-2.8/nf_core/components/components_command.py` & `nf-core-2.9/nf_core/components/components_command.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/components/components_test.py` & `nf-core-2.9/nf_core/components/components_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 from pathlib import Path
 from shutil import which
 
 import pytest
 import questionary
 import rich
+from git import InvalidGitRepositoryError, Repo
 
 import nf_core.modules.modules_utils
 import nf_core.utils
 from nf_core.components.components_command import ComponentCommand
 from nf_core.modules.modules_json import ModulesJson
 
 log = logging.getLogger(__name__)
@@ -175,14 +176,22 @@
 
     def _run_pytests(self):
         """Given a module/subworkflow name, run tests."""
         # Print nice divider line
         console = rich.console.Console()
         console.rule(self.component_name, style="black")
 
+        # Check uncommitted changed
+        try:
+            repo = Repo(self.dir)
+            if repo.is_dirty():
+                log.warning("You have uncommitted changes. Make sure to commit last changes before running the tests.")
+        except InvalidGitRepositoryError:
+            pass
+
         # Set pytest arguments
         tag = self.component_name
         if self.component_type == "subworkflows":
             tag = "subworkflows/" + tag
         command_args = ["--tag", f"{tag}", "--symlink", "--keep-workflow-wd", "--git-aware"]
         command_args += self.pytest_args
```

### Comparing `nf-core-2.8/nf_core/components/components_utils.py` & `nf-core-2.9/nf_core/components/components_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/components/create.py` & `nf-core-2.9/nf_core/components/create.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/components/info.py` & `nf-core-2.9/nf_core/components/info.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/components/install.py` & `nf-core-2.9/nf_core/components/install.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/components/list.py` & `nf-core-2.9/nf_core/components/list.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/components/remove.py` & `nf-core-2.9/nf_core/components/remove.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/components/update.py` & `nf-core-2.9/nf_core/components/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,24 +302,14 @@
                             default=True,
                             style=nf_core.utils.nfcore_question_style,
                         ).unsafe_ask()
                 if recursive_update and len(modules_to_update + subworkflows_to_update) > 0:
                     # Update linked components
                     self.update_linked_components(modules_to_update, subworkflows_to_update, updated)
                     self.manage_changes_in_linked_components(component, modules_to_update, subworkflows_to_update)
-            else:
-                # Don't save to a file, just iteratively update the variable
-                self.modules_json.update(
-                    self.component_type,
-                    modules_repo,
-                    component,
-                    version,
-                    installed_by=None,
-                    write_file=False,
-                )
 
         if self.save_diff_fn:
             # Write the modules.json diff to the file
             ModulesDiffer.append_modules_json_diff(
                 self.save_diff_fn,
                 old_modules_json,
                 self.modules_json.get_modules_json(),
```

### Comparing `nf-core-2.8/nf_core/create.py` & `nf-core-2.9/nf_core/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,18 @@
         # Now look in the template for more options, otherwise default to nf-core defaults
         param_dict["prefix"] = template_yaml.get("prefix", "nf-core")
         param_dict["branded"] = param_dict["prefix"] == "nf-core"
 
         skip_paths = [] if param_dict["branded"] else ["branded"]
 
         for t_area in template_areas:
-            if t_area in template_yaml.get("skip", []):
+            areas_to_skip = template_yaml.get("skip", [])
+            if isinstance(areas_to_skip, str):
+                areas_to_skip = [areas_to_skip]
+            if t_area in areas_to_skip:
                 if template_areas[t_area]["file"]:
                     skip_paths.append(t_area)
                 param_dict[t_area] = False
             else:
                 param_dict[t_area] = True
         # If github is selected, exclude also github_badges
         if not param_dict["github"]:
@@ -348,14 +351,15 @@
             # Update the .nf-core.yml with linting configurations
             self.fix_linting()
 
         log.debug("Dumping pipeline template yml to file")
         if self.template_yaml:
             with open(self.outdir / "pipeline_template.yml", "w") as fh:
                 yaml.safe_dump(self.template_yaml, fh)
+            run_prettier_on_file(self.outdir / "pipeline_template.yml")
 
     def update_nextflow_schema(self):
         """
         Removes unused parameters from the nextflow schema.
         """
         schema_path = self.outdir / "nextflow_schema.json"
 
@@ -399,29 +403,52 @@
                 f"assets/nf-core-{short_name}_logo_light.png",
                 f"docs/images/nf-core-{short_name}_logo_light.png",
                 f"docs/images/nf-core-{short_name}_logo_dark.png",
                 ".github/ISSUE_TEMPLATE/config.yml",
                 ".github/workflows/awstest.yml",
                 ".github/workflows/awsfulltest.yml",
             ],
+            "files_unchanged": [
+                "CODE_OF_CONDUCT.md",
+                f"assets/nf-core-{short_name}_logo_light.png",
+                f"docs/images/nf-core-{short_name}_logo_light.png",
+                f"docs/images/nf-core-{short_name}_logo_dark.png",
+            ],
             "nextflow_config": [
                 "manifest.name",
                 "manifest.homePage",
             ],
             "multiqc_config": ["report_comment"],
         }
 
         # Add GitHub hosting specific configurations
         if not self.template_params["github"]:
             lint_config["files_exist"].extend(
                 [
                     ".github/ISSUE_TEMPLATE/bug_report.yml",
+                    ".github/ISSUE_TEMPLATE/feature_request.yml",
+                    ".github/PULL_REQUEST_TEMPLATE.md",
+                    ".github/CONTRIBUTING.md",
+                    ".github/.dockstore.yml",
+                    ".gitignore",
+                ]
+            )
+            lint_config["files_unchanged"].extend(
+                [
+                    ".github/ISSUE_TEMPLATE/bug_report.yml",
+                    ".github/ISSUE_TEMPLATE/config.yml",
+                    ".github/ISSUE_TEMPLATE/feature_request.yml",
+                    ".github/PULL_REQUEST_TEMPLATE.md",
+                    ".github/workflows/branch.yml",
+                    ".github/workflows/linting_comment.yml",
+                    ".github/workflows/linting.yml",
+                    ".github/CONTRIBUTING.md",
+                    ".github/.dockstore.yml",
                 ]
             )
-            lint_config["files_unchanged"] = [".github/ISSUE_TEMPLATE/bug_report.yml"]
 
         # Add CI specific configurations
         if not self.template_params["ci"]:
             lint_config["files_exist"].extend(
                 [
                     ".github/workflows/branch.yml",
                     ".github/workflows/ci.yml",
@@ -438,18 +465,26 @@
                     "process.cpus",
                     "process.memory",
                     "process.time",
                     "custom_config",
                 ]
             )
 
+        # Add igenomes specific configurations
+        if not self.template_params["igenomes"]:
+            lint_config["files_exist"].extend(["conf/igenomes.config"])
+
         # Add github badges specific configurations
         if not self.template_params["github_badges"] or not self.template_params["github"]:
             lint_config["readme"] = ["nextflow_badge"]
 
+        # If the pipeline is unbranded
+        if not self.template_params["branded"]:
+            lint_config["files_unchanged"].extend([".github/ISSUE_TEMPLATE/bug_report.yml"])
+
         # Add the lint content to the preexisting nf-core config
         config_fn, nf_core_yml = nf_core.utils.load_tools_config(self.outdir)
         nf_core_yml["lint"] = lint_config
         with open(self.outdir / config_fn, "w") as fh:
             yaml.dump(nf_core_yml, fh, default_flow_style=False, sort_keys=False)
 
         run_prettier_on_file(os.path.join(self.outdir, config_fn))
@@ -457,15 +492,15 @@
     def make_pipeline_logo(self):
         """Fetch a logo for the new pipeline from the nf-core website"""
 
         logo_url = f"https://nf-co.re/logo/{self.template_params['short_name']}?theme=light"
         log.debug(f"Fetching logo from {logo_url}")
 
         email_logo_path = self.outdir / "assets" / f"{self.template_params['name_noslash']}_logo_light.png"
-        self.download_pipeline_logo(f"{logo_url}&w=400", email_logo_path)
+        self.download_pipeline_logo(f"{logo_url}?w=600&theme=light", email_logo_path)
         for theme in ["dark", "light"]:
             readme_logo_url = f"{logo_url}?w=600&theme={theme}"
             readme_logo_path = (
                 self.outdir / "docs" / "images" / f"{self.template_params['name_noslash']}_logo_{theme}.png"
             )
             self.download_pipeline_logo(readme_logo_url, readme_logo_path)
```

### Comparing `nf-core-2.8/nf_core/launch.py` & `nf-core-2.9/nf_core/launch.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/licences.py` & `nf-core-2.9/nf_core/licences.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/__init__.py` & `nf-core-2.9/nf_core/lint/__init__.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/actions_awsfulltest.py` & `nf-core-2.9/nf_core/lint/actions_awsfulltest.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/actions_awstest.py` & `nf-core-2.9/nf_core/lint/actions_awstest.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/actions_ci.py` & `nf-core-2.9/nf_core/lint/actions_ci.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/actions_schema_validation.py` & `nf-core-2.9/nf_core/lint/actions_schema_validation.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/files_exist.py` & `nf-core-2.9/nf_core/lint/files_exist.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         CODE_OF_CONDUCT.md
         docs/images/nf-core-PIPELINE_logo_light.png
         docs/images/nf-core-PIPELINE_logo_dark.png
         docs/output.md
         docs/README.md
         docs/usage.md
         lib/nfcore_external_java_deps.jar
-        lib/NfcoreSchema.groovy
         lib/NfcoreTemplate.groovy
         lib/Utils.groovy
         lib/WorkflowMain.groovy
         nextflow_schema.json
         nextflow.config
         README.md
 
@@ -157,15 +156,14 @@
         [os.path.join("docs", "images", f"nf-core-{short_name}_logo_light.png")],
         [os.path.join("docs", "images", f"nf-core-{short_name}_logo_dark.png")],
         [os.path.join("docs", "output.md")],
         [os.path.join("docs", "README.md")],
         [os.path.join("docs", "README.md")],
         [os.path.join("docs", "usage.md")],
         [os.path.join("lib", "nfcore_external_java_deps.jar")],
-        [os.path.join("lib", "NfcoreSchema.groovy")],
         [os.path.join("lib", "NfcoreTemplate.groovy")],
         [os.path.join("lib", "Utils.groovy")],
         [os.path.join("lib", "WorkflowMain.groovy")],
     ]
 
     files_warn = [
         ["main.nf"],
```

### Comparing `nf-core-2.8/nf_core/lint/files_unchanged.py` & `nf-core-2.9/nf_core/lint/files_unchanged.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         assets/nf-core-PIPELINE_logo_light.png
         assets/sendmail_template.txt
         CODE_OF_CONDUCT.md
         docs/images/nf-core-PIPELINE_logo_light.png
         docs/images/nf-core-PIPELINE_logo_dark.png
         docs/README.md'
         lib/nfcore_external_java_deps.jar
-        lib/NfcoreSchema.groovy
         lib/NfcoreTemplate.groovy
         ['LICENSE', 'LICENSE.md', 'LICENCE', 'LICENCE.md'], # NB: British / American spelling
 
     Files that can have additional content but must include the template contents::
 
         .gitignore
         .prettierignore
@@ -101,15 +100,14 @@
         [os.path.join("assets", "email_template.txt")],
         [os.path.join("assets", "sendmail_template.txt")],
         [os.path.join("assets", f"nf-core-{short_name}_logo_light.png")],
         [os.path.join("docs", "images", f"nf-core-{short_name}_logo_light.png")],
         [os.path.join("docs", "images", f"nf-core-{short_name}_logo_dark.png")],
         [os.path.join("docs", "README.md")],
         [os.path.join("lib", "nfcore_external_java_deps.jar")],
-        [os.path.join("lib", "NfcoreSchema.groovy")],
         [os.path.join("lib", "NfcoreTemplate.groovy")],
     ]
     files_partial = [
         [".gitignore", ".prettierignore", "pyproject.toml"],
     ]
 
     # Only show error messages from pipeline creation
```

### Comparing `nf-core-2.8/nf_core/lint/merge_markers.py` & `nf-core-2.9/nf_core/lint/merge_markers.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/modules_json.py` & `nf-core-2.9/nf_core/lint/modules_json.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/modules_structure.py` & `nf-core-2.9/nf_core/lint/modules_structure.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/multiqc_config.py` & `nf-core-2.9/nf_core/lint/multiqc_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,21 @@
         failed.append(f"'assets/multiqc_config.yml' does not meet requirements: {e}")
     else:
         passed.append("'assets/multiqc_config.yml' follows the ordering scheme of the minimally required plugins.")
 
     if "report_comment" not in ignore_configs:
         # Check that the minimum plugins exist and are coming first in the summary
         try:
+            version = self.nf_config.get("manifest.version", "").strip(" '\"")
             if "report_comment" not in mqc_yml:
                 raise AssertionError()
             if mqc_yml["report_comment"].strip() != (
-                f'This report has been generated by the <a href="https://github.com/nf-core/{self.pipeline_name}" '
+                f'This report has been generated by the <a href="https://github.com/nf-core/{self.pipeline_name}/{version}" '
                 f'target="_blank">nf-core/{self.pipeline_name}</a> analysis pipeline. For information about how to '
-                f'interpret these results, please see the <a href="https://nf-co.re/{self.pipeline_name}" '
+                f'interpret these results, please see the <a href="https://nf-co.re/{self.pipeline_name}/{version}/output" '
                 'target="_blank">documentation</a>.'
             ):
                 raise AssertionError()
         except (AssertionError, KeyError, TypeError):
             failed.append("'assets/multiqc_config.yml' does not contain a matching 'report_comment'.")
         else:
             passed.append("'assets/multiqc_config.yml' contains a matching 'report_comment'.")
```

### Comparing `nf-core-2.8/nf_core/lint/nextflow_config.py` & `nf-core-2.9/nf_core/lint/nextflow_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,19 +58,19 @@
         * Should always be set to default value ``master``
 
     * ``params.custom_config_base``
 
         * Should always be set to default value:
         ``https://raw.githubusercontent.com/nf-core/configs/${params.custom_config_version}``
 
-    * ``params.show_hidden_params``
+    * ``params.validationShowHiddenParams``
 
         * Determines whether boilerplate params are showed by schema. Set to ``false`` by default
 
-    * ``params.schema_ignore_params``
+    * ``params.validationSchemaIgnoreParams``
 
         * A comma separated string of inputs the schema validation should ignore.
 
     **The following variables throw warnings if missing:**
 
     * ``manifest.mainScript``: The filename of the main pipeline script (should be ``main.nf``)
     * ``timeline.file``, ``trace.file``, ``report.file``, ``dag.file``
@@ -126,16 +126,16 @@
         ["report.enabled"],
         ["dag.enabled"],
         ["process.cpus"],
         ["process.memory"],
         ["process.time"],
         ["params.outdir"],
         ["params.input"],
-        ["params.show_hidden_params"],
-        ["params.schema_ignore_params"],
+        ["params.validationShowHiddenParams"],
+        ["params.validationSchemaIgnoreParams"],
     ]
     # Throw a warning if these are missing
     config_warn = [
         ["manifest.mainScript"],
         ["timeline.file"],
         ["trace.file"],
         ["report.file"],
```

### Comparing `nf-core-2.8/nf_core/lint/pipeline_name_conventions.py` & `nf-core-2.9/nf_core/lint/pipeline_name_conventions.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/pipeline_todos.py` & `nf-core-2.9/nf_core/lint/pipeline_todos.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/readme.py` & `nf-core-2.9/nf_core/lint/readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ignore_configs = self.lint_config.get("readme", [])
 
     with open(os.path.join(self.wf_path, "README.md"), "r") as fh:
         content = fh.read()
 
     if "nextflow_badge" not in ignore_configs:
         # Check that there is a readme badge showing the minimum required version of Nextflow
-        # [![Nextflow](https://img.shields.io/badge/nextflow%20DSL2-%E2%89%A522.10.1-23aa62.svg)](https://www.nextflow.io/)
+        # [![Nextflow](https://img.shields.io/badge/nextflow%20DSL2-%E2%89%A523.04.0-23aa62.svg)](https://www.nextflow.io/)
         # and that it has the correct version
         nf_badge_re = r"\[!\[Nextflow\]\(https://img\.shields\.io/badge/nextflow%20DSL2-!?(?:%E2%89%A5|%3E%3D)([\d\.]+)-23aa62\.svg\)\]\(https://www\.nextflow\.io/\)"
         match = re.search(nf_badge_re, content)
         if match:
             nf_badge_version = match.group(1).strip("'\"")
             try:
                 if nf_badge_version != self.minNextflowVersion:
```

### Comparing `nf-core-2.8/nf_core/lint/schema_description.py` & `nf-core-2.9/nf_core/lint/schema_description.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/schema_lint.py` & `nf-core-2.9/nf_core/lint/schema_lint.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/schema_params.py` & `nf-core-2.9/nf_core/lint/schema_params.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/system_exit.py` & `nf-core-2.9/nf_core/lint/system_exit.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/template_strings.py` & `nf-core-2.9/nf_core/lint/template_strings.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint/version_consistency.py` & `nf-core-2.9/nf_core/lint/version_consistency.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/lint_utils.py` & `nf-core-2.9/nf_core/lint_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/list.py` & `nf-core-2.9/nf_core/list.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/module-template/modules/main.nf` & `nf-core-2.9/nf_core/module-template/modules/main.nf`

 * *Files 10% similar despite different names*

```diff
@@ -90,8 +90,30 @@
     {%- endif %}
 
     cat <<-END_VERSIONS > versions.yml
     "${task.process}":
         {{ tool }}: \$(echo \$(samtools --version 2>&1) | sed 's/^.*samtools //; s/Using.*\$//' ))
     END_VERSIONS
     """
+
+    stub:
+    def args = task.ext.args ?: ''
+    {% if has_meta -%}
+    def prefix = task.ext.prefix ?: "${meta.id}"
+    {%- endif %}
+    {% if not_empty_template -%}
+    // TODO nf-core: A stub section should mimic the execution of the original module as best as possible
+    //               Have a look at the following examples:
+    //               Simple example: https://github.com/nf-core/modules/blob/818474a292b4860ae8ff88e149fbcda68814114d/modules/nf-core/bcftools/annotate/main.nf#L47-L63
+    //               Complex example: https://github.com/nf-core/modules/blob/818474a292b4860ae8ff88e149fbcda68814114d/modules/nf-core/bedtools/split/main.nf#L38-L54
+    {%- endif %}
+    """
+    {% if not_empty_template -%}
+    touch ${prefix}.bam
+    {%- endif %}
+
+    cat <<-END_VERSIONS > versions.yml
+    "${task.process}":
+        {{ tool }}: \$(echo \$(samtools --version 2>&1) | sed 's/^.*samtools //; s/Using.*\$//' ))
+    END_VERSIONS
+    """
 }
```

### Comparing `nf-core-2.8/nf_core/module-template/modules/meta.yml` & `nf-core-2.9/nf_core/module-template/modules/meta.yml`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 {% endif -%}
 input:
   #{% if has_meta %} Only when we have meta
   - meta:
       type: map
       description: |
         Groovy Map containing sample information
-        e.g. [ id:'test', single_end:false ]
+        e.g. `[ id:'test', single_end:false ]`
   {% endif %}
   {% if not_empty_template -%}
   ## TODO nf-core: Delete / customise this example input
   {%- endif %}
   - {{ 'bam:' if not_empty_template else "input:" }}
       type: file
       description: {{ 'Sorted BAM/CRAM/SAM file' if not_empty_template else "" }}
@@ -45,15 +45,15 @@
 {% endif -%}
 output:
   #{% if has_meta -%} Only when we have meta
   - meta:
       type: map
       description: |
         Groovy Map containing sample information
-        e.g. [ id:'test', single_end:false ]
+        e.g. `[ id:'test', single_end:false ]`
   {% endif %}
   - versions:
       type: file
       description: File containing software versions
       pattern: "versions.yml"
   {% if not_empty_template -%}
   ## TODO nf-core: Delete / customise this example output
```

### Comparing `nf-core-2.8/nf_core/module-template/tests/main.nf` & `nf-core-2.9/nf_core/module-template/tests/main.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/module-template/tests/test.yml` & `nf-core-2.9/nf_core/module-template/tests/test.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/bump_versions.py` & `nf-core-2.9/nf_core/modules/bump_versions.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/create.py` & `nf-core-2.9/nf_core/modules/create.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/install.py` & `nf-core-2.9/nf_core/modules/install.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/lint/__init__.py` & `nf-core-2.9/nf_core/modules/lint/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     def __init__(
         self,
         dir,
         fail_warned=False,
         remote_url=None,
         branch=None,
         no_pull=False,
+        registry=None,
         hide_progress=False,
     ):
         super().__init__(
             "modules",
             dir=dir,
             remote_url=remote_url,
             branch=branch,
@@ -110,24 +111,34 @@
             if local_module_dir.exists():
                 self.all_local_modules = [
                     NFCoreModule(
                         m, None, Path(local_module_dir, m), self.repo_type, Path(self.dir), remote_module=False
                     )
                     for m in self.get_local_components()
                 ]
+            self.config = nf_core.utils.fetch_wf_config(self.dir, cache_config=True)
         else:
             module_dir = Path(self.dir, self.default_modules_path)
             self.all_remote_modules = [
                 NFCoreModule(m, None, module_dir / m, self.repo_type, Path(self.dir))
                 for m in self.get_components_clone_modules()
             ]
             self.all_local_modules = []
             if not self.all_remote_modules:
                 raise LookupError("No modules in 'modules' directory")
 
+            # This could be better, perhaps glob for all nextflow.config files in?
+            self.config = nf_core.utils.fetch_wf_config(Path(self.dir).joinpath("tests", "config"), cache_config=True)
+
+        if registry is None:
+            self.registry = self.config.get("docker.registry", "quay.io")
+        else:
+            self.registry = registry
+        log.debug(f"Registry set to {self.registry}")
+
         self.lint_config = None
         self.modules_json = None
 
     @staticmethod
     def get_all_lint_tests(is_pipeline):
         if is_pipeline:
             return [
@@ -141,14 +152,15 @@
             ]
         else:
             return ["main_nf", "meta_yml", "module_todos", "module_deprecations", "module_tests"]
 
     def lint(
         self,
         module=None,
+        registry="quay.io",
         key=(),
         all_modules=False,
         print_results=True,
         show_passed=False,
         sort_by="test",
         local=False,
         fix_version=False,
@@ -223,19 +235,19 @@
 
         # If it is a pipeline, load the lint config file and the modules.json file
         if self.repo_type == "pipeline":
             self.set_up_pipeline_files()
 
         # Lint local modules
         if local and len(local_modules) > 0:
-            self.lint_modules(local_modules, local=True, fix_version=fix_version)
+            self.lint_modules(local_modules, registry=registry, local=True, fix_version=fix_version)
 
         # Lint nf-core modules
         if len(remote_modules) > 0:
-            self.lint_modules(remote_modules, local=False, fix_version=fix_version)
+            self.lint_modules(remote_modules, registry=registry, local=False, fix_version=fix_version)
 
         if print_results:
             self._print_results(show_passed=show_passed, sort_by=sort_by)
             self.print_summary()
 
     def set_up_pipeline_files(self):
         self.load_lint_config()
@@ -260,20 +272,21 @@
                     "', '".join(bad_keys),
                 )
             )
 
         # If -k supplied, only run these tests
         self.lint_tests = [k for k in self.lint_tests if k in key]
 
-    def lint_modules(self, modules, local=False, fix_version=False):
+    def lint_modules(self, modules, registry="quay.io", local=False, fix_version=False):
         """
         Lint a list of modules
 
         Args:
             modules ([NFCoreModule]): A list of module objects
+            registry (str): The container registry to use. Should be quay.io in most situations.
             local (boolean): Whether the list consist of local or nf-core modules
             fix_version (boolean): Fix the module version if a newer version is available
         """
         progress_bar = rich.progress.Progress(
             "[bold blue]{task.description}",
             rich.progress.BarColumn(bar_width=None),
             "[magenta]{task.completed} of {task.total}[reset] » [bold yellow]{task.fields[test_name]}",
@@ -286,17 +299,17 @@
                 f"Linting {'local' if local else 'nf-core'} modules",
                 total=len(modules),
                 test_name=modules[0].module_name,
             )
 
             for mod in modules:
                 progress_bar.update(lint_progress, advance=1, test_name=mod.module_name)
-                self.lint_module(mod, progress_bar, local=local, fix_version=fix_version)
+                self.lint_module(mod, progress_bar, registry=registry, local=local, fix_version=fix_version)
 
-    def lint_module(self, mod, progress_bar, local=False, fix_version=False):
+    def lint_module(self, mod, progress_bar, registry, local=False, fix_version=False):
         """
         Perform linting on one module
 
         If the module is a local module we only check the `main.nf` file,
         and issue warnings instead of failures.
 
         If the module is a nf-core module we check for existence of the files
@@ -307,27 +320,27 @@
         If the linting is run for modules in the central nf-core/modules repo
         (repo_type==modules), files that are relevant for module testing are
         also examined
         """
 
         # Only check the main script in case of a local module
         if local:
-            self.main_nf(mod, fix_version, progress_bar)
+            self.main_nf(mod, fix_version, self.registry, progress_bar)
             self.passed += [LintResult(mod, *m) for m in mod.passed]
             warned = [LintResult(mod, *m) for m in (mod.warned + mod.failed)]
             if not self.fail_warned:
                 self.warned += warned
             else:
                 self.failed += warned
 
         # Otherwise run all the lint tests
         else:
             for test_name in self.lint_tests:
                 if test_name == "main_nf":
-                    getattr(self, test_name)(mod, fix_version, progress_bar)
+                    getattr(self, test_name)(mod, fix_version, self.registry, progress_bar)
                 else:
                     getattr(self, test_name)(mod)
 
             self.passed += [LintResult(mod, *m) for m in mod.passed]
             warned = [LintResult(mod, *m) for m in mod.warned]
             if not self.fail_warned:
                 self.warned += warned
```

### Comparing `nf-core-2.8/nf_core/modules/lint/main_nf.py` & `nf-core-2.9/nf_core/modules/lint/main_nf.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import nf_core
 import nf_core.modules.modules_utils
 from nf_core.modules.modules_differ import ModulesDiffer
 
 log = logging.getLogger(__name__)
 
 
-def main_nf(module_lint_object, module, fix_version, progress_bar):
+def main_nf(module_lint_object, module, fix_version, registry, progress_bar):
     """
     Lint a ``main.nf`` module file
 
     Can also be used to lint local module files,
     in which case failures will be reported as
     warnings.
 
@@ -117,15 +117,15 @@
     # Check that we have required sections
     if not len(outputs):
         module.failed.append(("main_nf_script_outputs", "No process 'output' block found", module.main_nf))
     else:
         module.passed.append(("main_nf_script_outputs", "Process 'output' block found", module.main_nf))
 
     # Check the process definitions
-    if check_process_section(module, process_lines, fix_version, progress_bar):
+    if check_process_section(module, process_lines, registry, fix_version, progress_bar):
         module.passed.append(("main_nf_container", "Container versions match", module.main_nf))
     else:
         module.warned.append(("main_nf_container", "Container versions do not match", module.main_nf))
 
     # Check the when statement
     check_when_section(module, when_lines)
 
@@ -205,30 +205,38 @@
     # Check the condition hasn't been changed.
     if lines[0].strip() != "task.ext.when == null || task.ext.when":
         self.failed.append(("when_condition", "when: condition has been altered", self.main_nf))
         return
     self.passed.append(("when_condition", "when: condition is unchanged", self.main_nf))
 
 
-def check_process_section(self, lines, fix_version, progress_bar):
-    """
-    Lint the section of a module between the process definition
+def check_process_section(self, lines, registry, fix_version, progress_bar):
+    """Lint the section of a module between the process definition
     and the 'input:' definition
     Specifically checks for correct software versions
     and containers
+
+    Args:
+        lines (List[str]): Content of process.
+        registry (str): Base Docker registry for containers. Typically quay.io.
+        fix_version (bool): Fix software version
+        progress_bar (ProgressBar): Progress bar to update.
+
+    Returns:
+        Optional[bool]: True if singularity and docker containers match, False otherwise. If process definition does not exist, None.
     """
     # Check that we have a process section
     if len(lines) == 0:
         self.failed.append(("process_exist", "Process definition does not exist", self.main_nf))
         return
     self.passed.append(("process_exist", "Process definition exists", self.main_nf))
 
     # Checks that build numbers of bioconda, singularity and docker container are matching
-    singularity_tag = "singularity"
-    docker_tag = "docker"
+    singularity_tag = None
+    docker_tag = None
     bioconda_packages = []
 
     # Process name should be all capital letters
     self.process_name = lines[0].split()[1]
     if all(x.upper() for x in self.process_name):
         self.passed.append(("process_capitals", "Process name is in capital letters", self.main_nf))
     else:
@@ -236,15 +244,20 @@
 
     # Check that process labels are correct
     check_process_labels(self, lines)
 
     # Deprecated enable_conda
     for i, l in enumerate(lines):
         url = None
-        l = l.strip(" '\"")
+        l = l.strip(" \n'\"}:")
+
+        # Catch preceeding "container "
+        if l.startswith("container"):
+            l = l.replace("container", "").strip(" \n'\"}:")
+
         if _container_type(l) == "conda":
             bioconda_packages = [b for b in l.split() if "bioconda::" in b]
             match = re.search(r"params\.enable_conda", l)
             if match is None:
                 self.passed.append(
                     (
                         "deprecated_enable_conda",
@@ -257,60 +270,75 @@
                     (
                         "deprecated_enable_conda",
                         f"Found deprecated parameter 'params.enable_conda' in the conda definition",
                         self.main_nf,
                     )
                 )
         if _container_type(l) == "singularity":
-            # e.g. "https://containers.biocontainers.pro/s3/SingImgsRepo/biocontainers/v1.2.0_cv1/biocontainers_v1.2.0_cv1.img' :" -> v1.2.0_cv1
-            # e.g. "https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0' :" -> 0.11.9--0
-            match = re.search(r"(?:/)?(?:biocontainers_)?(?::)?([A-Za-z\d\-_.]+?)(?:\.img)?'", l)
+            # e.g. "https://containers.biocontainers.pro/s3/SingImgsRepo/biocontainers/v1.2.0_cv1/biocontainers_v1.2.0_cv1.img -> v1.2.0_cv1
+            # e.g. "https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0 -> 0.11.9--0
+            # Please god let's find a better way to do this than regex
+            match = re.search(r"(?:[:.])?([A-Za-z\d\-_.]+?)(?:\.img)?(?:\.sif)?$", l)
             if match is not None:
                 singularity_tag = match.group(1)
                 self.passed.append(("singularity_tag", f"Found singularity tag: {singularity_tag}", self.main_nf))
             else:
                 self.failed.append(("singularity_tag", "Unable to parse singularity tag", self.main_nf))
                 singularity_tag = None
             url = urlparse(l.split("'")[0])
-            # lint double quotes
-            if l.count('"') > 2:
-                self.failed.append(
-                    (
-                        "container_links",
-                        "Too many double quotes found when specifying singularity container",
-                        self.main_nf,
-                    )
-                )
+
         if _container_type(l) == "docker":
-            # e.g. "quay.io/biocontainers/krona:2.7.1--pl526_5' }" -> 2.7.1--pl526_5
-            # e.g. "biocontainers/biocontainers:v1.2.0_cv1' }" -> v1.2.0_cv1
-            match = re.search(r"(?:[/])?(?::)?([A-Za-z\d\-_.]+)'", l)
+            # e.g. "quay.io/biocontainers/krona:2.7.1--pl526_5 -> 2.7.1--pl526_5
+            # e.g. "biocontainers/biocontainers:v1.2.0_cv1 -> v1.2.0_cv1
+            match = re.search(r":([A-Za-z\d\-_.]+)$", l)
             if match is not None:
                 docker_tag = match.group(1)
                 self.passed.append(("docker_tag", f"Found docker tag: {docker_tag}", self.main_nf))
             else:
                 self.failed.append(("docker_tag", "Unable to parse docker tag", self.main_nf))
                 docker_tag = None
-            if l.startswith("biocontainers/"):
-                # When we think it is a biocontainer, assume we are querying quay.io/biocontainers and insert quay.io as prefix
-                l = "quay.io/" + l
-            url = urlparse(l.split("'")[0])
-            # lint double quotes
-            if l.count('"') > 2:
+            if l.startswith(registry):
+                l_stripped = re.sub(r"\W+$", "", l)
                 self.failed.append(
-                    ("container_links", "Too many double quotes found when specifying docker container", self.main_nf)
+                    (
+                        "container_links",
+                        f"{l_stripped} container name found, please use just 'organisation/container:tag' instead.",
+                        self.main_nf,
+                    )
                 )
+            else:
+                self.passed.append(("container_links", f"Container prefix is correct", self.main_nf))
+
+            # Guess if container name is simple one (e.g. nfcore/ubuntu:20.04)
+            # If so, add quay.io as default container prefix
+            if l.count("/") == 1 and l.count(":") == 1:
+                l = "/".join([registry, l]).replace("//", "/")
+            url = urlparse(l.split("'")[0])
+
         # lint double quotes
-        if l.startswith("container"):
+        if l.startswith("container") or _container_type(l) == "docker" or _container_type(l) == "singularity":
             if l.count('"') > 2:
                 self.failed.append(
-                    ("container_links", "Too many double quotes found when specifying containers", self.main_nf)
+                    (
+                        "container_links",
+                        f"Too many double quotes found when specifying container: {l.lstrip('container ')}",
+                        self.main_nf,
+                    )
                 )
+            else:
+                self.passed.append(
+                    (
+                        "container_links",
+                        f"Correct number of double quotes found when specifying container: {l.lstrip('container ')}",
+                        self.main_nf,
+                    )
+                )
+
         # lint more than one container in the same line
-        if ("https://containers" in l or "https://depot" in l) and ("biocontainers/" in l or "quay.io/" in l):
+        if ("https://containers" in l or "https://depot" in l) and ("biocontainers/" in l or l.startswith(registry)):
             self.warned.append(
                 (
                     "container_links",
                     "Docker and Singularity containers specified in the same line. Only first one checked.",
                     self.main_nf,
                 )
             )
@@ -327,16 +355,22 @@
                 f"Connected to URL: {'https://' + urlunparse(url) if not url.scheme == 'https' else urlunparse(url)}, "
                 f"status_code: {response.status_code}"
             )
         except (requests.exceptions.RequestException, sqlite3.InterfaceError) as e:
             log.debug(f"Unable to connect to url '{urlunparse(url)}' due to error: {e}")
             self.failed.append(("container_links", "Unable to connect to container URL", self.main_nf))
             continue
-        if response.status_code != 200:
-            self.failed.append(("container_links", "Unable to connect to container URL", self.main_nf))
+        if not response.ok:
+            self.failed.append(
+                (
+                    "container_links",
+                    f"Unable to connect to {response.url}, status code: {response.status_code}",
+                    self.main_nf,
+                )
+            )
 
     # Check that all bioconda packages have build numbers
     # Also check for newer versions
     for bp in bioconda_packages:
         bp = bp.strip("'").strip('"')
         # Check for correct version and newer versions
         try:
@@ -388,15 +422,19 @@
                 else:
                     self.warned.append(
                         ("bioconda_latest", f"Conda update: {package} `{ver}` -> `{last_ver}`", self.main_nf)
                     )
             else:
                 self.passed.append(("bioconda_latest", f"Conda package is the latest available: `{bp}`", self.main_nf))
 
-    return docker_tag == singularity_tag
+    # Check if a tag exists at all. If not, return None.
+    if singularity_tag is None or docker_tag is None:
+        return None
+    else:
+        return docker_tag == singularity_tag
 
 
 def check_process_labels(self, lines):
     correct_process_labels = ["process_single", "process_low", "process_medium", "process_high", "process_long"]
     all_labels = [l.strip() for l in lines if l.lstrip().startswith("label ")]
     bad_labels = []
     good_labels = []
@@ -567,23 +605,19 @@
     return sorted(build_times, key=lambda tup: tup[0], reverse=True)[0][1]
 
 
 def _container_type(line):
     """Returns the container type of a build."""
     if line.startswith("conda"):
         return "conda"
-    if line.startswith("https://containers") or line.startswith("https://depot"):
+    if line.startswith("https://") or line.startswith("https://depot"):
         # Look for a http download URL.
         # Thanks Stack Overflow for the regex: https://stackoverflow.com/a/3809435/713980
         url_regex = (
             r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)"
         )
         url_match = re.search(url_regex, line, re.S)
         if url_match:
             return "singularity"
         return None
-    if (
-        line.startswith("biocontainers/")
-        or line.startswith("quay.io/")
-        or (line.count("/") == 1 and line.count(":") == 1)
-    ):
+    if line.count("/") >= 1 and line.count(":") == 1 and line.count(" ") == 0 and "https://" not in line:
         return "docker"
```

### Comparing `nf-core-2.8/nf_core/modules/lint/meta_yml.py` & `nf-core-2.9/nf_core/modules/lint/meta_yml.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/lint/module_changes.py` & `nf-core-2.9/nf_core/modules/lint/module_changes.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/lint/module_deprecations.py` & `nf-core-2.9/nf_core/modules/lint/module_deprecations.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/lint/module_patch.py` & `nf-core-2.9/nf_core/modules/lint/module_patch.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/lint/module_tests.py` & `nf-core-2.9/nf_core/modules/lint/module_tests.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/lint/module_todos.py` & `nf-core-2.9/nf_core/modules/lint/module_todos.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/lint/module_version.py` & `nf-core-2.9/nf_core/modules/lint/module_version.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/modules_differ.py` & `nf-core-2.9/nf_core/modules/modules_differ.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/modules_json.py` & `nf-core-2.9/nf_core/modules/modules_json.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/modules_repo.py` & `nf-core-2.9/nf_core/synced_repo.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,32 +3,30 @@
 import os
 import shutil
 from pathlib import Path
 
 import git
 import rich
 import rich.progress
-from git.exc import GitCommandError, InvalidGitRepositoryError
+from git.exc import GitCommandError
 
-import nf_core.modules.modules_json
-import nf_core.modules.modules_utils
-from nf_core.utils import NFCORE_DIR, load_tools_config
+from nf_core.utils import load_tools_config
 
 log = logging.getLogger(__name__)
 
 # Constants for the nf-core/modules repo used throughout the module files
 NF_CORE_MODULES_NAME = "nf-core"
 NF_CORE_MODULES_REMOTE = "https://github.com/nf-core/modules.git"
 NF_CORE_MODULES_DEFAULT_BRANCH = "master"
 
 
 class RemoteProgressbar(git.RemoteProgress):
     """
     An object to create a progressbar for when doing an operation with the remote.
-    Note that an initialized rich Progress (progress bar) object must be past
+    Note that an initialized rich Progress (progress bar) object must be passed
     during initialization.
     """
 
     def __init__(self, progress_bar, repo_name, remote_url, operation):
         """
         Initializes the object and adds a task to the progressbar passed as 'progress_bar'
 
@@ -54,42 +52,35 @@
         if not self.progress_bar.tasks[self.tid].started:
             self.progress_bar.start_task(self.tid)
         self.progress_bar.update(
             self.tid, total=max_count, completed=cur_count, state=f"{cur_count / max_count * 100:.1f}%"
         )
 
 
-class ModulesRepo:
+class SyncedRepo:
     """
-    An object to store details about the repository being used for modules.
-
-    Used by the `nf-core modules` top-level command with -r and -b flags,
-    so that this can be used in the same way by all sub-commands.
-
-    We keep track of the pull-status of the different installed repos in
-    the static variable local_repo_status. This is so we don't need to
-    pull a remote several times in one command.
+    An object to store details about a locally cached code repository.
     """
 
     local_repo_statuses = {}
     no_pull_global = False
 
     @staticmethod
     def local_repo_synced(repo_name):
         """
         Checks whether a local repo has been cloned/pull in the current session
         """
-        return ModulesRepo.local_repo_statuses.get(repo_name, False)
+        return SyncedRepo.local_repo_statuses.get(repo_name, False)
 
     @staticmethod
     def update_local_repo_status(repo_name, up_to_date):
         """
         Updates the clone/pull status of a local repo
         """
-        ModulesRepo.local_repo_statuses[repo_name] = up_to_date
+        SyncedRepo.local_repo_statuses[repo_name] = up_to_date
 
     @staticmethod
     def get_remote_branches(remote_url):
         """
         Get all branches from a remote repository
 
         Args:
@@ -114,15 +105,15 @@
 
     def __init__(self, remote_url=None, branch=None, no_pull=False, hide_progress=False):
         """
         Initializes the object and clones the git repository if it is not already present
         """
 
         # This allows us to set this one time and then keep track of the user's choice
-        ModulesRepo.no_pull_global |= no_pull
+        SyncedRepo.no_pull_global |= no_pull
 
         # Check if the remote seems to be well formed
         if remote_url is None:
             remote_url = NF_CORE_MODULES_REMOTE
 
         self.remote_url = remote_url
 
@@ -162,85 +153,14 @@
         if sha:
             if not self.sha_exists_on_branch(sha):
                 log.error(f"Commit SHA '{sha}' doesn't exist in '{self.remote_url}'")
                 return False
 
         return True
 
-    def setup_local_repo(self, remote, branch, hide_progress=True):
-        """
-        Sets up the local git repository. If the repository has been cloned previously, it
-        returns a git.Repo object of that clone. Otherwise it tries to clone the repository from
-        the provided remote URL and returns a git.Repo of the new clone.
-
-        Args:
-            remote (str): git url of remote
-            branch (str): name of branch to use
-        Sets self.repo
-        """
-        self.local_repo_dir = os.path.join(NFCORE_DIR, self.fullname)
-        try:
-            if not os.path.exists(self.local_repo_dir):
-                try:
-                    pbar = rich.progress.Progress(
-                        "[bold blue]{task.description}",
-                        rich.progress.BarColumn(bar_width=None),
-                        "[bold yellow]{task.fields[state]}",
-                        transient=True,
-                        disable=hide_progress or os.environ.get("HIDE_PROGRESS", None) is not None,
-                    )
-                    with pbar:
-                        self.repo = git.Repo.clone_from(
-                            remote,
-                            self.local_repo_dir,
-                            progress=RemoteProgressbar(pbar, self.fullname, self.remote_url, "Cloning"),
-                        )
-                    ModulesRepo.update_local_repo_status(self.fullname, True)
-                except GitCommandError:
-                    raise LookupError(f"Failed to clone from the remote: `{remote}`")
-                # Verify that the requested branch exists by checking it out
-                self.setup_branch(branch)
-            else:
-                self.repo = git.Repo(self.local_repo_dir)
-
-                if ModulesRepo.no_pull_global:
-                    ModulesRepo.update_local_repo_status(self.fullname, True)
-                # If the repo is already cloned, fetch the latest changes from the remote
-                if not ModulesRepo.local_repo_synced(self.fullname):
-                    pbar = rich.progress.Progress(
-                        "[bold blue]{task.description}",
-                        rich.progress.BarColumn(bar_width=None),
-                        "[bold yellow]{task.fields[state]}",
-                        transient=True,
-                        disable=hide_progress or os.environ.get("HIDE_PROGRESS", None) is not None,
-                    )
-                    with pbar:
-                        self.repo.remotes.origin.fetch(
-                            progress=RemoteProgressbar(pbar, self.fullname, self.remote_url, "Pulling")
-                        )
-                    ModulesRepo.update_local_repo_status(self.fullname, True)
-
-                # Before verifying the branch, fetch the changes
-                # Verify that the requested branch exists by checking it out
-                self.setup_branch(branch)
-
-                # Now merge the changes
-                tracking_branch = self.repo.active_branch.tracking_branch()
-                if tracking_branch is None:
-                    raise LookupError(f"There is no remote tracking branch '{self.branch}' in '{self.remote_url}'")
-                self.repo.git.merge(tracking_branch.name)
-        except (GitCommandError, InvalidGitRepositoryError) as e:
-            log.error(f"[red]Could not set up local cache of modules repository:[/]\n{e}\n")
-            if rich.prompt.Confirm.ask(f"[violet]Delete local cache '{self.local_repo_dir}' and try again?"):
-                log.info(f"Removing '{self.local_repo_dir}'")
-                shutil.rmtree(self.local_repo_dir)
-                self.setup_local_repo(remote, branch, hide_progress)
-            else:
-                raise LookupError("Exiting due to error with local modules git repo")
-
     def setup_branch(self, branch):
         """
         Verify that we have a branch and otherwise use the default one.
         The branch is then checked out to verify that it exists in the repo.
 
         Args:
             branch (str): Name of branch
@@ -272,15 +192,15 @@
         try:
             self.checkout_branch()
         except GitCommandError:
             raise LookupError(f"Branch '{self.branch}' not found in '{self.remote_url}'")
 
     def verify_branch(self):
         """
-        Verifies the active branch conforms do the correct directory structure
+        Verifies the active branch conforms to the correct directory structure
         """
         dir_names = os.listdir(self.local_repo_dir)
         if "modules" not in dir_names:
             err_str = f"Repository '{self.remote_url}' ({self.branch}) does not contain the 'modules/' directory"
             if "software" in dir_names:
                 err_str += (
                     ".\nAs of nf-core/tools version 2.0, the 'software/' directory should be renamed to 'modules/'"
@@ -390,15 +310,15 @@
     def get_component_git_log(self, component_name, component_type, depth=None):
         """
         Fetches the commit history the of requested module/subworkflow since a given date. The default value is
         not arbitrary - it is the last time the structure of the nf-core/modules repository was had an
         update breaking backwards compatibility.
         Args:
             component_name (str): Name of module/subworkflow
-            modules_repo (ModulesRepo): A ModulesRepo object configured for the repository in question
+            modules_repo (SyncedRepo): A SyncedRepo object configured for the repository in question
 
         Returns:
             ( dict ): Iterator of commit SHAs and associated (truncated) message
         """
         self.checkout_branch()
         component_path = os.path.join(component_type, self.repo_path, component_name)
         commits_new = self.repo.iter_commits(max_count=depth, paths=component_path)
```

### Comparing `nf-core-2.8/nf_core/modules/modules_test.py` & `nf-core-2.9/nf_core/modules/modules_test.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/modules_utils.py` & `nf-core-2.9/nf_core/modules/modules_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/nfcore_module.py` & `nf-core-2.9/nf_core/modules/nfcore_module.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/patch.py` & `nf-core-2.9/nf_core/modules/patch.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/test_yml_builder.py` & `nf-core-2.9/nf_core/modules/test_yml_builder.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/modules/update.py` & `nf-core-2.9/nf_core/modules/update.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/.devcontainer/devcontainer.json` & `nf-core-2.9/nf_core/pipeline-template/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/CONTRIBUTING.md` & `nf-core-2.9/nf_core/pipeline-template/.github/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -120,8 +120,7 @@
 - Tools installed
   - nf-core
   - Nextflow
 
 Devcontainer specs:
 
 - [DevContainer config](.devcontainer/devcontainer.json)
-- [Dockerfile](.devcontainer/Dockerfile)
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.yml` & `nf-core-2.9/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,13 @@
         Your verbose log file `.nextflow.log` is often useful _(this is a hidden file in the directory where you launched the pipeline)_ as well as custom Nextflow configuration files.
 
   - type: textarea
     id: system
     attributes:
       label: System information
       description: |
-        * Nextflow version _(eg. 22.10.1)_
+        * Nextflow version _(eg. 23.04.0)_
         * Hardware _(eg. HPC, Desktop, Cloud)_
         * Executor _(eg. slurm, local, awsbatch)_
         * Container engine: _(e.g. Docker, Singularity, Conda, Podman, Shifter, Charliecloud, or Apptainer)_
         * OS _(eg. CentOS Linux, macOS, Linux Mint)_
         * Version of {{ name }} _(eg. 1.1, 1.5, 1.8.2)_
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md` & `nf-core-2.9/nf_core/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/workflows/awsfulltest.yml` & `nf-core-2.9/nf_core/pipeline-template/.github/workflows/awsfulltest.yml`

 * *Files 13% similar despite different names*

```diff
@@ -10,25 +10,30 @@
 jobs:
   run-tower:
     name: Run AWS full tests
     if: github.repository == '{{ name }}'
     runs-on: ubuntu-latest
     steps:
       - name: Launch workflow via tower
-        uses: seqeralabs/action-tower-launch@v1
+        uses: seqeralabs/action-tower-launch@v2
         # TODO nf-core: You can customise AWS full pipeline tests as required
         # Add full size test data (but still relatively small datasets for few samples)
         # on the `test_full.config` test runs with only one set of parameters {%- raw %}
         with:
           workspace_id: ${{ secrets.TOWER_WORKSPACE_ID }}
           access_token: ${{ secrets.TOWER_ACCESS_TOKEN }}
           compute_env: ${{ secrets.TOWER_COMPUTE_ENV }}
+          revision: ${{ github.sha }}
           workdir: s3://${{ secrets.AWS_S3_BUCKET }}{% endraw %}/work/{{ short_name }}/{% raw %}work-${{ github.sha }}{% endraw %}
           parameters: |
             {
+              "hook_url": "{% raw %}${{ secrets.MEGATESTS_ALERTS_SLACK_HOOK_URL }}{% endraw %}",
               "outdir": "s3://{% raw %}${{ secrets.AWS_S3_BUCKET }}{% endraw %}/{{ short_name }}/{% raw %}results-${{ github.sha }}{% endraw %}"
             }
-          profiles: test_full,aws_tower
+          profiles: test_full
+
       - uses: actions/upload-artifact@v3
         with:
           name: Tower debug log file
-          path: tower_action_*.log
+          path: |
+            tower_action_*.log
+            tower_action_*.json
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/workflows/awstest.yml` & `nf-core-2.9/nf_core/pipeline-template/.github/workflows/awstest.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,26 @@
   run-tower:
     name: Run AWS tests
     if: github.repository == '{{ name }}'
     runs-on: ubuntu-latest
     steps:
       # Launch workflow using Tower CLI tool action {%- raw %}
       - name: Launch workflow via tower
-        uses: seqeralabs/action-tower-launch@v1
+        uses: seqeralabs/action-tower-launch@v2
         with:
           workspace_id: ${{ secrets.TOWER_WORKSPACE_ID }}
           access_token: ${{ secrets.TOWER_ACCESS_TOKEN }}
           compute_env: ${{ secrets.TOWER_COMPUTE_ENV }}
+          revision: ${{ github.sha }}
           workdir: s3://${{ secrets.AWS_S3_BUCKET }}{% endraw %}/work/{{ short_name }}/{% raw %}work-${{ github.sha }}{% endraw %}
           parameters: |
             {
               "outdir": "s3://{% raw %}${{ secrets.AWS_S3_BUCKET }}{% endraw %}/{{ short_name }}/{% raw %}results-test-${{ github.sha }}{% endraw %}"
             }
-          profiles: test,aws_tower
+          profiles: test
+
       - uses: actions/upload-artifact@v3
         with:
           name: Tower debug log file
-          path: tower_action_*.log
+          path: |
+            tower_action_*.log
+            tower_action_*.json
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/workflows/branch.yml` & `nf-core-2.9/nf_core/pipeline-template/.github/workflows/branch.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/workflows/ci.yml` & `nf-core-2.9/nf_core/pipeline-template/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name: Run pipeline with test data
     # Only run on push if this is the nf-core dev branch (merged PRs)
     if: "{% raw %}${{{% endraw %} github.event_name != 'push' || (github.event_name == 'push' && github.repository == '{{ name }}') {% raw %}}}{% endraw %}"
     runs-on: ubuntu-latest
     strategy:
       matrix:
         NXF_VER:
-          - "22.10.1"
+          - "23.04.0"
           - "latest-everything"
     steps:
       - name: Check out pipeline code
         uses: actions/checkout@v3
 
       - name: Install Nextflow
         uses: nf-core/setup-nextflow@v1
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/workflows/clean-up.yml` & `nf-core-2.9/nf_core/pipeline-template/.github/workflows/clean-up.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/workflows/fix-linting.yml` & `nf-core-2.9/nf_core/pipeline-template/.github/workflows/fix-linting.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/workflows/linting.yml` & `nf-core-2.9/nf_core/pipeline-template/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/.github/workflows/linting_comment.yml` & `nf-core-2.9/nf_core/pipeline-template/.github/workflows/linting_comment.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/.gitpod.yml` & `nf-core-2.9/nf_core/pipeline-template/.gitpod.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 image: nfcore/gitpod:latest
+tasks:
+  - name: Update Nextflow and setup pre-commit
+    command: |
+      pre-commit install --install-hooks
+      nextflow self-update
 
 vscode:
   extensions: # based on nf-core.nf-core-extensionpack
     - codezombiech.gitignore # Language support for .gitignore files
     # - cssho.vscode-svgviewer                 # SVG viewer
     - esbenp.prettier-vscode # Markdown/CommonMark linting and style checking for Visual Studio Code
     - eamodio.gitlens # Quickly glimpse into whom, why, and when a line or code block was changed
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/CITATIONS.md` & `nf-core-2.9/nf_core/pipeline-template/CITATIONS.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 
 > Di Tommaso P, Chatzou M, Floden EW, Barja PP, Palumbo E, Notredame C. Nextflow enables reproducible computational workflows. Nat Biotechnol. 2017 Apr 11;35(4):316-319. doi: 10.1038/nbt.3820. PubMed PMID: 28398311.
 
 ## Pipeline tools
 
 - [FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/)
 
+  > Andrews, S. (2010). FastQC: A Quality Control Tool for High Throughput Sequence Data [Online]. Available online https://www.bioinformatics.babraham.ac.uk/projects/fastqc/.
+
 - [MultiQC](https://pubmed.ncbi.nlm.nih.gov/27312411/)
+
   > Ewels P, Magnusson M, Lundin S, Käller M. MultiQC: summarize analysis results for multiple tools and samples in a single report. Bioinformatics. 2016 Oct 1;32(19):3047-8. doi: 10.1093/bioinformatics/btw354. Epub 2016 Jun 16. PubMed PMID: 27312411; PubMed Central PMCID: PMC5039924.
 
 ## Software packaging/containerisation tools
 
 - [Anaconda](https://anaconda.com)
 
   > Anaconda Software Distribution. Computer software. Vers. 2-2.4.0. Anaconda, Nov. 2016. Web.
@@ -27,9 +30,12 @@
 
 - [BioContainers](https://pubmed.ncbi.nlm.nih.gov/28379341/)
 
   > da Veiga Leprevost F, Grüning B, Aflitos SA, Röst HL, Uszkoreit J, Barsnes H, Vaudel M, Moreno P, Gatto L, Weber J, Bai M, Jimenez RC, Sachsenberg T, Pfeuffer J, Alvarez RV, Griss J, Nesvizhskii AI, Perez-Riverol Y. BioContainers: an open-source and community-driven framework for software standardization. Bioinformatics. 2017 Aug 15;33(16):2580-2582. doi: 10.1093/bioinformatics/btx192. PubMed PMID: 28379341; PubMed Central PMCID: PMC5870671.
 
 - [Docker](https://dl.acm.org/doi/10.5555/2600239.2600241)
 
+  > Merkel, D. (2014). Docker: lightweight linux containers for consistent development and deployment. Linux Journal, 2014(239), 2. doi: 10.5555/2600239.2600241.
+
 - [Singularity](https://pubmed.ncbi.nlm.nih.gov/28494014/)
+
   > Kurtzer GM, Sochat V, Bauer MW. Singularity: Scientific containers for mobility of compute. PLoS One. 2017 May 11;12(5):e0177459. doi: 10.1371/journal.pone.0177459. eCollection 2017. PubMed PMID: 28494014; PubMed Central PMCID: PMC5426675.
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/CODE_OF_CONDUCT.md` & `nf-core-2.9/nf_core/pipeline-template/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/LICENSE` & `nf-core-2.9/nf_core/pipeline-template/LICENSE`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/README.md` & `nf-core-2.9/nf_core/pipeline-template/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 {% if gh_badges -%}
 [![GitHub Actions CI Status](https://github.com/{{ name }}/workflows/nf-core%20CI/badge.svg)](https://github.com/{{ name }}/actions?query=workflow%3A%22nf-core+CI%22)
 [![GitHub Actions Linting Status](https://github.com/{{ name }}/workflows/nf-core%20linting/badge.svg)](https://github.com/{{ name }}/actions?query=workflow%3A%22nf-core+linting%22){% endif -%}
 {% if branded -%}[![AWS CI](https://img.shields.io/badge/CI%20tests-full%20size-FF9900?labelColor=000000&logo=Amazon%20AWS)](https://nf-co.re/{{ short_name }}/results){% endif -%}
 {%- if github_badges -%}
 [![Cite with Zenodo](http://img.shields.io/badge/DOI-10.5281/zenodo.XXXXXXX-1073c8?labelColor=000000)](https://doi.org/10.5281/zenodo.XXXXXXX)
 
-[![Nextflow](https://img.shields.io/badge/nextflow%20DSL2-%E2%89%A522.10.1-23aa62.svg)](https://www.nextflow.io/)
+[![Nextflow](https://img.shields.io/badge/nextflow%20DSL2-%E2%89%A523.04.0-23aa62.svg)](https://www.nextflow.io/)
 [![run with conda](http://img.shields.io/badge/run%20with-conda-3EB049?labelColor=000000&logo=anaconda)](https://docs.conda.io/en/latest/)
 [![run with docker](https://img.shields.io/badge/run%20with-docker-0db7ed?labelColor=000000&logo=docker)](https://www.docker.com/)
 [![run with singularity](https://img.shields.io/badge/run%20with-singularity-1d355c.svg?labelColor=000000)](https://sylabs.io/docs/)
 [![Launch on Nextflow Tower](https://img.shields.io/badge/Launch%20%F0%9F%9A%80-Nextflow%20Tower-%234256e7)](https://tower.nf/launch?pipeline=https://github.com/{{ name }})
 
 {% endif -%}
 {%- if branded -%}[![Get help on Slack](http://img.shields.io/badge/slack-nf--core%20%23{{ short_name }}-4A154B?labelColor=000000&logo=slack)](https://nfcore.slack.com/channels/{{ short_name }}){% endif -%}
@@ -78,19 +78,19 @@
 > **Warning:**
 > Please provide pipeline parameters via the CLI or Nextflow `-params-file` option. Custom config files including those
 > provided by the `-c` Nextflow option can be used to provide any configuration _**except for parameters**_;
 > see [docs](https://nf-co.re/usage/configuration#custom-configuration-files).
 
 {% if branded -%}
 
-For more details, please refer to the [usage documentation](https://nf-co.re/{{ short_name }}/usage) and the [parameter documentation](https://nf-co.re/{{ short_name }}/parameters).
+For more details and further functionality, please refer to the [usage documentation](https://nf-co.re/{{ short_name }}/usage) and the [parameter documentation](https://nf-co.re/{{ short_name }}/parameters).
 
 ## Pipeline output
 
-To see the the results of a test run with a full size dataset refer to the [results](https://nf-co.re/{{ short_name }}/results) tab on the nf-core website pipeline page.
+To see the results of an example test run with a full size dataset refer to the [results](https://nf-co.re/{{ short_name }}/results) tab on the nf-core website pipeline page.
 For more details about the output files and reports, please refer to the
 [output documentation](https://nf-co.re/{{ short_name }}/output).
 
 {% endif -%}
 
 ## Credits
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/assets/adaptivecard.json` & `nf-core-2.9/nf_core/pipeline-template/assets/adaptivecard.json`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/assets/email_template.html` & `nf-core-2.9/nf_core/pipeline-template/assets/email_template.html`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/assets/email_template.txt` & `nf-core-2.9/nf_core/pipeline-template/assets/email_template.txt`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/assets/schema_input.json` & `nf-core-2.9/nf_core/pipeline-template/assets/schema_input.json`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/assets/sendmail_template.txt` & `nf-core-2.9/nf_core/pipeline-template/assets/sendmail_template.txt`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/assets/slackreport.json` & `nf-core-2.9/nf_core/pipeline-template/assets/slackreport.json`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {
     "attachments": [
         {
             "fallback": "Plain-text summary of the attachment.",
             "color": "<% if (success) { %>good<% } else { %>danger<%} %>",
-            "author_name": "sanger-tol/readmapping v${version} - ${runName}",
+            "author_name": "{{ name }} v${version} - ${runName}",
             "author_icon": "https://www.nextflow.io/docs/latest/_static/favicon.ico",
             "text": "<% if (success) { %>Pipeline completed successfully!<% } else { %>Pipeline completed with errors<% } %>",
             "fields": [
                 {
                     "title": "Command used to launch the workflow",
                     "value": "```${commandLine}```",
                     "short": false
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/bin/check_samplesheet.py` & `nf-core-2.9/nf_core/pipeline-template/bin/check_samplesheet.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/conf/base.config` & `nf-core-2.9/nf_core/pipeline-template/conf/base.config`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/conf/igenomes.config` & `nf-core-2.9/nf_core/pipeline-template/conf/igenomes.config`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/conf/modules.config` & `nf-core-2.9/nf_core/pipeline-template/conf/modules.config`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/conf/test.config` & `nf-core-2.9/nf_core/pipeline-template/conf/test.config`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/conf/test_full.config` & `nf-core-2.9/nf_core/pipeline-template/conf/test_full.config`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
     Use as follows:
         nextflow run {{ name }} -profile test_full,<docker/singularity> --outdir <OUTDIR>
 
 ----------------------------------------------------------------------------------------
 */
 
-cleanup = true
-
 params {
     config_profile_name        = 'Full test profile'
     config_profile_description = 'Full test dataset to check pipeline function'
 
     // Input data for full size test
     // TODO nf-core: Specify the paths to your full test data ( on nf-core/test-datasets or directly in repositories, e.g. SRA)
     // TODO nf-core: Give any required params for the test so that command line flags are not needed
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/docs/README.md` & `nf-core-2.9/nf_core/pipeline-template/docs/README.md`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_adapter.png` & `nf-core-2.9/nf_core/pipeline-template/docs/images/mqc_fastqc_adapter.png`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_counts.png` & `nf-core-2.9/nf_core/pipeline-template/docs/images/mqc_fastqc_counts.png`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_quality.png` & `nf-core-2.9/nf_core/pipeline-template/docs/images/mqc_fastqc_quality.png`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/docs/output.md` & `nf-core-2.9/nf_core/pipeline-template/docs/output.md`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/docs/usage.md` & `nf-core-2.9/nf_core/pipeline-template/docs/usage.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 An [example samplesheet](../assets/samplesheet.csv) has been provided with the pipeline.
 
 ## Running the pipeline
 
 The typical command for running the pipeline is as follows:
 
 ```bash
-nextflow run {{ name }} --input samplesheet.csv --outdir <OUTDIR> --genome GRCh37 -profile docker
+nextflow run {{ name }} --input ./samplesheet.csv --outdir ./results --genome GRCh37 -profile docker
 ```
 
 This will launch the pipeline with the `docker` configuration profile. See below for more information about profiles.
 
 Note that the pipeline will create the following files in your working directory:
 
 ```bash
@@ -76,27 +76,27 @@
 ```
 
 If you wish to repeatedly use the same parameters for multiple runs, rather than specifying each flag in the command, you can specify these in a params file.
 
 Pipeline settings can be provided in a `yaml` or `json` file via `-params-file <file>`.
 
 > ⚠️ Do not use `-c <file>` to specify parameters as this will result in errors. Custom config files specified with `-c` must only be used for [tuning process resource specifications](https://nf-co.re/docs/usage/configuration#tuning-workflow-resources), other infrastructural tweaks (such as output directories), or module arguments (args).
-> The above pipeline run specified with a params file in yaml format:
+
+The above pipeline run specified with a params file in yaml format:
 
 ```bash
 nextflow run {{ name }} -profile docker -params-file params.yaml
 ```
 
 with `params.yaml` containing:
 
 ```yaml
 input: './samplesheet.csv'
 outdir: './results/'
 genome: 'GRCh37'
-input: 'data'
 <...>
 ```
 
 You can also generate such `YAML`/`JSON` files via [nf-core/launch](https://nf-co.re/launch).
 
 ### Updating the pipeline
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/lib/NfcoreTemplate.groovy` & `nf-core-2.9/nf_core/pipeline-template/lib/NfcoreTemplate.groovy`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
         // Render the HTML template
         def hf            = new File("$projectDir/assets/email_template.html")
         def html_template = engine.createTemplate(hf).make(email_fields)
         def email_html    = html_template.toString()
 
         // Render the sendmail template
-        def max_multiqc_email_size = params.max_multiqc_email_size as nextflow.util.MemoryUnit
+        def max_multiqc_email_size = (params.containsKey('max_multiqc_email_size') ? params.max_multiqc_email_size : 0) as nextflow.util.MemoryUnit
         def smail_fields           = [ email: email_address, subject: subject, email_txt: email_txt, email_html: email_html, projectDir: "$projectDir", mqcFile: mqc_report, mqcMaxSize: max_multiqc_email_size.toBytes() ]
         def sf                     = new File("$projectDir/assets/sendmail_template.txt")
         def sendmail_template      = engine.createTemplate(sf).make(smail_fields)
         def sendmail_html          = sendmail_template.toString()
 
         // Send the HTML e-mail
         Map colors = logColours(params.monochrome_logs)
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/lib/Utils.groovy` & `nf-core-2.9/nf_core/pipeline-template/lib/Utils.groovy`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/lib/nfcore_external_java_deps.jar` & `nf-core-2.9/nf_core/pipeline-template/lib/nfcore_external_java_deps.jar`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/main.nf` & `nf-core-2.9/nf_core/pipeline-template/main.nf`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     {{ name }}
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     Github : https://github.com/{{ name }}
 {%- if branded %}
     Website: https://nf-co.re/{{ short_name }}
     Slack  : https://nfcore.slack.com/channels/{{ short_name }}
-{% endif -%}
+{%- endif %}
 ----------------------------------------------------------------------------------------
 */
 
 nextflow.enable.dsl = 2
 {% if igenomes %}
 /*
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -23,14 +23,30 @@
 {% endif %}
 /*
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     VALIDATE & PRINT PARAMETER SUMMARY
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 */
 
+include { validateParameters; paramsHelp } from 'plugin/nf-validation'
+
+// Print help message if needed
+if (params.help) {
+    def logo = NfcoreTemplate.logo(workflow, params.monochrome_logs)
+    def citation = '\n' + WorkflowMain.citation(workflow) + '\n'
+    def String command = "nextflow run ${workflow.manifest.name} --input samplesheet.csv --genome GRCh37 -profile docker"
+    log.info logo + paramsHelp(command) + citation + NfcoreTemplate.dashedLine(params.monochrome_logs)
+    System.exit(0)
+}
+
+// Validate input parameters
+if (params.validate_params) {
+    validateParameters()
+}
+
 WorkflowMain.initialise(workflow, params, log)
 
 /*
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     NAMED WORKFLOW FOR PIPELINE
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 */
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/modules/local/samplesheet_check.nf` & `nf-core-2.9/nf_core/pipeline-template/modules/local/samplesheet_check.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/main.nf` & `nf-core-2.9/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/main.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/meta.yml` & `nf-core-2.9/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/meta.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/dumpsoftwareversions.py` & `nf-core-2.9/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/dumpsoftwareversions.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/main.nf` & `nf-core-2.9/nf_core/pipeline-template/modules/nf-core/fastqc/main.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/meta.yml` & `nf-core-2.9/nf_core/pipeline-template/modules/nf-core/fastqc/meta.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/main.nf` & `nf-core-2.9/nf_core/pipeline-template/modules/nf-core/multiqc/main.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/meta.yml` & `nf-core-2.9/nf_core/pipeline-template/modules/nf-core/multiqc/meta.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/modules.json` & `nf-core-2.9/nf_core/pipeline-template/modules.json`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/nextflow.config` & `nf-core-2.9/nf_core/pipeline-template/nextflow.config`

 * *Files 8% similar despite different names*

```diff
@@ -9,59 +9,65 @@
 // Global default params, used in configs
 params {
 
     // TODO nf-core: Specify your pipeline's command line flags
     // Input options
     input                      = null
 
-{% if igenomes %}
+    {%- if igenomes %}
     // References
     genome                     = null
     igenomes_base              = 's3://ngi-igenomes/igenomes'
     igenomes_ignore            = false
-    {% endif -%}
+    {% else %}
+    fasta                      = null
+    {%- endif %}
 
     // MultiQC options
     multiqc_config             = null
     multiqc_title              = null
     multiqc_logo               = null
     max_multiqc_email_size     = '25.MB'
     multiqc_methods_description = null
 
     // Boilerplate options
     outdir                     = null
-    tracedir                   = "${params.outdir}/pipeline_info"
     publish_dir_mode           = 'copy'
     email                      = null
     email_on_fail              = null
     plaintext_email            = false
     monochrome_logs            = false
     hook_url                   = null
     help                       = false
     version                    = false
-    validate_params            = true
-    show_hidden_params         = false
-    schema_ignore_params       = 'genomes'
-{% if nf_core_configs %}
 
     // Config options
+    config_profile_name        = null
+    config_profile_description = null
+
+    {%- if nf_core_configs %}
     custom_config_version      = 'master'
     custom_config_base         = "https://raw.githubusercontent.com/nf-core/configs/${params.custom_config_version}"
-    config_profile_description = null
     config_profile_contact     = null
     config_profile_url         = null
-    config_profile_name        = null
+    {% endif %}
 
-{% endif %}
     // Max resource options
     // Defaults only, expecting to be overwritten
     max_memory                 = '128.GB'
     max_cpus                   = 16
     max_time                   = '240.h'
 
+    // Schema validation default options
+    validationFailUnrecognisedParams = false
+    validationLenientMode            = false
+    validationSchemaIgnoreParams     = 'genomes'
+    validationShowHiddenParams       = false
+    validate_params                  = true
+
 }
 
 // Load base.config by default for all pipelines
 includeConfig 'conf/base.config'
 
 {% if nf_core_configs -%}
 // Load nf-core custom profiles from different Institutions
@@ -74,21 +80,21 @@
 // Load {{ name }} custom profiles from different institutions.
 // Warning: Uncomment only if a pipeline-specific instititutional config already exists on nf-core/configs!
 // try {
 //   includeConfig "${params.custom_config_base}/pipeline/{{ short_name }}.config"
 // } catch (Exception e) {
 //   System.err.println("WARNING: Could not load nf-core/config/{{ short_name }} profiles: ${params.custom_config_base}/pipeline/{{ short_name }}.config")
 // }
-{% endif %}
+{% endif -%}
 
 profiles {
     debug {
         dumpHashes             = true
         process.beforeScript   = 'echo $HOSTNAME'
-        cleanup = false
+        cleanup                = false
     }
     conda {
         conda.enabled          = true
         docker.enabled         = false
         singularity.enabled    = false
         podman.enabled         = false
         shifter.enabled        = false
@@ -103,15 +109,14 @@
         podman.enabled         = false
         shifter.enabled        = false
         charliecloud.enabled   = false
         apptainer.enabled      = false
     }
     docker {
         docker.enabled         = true
-        docker.registry        = 'quay.io'
         docker.userEmulation   = true
         conda.enabled          = false
         singularity.enabled    = false
         podman.enabled         = false
         shifter.enabled        = false
         charliecloud.enabled   = false
         apptainer.enabled      = false
@@ -127,15 +132,14 @@
         podman.enabled         = false
         shifter.enabled        = false
         charliecloud.enabled   = false
         apptainer.enabled      = false
     }
     podman {
         podman.enabled         = true
-        podman.registry        = 'quay.io'
         conda.enabled          = false
         docker.enabled         = false
         singularity.enabled    = false
         shifter.enabled        = false
         charliecloud.enabled   = false
         apptainer.enabled      = false
     }
@@ -171,22 +175,35 @@
         executor.cpus          = 16
         executor.memory        = 60.GB
     }
     test      { includeConfig 'conf/test.config'      }
     test_full { includeConfig 'conf/test_full.config' }
 }
 
-{% if igenomes %}
+// Set default registry for Apptainer, Docker, Podman and Singularity independent of -profile
+// Will not be used unless Apptainer / Docker / Podman / Singularity are enabled
+// Set to your registry if you have a mirror of containers
+apptainer.registry   = 'quay.io'
+docker.registry      = 'quay.io'
+podman.registry      = 'quay.io'
+singularity.registry = 'quay.io'
+
+// Nextflow plugins
+plugins {
+    id 'nf-validation' // Validation of pipeline parameters and creation of an input channel from a sample sheet
+}
+
+{% if igenomes -%}
 // Load igenomes.config if required
 if (!params.igenomes_ignore) {
     includeConfig 'conf/igenomes.config'
 } else {
     params.genomes = [:]
 }
-{% endif %}
+{% endif -%}
 
 // Export these variables to prevent local Python/R libraries from conflicting with those in the container
 // The JULIA depot path has been adjusted to a fixed path `/usr/local/share/julia` that needs to be used for packages in the container.
 // See https://apeltzer.github.io/post/03-julia-lang-nextflow/ for details on that. Once we have a common agreement on where to keep Julia packages, this is adjustable.
 
 env {
     PYTHONNOUSERSITE = 1
@@ -197,36 +214,36 @@
 
 // Capture exit codes from upstream processes when piping
 process.shell = ['/bin/bash', '-euo', 'pipefail']
 
 def trace_timestamp = new java.util.Date().format( 'yyyy-MM-dd_HH-mm-ss')
 timeline {
     enabled = true
-    file    = "${params.tracedir}/execution_timeline_${trace_timestamp}.html"
+    file    = "${params.outdir}/pipeline_info/execution_timeline_${trace_timestamp}.html"
 }
 report {
     enabled = true
-    file    = "${params.tracedir}/execution_report_${trace_timestamp}.html"
+    file    = "${params.outdir}/pipeline_info/execution_report_${trace_timestamp}.html"
 }
 trace {
     enabled = true
-    file    = "${params.tracedir}/execution_trace_${trace_timestamp}.txt"
+    file    = "${params.outdir}/pipeline_info/execution_trace_${trace_timestamp}.txt"
 }
 dag {
     enabled = true
-    file    = "${params.tracedir}/pipeline_dag_${trace_timestamp}.html"
+    file    = "${params.outdir}/pipeline_info/pipeline_dag_${trace_timestamp}.html"
 }
 
 manifest {
     name            = '{{ name }}'
     author          = """{{ author }}"""
     homePage        = 'https://github.com/{{ name }}'
     description     = """{{ description }}"""
     mainScript      = 'main.nf'
-    nextflowVersion = '!>=22.10.1'
+    nextflowVersion = '!>=23.04.0'
     version         = '{{ version }}'
     doi             = ''
 }
 
 // Load modules.config for DSL2 module specific options
 includeConfig 'conf/modules.config'
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/nextflow_schema.json` & `nf-core-2.9/nf_core/pipeline-template/nextflow_schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997726416955671%*

 * *Differences: {"'definitions'": "{'input_output_options': {'properties': {'input': {'exists': True, delete: "*

 * *                  "['schema']}}}, 'reference_genome_options': {'properties': {'fasta': {'exists': "*

 * *                  "True}}}, 'max_job_request_options': {'properties': {'max_time': {'pattern': "*

 * *                  "'^(\\\\d+\\\\.?\\\\s*(s|m|h|d|day)\\\\s*)+$'}}}, 'generic_options': "*

 * *                  "{'properties': {'help': {'default': False}, 'version': {'default': False}, "*

 * *                  "'plaintext_emai […]*

```diff
@@ -29,14 +29,15 @@
                     "fa_icon": "fas fa-exclamation-triangle",
                     "help_text": "An email address to send a summary email to when the pipeline is completed - ONLY sent if the pipeline does not exit successfully.",
                     "hidden": true,
                     "pattern": "^([a-zA-Z0-9_\\-\\.]+)@([a-zA-Z0-9_\\-\\.]+)\\.([a-zA-Z]{2,5})$",
                     "type": "string"
                 },
                 "help": {
+                    "default": false,
                     "description": "Display help text.",
                     "fa_icon": "fas fa-question-circle",
                     "hidden": true,
                     "type": "boolean"
                 },
                 "hook_url": {
                     "description": "Incoming hook URL for messaging service",
@@ -50,22 +51,24 @@
                     "description": "File size limit when attaching MultiQC reports to summary emails.",
                     "fa_icon": "fas fa-file-upload",
                     "hidden": true,
                     "pattern": "^\\d+(\\.\\d+)?\\.?\\s*(K|M|G|T)?B$",
                     "type": "string"
                 },
                 "monochrome_logs": {
+                    "default": false,
                     "description": "Do not use coloured log outputs.",
                     "fa_icon": "fas fa-palette",
                     "hidden": true,
                     "type": "boolean"
                 },
                 "multiqc_config": {
                     "description": "Custom config file to supply to MultiQC.",
                     "fa_icon": "fas fa-cog",
+                    "format": "file-path",
                     "hidden": true,
                     "type": "string"
                 },
                 "multiqc_logo": {
                     "description": "Custom logo file to supply to MultiQC. File name must also be set in the MultiQC config file",
                     "fa_icon": "fas fa-image",
                     "hidden": true,
@@ -73,14 +76,15 @@
                 },
                 "multiqc_methods_description": {
                     "description": "Custom MultiQC yaml file containing HTML including a methods description.",
                     "fa_icon": "fas fa-cog",
                     "type": "string"
                 },
                 "plaintext_email": {
+                    "default": false,
                     "description": "Send plain-text email instead of HTML.",
                     "fa_icon": "fas fa-remove-format",
                     "hidden": true,
                     "type": "boolean"
                 },
                 "publish_dir_mode": {
                     "default": "copy",
@@ -94,36 +98,47 @@
                         "move"
                     ],
                     "fa_icon": "fas fa-copy",
                     "help_text": "The Nextflow `publishDir` option specifies which intermediate files should be saved to the output directory. This option tells the pipeline what method should be used to move these files. See [Nextflow docs](https://www.nextflow.io/docs/latest/process.html#publishdir) for details.",
                     "hidden": true,
                     "type": "string"
                 },
-                "show_hidden_params": {
-                    "description": "Show all params when using `--help`",
-                    "fa_icon": "far fa-eye-slash",
-                    "help_text": "By default, parameters set as _hidden_ in the schema are not shown on the command line when a user runs with `--help`. Specifying this option will tell the pipeline to show all parameters.",
+                "validate_params": {
+                    "default": true,
+                    "description": "Boolean whether to validate parameters against the schema at runtime",
+                    "fa_icon": "fas fa-check-square",
                     "hidden": true,
                     "type": "boolean"
                 },
-                "tracedir": {
-                    "default": "${params.outdir}/pipeline_info",
-                    "description": "Directory to keep pipeline Nextflow logs and reports.",
-                    "fa_icon": "fas fa-cogs",
+                "validationFailUnrecognisedParams": {
+                    "default": false,
+                    "description": "Validation of parameters fails when an unrecognised parameter is found.",
+                    "fa_icon": "far fa-check-circle",
+                    "help_text": "By default, when an unrecognised parameter is found, it returns a warinig.",
                     "hidden": true,
-                    "type": "string"
+                    "type": "boolean"
                 },
-                "validate_params": {
-                    "default": true,
-                    "description": "Boolean whether to validate parameters against the schema at runtime",
-                    "fa_icon": "fas fa-check-square",
+                "validationLenientMode": {
+                    "default": false,
+                    "description": "Validation of parameters in lenient more.",
+                    "fa_icon": "far fa-check-circle",
+                    "help_text": "Allows string values that are parseable as numbers or booleans. For further information see [JSONSchema docs](https://github.com/everit-org/json-schema#lenient-mode).",
+                    "hidden": true,
+                    "type": "boolean"
+                },
+                "validationShowHiddenParams": {
+                    "default": false,
+                    "description": "Show all params when using `--help`",
+                    "fa_icon": "far fa-eye-slash",
+                    "help_text": "By default, parameters set as _hidden_ in the schema are not shown on the command line when a user runs with `--help`. Specifying this option will tell the pipeline to show all parameters.",
                     "hidden": true,
                     "type": "boolean"
                 },
                 "version": {
+                    "default": false,
                     "description": "Display version and exit.",
                     "fa_icon": "fas fa-question-circle",
                     "hidden": true,
                     "type": "boolean"
                 }
             },
             "title": "Generic options",
@@ -138,20 +153,20 @@
                     "fa_icon": "fas fa-envelope",
                     "help_text": "Set this parameter to your e-mail address to get a summary e-mail with details of the run sent to you when the workflow exits. If set in your user config file (`~/.nextflow/config`) then you don't need to specify this on the command line for every run.",
                     "pattern": "^([a-zA-Z0-9_\\-\\.]+)@([a-zA-Z0-9_\\-\\.]+)\\.([a-zA-Z]{2,5})$",
                     "type": "string"
                 },
                 "input": {
                     "description": "Path to comma-separated file containing information about the samples in the experiment.",
+                    "exists": true,
                     "fa_icon": "fas fa-file-csv",
                     "format": "file-path",
                     "help_text": "You will need to create a design file with information about the samples in your experiment before running the pipeline. Use this parameter to specify its location. It has to be a comma-separated file with 3 columns, and a header row.{% if branded %} See [usage docs](https://nf-co.re/{{ short_name }}/usage#samplesheet-input).{% endif %}",
                     "mimetype": "text/csv",
                     "pattern": "^\\S+\\.csv$",
-                    "schema": "assets/schema_input.json",
                     "type": "string"
                 },
                 "multiqc_title": {
                     "description": "MultiQC report title. Printed as page header, used for filename if not otherwise specified.",
                     "fa_icon": "fas fa-file-signature",
                     "type": "string"
                 },
@@ -241,27 +256,28 @@
                 },
                 "max_time": {
                     "default": "240.h",
                     "description": "Maximum amount of time that can be requested for any single job.",
                     "fa_icon": "far fa-clock",
                     "help_text": "Use to set an upper-limit for the time requirement for each process. Should be a string in the format integer-unit e.g. `--max_time '2.h'`",
                     "hidden": true,
-                    "pattern": "^(\\d+\\.?\\s*(s|m|h|day)\\s*)+$",
+                    "pattern": "^(\\d+\\.?\\s*(s|m|h|d|day)\\s*)+$",
                     "type": "string"
                 }
             },
             "title": "Max job request options",
             "type": "object"
         },
         "reference_genome_options": {
             "description": "Reference genome related files and options required for the workflow.",
             "fa_icon": "fas fa-dna",
             "properties": {
                 "fasta": {
                     "description": "Path to FASTA genome file.",
+                    "exists": true,
                     "fa_icon": "far fa-file-code",
                     "format": "file-path",
                     "help_text": "This parameter is *mandatory* if `--genome` is not specified. If you don't have a BWA index available this will be generated for you automatically. Combine with `--save_reference` to save BWA index for future runs.",
                     "mimetype": "text/plain",
                     "pattern": "^\\S+\\.fn?a(sta)?(\\.gz)?$",
                     "type": "string"
                 },
```

### Comparing `nf-core-2.8/nf_core/pipeline-template/subworkflows/local/input_check.nf` & `nf-core-2.9/nf_core/pipeline-template/subworkflows/local/input_check.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/pipeline-template/workflows/pipeline.nf` & `nf-core-2.9/nf_core/pipeline-template/workflows/pipeline.nf`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 /*
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-    VALIDATE INPUTS
+    PRINT PARAMS SUMMARY
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 */
 
-def summary_params = NfcoreSchema.paramsSummaryMap(workflow, params)
+include { paramsSummaryLog; paramsSummaryMap } from 'plugin/nf-validation'
 
-// Validate input parameters
-Workflow{{ short_name[0]|upper }}{{ short_name[1:] }}.initialise(params, log)
+def logo = NfcoreTemplate.logo(workflow, params.monochrome_logs)
+def citation = '\n' + WorkflowMain.citation(workflow) + '\n'
+def summary_params = paramsSummaryMap(workflow)
 
-// TODO nf-core: Add all file path parameters for the pipeline to the list below
-// Check input path parameters to see if they exist
-def checkPathParamList = [ params.input, params.multiqc_config, params.fasta ]
-for (param in checkPathParamList) { if (param) { file(param, checkIfExists: true) } }
+// Print parameter summary log to screen
+log.info logo + paramsSummaryLog(workflow) + citation
 
-// Check mandatory parameters
-if (params.input) { ch_input = file(params.input) } else { exit 1, 'Input samplesheet not specified!' }
+Workflow{{ short_name[0]|upper }}{{ short_name[1:] }}.initialise(params, log)
 
 /*
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     CONFIG FILES
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 */
 
@@ -65,17 +63,20 @@
 
     ch_versions = Channel.empty()
 
     //
     // SUBWORKFLOW: Read in samplesheet, validate and stage input files
     //
     INPUT_CHECK (
-        ch_input
+        file(params.input)
     )
     ch_versions = ch_versions.mix(INPUT_CHECK.out.versions)
+    // TODO: OPTIONAL, you can use nf-validation plugin to create an input channel from the samplesheet with Channel.fromSamplesheet("input")
+    // See the documentation https://nextflow-io.github.io/nf-validation/samplesheets/fromSamplesheet/
+    // ! There is currently no tooling to help you write a sample sheet schema
 
     //
     // MODULE: Run FastQC
     //
     FASTQC (
         INPUT_CHECK.out.reads
     )
@@ -87,15 +88,15 @@
 
     //
     // MODULE: MultiQC
     //
     workflow_summary    = Workflow{{ short_name[0]|upper }}{{ short_name[1:] }}.paramsSummaryMultiqc(workflow, summary_params)
     ch_workflow_summary = Channel.value(workflow_summary)
 
-    methods_description    = Workflow{{ short_name[0]|upper }}{{ short_name[1:] }}.methodsDescriptionText(workflow, ch_multiqc_custom_methods_description)
+    methods_description    = Workflow{{ short_name[0]|upper }}{{ short_name[1:] }}.methodsDescriptionText(workflow, ch_multiqc_custom_methods_description, params)
     ch_methods_description = Channel.value(methods_description)
 
     ch_multiqc_files = Channel.empty()
     ch_multiqc_files = ch_multiqc_files.mix(ch_workflow_summary.collectFile(name: 'workflow_summary_mqc.yaml'))
     ch_multiqc_files = ch_multiqc_files.mix(ch_methods_description.collectFile(name: 'methods_description_mqc.yaml'))
     ch_multiqc_files = ch_multiqc_files.mix(CUSTOM_DUMPSOFTWAREVERSIONS.out.mqc_yml.collect())
     ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect{it[1]}.ifEmpty([]))
```

### Comparing `nf-core-2.8/nf_core/refgenie.py` & `nf-core-2.9/nf_core/refgenie.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         refgenie_genomes_config_file = Path(nxf_home) / "nf-core/refgenie_genomes.config"
     else:
         log.info("Could not determine path to 'refgenie_genomes.config' file.")
         return False
 
     # Save the updated genome config
     try:
-        with open(refgenie_genomes_config_file, "w") as fh:
+        with open(refgenie_genomes_config_file, "w+") as fh:
             fh.write(refgenie_genomes)
         log.info(f"Updated nf-core genomes config: {refgenie_genomes_config_file}")
     except FileNotFoundError:
         log.warning(f"Could not write to {refgenie_genomes_config_file}")
         return False
 
     # Add include statement to NXF_HOME/config
```

### Comparing `nf-core-2.8/nf_core/schema.py` & `nf-core-2.9/nf_core/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,23 +234,28 @@
                 schema_no_required.pop("required")
             for group_key, group in schema_no_required.get("definitions", {}).items():
                 if "required" in group:
                     schema_no_required["definitions"][group_key].pop("required")
             jsonschema.validate(self.schema_defaults, schema_no_required)
         except jsonschema.exceptions.ValidationError as e:
             raise AssertionError(f"Default parameters are invalid: {e.message}")
+        for param, default in self.schema_defaults.items():
+            if default in ("null", "", None, "None"):
+                log.warning(
+                    f"[yellow][!] Default parameter '{param}' is empty or null. It is advisable to remove the default from the schema"
+                )
         log.info("[green][✓] Default parameters match schema validation")
 
         # Make sure every default parameter exists in the nextflow.config and is of correct type
         if self.pipeline_params == {}:
             self.get_wf_params()
 
         # Collect parameters to ignore
-        if "schema_ignore_params" in self.pipeline_params:
-            params_ignore = self.pipeline_params.get("schema_ignore_params", "").strip("\"'").split(",")
+        if "validationSchemaIgnoreParams" in self.pipeline_params:
+            params_ignore = self.pipeline_params.get("validationSchemaIgnoreParams", "").strip("\"'").split(",")
         else:
             params_ignore = []
 
         # Go over group keys
         for group_key, group in schema_no_required.get("definitions", {}).items():
             group_properties = group.get("properties")
             for param in group_properties:
@@ -755,16 +760,16 @@
         return False
 
     def add_schema_found_configs(self):
         """
         Add anything that's found in the Nextflow params that's missing in the pipeline schema
         """
         params_added = []
-        params_ignore = self.pipeline_params.get("schema_ignore_params", "").strip("\"'").split(",")
-        params_ignore.append("schema_ignore_params")
+        params_ignore = self.pipeline_params.get("validationSchemaIgnoreParams", "").strip("\"'").split(",")
+        params_ignore.append("validationSchemaIgnoreParams")
         for p_key, p_val in self.pipeline_params.items():
             # Check if key is in schema parameters
             if p_key not in self.schema_params and p_key not in params_ignore:
                 if (
                     self.no_prompts
                     or self.schema_from_scratch
                     or Confirm.ask(
```

### Comparing `nf-core-2.8/nf_core/subworkflow-template/subworkflows/main.nf` & `nf-core-2.9/nf_core/subworkflow-template/subworkflows/main.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/subworkflow-template/subworkflows/meta.yml` & `nf-core-2.9/nf_core/subworkflow-template/subworkflows/meta.yml`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,26 @@
   - samtools/index
 ## TODO nf-core: List all of the variables used as input, including their types and descriptions
 input:
   - meta:
       type: map
       description: |
         Groovy Map containing sample information
-        e.g. [ id:'test' ]
+        e.g. `[ id:'test' ]`
   - bam:
       type: file
       description: BAM/CRAM/SAM file
       pattern: "*.{bam,cram,sam}"
 ## TODO nf-core: List all of the variables used as output, including their types and descriptions
 output:
   - meta:
       type: map
       description: |
         Groovy Map containing sample information
-        e.g. [ id:'test' ]
+        e.g. `[ id:'test' ]`
   - bam:
       type: file
       description: Sorted BAM/CRAM/SAM file
       pattern: "*.{bam,cram,sam}"
   - bai:
       type: file
       description: BAM/CRAM/SAM samtools index
```

### Comparing `nf-core-2.8/nf_core/subworkflow-template/tests/main.nf` & `nf-core-2.9/nf_core/subworkflow-template/tests/main.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/subworkflow-template/tests/test.yml` & `nf-core-2.9/nf_core/subworkflow-template/tests/test.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/subworkflows/install.py` & `nf-core-2.9/nf_core/subworkflows/install.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/subworkflows/subworkflows_test.py` & `nf-core-2.9/nf_core/subworkflows/subworkflows_test.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/subworkflows/test_yml_builder.py` & `nf-core-2.9/nf_core/subworkflows/test_yml_builder.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/subworkflows/update.py` & `nf-core-2.9/nf_core/subworkflows/update.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/sync.py` & `nf-core-2.9/nf_core/sync.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/nf_core/utils.py` & `nf-core-2.9/nf_core/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Common utility functions for the nf-core python package.
 """
+import concurrent.futures
 import datetime
 import errno
 import hashlib
 import io
 import json
 import logging
 import mimetypes
@@ -54,34 +55,46 @@
 NFCORE_CACHE_DIR = os.path.join(
     os.environ.get("XDG_CACHE_HOME", os.path.join(os.getenv("HOME"), ".cache")),
     "nfcore",
 )
 NFCORE_DIR = os.path.join(os.environ.get("XDG_CONFIG_HOME", os.path.join(os.getenv("HOME"), ".config")), "nfcore")
 
 
+def fetch_remote_version(source_url):
+    response = requests.get(source_url, timeout=3)
+    remote_version = re.sub(r"[^0-9\.]", "", response.text)
+    return remote_version
+
+
 def check_if_outdated(current_version=None, remote_version=None, source_url="https://nf-co.re/tools_version"):
     """
     Check if the current version of nf-core is outdated
     """
     # Exit immediately if disabled via ENV var
     if os.environ.get("NFCORE_NO_VERSION_CHECK", False):
-        return True
+        return (True, "", "")
     # Set and clean up the current version string
     if current_version is None:
         current_version = nf_core.__version__
     current_version = re.sub(r"[^0-9\.]", "", current_version)
     # Build the URL to check against
     source_url = os.environ.get("NFCORE_VERSION_URL", source_url)
     source_url = f"{source_url}?v={current_version}"
-    # Fetch and clean up the remote version
-    if remote_version is None:
-        response = requests.get(source_url, timeout=3)
-        remote_version = re.sub(r"[^0-9\.]", "", response.text)
-    # Check if we have an available update
-    is_outdated = Version(remote_version) > Version(current_version)
+    # check if we have a newer version without blocking the rest of the script
+    is_outdated = False
+    if remote_version is None:  # we set it manually for tests
+        try:
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                future = executor.submit(fetch_remote_version, source_url)
+                remote_version = future.result()
+        except Exception as e:
+            log.debug(f"Could not check for nf-core updates: {e}")
+    if remote_version is not None:
+        if Version(remote_version) > Version(current_version):
+            is_outdated = True
     return (is_outdated, current_version, remote_version)
 
 
 def rich_force_colors():
     """
     Check if any environment variables are set to force Rich to use coloured output
     """
@@ -241,15 +254,15 @@
     # Hash the hash
     if len(concat_hash) > 0:
         bighash = hashlib.sha256(concat_hash.encode("utf-8")).hexdigest()
         cache_fn = f"wf-config-cache-{bighash[:25]}.json"
 
     if cache_basedir and cache_fn:
         cache_path = os.path.join(cache_basedir, cache_fn)
-        if os.path.isfile(cache_path):
+        if os.path.isfile(cache_path) and cache_config is True:
             log.debug(f"Found a config cache, loading: {cache_path}")
             with open(cache_path, "r") as fh:
                 try:
                     config = json.load(fh)
                 except json.JSONDecodeError as e:
                     raise UserWarning(f"Unable to load JSON file '{cache_path}' due to error {e}")
             return config
@@ -257,15 +270,15 @@
 
     # Call `nextflow config`
     nfconfig_raw = nextflow_cmd(f"nextflow config -flat {wf_path}")
     for l in nfconfig_raw.splitlines():
         ul = l.decode("utf-8")
         try:
             k, v = ul.split(" = ", 1)
-            config[k] = v
+            config[k] = v.strip("'\"")
         except ValueError:
             log.debug(f"Couldn't find key=value config pair:\n  {ul}")
 
     # Scrape main.nf for additional parameter declarations
     # Values in this file are likely to be complex, so don't both trying to capture them. Just get the param name.
     try:
         main_nf = os.path.join(wf_path, "main.nf")
@@ -819,42 +832,73 @@
         else:
             return pipeline
 
     log.info("Available nf-core pipelines: '{}'".format("', '".join([w.name for w in wfs.remote_workflows])))
     raise AssertionError(f"Not able to find pipeline '{pipeline}'")
 
 
-def prompt_pipeline_release_branch(wf_releases, wf_branches):
+def prompt_pipeline_release_branch(wf_releases, wf_branches, multiple=False):
     """Prompt for pipeline release / branch
 
     Args:
         wf_releases (array): Array of repo releases as returned by the GitHub API
         wf_branches (array): Array of repo branches, as returned by the GitHub API
+        multiple (bool): Allow selection of multiple releases & branches (for Tower)
 
     Returns:
         choice (str): Selected release / branch name
     """
-    # Prompt user for release tag
+    # Prompt user for release tag, tag_set will contain all available.
     choices = []
+    tag_set = []
 
     # Releases
     if len(wf_releases) > 0:
         for tag in map(lambda release: release.get("tag_name"), wf_releases):
             tag_display = [("fg:ansiblue", f"{tag}  "), ("class:choice-default", "[release]")]
             choices.append(questionary.Choice(title=tag_display, value=tag))
+            tag_set.append(tag)
 
     # Branches
     for branch in wf_branches.keys():
         branch_display = [("fg:ansiyellow", f"{branch}  "), ("class:choice-default", "[branch]")]
         choices.append(questionary.Choice(title=branch_display, value=branch))
+        tag_set.append(branch)
 
     if len(choices) == 0:
         return False
 
-    return questionary.select("Select release / branch:", choices=choices, style=nfcore_question_style).unsafe_ask()
+    if multiple:
+        return (
+            questionary.checkbox("Select release / branch:", choices=choices, style=nfcore_question_style).unsafe_ask(),
+            tag_set,
+        )
+
+    else:
+        return (
+            questionary.select("Select release / branch:", choices=choices, style=nfcore_question_style).unsafe_ask(),
+            tag_set,
+        )
+
+
+class SingularityCacheFilePathValidator(questionary.Validator):
+    """
+    Validator for file path specified as --singularity-cache-index argument in nf-core download
+    """
+
+    def validate(self, value):
+        if len(value.text):
+            if os.path.isfile(value.text):
+                return True
+            else:
+                raise questionary.ValidationError(
+                    message="Invalid remote cache index file", cursor_position=len(value.text)
+                )
+        else:
+            return True
 
 
 def get_repo_releases_branches(pipeline, wfs):
     """Fetches details of a nf-core workflow to download.
 
     Args:
         pipeline (str): GitHub repo username/repo
```

### Comparing `nf-core-2.8/nf_core.egg-info/PKG-INFO` & `nf-core-2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: nf-core
-Version: 2.8
-Summary: Helper tools for use with nf-core Nextflow pipelines.
-Home-page: https://github.com/nf-core/tools
-Author: Phil Ewels
-Author-email: phil.ewels@scilifelab.se
-License: MIT
-Keywords: nf-core,nextflow,bioinformatics,workflow,pipeline,biology,sequencing,NGS,next generation sequencing
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ![nf-core/tools](docs/images/nfcore-tools_logo_light.png#gh-light-mode-only) ![nf-core/tools](docs/images/nfcore-tools_logo_dark.png#gh-dark-mode-only) <!-- omit in toc -->
 
 [![Python tests](https://github.com/nf-core/tools/workflows/Python%20tests/badge.svg?branch=master&event=push)](https://github.com/nf-core/tools/actions?query=workflow%3A%22Python+tests%22+branch%3Amaster)
 [![codecov](https://codecov.io/gh/nf-core/tools/branch/master/graph/badge.svg)](https://codecov.io/gh/nf-core/tools)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![code style: prettier](https://img.shields.io/badge/code%20style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -29,15 +16,15 @@
 
 ## Table of contents <!-- omit in toc -->
 
 - [`nf-core` tools installation](#installation)
 - [`nf-core` tools update](#update-tools)
 - [`nf-core list` - List available pipelines](#listing-pipelines)
 - [`nf-core launch` - Run a pipeline with interactive parameter prompts](#launch-a-pipeline)
-- [`nf-core download` - Download pipeline for offline use](#downloading-pipelines-for-offline-use)
+- [`nf-core download` - Download a pipeline for offline use](#downloading-pipelines-for-offline-use)
 - [`nf-core licences` - List software licences in a pipeline](#pipeline-software-licences)
 - [`nf-core create` - Create a new pipeline with the nf-core template](#creating-a-new-pipeline)
 - [`nf-core lint` - Check pipeline code against nf-core guidelines](#linting-a-workflow)
 - [`nf-core schema` - Work with pipeline schema files](#pipeline-schema)
 - [`nf-core bump-version` - Update nf-core pipeline version number](#bumping-a-pipeline-version-number)
 - [`nf-core sync` - Synchronise pipeline TEMPLATE branches](#sync-a-pipeline-with-the-template)
 - [`nf-core modules` - commands for dealing with DSL2 modules](#modules)
@@ -336,15 +323,15 @@
 If run without any arguments, the download tool will interactively prompt you for the required information.
 Each option has a flag, if all are supplied then it will run without any user input needed.
 
 <!-- RICH-CODEX
 working_dir: tmp
 -->
 
-![`nf-core download rnaseq -r 3.8 --outdir nf-core-rnaseq -x none -c none`](docs/images/nf-core-download.svg)
+![`nf-core download rnaseq -r 3.8 --outdir nf-core-rnaseq -x none -s none -d`](docs/images/nf-core-download.svg)
 
 Once downloaded, you will see something like the following file structure for the downloaded pipeline:
 
 <!-- RICH-CODEX
 working_dir: tmp
 -->
 
@@ -352,26 +339,28 @@
 
 You can run the pipeline by simply providing the directory path for the `workflow` folder to your `nextflow run` command:
 
 ```bash
 nextflow run /path/to/download/nf-core-rnaseq-dev/workflow/ --input mydata.csv --outdir results  # usual parameters here
 ```
 
-> Note that if you downloaded singularity images, you will need to use `-profile singularity` or have it enabled in your config file.
+> Note that if you downloaded Singularity container images, you will need to use `-profile singularity` or have it enabled in your config file.
 
 ### Downloaded nf-core configs
 
 The pipeline files are automatically updated (`params.custom_config_base` is set to `../configs`), so that the local copy of institutional configs are available when running the pipeline.
 So using `-profile <NAME>` should work if available within [nf-core/configs](https://github.com/nf-core/configs).
 
-### Downloading singularity containers
+> ⚠️ This option is not available when downloading a pipeline for use with [Nextflow Tower](#adapting-downloads-to-nextflow-tower) because the application manages all configurations separately.
+
+### Downloading Apptainer containers
 
-If you're using Singularity, the `nf-core download` command can also fetch the required Singularity container images for you.
-To do this, select `singularity` in the prompt or specify `--container singularity` in the command.
-Your archive / target output directory will then include three folders: `workflow`, `configs` and also `singularity-containers`.
+If you're using [Singularity](https://apptainer.org) (Apptainer), the `nf-core download` command can also fetch the required container images for you.
+To do this, select `singularity` in the prompt or specify `--container-system singularity` in the command.
+Your archive / target output directory will then also include a separate folder `singularity-containers`.
 
 The downloaded workflow files are again edited to add the following line to the end of the pipeline's `nextflow.config` file:
 
 ```nextflow
 singularity.cacheDir = "${projectDir}/../singularity-images/"
 ```
 
@@ -381,43 +370,50 @@
 #### Singularity cache directory
 
 We highly recommend setting the `$NXF_SINGULARITY_CACHEDIR` environment variable on your system, even if that is a different system to where you will be running Nextflow.
 
 If found, the tool will fetch the Singularity images to this directory first before copying to the target output archive / directory.
 Any images previously fetched will be found there and copied directly - this includes images that may be shared with other pipelines or previous pipeline version downloads or download attempts.
 
-If you are running the download on the same system where you will be running the pipeline (eg. a shared filesystem where Nextflow won't have an internet connection at a later date), you can choose to _only_ use the cache via a prompt or cli options `--singularity-cache-only` / `--singularity-cache-copy`.
+If you are running the download on the same system where you will be running the pipeline (eg. a shared filesystem where Nextflow won't have an internet connection at a later date), you can choose to _only_ use the cache via a prompt or cli options `--container-cache-utilisation amend`. This instructs `nf-core download` to fetch all Singularity images to the `$NXF_SINGULARITY_CACHEDIR` directory but does _not_ copy them to the workflow archive / directory. The workflow config file is _not_ edited. This means that when you later run the workflow, Nextflow will just use the cache folder directly.
 
-This instructs `nf-core download` to fetch all Singularity images to the `$NXF_SINGULARITY_CACHEDIR` directory but does _not_ copy them to the workflow archive / directory.
-The workflow config file is _not_ edited. This means that when you later run the workflow, Nextflow will just use the cache folder directly.
+If you are downloading a workflow for a different system, you can provide information about the contents of its image cache to `nf-core download`. To avoid unnecessary container image downloads, choose `--container-cache-utilisation remote` and provide a list of already available images as plain text file to `--container-cache-index my_list_of_remotely_available_images.txt`. To generate this list on the remote system, run `find $NXF_SINGULARITY_CACHEDIR -name "*.img" > my_list_of_remotely_available_images.txt`. The tool will then only download and copy images into your output directory, which are missing on the remote system.
 
 #### How the Singularity image downloads work
 
 The Singularity image download finds containers using two methods:
 
 1. It runs `nextflow config` on the downloaded workflow to look for a `process.container` statement for the whole pipeline.
    This is the typical method used for DSL1 pipelines.
 2. It scrapes any files it finds with a `.nf` file extension in the workflow `modules` directory for lines
    that look like `container = "xxx"`. This is the typical method for DSL2 pipelines, which have one container per process.
 
-Some DSL2 modules have container addresses for docker (eg. `biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity continaer (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
+Some DSL2 modules have container addresses for docker (eg. `biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity container (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
 Where both are found, the download URL is preferred.
 
 Once a full list of containers is found, they are processed in the following order:
 
-1. If the target image already exists, nothing is done (eg. with `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` specified)
-2. If found in `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` is _not_ specified, they are copied to the output directory
+1. If the target image already exists, nothing is done (eg. with `$NXF_SINGULARITY_CACHEDIR` and `--container-cache-utilisation amend` specified)
+2. If found in `$NXF_SINGULARITY_CACHEDIR` and `--container-cache-utilisation copy` is specified, they are copied to the output directory
 3. If they start with `http` they are downloaded directly within Python (default 4 at a time, you can customise this with `--parallel-downloads`)
-4. If they look like a Docker image name, they are fetched using a `singularity pull` command
-   - This requires Singularity to be installed on the system and is substantially slower
+4. If they look like a Docker image name, they are fetched using a `singularity pull` command. Choose the container libraries (registries) queried by providing one or multiple `--container-library` parameter(s). For example, if you call `nf-core download` with `-l quay.io -l ghcr.io -l docker.io`, every image will be pulled from `quay.io` unless an error is encountered. Subsequently, `ghcr.io` and then `docker.io` will be queried for any image that has failed before.
+   - This requires Singularity/Apptainer to be installed on the system and is substantially slower
 
-Note that compressing many GBs of binary files can be slow, so specifying `--compress none` is recommended when downloading Singularity images.
+Note that compressing many GBs of binary files can be slow, so specifying `--compress none` is recommended when downloading Singularity images that are copied to the output directory.
 
 If the download speeds are much slower than your internet connection is capable of, you can set `--parallel-downloads` to a large number to download loads of images at once.
 
+### Adapting downloads to Nextflow Tower
+
+[seqeralabs® Nextflow Tower](https://cloud.tower.nf/) provides a graphical user interface to oversee pipeline runs, gather statistics and configure compute resources. While pipelines added to _Tower_ are preferably hosted at a Git service, providing them as disconnected, self-reliant repositories is also possible for premises with restricted network access. Choosing the `--tower` flag will download the pipeline in an appropriate form.
+
+Subsequently, the `*.git` folder can be moved to it's final destination and linked with a pipeline in _Tower_ using the `file:/` prefix.
+
+> 💡 Also without access to Tower, pipelines downloaded with the `--tower` flag can be run: `nextflow run -r 2.5 file:/path/to/pipelinedownload.git`. Downloads in this format allow you to include multiple revisions of a pipeline in a single file, but require that the revision (e.g. `-r 2.5`) is always explicitly specified.
+
 ## Pipeline software licences
 
 Sometimes it's useful to see the software licences of the tools used in a pipeline.
 You can use the `licences` subcommand to fetch and print the software licence from each conda / PyPI package used in an nf-core pipeline.
 
 > ⚠️ This command does not currently work for newer DSL2 pipelines. This will hopefully be addressed [soon](https://github.com/nf-core/tools/issues/1155).
 
@@ -571,15 +567,15 @@
 <!-- RICH-CODEX
 working_dir: tmp
 before_command: 'echo "{input: myfiles.csv, outdir: results}" > nf-params.json'
 timeout: 10
 after_command: rm nf-params.json
 -->
 
-![`nf-core schema validate nf-core-rnaseq/workflow nf-params.json`](docs/images/nf-core-schema-validate.svg)
+![`nf-core schema validate nf-core-rnaseq/3_8 nf-params.json`](docs/images/nf-core-schema-validate.svg)
 
 The `pipeline` option can be a directory containing a pipeline, a path to a schema file or the name of an nf-core pipeline (which will be downloaded using `nextflow pull`).
 
 ### Build a pipeline schema
 
 Manually building JSONSchema documents is not trivial and can be very error prone.
 Instead, the `nf-core schema build` command collects your pipeline parameters and gives interactive prompts about any missing or unexpected params.
@@ -908,14 +904,15 @@
 The command will automatically look through parent directories for this file to set the root path, so that you can run the command in a subdirectory.
 It will start in the current working directory, or whatever is specified with `--dir <directory>`.
 
 The `nf-core modules create` command will prompt you with the relevant questions in order to create all of the necessary module files.
 
 <!-- RICH-CODEX
 working_dir: tmp
+timeout: 10
 before_command: git clone https://github.com/nf-core/modules.git && cd modules
 fake_command: nf-core modules create fastqc --author @nf-core-bot  --label process_low --meta --force
 -->
 
 ![`cd modules && nf-core modules create fastqc --author @nf-core-bot  --label process_low --meta --force`](docs/images/nf-core-modules-create.svg)
 
 ### Create a module test config file
@@ -945,14 +942,16 @@
 
 ![`nf-core modules lint multiqc`](docs/images/nf-core-modules-lint.svg)
 
 ### Run the tests for a module using pytest
 
 To run unit tests of a module that you have installed or the test created by the command [`nf-core modules create-test-yml`](#create-a-module-test-config-file), you can use `nf-core modules test` command. This command runs the tests specified in `modules/tests/software/<tool>/<subtool>/test.yml` file using [pytest](https://pytest-workflow.readthedocs.io/en/stable/).
 
+> This command uses the pytest argument `--git-aware` to avoid copying the whole `.git` directory and files ignored by `git`. This means that it will only include files listed by `git ls-files`. Remember to **commit your changes** after adding a new module to add the new files to your git index.
+
 You can specify the module name in the form TOOL/SUBTOOL in command line or provide it later by prompts.
 
 <!-- RICH-CODEX
 working_dir: tmp/modules
 timeout: 30
 extra_env:
   PROFILE: 'conda'
@@ -1178,20 +1177,19 @@
 set to either `pipeline` or `modules`.
 The command will automatically look through parent directories for this file to set the root path, so that you can run the command in a subdirectory.
 It will start in the current working directory, or whatever is specified with `--dir <directory>`.
 
 The `nf-core subworkflows create` command will prompt you with the relevant questions in order to create all of the necessary subworkflow files.
 
 <!-- RICH-CODEX
-working_dir: tmp
-before_command: git clone https://github.com/nf-core/modules.git && cd modules
+working_dir: tmp/modules
 fake_command: nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force
 -->
 
-![`cd modules && nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force`](docs/images/nf-core-subworkflows-create.svg)
+![`nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force`](docs/images/nf-core-subworkflows-create.svg)
 
 ### Create a subworkflow test config file
 
 All subworkflows on [nf-core/modules](https://github.com/nf-core/modules) have a strict requirement of being unit tested using minimal test data.
 To help developers build new subworkflows, the `nf-core subworkflows create-test-yml` command automates the creation of the yaml file required to document the output file `md5sum` and other information generated by the testing.
 After you have written a minimal Nextflow script to test your subworkflow in `/tests/subworkflow/<subworkflow_name>/main.nf`, this command will run the tests for you and create the `/tests/subworkflow/<tool>/<subtool>/test.yml` file.
 
@@ -1203,14 +1201,16 @@
 
 ![`nf-core subworkflows create-test-yml bam_stats_samtools --no-prompts --force`](docs/images/nf-core-subworkflows-create-test.svg)
 
 ### Run the tests for a subworkflow using pytest
 
 To run unit tests of a subworkflow that you have installed or the test created by the command [`nf-core subworkflow create-test-yml`](#create-a-subworkflow-test-config-file), you can use `nf-core subworkflows test` command. This command runs the tests specified in `tests/subworkflows/<subworkflow_name>/test.yml` file using [pytest](https://pytest-workflow.readthedocs.io/en/stable/).
 
+> This command uses the pytest argument `--git-aware` to avoid copying the whole `.git` directory and files ignored by `git`. This means that it will only include files listed by `git ls-files`. Remember to **commit your changes** after adding a new subworkflow to add the new files to your git index.
+
 You can specify the subworkflow name in the form TOOL/SUBTOOL in command line or provide it later by prompts.
 
 <!-- RICH-CODEX
 working_dir: tmp/modules
 timeout: 30
 extra_env:
   PROFILE: 'conda'
```

### Comparing `nf-core-2.8/nf_core.egg-info/SOURCES.txt` & `nf-core-2.9/nf_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 nf_core/launch.py
 nf_core/licences.py
 nf_core/lint_utils.py
 nf_core/list.py
 nf_core/refgenie.py
 nf_core/schema.py
 nf_core/sync.py
+nf_core/synced_repo.py
 nf_core/utils.py
 nf_core.egg-info/PKG-INFO
 nf_core.egg-info/SOURCES.txt
 nf_core.egg-info/dependency_links.txt
 nf_core.egg-info/entry_points.txt
 nf_core.egg-info/not-zip-safe
 nf_core.egg-info/requires.txt
@@ -137,15 +138,14 @@
 nf_core/pipeline-template/conf/test_full.config
 nf_core/pipeline-template/docs/README.md
 nf_core/pipeline-template/docs/output.md
 nf_core/pipeline-template/docs/usage.md
 nf_core/pipeline-template/docs/images/mqc_fastqc_adapter.png
 nf_core/pipeline-template/docs/images/mqc_fastqc_counts.png
 nf_core/pipeline-template/docs/images/mqc_fastqc_quality.png
-nf_core/pipeline-template/lib/NfcoreSchema.groovy
 nf_core/pipeline-template/lib/NfcoreTemplate.groovy
 nf_core/pipeline-template/lib/Utils.groovy
 nf_core/pipeline-template/lib/WorkflowMain.groovy
 nf_core/pipeline-template/lib/WorkflowPipeline.groovy
 nf_core/pipeline-template/lib/nfcore_external_java_deps.jar
 nf_core/pipeline-template/modules/local/samplesheet_check.nf
 nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/main.nf
```

### Comparing `nf-core-2.8/setup.py` & `nf-core-2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
-version = "2.8"
+version = "2.9"
 
 with open("README.md") as f:
     readme = f.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
```

### Comparing `nf-core-2.8/tests/lint/actions_awsfulltest.py` & `nf-core-2.9/tests/lint/actions_awsfulltest.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/lint/actions_awstest.py` & `nf-core-2.9/tests/lint/actions_awstest.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/lint/actions_ci.py` & `nf-core-2.9/tests/lint/actions_ci.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/lint/actions_schema_validation.py` & `nf-core-2.9/tests/lint/actions_schema_validation.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/lint/files_exist.py` & `nf-core-2.9/tests/lint/files_exist.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/lint/files_unchanged.py` & `nf-core-2.9/tests/lint/files_unchanged.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/lint/merge_markers.py` & `nf-core-2.9/tests/lint/merge_markers.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/lint/nextflow_config.py` & `nf-core-2.9/tests/lint/nextflow_config.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/lint/version_consistency.py` & `nf-core-2.9/tests/lint/version_consistency.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/bump_versions.py` & `nf-core-2.9/tests/modules/bump_versions.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/create.py` & `nf-core-2.9/tests/modules/create.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/create_test_yml.py` & `nf-core-2.9/tests/modules/create_test_yml.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/info.py` & `nf-core-2.9/tests/modules/info.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/install.py` & `nf-core-2.9/tests/modules/install.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/lint.py` & `nf-core-2.9/tests/modules/lint.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,14 +78,29 @@
     module_lint = nf_core.modules.ModuleLint(dir=self.pipeline_dir, remote_url=GITLAB_URL)
     module_lint.lint(print_results=False, all_modules=True)
     assert len(module_lint.failed) == 1
     assert len(module_lint.passed) > 0
     assert len(module_lint.warned) >= 0
 
 
+def test_modules_lint_registry(self):
+    """Test linting the samtools module and alternative registry"""
+    self.mods_install.install("samtools")
+    module_lint = nf_core.modules.ModuleLint(dir=self.pipeline_dir, registry="public.ecr.aws")
+    module_lint.lint(print_results=False, module="samtools")
+    assert len(module_lint.failed) == 0, f"Linting failed with {[x.__dict__ for x in module_lint.failed]}"
+    assert len(module_lint.passed) > 0
+    assert len(module_lint.warned) >= 0
+    module_lint = nf_core.modules.ModuleLint(dir=self.pipeline_dir)
+    module_lint.lint(print_results=False, module="samtools")
+    assert len(module_lint.failed) == 0, f"Linting failed with {[x.__dict__ for x in module_lint.failed]}"
+    assert len(module_lint.passed) > 0
+    assert len(module_lint.warned) >= 0
+
+
 def test_modules_lint_patched_modules(self):
     """
     Test creating a patch file and applying it to a new version of the the files
     """
     setup_patch(self.pipeline_dir, True)
 
     # Create a patch file
```

### Comparing `nf-core-2.8/tests/modules/list.py` & `nf-core-2.9/tests/modules/list.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/modules_json.py` & `nf-core-2.9/tests/modules/modules_json.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/modules_test.py` & `nf-core-2.9/tests/modules/modules_test.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/patch.py` & `nf-core-2.9/tests/modules/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Test the 'nf-core modules patch' command
 
 Uses a branch (patch-tester) in the GitLab nf-core/modules-test repo when
 testing if the update commands works correctly with patch files
 """
 
 ORG_SHA = "002623ccc88a3b0cb302c7d8f13792a95354d9f2"
-CORRECT_SHA = "0245a9277d51a47c8aa68d264d294cf45312fab8"
+CORRECT_SHA = "1dff30bfca2d98eb7ac7b09269a15e822451d99f"
 SUCCEED_SHA = "ba15c20c032c549d77c5773659f19c2927daf48e"
 FAIL_SHA = "67b642d4471c4005220a342cad3818d5ba2b5a73"
 BISMARK_ALIGN = "bismark/align"
 REPO_NAME = "nf-core-test"
 PATCH_BRANCH = "patch-tester"
 REPO_URL = "https://gitlab.com/nf-core/modules-test.git"
```

### Comparing `nf-core-2.8/tests/modules/remove.py` & `nf-core-2.9/tests/modules/remove.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/modules/update.py` & `nf-core-2.9/tests/modules/update.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/subworkflows/create.py` & `nf-core-2.9/tests/subworkflows/create.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/subworkflows/create_test_yml.py` & `nf-core-2.9/tests/subworkflows/create_test_yml.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/subworkflows/info.py` & `nf-core-2.9/tests/subworkflows/info.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/subworkflows/install.py` & `nf-core-2.9/tests/subworkflows/install.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/subworkflows/list.py` & `nf-core-2.9/tests/subworkflows/list.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/subworkflows/remove.py` & `nf-core-2.9/tests/subworkflows/remove.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/subworkflows/subworkflows_test.py` & `nf-core-2.9/tests/subworkflows/subworkflows_test.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/subworkflows/update.py` & `nf-core-2.9/tests/subworkflows/update.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_bump_version.py` & `nf-core-2.9/tests/test_bump_version.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_cli.py` & `nf-core-2.9/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 @mock.patch("nf_core.__main__.nf_core_cli")
 def test_header(mock_cli):
     """Just try to execute the header function"""
     nf_core.__main__.run_nf_core()
 
 
 @mock.patch("nf_core.__main__.nf_core_cli")
-@mock.patch("nf_core.utils.check_if_outdated", return_value=(True, None, "dummy_version"))
+@mock.patch("nf_core.__main__.check_if_outdated", return_value=(True, None, "dummy_version"))
 def test_header_outdated(mock_check_outdated, mock_nf_core_cli, capsys):
     """Check cli notifies the user when nf_core is outdated"""
     nf_core.__main__.run_nf_core()
     captured = capsys.readouterr()
     assert "There is a new version of nf-core/tools available! (dummy_version)" in captured.err
 
 
@@ -161,32 +161,40 @@
     def test_cli_download(self, mock_dl):
         """Test nf-core pipeline is downloaded and cli parameters are passed on."""
         params = {
             "revision": "abcdef",
             "outdir": "/path/outdir",
             "compress": "tar.gz",
             "force": None,
-            "container": "singularity",
-            "singularity-cache-only": None,
+            "tower": None,
+            "download-configuration": None,
+            "container-system": "singularity",
+            "container-library": "quay.io",
+            "container-cache-utilisation": "copy",
+            "container-cache-index": "/path/index.txt",
             "parallel-downloads": 2,
         }
 
         cmd = ["download"] + self.assemble_params(params) + ["pipeline_name"]
         result = self.invoke_cli(cmd)
 
         assert result.exit_code == 0
 
         mock_dl.assert_called_once_with(
             cmd[-1],
-            params["revision"],
+            (params["revision"],),
             params["outdir"],
             params["compress"],
             "force" in params,
-            params["container"],
-            "singularity-cache-only" in params,
+            "tower" in params,
+            "download-configuration" in params,
+            params["container-system"],
+            (params["container-library"],),
+            params["container-cache-utilisation"],
+            params["container-cache-index"],
             params["parallel-downloads"],
         )
 
         mock_dl.return_value.download_workflow.assert_called_once()
 
     @mock.patch("nf_core.licences.WorkflowLicences")
     def test_licences(self, mock_lic):
```

### Comparing `nf-core-2.8/tests/test_create.py` & `nf-core-2.9/tests/test_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import nf_core.create
 
 from .utils import with_temporary_folder
 
 TEST_DATA_DIR = Path(__file__).parent / "data"
 PIPELINE_TEMPLATE_YML = TEST_DATA_DIR / "pipeline_create_template.yml"
+PIPELINE_TEMPLATE_YML_SKIP = TEST_DATA_DIR / "pipeline_create_template_skip.yml"
 
 
 class NfcoreCreateTest(unittest.TestCase):
     def setUp(self):
         self.pipeline_name = "nf-core/test"
         self.pipeline_description = "just for 4w3s0m3 tests"
         self.pipeline_author = "Chuck Norris"
@@ -103,7 +104,35 @@
         assert f" {self.default_branch}\n" in git.Repo.init(pipeline.outdir).git.branch()
 
         # Check pipeline yml has been dumped and matches input
         pipeline_template = os.path.join(pipeline.outdir, "pipeline_template.yml")
         assert os.path.exists(pipeline_template)
         with open(pipeline_template) as fh:
             assert fh.read() == PIPELINE_TEMPLATE_YML.read_text()
+
+    @with_temporary_folder
+    def test_pipeline_creation_with_yml_skip(self, tmp_path):
+        pipeline = nf_core.create.PipelineCreate(
+            name=self.pipeline_name,
+            description=self.pipeline_description,
+            author=self.pipeline_author,
+            version=self.pipeline_version,
+            no_git=False,
+            force=True,
+            outdir=tmp_path,
+            template_yaml_path=PIPELINE_TEMPLATE_YML_SKIP,
+            plain=True,
+            default_branch=self.default_branch,
+        )
+        pipeline.init_pipeline()
+        assert not os.path.isdir(os.path.join(pipeline.outdir, ".git"))
+
+        # Check pipeline yml has been dumped and matches input
+        pipeline_template = os.path.join(pipeline.outdir, "pipeline_template.yml")
+        assert os.path.exists(pipeline_template)
+        with open(pipeline_template) as fh:
+            assert fh.read() == PIPELINE_TEMPLATE_YML_SKIP.read_text()
+
+        # Check that some of the skipped files are not present
+        assert not os.path.exists(os.path.join(pipeline.outdir, "CODE_OF_CONDUCT.md"))
+        assert not os.path.exists(os.path.join(pipeline.outdir, ".github"))
+        assert not os.path.exists(os.path.join(pipeline.outdir, "conf", "igenomes.config"))
```

### Comparing `nf-core-2.8/tests/test_launch.py` & `nf-core-2.9/tests/test_launch.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_licenses.py` & `nf-core-2.9/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_lint.py` & `nf-core-2.9/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_lint_utils.py` & `nf-core-2.9/tests/test_lint_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_list.py` & `nf-core-2.9/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_modules.py` & `nf-core-2.9/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_refgenie.py` & `nf-core-2.9/tests/test_refgenie.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_schema.py` & `nf-core-2.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_subworkflows.py` & `nf-core-2.9/tests/test_subworkflows.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_sync.py` & `nf-core-2.9/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_test_utils.py` & `nf-core-2.9/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/test_utils.py` & `nf-core-2.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.8/tests/utils.py` & `nf-core-2.9/tests/utils.py`

 * *Files identical despite different names*

