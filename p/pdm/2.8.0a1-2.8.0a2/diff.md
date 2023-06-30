# Comparing `tmp/pdm-2.8.0a1.tar.gz` & `tmp/pdm-2.8.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.8.0a1.tar", last modified: Tue Jun 27 07:57:26 2023, max compression
+gzip compressed data, was "pdm-2.8.0a2.tar", last modified: Fri Jun 30 01:46:07 2023, max compression
```

## Comparing `pdm-2.8.0a1.tar` & `pdm-2.8.0a2.tar`

### file list

```diff
@@ -1,280 +1,280 @@
--rw-r--r--   0        0        0   126343 2023-06-27 07:57:18.746300 pdm-2.8.0a1/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-06-27 07:57:18.746300 pdm-2.8.0a1/LICENSE
--rw-r--r--   0        0        0     1075 2023-06-27 07:57:18.746300 pdm-2.8.0a1/LICENSE
--rw-r--r--   0        0        0     7937 2023-06-27 07:57:18.746300 pdm-2.8.0a1/README.md
--rw-r--r--   0        0        0     7937 2023-06-27 07:57:18.746300 pdm-2.8.0a1/README.md
--rw-r--r--   0        0        0     4559 2023-06-27 07:57:26.526371 pdm-2.8.0a1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-27 07:57:18.750300 pdm-2.8.0a1/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-06-27 07:57:18.750300 pdm-2.8.0a1/src/pdm/__version__.py
--rw-r--r--   0        0        0     3282 2023-06-27 07:57:18.750300 pdm-2.8.0a1/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-06-27 07:57:18.750300 pdm-2.8.0a1/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11850 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    16131 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     7104 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2857 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     4236 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6542 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     7165 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     3066 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     3689 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0    10543 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3589 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15754 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2196 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6596 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     8112 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6782 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     4271 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15489 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9370 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     6898 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     6489 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1723 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2426 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6149 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      819 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1279 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2759 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5137 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    50498 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18629 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25397 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10461 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/options.py
--rw-r--r--   0        0        0     6235 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/__init__.py
--rw-r--r--   0        0        0     3102 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/.gitignore
--rw-r--r--   0        0        0       18 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/README.md
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/__init__.py
--rw-r--r--   0        0        0      278 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/src/example_package/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/tests/__init__.py
--rw-r--r--   0        0        0    25152 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2373 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/compat.py
--rw-r--r--   0        0        0    10667 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8850 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/environments/base.py
--rw-r--r--   0        0        0     4255 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/environments/local.py
--rw-r--r--   0        0        0     1600 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1362 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1202 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5788 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2614 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7490 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7502 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2309 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1390 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10901 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18161 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10990 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     3162 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4698 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/backends.py
--rw-r--r--   0        0        0    11710 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/caches.py
--rw-r--r--   0        0        0    26580 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1845 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6323 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2195 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    21340 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    18792 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/search.py
--rw-r--r--   0        0        0     3363 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     1300 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5924 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2766 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16757 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/config.py
--rw-r--r--   0        0        0    26292 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/core.py
--rw-r--r--   0        0        0     2093 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/py.typed
--rw-r--r--   0        0        0    20067 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13176 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/signals.py
--rw-r--r--   0        0        0     8054 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/termui.py
--rw-r--r--   0        0        0    14101 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/__init__.py
--rw-r--r--   0        0        0     3723 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/conftest.py
--rw-r--r--   0        0        0    12362 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_add.py
--rw-r--r--   0        0        0     5775 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_cache.py
--rw-r--r--   0        0        0     9286 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4950 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_list.py
--rw-r--r--   0        0        0     6324 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7796 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_others.py
--rw-r--r--   0        0        0     6052 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3888 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_remove.py
--rw-r--r--   0        0        0    29259 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     2778 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_template.py
--rw-r--r--   0        0        0     8876 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/cli/test_update.py
--rw-r--r--   0        0        0     2997 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/cli/test_use.py
--rw-r--r--   0        0        0    10808 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-06-27 07:57:18.766300 pdm-2.8.0a1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-06-27 07:57:18.766300 pdm-2.8.0a1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-06-27 07:57:18.766300 pdm-2.8.0a1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-06-27 07:57:18.766300 pdm-2.8.0a1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-06-27 07:57:18.770300 pdm-2.8.0a1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       13 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      572 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      726 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      344 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo/pyproject.toml
--rw-r--r--   0        0        0       26 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1330 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_backends.py
--rw-r--r--   0        0        0    13344 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2556 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7704 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_integration.py
--rw-r--r--   0        0        0     3435 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_plugin.py
--rw-r--r--   0        0        0    12085 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_signals.py
--rw-r--r--   0        0        0     4409 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_utils.py
--rw-r--r--   0        0        0     9838 1970-01-01 00:00:00.000000 pdm-2.8.0a1/PKG-INFO
+-rw-r--r--   0        0        0   126958 2023-06-30 01:45:58.402574 pdm-2.8.0a2/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-06-30 01:45:58.402574 pdm-2.8.0a2/LICENSE
+-rw-r--r--   0        0        0     1075 2023-06-30 01:45:58.402574 pdm-2.8.0a2/LICENSE
+-rw-r--r--   0        0        0     7937 2023-06-30 01:45:58.402574 pdm-2.8.0a2/README.md
+-rw-r--r--   0        0        0     7937 2023-06-30 01:45:58.402574 pdm-2.8.0a2/README.md
+-rw-r--r--   0        0        0     4559 2023-06-30 01:46:06.994550 pdm-2.8.0a2/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3282 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11850 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    16246 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     7104 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2857 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6542 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     7165 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     3066 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     3689 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0    10543 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3638 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15754 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2196 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8112 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6782 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     4284 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15489 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9370 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     7260 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     6489 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1723 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2426 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6149 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      819 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1279 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2759 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5137 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    50498 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18629 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25397 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10461 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/options.py
+-rw-r--r--   0        0        0     6539 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/__init__.py
+-rw-r--r--   0        0        0     3102 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/.gitignore
+-rw-r--r--   0        0        0       18 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/src/example_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/tests/__init__.py
+-rw-r--r--   0        0        0    25152 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2373 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/compat.py
+-rw-r--r--   0        0        0    10667 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8850 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     4255 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1362 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1202 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2614 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7490 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7502 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2309 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1367 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10901 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18219 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10990 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4698 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    12115 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26580 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1845 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6323 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2195 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    21340 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18792 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/search.py
+-rw-r--r--   0        0        0     3363 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2766 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    16757 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/config.py
+-rw-r--r--   0        0        0    27068 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2093 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/py.typed
+-rw-r--r--   0        0        0    20067 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     2001 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13176 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/termui.py
+-rw-r--r--   0        0        0    14101 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12362 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5795 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4950 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6324 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6052 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3888 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29259 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     2778 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_template.py
+-rw-r--r--   0        0        0     8876 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2997 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10808 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-06-30 01:45:58.422574 pdm-2.8.0a2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-06-30 01:45:58.426574 pdm-2.8.0a2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       13 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      572 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      726 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      344 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1330 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13344 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2556 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7704 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_plugin.py
+-rw-r--r--   0        0        0    12085 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_signals.py
+-rw-r--r--   0        0        0     4409 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_utils.py
+-rw-r--r--   0        0        0     9838 1970-01-01 00:00:00.000000 pdm-2.8.0a2/PKG-INFO
```

### Comparing `pdm-2.8.0a1/CHANGELOG.md` & `pdm-2.8.0a2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Release v2.8.0a2 (2023-06-30)
+-----------------------------
+
+### Bug Fixes
+
+- Fix a bug that dependencies can't be updated when the table is separated by another table. [#2056](https://github.com/pdm-project/pdm/issues/2056)
+- Fix a bug that `*_lock` hooks are always emitted with dry_run=True in `pdm update`. [#2060](https://github.com/pdm-project/pdm/issues/2060)
+- Fix a bug that `pdm install --plugins` can't install self. [#2062](https://github.com/pdm-project/pdm/issues/2062)
+- Fix a cache collision between named requirements and url requirements. [#2064](https://github.com/pdm-project/pdm/issues/2064)
+
+
 Release v2.8.0a1 (2023-06-27)
 -----------------------------
 
 ### Features & Improvements
 
 - Add support for `cookiecutter` and `copier` as project generator. [#2059](https://github.com/pdm-project/pdm/issues/2059)
```

### Comparing `pdm-2.8.0a1/LICENSE` & `pdm-2.8.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/README.md` & `pdm-2.8.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/pyproject.toml` & `pdm-2.8.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.8.0a1"
+version = "2.8.0a2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
```

### Comparing `pdm-2.8.0a1/src/pdm/_types.py` & `pdm-2.8.0a2/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/builders/base.py` & `pdm-2.8.0a2/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/builders/editable.py` & `pdm-2.8.0a2/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/builders/sdist.py` & `pdm-2.8.0a2/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/builders/wheel.py` & `pdm-2.8.0a2/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/actions.py` & `pdm-2.8.0a2/src/pdm/cli/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,50 +356,55 @@
 
 # Moved functions
 def do_add(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
     from pdm.cli.commands.add import Command as AddCommand
 
     deprecation_warning(
         "`pdm.actions.do_add` has been moved to `pdm.cli.commands.add:Command.do_add` method, "
-        "This function will be removed in the future."
+        "This function will be removed in the future.",
+        stacklevel=2,
     )
     AddCommand().do_add(*args, **kwargs)
 
 
 def do_update(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
     from pdm.cli.commands.update import Command as UpdateCommand
 
     deprecation_warning(
         "`pdm.actions.do_update` has been moved to `pdm.cli.commands.update:Command.do_update` method, "
-        "This function will be removed in the future."
+        "This function will be removed in the future.",
+        stacklevel=2,
     )
     UpdateCommand().do_update(*args, **kwargs)
 
 
 def do_use(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
     from pdm.cli.commands.use import Command as UseCommand
 
     deprecation_warning(
         "`pdm.actions.do_use` has been moved to `pdm.cli.commands.use:Command.do_use` method, "
-        "This function will be removed in the future."
+        "This function will be removed in the future.",
+        stacklevel=2,
     )
     UseCommand().do_use(*args, **kwargs)
 
 
 def do_remove(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
     from pdm.cli.commands.remove import Command as RemoveCommand
 
     deprecation_warning(
         "`pdm.actions.do_remove` has been moved to `pdm.cli.commands.remove:Command.do_remove` method, "
-        "This function will be removed in the future."
+        "This function will be removed in the future.",
+        stacklevel=2,
     )
     RemoveCommand().do_remove(*args, **kwargs)
 
 
 def do_import(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
     from pdm.cli.commands.import_cmd import Command as ImportCommand
 
     deprecation_warning(
         "`pdm.actions.do_import` has been moved to `pdm.cli.commands.import_:Command.do_import` method, "
-        "This function will be removed in the future."
+        "This function will be removed in the future.",
+        stacklevel=2,
     )
     ImportCommand().do_import(*args, **kwargs)
```

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/add.py` & `pdm-2.8.0a2/src/pdm/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/base.py` & `pdm-2.8.0a2/src/pdm/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/build.py` & `pdm-2.8.0a2/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/cache.py` & `pdm-2.8.0a2/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/completion.py` & `pdm-2.8.0a2/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/config.py` & `pdm-2.8.0a2/src/pdm/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/export.py` & `pdm-2.8.0a2/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.8.0a2/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.8.0a2/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/import_cmd.py` & `pdm-2.8.0a2/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/info.py` & `pdm-2.8.0a2/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/init.py` & `pdm-2.8.0a2/src/pdm/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/install.py` & `pdm-2.8.0a2/src/pdm/cli/commands/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         environment = PythonEnvironment(project, python=sys.executable, prefix=str(plugin_root))
         with project.core.ui.open_spinner("[success]Installing plugins...[/]"):
             with project.core.ui.logging("install-plugins"):
                 install_requirements(
                     plugins, environment, clean=True, use_install_cache=project.config["install.cache"]
                 )
             if not plugin_root.joinpath(".gitignore").exists():
+                plugin_root.mkdir(exist_ok=True)
                 plugin_root.joinpath(".gitignore").write_text("*\n")
         project.core.ui.echo("Plugins are installed successfully into [primary].pdm-plugins[/].")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         if not project.pyproject.is_valid and termui.is_interactive():
             actions.ask_for_import(project)
```

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/list.py` & `pdm-2.8.0a2/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/lock.py` & `pdm-2.8.0a2/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.8.0a2/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/publish/package.py` & `pdm-2.8.0a2/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/publish/repository.py` & `pdm-2.8.0a2/src/pdm/cli/commands/publish/repository.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/remove.py` & `pdm-2.8.0a2/src/pdm/cli/commands/remove.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,28 +74,28 @@
         hooks = hooks or HookManager(project)
         check_project_file(project)
         if not packages:
             raise PdmUsageError("Must specify at least one package to remove.")
         group = selection.one()
         lock_groups = project.lockfile.groups
 
-        deps, _ = project.get_pyproject_dependencies(group, selection.dev or False)
+        deps, setter = project.use_pyproject_dependencies(group, selection.dev or False)
         project.core.ui.echo(
             f"Removing packages from [primary]{group}[/] "
             f"{'dev-' if selection.dev else ''}dependencies: " + ", ".join(f"[req]{name}[/]" for name in packages)
         )
         with cd(project.root):
             for name in packages:
                 req = parse_requirement(name)
                 matched_indexes = sorted((i for i, r in enumerate(deps) if req.matches(r)), reverse=True)
                 if not matched_indexes:
                     raise ProjectError(f"[req]{name}[/] does not exist in [primary]{group}[/] dependencies.")
                 for i in matched_indexes:
                     del deps[i]
-        cast(Array, deps).multiline(True)
+        setter(cast(Array, deps).multiline(True))
 
         if not dry_run:
             project.pyproject.write()
         if lock_groups and group not in lock_groups:
             project.core.ui.echo(
                 f"Group [success]{group}[/] isn't in lockfile, skipping lock.", style="warning", err=True
             )
```

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/run.py` & `pdm-2.8.0a2/src/pdm/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/search.py` & `pdm-2.8.0a2/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/self_cmd.py` & `pdm-2.8.0a2/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/show.py` & `pdm-2.8.0a2/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/sync.py` & `pdm-2.8.0a2/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/update.py` & `pdm-2.8.0a2/src/pdm/cli/commands/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,23 +150,28 @@
                 )
             )
         if unconstrained:
             for deps in updated_deps.values():
                 for dep in deps.values():
                     dep.specifier = get_specifier("")
         reqs = [r for deps in all_dependencies.values() for r in deps.values()]
-        resolved = do_lock(
-            project,
-            strategy,
-            chain.from_iterable(updated_deps.values()),
-            reqs,
-            dry_run=True,
-            hooks=hooks,
-            groups=locked_groups,
-        )
+        # Since dry run is always true in the locking,
+        # we need to emit the hook manually with the real dry_run value
+        hooks.try_emit("pre_lock", requirements=reqs, dry_run=dry_run)
+        with hooks.skipping("pre_lock", "post_lock"):
+            resolved = do_lock(
+                project,
+                strategy,
+                chain.from_iterable(updated_deps.values()),
+                reqs,
+                dry_run=True,
+                hooks=hooks,
+                groups=locked_groups,
+            )
+        hooks.try_emit("post_lock", resolution=resolved, dry_run=dry_run)
         for deps in updated_deps.values():
             populate_requirement_names(deps)
         if unconstrained:
             # Need to update version constraints
             save_version_specifiers(updated_deps, resolved, save)
             for group, deps in updated_deps.items():
                 project.add_dependencies(deps, group, selection.dev or False)
```

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/use.py` & `pdm-2.8.0a2/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.8.0a2/src/pdm/cli/commands/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/venv/activate.py` & `pdm-2.8.0a2/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/venv/backends.py` & `pdm-2.8.0a2/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/venv/create.py` & `pdm-2.8.0a2/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/venv/list.py` & `pdm-2.8.0a2/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/venv/purge.py` & `pdm-2.8.0a2/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/venv/remove.py` & `pdm-2.8.0a2/src/pdm/cli/commands/venv/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/commands/venv/utils.py` & `pdm-2.8.0a2/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/completions/pdm.bash` & `pdm-2.8.0a2/src/pdm/cli/completions/pdm.bash`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/completions/pdm.fish` & `pdm-2.8.0a2/src/pdm/cli/completions/pdm.fish`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/completions/pdm.ps1` & `pdm-2.8.0a2/src/pdm/cli/completions/pdm.ps1`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/completions/pdm.zsh` & `pdm-2.8.0a2/src/pdm/cli/completions/pdm.zsh`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/filters.py` & `pdm-2.8.0a2/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/hooks.py` & `pdm-2.8.0a2/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/options.py` & `pdm-2.8.0a2/src/pdm/cli/options.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/templates/__init__.py` & `pdm-2.8.0a2/src/pdm/cli/templates/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,14 +124,16 @@
         try:
             with open(self._path / "pyproject.toml", encoding="utf-8") as fp:
                 template_content = tomlkit.load(fp)
         except FileNotFoundError:
             template_content = tomlkit.document()
 
         merge_dictionary(content, template_content)
+        if "version" in content.get("project", {}).get("dynamic", []):
+            metadata["project"].pop("version", None)
         merge_dictionary(content, metadata)
         if "build-system" in metadata:
             content["build-system"] = metadata["build-system"]
         else:
             content.pop("build-system", None)
         with open(path, "w", encoding="utf-8") as fp:
             fp.write(tomlkit.dumps(content))
@@ -140,15 +142,20 @@
         from pdm.compat import importlib_resources
 
         files = importlib_resources.files(import_name)
 
         self.mirror(files, self._path, skip=[files / "__init__.py"], copyfunc=self._copy_package_file)
 
     def _prepare_git_template(self, url: str) -> None:
-        git_command = ["git", "clone", "--depth", "1", "--recursive", url, self._path.as_posix()]
+        left, amp, right = url.rpartition("@")
+        if left != "git" and amp:
+            extra_args = [f"--branch={right}"]
+        else:
+            extra_args = []
+        git_command = ["git", "clone", "--recursive", "--depth=1", *extra_args, url, self._path.as_posix()]
         result = subprocess.run(git_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         if result.returncode != 0:
             raise PdmException(f"Failed to clone template from git repository {url}: {result.stderr}")
         shutil.rmtree(self._path / ".git", ignore_errors=True)
 
     def _prepare_local_template(self, path: str) -> None:
         src = Path(path)
```

### Comparing `pdm-2.8.0a1/src/pdm/cli/templates/default/.gitignore` & `pdm-2.8.0a2/src/pdm/cli/templates/default/.gitignore`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/cli/utils.py` & `pdm-2.8.0a2/src/pdm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/compat.py` & `pdm-2.8.0a2/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/core.py` & `pdm-2.8.0a2/src/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/environments/__init__.py` & `pdm-2.8.0a2/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/environments/base.py` & `pdm-2.8.0a2/src/pdm/environments/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/environments/local.py` & `pdm-2.8.0a2/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/environments/python.py` & `pdm-2.8.0a2/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/exceptions.py` & `pdm-2.8.0a2/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/formats/__init__.py` & `pdm-2.8.0a2/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/formats/base.py` & `pdm-2.8.0a2/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/formats/flit.py` & `pdm-2.8.0a2/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/formats/pipfile.py` & `pdm-2.8.0a2/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/formats/poetry.py` & `pdm-2.8.0a2/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/formats/requirements.py` & `pdm-2.8.0a2/src/pdm/formats/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/formats/setup_py.py` & `pdm-2.8.0a2/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/installers/core.py` & `pdm-2.8.0a2/src/pdm/installers/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,10 @@
     reporter = project.get_reporter(reqs)
     resolver = project.core.resolver_class(provider, reporter)
     resolve_max_rounds = int(project.config["strategy.resolve_max_rounds"])
     backend = project.backend
     for req in reqs:
         if req.is_file_or_url:
             req.relocate(backend)  # type: ignore[attr-defined]
-    resolved, _ = resolve(
-        resolver,
-        reqs,
-        environment.python_requires,
-        max_rounds=resolve_max_rounds,
-    )
+    resolved, _ = resolve(resolver, reqs, environment.python_requires, max_rounds=resolve_max_rounds, keep_self=True)
     syncer = BaseSynchronizer(resolved, environment, clean=clean, retry_times=0, use_install_cache=use_install_cache)
     syncer.synchronize()
```

### Comparing `pdm-2.8.0a1/src/pdm/installers/installers.py` & `pdm-2.8.0a2/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/installers/manager.py` & `pdm-2.8.0a2/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/installers/packages.py` & `pdm-2.8.0a2/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/installers/synchronizers.py` & `pdm-2.8.0a2/src/pdm/installers/synchronizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,16 @@
     def get_manager(self) -> InstallManager:
         return self.environment.project.core.install_manager_class(
             self.environment, use_install_cache=self.use_install_cache
         )
 
     @property
     def self_key(self) -> str | None:
+        if not self.install_self:
+            return None
         name = self.environment.project.name
         if name:
             return normalize_name(name)
         return name
 
     def _should_update(self, dist: Distribution, can: Candidate) -> bool:
         """Check if the candidate should be updated"""
```

### Comparing `pdm-2.8.0a1/src/pdm/installers/uninstallers.py` & `pdm-2.8.0a2/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/auth.py` & `pdm-2.8.0a2/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/backends.py` & `pdm-2.8.0a2/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/caches.py` & `pdm-2.8.0a2/src/pdm/models/caches.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,22 +79,35 @@
 
 
 class CandidateInfoCache(JSONFileCache[Candidate, CandidateInfo]):
     """A cache manager that stores the
     candidate -> (dependencies, requires_python, summary) mapping.
     """
 
+    @staticmethod
+    def get_url_part(link: Link) -> str:
+        import base64
+
+        from pdm.utils import url_without_fragments
+
+        url = url_without_fragments(link.split_auth()[1])
+        return base64.urlsafe_b64encode(url.encode()).decode()
+
     @classmethod
     def _get_key(cls, obj: Candidate) -> str:
         # Name and version are set when dependencies are resolved,
         # so use them for cache key. Local directories won't be cached.
         if not obj.name or not obj.version:
             raise KeyError("The package is missing a name or version")
         extras = "[{}]".format(",".join(sorted(obj.req.extras))) if obj.req.extras else ""
-        return f"{obj.name}{extras}-{obj.version}"
+        version = obj.version
+        if not obj.req.is_named:
+            assert obj.link is not None
+            version = cls.get_url_part(obj.link)
+        return f"{obj.name}{extras}-{version}"
 
 
 class HashCache:
 
     """Caches hashes of PyPI artifacts so we do not need to re-download them.
 
     Hashes are only cached when the URL appears to contain a hash in it and the
```

### Comparing `pdm-2.8.0a1/src/pdm/models/candidates.py` & `pdm-2.8.0a2/src/pdm/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/in_process/__init__.py` & `pdm-2.8.0a2/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.8.0a2/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/in_process/parse_setup.py` & `pdm-2.8.0a2/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/in_process/pep508.py` & `pdm-2.8.0a2/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.8.0a2/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/markers.py` & `pdm-2.8.0a2/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/project_info.py` & `pdm-2.8.0a2/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/python.py` & `pdm-2.8.0a2/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/repositories.py` & `pdm-2.8.0a2/src/pdm/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/requirements.py` & `pdm-2.8.0a2/src/pdm/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/search.py` & `pdm-2.8.0a2/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/session.py` & `pdm-2.8.0a2/src/pdm/models/session.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/setup.py` & `pdm-2.8.0a2/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/specifiers.py` & `pdm-2.8.0a2/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/venv.py` & `pdm-2.8.0a2/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/versions.py` & `pdm-2.8.0a2/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/models/working_set.py` & `pdm-2.8.0a2/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/pep582/sitecustomize.py` & `pdm-2.8.0a2/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/project/config.py` & `pdm-2.8.0a2/src/pdm/project/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/project/core.py` & `pdm-2.8.0a2/src/pdm/project/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import contextlib
 import hashlib
 import os
 import re
 import shutil
 import sys
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Iterable, Mapping, cast
+from typing import TYPE_CHECKING, Any, Callable, Iterable, Mapping, cast
 
 import tomlkit
 from tomlkit.items import Array
 
 from pdm import termui
 from pdm._types import RepositoryConfig
 from pdm.compat import cached_property
@@ -520,59 +520,68 @@
         hash_in_lockfile = str(self.lockfile.hash)
         if not hash_in_lockfile:
             return False
         algo, hash_value = hash_in_lockfile.split(":")
         content_hash = self.pyproject.content_hash(algo)
         return content_hash == hash_value
 
-    def get_pyproject_dependencies(self, group: str, dev: bool = False) -> tuple[list[str], bool]:
-        """Get the dependencies array in the pyproject.toml
+    def use_pyproject_dependencies(
+        self, group: str, dev: bool = False
+    ) -> tuple[list[str], Callable[[list[str]], None]]:
+        """Get the dependencies array and setter in the pyproject.toml
         Return a tuple of two elements, the first is the dependencies array,
-        and the second tells whether it is a dev-dependencies group.
+        and the second value is a callable to set the dependencies array back.
         """
+
+        def update_dev_dependencies(deps: list[str]) -> None:
+            from tomlkit.container import OutOfOrderTableProxy
+
+            settings.setdefault("dev-dependencies", {})[group] = deps
+            if isinstance(self.pyproject._data["tool"], OutOfOrderTableProxy):
+                # In case of a separate table, we have to remove and re-add it to make the write correct.
+                # This may change the order of tables in the TOML file, but it's the best we can do.
+                # see bug pdm-project/pdm#2056 for details
+                del self.pyproject._data["tool"]["pdm"]
+                self.pyproject._data["tool"]["pdm"] = settings
+
         metadata, settings = self.pyproject.metadata, self.pyproject.settings
         if group == "default":
-            return metadata.setdefault("dependencies", []), False
-        deps_dict = {
-            False: metadata.get("optional-dependencies", {}),
-            True: settings.get("dev-dependencies", {}),
-        }
-        for is_dev, deps in deps_dict.items():
+            return metadata.get("dependencies", tomlkit.array()), lambda x: metadata.__setitem__("dependencies", x)
+        deps_setter = [
+            (
+                metadata.get("optional-dependencies", {}),
+                lambda x: metadata.setdefault("optional-dependencies", {}).__setitem__(group, x),
+            ),
+            (settings.get("dev-dependencies", {}), update_dev_dependencies),
+        ]
+        for deps, setter in deps_setter:
             if group in deps:
-                return deps[group], is_dev
-        if dev:
-            return (
-                settings.setdefault("dev-dependencies", {}).setdefault(group, []),
-                dev,
-            )
-        else:
-            return (
-                metadata.setdefault("optional-dependencies", {}).setdefault(group, []),
-                dev,
-            )
+                return deps[group], setter
+        # If not found, return an empty list and a setter to add the group
+        return tomlkit.array(), deps_setter[int(dev)][1]
 
     def add_dependencies(
         self,
         requirements: dict[str, Requirement],
         to_group: str = "default",
         dev: bool = False,
         show_message: bool = True,
     ) -> None:
-        deps, is_dev = self.get_pyproject_dependencies(to_group, dev)
-        cast(Array, deps).multiline(True)
+        deps, setter = self.use_pyproject_dependencies(to_group, dev)
         for _, dep in requirements.items():
             matched_index = next(
                 (i for i, r in enumerate(deps) if dep.matches(r)),
                 None,
             )
             req = dep.as_line()
             if matched_index is None:
                 deps.append(req)
             else:
                 deps[matched_index] = req
+        setter(cast(Array, deps).multiline(True))
         self.pyproject.write(show_message)
 
     def init_global_project(self) -> None:
         if not self.is_global or not self.pyproject.empty():
             return
         self.root.mkdir(parents=True, exist_ok=True)
         self.pyproject.set_data({"project": {"dependencies": ["pip", "setuptools", "wheel"]}})
@@ -666,14 +675,14 @@
         if self.config["python.use_venv"]:
             finder.add_provider(VenvProvider(self), 0)
         return finder
 
     # compatibility, shouldn't be used directly
     @property
     def meta(self) -> dict[str, Any]:
-        deprecation_warning("project.meta is deprecated, use project.pyproject.metadata instead")
+        deprecation_warning("project.meta is deprecated, use project.pyproject.metadata instead", stacklevel=2)
         return self.pyproject.metadata
 
     @property
     def tool_settings(self) -> dict[str, Any]:
-        deprecation_warning("project.tool_settings is deprecated, use project.pyproject.settings instead")
+        deprecation_warning("project.tool_settings is deprecated, use project.pyproject.settings instead", stacklevel=2)
         return self.pyproject.settings
```

### Comparing `pdm-2.8.0a1/src/pdm/project/lockfile.py` & `pdm-2.8.0a2/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/project/project_file.py` & `pdm-2.8.0a2/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/project/toml_file.py` & `pdm-2.8.0a2/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/pytest.py` & `pdm-2.8.0a2/src/pdm/pytest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/resolver/core.py` & `pdm-2.8.0a2/src/pdm/resolver/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 
 def resolve(
     resolver: Resolver,
     requirements: list[Requirement],
     requires_python: PySpecSet,
     max_rounds: int = 10000,
+    keep_self: bool = False,
 ) -> tuple[dict[str, Candidate], dict[tuple[str, str | None], list[Requirement]]]:
     """Core function to perform the actual resolve process.
     Return a tuple containing 2 items:
 
         1. A map of pinned candidates
         2. A map of resolved dependencies for each dependency group
     """
@@ -45,11 +46,11 @@
         # For source distribution whose name can only be determined after it is built,
         # the key in the resolution map should be updated.
         if key.startswith(":empty:"):
             new_key = provider.identify(candidate)
             mapping[new_key] = mapping.pop(key)
             key = new_key
 
-        if strip_extras(key)[0] == local_name:
+        if not keep_self and strip_extras(key)[0] == local_name:
             del mapping[key]
 
     return mapping, provider.fetched_dependencies
```

### Comparing `pdm-2.8.0a1/src/pdm/resolver/providers.py` & `pdm-2.8.0a2/src/pdm/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/resolver/python.py` & `pdm-2.8.0a2/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/resolver/reporters.py` & `pdm-2.8.0a2/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/signals.py` & `pdm-2.8.0a2/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/termui.py` & `pdm-2.8.0a2/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/src/pdm/utils.py` & `pdm-2.8.0a2/src/pdm/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/conftest.py` & `pdm-2.8.0a2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_add.py` & `pdm-2.8.0a2/tests/cli/test_add.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,25 +252,25 @@
     assert project.pyproject.metadata["dependencies"][0] == "urllib3<2,>=1.23b0"
 
 
 def test_add_editable_package_with_extras(project, working_set, pdm):
     project.environment.python_requires = PySpecSet(">=3.6")
     dep_path = FIXTURES.joinpath("projects/demo").as_posix()
     pdm(["add", "-dGdev", "-e", f"{dep_path}[security]"], obj=project, strict=True)
-    assert f"-e {path_to_url(dep_path)}#egg=demo[security]" in project.get_pyproject_dependencies("dev", True)[0]
+    assert f"-e {path_to_url(dep_path)}#egg=demo[security]" in project.use_pyproject_dependencies("dev", True)[0]
     assert "demo" in working_set
     assert "requests" in working_set
     assert "urllib3" in working_set
 
 
 def test_add_package_with_local_version(project, repository, working_set, pdm):
     repository.add_candidate("foo", "1.0-alpha.0+local")
     pdm(["add", "foo"], obj=project, strict=True)
     assert working_set["foo"].version == "1.0-alpha.0+local"
-    dependencies, _ = project.get_pyproject_dependencies("default")
+    dependencies, _ = project.use_pyproject_dependencies("default")
     assert dependencies[0] == "foo>=1.0a0"
 
 
 def test_add_group_to_lockfile(project, working_set, pdm):
     pdm(["add", "requests"], obj=project, strict=True)
     assert project.lockfile.groups == ["default"]
     pdm(["add", "--group", "tz", "pytz"], obj=project, strict=True)
```

### Comparing `pdm-2.8.0a1/tests/cli/test_build.py` & `pdm-2.8.0a2/tests/cli/test_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 def test_cli_build_with_config_settings(fixture_project, pdm):
     project = fixture_project("demo-src-package")
     result = pdm(["build", "-C--plat-name=win_amd64"], obj=project)
     assert result.exit_code == 0
     assert (project.root / "dist/demo_package-0.1.0-py3-none-win_amd64.whl").exists()
 
 
-@pytest.mark.network
+@pytest.mark.usefixtures("local_finder")
 @pytest.mark.parametrize("isolated", (True, False))
 def test_build_with_no_isolation(fixture_project, pdm, isolated):
     project = fixture_project("demo-failure")
     project.pyproject.set_data({"project": {"name": "demo", "version": "0.1.0"}})
     project.pyproject.write()
     pdm(["add", "first"], obj=project)
     args = ["build"]
```

### Comparing `pdm-2.8.0a1/tests/cli/test_cache.py` & `pdm-2.8.0a2/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_config.py` & `pdm-2.8.0a2/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_fix.py` & `pdm-2.8.0a2/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_hooks.py` & `pdm-2.8.0a2/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_init.py` & `pdm-2.8.0a2/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_install.py` & `pdm-2.8.0a2/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_list.py` & `pdm-2.8.0a2/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_lock.py` & `pdm-2.8.0a2/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_others.py` & `pdm-2.8.0a2/tests/cli/test_others.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_publish.py` & `pdm-2.8.0a2/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_remove.py` & `pdm-2.8.0a2/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_run.py` & `pdm-2.8.0a2/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_self_command.py` & `pdm-2.8.0a2/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_template.py` & `pdm-2.8.0a2/tests/cli/test_template.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_update.py` & `pdm-2.8.0a2/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_use.py` & `pdm-2.8.0a2/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/cli/test_venv.py` & `pdm-2.8.0a2/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/conftest.py` & `pdm-2.8.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.8.0a2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.8.0a2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.8.0a2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.8.0a2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.8.0a2/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.8.0a2/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.8.0a2/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.8.0a2/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.8.0a2/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.8.0a2/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/pypi.json` & `pdm-2.8.0a2/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/fixtures/pyproject.toml` & `pdm-2.8.0a2/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/models/test_backends.py` & `pdm-2.8.0a2/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/models/test_candidates.py` & `pdm-2.8.0a2/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/models/test_marker.py` & `pdm-2.8.0a2/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/models/test_requirements.py` & `pdm-2.8.0a2/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/models/test_setup_parsing.py` & `pdm-2.8.0a2/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/models/test_specifiers.py` & `pdm-2.8.0a2/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/models/test_versions.py` & `pdm-2.8.0a2/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/resolver/test_resolve.py` & `pdm-2.8.0a2/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/test_formats.py` & `pdm-2.8.0a2/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/test_installer.py` & `pdm-2.8.0a2/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/test_integration.py` & `pdm-2.8.0a2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/test_plugin.py` & `pdm-2.8.0a2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/test_project.py` & `pdm-2.8.0a2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/test_signals.py` & `pdm-2.8.0a2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/tests/test_utils.py` & `pdm-2.8.0a2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a1/PKG-INFO` & `pdm-2.8.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.8.0a1
+Version: 2.8.0a2
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.8.0a1 Summary: A modern Python
+Metadata-Version: 2.1 Name: pdm Version: 2.8.0a2 Summary: A modern Python
 package and dependency manager supporting the latest PEP standards Keywords:
 packaging dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

