# Comparing `tmp/napari-aphid-1.1.6.tar.gz` & `tmp/napari-aphid-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-aphid-1.1.6.tar", last modified: Tue Jan 31 07:25:26 2023, max compression
+gzip compressed data, was "napari-aphid-1.1.7.tar", last modified: Fri Jun 30 20:10:08 2023, max compression
```

## Comparing `napari-aphid-1.1.6.tar` & `napari-aphid-1.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 07:25:26.194316 napari-aphid-1.1.6/
-drwxrwxrwx   0        0        0        0 2023-01-31 07:25:26.114307 napari-aphid-1.1.6/.github/
-drwxrwxrwx   0        0        0        0 2023-01-31 07:25:26.143308 napari-aphid-1.1.6/.github/workflows/
--rw-rw-rw-   0        0        0     2904 2022-09-07 12:18:42.000000 napari-aphid-1.1.6/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1076 2022-09-07 12:18:42.000000 napari-aphid-1.1.6/.gitignore
-drwxrwxrwx   0        0        0        0 2023-01-31 07:25:26.152307 napari-aphid-1.1.6/.napari-hub/
--rw-rw-rw-   0        0        0      472 2022-09-07 12:18:42.000000 napari-aphid-1.1.6/.napari-hub/DESCRIPTION.md
--rw-rw-rw-   0        0        0      575 2023-01-31 07:18:51.000000 napari-aphid-1.1.6/.napari-hub/config.yml
--rw-rw-rw-   0        0        0     1208 2022-09-07 12:18:42.000000 napari-aphid-1.1.6/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1516 2022-09-07 12:18:42.000000 napari-aphid-1.1.6/LICENSE
--rw-rw-rw-   0        0        0      101 2022-09-07 12:18:42.000000 napari-aphid-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4218 2023-01-31 07:25:26.194316 napari-aphid-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2935 2023-01-31 07:18:51.000000 napari-aphid-1.1.6/README.md
--rw-rw-rw-   0        0        0      221 2023-01-13 13:31:05.000000 napari-aphid-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0     1914 2023-01-31 07:25:26.196316 napari-aphid-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1400 2023-01-31 07:19:26.000000 napari-aphid-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-31 07:25:26.115308 napari-aphid-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-01-31 07:25:26.165315 napari-aphid-1.1.6/src/napari_aphid/
--rw-rw-rw-   0        0        0     1019 2023-01-10 12:36:41.000000 napari-aphid-1.1.6/src/napari_aphid/RunBatch.ijm
--rw-rw-rw-   0        0        0      251 2023-01-31 07:19:15.000000 napari-aphid-1.1.6/src/napari_aphid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 07:25:26.193316 napari-aphid-1.1.6/src/napari_aphid/_tests/
--rw-rw-rw-   0        0        0        0 2022-09-07 12:18:42.000000 napari-aphid-1.1.6/src/napari_aphid/_tests/__init__.py
--rw-rw-rw-   0        0        0       86 2023-01-13 10:45:02.000000 napari-aphid-1.1.6/src/napari_aphid/_tests/test_widget.py
--rw-rw-rw-   0        0        0    33497 2023-01-20 08:26:09.000000 napari-aphid-1.1.6/src/napari_aphid/_widget.py
--rw-rw-rw-   0        0        0      797 2023-01-11 07:07:44.000000 napari-aphid-1.1.6/src/napari_aphid/napari.yaml
--rw-rw-rw-   0        0        0      382 2022-09-08 09:05:42.000000 napari-aphid-1.1.6/src/napari_aphid/path.py
-drwxrwxrwx   0        0        0        0 2023-01-31 07:25:26.191317 napari-aphid-1.1.6/src/napari_aphid.egg-info/
--rw-rw-rw-   0        0        0     4218 2023-01-31 07:25:26.000000 napari-aphid-1.1.6/src/napari_aphid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      652 2023-01-31 07:25:26.000000 napari-aphid-1.1.6/src/napari_aphid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 07:25:26.000000 napari-aphid-1.1.6/src/napari_aphid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-01-31 07:25:26.000000 napari-aphid-1.1.6/src/napari_aphid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      161 2023-01-31 07:25:26.000000 napari-aphid-1.1.6/src/napari_aphid.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-31 07:25:26.000000 napari-aphid-1.1.6/src/napari_aphid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      675 2023-01-20 08:07:34.000000 napari-aphid-1.1.6/tox.ini
+drwxrwxr-x   0 g-laris89  (1000) g-laris89  (1000)        0 2023-06-30 20:10:08.862600 napari-aphid-1.1.7/
+drwxrwxr-x   0 g-laris89  (1000) g-laris89  (1000)        0 2023-06-30 20:10:08.858600 napari-aphid-1.1.7/.github/
+drwxrwxr-x   0 g-laris89  (1000) g-laris89  (1000)        0 2023-06-30 20:10:08.858600 napari-aphid-1.1.7/.github/workflows/
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)     2814 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/.github/workflows/test_and_deploy.yml
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      992 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/.gitignore
+drwxrwxr-x   0 g-laris89  (1000) g-laris89  (1000)        0 2023-06-30 20:10:08.858600 napari-aphid-1.1.7/.napari-hub/
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      463 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/.napari-hub/DESCRIPTION.md
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      562 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/.napari-hub/config.yml
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)     1167 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/.pre-commit-config.yaml
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)     1488 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/LICENSE
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)       96 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/MANIFEST.in
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)     8147 2023-06-30 20:10:08.862600 napari-aphid-1.1.7/PKG-INFO
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)     6892 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/README.md
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      209 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/pyproject.toml
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)     1838 2023-06-30 20:10:08.862600 napari-aphid-1.1.7/setup.cfg
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)     1361 2023-06-30 20:09:44.000000 napari-aphid-1.1.7/setup.py
+drwxrwxr-x   0 g-laris89  (1000) g-laris89  (1000)        0 2023-06-30 20:10:08.858600 napari-aphid-1.1.7/src/
+drwxrwxr-x   0 g-laris89  (1000) g-laris89  (1000)        0 2023-06-30 20:10:08.862600 napari-aphid-1.1.7/src/napari_aphid/
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      988 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/src/napari_aphid/RunBatch.ijm
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      242 2023-06-30 20:09:58.000000 napari-aphid-1.1.7/src/napari_aphid/__init__.py
+drwxrwxr-x   0 g-laris89  (1000) g-laris89  (1000)        0 2023-06-30 20:10:08.862600 napari-aphid-1.1.7/src/napari_aphid/_tests/
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)        0 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/src/napari_aphid/_tests/__init__.py
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)       81 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/src/napari_aphid/_tests/test_widget.py
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)    32601 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/src/napari_aphid/_widget.py
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      773 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/src/napari_aphid/napari.yaml
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      369 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/src/napari_aphid/path.py
+drwxrwxr-x   0 g-laris89  (1000) g-laris89  (1000)        0 2023-06-30 20:10:08.862600 napari-aphid-1.1.7/src/napari_aphid.egg-info/
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)     8147 2023-06-30 20:10:08.000000 napari-aphid-1.1.7/src/napari_aphid.egg-info/PKG-INFO
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      652 2023-06-30 20:10:08.000000 napari-aphid-1.1.7/src/napari_aphid.egg-info/SOURCES.txt
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)        1 2023-06-30 20:10:08.000000 napari-aphid-1.1.7/src/napari_aphid.egg-info/dependency_links.txt
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)       58 2023-06-30 20:10:08.000000 napari-aphid-1.1.7/src/napari_aphid.egg-info/entry_points.txt
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      161 2023-06-30 20:10:08.000000 napari-aphid-1.1.7/src/napari_aphid.egg-info/requires.txt
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)       13 2023-06-30 20:10:08.000000 napari-aphid-1.1.7/src/napari_aphid.egg-info/top_level.txt
+-rw-rw-r--   0 g-laris89  (1000) g-laris89  (1000)      643 2023-06-30 20:07:12.000000 napari-aphid-1.1.7/tox.ini
```

### Comparing `napari-aphid-1.1.6/.github/workflows/test_and_deploy.yml` & `napari-aphid-1.1.7/.github/workflows/test_and_deploy.yml`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# This workflows will upload a Python Package using Twine when a release is created
-# For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
-
-name: tests
-
-on:
-  push:
-    branches:
-      - main
-      - npe2
-    tags:
-      - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
-  pull_request:
-    branches:
-      - main
-      - npe2
-  workflow_dispatch:
-
-jobs:
-  test:
-    name: ${{ matrix.platform }} py${{ matrix.python-version }}
-    runs-on: ${{ matrix.platform }}
-    strategy:
-      matrix:
-        platform: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ['3.8', '3.9', '3.10']
-
-    steps:
-      - uses: actions/checkout@v3
-
-      - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python-version }}
-
-      # these libraries enable testing on Qt on linux
-      - uses: tlambert03/setup-qt-libs@v1
-
-      # strategy borrowed from vispy for installing opengl libs on windows
-      - name: Install Windows OpenGL
-        if: runner.os == 'Windows'
-        run: |
-          git clone --depth 1 https://github.com/pyvista/gl-ci-helpers.git
-          powershell gl-ci-helpers/appveyor/install_opengl.ps1
-
-      # note: if you need dependencies from conda, considering using
-      # setup-miniconda: https://github.com/conda-incubator/setup-miniconda
-      # and
-      # tox-conda: https://github.com/tox-dev/tox-conda
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python -m pip install setuptools tox tox-gh-actions
-
-      # this runs the platform-specific tests declared in tox.ini
-      - name: Test with tox
-        uses: GabrielBB/xvfb-action@v1
-        with:
-          run: python -m tox
-        env:
-          PLATFORM: ${{ matrix.platform }}
-
-      - name: Coverage
-        uses: codecov/codecov-action@v2
-
-  deploy:
-    # this will run when you have tagged a commit, starting with "v*"
-    # and requires that you have put your twine API key in your
-    # github secrets (see readme for details)
-    needs: [test]
-    runs-on: ubuntu-latest
-    if: contains(github.ref, 'tags')
-    steps:
-      - uses: actions/checkout@v2
-      - name: Set up Python
-        uses: actions/setup-python@v2
-        with:
-          python-version: "3.x"
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          pip install -U setuptools setuptools_scm wheel twine build
-      - name: Build and publish
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
-        run: |
-          git tag
-          python -m build .
-          twine upload dist/*
+# This workflows will upload a Python Package using Twine when a release is created
+# For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
+
+name: tests
+
+on:
+  push:
+    branches:
+      - main
+      - npe2
+    tags:
+      - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
+  pull_request:
+    branches:
+      - main
+      - npe2
+  workflow_dispatch:
+
+jobs:
+  test:
+    name: ${{ matrix.platform }} py${{ matrix.python-version }}
+    runs-on: ${{ matrix.platform }}
+    strategy:
+      matrix:
+        platform: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: ['3.8', '3.9', '3.10']
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      # these libraries enable testing on Qt on linux
+      - uses: tlambert03/setup-qt-libs@v1
+
+      # strategy borrowed from vispy for installing opengl libs on windows
+      - name: Install Windows OpenGL
+        if: runner.os == 'Windows'
+        run: |
+          git clone --depth 1 https://github.com/pyvista/gl-ci-helpers.git
+          powershell gl-ci-helpers/appveyor/install_opengl.ps1
+
+      # note: if you need dependencies from conda, considering using
+      # setup-miniconda: https://github.com/conda-incubator/setup-miniconda
+      # and
+      # tox-conda: https://github.com/tox-dev/tox-conda
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          python -m pip install setuptools tox tox-gh-actions
+
+      # this runs the platform-specific tests declared in tox.ini
+      - name: Test with tox
+        uses: GabrielBB/xvfb-action@v1
+        with:
+          run: python -m tox
+        env:
+          PLATFORM: ${{ matrix.platform }}
+
+      - name: Coverage
+        uses: codecov/codecov-action@v2
+
+  deploy:
+    # this will run when you have tagged a commit, starting with "v*"
+    # and requires that you have put your twine API key in your
+    # github secrets (see readme for details)
+    needs: [test]
+    runs-on: ubuntu-latest
+    if: contains(github.ref, 'tags')
+    steps:
+      - uses: actions/checkout@v2
+      - name: Set up Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: "3.x"
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install -U setuptools setuptools_scm wheel twine build
+      - name: Build and publish
+        env:
+          TWINE_USERNAME: __token__
+          TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
+        run: |
+          git tag
+          python -m build .
+          twine upload dist/*
```

### Comparing `napari-aphid-1.1.6/.pre-commit-config.yaml` & `napari-aphid-1.1.7/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
-    hooks:
-      - id: check-docstring-first
-      - id: end-of-file-fixer
-      - id: trailing-whitespace
-        exclude: ^.napari-hub/*
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.1
-    hooks:
-      - id: pyupgrade
-        args: [--py38-plus, --keep-runtime-typing]
-  - repo: https://github.com/myint/autoflake
-    rev: v1.4
-    hooks:
-      - id: autoflake
-        args: ["--in-place", "--remove-all-unused-imports"]
-  - repo: https://github.com/psf/black
-    rev: 22.3.0
-    hooks:
-      - id: black
-  - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
-    hooks:
-      - id: flake8
-        additional_dependencies: [flake8-typing-imports>=1.9.0]
-  - repo: https://github.com/tlambert03/napari-plugin-checks
-    rev: v0.2.0
-    hooks:
-      - id: napari-plugin-checks
-  # https://mypy.readthedocs.io/en/stable/introduction.html
-  # you may wish to add this as well!
-  # - repo: https://github.com/pre-commit/mirrors-mypy
-  #   rev: v0.910-1
-  #   hooks:
-  #     - id: mypy
+repos:
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
+    hooks:
+      - id: check-docstring-first
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+        exclude: ^.napari-hub/*
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.10.1
+    hooks:
+      - id: isort
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v2.32.1
+    hooks:
+      - id: pyupgrade
+        args: [--py38-plus, --keep-runtime-typing]
+  - repo: https://github.com/myint/autoflake
+    rev: v1.4
+    hooks:
+      - id: autoflake
+        args: ["--in-place", "--remove-all-unused-imports"]
+  - repo: https://github.com/psf/black
+    rev: 22.3.0
+    hooks:
+      - id: black
+  - repo: https://github.com/PyCQA/flake8
+    rev: 4.0.1
+    hooks:
+      - id: flake8
+        additional_dependencies: [flake8-typing-imports>=1.9.0]
+  - repo: https://github.com/tlambert03/napari-plugin-checks
+    rev: v0.2.0
+    hooks:
+      - id: napari-plugin-checks
+  # https://mypy.readthedocs.io/en/stable/introduction.html
+  # you may wish to add this as well!
+  # - repo: https://github.com/pre-commit/mirrors-mypy
+  #   rev: v0.910-1
+  #   hooks:
+  #     - id: mypy
```

### Comparing `napari-aphid-1.1.6/LICENSE` & `napari-aphid-1.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-
-Copyright (c) 2022, Herearii Metuarea
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of napari-aphid nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+Copyright (c) 2022, Herearii Metuarea
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of napari-aphid nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `napari-aphid-1.1.6/setup.cfg` & `napari-aphid-1.1.7/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,115 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206e 6170 6172 692d 6170 6869 640d   = napari-aphid.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e31 2e36  .version = 1.1.6
-00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
-00000040: 4120 706c 7567 696e 2074 6f20 636c 6173  A plugin to clas
-00000050: 7369 6679 2061 7068 6964 7320 6279 2073  sify aphids by s
-00000060: 7461 6765 206f 6620 6465 7665 6c6f 706d  tage of developm
-00000070: 656e 742e 0d0a 6c6f 6e67 5f64 6573 6372  ent...long_descr
-00000080: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
-00000090: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
-000000a0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
-000000b0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
-000000c0: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
-000000d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000000e0: 6d2f 6865 7265 6172 6969 6d2f 6e61 7061  m/hereariim/napa
-000000f0: 7269 2d61 7068 6964 0d0a 6175 7468 6f72  ri-aphid..author
-00000100: 203d 2048 6572 6561 7269 6920 4d65 7475   = Herearii Metu
-00000110: 6172 6561 0d0a 6175 7468 6f72 5f65 6d61  area..author_ema
-00000120: 696c 203d 2068 6572 6561 7269 692e 6d65  il = herearii.me
-00000130: 7475 6172 6561 4067 6d61 696c 2e63 6f6d  tuarea@gmail.com
-00000140: 0d0a 6c69 6365 6e73 6520 3d20 4253 442d  ..license = BSD-
-00000150: 332d 436c 6175 7365 0d0a 6c69 6365 6e73  3-Clause..licens
-00000160: 655f 6669 6c65 7320 3d20 4c49 4345 4e53  e_files = LICENS
-00000170: 450d 0a63 6c61 7373 6966 6965 7273 203d  E..classifiers =
-00000180: 200d 0a09 4465 7665 6c6f 706d 656e 7420   ...Development 
-00000190: 5374 6174 7573 203a 3a20 3220 2d20 5072  Status :: 2 - Pr
-000001a0: 652d 416c 7068 610d 0a09 4672 616d 6577  e-Alpha...Framew
-000001b0: 6f72 6b20 3a3a 206e 6170 6172 690d 0a09  ork :: napari...
-000001c0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-000001d0: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
-000001e0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-000001f0: 2041 7070 726f 7665 6420 3a3a 2042 5344   Approved :: BSD
-00000200: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-00000210: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000220: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
-00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000240: 7561 6765 203a 3a20 5079 7468 6f6e 0d0a  uage :: Python..
-00000250: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000260: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000270: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
-00000280: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000290: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
-000002a0: 6c79 0d0a 0950 726f 6772 616d 6d69 6e67  ly...Programming
-000002b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002c0: 686f 6e20 3a3a 2033 2e38 0d0a 0950 726f  hon :: 3.8...Pro
-000002d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002f0: 2e39 0d0a 0950 726f 6772 616d 6d69 6e67  .9...Programming
-00000300: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000310: 686f 6e20 3a3a 2033 2e31 300d 0a09 546f  hon :: 3.10...To
-00000320: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-00000330: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
-00000340: 2049 6d61 6765 2050 726f 6365 7373 696e   Image Processin
-00000350: 670d 0a70 726f 6a65 6374 5f75 726c 7320  g..project_urls 
-00000360: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
-00000370: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000380: 622e 636f 6d2f 6865 7265 6172 6969 6d2f  b.com/hereariim/
-00000390: 6e61 7061 7269 2d61 7068 6964 2f69 7373  napari-aphid/iss
-000003a0: 7565 730d 0a09 446f 6375 6d65 6e74 6174  ues...Documentat
-000003b0: 696f 6e20 3d20 6874 7470 733a 2f2f 6769  ion = https://gi
-000003c0: 7468 7562 2e63 6f6d 2f68 6572 6561 7269  thub.com/hereari
-000003d0: 696d 2f6e 6170 6172 692d 6170 6869 6423  im/napari-aphid#
-000003e0: 5245 4144 4d45 2e6d 640d 0a09 536f 7572  README.md...Sour
-000003f0: 6365 2043 6f64 6520 3d20 6874 7470 733a  ce Code = https:
-00000400: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6572  //github.com/her
-00000410: 6561 7269 696d 2f6e 6170 6172 692d 6170  eariim/napari-ap
-00000420: 6869 640d 0a09 5573 6572 2053 7570 706f  hid...User Suppo
-00000430: 7274 203d 2068 7474 7073 3a2f 2f67 6974  rt = https://git
-00000440: 6875 622e 636f 6d2f 6865 7265 6172 6969  hub.com/herearii
-00000450: 6d2f 6e61 7061 7269 2d61 7068 6964 2f69  m/napari-aphid/i
-00000460: 7373 7565 730d 0a0d 0a5b 6f70 7469 6f6e  ssues....[option
-00000470: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
-00000480: 696e 643a 0d0a 696e 7374 616c 6c5f 7265  ind:..install_re
-00000490: 7175 6972 6573 203d 200d 0a09 6e61 7061  quires = ...napa
-000004a0: 7269 0d0a 096e 756d 7079 0d0a 096d 6167  ri...numpy...mag
-000004b0: 6963 6775 690d 0a09 7174 7079 0d0a 096f  icgui...qtpy...o
-000004c0: 7065 6e63 762d 7079 7468 6f6e 2d68 6561  pencv-python-hea
-000004d0: 646c 6573 730d 0a09 7363 696b 6974 2d6c  dless...scikit-l
-000004e0: 6561 726e 0d0a 0973 6369 6b69 742d 696d  earn...scikit-im
-000004f0: 6167 650d 0a09 6835 7079 0d0a 096d 6174  age...h5py...mat
-00000500: 706c 6f74 6c69 620d 0a09 7061 6e64 6173  plotlib...pandas
-00000510: 0d0a 0973 6369 7079 0d0a 7079 7468 6f6e  ...scipy..python
-00000520: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000530: 380d 0a69 6e63 6c75 6465 5f70 6163 6b61  8..include_packa
-00000540: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
-00000550: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000560: 093d 7372 630d 0a0d 0a5b 6f70 7469 6f6e  .=src....[option
-00000570: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000580: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000590: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-000005a0: 706f 696e 7473 5d0d 0a6e 6170 6172 692e  points]..napari.
-000005b0: 6d61 6e69 6665 7374 203d 200d 0a09 6e61  manifest = ...na
-000005c0: 7061 7269 2d61 7068 6964 203d 206e 6170  pari-aphid = nap
-000005d0: 6172 695f 6170 6869 643a 6e61 7061 7269  ari_aphid:napari
-000005e0: 2e79 616d 6c0d 0a0d 0a5b 6f70 7469 6f6e  .yaml....[option
-000005f0: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
-00000600: 5d0d 0a74 6573 7469 6e67 203d 200d 0a09  ]..testing = ...
-00000610: 746f 780d 0a09 7079 7465 7374 2020 2320  tox...pytest  # 
-00000620: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-00000630: 6573 742e 6f72 672f 656e 2f6c 6174 6573  est.org/en/lates
-00000640: 742f 636f 6e74 656e 7473 2e68 746d 6c0d  t/contents.html.
-00000650: 0a09 7079 7465 7374 2d63 6f76 2020 2320  ..pytest-cov  # 
-00000660: 6874 7470 733a 2f2f 7079 7465 7374 2d63  https://pytest-c
-00000670: 6f76 2e72 6561 6474 6865 646f 6373 2e69  ov.readthedocs.i
-00000680: 6f2f 656e 2f6c 6174 6573 742f 0d0a 0970  o/en/latest/...p
-00000690: 7974 6573 742d 7174 2020 2320 6874 7470  ytest-qt  # http
-000006a0: 733a 2f2f 7079 7465 7374 2d71 742e 7265  s://pytest-qt.re
-000006b0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-000006c0: 6c61 7465 7374 2f0d 0a09 6e61 7061 7269  latest/...napari
-000006d0: 0d0a 0970 7971 7435 0d0a 0d0a 5b6f 7074  ...pyqt5....[opt
-000006e0: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-000006f0: 615d 0d0a 6e61 7061 7269 2d61 7068 6964  a]..napari-aphid
-00000700: 203d 206e 6170 6172 692e 7961 6d6c 0d0a   = napari.yaml..
-00000710: 0d0a 5b74 6573 7470 7970 695d 0d0a 7573  ..[testpypi]..us
-00000720: 6572 6e61 6d65 203d 2022 686d 6574 7561  ername = "hmetua
-00000730: 220d 0a70 6173 7377 6f72 6420 3d20 2253  "..password = "S
-00000740: 6f75 736d 6172 696e 3133 2b22 0d0a 0d0a  ousmarin13+"....
-00000750: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000760: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000770: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6e61 7061 7269 2d61 7068 6964 0a76  = napari-aphid.v
+00000020: 6572 7369 6f6e 203d 2031 2e31 2e37 0a64  ersion = 1.1.7.d
+00000030: 6573 6372 6970 7469 6f6e 203d 2041 2070  escription = A p
+00000040: 6c75 6769 6e20 746f 2063 6c61 7373 6966  lugin to classif
+00000050: 7920 6170 6869 6473 2062 7920 7374 6167  y aphids by stag
+00000060: 6520 6f66 2064 6576 656c 6f70 6d65 6e74  e of development
+00000070: 2e0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+00000080: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+00000090: 452e 6d64 0a6c 6f6e 675f 6465 7363 7269  E.md.long_descri
+000000a0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+000000b0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+000000c0: 776e 0a75 726c 203d 2068 7474 7073 3a2f  wn.url = https:/
+000000d0: 2f67 6974 6875 622e 636f 6d2f 6865 7265  /github.com/here
+000000e0: 6172 6969 6d2f 6e61 7061 7269 2d61 7068  ariim/napari-aph
+000000f0: 6964 0a61 7574 686f 7220 3d20 4865 7265  id.author = Here
+00000100: 6172 6969 204d 6574 7561 7265 610a 6175  arii Metuarea.au
+00000110: 7468 6f72 5f65 6d61 696c 203d 2068 6572  thor_email = her
+00000120: 6561 7269 692e 6d65 7475 6172 6561 4067  earii.metuarea@g
+00000130: 6d61 696c 2e63 6f6d 0a6c 6963 656e 7365  mail.com.license
+00000140: 203d 2042 5344 2d33 2d43 6c61 7573 650a   = BSD-3-Clause.
+00000150: 6c69 6365 6e73 655f 6669 6c65 7320 3d20  license_files = 
+00000160: 4c49 4345 4e53 450a 636c 6173 7369 6669  LICENSE.classifi
+00000170: 6572 7320 3d20 0a09 4465 7665 6c6f 706d  ers = ..Developm
+00000180: 656e 7420 5374 6174 7573 203a 3a20 3220  ent Status :: 2 
+00000190: 2d20 5072 652d 416c 7068 610a 0946 7261  - Pre-Alpha..Fra
+000001a0: 6d65 776f 726b 203a 3a20 6e61 7061 7269  mework :: napari
+000001b0: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+000001c0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+000001d0: 730a 094c 6963 656e 7365 203a 3a20 4f53  s..License :: OS
+000001e0: 4920 4170 7072 6f76 6564 203a 3a20 4253  I Approved :: BS
+000001f0: 4420 4c69 6365 6e73 650a 094f 7065 7261  D License..Opera
+00000200: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00000210: 5320 496e 6465 7065 6e64 656e 740a 0950  S Independent..P
+00000220: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000230: 6167 6520 3a3a 2050 7974 686f 6e0a 0950  age :: Python..P
+00000240: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000250: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000260: 2033 0a09 5072 6f67 7261 6d6d 696e 6720   3..Programming 
+00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000280: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790a  on :: 3 :: Only.
+00000290: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002b0: 3a3a 2033 2e38 0a09 5072 6f67 7261 6d6d  :: 3.8..Programm
+000002c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002d0: 5079 7468 6f6e 203a 3a20 332e 390a 0950  Python :: 3.9..P
+000002e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000300: 2033 2e31 300a 0954 6f70 6963 203a 3a20   3.10..Topic :: 
+00000310: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
+00000320: 6565 7269 6e67 203a 3a20 496d 6167 6520  eering :: Image 
+00000330: 5072 6f63 6573 7369 6e67 0a70 726f 6a65  Processing.proje
+00000340: 6374 5f75 726c 7320 3d20 0a09 4275 6720  ct_urls = ..Bug 
+00000350: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+00000360: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6572  //github.com/her
+00000370: 6561 7269 696d 2f6e 6170 6172 692d 6170  eariim/napari-ap
+00000380: 6869 642f 6973 7375 6573 0a09 446f 6375  hid/issues..Docu
+00000390: 6d65 6e74 6174 696f 6e20 3d20 6874 7470  mentation = http
+000003a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+000003b0: 6572 6561 7269 696d 2f6e 6170 6172 692d  ereariim/napari-
+000003c0: 6170 6869 6423 5245 4144 4d45 2e6d 640a  aphid#README.md.
+000003d0: 0953 6f75 7263 6520 436f 6465 203d 2068  .Source Code = h
+000003e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000003f0: 6d2f 6865 7265 6172 6969 6d2f 6e61 7061  m/hereariim/napa
+00000400: 7269 2d61 7068 6964 0a09 5573 6572 2053  ri-aphid..User S
+00000410: 7570 706f 7274 203d 2068 7474 7073 3a2f  upport = https:/
+00000420: 2f67 6974 6875 622e 636f 6d2f 6865 7265  /github.com/here
+00000430: 6172 6969 6d2f 6e61 7061 7269 2d61 7068  ariim/napari-aph
+00000440: 6964 2f69 7373 7565 730a 0a5b 6f70 7469  id/issues..[opti
+00000450: 6f6e 735d 0a70 6163 6b61 6765 7320 3d20  ons].packages = 
+00000460: 6669 6e64 3a0a 696e 7374 616c 6c5f 7265  find:.install_re
+00000470: 7175 6972 6573 203d 200a 096e 6170 6172  quires = ..napar
+00000480: 690a 096e 756d 7079 0a09 6d61 6769 6367  i..numpy..magicg
+00000490: 7569 0a09 7174 7079 0a09 6f70 656e 6376  ui..qtpy..opencv
+000004a0: 2d70 7974 686f 6e2d 6865 6164 6c65 7373  -python-headless
+000004b0: 0a09 7363 696b 6974 2d6c 6561 726e 0a09  ..scikit-learn..
+000004c0: 7363 696b 6974 2d69 6d61 6765 0a09 6835  scikit-image..h5
+000004d0: 7079 0a09 6d61 7470 6c6f 746c 6962 0a09  py..matplotlib..
+000004e0: 7061 6e64 6173 0a09 7363 6970 790a 7079  pandas..scipy.py
+000004f0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000500: 3e3d 332e 380a 696e 636c 7564 655f 7061  >=3.8.include_pa
+00000510: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
+00000520: 650a 7061 636b 6167 655f 6469 7220 3d20  e.package_dir = 
+00000530: 0a09 3d73 7263 0a0a 5b6f 7074 696f 6e73  ..=src..[options
+00000540: 2e70 6163 6b61 6765 732e 6669 6e64 5d0a  .packages.find].
+00000550: 7768 6572 6520 3d20 7372 630a 0a5b 6f70  where = src..[op
+00000560: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+00000570: 7473 5d0a 6e61 7061 7269 2e6d 616e 6966  ts].napari.manif
+00000580: 6573 7420 3d20 0a09 6e61 7061 7269 2d61  est = ..napari-a
+00000590: 7068 6964 203d 206e 6170 6172 695f 6170  phid = napari_ap
+000005a0: 6869 643a 6e61 7061 7269 2e79 616d 6c0a  hid:napari.yaml.
+000005b0: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+000005c0: 5f72 6571 7569 7265 5d0a 7465 7374 696e  _require].testin
+000005d0: 6720 3d20 0a09 746f 780a 0970 7974 6573  g = ..tox..pytes
+000005e0: 7420 2023 2068 7474 7073 3a2f 2f64 6f63  t  # https://doc
+000005f0: 732e 7079 7465 7374 2e6f 7267 2f65 6e2f  s.pytest.org/en/
+00000600: 6c61 7465 7374 2f63 6f6e 7465 6e74 732e  latest/contents.
+00000610: 6874 6d6c 0a09 7079 7465 7374 2d63 6f76  html..pytest-cov
+00000620: 2020 2320 6874 7470 733a 2f2f 7079 7465    # https://pyte
+00000630: 7374 2d63 6f76 2e72 6561 6474 6865 646f  st-cov.readthedo
+00000640: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000650: 0a09 7079 7465 7374 2d71 7420 2023 2068  ..pytest-qt  # h
+00000660: 7474 7073 3a2f 2f70 7974 6573 742d 7174  ttps://pytest-qt
+00000670: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000680: 656e 2f6c 6174 6573 742f 0a09 6e61 7061  en/latest/..napa
+00000690: 7269 0a09 7079 7174 350a 0a5b 6f70 7469  ri..pyqt5..[opti
+000006a0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
+000006b0: 5d0a 6e61 7061 7269 2d61 7068 6964 203d  ].napari-aphid =
+000006c0: 206e 6170 6172 692e 7961 6d6c 0a0a 5b74   napari.yaml..[t
+000006d0: 6573 7470 7970 695d 0a75 7365 726e 616d  estpypi].usernam
+000006e0: 6520 3d20 2268 6d65 7475 6122 0a70 6173  e = "hmetua".pas
+000006f0: 7377 6f72 6420 3d20 2253 6f75 736d 6172  sword = "Sousmar
+00000700: 696e 3133 2b22 0a0a 5b65 6767 5f69 6e66  in13+"..[egg_inf
+00000710: 6f5d 0a74 6167 5f62 7569 6c64 203d 200a  o].tag_build = .
+00000720: 7461 675f 6461 7465 203d 2030 0a0a       tag_date = 0..
```

### Comparing `napari-aphid-1.1.6/setup.py` & `napari-aphid-1.1.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""Setup for the python package.""" 
-from setuptools import setup, find_packages
-with open("README.md", "r", encoding="utf-8") as fh: 
-     long_description = fh.read() 
-setup(    
-    author="Herearii Metuarea",    
-    author_email="herearii.metuarea@gmail.com",
-    name='napari-aphid', 
-    description='A plugin to classify aphids by stage of development.',  
-    version="1.1.6",    
-    long_description=long_description, 
-    long_description_content_type="text/markdown",  
-    url='https://github.com/hereariim/napari-aphid', 
-    packages=find_packages(),
-    python_requires=">=3.8",
-    install_requires=['napari',
-    'numpy',
-    'magicgui',
-    'qtpy',
-    'opencv-python-headless',
-    'scikit-learn',
-    'scikit-image',
-    'h5py',
-    'matplotlib',
-    'pandas',
-    'scipy'], 
-    classifiers=[ 'Development Status :: 2 - Pre-Alpha',
-    'Framework :: napari',
-    'Intended Audience :: Developers',
-    'License :: OSI Approved :: BSD License',
-    'Operating System :: OS Independent',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Topic :: Scientific/Engineering :: Image Processing',
-                ],
+"""Setup for the python package.""" 
+from setuptools import setup, find_packages
+with open("README.md", "r", encoding="utf-8") as fh: 
+     long_description = fh.read() 
+setup(    
+    author="Herearii Metuarea",    
+    author_email="herearii.metuarea@gmail.com",
+    name='napari-aphid', 
+    description='A plugin to classify aphids by stage of development.',  
+    version="1.1.7",    
+    long_description=long_description, 
+    long_description_content_type="text/markdown",  
+    url='https://github.com/hereariim/napari-aphid', 
+    packages=find_packages(),
+    python_requires=">=3.8",
+    install_requires=['napari',
+    'numpy',
+    'magicgui',
+    'qtpy',
+    'opencv-python-headless',
+    'scikit-learn',
+    'scikit-image',
+    'h5py',
+    'matplotlib',
+    'pandas',
+    'scipy'], 
+    classifiers=[ 'Development Status :: 2 - Pre-Alpha',
+    'Framework :: napari',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: BSD License',
+    'Operating System :: OS Independent',
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Topic :: Scientific/Engineering :: Image Processing',
+                ],
      )
```

### Comparing `napari-aphid-1.1.6/src/napari_aphid/RunBatch.ijm` & `napari-aphid-1.1.7/src/napari_aphid/RunBatch.ijm`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-t1 = getTime();
-outputDataset = getArgument();
-compressionLevel = 0;
-
-dir = getArgument();
-subfolders = getFileList(dir);
-print("\\Clear");
-setBatchMode(true);
-for (i = 0; i < subfolders.length; i++) {
-	showProgress(i+1, subfolders.length);
-	print("Entering folder " + subfolders[i]);
-	folder = dir + subfolders[i];
-	files = getFileList(folder);
-	for (f = 0; f < files.length; f++) {
-		file = files[f];
-		filesString = String.join(files, ",");
-		if (endsWith(file, ".h5")) continue;
-		out = replace(file, "png", "h5");
-		if (indexOf(filesString, out)>-1) continue;
-		print("Processing file " + file);
-		open(folder + file);
-		outputPath = folder + File.nameWithoutExtension + ".h5";			
-		exportArgs = "select=" + outputPath + " datasetname=" + outputDataset + " compressionlevel=" + compressionLevel;
-		run("Export HDF5", exportArgs);
-		close("*");
-		if (f%10==0) run("Collect Garbage");
-	}
-}
-setBatchMode(false);
-t2 = getTime();
-print("batch convert to h5 took: " + (t2-t1)/1000 + "s");
+t1 = getTime();
+outputDataset = getArgument();
+compressionLevel = 0;
+
+dir = getArgument();
+subfolders = getFileList(dir);
+print("\\Clear");
+setBatchMode(true);
+for (i = 0; i < subfolders.length; i++) {
+	showProgress(i+1, subfolders.length);
+	print("Entering folder " + subfolders[i]);
+	folder = dir + subfolders[i];
+	files = getFileList(folder);
+	for (f = 0; f < files.length; f++) {
+		file = files[f];
+		filesString = String.join(files, ",");
+		if (endsWith(file, ".h5")) continue;
+		out = replace(file, "png", "h5");
+		if (indexOf(filesString, out)>-1) continue;
+		print("Processing file " + file);
+		open(folder + file);
+		outputPath = folder + File.nameWithoutExtension + ".h5";			
+		exportArgs = "select=" + outputPath + " datasetname=" + outputDataset + " compressionlevel=" + compressionLevel;
+		run("Export HDF5", exportArgs);
+		close("*");
+		if (f%10==0) run("Collect Garbage");
+	}
+}
+setBatchMode(false);
+t2 = getTime();
+print("batch convert to h5 took: " + (t2-t1)/1000 + "s");
```

### Comparing `napari-aphid-1.1.6/src/napari_aphid.egg-info/SOURCES.txt` & `napari-aphid-1.1.7/src/napari_aphid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

