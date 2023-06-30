# Comparing `tmp/shiny_mdc-1.7.0.tar.gz` & `tmp/shiny_mdc-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.7.0.tar", max compression
+gzip compressed data, was "shiny_mdc-1.7.1.tar", max compression
```

## Comparing `shiny_mdc-1.7.0.tar` & `shiny_mdc-1.7.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     6984 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/LICENSE
--rw-r--r--   0        0        0       78 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/README.md
--rw-r--r--   0        0        0     2297 2023-06-29 04:58:18.288915 shiny_mdc-1.7.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4782 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     5084 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-06-29 04:58:18.292915 shiny_mdc-1.7.0/shinymdc/_version.py
--rw-r--r--   0        0        0      410 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      879 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      316 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0      491 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/bibnonatsetup.tex
--rw-r--r--   0        0        0      324 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/bibnosupersetup.tex
--rw-r--r--   0        0        0      745 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/bibsupersetup.tex
--rw-r--r--   0        0        0     3266 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-06-29 04:57:56.244913 shiny_mdc-1.7.0/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0     1202 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      503 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    19497 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/shinymdc.py
--rw-r--r--   0        0        0     1017 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1302 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1423 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2170 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      916 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     3136 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      464 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2483 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/test/figures/lines.png
--rw-r--r--   0        0        0     2988 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/test/main.md
--rwxr-xr-x   0        0        0      315 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/test/make.sh
--rw-r--r--   0        0        0     1166 2023-06-29 04:57:56.248913 shiny_mdc-1.7.0/test/references.bib
--rw-r--r--   0        0        0   690901 2023-06-29 04:57:56.252913 shiny_mdc-1.7.0/test/samples/basic.pdf
--rw-r--r--   0        0        0   414185 2023-06-29 04:57:56.252913 shiny_mdc-1.7.0/test/samples/iccv.pdf
--rw-r--r--   0        0        0   407653 2023-06-29 04:57:56.256913 shiny_mdc-1.7.0/test/samples/iclr.pdf
--rw-r--r--   0        0        0   446740 2023-06-29 04:57:56.260913 shiny_mdc-1.7.0/test/samples/icml.pdf
--rw-r--r--   0        0        0   451322 2023-06-29 04:57:56.260913 shiny_mdc-1.7.0/test/samples/neurips.pdf
--rw-r--r--   0        0        0   600276 2023-06-29 04:57:56.264913 shiny_mdc-1.7.0/test/samples/spacious.pdf
--rw-r--r--   0        0        0   555527 2023-06-29 04:57:56.264913 shiny_mdc-1.7.0/test/samples/standalone.pdf
--rw-r--r--   0        0        0   425326 2023-06-29 04:57:56.268913 shiny_mdc-1.7.0/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-06-29 04:57:56.268913 shiny_mdc-1.7.0/test/sections/appendix1.md
--rw-r--r--   0        0        0     1624 2023-06-29 04:57:56.268913 shiny_mdc-1.7.0/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-06-29 04:57:56.268913 shiny_mdc-1.7.0/test/sections/empty.md
--rw-r--r--   0        0        0     2326 2023-06-29 04:57:56.268913 shiny_mdc-1.7.0/test/sections/main1.md
--rw-r--r--   0        0        0     1351 2023-06-29 04:57:56.268913 shiny_mdc-1.7.0/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-06-29 04:57:56.268913 shiny_mdc-1.7.0/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-06-29 04:57:56.268913 shiny_mdc-1.7.0/test/utils/ext.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     7079 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/LICENSE
+-rw-r--r--   0        0        0       78 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/README.md
+-rw-r--r--   0        0        0     2313 2023-06-30 00:42:13.354307 shiny_mdc-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4782 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     5084 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-06-30 00:42:13.354307 shiny_mdc-1.7.1/shinymdc/_version.py
+-rw-r--r--   0        0        0      410 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      879 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      316 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0      491 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/bibnonatsetup.tex
+-rw-r--r--   0        0        0      324 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/bibnosupersetup.tex
+-rw-r--r--   0        0        0      745 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/bibsupersetup.tex
+-rw-r--r--   0        0        0     3266 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0     1202 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      503 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    19497 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0     1017 2023-06-30 00:41:54.542353 shiny_mdc-1.7.1/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1302 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1423 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2170 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      916 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     3136 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      464 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2483 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/test/figures/lines.png
+-rw-r--r--   0        0        0     2988 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-06-30 00:41:54.546353 shiny_mdc-1.7.1/test/references.bib
+-rw-r--r--   0        0        0   690901 2023-06-30 00:41:54.550353 shiny_mdc-1.7.1/test/samples/basic.pdf
+-rw-r--r--   0        0        0   414185 2023-06-30 00:41:54.550353 shiny_mdc-1.7.1/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   407653 2023-06-30 00:41:54.554353 shiny_mdc-1.7.1/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   446740 2023-06-30 00:41:54.554353 shiny_mdc-1.7.1/test/samples/icml.pdf
+-rw-r--r--   0        0        0   451322 2023-06-30 00:41:54.558353 shiny_mdc-1.7.1/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   600276 2023-06-30 00:41:54.562353 shiny_mdc-1.7.1/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   555527 2023-06-30 00:41:54.562353 shiny_mdc-1.7.1/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   425326 2023-06-30 00:41:54.566353 shiny_mdc-1.7.1/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-06-30 00:41:54.566353 shiny_mdc-1.7.1/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1624 2023-06-30 00:41:54.566353 shiny_mdc-1.7.1/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-06-30 00:41:54.566353 shiny_mdc-1.7.1/test/sections/empty.md
+-rw-r--r--   0        0        0     2326 2023-06-30 00:41:54.566353 shiny_mdc-1.7.1/test/sections/main1.md
+-rw-r--r--   0        0        0     1351 2023-06-30 00:41:54.566353 shiny_mdc-1.7.1/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-06-30 00:41:54.566353 shiny_mdc-1.7.1/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-06-30 00:41:54.566353 shiny_mdc-1.7.1/test/utils/ext.md
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 shiny_mdc-1.7.1/PKG-INFO
```

### Comparing `shiny_mdc-1.7.0/CHANGELOG.md` & `shiny_mdc-1.7.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [1.7.1](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.7.0...v1.7.1) (2023-06-30)
+
 ## [1.7.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.6.0...v1.7.0) (2023-06-29)
 
 
 ### Features
 
 * allow specifying document url ([2cd7514](https://github.com/jayanthkoushik/shiny-mdc/commit/2cd7514326d97fc16c3addf2ec852f3709318ae8))
```

### Comparing `shiny_mdc-1.7.0/LICENSE` & `shiny_mdc-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/pyproject.toml` & `shiny_mdc-1.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.7.0"  # managed by `poetry-dynamic-versioning`
+version = "1.7.1"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
@@ -25,14 +25,15 @@
 
 [tool.poetry.scripts]
 shinymdc = "shinymdc.shinymdc:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 corgy = { version="^8.1.1", extras = ["colors"] }
+pyyaml = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.0"
 black = "^22.0"
 isort = "^5.1"
 pylint = "^2.14"
 mypy = "^1.1"
```

### Comparing `shiny_mdc-1.7.0/shinymdc/_latexmk.py` & `shiny_mdc-1.7.1/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/_liquid.py` & `shiny_mdc-1.7.1/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/_pandoc.py` & `shiny_mdc-1.7.1/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/_templates.py` & `shiny_mdc-1.7.1/shinymdc/_templates.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.7.1/shinymdc/resources/dynamic/authsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.7.1/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/bibsupersetup.tex` & `shiny_mdc-1.7.1/shinymdc/resources/static/bibsupersetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.7.1/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.7.1/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.7.1/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.7.1/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.7.1/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.7.1/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.7.1/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.7.1/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.7.1/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.7.1/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.7.1/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.7.1/shinymdc/resources/static/miscsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.7.1/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/shinymdc.py` & `shiny_mdc-1.7.1/shinymdc/shinymdc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/templates/basic.tex` & `shiny_mdc-1.7.1/shinymdc/templates/basic.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/templates/iccv.tex` & `shiny_mdc-1.7.1/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/templates/iclr.tex` & `shiny_mdc-1.7.1/shinymdc/templates/iclr.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/templates/icml.tex` & `shiny_mdc-1.7.1/shinymdc/templates/icml.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/templates/neurips.tex` & `shiny_mdc-1.7.1/shinymdc/templates/neurips.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/templates/spacious.tex` & `shiny_mdc-1.7.1/shinymdc/templates/spacious.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/shinymdc/templates/stylish.tex` & `shiny_mdc-1.7.1/shinymdc/templates/stylish.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/figures/anscombe.pdf` & `shiny_mdc-1.7.1/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/figures/densities.pdf` & `shiny_mdc-1.7.1/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/figures/diamonds.pdf` & `shiny_mdc-1.7.1/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/figures/gaussian2d.pdf` & `shiny_mdc-1.7.1/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/figures/lines.png` & `shiny_mdc-1.7.1/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/main.md` & `shiny_mdc-1.7.1/test/main.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/references.bib` & `shiny_mdc-1.7.1/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/samples/basic.pdf` & `shiny_mdc-1.7.1/test/samples/basic.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/samples/iccv.pdf` & `shiny_mdc-1.7.1/test/samples/iccv.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/samples/iclr.pdf` & `shiny_mdc-1.7.1/test/samples/iclr.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/samples/icml.pdf` & `shiny_mdc-1.7.1/test/samples/icml.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/samples/neurips.pdf` & `shiny_mdc-1.7.1/test/samples/neurips.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/samples/spacious.pdf` & `shiny_mdc-1.7.1/test/samples/spacious.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/samples/standalone.pdf` & `shiny_mdc-1.7.1/test/samples/standalone.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/samples/stylish.pdf` & `shiny_mdc-1.7.1/test/samples/stylish.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/sections/appendix1.md` & `shiny_mdc-1.7.1/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/sections/appendix2.md` & `shiny_mdc-1.7.1/test/sections/appendix2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/sections/main1.md` & `shiny_mdc-1.7.1/test/sections/main1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/sections/main2.md` & `shiny_mdc-1.7.1/test/sections/main2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/test/utils/commands.md` & `shiny_mdc-1.7.1/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.7.0/PKG-INFO` & `shiny_mdc-1.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.7.0
+Version: 1.7.1
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: corgy[colors] (>=8.1.1,<9.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/jayanthkoushik/shinymdc
 Description-Content-Type: text/markdown
 
 # shiny-mdc
 
 Tool to compile markdown files to tex/pdf using pandoc, latexmk.
```

