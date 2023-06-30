# Comparing `tmp/pretext-1.6.1.dev20230628.tar.gz` & `tmp/pretext-1.6.1.dev20230629.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230628.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230629.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230628.tar` & `pretext-1.6.1.dev20230629.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-28 06:14:51.233658 pretext-1.6.1.dev20230628/LICENSE
--rw-r--r--   0        0        0     9757 2023-06-28 06:14:51.233658 pretext-1.6.1.dev20230628/README.md
--rw-r--r--   0        0        0     1909 2023-06-28 06:15:30.025987 pretext-1.6.1.dev20230628/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-28 06:14:51.233658 pretext-1.6.1.dev20230628/pretext/__main__.py
--rw-r--r--   0        0        0     8531 2023-06-28 06:14:51.233658 pretext-1.6.1.dev20230628/pretext/build.py
--rw-r--r--   0        0        0    25736 2023-06-28 06:14:51.233658 pretext-1.6.1.dev20230628/pretext/cli.py
--rw-r--r--   0        0        0     5856 2023-06-28 06:14:51.233658 pretext-1.6.1.dev20230628/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-06-28 06:14:51.237658 pretext-1.6.1.dev20230628/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-28 06:14:51.237658 pretext-1.6.1.dev20230628/pretext/core/__init__.py
--rw-r--r--   0        0        0   172492 2023-06-28 06:15:35.234025 pretext-1.6.1.dev20230628/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-06-28 06:14:51.237658 pretext-1.6.1.dev20230628/pretext/core/resources.py
--rw-r--r--   0        0        0  1041510 2023-06-28 06:15:35.234025 pretext-1.6.1.dev20230628/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-06-28 06:14:51.237658 pretext-1.6.1.dev20230628/pretext/generate.py
--rw-r--r--   0        0        0    29108 2023-06-28 06:14:51.237658 pretext-1.6.1.dev20230628/pretext/project.py
--rw-r--r--   0        0        0      739 2023-06-28 06:14:51.237658 pretext-1.6.1.dev20230628/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-28 06:15:35.338025 pretext-1.6.1.dev20230628/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-28 06:15:35.338025 pretext-1.6.1.dev20230628/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160110 2023-06-28 06:15:35.302025 pretext-1.6.1.dev20230628/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7616 2023-06-28 06:15:35.306025 pretext-1.6.1.dev20230628/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173309 2023-06-28 06:15:35.334025 pretext-1.6.1.dev20230628/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2192 2023-06-28 06:15:35.338025 pretext-1.6.1.dev20230628/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4657 2023-06-28 06:15:35.318025 pretext-1.6.1.dev20230628/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-28 06:15:35.338025 pretext-1.6.1.dev20230628/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-28 06:15:35.338025 pretext-1.6.1.dev20230628/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8392 2023-06-28 06:15:35.310025 pretext-1.6.1.dev20230628/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    25086 2023-06-28 06:14:51.237658 pretext-1.6.1.dev20230628/pretext/utils.py
--rw-r--r--   0        0        0     3333 2023-06-28 06:15:30.025987 pretext-1.6.1.dev20230628/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230628/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-29 06:19:31.808368 pretext-1.6.1.dev20230629/LICENSE
+-rw-r--r--   0        0        0     9757 2023-06-29 06:19:31.808368 pretext-1.6.1.dev20230629/README.md
+-rw-r--r--   0        0        0     1909 2023-06-29 06:20:11.630612 pretext-1.6.1.dev20230629/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/__main__.py
+-rw-r--r--   0        0        0     8531 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/build.py
+-rw-r--r--   0        0        0    25736 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/cli.py
+-rw-r--r--   0        0        0     5856 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172492 2023-06-29 06:20:16.986914 pretext-1.6.1.dev20230629/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/core/resources.py
+-rw-r--r--   0        0        0  1042093 2023-06-29 06:20:16.986914 pretext-1.6.1.dev20230629/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/generate.py
+-rw-r--r--   0        0        0    29108 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/project.py
+-rw-r--r--   0        0        0      739 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-29 06:20:17.086919 pretext-1.6.1.dev20230629/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-29 06:20:17.086919 pretext-1.6.1.dev20230629/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160110 2023-06-29 06:20:17.050917 pretext-1.6.1.dev20230629/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7616 2023-06-29 06:20:17.054917 pretext-1.6.1.dev20230629/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173309 2023-06-29 06:20:17.082919 pretext-1.6.1.dev20230629/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2192 2023-06-29 06:20:17.086919 pretext-1.6.1.dev20230629/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4657 2023-06-29 06:20:17.066918 pretext-1.6.1.dev20230629/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-29 06:20:17.086919 pretext-1.6.1.dev20230629/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-29 06:20:17.086919 pretext-1.6.1.dev20230629/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8392 2023-06-29 06:20:17.062918 pretext-1.6.1.dev20230629/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    25086 2023-06-29 06:19:31.812368 pretext-1.6.1.dev20230629/pretext/utils.py
+-rw-r--r--   0        0        0     3333 2023-06-29 06:20:11.630612 pretext-1.6.1.dev20230629/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230629/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230628/LICENSE` & `pretext-1.6.1.dev20230629/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/README.md` & `pretext-1.6.1.dev20230629/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/__init__.py` & `pretext-1.6.1.dev20230629/pretext/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = '61af1390d2c4f631f1cc6affc27bebdd0db1dfe9'
+CORE_COMMIT = '4da2a0f824785143c917c0f16007cbd0d48ba88d'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.6.1.dev20230628/pretext/build.py` & `pretext-1.6.1.dev20230629/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/cli.py` & `pretext-1.6.1.dev20230629/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/codechat.py` & `pretext-1.6.1.dev20230629/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230629/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/core/pretext.py` & `pretext-1.6.1.dev20230629/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/core/resources.py` & `pretext-1.6.1.dev20230629/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/core/resources.zip` & `pretext-1.6.1.dev20230629/pretext/core/resources.zip`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
-Zip file size: 1041510 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-28 06:15 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-28 06:15 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-28 06:15 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-28 06:15 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-28 06:15 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-28 06:15 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-28 06:15 pretext/__init__.py
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-28 06:15 pretext/pretext
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-28 06:15 pretext/README.md
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-28 06:15 pretext/pretext.cfg
--rw-r--r--  2.0 unx   172492 b- defN 23-Jun-28 06:15 pretext/pretext.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-28 06:15 pretext/module-test.py
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-28 06:15 pretext/braille_format.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 xsl/utilities/
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-28 06:15 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx   612399 b- defN 23-Jun-28 06:15 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-28 06:15 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Jun-28 06:15 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-28 06:15 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-28 06:15 xsl/README.md
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-28 06:15 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-28 06:15 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-28 06:15 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-28 06:15 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-28 06:15 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx   110044 b- defN 23-Jun-28 06:15 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-28 06:15 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-28 06:15 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-28 06:15 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-28 06:15 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-28 06:15 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   544229 b- defN 23-Jun-28 06:15 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-28 06:15 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-28 06:15 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-28 06:15 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx   112450 b- defN 23-Jun-28 06:15 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-28 06:15 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-28 06:15 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-28 06:15 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-28 06:15 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-28 06:15 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-28 06:15 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-28 06:15 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-28 06:15 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-28 06:15 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-28 06:15 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-28 06:15 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-28 06:15 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-28 06:15 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-28 06:15 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-28 06:15 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-28 06:15 xsl/entities.ent
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-28 06:15 xsl/pretext-json-manifest.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-28 06:15 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-28 06:15 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-28 06:15 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-28 06:15 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-28 06:15 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-28 06:15 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-28 06:15 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-28 06:15 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-28 06:15 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-28 06:15 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-28 06:15 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-28 06:15 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-28 06:15 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-28 06:15 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-28 06:15 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-28 06:15 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Jun-28 06:15 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-28 06:15 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx     4760 b- defN 23-Jun-28 06:15 xsl/localizations/README.md
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-28 06:15 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-28 06:15 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-28 06:15 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-28 06:15 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-28 06:15 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    20465 b- defN 23-Jun-28 06:15 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-28 06:15 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-28 06:15 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-28 06:15 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    15850 b- defN 23-Jun-28 06:15 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-28 06:15 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-28 06:15 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-28 06:15 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-28 06:15 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-28 06:15 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-28 06:15 xsl/utilities/README.md
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-28 06:15 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-28 06:15 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-28 06:15 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-28 06:15 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-28 06:15 schema/pretext-dev.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-28 06:15 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-28 06:15 schema/README.md
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-28 06:15 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-28 06:15 schema/pretext.rng
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-28 06:15 schema/pretext.xml
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-28 06:15 schema/pretext.rnc
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-28 06:15 schema/build.sh
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-28 06:15 schema/xml.xsd
--rw-r--r--  2.0 unx    25870 b- defN 23-Jun-28 06:15 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-28 06:15 schema/pretext.xsd
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-28 06:15 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-28 06:15 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-28 06:15 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-28 06:15 css/update_css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-28 06:15 css/README.md
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-28 06:15 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-28 06:15 css/style_oscarlevin.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-28 06:15 css/mathbook-content.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-28 06:15 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-28 06:15 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-28 06:15 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-28 06:15 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-28 06:15 css/colors_red_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-28 06:15 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-28 06:15 css/colors_green_blue.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-28 06:15 css/epub.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-28 06:15 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-28 06:15 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-28 06:15 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-28 06:15 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-28 06:15 css/kindle.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-28 06:15 css/style_default.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-28 06:15 css/pretext_add_on.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-28 06:15 css/setcolors.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-28 06:15 css/style_soundwriting.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-28 06:15 css/colors_blue_green.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-28 06:15 css/colors_brown_gold.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-28 06:15 css/mathbook-3.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-28 06:15 css/mathbook-add-on.css
-142 files, 4836058 bytes uncompressed, 1023936 bytes compressed:  78.8%
+Zip file size: 1042093 bytes, number of entries: 142
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-29 06:20 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-29 06:20 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-29 06:20 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-29 06:20 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 06:20 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-29 06:20 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 06:20 pretext/__init__.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-29 06:20 pretext/pretext
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-29 06:20 pretext/README.md
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-29 06:20 pretext/pretext.cfg
+-rw-r--r--  2.0 unx   172492 b- defN 23-Jun-29 06:20 pretext/pretext.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-29 06:20 pretext/module-test.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-29 06:20 pretext/braille_format.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 xsl/utilities/
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-29 06:20 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx   612195 b- defN 23-Jun-29 06:20 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-29 06:20 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Jun-29 06:20 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-29 06:20 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-29 06:20 xsl/README.md
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-29 06:20 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-29 06:20 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   548426 b- defN 23-Jun-29 06:20 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-29 06:20 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-29 06:20 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx   110044 b- defN 23-Jun-29 06:20 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-29 06:20 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-29 06:20 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-29 06:20 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-29 06:20 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-29 06:20 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jun-29 06:20 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-29 06:20 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-29 06:20 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-29 06:20 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jun-29 06:20 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-29 06:20 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-29 06:20 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-29 06:20 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-29 06:20 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-29 06:20 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-29 06:20 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-29 06:20 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-29 06:20 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-29 06:20 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-29 06:20 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-29 06:20 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-29 06:20 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-29 06:20 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-29 06:20 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-29 06:20 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-29 06:20 xsl/entities.ent
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-29 06:20 xsl/pretext-json-manifest.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-29 06:20 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-29 06:20 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-29 06:20 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-29 06:20 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-29 06:20 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-29 06:20 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-29 06:20 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-29 06:20 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-29 06:20 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-29 06:20 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-29 06:20 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-29 06:20 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-29 06:20 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-29 06:20 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-29 06:20 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    17056 b- defN 23-Jun-29 06:20 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Jun-29 06:20 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    16534 b- defN 23-Jun-29 06:20 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx     4760 b- defN 23-Jun-29 06:20 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    17231 b- defN 23-Jun-29 06:20 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16837 b- defN 23-Jun-29 06:20 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16349 b- defN 23-Jun-29 06:20 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16500 b- defN 23-Jun-29 06:20 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17081 b- defN 23-Jun-29 06:20 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    20481 b- defN 23-Jun-29 06:20 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    17301 b- defN 23-Jun-29 06:20 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    19185 b- defN 23-Jun-29 06:20 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    15582 b- defN 23-Jun-29 06:20 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    15866 b- defN 23-Jun-29 06:20 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16252 b- defN 23-Jun-29 06:20 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16312 b- defN 23-Jun-29 06:20 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    19326 b- defN 23-Jun-29 06:20 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    16085 b- defN 23-Jun-29 06:20 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-29 06:20 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-29 06:20 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-29 06:20 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-29 06:20 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-29 06:20 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-29 06:20 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-29 06:20 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-29 06:20 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-29 06:20 schema/README.md
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-29 06:20 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-29 06:20 schema/pretext.rng
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-29 06:20 schema/pretext.xml
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-29 06:20 schema/pretext.rnc
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-29 06:20 schema/build.sh
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-29 06:20 schema/xml.xsd
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jun-29 06:20 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-29 06:20 schema/pretext.xsd
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-29 06:20 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-29 06:20 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-29 06:20 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-29 06:20 css/update_css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-29 06:20 css/README.md
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-29 06:20 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-29 06:20 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-29 06:20 css/mathbook-content.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-29 06:20 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-29 06:20 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-29 06:20 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-29 06:20 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-29 06:20 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-29 06:20 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-29 06:20 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-29 06:20 css/epub.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-29 06:20 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-29 06:20 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-29 06:20 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-29 06:20 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-29 06:20 css/kindle.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-29 06:20 css/style_default.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-29 06:20 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-29 06:20 css/setcolors.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-29 06:20 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-29 06:20 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-29 06:20 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-29 06:20 css/mathbook-3.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-29 06:20 css/mathbook-add-on.css
+142 files, 4837859 bytes uncompressed, 1024519 bytes compressed:  78.8%
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -12227,22 +12227,15 @@
   <!-- and come through as a key; but perhaps this template    -->
   <!-- can stay as is.                                         -->
   <xsl:template name="language-attributes">
     <xsl:attribute name="lang">
       <xsl:value-of select="$document-language"/>
     </xsl:attribute>
     <xsl:attribute name="dir">
-      <xsl:choose>
-        <xsl:when test="$document-language = 'ku-CKB'">
-          <xsl:text>rtl</xsl:text>
-        </xsl:when>
-        <xsl:otherwise>
-          <xsl:text>ltr</xsl:text>
-        </xsl:otherwise>
-      </xsl:choose>
+      <xsl:value-of select="$document-language-direction"/>
     </xsl:attribute>
   </xsl:template>
   <!-- ############## -->
   <!-- LaTeX Preamble -->
   <!-- ############## -->
   <!-- First a variable to massage the author-supplied -->
   <!-- package list to the form MathJax expects        -->
```

#### xsl/pretext-common.xsl

##### xsl/pretext-common.xsl

```diff
@@ -2114,17 +2114,26 @@
             <xsl:message>PTX:BUG:     asking if a &quot;frontmatter&quot; is a leaf, for a document that is not a &quot;book&quot; nor an &quot;article&quot;</xsl:message>
           </xsl:otherwise>
         </xsl:choose>
       </xsl:when>
       <xsl:when test="self::backmatter">
         <xsl:value-of select="false()"/>
       </xsl:when>
+      <!-- The presence of a traditional division is emblematic of a structured -->
+      <!-- division, so not a leaf of the structural/document tree              -->
       <xsl:when test="part or chapter or section or subsection or subsubsection">
         <xsl:value-of select="false()"/>
       </xsl:when>
+      <!-- One exception, a division full of only "worksheet" (as a subdivision, -->
+      <!-- there could be metadata, "introduction", etc.)  We know there are no  -->
+      <!-- traditional divisions as subdiivisions at this point.  So we test for -->
+      <!-- at least one worksheet and no other specialized divisions.            -->
+      <xsl:when test="worksheet and not(exercises|references|glossary|reading-questions|solutions)">
+        <xsl:value-of select="false()"/>
+      </xsl:when>
       <xsl:otherwise>
         <xsl:value-of select="true()"/>
       </xsl:otherwise>
     </xsl:choose>
   </xsl:template>
   <!-- This once just returned false,      -->
   <!-- but should maybe not even be called -->
@@ -3273,14 +3282,28 @@
     </xsl:choose>
   </xsl:template>
   <!-- And with no better match, the default is  -->
   <!-- the PreTeXt name for the element itself. -->
   <xsl:template match="*" mode="string-id">
     <xsl:value-of select="local-name(.)"/>
   </xsl:template>
+  <!-- ################## -->
+  <!-- Language direction -->
+  <!-- ################## -->
+  <!-- Every localiztion should specify the direction of the  -->
+  <!-- language, which we record as a variable and as a flag. -->
+  <xsl:variable name="document-language-direction">
+    <xsl:value-of select="$localizations/locale[@language = $document-language]/@direction"/>
+  </xsl:variable>
+  <!-- We consider right-to-left as exceptional, so we set a flag   -->
+  <!-- for this case.  This should be the primary determinant in    -->
+  <!-- code such as the LaTeX coionversion, though the actual value -->
+  <!-- of "$language-direction" is meant to be used in attributes   -->
+  <!-- for HTML pages.                                              -->
+  <xsl:variable name="b-rtl" select="$document-language-direction = 'rtl'"/>
   <!-- ##### -->
   <!-- Icons -->
   <!-- ##### -->
   <!-- Comments are Unicode names, from fileformat.info -->
   <!-- @latex takes priority for LaTeX output when the  -->
   <!-- Font Awesome name has changed, but the LaTeX     -->
   <!-- package is lagging.  This needs to be in the     -->
```

#### xsl/localizations/bg-BG.xml

##### xsl/localizations/bg-BG.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- bg-BG, Bulgarian (Bulgaria) -->
 <!-- Boyko Bantchev, bantchev@gmail.com, 2019-07-04 -->
-<locale language="bg-BG">
+<locale language="bg-BG" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Теорема</localization>
   <localization string-id="corollary">Следствие</localization>
   <localization string-id="lemma">Лема</localization>
   <localization string-id="algorithm">Алгоритъм</localization>
   <localization string-id="proposition">Предложение</localization>
```

#### xsl/localizations/es-ES.xml

##### xsl/localizations/es-ES.xml

```diff
@@ -17,15 +17,15 @@
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- es-ES, Spanish (Spain) -->
 <!-- Juan José Torrens, jjtorrens@unavarra.es, 2014-10-27 -->
 <!-- Julian Pfeifle, julian.pfeifle@upc.edu, 2020-05-28 -->
-<locale language="es-ES">
+<locale language="es-ES" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Teorema</localization>
   <localization string-id="corollary">Corolario</localization>
   <localization string-id="lemma">Lema</localization>
   <localization string-id="algorithm">Algoritmo</localization>
   <localization string-id="proposition">Proposición</localization>
```

#### xsl/localizations/de-DE.xml

##### xsl/localizations/de-DE.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- de-DE, German (Germany) -->
 <!-- Karl-Dieter Crisman, kcrisman@gmail.com, 2020-06-01   -->
-<locale language="de-DE">
+<locale language="de-DE" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Satz</localization>
   <localization string-id="corollary">Korollar</localization>
   <localization string-id="lemma">Hilfssatz</localization>
   <localization string-id="algorithm">Algorithmus</localization>
   <localization string-id="proposition">Proposition</localization>
```

#### xsl/localizations/af-ZA.xml

##### xsl/localizations/af-ZA.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- af-ZA, Afrikaans (South Africa) -->
 <!-- Dirk Basson, djbasson@sun.ac.za, 2018-03-23 -->
-<locale language="af-ZA">
+<locale language="af-ZA" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Stelling</localization>
   <localization string-id="corollary">Gevolg</localization>
   <localization string-id="lemma">Hulpstelling</localization>
   <!-- Or "Lemma" as well -->
   <localization string-id="algorithm">Algoritme</localization>
```

#### xsl/localizations/fr-FR.xml

##### xsl/localizations/fr-FR.xml

```diff
@@ -15,15 +15,15 @@
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- fr-FR, French (France) -->
 <!-- Thomas W. Judson, judsontw@sfasu.edu, 2016-03-23 -->
 <!-- Julien Giol, julien.giol@gmail.com, 2018-02-05   -->
 <!-- Jean-Sébastien Turcotte, js.turcotte@cgodin.qc.ca, 2021-02-19-->
 <!-- If/when a new string-id gets translated in French for the first time, it should also be translated into fr-CA -->
-<locale language="fr-FR">
+<locale language="fr-FR" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Théorème</localization>
   <localization string-id="corollary">Corollaire</localization>
   <localization string-id="lemma">Lemme</localization>
   <localization string-id="algorithm">Algorithme</localization>
   <localization string-id="proposition">Proposition</localization>
```

#### xsl/localizations/fr-CA.xml

##### xsl/localizations/fr-CA.xml

```diff
@@ -14,15 +14,15 @@
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- fr-CA, French (Canada) -->
 <!-- based on initial fr-FR translation -->
 <!-- Jean-Sébastien Turcotte, js.turcotte@cgodin.qc.ca, 2021-02-19-->
 <!-- If/when a new string-id gets translated in French for the first time, it should also be translated into fr-FR -->
-<locale language="fr-CA">
+<locale language="fr-CA" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Théorème</localization>
   <localization string-id="corollary">Corollaire</localization>
   <localization string-id="lemma">Lemme</localization>
   <localization string-id="algorithm">Algorithme</localization>
   <localization string-id="proposition">Proposition</localization>
```

#### xsl/localizations/pt-PT.xml

##### xsl/localizations/pt-PT.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- pt-PT, Portugese (Portugal) -->
 <!-- António Pereira, apereiraua@gmail.com, 2015-07-26 -->
-<locale language="pt-PT">
+<locale language="pt-PT" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Teorema</localization>
   <localization string-id="corollary">Corolário</localization>
   <localization string-id="lemma">Lema</localization>
   <localization string-id="algorithm">Algoritmo</localization>
   <localization string-id="proposition">Proposição</localization>
```

#### xsl/localizations/ku-CKB.xml

##### xsl/localizations/ku-CKB.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- ku-CKB, Kurdish (Cental Kurdish) -->
 <!-- Rebin Muhammad, reben80@gmail.com, 2023-06-24 -->
-<locale language="ku-CKB">
+<locale language="ku-CKB" direction="rtl">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">بیردۆز</localization>
   <localization string-id="corollary">ئاکام</localization>
   <localization string-id="lemma">لێما</localization>
   <localization string-id="algorithm">ئەلگۆریزم</localization>
   <localization string-id="proposition">دەستەواژە</localization>
```

#### xsl/localizations/fi-FI.xml

##### xsl/localizations/fi-FI.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- fi-FI, Finnish (Finland) -->
 <!-- Lasse M. Manninen lasse.m.manninen@gmail.com   -->
-<locale language="fi-FI">
+<locale language="fi-FI" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Lause</localization>
   <localization string-id="corollary">Seuraus</localization>
   <localization string-id="lemma">Lemma</localization>
   <localization string-id="algorithm">Algoritmi</localization>
   <localization string-id="proposition">Propositio</localization>
```

#### xsl/localizations/nl-NL.xml

##### xsl/localizations/nl-NL.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- nl-NL, Dutch (The Netherlands) -->
 <!-- Gosia Wrzesinska, gosia@coderso.com, 2022-12-21   -->
-<locale language="nl-NL">
+<locale language="nl-NL" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Stelling</localization>
   <localization string-id="corollary">Gevolg</localization>
   <localization string-id="lemma">Lemma</localization>
   <localization string-id="algorithm">Algoritme</localization>
   <localization string-id="proposition">Propositie</localization>
```

#### xsl/localizations/cs-CZ.xml

##### xsl/localizations/cs-CZ.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- cs-CZ, Czech (Czechia) -->
 <!-- Jiri Lebl, lebl@okstate.edu, 2023-05-21   -->
-<locale language="cs-CZ">
+<locale language="cs-CZ" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Teorém</localization>
   <localization string-id="corollary">Důsledek</localization>
   <localization string-id="lemma">Lemma</localization>
   <localization string-id="algorithm">Algoritmus</localization>
   <localization string-id="proposition">Věta</localization>
```

#### xsl/localizations/it-IT.xml

##### xsl/localizations/it-IT.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- it-IT, Italian (Italy) -->
 <!-- Valerio Monti, gedeonedepaperoni@gmail.com, 2020-07-27   -->
-<locale language="it-IT">
+<locale language="it-IT" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Teorema</localization>
   <localization string-id="corollary">Corollario</localization>
   <localization string-id="lemma">Lemma</localization>
   <localization string-id="algorithm">Algoritmo</localization>
   <localization string-id="proposition">Proposizione</localization>
```

#### xsl/localizations/ca-ES.xml

##### xsl/localizations/ca-ES.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- ca-ES, Catalan (Spain) -->
 <!-- Jordi Saludes, jordi.saludes@upc.edu, 2021-07-13 -->
-<locale language="ca-ES">
+<locale language="ca-ES" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Teorema</localization>
   <localization string-id="corollary">Corol·lari</localization>
   <localization string-id="lemma">Lema</localization>
   <localization string-id="algorithm">Algorisme</localization>
   <localization string-id="proposition">Proposició</localization>
```

#### xsl/localizations/pt-BR.xml

##### xsl/localizations/pt-BR.xml

```diff
@@ -18,15 +18,15 @@
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- pt-BR, Portugese (Brazil)-->
 <!-- Igor Morgado, morgado.igor@gmail.com, 2014-08-11, 2014-08-14 -->
 <!-- Vinicius Monego, monego@posteo.net, 2020-11-07 -->
 <!-- Leon Silva, leon.silva@ufrpe.br, 2022-03-30 -->
-<locale language="pt-BR">
+<locale language="pt-BR" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Teorema</localization>
   <localization string-id="corollary">Corolário</localization>
   <localization string-id="lemma">Lema</localization>
   <localization string-id="algorithm">Algoritmo</localization>
   <localization string-id="proposition">Proposição</localization>
```

#### xsl/localizations/en-US.xml

##### xsl/localizations/en-US.xml

```diff
@@ -16,16 +16,19 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- en-US, English (United States) -->
 <!-- Robert A. Beezer, beezer@pugetsound.edu, 2014-08-11   -->
-<!-- <locale language="en-US"> -->
-<locale language="en-US">
+<!-- Every localization should specify the direction of the language, -->
+<!-- there is no assumed default.  Left-to-right is "ltr" and         -->
+<!-- right-to-left is "rtl".  Provide these exactly as written since  -->
+<!-- they can migrate untouched into output (e.g. HTML).              -->
+<locale language="en-US" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Theorem</localization>
   <localization string-id="corollary">Corollary</localization>
   <localization string-id="lemma">Lemma</localization>
   <localization string-id="algorithm">Algorithm</localization>
   <localization string-id="proposition">Proposition</localization>
```

#### xsl/localizations/hu-HU.xml

##### xsl/localizations/hu-HU.xml

```diff
@@ -16,15 +16,15 @@
 
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!-- See  xsl/localizations/README.md  for an explanation of this file -->
 <!-- hu-HU, Hungarian (Hungary) -->
 <!-- Sándor Czirbusz, czirbusz@gmail.com, 2017-04-09 -->
-<locale language="hu-HU">
+<locale language="hu-HU" direction="ltr">
   <!-- THEOREM-LIKE blocks -->
   <!-- Environments which have proofs, plus proofs themselves -->
   <localization string-id="theorem">Tétel</localization>
   <localization string-id="corollary">Következmény</localization>
   <localization string-id="lemma">Lemma</localization>
   <localization string-id="algorithm">Algoritmus</localization>
   <localization string-id="proposition">Állítás</localization>
```

### Comparing `pretext-1.6.1.dev20230628/pretext/generate.py` & `pretext-1.6.1.dev20230629/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/project.py` & `pretext-1.6.1.dev20230629/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230629/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230629/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230629/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160110 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 source/
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-28 06:15 project.ptx
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-28 06:14 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-28 06:15 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-28 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-28 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-28 06:14 assets/frog.jpg
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-28 06:14 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-28 06:14 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-28 06:14 source/main.ptx
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-28 06:14 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-29 06:20 project.ptx
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-29 06:19 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-29 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-29 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-29 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-29 06:19 assets/frog.jpg
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-29 06:19 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-29 06:19 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-29 06:19 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-29 06:19 publication/publication.ptx
 14 files, 164841 bytes uncompressed, 158588 bytes compressed:  3.8%
```

### Comparing `pretext-1.6.1.dev20230628/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230629/pretext/templates/resources/book.zip`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7616 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 source/
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-28 06:15 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-28 06:14 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-28 06:15 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-28 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-28 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-28 06:14 source/main.ptx
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-28 06:14 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-29 06:20 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-29 06:19 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-29 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-29 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-29 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-29 06:19 source/main.ptx
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-29 06:19 publication/publication.ptx
 10 files, 15809 bytes uncompressed, 6522 bytes compressed:  58.7%
```

### Comparing `pretext-1.6.1.dev20230628/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230629/pretext/templates/resources/demo.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173309 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 source/
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-28 06:15 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-28 06:14 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-28 06:15 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-28 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-28 06:15 .devcontainer/devcontainer.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-28 06:14 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-28 06:14 assets/jsxgraph/infinity.js
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 source/images/
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-28 06:14 source/ex-first.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-28 06:14 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-28 06:14 source/ch-empty.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-28 06:14 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-28 06:14 source/frontmatter.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-28 06:14 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-28 06:14 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-28 06:14 source/sec-features.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-28 06:14 source/fig-tikz.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-28 06:14 source/ch-generate.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-28 06:14 source/ch-features.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-28 06:14 source/docinfo.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-28 06:14 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-28 06:14 source/main.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-28 06:14 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-28 06:14 source/backmatter.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-28 06:14 source/images/cflag.asy
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-28 06:14 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-28 06:14 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-28 06:14 source/images/tikz.tex
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-28 06:14 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-29 06:20 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-29 06:19 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-29 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-29 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-29 06:20 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-29 06:19 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-29 06:19 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 source/images/
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-29 06:19 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-29 06:19 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-29 06:19 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-29 06:19 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-29 06:19 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-29 06:19 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-29 06:19 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-29 06:19 source/sec-features.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-29 06:19 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-29 06:19 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-29 06:19 source/ch-features.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-29 06:19 source/docinfo.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-29 06:19 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-29 06:19 source/main.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-29 06:19 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-29 06:19 source/backmatter.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-29 06:19 source/images/cflag.asy
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-29 06:19 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-29 06:19 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-29 06:19 source/images/tikz.tex
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-29 06:19 publication/publication.ptx
 34 files, 190104 bytes uncompressed, 169353 bytes compressed:  10.9%
```

### Comparing `pretext-1.6.1.dev20230628/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230629/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230629/pretext/templates/resources/hello.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4657 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 source/
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-28 06:14 project.ptx
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-28 06:14 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-28 06:15 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-28 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-28 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-28 06:14 source/main.ptx
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-28 06:14 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 source/
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-29 06:19 project.ptx
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-29 06:19 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-29 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-29 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-29 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-29 06:19 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-29 06:19 publication/publication.ptx
 10 files, 7820 bytes uncompressed, 3563 bytes compressed:  54.4%
```

### Comparing `pretext-1.6.1.dev20230628/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230629/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230629/pretext/templates/resources/slideshow.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8392 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 06:14 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-28 06:14 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-28 06:15 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-28 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-28 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-28 06:14 xsl/slides.xsl
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-28 06:14 source/main.ptx
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-28 06:14 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-29 06:19 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-29 06:19 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-29 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-29 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-29 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-29 06:19 xsl/slides.xsl
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-29 06:19 source/main.ptx
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-29 06:19 publication/publication.ptx
 11 files, 20407 bytes uncompressed, 7204 bytes compressed:  64.7%
```

### Comparing `pretext-1.6.1.dev20230628/pretext/utils.py` & `pretext-1.6.1.dev20230629/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230628/pyproject.toml` & `pretext-1.6.1.dev20230629/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230628"
+version = "1.6.1.dev20230629"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230628/PKG-INFO` & `pretext-1.6.1.dev20230629/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230628
+Version: 1.6.1.dev20230629
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

