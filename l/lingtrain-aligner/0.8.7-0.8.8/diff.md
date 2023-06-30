# Comparing `tmp/lingtrain-aligner-0.8.7.tar.gz` & `tmp/lingtrain-aligner-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/f/git/lingtrain-aligner/dist/tmphrp1h9xj/lingtrain-aligner-0.8.7.tar", last modified: Sun Dec 11 09:01:32 2022, max compression
+gzip compressed data, was "lingtrain-aligner-0.8.8.tar", last modified: Thu Jun 29 14:33:41 2023, max compression
```

## Comparing `lingtrain-aligner-0.8.7.tar` & `lingtrain-aligner-0.8.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 serega    (1000) serega    (1000)        0 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/
--rwxrwxrwx   0 serega    (1000) serega    (1000)    35823 2021-04-21 06:49:05.000000 lingtrain-aligner-0.8.7/LICENSE
--rwxrwxrwx   0 serega    (1000) serega    (1000)     3584 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/PKG-INFO
--rwxrwxrwx   0 serega    (1000) serega    (1000)      108 2021-04-21 06:57:56.000000 lingtrain-aligner-0.8.7/pyproject.toml
--rwxrwxrwx   0 serega    (1000) serega    (1000)     2983 2022-09-06 07:40:35.000000 lingtrain-aligner-0.8.7/README.md
--rwxrwxrwx   0 serega    (1000) serega    (1000)      730 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/setup.cfg
-drwxrwxrwx   0 serega    (1000) serega    (1000)        0 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/src/
-drwxrwxrwx   0 serega    (1000) serega    (1000)        0 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/
--rwxrwxrwx   0 serega    (1000) serega    (1000)    29166 2022-12-10 12:59:06.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/aligner.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)      166 2022-12-10 14:02:39.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/constants.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)    18918 2022-12-10 15:01:28.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/helper.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)      851 2022-09-08 09:27:57.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/i18n.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)     1437 2022-09-08 09:27:54.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/metrics.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)      651 2022-09-08 09:27:53.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/model_dispatcher.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)     6394 2022-09-08 14:08:36.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/preprocessor.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)    39633 2022-09-12 05:56:29.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/reader.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)    14421 2022-09-08 13:29:16.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/resolver.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)    16020 2022-09-12 05:30:33.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/saver.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)     5607 2022-09-22 06:33:41.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/sententense_transformers_models.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)     8412 2022-11-05 06:54:51.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/splitter.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)     6953 2022-09-08 09:28:05.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/vis_helper.py
--rwxrwxrwx   0 serega    (1000) serega    (1000)        0 2021-04-19 09:16:20.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner/__init__.py
-drwxrwxrwx   0 serega    (1000) serega    (1000)        0 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner.egg-info/
--rwxrwxrwx   0 serega    (1000) serega    (1000)        1 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner.egg-info/dependency_links.txt
--rwxrwxrwx   0 serega    (1000) serega    (1000)     3584 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner.egg-info/PKG-INFO
--rwxrwxrwx   0 serega    (1000) serega    (1000)      723 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner.egg-info/SOURCES.txt
--rwxrwxrwx   0 serega    (1000) serega    (1000)       18 2022-12-11 09:01:32.000000 lingtrain-aligner-0.8.7/src/lingtrain_aligner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 14:33:41.718285 lingtrain-aligner-0.8.8/
+-rw-rw-rw-   0        0        0    35823 2021-04-21 06:49:05.000000 lingtrain-aligner-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0     3615 2023-06-29 14:33:41.719287 lingtrain-aligner-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2983 2022-09-06 07:40:35.000000 lingtrain-aligner-0.8.8/README.md
+-rw-rw-rw-   0        0        0      108 2021-04-21 06:57:56.000000 lingtrain-aligner-0.8.8/pyproject.toml
+-rw-rw-rw-   0        0        0      760 2023-06-29 14:33:41.719287 lingtrain-aligner-0.8.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 14:33:41.704421 lingtrain-aligner-0.8.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 14:33:41.715286 lingtrain-aligner-0.8.8/src/lingtrain_aligner/
+-rw-rw-rw-   0        0        0        0 2023-06-29 08:45:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/__init__.py
+-rw-rw-rw-   0        0        0    37324 2023-06-29 13:35:08.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/aligner.py
+-rw-rw-rw-   0        0        0      166 2023-06-29 14:28:21.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/constants.py
+-rw-rw-rw-   0        0        0    19245 2023-06-29 09:32:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/helper.py
+-rw-rw-rw-   0        0        0      851 2023-06-29 08:45:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/i18n.py
+-rw-rw-rw-   0        0        0     1437 2023-06-29 08:45:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/metrics.py
+-rw-rw-rw-   0        0        0      651 2023-06-29 08:45:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/model_dispatcher.py
+-rw-rw-rw-   0        0        0     6417 2023-06-29 14:25:57.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/preprocessor.py
+-rw-rw-rw-   0        0        0    39633 2023-06-29 08:45:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/reader.py
+-rw-rw-rw-   0        0        0    14421 2023-06-29 08:45:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/resolver.py
+-rw-rw-rw-   0        0        0    16020 2023-06-29 08:45:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/saver.py
+-rw-rw-rw-   0        0        0     5607 2023-06-29 08:45:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/sententense_transformers_models.py
+-rw-rw-rw-   0        0        0     8412 2023-06-29 08:45:54.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/splitter.py
+-rw-rw-rw-   0        0        0     6953 2023-06-29 14:26:06.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner/vis_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:33:41.718285 lingtrain-aligner-0.8.8/src/lingtrain_aligner.egg-info/
+-rw-rw-rw-   0        0        0     3615 2023-06-29 14:33:41.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-06-29 14:33:41.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:33:41.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-29 14:33:41.000000 lingtrain-aligner-0.8.8/src/lingtrain_aligner.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lingtrain-aligner-0.8.7/LICENSE` & `lingtrain-aligner-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/PKG-INFO` & `lingtrain-aligner-0.8.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,68 @@
-Metadata-Version: 2.1
-Name: lingtrain-aligner
-Version: 0.8.7
-Summary: Alignment tool for texts in different languages
-Home-page: https://github.com/averkij/lingtrain-aligner
-Author: Sergei Averkiev
-Author-email: averoo@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/averkij/lingtrain-aligner/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![PyPI - PyPi](https://img.shields.io/pypi/v/lingtrain-aligner)](https://pypi.org/project/lingtrain-aligner) [![Downloads](https://static.pepy.tech/personalized-badge/lingtrain-aligner?period=total&units=abbreviation&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/lingtrain-aligner)
-
-# Lingtrain Aligner
-
-ML powered library for the accurate texts alignment in different languages.
-
-- 🔥 [How to create bilingual books. Part 2. Lingtrain Alignment Studio](https://habr.com/ru/post/590549/)
-- 💡 [Lingtrain Aligner. How to make parallel books for language learning. Part 1. Python and Colab version](https://habr.com/ru/post/586574/)
-
-![Cover](https://i.imgur.com/WQWB4v0.png)
-
-## Purpose
-
-Main purpose of this alignment tool is to build parallel corpora using two or more raw texts in different languages. Texts should contain the same information (i.e., one text should be a translated analog oh the other text). E.g., it can be the _Drei Kameraden_ by Remarque in German and the _Three Comrades_ — it's translation into English.
-
-## Process
-
-There are plenty of obstacles during the alignment process:
-
-- The translator could translate several sentences as one.
-- The translator could translate one sentence as many.
-- There are some service marks in the text
-    - Page numbers
-    - Chapters and other section headings
-    - Author and title information
-    - Notes
-
-While service marks can be handled manually (the tool helps to detect them), the translation conflicts should be handled more carefully.
-
-Lingtrain Aligner tool will do almost all alignment work for you. It matches the sentence pairs automatically using the multilingual machine learning models. Then it searches for the alignment conflicts and resolves them. As output you will have the parallel corpora either as two distinct plain text files or as the merged corpora in widely used TMX format.
-
-### Supported languages and models
-
-Automated alignment process relies on the sentence embeddings models. Embeddings are multidimensional vectors of a special kind which are used to calculate a distance between the sentences. Supported languages list depend on the selected backend model.
-
-- **distiluse-base-multilingual-cased-v2**
-  - more reliable and fast
-  - moderate weights size — 500MB
-  - supports 50+ languages
-  - full list of supported languages can be found in [this paper](https://arxiv.org/abs/2004.09813)
-- **LaBSE (Language-agnostic BERT Sentence Embedding)**
-  - can be used for rare languages
-  - pretty heavy weights — 1.8GB
-  - supports 100+ languages
-  - full list of supported languages can be found [here](https://arxiv.org/abs/2007.01852)
-
-## Profit
-
-- Parallel corpora by itself can used as the resource for machine translation models or for linguistic researches.
-- My personal goal of this project is to help people building parallel translated books for the foreign language learning. 
-
-
-
-
+Metadata-Version: 2.1
+Name: lingtrain-aligner
+Version: 0.8.8
+Summary: Alignment tool for texts in different languages
+Home-page: https://github.com/averkij/lingtrain-aligner
+Author: Sergei Averkiev
+Author-email: averoo@gmail.com
+Project-URL: Bug Tracker, https://github.com/averkij/lingtrain-aligner/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Text Processing :: Linguistic
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI - PyPi](https://img.shields.io/pypi/v/lingtrain-aligner)](https://pypi.org/project/lingtrain-aligner) [![Downloads](https://static.pepy.tech/personalized-badge/lingtrain-aligner?period=total&units=abbreviation&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/lingtrain-aligner)
+
+# Lingtrain Aligner
+
+ML powered library for the accurate texts alignment in different languages.
+
+- 🔥 [How to create bilingual books. Part 2. Lingtrain Alignment Studio](https://habr.com/ru/post/590549/)
+- 💡 [Lingtrain Aligner. How to make parallel books for language learning. Part 1. Python and Colab version](https://habr.com/ru/post/586574/)
+
+![Cover](https://i.imgur.com/WQWB4v0.png)
+
+## Purpose
+
+Main purpose of this alignment tool is to build parallel corpora using two or more raw texts in different languages. Texts should contain the same information (i.e., one text should be a translated analog oh the other text). E.g., it can be the _Drei Kameraden_ by Remarque in German and the _Three Comrades_ — it's translation into English.
+
+## Process
+
+There are plenty of obstacles during the alignment process:
+
+- The translator could translate several sentences as one.
+- The translator could translate one sentence as many.
+- There are some service marks in the text
+    - Page numbers
+    - Chapters and other section headings
+    - Author and title information
+    - Notes
+
+While service marks can be handled manually (the tool helps to detect them), the translation conflicts should be handled more carefully.
+
+Lingtrain Aligner tool will do almost all alignment work for you. It matches the sentence pairs automatically using the multilingual machine learning models. Then it searches for the alignment conflicts and resolves them. As output you will have the parallel corpora either as two distinct plain text files or as the merged corpora in widely used TMX format.
+
+### Supported languages and models
+
+Automated alignment process relies on the sentence embeddings models. Embeddings are multidimensional vectors of a special kind which are used to calculate a distance between the sentences. Supported languages list depend on the selected backend model.
+
+- **distiluse-base-multilingual-cased-v2**
+  - more reliable and fast
+  - moderate weights size — 500MB
+  - supports 50+ languages
+  - full list of supported languages can be found in [this paper](https://arxiv.org/abs/2004.09813)
+- **LaBSE (Language-agnostic BERT Sentence Embedding)**
+  - can be used for rare languages
+  - pretty heavy weights — 1.8GB
+  - supports 100+ languages
+  - full list of supported languages can be found [here](https://arxiv.org/abs/2007.01852)
+
+## Profit
+
+- Parallel corpora by itself can used as the resource for machine translation models or for linguistic researches.
+- My personal goal of this project is to help people building parallel translated books for the foreign language learning. 
+
+
```

### Comparing `lingtrain-aligner-0.8.7/README.md` & `lingtrain-aligner-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/aligner.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/aligner.py`

 * *Files 12% similar despite different names*

```diff
@@ -273,54 +273,78 @@
     show_progress_bar=False,
     shift=0,
     show_info=False,
     show_regression=False,
     model=None,
     use_proxy_from=False,
     use_proxy_to=False,
+    use_segments=False,
+    segmentation_marks=[preprocessor.H2],
 ):
     result = []
-    splitted_from = get_splitted_from(db_path)
-    splitted_to = get_splitted_to(db_path)
-    proxy_from = get_proxy_from(db_path)
-    proxy_to = get_proxy_to(db_path)
-
-    task_list = [
-        (
-            lines_from_batch,
-            lines_to_batch,
-            proxy_from_batch,
-            proxy_to_batch,
-            line_ids_from,
-            line_ids_to,
-            batch_id,
-        )
-        for lines_from_batch, lines_to_batch, proxy_from_batch, proxy_to_batch, line_ids_from, line_ids_to, batch_id in get_batch_intersected(
-            splitted_from,
-            splitted_to,
-            batch_size,
-            window,
-            batch_ids,
-            batch_shift=shift,
-            iter3=proxy_from,
-            iter4=proxy_to,
-        )
-    ]
+    if use_segments:
+        left_segments, right_segments = calculate_segments(db_path, segmentation_marks)
+        task_list = [
+            (
+                lines_from_batch,
+                lines_to_batch,
+                proxy_from_batch,
+                proxy_to_batch,
+                line_ids_from,
+                line_ids_to,
+                batch_id,
+            )
+            for lines_from_batch, lines_to_batch, proxy_from_batch, proxy_to_batch, line_ids_from, line_ids_to, batch_id in get_batch_intersected_for_segments(
+                db_path=db_path,
+                left_segments=left_segments,
+                right_segments=right_segments,
+                batch_size=batch_size,
+                window=window,
+                batch_ids=batch_ids,
+                batch_shift=shift,
+            )
+        ]
+    else:
+        splitted_from = get_splitted_from(db_path)
+        splitted_to = get_splitted_to(db_path)
+        proxy_from = get_proxy_from(db_path)
+        proxy_to = get_proxy_to(db_path)
+        task_list = [
+            (
+                lines_from_batch,
+                lines_to_batch,
+                proxy_from_batch,
+                proxy_to_batch,
+                line_ids_from,
+                line_ids_to,
+                batch_id,
+            )
+            for lines_from_batch, lines_to_batch, proxy_from_batch, proxy_to_batch, line_ids_from, line_ids_to, batch_id in get_batch_intersected(
+                splitted_from,
+                splitted_to,
+                batch_size,
+                window,
+                batch_ids,
+                batch_shift=shift,
+                iter3=proxy_from,
+                iter4=proxy_to,
+            )
+        ]
 
     count = 0
     for (
         lines_from_batch,
         lines_to_batch,
         proxy_from_batch,
         proxy_to_batch,
         line_ids_from,
         line_ids_to,
         batch_id,
     ) in task_list:
-        print("batch:", count)
+        print(f"batch: {count} ({batch_id})")
         texts_from, texts_to = process_batch(
             lines_from_batch,
             lines_to_batch,
             proxy_from_batch,
             proxy_to_batch,
             line_ids_from,
             line_ids_to,
@@ -348,15 +372,15 @@
         return
 
     # sort by batch_id (will be useful with parallel processing)
     result.sort()
     save_db(db_path, result)
 
 
-# HELPERS
+# CONTENT HELPERS
 
 
 def get_splitted_from(db_path):
     """Get lines from splitted_from"""
     with sqlite3.connect(db_path) as db:
         res = db.execute(f"select f.text from splitted_from f order by f.id").fetchall()
     return [x[0] for x in res]
@@ -365,14 +389,38 @@
 def get_splitted_to(db_path):
     """Get lines from splitted_to"""
     with sqlite3.connect(db_path) as db:
         res = db.execute(f"select t.text from splitted_to t order by t.id").fetchall()
     return [x[0] for x in res]
 
 
+def get_splitted_from_by_par_with_line_id(db_path, par_id_start, par_id_end):
+    """Get lines from splitted_from by paragraphs"""
+    with sqlite3.connect(db_path) as db:
+        res = db.execute(
+            f"""select f.id, f.text from splitted_from f
+                                where paragraph > ? and paragraph < ?
+                                order by f.id""",
+            (par_id_start, par_id_end),
+        ).fetchall()
+    return [(x[0], x[1]) for x in res]
+
+
+def get_splitted_to_by_par_with_line_id(db_path, par_id_start, par_id_end):
+    """Get lines from splitted_from by paragraphs"""
+    with sqlite3.connect(db_path) as db:
+        res = db.execute(
+            f"""select f.id, f.text from splitted_to f
+                                where paragraph > ? and paragraph < ?
+                                order by f.id""",
+            (par_id_start, par_id_end),
+        ).fetchall()
+    return [(x[0], x[1]) for x in res]
+
+
 def get_proxy_from(db_path):
     """Get lines from proxy_from"""
     with sqlite3.connect(db_path) as db:
         res = db.execute(
             f"select f.proxy_text from splitted_from f order by f.id"
         ).fetchall()
     return [x[0] for x in res]
@@ -383,65 +431,246 @@
     with sqlite3.connect(db_path) as db:
         res = db.execute(
             f"select t.proxy_text from splitted_to t order by t.id"
         ).fetchall()
     return [x[0] for x in res]
 
 
+def get_proxy_from_by_par_with_line_id(db_path, par_id_start, par_id_end):
+    """Get proxy lines from splitted_from by paragraphs"""
+    with sqlite3.connect(db_path) as db:
+        res = db.execute(
+            f"""select f.id, f.proxy_text from splitted_from f
+                                where paragraph > ? and paragraph < ?
+                                order by f.id""",
+            (par_id_start, par_id_end),
+        ).fetchall()
+    return [(x[0], x[1]) for x in res]
+
+
+def get_proxy_to_by_par_with_line_id(db_path, par_id_start, par_id_end):
+    """Get proxy lines from splitted_from by paragraphs"""
+    with sqlite3.connect(db_path) as db:
+        res = db.execute(
+            f"""select f.id, f.proxy_text from splitted_to f
+                                where paragraph > ? and paragraph < ?
+                                order by f.id""",
+            (par_id_start, par_id_end),
+        ).fetchall()
+    return [(x[0], x[1]) for x in res]
+
+
 def best_per_row_with_ones(sim_matrix):
     """Transfor matrix by leaving only best match"""
     sim_matrix_best = np.zeros_like(sim_matrix)
     max_sim = sim_matrix.argmax(1)
     sim_matrix_best[range(sim_matrix.shape[0]), max_sim] = 1
     return sim_matrix_best
 
 
 def get_batch_intersected(
-    iter1, iter2, n, window, batch_ids=[], batch_shift=0, iter3=[], iter4=[]
+    iter1,
+    iter2,
+    n,
+    window,
+    batch_ids=[],
+    batch_shift=0,
+    iter3=[],
+    iter4=[],
+    start_batch_id=0,
+    batch_start_line_id_from=0,
+    batch_start_line_id_to=0,
 ):
     """Get batch with an additional window"""
     l1 = len(iter1)
     l2 = len(iter2)
+
     k = int(round(n * l2 / l1))
     kdx = 0 - k
 
     if not iter3:
         iter3 = ["" for _ in range(l1)]
     if not iter4:
         iter4 = ["" for _ in range(l2)]
 
     if k < window * 2:
         # subbatches will be intersected
         logging.warning(
             f"Batch for the second language is too small. k = {k}, window = {window}"
         )
 
-    counter = 0
+    counter = start_batch_id
     for ndx in range(0, l1, n):
         kdx += k
         if counter in batch_ids or len(batch_ids) == 0:
             yield iter1[ndx : min(ndx + n, l1)], iter2[
                 max(0, kdx - window + batch_shift) : min(
                     kdx + k + window + batch_shift, l2
                 )
             ], iter3[ndx : min(ndx + n, l1)], iter4[
                 max(0, kdx - window + batch_shift) : min(
                     kdx + k + window + batch_shift, l2
                 )
             ], list(
-                range(ndx, min(ndx + n, l1))
+                range(
+                    ndx + batch_start_line_id_from,
+                    min(
+                        ndx + batch_start_line_id_from + n,
+                        batch_start_line_id_from + l1,
+                    ),
+                )
             ), list(
                 range(
-                    max(0, kdx - window + batch_shift),
-                    min(kdx + k + window + batch_shift, l2),
+                    max(
+                        batch_start_line_id_to,
+                        batch_start_line_id_to + kdx - window + batch_shift,
+                    ),
+                    min(
+                        batch_start_line_id_to + kdx + k + window + batch_shift,
+                        batch_start_line_id_to + l2,
+                    ),
                 )
             ), counter
         counter += 1
 
 
+def get_batch_intersected_for_segments(
+    db_path,
+    left_segments,
+    right_segments,
+    batch_size,
+    window,
+    batch_ids=[],
+    batch_shift=0,
+):
+    """Get batches based on segments structure."""
+    start_batch_id = 0
+
+    for left, right in zip(left_segments, right_segments):
+        iter1 = get_splitted_from_by_par_with_line_id(db_path, left[0], left[1])
+        iter2 = get_splitted_to_by_par_with_line_id(db_path, right[0], right[1])
+        iter3 = get_proxy_from_by_par_with_line_id(db_path, left[0], left[1])
+        iter4 = get_proxy_to_by_par_with_line_id(db_path, right[0], right[1])
+
+        if not iter1:
+            print("Empty segment occured. Probably no text between segment delimeters")
+            continue
+
+        for (
+            lines_from_batch,
+            lines_to_batch,
+            proxy_from_batch,
+            proxy_to_batch,
+            line_ids_from,
+            line_ids_to,
+            batch_id,
+        ) in get_batch_intersected(
+            [x[1] for x in iter1],
+            [x[1] for x in iter2],
+            batch_size,
+            window,
+            batch_ids=[],  # we need to return all batches to estimate needed [batch_ids]
+            batch_shift=batch_shift,
+            iter3=[x[1] for x in iter3],
+            iter4=[x[1] for x in iter4],
+            start_batch_id=start_batch_id,
+            batch_start_line_id_from=iter1[0][0],
+            batch_start_line_id_to=iter2[0][0],
+        ):
+            if batch_id in batch_ids:
+                yield lines_from_batch, lines_to_batch, proxy_from_batch, proxy_to_batch, line_ids_from, line_ids_to, batch_id
+
+            start_batch_id += 1
+
+
+def calculate_segments(db_path, segmentation_marks=[preprocessor.H2]):
+    """Calculate segments based on metadata"""
+    left_nails, right_nails = [], []
+    meta = helper.get_meta_dict(db_path)
+    for mark in meta:
+        if mark.split("_")[0] in segmentation_marks:
+            # print(mark)
+            for segment_mark in meta[mark]:
+                if mark.split("_")[-1] == "from":
+                    # print(segment_mark)
+                    left_nails.append(segment_mark[2])  # line_id
+                else:
+                    right_nails.append(segment_mark[2])  # line_id
+
+    # remove duplicates
+    left_nails = sorted(list(set(left_nails)))
+    right_nails = sorted(list(set(right_nails)))
+
+    assert len(left_nails) == len(
+        right_nails
+    ), f"Error. Different amount of segmentation marks in your texts ({', '.join(segmentation_marks)})"
+
+    left_nails.sort()
+    right_nails.sort()
+
+    left_segments, right_segments = [], []
+    left_len, right_len = helper.get_splitted_lenght(db_path)
+
+    for i in range(1, len(left_nails)):
+        left_segments.append((left_nails[i - 1], left_nails[i]))
+        right_segments.append((right_nails[i - 1], right_nails[i]))
+
+    # insert last or the only segment
+    if len(left_nails) == 0:
+        left_segments.append((0, left_len))
+        right_segments.append((0, right_len))
+    else:
+        left_segments.append((left_nails[-1], left_len))
+        right_segments.append((right_nails[-1], right_len))
+
+    return left_segments, right_segments
+
+
+def get_batch_intersected_for_segments_list(
+    db_path, left_segments, right_segments, batch_size
+):
+    """Get batche structure based on segments."""
+    res = []
+    start_batch_id = 0
+
+    for left, right in zip(left_segments, right_segments):
+        segment_batches = []
+        iter1 = get_splitted_from_by_par_with_line_id(db_path, left[0], left[1])
+        iter2 = get_splitted_to_by_par_with_line_id(db_path, right[0], right[1])
+
+        if not iter1:
+            print("Empty segment occured. Probably no text between segment delimeters")
+            continue
+
+        for (
+            _,
+            _,
+            _,
+            _,
+            _,
+            _,
+            batch_id,
+        ) in get_batch_intersected(
+            [x[1] for x in iter1],
+            [x[1] for x in iter2],
+            batch_size,
+            window=0,
+            batch_ids=[],  # we need to return all batches to estimate needed [batch_ids]
+            start_batch_id=start_batch_id,
+            batch_start_line_id_from=iter1[0][0],
+            batch_start_line_id_to=iter2[0][0],
+        ):
+            segment_batches.append(batch_id)
+            start_batch_id += 1
+
+        res.append(segment_batches)
+
+    return res
+
+
 def get_sim_matrix(vec1, vec2, window):
     """Calculate similarity matrix"""
     sim_matrix = np.zeros((len(vec1), len(vec2)))
     k = len(vec1) / len(vec2)
     for i, vector1 in enumerate(vec1):
         for j, vector2 in enumerate(vec2):
             if (j * k > i - window) & (j * k < i + window):
```

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/helper.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,22 @@
         for id, text_to, similarity in db.execute(
             f'select t.id, t.text, t.similarity from processing_to t where t.id in ({",".join([str(x) for x in ids])})'
         ):
             res.append((id, text_to, similarity))
     return res
 
 
+def get_splitted_lenght(db_path):
+    """Get splitted_from and splitted_to lenghts"""
+    with sqlite3.connect(db_path) as db:
+        len_from = db.execute(f"select count(*) from splitted_from").fetchone()[0]
+        len_to = db.execute(f"select count(*) from splitted_to").fetchone()[0]
+    return len_from, len_to
+
+
 def get_splitted_from_by_id(db_path, ids):
     """Get lines from splitted_from by ids"""
     res = []
     with sqlite3.connect(db_path) as db:
         for (
             id,
             text_from,
```

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/i18n.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/i18n.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/metrics.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/metrics.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/model_dispatcher.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/model_dispatcher.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/preprocessor.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 DIVIDER = "divider"
 TITLE = "title"
 AUTHOR = "author"
 TRANSLATOR = "translator"
 QUOTE_TEXT = "qtext"
 QUOTE_NAME = "qname"
 IMAGE = "image"
+SEGMENT = "segment"
 
 MARK_META = [
     H1,
     H2,
     H3,
     H4,
     H5,
@@ -220,8 +221,8 @@
         ending = f"{PARAGRAPH_MARK}{mark}."
         if line.endswith(ending):
             res.append((line[: len(line) - len(ending)], ix, mark))
     return res
 
 
 def get_all_meta_marks():
-    return [f"{PARAGRAPH_MARK}{m}" for m in MARK_META]
+    return [f"{PARAGRAPH_MARK}{m}" for m in MARK_META]
```

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/reader.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/reader.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/resolver.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/resolver.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/saver.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/saver.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/sententense_transformers_models.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/sententense_transformers_models.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/splitter.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/splitter.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner/vis_helper.py` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner/vis_helper.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner.egg-info/PKG-INFO` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,68 @@
-Metadata-Version: 2.1
-Name: lingtrain-aligner
-Version: 0.8.7
-Summary: Alignment tool for texts in different languages
-Home-page: https://github.com/averkij/lingtrain-aligner
-Author: Sergei Averkiev
-Author-email: averoo@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/averkij/lingtrain-aligner/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![PyPI - PyPi](https://img.shields.io/pypi/v/lingtrain-aligner)](https://pypi.org/project/lingtrain-aligner) [![Downloads](https://static.pepy.tech/personalized-badge/lingtrain-aligner?period=total&units=abbreviation&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/lingtrain-aligner)
-
-# Lingtrain Aligner
-
-ML powered library for the accurate texts alignment in different languages.
-
-- 🔥 [How to create bilingual books. Part 2. Lingtrain Alignment Studio](https://habr.com/ru/post/590549/)
-- 💡 [Lingtrain Aligner. How to make parallel books for language learning. Part 1. Python and Colab version](https://habr.com/ru/post/586574/)
-
-![Cover](https://i.imgur.com/WQWB4v0.png)
-
-## Purpose
-
-Main purpose of this alignment tool is to build parallel corpora using two or more raw texts in different languages. Texts should contain the same information (i.e., one text should be a translated analog oh the other text). E.g., it can be the _Drei Kameraden_ by Remarque in German and the _Three Comrades_ — it's translation into English.
-
-## Process
-
-There are plenty of obstacles during the alignment process:
-
-- The translator could translate several sentences as one.
-- The translator could translate one sentence as many.
-- There are some service marks in the text
-    - Page numbers
-    - Chapters and other section headings
-    - Author and title information
-    - Notes
-
-While service marks can be handled manually (the tool helps to detect them), the translation conflicts should be handled more carefully.
-
-Lingtrain Aligner tool will do almost all alignment work for you. It matches the sentence pairs automatically using the multilingual machine learning models. Then it searches for the alignment conflicts and resolves them. As output you will have the parallel corpora either as two distinct plain text files or as the merged corpora in widely used TMX format.
-
-### Supported languages and models
-
-Automated alignment process relies on the sentence embeddings models. Embeddings are multidimensional vectors of a special kind which are used to calculate a distance between the sentences. Supported languages list depend on the selected backend model.
-
-- **distiluse-base-multilingual-cased-v2**
-  - more reliable and fast
-  - moderate weights size — 500MB
-  - supports 50+ languages
-  - full list of supported languages can be found in [this paper](https://arxiv.org/abs/2004.09813)
-- **LaBSE (Language-agnostic BERT Sentence Embedding)**
-  - can be used for rare languages
-  - pretty heavy weights — 1.8GB
-  - supports 100+ languages
-  - full list of supported languages can be found [here](https://arxiv.org/abs/2007.01852)
-
-## Profit
-
-- Parallel corpora by itself can used as the resource for machine translation models or for linguistic researches.
-- My personal goal of this project is to help people building parallel translated books for the foreign language learning. 
-
-
-
-
+Metadata-Version: 2.1
+Name: lingtrain-aligner
+Version: 0.8.8
+Summary: Alignment tool for texts in different languages
+Home-page: https://github.com/averkij/lingtrain-aligner
+Author: Sergei Averkiev
+Author-email: averoo@gmail.com
+Project-URL: Bug Tracker, https://github.com/averkij/lingtrain-aligner/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Text Processing :: Linguistic
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI - PyPi](https://img.shields.io/pypi/v/lingtrain-aligner)](https://pypi.org/project/lingtrain-aligner) [![Downloads](https://static.pepy.tech/personalized-badge/lingtrain-aligner?period=total&units=abbreviation&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/lingtrain-aligner)
+
+# Lingtrain Aligner
+
+ML powered library for the accurate texts alignment in different languages.
+
+- 🔥 [How to create bilingual books. Part 2. Lingtrain Alignment Studio](https://habr.com/ru/post/590549/)
+- 💡 [Lingtrain Aligner. How to make parallel books for language learning. Part 1. Python and Colab version](https://habr.com/ru/post/586574/)
+
+![Cover](https://i.imgur.com/WQWB4v0.png)
+
+## Purpose
+
+Main purpose of this alignment tool is to build parallel corpora using two or more raw texts in different languages. Texts should contain the same information (i.e., one text should be a translated analog oh the other text). E.g., it can be the _Drei Kameraden_ by Remarque in German and the _Three Comrades_ — it's translation into English.
+
+## Process
+
+There are plenty of obstacles during the alignment process:
+
+- The translator could translate several sentences as one.
+- The translator could translate one sentence as many.
+- There are some service marks in the text
+    - Page numbers
+    - Chapters and other section headings
+    - Author and title information
+    - Notes
+
+While service marks can be handled manually (the tool helps to detect them), the translation conflicts should be handled more carefully.
+
+Lingtrain Aligner tool will do almost all alignment work for you. It matches the sentence pairs automatically using the multilingual machine learning models. Then it searches for the alignment conflicts and resolves them. As output you will have the parallel corpora either as two distinct plain text files or as the merged corpora in widely used TMX format.
+
+### Supported languages and models
+
+Automated alignment process relies on the sentence embeddings models. Embeddings are multidimensional vectors of a special kind which are used to calculate a distance between the sentences. Supported languages list depend on the selected backend model.
+
+- **distiluse-base-multilingual-cased-v2**
+  - more reliable and fast
+  - moderate weights size — 500MB
+  - supports 50+ languages
+  - full list of supported languages can be found in [this paper](https://arxiv.org/abs/2004.09813)
+- **LaBSE (Language-agnostic BERT Sentence Embedding)**
+  - can be used for rare languages
+  - pretty heavy weights — 1.8GB
+  - supports 100+ languages
+  - full list of supported languages can be found [here](https://arxiv.org/abs/2007.01852)
+
+## Profit
+
+- Parallel corpora by itself can used as the resource for machine translation models or for linguistic researches.
+- My personal goal of this project is to help people building parallel translated books for the foreign language learning. 
+
+
```

### Comparing `lingtrain-aligner-0.8.7/src/lingtrain_aligner.egg-info/SOURCES.txt` & `lingtrain-aligner-0.8.8/src/lingtrain_aligner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

