# Comparing `tmp/pydantic-openapi-helper-0.2.7.tar.gz` & `tmp/pydantic-openapi-helper-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydantic-openapi-helper-0.2.7.tar", last modified: Wed May 12 01:37:44 2021, max compression
+gzip compressed data, was "dist/pydantic-openapi-helper-0.2.9.tar", last modified: Wed Feb  9 22:34:57 2022, max compression
```

## Comparing `pydantic-openapi-helper-0.2.7.tar` & `pydantic-openapi-helper-0.2.9.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/.dependabot/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/.dependabot/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      374 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     3668 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)     7115 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     5021 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    11802 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper/inheritance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      793 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/pydantic_openapi_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      987 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-12 01:37:44.000000 pydantic-openapi-helper-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-05-12 01:36:59.000000 pydantic-openapi-helper-0.2.7/tests/example_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/docs/_build/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     3668 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (121)     7115 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5021 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11802 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper/inheritance.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/pydantic_openapi_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 22:34:57.000000 pydantic-openapi-helper-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-02-09 22:33:50.000000 pydantic-openapi-helper-0.2.9/tests/example_test.py
```

### Comparing `pydantic-openapi-helper-0.2.7/.github/workflows/ci.yaml` & `pydantic-openapi-helper-0.2.9/.github/workflows/ci.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -23,20 +23,37 @@
           python -m pip install --upgrade pip
           pip install -r requirements.txt
           pip install -r dev-requirements.txt
       - name: install semantic-release
         run:
           npm install @semantic-release/exec
       - name: run semantic release
-        run:
-          npx semantic-release
+        id: new_release
+        run: |
+          nextRelease="`npx semantic-release@^17.0.0 --dryRun | grep -oP 'Published release \K.*? ' || true`"
+          npx semantic-release@^17.0.0
+          echo "::set-output name=tag::$nextRelease"
         env:
-          GITHUB_TOKEN: ${{ secrets.GH_TOKEN }}
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           PYPI_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
           PYPI_USERNAME: ${{ secrets.PYPI_USERNAME }}
+      - name: sleep for 5 minutes for PyPI update
+        if: contains(steps.new_release.outputs.tag, '.')
+        run: sleep 300s
+        shell: bash
+      - name: Update honeybee-schema
+        if: contains(steps.new_release.outputs.tag, '.')
+        env:
+          DISPATCH_REPO: ladybug-tools/honeybee-schema
+          DEPS_TOKEN: ${{ secrets.DEPS_UPDATING }}
+        run: |
+          curl -X POST https://api.github.com/repos/$DISPATCH_REPO/dispatches \
+          -H "Accept: application/vnd.github.everest-preview+json" \
+          -d '{"event_type": "honeybee_schema_release", "client_payload": {"version": "${{ steps.new_release.outputs.tag }}"}}' \
+          -u ladybugbot:$DEPS_TOKEN
 
   docs:
     name: Generate docs
     runs-on: ubuntu-latest
     if: github.ref == 'refs/heads/master' && github.repository_owner == 'ladybug-tools'
     steps:
       - uses: actions/checkout@v2
@@ -50,13 +67,13 @@
           pip install -r dev-requirements.txt
           sphinx-apidoc -f -e -d 4 -o ./docs/modules ./pydantic_openapi_helper
           sphinx-build -b html ./docs ./docs/_build
       - name: deploy to github pages
         uses: peaceiris/actions-gh-pages@v3
         with:
           # this will use ladybugbot token
-          github_token: ${{ secrets.GH_TOKEN }}
+          github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_branch: gh-pages
           publish_dir: docs/_build/
           force_orphan: true
           keep_files: false
           full_commit_message: 'deploy: update docs'
```

### Comparing `pydantic-openapi-helper-0.2.7/LICENSE` & `pydantic-openapi-helper-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-openapi-helper-0.2.7/PKG-INFO` & `pydantic-openapi-helper-0.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: pydantic-openapi-helper
-Version: 0.2.7
+Version: 0.2.9
 Summary: A small module to add additional post-processing to the OpenAPI schemas that are generated by Pydantic.
 Home-page: https://github.com/ladybug-tools/pydantic-openapi-helper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: MIT
-Description: [![Build Status](https://travis-ci.com/ladybug-tools/pydantic-openapi-helper.svg?branch=master)](https://travis-ci.com/ladybug-tools/pydantic-openapi-helper)
-        
-        [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
-        
-        # pydantic-openapi-helper
-        
-        A small module to add additional post-processing to the OpenAPI schemas that are generated
-        by Pydantic.
-        
-        This module is designed to work with Ladybug Tools schema libraries such as
-        [honeybee-schema](https://github.com/ladybug-tools/honeybee-schema/),
-        [dragonfly-schema](https://github.com/ladybug-tools/dragonfly-schema/) and
-        [queenbee](https://github.com/ladybug-tools/queenbee/) but might be also helpful for
-        other projects.
-        
-        The most important feature of the library is to generate an OpenAPI schema to use
-        polymorphism. It adds referenced values to subclasses using allOf field as explained in
-        this post: https://swagger.io/docs/specification/data-models/inheritance-and-polymorphism
-        
-        We are not intending to support the development for make this library work universally
-        but you are more than welcome to fork and make your own version of the library.
-        
-        
-        ## installation
-        
-        `python3 -m pip install pydantic-openapi-helper`
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Build Status](https://travis-ci.com/ladybug-tools/pydantic-openapi-helper.svg?branch=master)](https://travis-ci.com/ladybug-tools/pydantic-openapi-helper)
+
+[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
+
+# pydantic-openapi-helper
+
+A small module to add additional post-processing to the OpenAPI schemas that are generated
+by Pydantic.
+
+This module is designed to work with Ladybug Tools schema libraries such as
+[honeybee-schema](https://github.com/ladybug-tools/honeybee-schema/),
+[dragonfly-schema](https://github.com/ladybug-tools/dragonfly-schema/) and
+[queenbee](https://github.com/ladybug-tools/queenbee/) but might be also helpful for
+other projects.
+
+The most important feature of the library is to generate an OpenAPI schema to use
+polymorphism. It adds referenced values to subclasses using allOf field as explained in
+this post: https://swagger.io/docs/specification/data-models/inheritance-and-polymorphism
+
+We are not intending to support the development for make this library work universally
+but you are more than welcome to fork and make your own version of the library.
+
+
+## installation
+
+`python3 -m pip install pydantic-openapi-helper`
+
+
```

### Comparing `pydantic-openapi-helper-0.2.7/README.md` & `pydantic-openapi-helper-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-openapi-helper-0.2.7/docs/_static/custom.css` & `pydantic-openapi-helper-0.2.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `pydantic-openapi-helper-0.2.7/docs/_templates/layout.html` & `pydantic-openapi-helper-0.2.9/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pydantic-openapi-helper-0.2.7/docs/conf.py` & `pydantic-openapi-helper-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydantic-openapi-helper-0.2.7/pydantic_openapi_helper/core.py` & `pydantic-openapi-helper-0.2.9/pydantic_openapi_helper/core.py`

 * *Files identical despite different names*

### Comparing `pydantic-openapi-helper-0.2.7/pydantic_openapi_helper/helper.py` & `pydantic-openapi-helper-0.2.9/pydantic_openapi_helper/helper.py`

 * *Files identical despite different names*

### Comparing `pydantic-openapi-helper-0.2.7/pydantic_openapi_helper/inheritance.py` & `pydantic-openapi-helper-0.2.9/pydantic_openapi_helper/inheritance.py`

 * *Files identical despite different names*

### Comparing `pydantic-openapi-helper-0.2.7/pydantic_openapi_helper.egg-info/PKG-INFO` & `pydantic-openapi-helper-0.2.9/pydantic_openapi_helper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: pydantic-openapi-helper
-Version: 0.2.7
+Version: 0.2.9
 Summary: A small module to add additional post-processing to the OpenAPI schemas that are generated by Pydantic.
 Home-page: https://github.com/ladybug-tools/pydantic-openapi-helper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: MIT
-Description: [![Build Status](https://travis-ci.com/ladybug-tools/pydantic-openapi-helper.svg?branch=master)](https://travis-ci.com/ladybug-tools/pydantic-openapi-helper)
-        
-        [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
-        
-        # pydantic-openapi-helper
-        
-        A small module to add additional post-processing to the OpenAPI schemas that are generated
-        by Pydantic.
-        
-        This module is designed to work with Ladybug Tools schema libraries such as
-        [honeybee-schema](https://github.com/ladybug-tools/honeybee-schema/),
-        [dragonfly-schema](https://github.com/ladybug-tools/dragonfly-schema/) and
-        [queenbee](https://github.com/ladybug-tools/queenbee/) but might be also helpful for
-        other projects.
-        
-        The most important feature of the library is to generate an OpenAPI schema to use
-        polymorphism. It adds referenced values to subclasses using allOf field as explained in
-        this post: https://swagger.io/docs/specification/data-models/inheritance-and-polymorphism
-        
-        We are not intending to support the development for make this library work universally
-        but you are more than welcome to fork and make your own version of the library.
-        
-        
-        ## installation
-        
-        `python3 -m pip install pydantic-openapi-helper`
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Build Status](https://travis-ci.com/ladybug-tools/pydantic-openapi-helper.svg?branch=master)](https://travis-ci.com/ladybug-tools/pydantic-openapi-helper)
+
+[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
+
+# pydantic-openapi-helper
+
+A small module to add additional post-processing to the OpenAPI schemas that are generated
+by Pydantic.
+
+This module is designed to work with Ladybug Tools schema libraries such as
+[honeybee-schema](https://github.com/ladybug-tools/honeybee-schema/),
+[dragonfly-schema](https://github.com/ladybug-tools/dragonfly-schema/) and
+[queenbee](https://github.com/ladybug-tools/queenbee/) but might be also helpful for
+other projects.
+
+The most important feature of the library is to generate an OpenAPI schema to use
+polymorphism. It adds referenced values to subclasses using allOf field as explained in
+this post: https://swagger.io/docs/specification/data-models/inheritance-and-polymorphism
+
+We are not intending to support the development for make this library work universally
+but you are more than welcome to fork and make your own version of the library.
+
+
+## installation
+
+`python3 -m pip install pydantic-openapi-helper`
+
+
```

### Comparing `pydantic-openapi-helper-0.2.7/pydantic_openapi_helper.egg-info/SOURCES.txt` & `pydantic-openapi-helper-0.2.9/pydantic_openapi_helper.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 LICENSE
 README.md
 deploy.sh
 dev-requirements.txt
 requirements.txt
 setup.cfg
 setup.py
-.dependabot/config.yml
+.github/dependabot.yml
 .github/workflows/ci.yaml
 docs/README.md
 docs/conf.py
 docs/index.rst
 docs/modules.rst
 docs/_build/.nojekyll
 docs/_build/README.md
```

### Comparing `pydantic-openapi-helper-0.2.7/setup.py` & `pydantic-openapi-helper-0.2.9/setup.py`

 * *Files identical despite different names*

