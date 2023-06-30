# Comparing `tmp/jupyterlab_templates-0.4.0.tar.gz` & `tmp/jupyterlab_templates-0.4.1.tar.gz`

## Comparing `jupyterlab_templates-0.4.0.tar` & `jupyterlab_templates-0.4.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/.bumpversion.cfg
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/.gitattributes
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/MANIFEST.in
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/Makefile
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/setup.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/.eslintrc.js
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/babel.config.js
--rw-r--r--   0        0        0    37425 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/icon.png
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/jest.config.js
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/package.json
--rw-r--r--   0        0        0   352237 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/yarn.lock
--rw-r--r--   0        0        0    55537 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/src/index.js
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/style/icon.svg
--rw-r--r--   0        0        0    50291 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/style/index.css
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/tests/activate.test.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/tests/assetsTransformer.js
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/tests/export.test.js
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/tests/fileMock.js
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/js/tests/styleMock.js
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/_version.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/extension.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/extension/install.json
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/extension/jupyterlab_templates.json
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/extension/notebook_templates/jupyterlab_templates/Sample.ipynb
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/package.json
--rw-r--r--   0        0        0   105973 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/static/568.7c3fb82db0068d774682.js
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/static/873.6ea510b34d81274bc9b0.js
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/static/remoteEntry.16bfd2a294ef1e5cdaee.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/static/style.js
--rw-r--r--   0        0        0    19725 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/templates/jupyterlab_templates/Sample.ipynb
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/tests/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/tests/test_all.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/tests/test_extension.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/jupyterlab_templates/tests/test_init.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/.gitignore
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/AUTHORS
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/LICENSE
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/NOTICE
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/README.md
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    17641 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/.bumpversion.cfg
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/.gitattributes
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/MANIFEST.in
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/Makefile
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/setup.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/.eslintrc.js
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/babel.config.js
+-rw-r--r--   0        0        0    37425 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/icon.png
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/jest.config.js
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/package.json
+-rw-r--r--   0        0        0   353085 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/yarn.lock
+-rw-r--r--   0        0        0    55949 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/src/index.js
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/style/icon.svg
+-rw-r--r--   0        0        0    50291 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/style/index.css
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/tests/activate.test.js
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/tests/assetsTransformer.js
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/tests/export.test.js
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/tests/fileMock.js
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/js/tests/styleMock.js
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/_version.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/extension.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/extension/install.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/extension/jupyterlab_templates.json
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/extension/notebook_templates/jupyterlab_templates/Sample.ipynb
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/package.json
+-rw-r--r--   0        0        0   106105 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/static/568.bca76f9a3703a686ab31.js
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/static/873.6ea510b34d81274bc9b0.js
+-rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/static/remoteEntry.dc333b99e046544e4b16.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/static/style.js
+-rw-r--r--   0        0        0    19725 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/templates/jupyterlab_templates/Sample.ipynb
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/tests/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/tests/test_all.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/tests/test_extension.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/jupyterlab_templates/tests/test_init.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/.gitignore
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/AUTHORS
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/LICENSE
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/NOTICE
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/README.md
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    18037 2020-02-02 00:00:00.000000 jupyterlab_templates-0.4.1/PKG-INFO
```

### Comparing `jupyterlab_templates-0.4.0/.bumpversion.cfg` & `jupyterlab_templates-0.4.1/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.0
+current_version = 0.4.1
 commit = True
 tag = False
 
 [bumpversion:file:jupyterlab_templates/_version.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `jupyterlab_templates-0.4.0/CONTRIBUTING.md` & `jupyterlab_templates-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/MANIFEST.in` & `jupyterlab_templates-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/Makefile` & `jupyterlab_templates-0.4.1/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install:  ## install to site-packages
 	python -m pip install .
 
 ###########
 # Testing #
 ###########
 testpy: ## Clean and Make unit tests
-	python -m pytest -v jupyterlab_templates/tests --junitxml=python_junit.xml --cov=jupyterlab_templates --cov-report=xml:.coverage.xml --cov-branch --cov-fail-under=20 --cov-report term-missing
+	python -m pytest -v jupyterlab_templates/tests --junitxml=junit.xml --cov=jupyterlab_templates --cov-report=xml:.coverage.xml --cov-branch --cov-fail-under=20 --cov-report term-missing
 
 testjs: ## Clean and Make js tests
 	cd js; yarn test
 
 test: tests
 tests: testpy testjs ## run the tests
```

### Comparing `jupyterlab_templates-0.4.0/js/.eslintrc.js` & `jupyterlab_templates-0.4.1/js/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/js/icon.png` & `jupyterlab_templates-0.4.1/js/icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/js/package.json` & `jupyterlab_templates-0.4.1/js/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9628571428571429%*

 * *Differences: {"'devDependencies'": "{'jest-junit': '^15.0.0'}", "'version'": "'0.4.1'"}*

```diff
@@ -28,14 +28,15 @@
         "eslint-plugin-import": "^2.27.5",
         "eslint-plugin-jest": "^27.2.1",
         "eslint-plugin-json": "^3.1.0",
         "eslint-plugin-prettier": "^4.0.0",
         "isomorphic-fetch": "^3.0.0",
         "jest": "^29.4.3",
         "jest-environment-jsdom": "^29.4.3",
+        "jest-junit": "^15.0.0",
         "jest-transform-css": "^6.0.1",
         "mkdirp": "^2.1.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.4",
         "rimraf": "^4.1.2"
     },
     "files": [
@@ -80,9 +81,9 @@
         "check-security": "auditjs-screener 5",
         "clean": "rimraf lib",
         "fix": "yarn lint --fix",
         "lint": "eslint -c .eslintrc.js --ext .js src/ tests/",
         "prepublishOnly": "npm run build",
         "test": "jest --coverage --collectCoverageFrom=src/*.{js}"
     },
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `jupyterlab_templates-0.4.0/js/yarn.lock` & `jupyterlab_templates-0.4.1/js/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -4829,14 +4829,24 @@
     jest-util "^29.4.3"
     jest-worker "^29.4.3"
     micromatch "^4.0.4"
     walker "^1.0.8"
   optionalDependencies:
     fsevents "^2.3.2"
 
+jest-junit@^15.0.0:
+  version "15.0.0"
+  resolved "https://registry.yarnpkg.com/jest-junit/-/jest-junit-15.0.0.tgz#a47544ab42e9f8fe7ada56306c218e09e52bd690"
+  integrity sha512-Z5sVX0Ag3HZdMUnD5DFlG+1gciIFSy7yIVPhOdGUi8YJaI9iLvvBb530gtQL2CHmv0JJeiwRZenr0VrSR7frvg==
+  dependencies:
+    mkdirp "^1.0.4"
+    strip-ansi "^6.0.1"
+    uuid "^8.3.2"
+    xml "^1.0.1"
+
 jest-leak-detector@^29.4.3:
   version "29.4.3"
   resolved "https://registry.yarnpkg.com/jest-leak-detector/-/jest-leak-detector-29.4.3.tgz#2b35191d6b35aa0256e63a9b79b0f949249cf23a"
   integrity sha512-9yw4VC1v2NspMMeV3daQ1yXPNxMgCzwq9BocCwYrRgXe4uaEJPAN0ZK37nFBhcy3cUwEVstFecFLaTHpF7NiGA==
   dependencies:
     jest-get-type "^29.4.3"
     pretty-format "^29.4.3"
@@ -7154,14 +7164,19 @@
   integrity sha512-mLs5zAK+ctllYBj+iAQvlDCwoxU/WDOUaJkcFudeiAX6OajC6BKXJUa9a+tbtkC11dz2Ufb7h0lyvIOVn4LADA==
 
 uuid@^3.3.2:
   version "3.4.0"
   resolved "https://registry.yarnpkg.com/uuid/-/uuid-3.4.0.tgz#b23e4358afa8a202fe7a100af1f5f883f02007ee"
   integrity sha512-HjSDRw6gZE5JMggctHBcjVak08+KEVhSIiDzFnT9S9aegmp85S/bReBVTb4QTFaRNptJ9kuYaNhnbNEOkbKb/A==
 
+uuid@^8.3.2:
+  version "8.3.2"
+  resolved "https://registry.yarnpkg.com/uuid/-/uuid-8.3.2.tgz#80d5b5ced271bb9af6c445f21a1a04c606cefbe2"
+  integrity sha512-+NYs2QeMWy+GWFOEm9xnn6HCDp0l7QBD7ml8zLUmJ+93Q5NF0NocErnwkTkXVFNiX3/fpC6afS8Dhb/gz7R7eg==
+
 v8-to-istanbul@^9.0.1:
   version "9.0.1"
   resolved "https://registry.yarnpkg.com/v8-to-istanbul/-/v8-to-istanbul-9.0.1.tgz#b6f994b0b5d4ef255e17a0d17dc444a9f5132fa4"
   integrity sha512-74Y4LqY74kLE6IFyIjPtkSTWzUZmj8tdHT9Ii/26dvQ6K9Dl2NbEfj0XgU2sHCtKgt5VupqhlO/5aWuqS+IY1w==
   dependencies:
     "@jridgewell/trace-mapping" "^0.3.12"
     "@types/istanbul-lib-coverage" "^2.0.1"
@@ -7474,14 +7489,19 @@
   integrity sha512-F+P9Jil7UiSKSkppIiD94dN07AwvFixvLIj1Og1Rl9GGMuNipJnV9JzjD6XuqmAeiswGvUmNLjr5cFuXwNS77Q==
 
 xml-name-validator@^4.0.0:
   version "4.0.0"
   resolved "https://registry.yarnpkg.com/xml-name-validator/-/xml-name-validator-4.0.0.tgz#79a006e2e63149a8600f15430f0a4725d1524835"
   integrity sha512-ICP2e+jsHvAj2E2lIHxa5tjXRlKDJo4IdvPvCXbXQGdzSfmSpNVyIKMvoZHjDY9DP0zV17iI85o90vRFXNccRw==
 
+xml@^1.0.1:
+  version "1.0.1"
+  resolved "https://registry.yarnpkg.com/xml/-/xml-1.0.1.tgz#78ba72020029c5bc87b8a81a3cfcd74b4a2fc1e5"
+  integrity sha512-huCv9IH9Tcf95zuYCsQraZtWnJvBtLVE0QHMOs8bWyZAFZNDcYjsPq1nEx8jKA9y+Beo9v+7OBPRisQTjinQMw==
+
 xmlbuilder@^13.0.2:
   version "13.0.2"
   resolved "https://registry.yarnpkg.com/xmlbuilder/-/xmlbuilder-13.0.2.tgz#02ae33614b6a047d1c32b5389c1fdacb2bce47a7"
   integrity sha512-Eux0i2QdDYKbdbA6AM6xE4m6ZTZr4G4xF9kahI2ukSEMCzwce2eX9WlTI5J3s+NU7hpasFsr8hWIONae7LluAQ==
 
 xmlchars@^2.2.0:
   version "2.2.0"
@@ -7539,17 +7559,17 @@
 
 yallist@^4.0.0:
   version "4.0.0"
   resolved "https://registry.yarnpkg.com/yallist/-/yallist-4.0.0.tgz#9bb92790d9c0effec63be73519e11a35019a3a72"
   integrity sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==
 
 yaml@^2.1.1:
-  version "2.2.1"
-  resolved "https://registry.yarnpkg.com/yaml/-/yaml-2.2.1.tgz#3014bf0482dcd15147aa8e56109ce8632cd60ce4"
-  integrity sha512-e0WHiYql7+9wr4cWMx3TVQrNwejKaEe7/rHNmQmqRjazfOP5W8PB6Jpebb5o6fIapbz9o9+2ipcaTM2ZwDI6lw==
+  version "2.2.2"
+  resolved "https://registry.yarnpkg.com/yaml/-/yaml-2.2.2.tgz#ec551ef37326e6d42872dad1970300f8eb83a073"
+  integrity sha512-CBKFWExMn46Foo4cldiChEzn7S7SRV+wqiluAb6xmueD/fGyRHIhX8m14vVGgeFWjN540nKCNVj6P21eQjgTuA==
 
 yargs-parser@^20.2.2:
   version "20.2.9"
   resolved "https://registry.yarnpkg.com/yargs-parser/-/yargs-parser-20.2.9.tgz#2eb7dc3b0289718fc295f362753845c41a0c94ee"
   integrity sha512-y11nGElTIV+CT3Zv9t7VKl+Q3hTQoT9a1Qzezhhl6Rp21gJ/IVTW7Z3y9EWXhuUBC2Shnf+DX0antecpAwSP8w==
 
 yargs-parser@^21.1.1:
```

### Comparing `jupyterlab_templates-0.4.0/js/src/index.js` & `jupyterlab_templates-0.4.1/js/src/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -120,30 +120,37 @@
                                 }).then((res2) => {
                                     const data = res2.json();
                                     const {
                                         path
                                     } = browser.defaultBrowser.model;
 
                                     return new Promise((resolve) => {
+                                        const ext = data.filename.split(".").pop().toLowerCase();
+                                        const isNotebook = ext === "ipynb";
                                         app.commands
                                             .execute("docmanager:new-untitled", {
+                                                ext,
                                                 path,
-                                                type: "notebook",
+                                                type: isNotebook ? "notebook" : "file",
                                             })
                                             .then((model) => {
                                                 app.commands
                                                     .execute("docmanager:open", {
-                                                        factory: "Notebook",
+                                                        factory: isNotebook ? "Notebook" : null,
                                                         path: model.path,
                                                     })
                                                     .then((widget) => {
                                                         // eslint-disable-next-line no-param-reassign
                                                         widget.isUntitled = true;
                                                         widget.context.ready.then(() => {
-                                                            widget.model.fromString(data.content);
+                                                            if (isNotebook) {
+                                                                widget.model.fromString(data.content);
+                                                            } else {
+                                                                widget.content.editor._editor.setValue(data.content);
+                                                            }
                                                             resolve(widget);
                                                         });
                                                     });
                                             });
                                     });
                                 });
                             }
```

### Comparing `jupyterlab_templates-0.4.0/js/style/icon.svg` & `jupyterlab_templates-0.4.1/js/style/icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/js/style/index.css` & `jupyterlab_templates-0.4.1/js/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/__init__.py` & `jupyterlab_templates-0.4.1/jupyterlab_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/extension.py` & `jupyterlab_templates-0.4.1/jupyterlab_templates/extension.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # *****************************************************************************
 #
 # Copyright (c) 2020, the jupyterlab_templates authors.
 #
 # This file is part of the jupyterlab_templates library, distributed under the terms of
 # the Apache License 2.0.  The full license can be found in the LICENSE file.
 #
-import fnmatch
 import json
 import os
 import os.path
 import jupyter_core.paths
 import tornado.web
 
 from io import open
-from notebook.base.handlers import IPythonHandler
-from notebook.utils import url_path_join
+from fnmatch import fnmatch
+from jupyter_server.base.handlers import JupyterHandler
+from jupyter_server.utils import url_path_join
+
+TEMPLATES_IGNORE_FILE = ".jupyterlab_templates_ignore"
 
 
 class TemplatesLoader:
-    def __init__(self, template_dirs):
+    def __init__(self, template_dirs, allowed_extensions=None):
         self.template_dirs = template_dirs
+        self.allowed_extensions = allowed_extensions or ["*.ipynb"]
 
     def get_templates(self):
         templates = {}
         template_by_path = {}
 
         for path in self.template_dirs:
             # in order to produce correct filenames, abspath should point to the parent directory of path
@@ -31,15 +34,24 @@
             files = []
             # get all files in subdirectories
             for dirname, _, filenames in os.walk(path, followlinks=True):
                 if dirname == path:
                     # Skip top level
                     continue
 
-                for filename in fnmatch.filter(filenames, "*.ipynb"):
+                if TEMPLATES_IGNORE_FILE in filenames:
+                    # skip this very directory (subdirectories will still be considered)
+                    continue
+
+                _files = [
+                    x
+                    for x in filenames
+                    if any(fnmatch(x, y) for y in self.allowed_extensions)
+                ]
+                for filename in _files:
                     if ".ipynb_checkpoints" not in dirname:
                         files.append(
                             (
                                 os.path.join(dirname, filename),
                                 dirname.replace(path, ""),
                                 filename,
                             )
@@ -71,28 +83,28 @@
 
                 # full data
                 template_by_path[data["name"]] = data
 
         return templates, template_by_path
 
 
-class TemplatesHandler(IPythonHandler):
+class TemplatesHandler(JupyterHandler):
     def initialize(self, loader):
         self.loader = loader
 
     @tornado.web.authenticated
     def get(self):
         temp = self.get_argument("template", "")
         if temp:
             self.finish(self.loader.get_templates()[1][temp])
         else:
             self.set_status(404)
 
 
-class TemplateNamesHandler(IPythonHandler):
+class TemplateNamesHandler(JupyterHandler):
     def initialize(self, loader):
         self.loader = loader
 
     @tornado.web.authenticated
     def get(self):
         self.finish(json.dumps(self.loader.get_templates()[0]))
 
@@ -105,14 +117,18 @@
         nb_server_app (NotebookWebApplication): handle to the Notebook webserver instance.
     """
     web_app = nb_server_app.web_app
     template_dirs = nb_server_app.config.get("JupyterLabTemplates", {}).get(
         "template_dirs", []
     )
 
+    allowed_extensions = nb_server_app.config.get("JupyterLabTemplates", {}).get(
+        "allowed_extensions", ["*.ipynb"]
+    )
+
     if nb_server_app.config.get("JupyterLabTemplates", {}).get("include_default", True):
         template_dirs.insert(0, os.path.join(os.path.dirname(__file__), "templates"))
 
     base_url = web_app.settings["base_url"]
 
     host_pattern = ".*$"
     nb_server_app.log.info(
@@ -127,15 +143,15 @@
             [
                 os.path.join(x, "notebook_templates")
                 for x in jupyter_core.paths.jupyter_path()
             ]
         )
     nb_server_app.log.info("Search paths:\n\t%s" % "\n\t".join(template_dirs))
 
-    loader = TemplatesLoader(template_dirs)
+    loader = TemplatesLoader(template_dirs, allowed_extensions=allowed_extensions)
     nb_server_app.log.info(
         "Available templates:\n\t%s"
         % "\n\t".join(t for t in loader.get_templates()[1].keys())
     )
 
     web_app.add_handlers(
         host_pattern,
```

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/extension/notebook_templates/jupyterlab_templates/Sample.ipynb` & `jupyterlab_templates-0.4.1/jupyterlab_templates/extension/notebook_templates/jupyterlab_templates/Sample.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/package.json` & `jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9617410714285715%*

 * *Differences: {"'devDependencies'": "{'jest-junit': '^15.0.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.dc333b99e046544e4b16.js'}}",*

 * * "'version'": "'0.4.1'"}*

```diff
@@ -28,28 +28,29 @@
         "eslint-plugin-import": "^2.27.5",
         "eslint-plugin-jest": "^27.2.1",
         "eslint-plugin-json": "^3.1.0",
         "eslint-plugin-prettier": "^4.0.0",
         "isomorphic-fetch": "^3.0.0",
         "jest": "^29.4.3",
         "jest-environment-jsdom": "^29.4.3",
+        "jest-junit": "^15.0.0",
         "jest-transform-css": "^6.0.1",
         "mkdirp": "^2.1.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.4",
         "rimraf": "^4.1.2"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.16bfd2a294ef1e5cdaee.js"
+            "load": "static/remoteEntry.dc333b99e046544e4b16.js"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_templates"
                 },
                 "managers": [
@@ -84,9 +85,9 @@
         "check-security": "auditjs-screener 5",
         "clean": "rimraf lib",
         "fix": "yarn lint --fix",
         "lint": "eslint -c .eslintrc.js --ext .js src/ tests/",
         "prepublishOnly": "npm run build",
         "test": "jest --coverage --collectCoverageFrom=src/*.{js}"
     },
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/static/568.7c3fb82db0068d774682.js` & `jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/static/568.bca76f9a3703a686ab31.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunkjupyterlab_templates = self.webpackChunkjupyterlab_templates || []).push([
     [568], {
         568: (A, I, E) => {
             Object.defineProperty(I, "__esModule", {
                 value: !0
             }), I.OpenTemplateWidget = void 0, I._activate = S, I.default = void 0;
-            var C = E(884),
-                Q = E(848),
-                g = E(643),
-                k = E(529),
-                J = E(448),
-                R = E(431),
+            var C = E(303),
+                Q = E(344),
+                g = E(122),
+                k = E(71),
+                J = E(535),
+                R = E(832),
                 B = E(760);
             let i;
             E(549);
             class M extends R.Widget {
                 constructor() {
                     const A = document.createElement("div"),
                         I = document.createElement("label");
@@ -62,24 +62,27 @@
                                             template: I.value
                                         }).then((I => {
                                             const C = I.json(),
                                                 {
                                                     path: Q
                                                 } = E.defaultBrowser.model;
                                             return new Promise((I => {
+                                                const E = C.filename.split(".").pop().toLowerCase(),
+                                                    g = "ipynb" === E;
                                                 A.commands.execute("docmanager:new-untitled", {
+                                                    ext: E,
                                                     path: Q,
-                                                    type: "notebook"
+                                                    type: g ? "notebook" : "file"
                                                 }).then((E => {
                                                     A.commands.execute("docmanager:open", {
-                                                        factory: "Notebook",
+                                                        factory: g ? "Notebook" : null,
                                                         path: E.path
                                                     }).then((A => {
                                                         A.isUntitled = !0, A.context.ready.then((() => {
-                                                            A.model.fromString(C.content), I(A)
+                                                            g ? A.model.fromString(C.content) : A.content.editor._editor.setValue(C.content), I(A)
                                                         }))
                                                     }))
                                                 }))
                                             }))
                                         }))
                                     }))
                                 },
```

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/static/873.6ea510b34d81274bc9b0.js` & `jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/static/873.6ea510b34d81274bc9b0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/static/remoteEntry.16bfd2a294ef1e5cdaee.js` & `jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/static/remoteEntry.dc333b99e046544e4b16.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -42,18 +42,18 @@
         }), r
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        568: "7c3fb82db0068d774682",
+        568: "bca76f9a3703a686ab31",
         873: "6ea510b34d81274bc9b0"
     } [e] + ".js?v=" + {
-        568: "7c3fb82db0068d774682",
+        568: "bca76f9a3703a686ab31",
         873: "6ea510b34d81274bc9b0"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("jupyterlab_templates", "0.4.0", (() => w.e(568).then((() => () => w(568))))), u("requests-helper", "0.1.5", (() => w.e(873).then((() => () => w(873)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab_templates", "0.4.1", (() => w.e(568).then((() => () => w(568))))), u("requests-helper", "0.1.5", (() => w.e(873).then((() => () => w(873)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -211,23 +211,23 @@
     }, p = e => (e.loaded = 1, e.get()), c = (d = e => function(r, t, n, a) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
     })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = d(((e, r, t, n, a) => {
         var o = r && w.o(r, t) && f(r, t, n);
         return o ? p(o) : a()
     })), v = {}, b = {
-        431: () => c("default", "@lumino/widgets", [1, 1, 37, 1]),
-        448: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 2]),
-        529: () => c("default", "@jupyterlab/launcher", [1, 3, 6, 2]),
-        643: () => c("default", "@jupyterlab/filebrowser", [1, 3, 6, 2]),
+        71: () => c("default", "@jupyterlab/launcher", [1, 3, 6, 5]),
+        122: () => c("default", "@jupyterlab/filebrowser", [1, 3, 6, 5]),
+        303: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        344: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
+        535: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 5]),
         760: () => h("default", "requests-helper", [2, 0, 1, 5], (() => w.e(873).then((() => () => w(873))))),
-        848: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 2]),
-        884: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 2])
+        832: () => c("default", "@lumino/widgets", [1, 1, 37, 2])
     }, m = {
-        568: [431, 448, 529, 643, 760, 848, 884]
+        568: [71, 122, 303, 344, 535, 760, 832]
     }, w.f.consumes = (e, r) => {
         w.o(m, e) && m[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/labextension/static/third-party-licenses.json` & `jupyterlab_templates-0.4.1/jupyterlab_templates/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/templates/jupyterlab_templates/Sample.ipynb` & `jupyterlab_templates-0.4.1/jupyterlab_templates/templates/jupyterlab_templates/Sample.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/tests/test_extension.py` & `jupyterlab_templates-0.4.1/jupyterlab_templates/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/jupyterlab_templates/tests/test_init.py` & `jupyterlab_templates-0.4.1/jupyterlab_templates/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/.gitignore` & `jupyterlab_templates-0.4.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 # Unit test / coverage reports
 htmlcov/
 .tox/
 .coverage
 .coverage.*
 .cache
 python_junit.xml
+junit.xml
 nosetests.xml
 coverage.xml
 *,cover
 .hypothesis/
 .pytest_cache
 .ruff_cache
```

### Comparing `jupyterlab_templates-0.4.0/LICENSE` & `jupyterlab_templates-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_templates-0.4.0/README.md` & `jupyterlab_templates-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,28 +35,32 @@
 jupyter server extension enable --py jupyterlab_templates
 ```
 
 ## Adding templates
 install the server extension, and add the following to `jupyter_notebook_config.py`
 
 ```python3
+c.JupyterLabTemplates.allowed_extensions = ["*.ipynb"]
 c.JupyterLabTemplates.template_dirs = ['list', 'of', 'template', 'directories']
 c.JupyterLabTemplates.include_default = True
 c.JupyterLabTemplates.include_core_paths = True
 ```
 
 ## Templates for libraries
 The extension will search *subdirectories* of each parent directory specified in `template_dirs` for templates.
 **Note!** Templates in the parent directories will be ignored. You must put the templates in *subdirectories*, in order to keep everything organized.  
 
 If `include_default = True` the `notebook_templates` directory under the [jupyter data folder](https://jupyter.readthedocs.io/en/latest/use/jupyter-directories.html) is one of the default parent directories. Thus, if you have tutorials or guides you'd like to install for users, simply copy them into your jupyter data folder inside the `notebook_templates` directory, e.g. `/usr/local/share/jupyter/notebook_templates/bqplot` for `bqplot`.
 
+If you want to exclude templates from a specific directory, please add a file `.jupyterlab_templates_ignore` to to this location.
+All notebooks in this directory will be ignored (but has no effect on subdirectories).
 
 ### Flags
-- `template_dirs`: a list of absolute directory paths. All `.ipynb` files in any *subdirectories* of these paths will be listed as templates
+- `allowed_extensions`: a list of extensions to allow templates for. (optional, default `["*.ipynb"]`)
+- `template_dirs`: a list of absolute directory paths. All files matching `allowed_extensions` in any *subdirectories* of these paths will be listed as templates
 - `include_default`: include the default Sample template (default True)
 - `include_core_paths`: include jupyter core paths (see: jupyter --paths) (default True)
 
 
 ## Development
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.
```

### Comparing `jupyterlab_templates-0.4.0/pyproject.toml` & `jupyterlab_templates-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "jupyterlab>=3.5,<4",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab_templates"
 description = "notebook templates for jupyterlab"
-version = "0.4.0"
+version = "0.4.1"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "the jupyterlab_templates authors" },
 ]
 keywords = [
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
-    "jupyterlab>=3.5"
+    "jupyterlab>=3.5",
 ]
 
 [project.optional-dependencies]
 develop = [
     "black>=23",
     "check-manifest",
     "ruff",
@@ -47,16 +47,16 @@
 ]
 test = [
     "pytest",
     "pytest-cov",
 ]
 
 [project.urls]
-repository = "https://github.com/finos/jupyterlab_templates"
-homepage = "https://github.com/finos/jupyterlab_templates"
+Repository = "https://github.com/finos/jupyterlab_templates"
+Homepage = "https://github.com/finos/jupyterlab_templates"
 
 [tool.check-manifest]
 ignore = [
 	"jupyterlab_templates/labextension/**",
 	"js/**"
 ]
```

### Comparing `jupyterlab_templates-0.4.0/PKG-INFO` & `jupyterlab_templates-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jupyterlab_templates
-Version: 0.4.0
+Version: 0.4.1
 Summary: notebook templates for jupyterlab
-Project-URL: repository, https://github.com/finos/jupyterlab_templates
-Project-URL: homepage, https://github.com/finos/jupyterlab_templates
+Project-URL: Repository, https://github.com/finos/jupyterlab_templates
+Project-URL: Homepage, https://github.com/finos/jupyterlab_templates
 Author: the jupyterlab_templates authors
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -271,28 +271,32 @@
 jupyter server extension enable --py jupyterlab_templates
 ```
 
 ## Adding templates
 install the server extension, and add the following to `jupyter_notebook_config.py`
 
 ```python3
+c.JupyterLabTemplates.allowed_extensions = ["*.ipynb"]
 c.JupyterLabTemplates.template_dirs = ['list', 'of', 'template', 'directories']
 c.JupyterLabTemplates.include_default = True
 c.JupyterLabTemplates.include_core_paths = True
 ```
 
 ## Templates for libraries
 The extension will search *subdirectories* of each parent directory specified in `template_dirs` for templates.
 **Note!** Templates in the parent directories will be ignored. You must put the templates in *subdirectories*, in order to keep everything organized.  
 
 If `include_default = True` the `notebook_templates` directory under the [jupyter data folder](https://jupyter.readthedocs.io/en/latest/use/jupyter-directories.html) is one of the default parent directories. Thus, if you have tutorials or guides you'd like to install for users, simply copy them into your jupyter data folder inside the `notebook_templates` directory, e.g. `/usr/local/share/jupyter/notebook_templates/bqplot` for `bqplot`.
 
+If you want to exclude templates from a specific directory, please add a file `.jupyterlab_templates_ignore` to to this location.
+All notebooks in this directory will be ignored (but has no effect on subdirectories).
 
 ### Flags
-- `template_dirs`: a list of absolute directory paths. All `.ipynb` files in any *subdirectories* of these paths will be listed as templates
+- `allowed_extensions`: a list of extensions to allow templates for. (optional, default `["*.ipynb"]`)
+- `template_dirs`: a list of absolute directory paths. All files matching `allowed_extensions` in any *subdirectories* of these paths will be listed as templates
 - `include_default`: include the default Sample template (default True)
 - `include_core_paths`: include jupyter core paths (see: jupyter --paths) (default True)
 
 
 ## Development
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.
```

