# Comparing `tmp/craft-archives-1.1.0.tar.gz` & `tmp/craft-archives-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-archives-1.1.0.tar", last modified: Tue May 30 17:09:56 2023, max compression
+gzip compressed data, was "craft-archives-1.1.1.tar", last modified: Fri Jun 30 19:29:03 2023, max compression
```

## Comparing `craft-archives-1.1.0.tar` & `craft-archives-1.1.1.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.202324 craft-archives-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.codespell_ignore_lines
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.190324 craft-archives-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/renovate.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.190324 craft-archives-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/cla-check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/release-drafter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/release-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.yamlignore
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-30 17:09:37.000000 craft-archives-1.1.0/HACKING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-30 17:09:37.000000 craft-archives-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-30 17:09:56.202324 craft-archives-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-30 17:09:37.000000 craft-archives-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/craft_archives/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/craft_archives/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_ppa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_preferences_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_sources_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_uca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/package_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/craft_archives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.190324 craft-archives-1.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/docs/explanation/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/explanation/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/docs/howto/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/howto/add_repo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/howto/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/reference/repo_properties.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-30 17:09:37.000000 craft-archives-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 17:09:56.202324 craft-archives-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/integration/repo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/integration/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/integration/repo/test_apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/integration/repo/test_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/FC42E99D.asc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/empty.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/expected.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/many_blank_lines.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/no_header.preferences
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/only_comment.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/with_header.preferences
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.202324 craft-archives-1.1.0/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14026 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_ppa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_preferences_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_sources_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_uca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_package_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tox.ini
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.694146 craft-archives-1.1.1/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       77 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.codespell_ignore_lines
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.editorconfig
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/.github/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/release-drafter.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3504 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/renovate.json5
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/.github/workflows/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/cla-check.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      822 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/docs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      586 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1448 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/release-publish.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2411 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.github/workflows/tests.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1961 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.gitignore
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      485 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.readthedocs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        6 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.yamlignore
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      201 2023-06-30 19:19:48.000000 craft-archives-1.1.1/.yamllint.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3839 2023-06-30 19:19:48.000000 craft-archives-1.1.1/HACKING.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-06-30 19:19:48.000000 craft-archives-1.1.1/LICENSE
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1489 2023-06-30 19:29:03.694146 craft-archives-1.1.1/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      605 2023-06-30 19:19:48.000000 craft-archives-1.1.1/README.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/craft_archives/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1015 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      160 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives/_version.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1151 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/errors.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/craft_archives/repo/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      874 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    13124 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_key_manager.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1985 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_ppa.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6318 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_preferences_manager.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10621 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_sources_manager.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1573 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/apt_uca.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4618 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5067 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/installer.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    11312 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/package_repository.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1142 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/repo/projects.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3439 2023-06-30 19:19:48.000000 craft-archives-1.1.1/craft_archives/utils.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/craft_archives.egg-info/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1489 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2197 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      505 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/requires.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       15 2023-06-30 19:29:03.000000 craft-archives-1.1.1/craft_archives.egg-info/top_level.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.686146 craft-archives-1.1.1/docs/_static/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/_static/css/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/_static/css/custom.css
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      757 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/changelog.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1678 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/conf.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/explanation/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       72 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/explanation/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/howto/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1500 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/howto/add_repo.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       83 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/howto/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1765 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/reference/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      178 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/reference/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6034 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/reference/repo_properties.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/docs/tutorials/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      238 2023-06-30 19:19:48.000000 craft-archives-1.1.1/docs/tutorials/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8193 2023-06-30 19:19:48.000000 craft-archives-1.1.1/pyproject.toml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2023-06-30 19:29:03.694146 craft-archives-1.1.1/setup.cfg
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1375 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/integration/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/integration/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/integration/repo/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/integration/repo/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6626 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/integration/repo/test_apt_key_manager.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7830 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/integration/repo/test_installer.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/test_data/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1619 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/FC42E99D.asc
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/empty.preferences
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      173 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/expected.preferences
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      127 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/many_blank_lines.preferences
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/test_data/multi-keys/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2419 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/multi-keys/0264B26D.asc
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    15720 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/multi-keys/9E61EF26.asc
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      226 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/no_header.preferences
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       35 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/only_comment.preferences
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      259 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/test_data/with_header.preferences
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.690147 craft-archives-1.1.1/tests/unit/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:29:03.694146 craft-archives-1.1.1/tests/unit/repo/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    17516 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_key_manager.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1890 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_ppa.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6936 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_preferences_manager.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8974 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_sources_manager.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1890 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_apt_uca.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4282 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_installer.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16191 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_package_repository.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1470 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tests/unit/repo/test_projects.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4663 2023-06-30 19:19:48.000000 craft-archives-1.1.1/tox.ini
```

### Comparing `craft-archives-1.1.0/.editorconfig` & `craft-archives-1.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/.github/renovate.json5` & `craft-archives-1.1.1/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/.github/workflows/docs.yaml` & `craft-archives-1.1.1/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/.github/workflows/release-drafter.yaml` & `craft-archives-1.1.1/.github/workflows/release-drafter.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/.github/workflows/release-publish.yaml` & `craft-archives-1.1.1/.github/workflows/release-publish.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 name: Release
 on:
   push:
     tags:
-      - v*
+      # These tags should be protected, remember to enable the rule:
+      # https://github.com/canonical/starbase/settings/tag_protection
+      - "[0-9]+.[0-9]+.[0-9]+"
 
 permissions:
   contents: write
 
 jobs:
   source-wheel:
     runs-on: ubuntu-latest
```

### Comparing `craft-archives-1.1.0/.github/workflows/tests.yaml` & `craft-archives-1.1.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/.gitignore` & `craft-archives-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/.pre-commit-config.yaml` & `craft-archives-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/HACKING.rst` & `craft-archives-1.1.1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/LICENSE` & `craft-archives-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/PKG-INFO` & `craft-archives-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-archives
-Version: 1.1.0
+Version: 1.1.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft-archives-1.1.0/README.rst` & `craft-archives-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/__init__.py` & `craft-archives-1.1.1/craft_archives/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/errors.py` & `craft-archives-1.1.1/craft_archives/errors.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/repo/__init__.py` & `craft-archives-1.1.1/craft_archives/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/repo/apt_key_manager.py` & `craft-archives-1.1.1/craft_archives/repo/apt_key_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """APT key management helpers."""
 
 # pyright: reportMissingTypeStubs=false
+from __future__ import annotations
 
 import logging
 import pathlib
 import subprocess
 import tempfile
 from contextlib import contextmanager
-from typing import Iterable, Iterator, List, Optional
+from typing import Iterable, Iterator, List, Optional, Union
 
 from . import apt_ppa, errors, package_repository
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_APT_KEYSERVER = "keyserver.ubuntu.com"
 
@@ -39,29 +40,37 @@
 
 
 def _call_gpg(
     *parameters: str,
     keyring: Optional[pathlib.Path] = None,
     base_parameters: Iterable[str] = _GPG_PREFIX,
     stdin: Optional[bytes] = None,
+    log: bool = False,
 ) -> bytes:
     if keyring:
         command = [*base_parameters, "--keyring", f"gnupg-ring:{keyring}", *parameters]
     else:
         command = [*base_parameters, *parameters]
     logger.debug(f"Executing command: {command}")
     env = {"LANG": "C.UTF-8"}
-    process = subprocess.run(
-        command,
-        input=stdin,
-        capture_output=True,
-        check=True,
-        env=env,
-    )
-    return process.stdout
+    try:
+        process = subprocess.run(
+            command,
+            input=stdin,
+            capture_output=True,
+            check=True,
+            env=env,
+        )
+        if log:
+            _log_gpg(process)
+        return process.stdout
+    except subprocess.CalledProcessError as error:
+        if log:
+            _log_gpg(error)
+        raise
 
 
 def get_keyring_path(
     key_id: str,
     *,
     is_ascii: bool = False,
     base_path: pathlib.Path = KEYRINGS_PATH,
@@ -130,33 +139,47 @@
           system root "/".
         """
         if root is None:
             return KEYRINGS_PATH
         return root / "etc/apt/keyrings"
 
     @classmethod
-    def get_key_fingerprints(cls, *, key: str) -> List[str]:
-        """List fingerprints found in specified key.
+    def get_key_fingerprints(cls, *, key: Union[str, bytes]) -> List[str]:
+        """List fingerprints found in the specified key.
+
+        Fingerprints for subkeys are not returned. Fingerprints for primary keys are
+        returned in the order that they are found, even if the keys are expired.
 
         :param key: Key data (string) to parse.
 
         :returns: List of key fingerprints/IDs.
         """
+        if isinstance(key, str):
+            key_bytes = key.encode()
+        else:
+            key_bytes = key
+
         with _temporary_home_dir() as tmpdir:
             response = _call_gpg(
                 "--homedir",
                 str(tmpdir),
                 "--import-options",
                 "show-only",
                 "--import",
-                stdin=key.encode(),
+                stdin=key_bytes,
             ).splitlines()
         fingerprints: List[str] = []
+        # Only export fingerprints for primary keys.
+        is_primary = False
         for line in response:
-            if line.startswith(b"fpr:"):
+            if line.startswith(b"pub:"):
+                is_primary = True
+            elif line.startswith(b"sub:"):
+                is_primary = False
+            if line.startswith(b"fpr:") and is_primary:
                 fingerprints.append(line[4:].decode().strip(":"))
         return fingerprints
 
     def is_key_installed(self, *, key_id: str) -> bool:
         """Check if specified key_id is installed.
 
         :param key_id: Key ID to check for. The key will be looked for in the
@@ -177,39 +200,63 @@
             _call_gpg("--list-keys", key_id, keyring=keyring_file)
         except subprocess.CalledProcessError as error:
             logger.warning(f"gpg error: {error.output.decode()}")
             return False
         else:
             return True
 
-    def install_key(self, *, key: str) -> None:
+    def install_key(self, *, key: str, key_id: Optional[str] = None) -> None:
         """Install given key.
 
-        :param key: Key to install.
+        :param key: Contents of key to install.
+        :param key_id: The optional fingerprint of the desired primary key in ``key``.
+            If provided, this fingerprint will be checked after the import is done to
+            ensure that it is present, and the imported file will use this fingerprint
+            for its filename (short id).
 
         :raises: AptGPGKeyInstallError if unable to install key.
         """
         logger.debug(f"Importing key {key}")
         fingerprints = self.get_key_fingerprints(key=key)
         if not fingerprints:
             raise errors.AptGPGKeyInstallError("Invalid GPG key", key=key)
-        if len(fingerprints) != 1:
+
+        if key_id and key_id not in fingerprints:
             raise errors.AptGPGKeyInstallError(
-                "Key must be a single key, not multiple.", key=key
+                "Desired key_id not found in fingerprints", key=key
             )
 
         self._create_keyrings_path()
-        keyring_path = get_keyring_path(fingerprints[0], base_path=self._keyrings_path)
-        try:
-            _call_gpg("--import", "-", keyring=keyring_path, stdin=key.encode())
-        except subprocess.CalledProcessError as error:
-            raise errors.AptGPGKeyInstallError(error.output.decode(), key=key)
+        target_id = key_id or fingerprints[0]
+        keyring_path = get_keyring_path(target_id, base_path=self._keyrings_path)
+
+        # Note: use a temporary homedir because otherwise local configuration can influence
+        # how GPG behaves when importing keys.
+        with _temporary_home_dir() as tmpdir:
+            try:
+                _call_gpg(
+                    "--homedir",
+                    str(tmpdir),
+                    "--import",
+                    "-",
+                    keyring=keyring_path,
+                    stdin=key.encode(),
+                    log=True,
+                )
+            except subprocess.CalledProcessError as error:
+                raise errors.AptGPGKeyInstallError(error.stderr.decode(), key=key)
+
+        if key_id is not None:
+            # Make sure the imported key has the expected key_id
+            imported_keyring = keyring_path.read_bytes()
+            if key_id not in self.get_key_fingerprints(key=imported_keyring):
+                raise errors.AptGPGKeyInstallError(f"key-id {key_id} not imported.")
 
         _configure_keyring_file(keyring_path)
-        logger.debug(f"Installed apt repository key:\n{key}")
+        logger.debug(f"Installed apt repository key:\n{key_id or key}")
 
     def install_key_from_keyserver(
         self, *, key_id: str, key_server: str = DEFAULT_APT_KEYSERVER
     ) -> None:
         """Install key from specified key server.
 
         :param key_id: Key ID to install.
@@ -276,15 +323,15 @@
         # install a fresh one.
         keyring_path = get_keyring_path(key_id, base_path=self._keyrings_path)
         if keyring_path.parent.is_dir():
             keyring_path.unlink(missing_ok=True)
 
         key_path = self.find_asset_with_key_id(key_id=key_id)
         if key_path is not None:
-            self.install_key(key=key_path.read_text())
+            self.install_key(key=key_path.read_text(), key_id=key_id)
         else:
             self.install_key_from_keyserver(key_id=key_id, key_server=key_server)
 
         return True
 
     def _create_keyrings_path(self) -> None:
         """Create the directory that will contain the keys, if necessary."""
@@ -298,7 +345,18 @@
 @contextmanager
 def _temporary_home_dir() -> Iterator[pathlib.Path]:
     """Yield a temporary directory with proper permissions for gpg."""
     with tempfile.TemporaryDirectory() as tmpdir_str:
         tmpdir = pathlib.Path(tmpdir_str)
         tmpdir.chmod(0o700)
         yield tmpdir
+
+
+def _log_gpg(
+    entity: Union[subprocess.CompletedProcess[bytes], subprocess.CalledProcessError]
+) -> None:
+    if entity.stdout:
+        logger.debug("gpg stdout:")
+        logger.debug(entity.stdout.decode())
+    if entity.stderr:
+        logger.debug("gpg stderr:")
+        logger.debug(entity.stderr.decode())
```

### Comparing `craft-archives-1.1.0/craft_archives/repo/apt_ppa.py` & `craft-archives-1.1.1/craft_archives/repo/apt_ppa.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/repo/apt_preferences_manager.py` & `craft-archives-1.1.1/craft_archives/repo/apt_preferences_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/repo/apt_sources_manager.py` & `craft-archives-1.1.1/craft_archives/repo/apt_sources_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/repo/apt_uca.py` & `craft-archives-1.1.1/craft_archives/repo/apt_uca.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/repo/errors.py` & `craft-archives-1.1.1/craft_archives/repo/errors.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/repo/installer.py` & `craft-archives-1.1.1/craft_archives/repo/installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,22 +119,21 @@
 def _verify_all_key_assets_installed(
     *,
     key_assets: pathlib.Path,
     key_manager: AptKeyManager,
 ) -> None:
     """Verify all configured key assets are utilized, error if not."""
     for key_asset in key_assets.glob("*"):
-        key = key_asset.read_text()
-        for key_id in key_manager.get_key_fingerprints(key=key):
-            if not key_manager.is_key_installed(key_id=key_id):
-                raise errors.PackageRepositoryError(
-                    "Found unused key asset {key_asset!r}.",
-                    details="All configured key assets must be utilized.",
-                    resolution="Verify key usage and remove all unused keys.",
-                )
+        key_id = key_asset.stem
+        if not key_manager.is_key_installed(key_id=key_id):
+            raise errors.PackageRepositoryError(
+                "Found unused key asset {key_asset!r}.",
+                details="All configured key assets must be utilized.",
+                resolution="Verify key usage and remove all unused keys.",
+            )
 
 
 def _unmarshal_repositories(
     project_repositories: List[Dict[str, Any]]
 ) -> List[PackageRepository]:
     """Create package repositories objects from project data."""
     repositories: List[PackageRepository] = []
```

### Comparing `craft-archives-1.1.0/craft_archives/repo/package_repository.py` & `craft-archives-1.1.1/craft_archives/repo/package_repository.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/repo/projects.py` & `craft-archives-1.1.1/craft_archives/repo/projects.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives/utils.py` & `craft-archives-1.1.1/craft_archives/utils.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/craft_archives.egg-info/PKG-INFO` & `craft-archives-1.1.1/craft_archives.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-archives
-Version: 1.1.0
+Version: 1.1.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft-archives-1.1.0/craft_archives.egg-info/SOURCES.txt` & `craft-archives-1.1.1/craft_archives.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 tests/test_data/FC42E99D.asc
 tests/test_data/empty.preferences
 tests/test_data/expected.preferences
 tests/test_data/many_blank_lines.preferences
 tests/test_data/no_header.preferences
 tests/test_data/only_comment.preferences
 tests/test_data/with_header.preferences
+tests/test_data/multi-keys/0264B26D.asc
+tests/test_data/multi-keys/9E61EF26.asc
 tests/unit/__init__.py
 tests/unit/repo/__init__.py
 tests/unit/repo/test_apt_key_manager.py
 tests/unit/repo/test_apt_ppa.py
 tests/unit/repo/test_apt_preferences_manager.py
 tests/unit/repo/test_apt_sources_manager.py
 tests/unit/repo/test_apt_uca.py
```

### Comparing `craft-archives-1.1.0/docs/conf.py` & `craft-archives-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/docs/howto/add_repo.rst` & `craft-archives-1.1.1/docs/howto/add_repo.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/docs/index.rst` & `craft-archives-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/docs/reference/repo_properties.rst` & `craft-archives-1.1.1/docs/reference/repo_properties.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/pyproject.toml` & `craft-archives-1.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 dynamic = ["version", "readme"]
 dependencies = [
     "distro>=1.3.0",
     "launchpadlib",
     "lazr.restfulclient",
     "lazr.uri",
     "overrides",
-    "pydantic",
+    "pydantic<2.0.0",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: POSIX :: Linux",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
@@ -30,14 +30,15 @@
 [project.optional-dependencies]
 dev = [
     "pytest==7.3.1",
     "pytest-cov==4.0.0",
     "pytest-check==2.1.4",
     "coverage[toml]==7.2.5",
     "pytest-mock==3.10.0",
+    "python-gnupg==0.5.0",
 ]
 lint = [
     "black==23.3.0",
     "codespell[toml]==2.2.4",
     "ruff==0.0.269",
     "yamllint==1.32.0"
 ]
@@ -63,29 +64,39 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 readme = {file = "README.rst"}
 
 [tool.setuptools.packages.find]
-exclude = [
-    "dist",
-    "docs",
-    "results",
-    "tests",
-]
+include = ["*craft*"]
+namespaces = false
 
 [tool.setuptools_scm]
 write_to = "craft_archives/_version.py"
+# the version comes from the latest annotated git tag formatted as 'X.Y.Z'
+# version scheme:
+#   - X.Y.Z.post<commits since tag>+g<hash>.d<%Y%m%d>
+# parts of scheme:
+#   - X.Y.Z - most recent git tag
+#   - post<commits since tag>+g<hash> - present when current commit is not tagged
+#   - .d<%Y%m%d> - present when working dir is dirty
+# version scheme when no tags exist:
+#   - 0.0.post<total commits>+g<hash>
+version_scheme = "post-release"
+# deviations from the default 'git describe' command:
+# - only match annotated tags
+# - only match tags formatted as 'X.Y.Z'
+git_describe_command = "git describe --dirty --long --match '[0-9]*.[0-9]*.[0-9]*' --exclude '*[^0-9.]*'"
 
 [tool.black]
 target-version = ["py38"]
 
 [tool.codespell]
-ignore-words-list = "buildd,crate,keyserver,comandos,ro,dedent,dedented"
+ignore-words-list = "buildd,crate,keyserver,comandos,ro,dedent,dedented,fpr"
 skip = ".tox,.git,build,.*_cache,__pycache__,*.tar,*.snap,*.png,./node_modules,./docs/_build,.direnv,.venv,venv,.vscode"
 quiet-level = 3
 check-filenames = true
 exclude-file = ".codespell_ignore_lines"
 
 [tool.isort]
 multi_line_output = 3
@@ -207,15 +218,16 @@
     "E501",  # Line too long (reason: black will automatically fix this for us)
     "D105",  # Missing docstring in magic method (reason: magic methods already have definitions)
     "D107",  # Missing docstring in __init__ (reason: documented in class docstring)
     "D203",  # 1 blank line required before class docstring (reason: pep257 default)
     "D213",  # Multi-line docstring summary should start at the second line (reason: pep257 default)
     "D215",  # Section underline is over-indented (reason: pep257 default)
     "A003",  # Class attribute shadowing built-in (reason: Class attributes don't often get bare references)
-
+    "UP006", # Use `list` instead of `List` for type annotation
+    "UP007", # Use `X | Y` for type annotations
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/**.py" = [  # Some things we want for the moin project are unnecessary in tests.
     "D",  # Ignore docstring rules in tests
     "ANN", # Ignore type annotations in tests
     "S101",  # Allow assertions in tests
```

### Comparing `craft-archives-1.1.0/tests/conftest.py` & `craft-archives-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/tests/integration/repo/test_installer.py` & `craft-archives-1.1.1/tests/integration/repo/test_installer.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,14 +64,25 @@
     Suites: {codename}-updates/{cloud}
     Components: main
     Architectures: amd64
     Signed-By: {key_location}/craft-EC4926EA.gpg
     """
 ).lstrip()
 
+PUPPET_SOURCES = dedent(
+    """
+    Types: deb
+    URIs: http://apt.puppet.com
+    Suites: focal
+    Components: puppet-tools
+    Architectures: amd64
+    Signed-By: {key_location}/craft-9E61EF26.gpg
+    """
+).lstrip()
+
 PREFERENCES = dedent(
     """
     # This file is managed by craft-archives
     Package: *
     Pin: origin "ppa.launchpad.net"
     Pin-Priority: 100
 
@@ -147,23 +158,32 @@
         # a "cloud" repo
         {
             "type": "apt",
             "cloud": CLOUD_DATA["cloud"],
             "pocket": "updates",
             "priority": 123,
         },
+        # A key with multiple keys inside.
+        {
+            "type": "apt",
+            "components": ["puppet-tools"],
+            "suites": ["focal"],
+            "url": "http://apt.puppet.com",
+            "key-id": "D6811ED3ADEEB8441AF5AA8F4528B6CD9E61EF26",
+        },
     ]
 
 
 @pytest.fixture
-def test_keys_dir(tmp_path, sample_key_path) -> Path:
+def test_keys_dir(tmp_path, test_data_dir) -> Path:
     target_dir = tmp_path / "keys"
     target_dir.mkdir()
 
-    shutil.copy2(sample_key_path, target_dir)
+    shutil.copy2(test_data_dir / "FC42E99D.asc", target_dir)
+    shutil.copy2(test_data_dir / "multi-keys/9E61EF26.asc", target_dir)
 
     return target_dir
 
 
 def test_install(fake_etc_apt, all_repo_types, test_keys_dir):
     """Integrated test that checks the configuration of keys, sources and pins."""
 
@@ -188,15 +208,20 @@
     check_preferences(etc_apt)
 
 
 def check_keyrings(etc_apt_dir: Path) -> None:
     keyrings_dir = etc_apt_dir / "keyrings"
 
     # Must have exactly these keyring files, one for each repo
-    expected_key_ids = ("6A755776", "FC42E99D", "EC4926EA")
+    expected_key_ids = (
+        "6A755776",
+        "FC42E99D",
+        "EC4926EA",
+        "9E61EF26",
+    )
 
     assert len(list(keyrings_dir.iterdir())) == len(expected_key_ids)
     for key_id in expected_key_ids:
         keyring_file = keyrings_dir / f"craft-{key_id}.gpg"
         assert keyring_file.is_file()
 
 
@@ -217,14 +242,15 @@
             codename=VERSION_CODENAME, key_location=signed_by_location
         ),
         f"cloud-{cloud_name}": CLOUD_SOURCES.format(
             cloud=cloud_name,
             codename=codename,
             key_location=signed_by_location,
         ),
+        "http_apt_puppet_com": PUPPET_SOURCES.format(key_location=signed_by_location),
     }
 
     assert len(list(keyrings_on_fs.iterdir())) == len(source_to_contents)
 
     for source_repo, expected_contents in source_to_contents.items():
         source_file = sources_dir / f"craft-{source_repo}.sources"
         assert source_file.is_file()
```

### Comparing `craft-archives-1.1.0/tests/test_data/FC42E99D.asc` & `craft-archives-1.1.1/tests/test_data/FC42E99D.asc`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/tests/unit/repo/test_apt_key_manager.py` & `craft-archives-1.1.1/tests/unit/repo/test_apt_key_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,14 +32,46 @@
 
 SAMPLE_GPG_SHOW_KEY_OUTPUT = b"""\
 pub:-:4096:1:F1831DDAFC42E99D:1416490823:::-:::scSC::::::23::0:
 fpr:::::::::FAKE-KEY-ID-FROM-GNUPG:
 uid:-::::1416490823::DCB9EEE37DC9FD84C3DB333BFBF6C41A075EEF62::Launchpad PPA for Snappy Developers::::::::::0:
 """
 
+# Real output listing keys with sub/multiple keys.
+
+# Docker repo: 1 primary key ("pub:") and 1 subkey ("sub:")
+SAMPLE_GPG_DOCKER_OUTPUT = b"""\
+pub:-:4096:1:8D81803C0EBFCD88:1487788586:::-:::escaESCA::::::23::0:
+fpr:::::::::9DC858229FC7DD38854AE2D88D81803C0EBFCD88:
+uid:-::::1487792064::B50C6A3598EE2C27B34302761B93B277BF674C93::Docker Release (CE deb) <docker@docker.com>::::::::::0:
+sub:-:4096:1:7EA0A9C3F273FCD8:1487788586::::::s::::::23:
+fpr:::::::::D3306A018370199E527AE7997EA0A9C3F273FCD8:
+"""
+
+# Puppet repo: Multiple primary and subkeys, most expired ("pub:e:" and "sub:e:").
+SAMPLE_GPG_PUPPET_OUTPUT = b"""\
+pub:e:4096:1:B8F999C007BB6C57:1360109177:1549910347::-:::sc::::::23::0:
+fpr:::::::::8735F5AF62A99A628EC13377B8F999C007BB6C57:
+uid:e::::1455302347::A8FC88656336852AD4301DF059CEE6134FD37C21::Puppet Labs Nightly Build Key (Puppet Labs Nightly Build Key) <delivery@puppetlabs.com>::::::::::0:
+uid:e::::1455302347::4EF2A82F1FF355343885012A832C628E1A4F73A8::Puppet Labs Nightly Build Key (Puppet Labs Nightly Build Key) <info@puppetlabs.com>::::::::::0:
+sub:e:4096:1:AE8282E5A5FC3E74:1360109177:1549910293:::::e::::::23:
+fpr:::::::::F838D657CCAF0E4A6375B0E9AE8282E5A5FC3E74:
+gpg: key 7F438280EF8D349F: 8 signatures not checked due to missing keys
+pub:e:4096:1:7F438280EF8D349F:1471554366:1629234366::-:::sc::::::23::0:
+fpr:::::::::6F6B15509CF8E59E6E469F327F438280EF8D349F:
+uid:e::::1471554366::B648B946D1E13EEA5F4081D8FE5CF4D001200BC7::Puppet, Inc. Release Key (Puppet, Inc. Release Key) <release@puppet.com>::::::::::0:
+sub:e:4096:1:A2D80E04656674AE:1471554366:1629234366:::::e::::::23:
+fpr:::::::::07F5ABF8FE84BC3736D2AAD3A2D80E04656674AE:
+pub:-:4096:1:4528B6CD9E61EF26:1554759562:1743975562::-:::scESC::::::23::0:
+fpr:::::::::D6811ED3ADEEB8441AF5AA8F4528B6CD9E61EF26:
+uid:-::::1554759562::B648B946D1E13EEA5F4081D8FE5CF4D001200BC7::Puppet, Inc. Release Key (Puppet, Inc. Release Key) <release@puppet.com>::::::::::0:
+sub:-:4096:1:F230A24E9F057A83:1554759562:1743975562:::::e::::::23:
+fpr:::::::::90A29D0A6576E2CA185AED3EF230A24E9F057A83:
+"""
+
 
 @pytest.fixture(autouse=True)
 def mock_environ_copy(mocker):
     yield mocker.patch("os.environ.copy")
 
 
 @pytest.fixture(autouse=True)
@@ -105,18 +137,15 @@
     apt_gpg,
 ):
     key_path = apt_gpg.find_asset_with_key_id(key_id="foo")
 
     assert key_path is None
 
 
-def test_get_key_fingerprints(
-    apt_gpg,
-    mock_run,
-):
+def test_get_key_fingerprints(apt_gpg, mock_run):
     mock_run.return_value.stdout = SAMPLE_GPG_SHOW_KEY_OUTPUT
 
     ids = apt_gpg.get_key_fingerprints(key="8" * 40)
 
     assert ids == ["FAKE-KEY-ID-FROM-GNUPG"]
     assert mock_run.mock_calls == [
         call(
@@ -136,14 +165,38 @@
             check=True,
             env={"LANG": "C.UTF-8"},
         )
     ]
 
 
 @pytest.mark.parametrize(
+    "sample_output,expected_keys",
+    [
+        (SAMPLE_GPG_DOCKER_OUTPUT, ["9DC858229FC7DD38854AE2D88D81803C0EBFCD88"]),
+        (
+            SAMPLE_GPG_PUPPET_OUTPUT,
+            [
+                "8735F5AF62A99A628EC13377B8F999C007BB6C57",
+                "6F6B15509CF8E59E6E469F327F438280EF8D349F",
+                "D6811ED3ADEEB8441AF5AA8F4528B6CD9E61EF26",
+            ],
+        ),
+    ],
+)
+def test_get_key_fingerprints_multi_keys(
+    apt_gpg, mock_run, sample_output, expected_keys
+):
+    mock_run.return_value.stdout = sample_output
+
+    ids = apt_gpg.get_key_fingerprints(key="8" * 40)
+
+    assert ids == expected_keys
+
+
+@pytest.mark.parametrize(
     "should_raise,expected_is_installed",
     [
         (True, False),
         (False, True),
     ],
 )
 def test_is_key_installed(
@@ -199,21 +252,27 @@
 
     is_installed = apt_gpg.is_key_installed(key_id="foo")
 
     assert is_installed is False
     mock_logger.warning.assert_called_once_with("gpg error: some error")
 
 
+@pytest.mark.parametrize("key_id", (None, "FAKE-KEY-ID-FROM-GNUPG"))
 def test_install_key(
-    apt_gpg, mock_run, mock_chmod, sample_key_string, sample_key_bytes
+    apt_gpg, mock_run, mock_chmod, sample_key_string, sample_key_bytes, tmp_path, key_id
 ):
     mock_run.return_value.stdout = SAMPLE_GPG_SHOW_KEY_OUTPUT
+    mock_run.return_value.stderr = None
 
     apt_gpg.install_key(key=sample_key_string)
 
+    # The key should be imported to a file that contains the short-id of the
+    # "FAKE-KEY-ID-FROM-GNUPG" fingerprint, (so the last 8 characters).
+    expected_imported_keyring = f"gnupg-ring:{tmp_path / 'craft-OM-GNUPG.gpg'}"
+
     assert mock_run.mock_calls == [
         call(
             [
                 "gpg",
                 "--batch",
                 "--no-default-keyring",
                 "--with-colons",
@@ -231,14 +290,16 @@
         call(
             [
                 "gpg",
                 "--batch",
                 "--no-default-keyring",
                 "--with-colons",
                 "--keyring",
+                expected_imported_keyring,
+                "--homedir",
                 mock.ANY,
                 "--import",
                 "-",
             ],
             input=sample_key_bytes,
             capture_output=True,
             check=True,
@@ -278,42 +339,45 @@
 
 
 def test_install_key_with_gpg_failure(apt_gpg, mock_run):
     mock_run.side_effect = [
         subprocess.CompletedProcess(
             ["gpg", "--do-something"], returncode=0, stdout=SAMPLE_GPG_SHOW_KEY_OUTPUT
         ),
-        subprocess.CalledProcessError(cmd=["foo"], returncode=1, output=b"some error"),
+        subprocess.CalledProcessError(cmd=["foo"], returncode=1, stderr=b"some error"),
     ]
 
     with pytest.raises(errors.AptGPGKeyInstallError) as raised:
         apt_gpg.install_key(key="FAKEKEY")
 
     assert str(raised.value) == "Failed to install GPG key: some error"
 
 
-@pytest.mark.parametrize(
-    "fingerprints,error",
-    [
-        pytest.param([], "Invalid GPG key", id="no keys"),
-        pytest.param(
-            ["finger1", "finger2"],
-            "Key must be a single key, not multiple.",
-            id="multiple keys",
-        ),
-    ],
-)
-def test_install_key_with_key_issue(apt_gpg, mocker, fingerprints, error):
+def test_install_key_with_no_fingerprints(apt_gpg, mocker):
+    """Test installing key contents that have no fingerprints at all."""
     mock_fingerprints = mocker.patch.object(apt_gpg, "get_key_fingerprints")
-    mock_fingerprints.return_value = fingerprints
+    mock_fingerprints.return_value = []
 
     with pytest.raises(errors.AptGPGKeyInstallError) as raised:
         apt_gpg.install_key(key="key")
 
-    assert str(raised.value) == f"Failed to install GPG key: {error}"
+    assert str(raised.value) == "Failed to install GPG key: Invalid GPG key"
+
+
+def test_install_key_with_invalid_key_id(apt_gpg, mocker):
+    """Test installing key contents where the desired key-id is *not* among the
+    existing fingerprints."""
+    mock_fingerprints = mocker.patch.object(apt_gpg, "get_key_fingerprints")
+    mock_fingerprints.return_value = ["FINGERPRINT-1", "FINGERPRINT-2"]
+
+    expected_error = (
+        "Failed to install GPG key: Desired key_id not found in fingerprints"
+    )
+    with pytest.raises(errors.AptGPGKeyInstallError, match=expected_error):
+        apt_gpg.install_key(key="key", key_id="IM-NOT-THERE")
 
 
 def test_install_key_from_keyserver(apt_gpg, mock_run, mock_chmod):
     apt_gpg.install_key_from_keyserver(key_id="FAKE_KEY", key_server="key.server")
 
     assert mock_run.mock_calls == [
         call(
@@ -400,15 +464,15 @@
         suites=["xenial"],
         url="http://archive.ubuntu.com/ubuntu",
     )
 
     updated = apt_gpg.install_package_repository_key(package_repo=package_repo)
 
     assert updated is True
-    assert mock_install_key.mock_calls == [call(key="key-data")]
+    assert mock_install_key.mock_calls == [call(key="key-data", key_id=key_id)]
 
 
 def test_install_package_repository_key_apt_from_keyserver(apt_gpg, mocker):
     mock_install_key_from_keyserver = mocker.patch(
         "craft_archives.repo.apt_key_manager.AptKeyManager.install_key_from_keyserver"
     )
     mocker.patch(
```

### Comparing `craft-archives-1.1.0/tests/unit/repo/test_apt_ppa.py` & `craft-archives-1.1.1/tests/unit/repo/test_apt_ppa.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/tests/unit/repo/test_apt_preferences_manager.py` & `craft-archives-1.1.1/tests/unit/repo/test_apt_preferences_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/tests/unit/repo/test_apt_sources_manager.py` & `craft-archives-1.1.1/tests/unit/repo/test_apt_sources_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/tests/unit/repo/test_apt_uca.py` & `craft-archives-1.1.1/tests/unit/repo/test_apt_uca.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/tests/unit/repo/test_installer.py` & `craft-archives-1.1.1/tests/unit/repo/test_installer.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/tests/unit/repo/test_package_repository.py` & `craft-archives-1.1.1/tests/unit/repo/test_package_repository.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/tests/unit/repo/test_projects.py` & `craft-archives-1.1.1/tests/unit/repo/test_projects.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.0/tox.ini` & `craft-archives-1.1.1/tox.ini`

 * *Files identical despite different names*

