# Comparing `tmp/topic_wizard-0.2.6.tar.gz` & `tmp/topic_wizard-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic_wizard-0.2.6.tar", max compression
+gzip compressed data, was "topic_wizard-0.3.0.tar", max compression
```

## Comparing `topic_wizard-0.2.6.tar` & `topic_wizard-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,51 @@
--rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.2.6/LICENSE
--rw-r--r--   0        0        0     2908 2023-05-17 11:35:28.098112 topic_wizard-0.2.6/README.md
--rw-r--r--   0        0        0      640 2023-06-26 07:38:06.759482 topic_wizard-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      404 2023-05-17 10:58:27.942406 topic_wizard-0.2.6/topicwizard/__init__.py
--rw-r--r--   0        0        0     7219 2023-05-17 10:58:27.942406 topic_wizard-0.2.6/topicwizard/app.py
--rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.2.6/topicwizard/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.6/topicwizard/blueprints/__init__.py
--rw-r--r--   0        0        0     5602 2023-02-19 17:44:29.048902 topic_wizard-0.2.6/topicwizard/blueprints/app.py
--rw-r--r--   0        0        0     4322 2023-05-17 11:05:13.211055 topic_wizard-0.2.6/topicwizard/blueprints/documents.py
--rw-r--r--   0        0        0     1091 2023-05-17 13:10:22.409355 topic_wizard-0.2.6/topicwizard/blueprints/groups.py
--rw-r--r--   0        0        0     1985 2023-06-26 07:34:43.425897 topic_wizard-0.2.6/topicwizard/blueprints/template.py
--rw-r--r--   0        0        0     5082 2023-05-17 11:05:33.415089 topic_wizard-0.2.6/topicwizard/blueprints/topics.py
--rw-r--r--   0        0        0     3015 2023-05-17 11:05:57.615132 topic_wizard-0.2.6/topicwizard/blueprints/words.py
--rw-r--r--   0        0        0     3010 2023-05-17 11:32:05.865790 topic_wizard-0.2.6/topicwizard/compatibility/bertopic.py
--rw-r--r--   0        0        0     6425 2023-05-17 11:33:07.273886 topic_wizard-0.2.6/topicwizard/compatibility/gensim.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.6/topicwizard/components/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.6/topicwizard/components/documents/__init__.py
--rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.2.6/topicwizard/components/documents/document_map.py
--rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.2.6/topicwizard/components/documents/document_pie.py
--rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.2.6/topicwizard/components/documents/document_selector.py
--rw-r--r--   0        0        0     1468 2023-04-24 14:04:50.954173 topic_wizard-0.2.6/topicwizard/components/documents/document_timeline.py
--rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/documents/document_wordcloud.py
--rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/documents/window_slider.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/__init__.py
--rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/intertopic_map.py
--rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/relevance_slider.py
--rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/topic_barplot.py
--rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/topic_namer.py
--rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/topic_switcher.py
--rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/wordcloud.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/words/__init__.py
--rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.2.6/topicwizard/components/words/association_slider.py
--rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/words/word_barplot.py
--rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.2.6/topicwizard/components/words/word_map.py
--rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.2.6/topicwizard/components/words/word_selector.py
--rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.2.6/topicwizard/plots/__init__.py
--rw-r--r--   0        0        0     5183 2023-05-17 10:58:27.942406 topic_wizard-0.2.6/topicwizard/plots/documents.py
--rw-r--r--   0        0        0     4257 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/plots/topics.py
--rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.2.6/topicwizard/plots/words.py
--rw-r--r--   0        0        0     2708 2023-04-24 13:29:18.682128 topic_wizard-0.2.6/topicwizard/prepare/documents.py
--rw-r--r--   0        0        0     3681 2023-05-17 13:42:09.111617 topic_wizard-0.2.6/topicwizard/prepare/groups.py
--rw-r--r--   0        0        0     4895 2023-05-17 10:58:27.942406 topic_wizard-0.2.6/topicwizard/prepare/topics.py
--rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.2.6/topicwizard/prepare/utils.py
--rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.2.6/topicwizard/prepare/words.py
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 topic_wizard-0.2.6/setup.py
--rw-r--r--   0        0        0     3931 1970-01-01 00:00:00.000000 topic_wizard-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3746 2023-06-30 16:33:58.855285 topic_wizard-0.3.0/README.md
+-rw-r--r--   0        0        0      640 2023-06-30 16:34:27.363320 topic_wizard-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-06-30 14:25:27.164990 topic_wizard-0.3.0/topicwizard/__init__.py
+-rw-r--r--   0        0        0     8707 2023-06-30 16:17:44.330421 topic_wizard-0.3.0/topicwizard/app.py
+-rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.3.0/topicwizard/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.0/topicwizard/blueprints/__init__.py
+-rw-r--r--   0        0        0     6348 2023-06-30 14:13:08.495596 topic_wizard-0.3.0/topicwizard/blueprints/app.py
+-rw-r--r--   0        0        0     4322 2023-05-17 11:05:13.211055 topic_wizard-0.3.0/topicwizard/blueprints/documents.py
+-rw-r--r--   0        0        0     1091 2023-05-17 13:10:22.409355 topic_wizard-0.3.0/topicwizard/blueprints/groups.py
+-rw-r--r--   0        0        0     2338 2023-06-30 14:20:46.656474 topic_wizard-0.3.0/topicwizard/blueprints/template.py
+-rw-r--r--   0        0        0     4979 2023-06-30 14:12:57.739575 topic_wizard-0.3.0/topicwizard/blueprints/topics.py
+-rw-r--r--   0        0        0     3015 2023-05-17 11:05:57.615132 topic_wizard-0.3.0/topicwizard/blueprints/words.py
+-rw-r--r--   0        0        0     3010 2023-05-17 11:32:05.865790 topic_wizard-0.3.0/topicwizard/compatibility/bertopic.py
+-rw-r--r--   0        0        0     6425 2023-05-17 11:33:07.273886 topic_wizard-0.3.0/topicwizard/compatibility/gensim.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.0/topicwizard/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.0/topicwizard/components/documents/__init__.py
+-rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.3.0/topicwizard/components/documents/document_map.py
+-rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.3.0/topicwizard/components/documents/document_pie.py
+-rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.3.0/topicwizard/components/documents/document_selector.py
+-rw-r--r--   0        0        0     1468 2023-04-24 14:04:50.954173 topic_wizard-0.3.0/topicwizard/components/documents/document_timeline.py
+-rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/documents/document_wordcloud.py
+-rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/documents/window_slider.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/__init__.py
+-rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/intertopic_map.py
+-rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/relevance_slider.py
+-rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/topic_barplot.py
+-rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/topic_namer.py
+-rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/topic_switcher.py
+-rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/topics/wordcloud.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/words/__init__.py
+-rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.3.0/topicwizard/components/words/association_slider.py
+-rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.3.0/topicwizard/components/words/word_barplot.py
+-rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.3.0/topicwizard/components/words/word_map.py
+-rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.3.0/topicwizard/components/words/word_selector.py
+-rw-r--r--   0        0        0      498 2023-06-30 13:57:55.717853 topic_wizard-0.3.0/topicwizard/figures/__init__.py
+-rw-r--r--   0        0        0     7715 2023-06-30 16:01:00.587374 topic_wizard-0.3.0/topicwizard/figures/documents.py
+-rw-r--r--   0        0        0     9340 2023-06-30 13:03:18.543793 topic_wizard-0.3.0/topicwizard/figures/topics.py
+-rw-r--r--   0        0        0     6392 2023-06-30 15:39:09.394441 topic_wizard-0.3.0/topicwizard/figures/words.py
+-rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.3.0/topicwizard/plots/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-17 10:58:27.942406 topic_wizard-0.3.0/topicwizard/plots/documents.py
+-rw-r--r--   0        0        0     4244 2023-06-26 12:14:28.818856 topic_wizard-0.3.0/topicwizard/plots/topics.py
+-rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.3.0/topicwizard/plots/words.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:10:25.930511 topic_wizard-0.3.0/topicwizard/prepare/__init__.py
+-rw-r--r--   0        0        0     2708 2023-06-26 13:03:03.519611 topic_wizard-0.3.0/topicwizard/prepare/documents.py
+-rw-r--r--   0        0        0     3681 2023-05-17 13:42:09.111617 topic_wizard-0.3.0/topicwizard/prepare/groups.py
+-rw-r--r--   0        0        0     4895 2023-05-17 10:58:27.942406 topic_wizard-0.3.0/topicwizard/prepare/topics.py
+-rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.3.0/topicwizard/prepare/utils.py
+-rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.3.0/topicwizard/prepare/words.py
+-rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 topic_wizard-0.3.0/setup.py
+-rw-r--r--   0        0        0     4769 1970-01-01 00:00:00.000000 topic_wizard-0.3.0/PKG-INFO
```

### Comparing `topic_wizard-0.2.6/LICENSE` & `topic_wizard-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/README.md` & `topic_wizard-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 
 
 
 https://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4
 
-## New in version 0.2.5 🌟 🌟
+## New in version 0.3.0 🌟 🌟
 
- - [Compatiblity with Gensim topic models](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html) 💥
- - [Compatibility with BERTopic](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html)(experimental 🧪)
- - Topic name inference 🧠
+ - Exclude pages, that are not needed :bird:
+ - Self-contained interactive figures :gift:
+ - Topic name inference is now default behavior and is done implicitly.
 
 
 ## Features
 
 -   Investigate complex relations between topics, words and documents
 -   Highly interactive
 -   Automatically infer topic names
@@ -62,37 +62,71 @@
     NMF(n_components=10),
 )
 
 # Then fit it on the given texts
 topic_pipeline.fit(texts)
 ```
 
-### Step 2:
+### Step 2a:
 
-Visualize with topicwizard.
+Visualize with the topicwizard webapp :bulb:
 
 ```python
 import topicwizard
 
-# You can get automatically assigned topic labels, that you can change manually later
-topic_names = topicwizard.infer_topic_names(pipeline=pipeline)
-
-# Then you can visualize your results
-topicwizard.visualize(pipeline=topic_pipeline, corpus=texts, topic_names=topic_names)
+topicwizard.visualize(pipeline=topic_pipeline, corpus=texts)
 ```
 
-### Step 3:
+From version 0.3.0 you can also disable pages you do not wish to display thereby sparing a lot of time for yourself:
 
-Investigate :eyes: .
+```python
+import topicwizard
 
-#### a) Topics
+# A large corpus takes a looong time to compute 2D projections for so
+# so you can speed up preprocessing by disabling it alltogether.
+topicwizard.visualize(pipeline=topic_pipeline, corpus=texts, exclude_pages=["documents"])
+```
 
 ![topics screenshot](assets/screenshot_topics.png)
-
-#### b) Words
-
 ![words screenshot](assets/screenshot_words.png)
 ![words screenshot](assets/screenshot_words_zoomed.png)
+![documents screenshot](assets/screenshot_documents.png)
 
-#### c) Documents
+Ooooor...
 
-![documents screenshot](assets/screenshot_documents.png)
+### Step 2b:
+
+Produce high quality self-contained HTML plots and create your own dashboards/reports :strawberry:
+
+### Map of words
+
+```python
+from topicwizard.figures import word_map
+
+word_map(corpus=texts, pipeline=pipeline)
+```
+
+![word map screenshot](assets/word_map.png)
+
+### Timelines of topic distributions
+
+```python
+from topicwizard.figures import document_topic_timeline
+
+document_topic_timeline(
+    "Joe Biden takes over presidential office from Donald Trump.",
+    pipeline=pipeline,
+)
+```
+![document timeline](assets/document_topic_timeline.png)
+
+### Wordclouds of your topics :cloud:
+
+```python
+from topicwizard.figures import topic_wordclouds
+
+topic_wordclouds(corpus=texts, pipeline=pipeline)
+```
+
+![wordclouds](assets/topic_wordclouds.png)
+
+### And much more ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))
```

### Comparing `topic_wizard-0.2.6/pyproject.toml` & `topic_wizard-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "topic-wizard"
-version = "0.2.6"
+version = "0.3.0"
 description = "Pretty and opinionated topic model visualization in Python."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "topicwizard"}]
 
 [tool.poetry.dependencies]
```

### Comparing `topic_wizard-0.2.6/topicwizard/app.py` & `topic_wizard-0.3.0/topicwizard/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import subprocess
 import sys
 import threading
 import time
-from typing import Any, Callable, Iterable, List, Optional
+from typing import Any, Callable, Iterable, List, Literal, Optional, Set
 
 import joblib
 from dash_extensions.enrich import Dash, DashBlueprint
 from sklearn.pipeline import Pipeline
 
 from topicwizard.blueprints.app import create_blueprint
 from topicwizard.blueprints.template import prepare_blueprint
@@ -23,30 +23,38 @@
 
 def get_app_blueprint(
     vectorizer: Any,
     topic_model: Any,
     corpus: Iterable[str],
     document_names: Optional[List[str]] = None,
     topic_names: Optional[List[str]] = None,
+    *args,
+    **kwargs,
 ) -> DashBlueprint:
     blueprint = prepare_blueprint(
         vectorizer=vectorizer,
         topic_model=topic_model,
         corpus=corpus,
         document_names=document_names,
         topic_names=topic_names,
         create_blueprint=create_blueprint,
+        *args,
+        **kwargs,
     )
     return blueprint
 
 
+PageName = Literal["topics", "documents", "words"]
+
+
 def get_dash_app(
     vectorizer: Any,
     topic_model: Any,
     corpus: Iterable[str],
+    exclude_pages: Set[PageName],
     document_names: Optional[List[str]] = None,
     topic_names: Optional[List[str]] = None,
 ) -> Dash:
     """Returns topicwizard Dash application.
 
     Parameters
     ----------
@@ -58,28 +66,29 @@
         into topic distributions.
     corpus: iterable of str
         List of all works in the corpus you intend to visualize.
     document_names: list of str, default None
         List of document names in the corpus, if not provided documents will
         be labeled 'Document <index>'.
     topic_names: list of str, default None
-        List of topic names in the corpus, if not provided topics will initially
-        be labeled 'Topic <index>'.
+        List of topic names in the corpus, if not provided, topic
+        labels will be inferred.
 
     Returns
     -------
     Dash
         Dash application object for topicwizard.
     """
     blueprint = get_app_blueprint(
         vectorizer=vectorizer,
         topic_model=topic_model,
         corpus=corpus,
         document_names=document_names,
         topic_names=topic_names,
+        exclude_pages=exclude_pages,
     )
     app = Dash(
         __name__,
         blueprint=blueprint,
         title="topicwizard",
         external_scripts=[
             {
@@ -90,29 +99,29 @@
                 "crossorigin": "anonymous",
             },
         ],
     )
     return app
 
 
-def load_app(filename: str) -> Dash:
+def load_app(filename: str, exclude_pages: Set[PageName]) -> Dash:
     """Loads and prepares saved app from disk.
 
     Parameters
     ----------
     filename: str
         Path to the file where the data is stored.
 
     Returns
     -------
     Dash
         Dash application.
     """
     data = joblib.load(filename)
-    return get_dash_app(**data)
+    return get_dash_app(**data, exclude_pages=exclude_pages)
 
 
 def open_url(url: str) -> None:
     if sys.platform == "win32":
         os.startfile(url)
     elif sys.platform == "darwin":
         subprocess.Popen(["open", url])
@@ -166,47 +175,68 @@
     else:
         open_url(url)
         app.run_server(port=port)
 
 
 def load(
     filename: str,
+    exclude_pages: Optional[Iterable[PageName]] = None,
     port: int = 8050,
 ) -> Optional[threading.Thread]:
     """Visualizes topic model data loaded from disk.
 
     Parameters
     ----------
     filename: str
         Path to the file where the data is stored.
+    exclude_pages: iterable of {"topics", "documents", "words"}
+        Set of pages you want to exclude from the application.
+        This can be relevant as with larger corpora for example,
+        calculating UMAP embeddings for documents or words can take
+        a long time and you might not be interested in them.
     port: int, default 8050
         Port where the application should run in localhost. Defaults to 8050.
-    enable_notebook: bool, default False
-        Specifies whether topicwizard should run in a Jupyter notebook.
 
     Returns
     -------
     Thread or None
         Returns a Thread if running in a Jupyter notebook (so you can close the server)
         returns None otherwise.
     """
     print("Preparing data")
-    app = load_app(filename)
+    exclude_pages = set() if exclude_pages is None else set(exclude_pages)
+    app = load_app(filename, exclude_pages=exclude_pages)
     return run_app(app, port=port)
 
 
+def split_pipeline(
+    vectorizer: Any, topic_model: Any, pipeline: Optional[Pipeline]
+) -> tuple[Any, Any]:
+    """Check which arguments are provided,
+    raises error if the arguments are not satisfactory, and if needed
+    splits Pipeline into vectorizer and topic model."""
+    if (vectorizer is None) or (topic_model is None):
+        if pipeline is None:
+            raise TypeError(
+                "Either pipeline, or vectorizer and topic model have to be provided"
+            )
+        _, vectorizer = pipeline.steps[0]
+        _, topic_model = pipeline.steps[-1]
+    return vectorizer, topic_model
+
+
 def visualize(
     corpus: Iterable[str],
     vectorizer: Optional[Any] = None,
     topic_model: Optional[Any] = None,
     pipeline: Optional[Pipeline] = None,
     document_names: Optional[List[str]] = None,
     topic_names: Optional[List[str]] = None,
+    exclude_pages: Optional[Iterable[PageName]] = None,
     port: int = 8050,
-    enable_notebook: bool = False,
 ) -> Optional[threading.Thread]:
     """Visualizes your topic model with topicwizard.
 
     Parameters
     ----------
     corpus: iterable of str
         List of all works in the corpus you intend to visualize.
@@ -220,33 +250,35 @@
         Sklearn compatible pipeline, that has two components:
         a vectorizer and a topic model.
         Ignored if vectorizer and topic_model are provided.
     document_names: list of str, default None
         List of document names in the corpus, if not provided documents will
         be labeled 'Document <index>'.
     topic_names: list of str, default None
-        List of topic names in the corpus, if not provided topics will initially
-        be labeled 'Topic <index>'.
+        List of topic names in the corpus, if not provided topic
+        names will be inferred.
+    exclude_pages: iterable of {"topics", "documents", "words"}
+        Set of pages you want to exclude from the application.
+        This can be relevant as with larger corpora for example,
+        calculating UMAP embeddings for documents or words can take
+        a long time and you might not be interested in them.
     port: int, default 8050
         Port where the application should run in localhost. Defaults to 8050.
 
     Returns
     -------
     Thread or None
         Returns a Thread if running in a Jupyter notebook (so you can close the server)
         returns None otherwise.
     """
-    if (vectorizer is None) and (topic_model is None):
-        assert (
-            pipeline is not None
-        ), "Either pipeline or vectorizer and topic model have to be provided"
-        (_, vectorizer), (_, topic_model) = pipeline.steps
-
+    vectorizer, topic_model = split_pipeline(vectorizer, topic_model, pipeline)
+    exclude_pages = set() if exclude_pages is None else set(exclude_pages)
     print("Preprocessing")
     app = get_dash_app(
         vectorizer=vectorizer,
         topic_model=topic_model,
         corpus=corpus,
         document_names=document_names,
         topic_names=topic_names,
+        exclude_pages=exclude_pages,
     )
     return run_app(app, port=port)
```

### Comparing `topic_wizard-0.2.6/topicwizard/assets/favicon.ico` & `topic_wizard-0.3.0/topicwizard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/blueprints/app.py` & `topic_wizard-0.3.0/topicwizard/blueprints/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,117 @@
-from typing import Any, Dict, List
+from io import BytesIO
+from typing import Any, Dict, List, Set
 
 import dash_mantine_components as dmc
 import joblib
-from io import BytesIO
 import numpy as np
 from dash_extensions.enrich import (
     DashBlueprint,
-    exceptions,
     Input,
     Output,
     State,
     dcc,
+    exceptions,
     html,
 )
 from dash_iconify import DashIconify
 
 import topicwizard.blueprints.documents as documents
 import topicwizard.blueprints.topics as topics
 import topicwizard.blueprints.words as words
+from topicwizard.blueprints.template import create_blank_page
 
 
 def create_blueprint(
     vocab: np.ndarray,
     document_term_matrix: np.ndarray,
     document_topic_matrix: np.ndarray,
     topic_term_matrix: np.ndarray,
     document_names: List[str],
     corpus: List[str],
     vectorizer: Any,
     topic_model: Any,
     topic_names: List[str],
+    exclude_pages: Set[str],
 ) -> DashBlueprint:
     # --------[ Collecting blueprints ]--------
-    topic_blueprint = topics.create_blueprint(
-        vocab=vocab,
-        document_term_matrix=document_term_matrix,
-        document_topic_matrix=document_topic_matrix,
-        topic_term_matrix=topic_term_matrix,
-        document_names=document_names,
-        corpus=corpus,
-        vectorizer=vectorizer,
-        topic_model=topic_model,
-        topic_names=topic_names,
+    topic_blueprint = (
+        topics.create_blueprint(
+            vocab=vocab,
+            document_term_matrix=document_term_matrix,
+            document_topic_matrix=document_topic_matrix,
+            topic_term_matrix=topic_term_matrix,
+            document_names=document_names,
+            corpus=corpus,
+            vectorizer=vectorizer,
+            topic_model=topic_model,
+            topic_names=topic_names,
+        )
+        if "topics" not in exclude_pages
+        else create_blank_page("topics")
     )
-    documents_blueprint = documents.create_blueprint(
-        vocab=vocab,
-        document_term_matrix=document_term_matrix,
-        document_topic_matrix=document_topic_matrix,
-        topic_term_matrix=topic_term_matrix,
-        document_names=document_names,
-        corpus=corpus,
-        vectorizer=vectorizer,
-        topic_model=topic_model,
-        topic_names=topic_names,
+    documents_blueprint = (
+        documents.create_blueprint(
+            vocab=vocab,
+            document_term_matrix=document_term_matrix,
+            document_topic_matrix=document_topic_matrix,
+            topic_term_matrix=topic_term_matrix,
+            document_names=document_names,
+            corpus=corpus,
+            vectorizer=vectorizer,
+            topic_model=topic_model,
+            topic_names=topic_names,
+        )
+        if "documents" not in exclude_pages
+        else create_blank_page("documents")
     )
-    words_blueprint = words.create_blueprint(
-        vocab=vocab,
-        document_term_matrix=document_term_matrix,
-        document_topic_matrix=document_topic_matrix,
-        topic_term_matrix=topic_term_matrix,
-        document_names=document_names,
-        corpus=corpus,
-        vectorizer=vectorizer,
-        topic_model=topic_model,
-        topic_names=topic_names,
+    words_blueprint = (
+        words.create_blueprint(
+            vocab=vocab,
+            document_term_matrix=document_term_matrix,
+            document_topic_matrix=document_topic_matrix,
+            topic_term_matrix=topic_term_matrix,
+            document_names=document_names,
+            corpus=corpus,
+            vectorizer=vectorizer,
+            topic_model=topic_model,
+            topic_names=topic_names,
+        )
+        if "words" not in exclude_pages
+        else create_blank_page("words")
     )
+    options = []
+    for option in ["Topics", "Words", "Documents"]:
+        if option.lower() not in exclude_pages:
+            options.append(option)
     blueprints = [
         topic_blueprint,
         words_blueprint,
         documents_blueprint,
     ]
 
     # --------[ Creating app blueprint ]--------
     app_blueprint = DashBlueprint()
 
     app_blueprint.layout = html.Div(
         [
             dcc.Download("download_data"),
+            dcc.Store(
+                "topic_names",
+                data=topic_names,
+            ),
             topic_blueprint.layout,
             words_blueprint.layout,
             documents_blueprint.layout,
             html.Div(
                 [
                     dmc.SegmentedControl(
                         id="page_picker",
-                        data=["Topics", "Words", "Documents"],
-                        value="Topics",
+                        data=options,
+                        value=options[0],
                         color="orange",
                         size="md",
                         radius="xl",
                     ),
                     html.Div(className="w-5"),
                     dmc.ActionIcon(
                         DashIconify(
```

### Comparing `topic_wizard-0.2.6/topicwizard/blueprints/documents.py` & `topic_wizard-0.3.0/topicwizard/blueprints/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/blueprints/groups.py` & `topic_wizard-0.3.0/topicwizard/blueprints/groups.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/blueprints/template.py` & `topic_wizard-0.3.0/topicwizard/blueprints/template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 from typing import Any, Callable, Iterable, List, Optional
 from warnings import warn
 
 import numpy as np
-from dash_extensions.enrich import DashBlueprint
+from dash_extensions.enrich import DashBlueprint, html
+from sklearn.pipeline import make_pipeline
 
+from topicwizard.prepare.topics import infer_topic_names
 from topicwizard.prepare.utils import get_vocab, prepare_transformed_data
 
 BlueprintCreator = Callable[..., DashBlueprint]
 
 
+def create_blank_page(name: str) -> DashBlueprint:
+    blueprint = DashBlueprint()
+    blueprint.layout = html.Div(id=f"{name}_container")
+    return blueprint
+
+
 def prepare_blueprint(
     vectorizer: Any,
     topic_model: Any,
     corpus: Iterable[str],
     create_blueprint: BlueprintCreator,
     document_names: Optional[List[str]] = None,
     topic_names: Optional[List[str]] = None,
+    *args,
+    **kwargs,
 ) -> DashBlueprint:
     corpus = list(corpus)
     n_documents = len(corpus)
     if document_names is None:
         document_names = [f"Document {i}" for i in range(n_documents)]
     vocab = get_vocab(vectorizer)
     (
@@ -36,20 +46,22 @@
         )
         corpus = list(np.array(corpus)[~nan_documents])
         document_topic_matrix = document_topic_matrix[~nan_documents]
         document_term_matrix = document_term_matrix[~nan_documents]
         document_names = list(np.array(document_names)[~nan_documents])
     n_topics = topic_term_matrix.shape[0]
     if topic_names is None:
-        topic_names = [f"Topic {i}" for i in range(n_topics)]
+        topic_names = infer_topic_names(pipeline=make_pipeline(vectorizer, topic_model))
     blueprint = create_blueprint(
         vocab=vocab,
         document_term_matrix=document_term_matrix,
         document_topic_matrix=document_topic_matrix,
         topic_term_matrix=topic_term_matrix,
         document_names=document_names,
         corpus=corpus,
         vectorizer=vectorizer,
         topic_model=topic_model,
         topic_names=topic_names,
+        *args,
+        **kwargs,
     )
     return blueprint
```

### Comparing `topic_wizard-0.2.6/topicwizard/blueprints/topics.py` & `topic_wizard-0.3.0/topicwizard/blueprints/topics.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,18 +75,14 @@
     ]
     # layouts = [blueprint.layout for blueprint in blueprints]
 
     # --------[ Creating app blueprint ]--------
     app_blueprint = DashBlueprint()
     app_blueprint.layout = html.Div(
         [
-            dcc.Store(
-                "topic_names",
-                data=topic_names,
-            ),
             dcc.Store("current_topic", data=0),
             dmc.Grid(
                 [
                     dmc.Col(topic_switcher.layout, span="content"),
                     dmc.Col(topic_namer.layout, span=4),
                     dmc.Col(relevance_slider.layout, span=4),
                 ],
```

### Comparing `topic_wizard-0.2.6/topicwizard/blueprints/words.py` & `topic_wizard-0.3.0/topicwizard/blueprints/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/compatibility/bertopic.py` & `topic_wizard-0.3.0/topicwizard/compatibility/bertopic.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/compatibility/gensim.py` & `topic_wizard-0.3.0/topicwizard/compatibility/gensim.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/documents/document_map.py` & `topic_wizard-0.3.0/topicwizard/components/documents/document_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/documents/document_pie.py` & `topic_wizard-0.3.0/topicwizard/components/documents/document_pie.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/documents/document_selector.py` & `topic_wizard-0.3.0/topicwizard/components/documents/document_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/documents/document_timeline.py` & `topic_wizard-0.3.0/topicwizard/components/documents/document_timeline.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/documents/document_wordcloud.py` & `topic_wizard-0.3.0/topicwizard/components/documents/document_wordcloud.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/documents/window_slider.py` & `topic_wizard-0.3.0/topicwizard/components/documents/window_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/topics/intertopic_map.py` & `topic_wizard-0.3.0/topicwizard/components/topics/intertopic_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/topics/relevance_slider.py` & `topic_wizard-0.3.0/topicwizard/components/topics/relevance_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/topics/topic_namer.py` & `topic_wizard-0.3.0/topicwizard/components/topics/topic_namer.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/topics/topic_switcher.py` & `topic_wizard-0.3.0/topicwizard/components/topics/topic_switcher.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/words/association_slider.py` & `topic_wizard-0.3.0/topicwizard/components/words/association_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/words/word_barplot.py` & `topic_wizard-0.3.0/topicwizard/components/words/word_barplot.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/words/word_map.py` & `topic_wizard-0.3.0/topicwizard/components/words/word_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/components/words/word_selector.py` & `topic_wizard-0.3.0/topicwizard/components/words/word_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/plots/documents.py` & `topic_wizard-0.3.0/topicwizard/plots/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/plots/topics.py` & `topic_wizard-0.3.0/topicwizard/plots/topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Module containing plotting utilities for topics."""
 from typing import List
+
+import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from PIL import Image
 from wordcloud import WordCloud
-import numpy as np
 
 
 def intertopic_map(
     x: np.ndarray,
     y: np.ndarray,
     topic_importances: np.ndarray,
     topic_names: List[str],
@@ -35,17 +36,15 @@
         modebar_remove=["lasso2d", "select2d"],
         showlegend=False,
         hovermode="closest",
         plot_bgcolor="white",
         dragmode="pan",
         margin=dict(l=0, r=0, b=0, t=0, pad=0),
     )
-    fig.update_traces(
-        textposition="top center", hovertemplate="", hoverinfo="none"
-    )
+    fig.update_traces(textposition="top center", hovertemplate="", hoverinfo="none")
     fig.update_coloraxes(showscale=False)
     fig.update_xaxes(
         showticklabels=False,
         title="",
         gridcolor="#e5e7eb",
         linecolor="#f9fafb",
         linewidth=6,
```

### Comparing `topic_wizard-0.2.6/topicwizard/plots/words.py` & `topic_wizard-0.3.0/topicwizard/plots/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/prepare/documents.py` & `topic_wizard-0.3.0/topicwizard/prepare/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/prepare/groups.py` & `topic_wizard-0.3.0/topicwizard/prepare/groups.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/prepare/topics.py` & `topic_wizard-0.3.0/topicwizard/prepare/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/prepare/utils.py` & `topic_wizard-0.3.0/topicwizard/prepare/utils.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.6/topicwizard/prepare/words.py` & `topic_wizard-0.3.0/topicwizard/prepare/words.py`

 * *Files identical despite different names*

