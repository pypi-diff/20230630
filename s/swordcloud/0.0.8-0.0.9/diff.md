# Comparing `tmp/swordcloud-0.0.8.tar.gz` & `tmp/swordcloud-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swordcloud-0.0.8.tar", last modified: Thu Dec  1 03:24:55 2022, max compression
+gzip compressed data, was "D:\University\RA\swordcloud\dist\.tmp-axe04usc\swordcloud-0.0.9.tar", last modified: Fri Jun 30 05:11:41 2023, max compression
```

## Comparing `swordcloud-0.0.8.tar` & `swordcloud-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 pzzlng1    (502) staff       (20)        0 2022-12-01 03:24:55.943416 swordcloud-0.0.8/
--rw-r--r--   0 pzzlng1    (502) staff       (20)      573 2022-12-01 03:24:55.943237 swordcloud-0.0.8/PKG-INFO
--rw-r--r--   0 pzzlng1    (502) staff       (20)      950 2022-08-15 04:25:27.000000 swordcloud-0.0.8/README.md
--rw-r--r--   0 pzzlng1    (502) staff       (20)       38 2022-12-01 03:24:55.943462 swordcloud-0.0.8/setup.cfg
--rw-r--r--   0 pzzlng1    (502) staff       (20)     1062 2022-12-01 03:15:12.000000 swordcloud-0.0.8/setup.py
-drwxr-xr-x   0 pzzlng1    (502) staff       (20)        0 2022-12-01 03:24:55.941922 swordcloud-0.0.8/swordcloud/
--rw-r--r--   0 pzzlng1    (502) staff       (20)    99980 2022-02-22 19:32:59.000000 swordcloud-0.0.8/swordcloud/THSarabun.ttf
--rw-r--r--   0 pzzlng1    (502) staff       (20)      401 2022-08-14 20:14:40.000000 swordcloud-0.0.8/swordcloud/__init__.py
--rw-r--r--   0 pzzlng1    (502) staff       (20)     2621 2022-07-07 06:39:49.000000 swordcloud-0.0.8/swordcloud/color_from_image.py
--rw-r--r--   0 pzzlng1    (502) staff       (20)     4172 2022-08-14 20:11:30.000000 swordcloud-0.0.8/swordcloud/processing.py
--rw-r--r--   0 pzzlng1    (502) staff       (20)     2182 2022-07-07 06:39:49.000000 swordcloud-0.0.8/swordcloud/query_integral_image.py
--rw-r--r--   0 pzzlng1    (502) staff       (20)     1050 2022-02-22 19:32:59.000000 swordcloud-0.0.8/swordcloud/stopwords
--rw-r--r--   0 pzzlng1    (502) staff       (20)    20658 2022-07-05 11:13:08.000000 swordcloud-0.0.8/swordcloud/thstopwords
--rw-r--r--   0 pzzlng1    (502) staff       (20)     6247 2022-07-07 06:39:49.000000 swordcloud-0.0.8/swordcloud/tokenization.py
--rw-r--r--   0 pzzlng1    (502) staff       (20)    43937 2022-12-01 03:12:39.000000 swordcloud-0.0.8/swordcloud/wordcloud.py
-drwxr-xr-x   0 pzzlng1    (502) staff       (20)        0 2022-12-01 03:24:55.943030 swordcloud-0.0.8/swordcloud.egg-info/
--rw-r--r--   0 pzzlng1    (502) staff       (20)      573 2022-12-01 03:24:55.000000 swordcloud-0.0.8/swordcloud.egg-info/PKG-INFO
--rw-r--r--   0 pzzlng1    (502) staff       (20)      421 2022-12-01 03:24:55.000000 swordcloud-0.0.8/swordcloud.egg-info/SOURCES.txt
--rw-r--r--   0 pzzlng1    (502) staff       (20)        1 2022-12-01 03:24:55.000000 swordcloud-0.0.8/swordcloud.egg-info/dependency_links.txt
--rw-r--r--   0 pzzlng1    (502) staff       (20)       97 2022-12-01 03:24:55.000000 swordcloud-0.0.8/swordcloud.egg-info/requires.txt
--rw-r--r--   0 pzzlng1    (502) staff       (20)       11 2022-12-01 03:24:55.000000 swordcloud-0.0.8/swordcloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 05:11:41.380616 swordcloud-0.0.9/
+-rw-rw-rw-   0        0        0      106 2023-06-28 19:53:18.000000 swordcloud-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8462 2023-06-30 05:11:41.380616 swordcloud-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7826 2023-06-29 08:18:06.000000 swordcloud-0.0.9/README.md
+-rw-rw-rw-   0        0        0      984 2023-06-28 17:34:51.000000 swordcloud-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 05:11:41.380616 swordcloud-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 05:11:41.301025 swordcloud-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 05:11:41.347849 swordcloud-0.0.9/src/swordcloud/
+-rw-rw-rw-   0        0        0    99980 2023-06-20 07:57:41.000000 swordcloud-0.0.9/src/swordcloud/THSarabun.ttf
+-rw-rw-rw-   0        0        0       40 2023-06-28 12:09:59.000000 swordcloud-0.0.9/src/swordcloud/__init__.py
+-rw-rw-rw-   0        0        0     5759 2023-06-28 16:55:49.000000 swordcloud-0.0.9/src/swordcloud/color_func.py
+-rw-rw-rw-   0        0        0     3375 2023-06-28 16:26:00.000000 swordcloud-0.0.9/src/swordcloud/occupancy.py
+-rw-rw-rw-   0        0        0     3897 2023-06-28 16:26:20.000000 swordcloud-0.0.9/src/swordcloud/processing.py
+-rw-rw-rw-   0        0        0     1242 2023-06-20 07:57:41.000000 swordcloud-0.0.9/src/swordcloud/stopwords
+-rw-rw-rw-   0        0        0    21787 2023-06-20 07:57:41.000000 swordcloud-0.0.9/src/swordcloud/thstopwords
+-rw-rw-rw-   0        0        0     5706 2023-06-28 16:26:49.000000 swordcloud-0.0.9/src/swordcloud/tokenization.py
+-rw-rw-rw-   0        0        0    43158 2023-06-30 04:55:58.000000 swordcloud-0.0.9/src/swordcloud/wordcloud.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:11:41.380616 swordcloud-0.0.9/src/swordcloud.egg-info/
+-rw-rw-rw-   0        0        0     8462 2023-06-30 05:11:41.000000 swordcloud-0.0.9/src/swordcloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-06-30 05:11:41.000000 swordcloud-0.0.9/src/swordcloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 05:11:41.000000 swordcloud-0.0.9/src/swordcloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-06-30 05:11:41.000000 swordcloud-0.0.9/src/swordcloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 05:11:41.000000 swordcloud-0.0.9/src/swordcloud.egg-info/top_level.txt
```

### Comparing `swordcloud-0.0.8/swordcloud/THSarabun.ttf` & `swordcloud-0.0.9/src/swordcloud/THSarabun.ttf`

 * *Files identical despite different names*

### Comparing `swordcloud-0.0.8/swordcloud/tokenization.py` & `swordcloud-0.0.9/src/swordcloud/tokenization.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,171 +1,158 @@
-from __future__ import division
-
-from collections import defaultdict
-from itertools import tee
-from math import log
-from operator import itemgetter
-from pythainlp.util.trie import Trie
-
-
-def l(k, n, x):  # noqa: E741, E743
-    # dunning's likelihood ratio with notation from
-    # http://nlp.stanford.edu/fsnlp/promo/colloc.pdf p162
-    return log(max(x, 1e-10)) * k + log(max(1 - x, 1e-10)) * (n - k)
-
-
-def score(count_bigram, count1, count2, n_words):
-    """Collocation score"""
-    if n_words <= count1 or n_words <= count2:
-        # only one words appears in the whole document
-        return 0
-    N = n_words
-    c12 = count_bigram
-    c1 = count1
-    c2 = count2
-    p = c2 / N
-    p1 = c12 / c1
-    p2 = (c2 - c12) / (N - c1)
-    score = (l(c12, c1, p) + l(c2 - c12, N - c1, p)
-             - l(c12, c1, p1) - l(c2 - c12, N - c1, p2))
-    return -2 * score
-
-
-def pairwise(iterable):
-    # from itertool recipies
-    # is -> (s0,s1), (s1,s2), (s2, s3), ...
-    a, b = tee(iterable)
-    next(b, None)
-    return zip(a, b)
-
-
-def unigrams_and_bigrams(words, stopwords, normalize_plurals=True, collocation_threshold=30):
-    # We must create the bigrams before removing the stopword tokens from the words, or else we get bigrams like
-    # "thank much" from "thank you very much".
-    # We don't allow any of the words in the bigram to be stopwords
-    bigrams = list(p for p in pairwise(words) if not any(w.lower() in stopwords for w in p))
-    unigrams = list(w for w in words if w.lower() not in stopwords)
-    n_words = len(unigrams)
-    counts_unigrams, standard_form = process_tokens(
-        unigrams, normalize_plurals=normalize_plurals)
-    counts_bigrams, standard_form_bigrams = process_tokens(
-        [" ".join(bigram) for bigram in bigrams],
-        normalize_plurals=normalize_plurals)
-    # create a copy of counts_unigram so the score computation is not changed
-    orig_counts = counts_unigrams.copy()
-
-    # Include bigrams that are also collocations
-    for bigram_string, count in counts_bigrams.items():
-        bigram = tuple(bigram_string.split(" "))
-        word1 = standard_form[bigram[0].lower()]
-        word2 = standard_form[bigram[1].lower()]
-
-        collocation_score = score(count, orig_counts[word1], orig_counts[word2], n_words)
-        if collocation_score > collocation_threshold:
-            # bigram is a collocation
-            # discount words in unigrams dict. hack because one word might
-            # appear in multiple collocations at the same time
-            # (leading to negative counts)
-            counts_unigrams[word1] -= counts_bigrams[bigram_string]
-            counts_unigrams[word2] -= counts_bigrams[bigram_string]
-            counts_unigrams[bigram_string] = counts_bigrams[bigram_string]
-    for word, count in list(counts_unigrams.items()):
-        if count <= 0:
-            del counts_unigrams[word]
-    return counts_unigrams
-
-
-def process_tokens(words, normalize_plurals=True):
-    """Normalize cases and remove plurals.
-
-    Each word is represented by the most common case.
-    If a word appears with an "s" on the end and without an "s" on the end,
-    the version with "s" is assumed to be a plural and merged with the
-    version without "s" (except if the word ends with "ss").
-
-    Parameters
-    ----------
-    words : iterable of strings
-        Words to count.
-
-    normalize_plurals : bool, default=True
-        Whether to try and detect plurals and remove trailing "s".
-
-    Returns
-    -------
-    counts : dict from string to int
-        Counts for each unique word, with cases represented by the most common
-        case, and plurals removed.
-
-    standard_forms : dict from string to string
-        For each lower-case word the standard capitalization.
-    """
-    # words can be either a list of unigrams or bigrams
-    # d is a dict of dicts.
-    # Keys of d are word.lower(). Values are dicts
-    # counting frequency of each capitalization
-    d = defaultdict(dict)
-    for word in words:
-        word_lower = word.lower()
-        # get dict of cases for word_lower
-        case_dict = d[word_lower]
-        # increase this case
-        case_dict[word] = case_dict.get(word, 0) + 1
-    if normalize_plurals:
-        # merge plurals into the singular count (simple cases only)
-        merged_plurals = {}
-        for key in list(d.keys()):
-            if key.endswith('s') and not key.endswith("ss"):
-                key_singular = key[:-1]
-                if key_singular in d:
-                    dict_plural = d[key]
-                    dict_singular = d[key_singular]
-                    for word, count in dict_plural.items():
-                        singular = word[:-1]
-                        dict_singular[singular] = (
-                            dict_singular.get(singular, 0) + count)
-                    merged_plurals[key] = key_singular
-                    del d[key]
-    fused_cases = {}
-    standard_cases = {}
-    item1 = itemgetter(1)
-    for word_lower, case_dict in d.items():
-        # Get the most popular case.
-        first = max(case_dict.items(), key=item1)[0]
-        fused_cases[first] = sum(case_dict.values())
-        standard_cases[word_lower] = first
-    if normalize_plurals:
-        # add plurals to fused cases:
-        for plural, singular in merged_plurals.items():
-            standard_cases[plural] = standard_cases[singular.lower()]
-    return fused_cases, standard_cases
-
-
-def word_tokenize(text: str, custom_dict: Trie = None, keep_whitespace=True):
-
-    """
-    Word tokenizer.
-    (override from PyThaiNLP.word_tokenize)
-
-    Tokenizes running text into words (list of strings).
-
-    :param str text: text to be tokenized
-
-    :param pythainlp.util.Trie custom_dict: dictionary trie
-    :param bool keep_whitespace: True to keep whitespaces, a common mark
-                                 for end of phrase in Thai.
-                                 Otherwise, whitespaces are omitted.
-    :return: list of words
-    """
-
-    if not text or not isinstance(text, str):
-        return []
-    
-    from pythainlp.tokenize.newmm import segment
-
-    segments = segment(text, custom_dict)
-
-    if not keep_whitespace:
-        segments = [token.strip(" ") for token in segments if token.strip(" ")]
-
-    return segments
-
+from collections import defaultdict, Counter
+from itertools import tee
+from math import log
+from pythainlp.util.trie import Trie
+from pythainlp.tokenize.newmm import segment
+from typing import Sequence, Iterable, Set, Dict, Optional
+
+def l(k: int, n: int, x: float):
+    """
+    dunning's likelihood ratio with notation from
+    http://nlp.stanford.edu/fsnlp/promo/colloc.pdf p162
+    """
+    return log(max(x, 1e-10)) * k + log(max(1 - x, 1e-10)) * (n - k)
+
+def score(count_bigram: int, count1: int, count2: int, n_words: int):
+    """Collocation score"""
+    if n_words <= count1 or n_words <= count2:
+        # only one words appears in the whole document
+        return 0
+    N = n_words
+    c12 = count_bigram
+    c1 = count1
+    c2 = count2
+    p = c2 / N
+    p1 = c12 / c1
+    p2 = (c2 - c12) / (N - c1)
+    score = l(c12, c1, p) + l(c2 - c12, N - c1, p) - l(c12, c1, p1) - l(c2 - c12, N - c1, p2)
+    return -2 * score
+
+def pairwise(iterable: Iterable[str]):
+    """
+    from itertool recipies:
+    s -> (s0,s1), (s1,s2), (s2, s3), ...
+    """
+    a, b = tee(iterable)
+    next(b, None)
+    return zip(a, b)
+
+def unigrams_and_bigrams(
+    words: Sequence[str],
+    stopwords: Set[str],
+    collocation_threshold: int,
+):
+    """
+    We must create the bigrams before removing the stopword tokens from the words, or else we get bigrams like
+    "thank much" from "thank you very much".
+    We don't allow any of the words in the bigram to be stopwords
+    """
+    bigrams = [p for p in pairwise(words) if not any(w.lower() in stopwords for w in p)]
+    unigrams = [w for w in words if w.lower() not in stopwords]
+    n_words = len(unigrams)
+
+    counts_unigrams = Counter(unigrams)
+    counts_bigrams = Counter(bigrams)
+    # create a copy of counts_unigram so the score computation is not changed
+    orig_counts = counts_unigrams.copy()
+
+    # Include bigrams that are also collocations
+    for bigram, count in counts_bigrams.items():
+        bigram_string = ''.join(bigram)
+        word1, word2 = bigram
+        collocation_score = score(count, orig_counts[word1], orig_counts[word2], n_words)
+        if collocation_score > collocation_threshold:
+            # bigram is a collocation
+            # discount words in unigrams dict. hack because one word might
+            # appear in multiple collocations at the same time
+            # (leading to negative counts)
+            counts_unigrams[word1] -= counts_bigrams[bigram]
+            counts_unigrams[word2] -= counts_bigrams[bigram]
+            counts_unigrams[bigram_string] = counts_bigrams[bigram]
+    for word, count in list(counts_unigrams.items()):
+        if count <= 0:
+            del counts_unigrams[word]
+    return counts_unigrams
+
+def process_tokens(words: Iterable[str], normalize_plurals: bool):
+    """
+    Normalize cases and remove plurals.
+
+    Each word is represented by the most common case.
+    If a word appears with an "s" on the end and without an "s" on the end,
+    the version with "s" is assumed to be a plural and merged with the
+    version without "s" (except if the word ends with "ss").
+
+    Parameters
+    ----------
+    `words` : `Iterable[str]`
+        Words to count.
+    `normalize_plurals` : `bool`
+        Whether to try and detect plurals and remove trailing "s".
+
+    Returns
+    -------
+    `counts` : `Counter[str]`
+        Counts for each unique word, with cases represented by the most common
+        case, and plurals removed.
+    """
+    # words can be either a list of unigrams or bigrams
+    # d is a dict of dicts.
+    # Keys of d are word.lower(). Values are dicts
+    # counting frequency of each capitalization
+    d: Dict[str, Counter[str]] = defaultdict(Counter)
+    for word in words:
+        word_lower = word.lower()
+        # get dict of cases for word_lower
+        case_dict = d[word_lower]
+        # increase this case
+        case_dict[word] += 1
+    if normalize_plurals:
+        # merge plurals into the singular count (simple cases only)
+        for key in list(d.keys()):
+            if key.endswith('s') and not key.endswith("ss"):
+                key_singular = key[:-1]
+                if key_singular in d:
+                    dict_plural = d[key]
+                    dict_singular = d[key_singular]
+                    for word, count in dict_plural.items():
+                        singular = word[:-1]
+                        dict_singular[singular] += count
+                    del d[key]
+    fused_cases: Counter[str] = Counter()
+    for word_lower, case_dict in d.items():
+        # Get the most popular case.
+        first = case_dict.most_common(1)[0][0]
+        fused_cases[first] = sum(case_dict.values())
+    return fused_cases
+
+def word_tokenize(text: str, custom_dict: Optional[Trie] = None, keep_whitespace: bool = False):
+    """
+    Word tokenizer.
+    (override from PyThaiNLP.word_tokenize)
+
+    Tokenizes running text into words (list of strings).
+
+    Parameters
+    ----------
+    `text`: `str`
+        Text to be tokenized
+    `custom_dict`: `pythainlp.util.Trie` (default=None)
+        Dictionary trie
+    `keep_whitespace`: `bool` (default=False)
+        True to keep whitespaces, a common mark
+        for end of phrase in Thai.
+        Otherwise, whitespaces are omitted.
+
+    Returns
+    -------
+    list of words: `list[str]`
+    """
+    if custom_dict is not None:
+        segments = segment(text, custom_dict)
+    else:
+        segments = segment(text)
+
+    if not keep_whitespace:
+        segments = [token.strip() for token in segments if token.strip()]
+
+    return segments
```

### Comparing `swordcloud-0.0.8/swordcloud/wordcloud.py` & `swordcloud-0.0.9/src/swordcloud/wordcloud.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,1175 +1,1132 @@
-# coding=utf-8
-# derived from: amueller/wordcloud, Author: Andreas Christian Mueller <t3kcit@gmail.com>
-#
-# (c) 2012
-# Modified by: Paul Nechifor <paul@nechifor.net>
-#
-# License: MIT
-
-from __future__ import division
-
-import base64
-import colorsys
-import io
-import os
-import re
-import sys
-import warnings
-from operator import itemgetter
-from random import Random
-from xml.sax import saxutils
-from collections import Counter
-
-import matplotlib
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-from PIL import Image, ImageColor, ImageDraw, ImageFilter, ImageFont
-
-from .query_integral_image import query_integral_image
-from .tokenization import process_tokens, unigrams_and_bigrams, word_tokenize
-from .processing import plot_TSNE, embed_w2v, kmeans_cluster
-
-FILE = os.path.dirname(__file__)
-FONT_PATH = os.environ.get('FONT_PATH', os.path.join(FILE, 'THSarabun.ttf'))
-STOPWORDS = set(map(str.strip, open(os.path.join(FILE, 'stopwords')).readlines()))
-STOPWORDS_TH = set(map(str.strip, open(os.path.join(FILE, 'thstopwords')).readlines()))
-
-
-
-class IntegralOccupancyMap(object):
-    def __init__(self, height, width, mask):
-        self.height = height
-        self.width = width
-        self.text_boxes = []
-        if mask is not None:
-            # the order of the cumsum's is important for speed ?!
-            self.integral = np.cumsum(np.cumsum(255 * mask, axis=1),
-                                      axis=0).astype(np.uint32)
-        else:
-            self.integral = np.zeros((height, width), dtype=np.uint32)
-
-    def sample_position(self, size_x, size_y, random_state):
-        return query_integral_image(self.integral, size_x, size_y,
-                                    random_state)
-    
-    def update(self, img_array, pos_x, pos_y):
-        partial_integral = np.cumsum(np.cumsum(img_array[pos_x:, pos_y:],
-                                               axis=1), axis=0)
-        # paste recomputed part into old image
-        # if x or y is zero it is a bit annoying
-        if pos_x > 0:
-            if pos_y > 0:
-                partial_integral += (self.integral[pos_x - 1, pos_y:]
-                                     - self.integral[pos_x - 1, pos_y - 1])
-            else:
-                partial_integral += self.integral[pos_x - 1, pos_y:]
-        if pos_y > 0:
-            partial_integral += self.integral[pos_x:, pos_y - 1][:, np.newaxis]
-
-        self.integral[pos_x:, pos_y:] = partial_integral
-
-
-class colormap_color_func(object):
-    """Color func created from matplotlib colormap.
-
-    Parameters
-    ----------
-    colormap : string or matplotlib colormap
-        Colormap to sample from
-
-    Example
-    -------
-    >>> WordCloud(color_func=colormap_color_func("magma"))
-
-    """
-    def __init__(self, colormap):
-        self.colormap = plt.cm.get_cmap(colormap)
-
-    def __call__(self, word, font_size, position, orientation,
-                 random_state=None, **kwargs):
-        if random_state is None:
-            random_state = Random()
-        r, g, b, _ = np.maximum(0, 255 * np.array(self.colormap(
-            random_state.uniform(0, 1))))
-        return "rgb({:.0f}, {:.0f}, {:.0f})".format(r, g, b)
-
-
-def get_single_color_func(color):
-    """Create a color function which returns a single hue and saturation with.
-    different values (HSV). Accepted values are color strings as usable by
-    PIL/Pillow.
-
-    >>> color_func1 = get_single_color_func('deepskyblue')
-    >>> color_func2 = get_single_color_func('#00b4d2')
-    """
-    old_r, old_g, old_b = ImageColor.getrgb(color)
-
-    def single_color_func(word=None, font_size=None, position=None,orientation=None, font_path=None, random_state=None):
-        return 'rgb({:.0f}, {:.0f}, {:.0f})'.format(old_r, old_g, old_b)
-    
-    return single_color_func
-
-## from "examples/colored_by_group.py"
-class simple_grouped_color_func(object):
-    """Create a color function object which assigns EXACT colors
-       to certain words based on the color to words mapping
-
-       Parameters
-       ----------
-       color_to_words : dict(str -> list(str))
-         A dictionary that maps a color to the list of words.
-
-       default_color : str
-         Color that will be assigned to a word that's not a member
-         of any value from color_to_words.
-    """
-
-    def __init__(self, color_to_words, default_color):
-        self.word_to_color = {word: color
-                              for (color, words) in color_to_words.items()
-                              for word in words}
-
-        self.default_color = default_color
-
-    def __call__(self, word, **kwargs):
-        return self.word_to_color.get(word, self.default_color)
-
-
-## from "examples/colored_by_group.py"
-class grouped_color_func(object):
-    """Create a color function object which assigns DIFFERENT SHADES of
-       specified colors to certain words based on the color to words mapping.
-
-       Uses wordcloud.get_single_color_func
-
-       Parameters
-       ----------
-       color_to_words : dict(str -> list(str))
-         A dictionary that maps a color to the list of words.
-
-       default_color : str
-         Color that will be assigned to a word that's not a member
-         of any value from color_to_words.
-    """
-
-    def __init__(self, color_to_words, default_color):
-        self.color_func_to_words = [
-            (get_single_color_func(color), set(words))
-            for (color, words) in color_to_words.items()]
-
-        self.default_color_func = get_single_color_func(default_color)
-
-    def get_color_func(self, word):
-        """Returns a single_color_func associated with the word"""
-        try:
-            color_func = next(
-                color_func for (color_func, words) in self.color_func_to_words
-                if word in words)
-        except StopIteration:
-            color_func = self.default_color_func
-
-        return color_func
-
-    def __call__(self, word, **kwargs):
-        return self.get_color_func(word)(word, **kwargs)
-
-
-class WordCloud(object):
-    r"""Word cloud object for generating and drawing.
-
-    Parameters
-    ----------
-    font_path : string
-        Font path to the font that will be used (OTF or TTF).
-        Defaults to DroidSansMono path on a Linux machine. If you are on
-        another OS or don't have this font, you need to adjust this path.
-
-    width : int (default=400)
-        Width of the canvas.
-
-    height : int (default=200)
-        Height of the canvas.
-
-    prefer_horizontal : float (default=0.90)
-        The ratio of times to try horizontal fitting as opposed to vertical.
-        If prefer_horizontal < 1, the algorithm will try rotating the word
-        if it doesn't fit. (There is currently no built-in way to get only
-        vertical words.)
-
-    mask : nd-array or None (default=None)
-        If not None, gives a binary mask on where to draw words. If mask is not
-        None, width and height will be ignored and the shape of mask will be
-        used instead. All white (#FF or #FFFFFF) entries will be considerd
-        "masked out" while other entries will be free to draw on. [This
-        changed in the most recent version!]
-
-    contour_width: float (default=0)
-        If mask is not None and contour_width > 0, draw the mask contour.
-
-    contour_color: color value (default="black")
-        Mask contour color.
-
-    scale : float (default=1)
-        Scaling between computation and drawing. For large word-cloud images,
-        using scale instead of larger canvas size is significantly faster, but
-        might lead to a coarser fit for the words.
-
-    min_font_size : int (default=4)
-        Smallest font size to use. Will stop when there is no more room in this
-        size.
-
-    font_step : int (default=1)
-        Step size for the font. font_step > 1 might speed up computation but
-        give a worse fit.
-
-    max_words : number (default=200)
-        The maximum number of words.
-
-    stopwords : set of strings or None
-        The words that will be eliminated. If None, the build-in STOPWORDS
-        list will be used. Ignored if using generate_from_frequencies.
-
-    background_color : color value (default="black")
-        Background color for the word cloud image.
-
-    max_font_size : int or None (default=None)
-        Maximum font size for the largest word. If None, height of the image is
-        used.
-
-    mode : string (default="RGB")
-        Transparent background will be generated when mode is "RGBA" and
-        background_color is None.
-
-    relative_scaling : float (default='auto')
-        Importance of relative word frequencies for font-size.  With
-        relative_scaling=0, only word-ranks are considered.  With
-        relative_scaling=1, a word that is twice as frequent will have twice
-        the size.  If you want to consider the word frequencies and not only
-        their rank, relative_scaling around .5 often looks good.
-        If 'auto' it will be set to 0.5 unless repeat is true, in which
-        case it will be set to 0.
-
-        .. versionchanged: 2.0
-            Default is now 'auto'.
-
-    color_func : callable, default=None
-        Callable with parameters word, font_size, position, orientation,
-        font_path, random_state that returns a PIL color for each word.
-        Overwrites "colormap".
-        See colormap for specifying a matplotlib colormap instead.
-        To create a word cloud with a single color, use
-        ``color_func=lambda *args, **kwargs: "white"``.
-        The single color can also be specified using RGB code. For example
-        ``color_func=lambda *args, **kwargs: (255,0,0)`` sets color to red.
-
-    regexp : string or None (optional)
-        Regular expression to split the input text into tokens in process_text.
-        If None is specified, ``r"\w[\w']+"`` is used. Ignored if using
-        generate_from_frequencies.
-
-    collocations : bool, default=True
-        Whether to include collocations (bigrams) of two words. Ignored if using
-        generate_from_frequencies.
-
-
-        .. versionadded: 2.0
-
-    colormap : string or matplotlib colormap, default="viridis"
-        Matplotlib colormap to randomly draw colors from for each word.
-        Ignored if "color_func" is specified.
-
-        .. versionadded: 2.0
-
-    normalize_plurals : bool, default=True
-        Whether to remove trailing 's' from words. If True and a word
-        appears with and without a trailing 's', the one with trailing 's'
-        is removed and its counts are added to the version without
-        trailing 's' -- unless the word ends with 'ss'. Ignored if using
-        generate_from_frequencies.
-
-    repeat : bool, default=False
-        Whether to repeat words and phrases until max_words or min_font_size
-        is reached.
-
-    include_numbers : bool, default=False
-        Whether to include numbers as phrases or not.
-
-    min_word_length : int, default=0
-        Minimum number of letters a word must have to be included.
-
-    collocation_threshold: int, default=30
-        Bigrams must have a Dunning likelihood collocation score greater than this
-        parameter to be counted as bigrams. Default of 30 is arbitrary.
-
-        See Manning, C.D., Manning, C.D. and Schütze, H., 1999. Foundations of
-        Statistical Natural Language Processing. MIT press, p. 162
-        https://nlp.stanford.edu/fsnlp/promo/colloc.pdf#page=22
-
-    Attributes
-    ----------
-    ``words_`` : dict of string to float
-        Word tokens with associated frequency.
-
-        .. versionchanged: 2.0
-            ``words_`` is now a dictionary
-
-    ``layout_`` : list of tuples ((string, float), int, (int, int), int, color))
-        Encodes the fitted word cloud. For each word, it encodes the string, 
-        normalized frequency, font size, position, orientation, and color.
-        The frequencies are normalized by the most commonly occurring word.
-        The color is in the format of 'rgb(R, G, B).'
-
-    Notes
-    -----
-    Larger canvases with make the code significantly slower. If you need a
-    large word cloud, try a lower canvas size, and set the scale parameter.
-
-    The algorithm might give more weight to the ranking of the words
-    than their actual frequencies, depending on the ``max_font_size`` and the
-    scaling heuristic.
-    """
-
-    def __init__(self, font_path=None, width=400, height=200, margin=2,
-                 ranks_only=None, prefer_horizontal=.9, mask=None, scale=1,
-                 color_func=None, max_words=200, min_font_size=4,
-                 stopwords=None, random_state=None, background_color='black',
-                 max_font_size=None, font_step=1, mode="RGB",
-                 relative_scaling='auto', regexp=None, collocations=True,
-                 colormap=None, normalize_plurals=True, contour_width=0,
-                 contour_color='black', repeat=False,
-                 include_numbers=False, min_word_length=0, collocation_threshold=30, language='TH'):
-        if font_path is None:
-            font_path = FONT_PATH
-        if color_func is None and colormap is None:
-            version = matplotlib.__version__
-            if version[0] < "2" and version[2] < "5":
-                colormap = "hsv"
-            else:
-                colormap = "viridis"
-        self.colormap = colormap
-        self.collocations = collocations
-        self.font_path = font_path
-        self.width = width
-        self.height = height
-        self.margin = margin
-        self.prefer_horizontal = prefer_horizontal
-        self.mask = mask
-        self.contour_color = contour_color
-        self.contour_width = contour_width
-        self.scale = scale
-        self.color_func = color_func or colormap_color_func(colormap)
-        self.max_words = max_words
-        self.stopwords = stopwords if stopwords is not None else STOPWORDS
-        self.stopwordsth = stopwords if stopwords is not None else STOPWORDS_TH
-        self.min_font_size = min_font_size
-        self.font_step = font_step
-        self.regexp = regexp
-        if isinstance(random_state, int):
-            random_state = Random(random_state)
-        self.random_state = random_state
-        self.background_color = background_color
-        self.max_font_size = max_font_size
-        self.mode = mode
-        self.language = language
-
-        if relative_scaling == "auto":
-            if repeat:
-                relative_scaling = 0
-            else:
-                relative_scaling = .5
-
-        if relative_scaling < 0 or relative_scaling > 1:
-            raise ValueError("relative_scaling needs to be "
-                             "between 0 and 1, got %f." % relative_scaling)
-        self.relative_scaling = relative_scaling
-        if ranks_only is not None:
-            warnings.warn("ranks_only is deprecated and will be removed as"
-                          " it had no effect. Look into relative_scaling.",
-                          DeprecationWarning)
-        self.normalize_plurals = normalize_plurals
-        self.repeat = repeat
-        self.include_numbers = include_numbers
-        self.min_word_length = min_word_length
-        self.collocation_threshold = collocation_threshold
-
-        # Override the width and height if there is a mask
-        if mask is not None:
-            self.width = mask.shape[1]
-            self.height = mask.shape[0]
-
-
-    def generate_from_frequencies(self, frequencies, max_font_size=None, tsne_plot=None, plot_now=True):  # noqa: C901
-        """Create a word_cloud from words and frequencies.
-
-        Parameters
-        ----------
-        frequencies : dict {string: float}
-            A contains words and associated frequency.
-
-        max_font_size : int
-            Use this font-size instead of self.max_font_size
-
-        Returns
-        -------
-        self
-
-        """
-        
-        ## edit
-        if tsne_plot == None:
-            tsne_plot = plot_TSNE(embed_w2v(frequencies,lang=self.language), lang=self.language)
-        
-        maxX = 0
-        maxY = 0
-        for ind in tsne_plot.values():
-            if ind[0] > maxX:
-                maxX = ind[0]
-            if ind[1] > maxY:
-                maxY = ind[1]
-        
-        # make sure frequencies are sorted and normalized
-        frequencies = sorted(frequencies.items(), key=itemgetter(1), reverse=True)
-        if len(frequencies) <= 0:
-            raise ValueError("We need at least 1 word to plot a word cloud, "
-                             "got %d." % len(frequencies))
-        frequencies = frequencies[:self.max_words]
-
-        # largest entry will be 1
-        max_frequency = float(frequencies[0][1])
-
-        frequencies = [(word, freq / max_frequency)
-                       for word, freq in frequencies]
-
-        if self.random_state is not None:
-            random_state = self.random_state
-        else:
-            random_state = Random()
-
-        if self.mask is not None:
-            boolean_mask = self._get_bolean_mask(self.mask)
-            width = self.mask.shape[1]
-            height = self.mask.shape[0]
-        else:
-            boolean_mask = None
-            height, width = self.height, self.width
-        occupancy = IntegralOccupancyMap(height, width, boolean_mask)
-
-        # create image
-        img_grey = Image.new("L", (width, height))
-        draw = ImageDraw.Draw(img_grey)
-        img_array = np.asarray(img_grey)
-        font_sizes, positions, orientations, colors = [], [], [], []
-
-        last_freq = 1.
-
-        if max_font_size is None:
-            # if not provided use default font_size
-            max_font_size = self.max_font_size
-
-        if max_font_size is None:
-            # figure out a good font size by trying to draw with
-            # just the first two words
-            if len(frequencies) == 1:
-                # we only have one word. We make it big!
-                font_size = self.height
-            else:
-                self.generate_from_frequencies(dict(frequencies[:2]),
-                                               max_font_size=self.height, plot_now=False, tsne_plot=tsne_plot)
-                # find font sizes
-                sizes = [x[1] for x in self.layout_]
-                try:
-                    font_size = int(2 * sizes[0] * sizes[1]
-                                    / (sizes[0] + sizes[1]))
-                # quick fix for if self.layout_ contains less than 2 values
-                # on very small images it can be empty
-                except IndexError:
-                    try:
-                        font_size = sizes[0]
-                    except IndexError:
-                        raise ValueError(
-                            "Couldn't find space to draw. Either the Canvas size"
-                            " is too small or too much of the image is masked "
-                            "out.")
-        else:
-            font_size = max_font_size
-
-        self.words_ = dict(frequencies)
-
-        if self.repeat and len(frequencies) < self.max_words:
-            # pad frequencies with repeating words.
-            times_extend = int(np.ceil(self.max_words / len(frequencies))) - 1
-            # get smallest frequency
-            frequencies_org = list(frequencies)
-            downweight = frequencies[-1][1]
-            for i in range(times_extend):
-                frequencies.extend([(word, freq * downweight ** (i + 1))
-                                    for word, freq in frequencies_org])
-
-        # start drawing grey image
-        
-        ## edit
-        collect_font_size = []
-        
-        for word, freq in frequencies:
-            if freq == 0:
-                continue
-            # select the font size
-            rs = self.relative_scaling
-            if rs != 0:
-                font_size = int(round((rs * (freq / float(last_freq))
-                                       + (1 - rs)) * font_size))
-            if random_state.random() < self.prefer_horizontal:
-                orientation = None
-            else:
-                orientation = Image.ROTATE_90
-            tried_other_orientation = False
-            while True:
-                # try to find a position
-                font = ImageFont.truetype(self.font_path, font_size)
-                # transpose font optionally
-                transposed_font = ImageFont.TransposedFont(
-                    font, orientation=orientation)
-                # get size of resulting text
-                box_size = draw.textsize(word, font=transposed_font)
-                # find possible places using integral image:
-                
-                ## edit
-                if word in tsne_plot.keys():
-                    resu = tsne_plot[word]
-                    to_mul_x = width/maxX
-                    to_mul_y = height/maxY
-                    fix_state = (to_mul_x*resu[0],to_mul_y*resu[1]) # x
-                    result = occupancy.sample_position(box_size[1] + self.margin,
-                                                        box_size[0] + self.margin,
-                                                        fix_state)
-                # else:
-                #     result = occupancy.sample_position(box_size[1] + self.margin,
-                #                                        box_size[0] + self.margin,
-                #                                        random_state)
-                
-                if result is not None or font_size < self.min_font_size:
-                    # either we found a place or font-size went too small
-                    break
-                # if we didn't find a place, make font smaller
-                # but first try to rotate!
-                if not tried_other_orientation and self.prefer_horizontal < 1:
-                    orientation = (Image.ROTATE_90 if orientation is None else
-                                   Image.ROTATE_90)
-                    tried_other_orientation = True
-                else:
-                    font_size -= self.font_step
-                    orientation = None
-
-            if font_size < self.min_font_size:
-                # we were unable to draw any more
-                break
-
-            x, y = np.array(result) + self.margin // 2
-            
-            ## edit
-            occupancy.text_boxes.append((x,y, font_size* len(word), font_size))
-            # actually draw the text
-            draw.text((y, x), word, fill="white", font=transposed_font)
-            positions.append((x, y))
-            orientations.append(orientation)
-            font_sizes.append(font_size)
-            # if tsne_plot != None:
-            colors.append(self.color_func(word, font_size=font_size,
-                                            position=(x, y),
-                                            orientation=orientation,
-                                            random_state=None,
-                                            font_path=self.font_path))
-            # else:
-            #     colors.append(self.color_func(word, font_size=font_size,
-            #                                   position=(x, y),
-            #                                   orientation=orientation,
-            #                                   random_state=random_state,
-            #                                   font_path=self.font_path))
-            collect_font_size.append((word,font_size))
-            
-            # recompute integral image
-            if self.mask is None:
-                img_array = np.asarray(img_grey)
-            else:
-                img_array = np.asarray(img_grey) + boolean_mask
-            # recompute bottom right
-            # the order of the cumsum's is important for speed ?!
-            occupancy.update(img_array, x, y)
-            last_freq = freq
-
-        self.layout_ = list(zip(frequencies, font_sizes, positions,
-                                orientations, colors))
-        ## edit
-        # print(collect_font_size)
-        if plot_now:
-            plt.style.use('ggplot')
-            plt.figure(figsize=(32,18))
-            plt.imshow(self,interpolation="bilinear")
-            plt.axis('off')
-            plt.show()
-        return self
-
-    def process_text(self, text, most_common=60):
-        """Tokenization, a.k.a. splits a long text into words, eliminates the stopwords.
-
-        Parameters
-        ----------
-        text : string
-            The text to be processed.
-
-        Returns
-        -------
-        words : dict (string, int)
-            Word tokens with associated frequency.
-
-        Notes
-        -----
-        There are better ways to do word tokenization, but I don't want to
-        include all those things.
-        """
-
-        if self.language == 'TH':
-            stopwords = set([i for i in self.stopwordsth])
-            if type(text) is str:
-                words = word_tokenize(text)
-            else:
-                words = []
-                for t in text:
-                    words.extend(word_tokenize(t))
-            words = [word for word in words if word not in stopwords and word.isspace() is False and word.isnumeric() == False]
-            word_counter = Counter(words).most_common(most_common)
-            word_counts = dict(word_counter)
-
-        elif self.language == 'EN':
-
-            flags = (re.UNICODE if sys.version < '3' and type(text) is unicode  # noqa: F821
-                    else 0)
-            pattern = r"\w[\w']*" if self.min_word_length <= 1 else r"\w[\w']+"
-            regexp = self.regexp if self.regexp is not None else pattern
-
-            words = re.findall(regexp, text, flags)
-            # remove 's
-            words = [word[:-2] if word.lower().endswith("'s") else word
-                    for word in words]
-            # remove numbers
-            if not self.include_numbers:
-                words = [word for word in words if not word.isdigit()]
-            # remove short words
-            if self.min_word_length:
-                words = [word for word in words if len(word) >= self.min_word_length]
-
-            stopwords = set([i.lower() for i in self.stopwords])
-            if self.collocations:
-                word_counts = unigrams_and_bigrams(words, stopwords, self.normalize_plurals, self.collocation_threshold)
-            else:
-                # remove stopwords
-                words = [word for word in words if word.lower() not in stopwords]
-                word_counts, _ = process_tokens(words, self.normalize_plurals)
-
-        return word_counts
-
-    def generate_from_text(self, text, tsne_plot=None, kmeans=False, plot_now=True):
-        """Generate wordcloud from text.
-
-        The input "text" is expected to be a natural text. If you pass a sorted
-        list of words, words will appear in your output twice.
-
-        Calls process_text and generate_from_frequencies.
-
-        Returns
-        -------
-        self
-        """
-        words = self.process_text(text)
-        if kmeans:
-            if not plot_now:
-                print('kmeans option overrides plot_now option')
-            self.generate_kmeans_cloud(words)
-        else:
-            self.generate_from_frequencies(words, tsne_plot, plot_now=plot_now)
-        return self
-
-
-    def gen_kmeans_frequencies(self, model, word_count, label=None, NUM_CLUSTERS=6, size_min=10, size_max=12):
-        """
-        Parameters
-        ----------
-        model : gensim.models.KeyedVector or list of tuple of (str, list[str])
-            word vector model (must come with 'labels') or list of tuple of word and word vectors (no 'labels' needed)
-
-        label : list of str (optional)
-            words that we focused on; only in case of the 'model' is a whole word vector model.
-        
-        Returns
-        -------
-        List from str to tuple of floats, contains coordinates of words.
-        """
-
-        if label is None:
-            label = list(map(lambda x: x[0], model))
-        #   tokens = list(map(lambda x: x[1], model))
-        # else:
-        #   tokens = [model[word] for word in labels]
-
-        df = pd.DataFrame(data={'word': label, 'cluster': kmeans_cluster(model,NUM_CLUSTERS,size_min,size_max)})
-        df['word_count'] = df['word'].map(word_count)
-        k_means_freq = []
-        
-        for i in range(NUM_CLUSTERS):
-            clus_i = df.loc[df['cluster'] == i]
-            clus_i['total'] = clus_i['word_count'].sum()
-            clus_i_dict = {}
-            for _, row in clus_i.iterrows():
-                clus_i_dict[row['word']] = row['word_count']/row['total']
-            sorted_dict_i = sorted(clus_i_dict.items(), key=lambda item: item[1],reverse=True)
-
-            lst = []
-            for k,v in sorted_dict_i:
-                lst.append((k,v))
-            k_means_freq.append((i,lst))
-
-        return k_means_freq
-
-
-    def generate_kmeans_cloud(self, freq):
-        
-        model = embed_w2v(freq, lang=self.language)
-        kmeans_freq = self.gen_kmeans_frequencies(model, freq, NUM_CLUSTERS=6, size_min=10,size_max=12)
-        print(kmeans_freq)
-
-        clouds = []
-        for i in range(6):
-            cloud = WordCloud(font_path=self.font_path,
-                            background_color=self.background_color,
-                            width=self.width//3,
-                            height=self.height//2,
-                            max_words=20,
-                            max_font_size=self.max_font_size,
-                            colormap=self.colormap,
-                            color_func=self.color_func,
-                            prefer_horizontal=1.0,
-                            language=self.language)
-            clouds.append(cloud)
-
-        # Users have no choice but plotting now
-        fig, axes = plt.subplots(2,3, figsize=(32,18), sharex=True, sharey=True)
-
-        for i, ax in enumerate(axes.flatten()):
-            fig.add_subplot(ax)
-            fig.tight_layout(rect=[0, 0.03, 1, 0.95])
-                
-            topic_words = dict(kmeans_freq[i][1]) #list of (words, freq)
-            clouds[i].generate_from_frequencies(topic_words, plot_now=False) # set topic
-            # print(f'generating cloud {i}')
-            plt.gca().imshow(clouds[i],aspect="auto",interpolation = "bilinear")  # blur it right here
-            plt.gca().axis('off')
-
-        # plt.subplots_adjust(wspace=0, hspace=0)
-        # plt.margins(x=0, y=0)
-        plt.show()
-
-        return clouds
-
-    def _check_generated(self):
-        """Check if ``layout_`` was computed, otherwise raise error."""
-        if not hasattr(self, "layout_"):
-            raise ValueError("WordCloud has not been calculated, call generate"
-                             " first.")
-
-    def to_image(self):
-        self._check_generated()
-        if self.mask is not None:
-            width = self.mask.shape[1]
-            height = self.mask.shape[0]
-        else:
-            height, width = self.height, self.width
-
-        img = Image.new(self.mode, (int(width * self.scale),
-                                    int(height * self.scale)),
-                        self.background_color)
-        draw = ImageDraw.Draw(img)
-        for (word, count), font_size, position, orientation, color in self.layout_:
-            font = ImageFont.truetype(self.font_path,
-                                      int(font_size * self.scale))
-            transposed_font = ImageFont.TransposedFont(
-                font, orientation=orientation)
-            pos = (int(position[1] * self.scale),
-                   int(position[0] * self.scale))
-            draw.text(pos, word, fill=color, font=transposed_font)
-
-        return self._draw_contour(img=img)
-
-    def recolor(self, random_state=None, color_func=None, colormap=None):
-        """Recolor existing layout.
-
-        Applying a new coloring is much faster than generating the whole
-        wordcloud.
-
-        Parameters
-        ----------
-        random_state : RandomState, int, or None, default=None
-            If not None, a fixed random state is used. If an int is given, this
-            is used as seed for a random.Random state.
-
-        color_func : function or None, default=None
-            Function to generate new color from word count, font size, position
-            and orientation.  If None, self.color_func is used.
-
-        colormap : string or matplotlib colormap, default=None
-            Use this colormap to generate new colors. Ignored if color_func
-            is specified. If None, self.color_func (or self.color_map) is used.
-
-        Returns
-        -------
-        self
-        """
-        if isinstance(random_state, int):
-            random_state = Random(random_state)
-        self._check_generated()
-
-        if color_func is None:
-            if colormap is None:
-                color_func = self.color_func
-            else:
-                color_func = colormap_color_func(colormap)
-        self.layout_ = [(word_freq, font_size, position, orientation,
-                         color_func(word=word_freq[0], font_size=font_size,
-                                    position=position, orientation=orientation,
-                                    random_state=random_state,
-                                    font_path=self.font_path))
-                        for word_freq, font_size, position, orientation, _
-                        in self.layout_]
-        return self
-
-    def to_file(self, filename):
-        """Export to image file.
-
-        Parameters
-        ----------
-        filename : string
-            Location to write to.
-
-        Returns
-        -------
-        self
-        """
-
-        img = self.to_image()
-        img.save(filename, optimize=True)
-        return self
-
-    def to_array(self):
-        """Convert to numpy array.
-
-        Returns
-        -------
-        image : nd-array size (width, height, 3)
-            Word cloud image as numpy matrix.
-        """
-        return np.array(self.to_image())
-
-    def __array__(self):
-        """Convert to numpy array.
-
-        Returns
-        -------
-        image : nd-array size (width, height, 3)
-            Word cloud image as numpy matrix.
-        """
-        return self.to_array()
-
-    def to_svg(self, embed_font=False, optimize_embedded_font=True, embed_image=False):
-        """Export to SVG.
-
-        Font is assumed to be available to the SVG reader. Otherwise, text
-        coordinates may produce artifacts when rendered with replacement font.
-        It is also possible to include a subset of the original font in WOFF
-        format using ``embed_font`` (requires `fontTools`).
-
-        Note that some renderers do not handle glyphs the same way, and may
-        differ from ``to_image`` result. In particular, Complex Text Layout may
-        not be supported. In this typesetting, the shape or positioning of a
-        grapheme depends on its relation to other graphemes.
-
-        Pillow, since version 4.2.0, supports CTL using ``libraqm``. However,
-        due to dependencies, this feature is not always enabled. Hence, the
-        same rendering differences may appear in ``to_image``. As this
-        rasterized output is used to compute the layout, this also affects the
-        layout generation. Use ``PIL.features.check`` to test availability of
-        ``raqm``.
-
-        Consistant rendering is therefore expected if both Pillow and the SVG
-        renderer have the same support of CTL.
-
-        Contour drawing is not supported.
-
-        Parameters
-        ----------
-        embed_font : bool, default=False
-            Whether to include font inside resulting SVG file.
-
-        optimize_embedded_font : bool, default=True
-            Whether to be aggressive when embedding a font, to reduce size. In
-            particular, hinting tables are dropped, which may introduce slight
-            changes to character shapes (w.r.t. `to_image` baseline).
-
-        embed_image : bool, default=False
-            Whether to include rasterized image inside resulting SVG file.
-            Useful for debugging.
-
-        Returns
-        -------
-        content : string
-            Word cloud image as SVG string
-        """
-
-        # TODO should add option to specify URL for font (i.e. WOFF file)
-
-        # Make sure layout is generated
-        self._check_generated()
-
-        # Get output size, in pixels
-        if self.mask is not None:
-            width = self.mask.shape[1]
-            height = self.mask.shape[0]
-        else:
-            height, width = self.height, self.width
-
-        # Get max font size
-        if self.max_font_size is None:
-            max_font_size = max(w[1] for w in self.layout_)
-        else:
-            max_font_size = self.max_font_size
-
-        # Text buffer
-        result = []
-
-        # Get font information
-        font = ImageFont.truetype(self.font_path, int(max_font_size * self.scale))
-        raw_font_family, raw_font_style = font.getname()
-        # TODO properly escape/quote this name?
-        font_family = repr(raw_font_family)
-        # TODO better support for uncommon font styles/weights?
-        raw_font_style = raw_font_style.lower()
-        if 'bold' in raw_font_style:
-            font_weight = 'bold'
-        else:
-            font_weight = 'normal'
-        if 'italic' in raw_font_style:
-            font_style = 'italic'
-        elif 'oblique' in raw_font_style:
-            font_style = 'oblique'
-        else:
-            font_style = 'normal'
-
-        # Add header
-        result.append(
-            '<svg'
-            ' xmlns="http://www.w3.org/2000/svg"'
-            ' width="{}"'
-            ' height="{}"'
-            '>'
-            .format(
-                width * self.scale,
-                height * self.scale
-            )
-        )
-
-        # Embed font, if requested
-        if embed_font:
-
-            # Import here, to avoid hard dependency on fonttools
-            import fontTools
-            import fontTools.subset
-
-            # Subset options
-            options = fontTools.subset.Options(
-
-                # Small impact on character shapes, but reduce size a lot
-                hinting=not optimize_embedded_font,
-
-                # On small subsets, can improve size
-                desubroutinize=optimize_embedded_font,
-
-                # Try to be lenient
-                ignore_missing_glyphs=True,
-            )
-
-            # Load and subset font
-            ttf = fontTools.subset.load_font(self.font_path, options)
-            subsetter = fontTools.subset.Subsetter(options)
-            characters = {c for item in self.layout_ for c in item[0][0]}
-            text = ''.join(characters)
-            subsetter.populate(text=text)
-            subsetter.subset(ttf)
-
-            # Export as WOFF
-            # TODO is there a better method, i.e. directly export to WOFF?
-            buffer = io.BytesIO()
-            ttf.saveXML(buffer)
-            buffer.seek(0)
-            woff = fontTools.ttLib.TTFont(flavor='woff')
-            woff.importXML(buffer)
-
-            # Create stylesheet with embedded font face
-            buffer = io.BytesIO()
-            woff.save(buffer)
-            data = base64.b64encode(buffer.getbuffer()).decode('ascii')
-            url = 'data:application/font-woff;charset=utf-8;base64,' + data
-            result.append(
-                '<style>'
-                '@font-face{{'
-                'font-family:{};'
-                'font-weight:{};'
-                'font-style:{};'
-                'src:url("{}")format("woff");'
-                '}}'
-                '</style>'
-                .format(
-                    font_family,
-                    font_weight,
-                    font_style,
-                    url
-                )
-            )
-
-        # Select global style
-        result.append(
-            '<style>'
-            'text{{'
-            'font-family:{};'
-            'font-weight:{};'
-            'font-style:{};'
-            '}}'
-            '</style>'
-            .format(
-                font_family,
-                font_weight,
-                font_style
-            )
-        )
-
-        # Add background
-        if self.background_color is not None:
-            result.append(
-                '<rect'
-                ' width="100%"'
-                ' height="100%"'
-                ' style="fill:{}"'
-                '>'
-                '</rect>'
-                .format(self.background_color)
-            )
-
-        # Embed image, useful for debug purpose
-        if embed_image:
-            image = self.to_image()
-            data = io.BytesIO()
-            image.save(data, format='JPEG')
-            data = base64.b64encode(data.getbuffer()).decode('ascii')
-            result.append(
-                '<image'
-                ' width="100%"'
-                ' height="100%"'
-                ' href="data:image/jpg;base64,{}"'
-                '/>'
-                .format(data)
-            )
-
-        # For each word in layout
-        for (word, count), font_size, (y, x), orientation, color in self.layout_:
-            x *= self.scale
-            y *= self.scale
-
-            # Get text metrics
-            font = ImageFont.truetype(self.font_path, int(font_size * self.scale))
-            (size_x, size_y), (offset_x, offset_y) = font.font.getsize(word)
-            ascent, descent = font.getmetrics()
-
-            # Compute text bounding box
-            min_x = -offset_x
-            max_x = size_x - offset_x
-            max_y = ascent - offset_y
-
-            # Compute text attributes
-            attributes = {}
-            if orientation == Image.ROTATE_90:
-                x += max_y
-                y += max_x - min_x
-                transform = 'translate({},{}) rotate(-90)'.format(x, y)
-            else:
-                x += min_x
-                y += max_y
-                transform = 'translate({},{})'.format(x, y)
-
-            # Create node
-            attributes = ' '.join('{}="{}"'.format(k, v) for k, v in attributes.items())
-            result.append(
-                '<text'
-                ' transform="{}"'
-                ' font-size="{}"'
-                ' style="fill:{}"'
-                '>'
-                '{}'
-                '</text>'
-                .format(
-                    transform,
-                    font_size * self.scale,
-                    color,
-                    saxutils.escape(word)
-                )
-            )
-
-        # TODO draw contour
-
-        # Complete SVG file
-        result.append('</svg>')
-        return '\n'.join(result)
-
-    def _get_bolean_mask(self, mask):
-        """Cast to two dimensional boolean mask."""
-        if mask.dtype.kind == 'f':
-            warnings.warn("mask image should be unsigned byte between 0"
-                          " and 255. Got a float array")
-        if mask.ndim == 2:
-            boolean_mask = mask == 255
-        elif mask.ndim == 3:
-            # if all channels are white, mask out
-            boolean_mask = np.all(mask[:, :, :3] == 255, axis=-1)
-        else:
-            raise ValueError("Got mask of invalid shape: %s" % str(mask.shape))
-        return boolean_mask
-
-    def _draw_contour(self, img):
-        """Draw mask contour on a pillow image."""
-        if self.mask is None or self.contour_width == 0:
-            return img
-
-        mask = self._get_bolean_mask(self.mask) * 255
-        contour = Image.fromarray(mask.astype(np.uint8))
-        contour = contour.resize(img.size)
-        contour = contour.filter(ImageFilter.FIND_EDGES)
-        contour = np.array(contour)
-
-        # make sure borders are not drawn before changing width
-        contour[[0, -1], :] = 0
-        contour[:, [0, -1]] = 0
-
-        # use gaussian to change width, divide by 10 to give more resolution
-        radius = self.contour_width / 10
-        contour = Image.fromarray(contour)
-        contour = contour.filter(ImageFilter.GaussianBlur(radius=radius))
-        contour = np.array(contour) > 0
-        contour = np.dstack((contour, contour, contour))
-
-        # color the contour
-        ret = np.array(img) * np.invert(contour)
-        if self.contour_color != 'black':
-            color = Image.new(img.mode, img.size, self.contour_color)
-            ret += np.array(color) * contour
-
-        return Image.fromarray(ret)
-
-
-
+# Derived from: amueller/wordcloud
+# Author: Andreas Christian Mueller <t3kcit@gmail.com>
+#
+# (c) 2012
+# Modified by: Paul Nechifor <paul@nechifor.net>
+#
+# License: MIT
+
+import re
+from base64 import b64encode
+from io import BytesIO
+from os import path, environ
+from operator import itemgetter
+from random import Random
+from xml.sax import saxutils
+from collections import Counter
+from math import sqrt, ceil
+from itertools import zip_longest
+from typing import Dict, Tuple, List, Set, Union, Optional, Literal
+
+import matplotlib.pyplot as plt
+import numpy as np
+from numpy.typing import NDArray
+from pandas import DataFrame
+from PIL import Image, ImageDraw, ImageFont
+
+from gensim.models import KeyedVectors
+import gensim.downloader as api
+from pythainlp.word_vector import WordVector
+
+from .tokenization import process_tokens, unigrams_and_bigrams, word_tokenize
+from .processing import plot_TSNE, kmeans_cluster
+from .occupancy import IntegralOccupancyMap
+from .color_func import RandomColorFunc, Color, ColorFunc
+
+FILE = path.dirname(__file__)
+DEFAULT_FONT_PATH = environ.get('FONT_PATH', path.join(FILE, 'THSarabun.ttf'))
+DEFAULT_EN_STOPWORDS = set(map(str.strip, open(path.join(FILE, 'stopwords'), encoding="utf8")))
+DEFAULT_TH_STOPWORDS = set(map(str.strip, open(path.join(FILE, 'thstopwords'), encoding="utf8")))
+
+class SemanticWordCloud:
+    """
+    Semantic word cloud object for generating and drawing.
+
+    Parameters
+    ----------
+    `language` : `str`
+        Language of input text, can be 'TH' or 'EN'
+
+    `model` : `gensim.models.KeyedVectors` or `str` (default=None)
+        Word vector model. If None, the default model will be used,
+        which is 'glove-wiki-gigaword-50' for English and 'thai2fit-wv' for Thai.
+
+    `width` : `int` (default=400)
+        Width of the canvas.
+
+    `height` : `int` (default=200)
+        Height of the canvas.
+
+    `margin` : `int` (default=2)
+        Margin of text boxes
+
+    `scale` : `float` (default=1)
+        Scaling between computation and drawing. For large word-cloud images,
+        using scale instead of larger canvas size is significantly faster, but
+        might lead to a coarser fit for the words.
+
+    `prefer_horizontal` : `float` (default=0.9)
+        The ratio of times to try horizontal fitting as opposed to vertical.
+        If prefer_horizontal < 1, the algorithm will try rotating the word
+        if it doesn't fit. (There is currently no built-in way to get only
+        vertical words.)
+
+    `color_func` : `Callable`, (default=None)
+        Callable with parameters word, font_size, position, orientation,
+        font_path, random_state that returns a PIL color for each word.
+
+        See swordcloud.color_func for available built-in color functions.
+
+    `background_color` : `Color` (default="white")
+        Background color for the word cloud image.
+
+    `mode` : `str` (default="RGB")
+        Transparent background will be generated when mode is "RGBA" and
+        background_color is None.
+
+    `min_word_length` : `int`, default=0
+        Minimum number of letters a word must have to be included.
+
+    `max_words` : `int` (default=200)
+        The maximum number of words.
+
+    `stopwords` : `set[str]` (default=None)
+        The words that will be eliminated. If None, the build-in STOPWORDS
+        list will be used. Only used when using `generate_from_text` method.
+
+    `font_path` : `str` (default=None)
+        Path to the font file that will be used (OTF or TTF).
+        If None, defaults to the FONT_PATH environment variable.
+        If FONT_PATH is not available, uses THSarabun,
+        which is bundled with swordcloud.
+
+    `min_font_size` : `int` (default=4)
+        Smallest font size to use. Will stop when there is no more room in this
+        size.
+
+    `max_font_size` : `int` (default=None)
+        Maximum font size for the largest word. If None, height of the image is
+        used.
+
+    `font_step` : `int` (default=1)
+        Step size for the font. font_step > 1 might speed up computation but
+        give a worse fit.
+
+    `relative_scaling` : `float` (default='auto')
+        Importance of relative word frequencies for font-size. With
+        relative_scaling=0, only word-ranks are considered.  With
+        relative_scaling=1, a word that is twice as frequent will have twice
+        the size.  If you want to consider the word frequencies and not only
+        their rank, relative_scaling around .5 often looks good.
+        If 'auto' it will be set to 0.5 unless repeat is true, in which
+        case it will be set to 0.
+
+    `regexp` : `str` (default=None)
+        Regular expression to split the input text into tokens in process_text,
+        overriding the default tokenizer. Only used when using `generate_from_text` method.
+
+    `normalize_plurals` : `bool`, (default=True)
+        For English only.
+        Whether to remove trailing 's' from words. If True and a word
+        appears with and without a trailing 's', the one with trailing 's'
+        is removed and its counts are added to the version without
+        trailing 's' -- unless the word ends with 'ss'.
+        Only used when using `generate_from_text` method.
+
+    `repeat` : `bool`, (default=False)
+        Whether to repeat words and phrases until max_words or min_font_size
+        is reached.
+
+    `include_numbers` : `bool`, (default=False)
+        Whether to include numbers as phrases or not.
+        Only used when using `generate_from_text` method.
+
+    `collocations` : `bool`, (default=False)
+        Whether to include collocations (bigrams) of two words.
+        Only used when using `generate_from_text` method.
+
+    `collocation_threshold`: `int`, (default=30)
+        Bigrams must have a Dunning likelihood collocation score greater than this
+        parameter to be counted as bigrams. Default of 30 is arbitrary.
+
+        See Manning, C.D., Manning, C.D. and Schütze, H., 1999. Foundations of
+        Statistical Natural Language Processing. MIT press, p. 162
+        https://nlp.stanford.edu/fsnlp/promo/colloc.pdf#page=22
+
+    `random_state` : `random.Random` or `int` (default=None)
+        Random state to be used for random drawing.
+
+    Attributes
+    ----------
+    `sub_clouds` : `list[SemanticWordCloud]`
+        List of sub clouds generated by K-Means algorithm.
+        This attribute only exists after `generate_kmeans_cloud`
+        or `generate_from_text` with `kmeans` is called.
+
+    `words_` : `dict[str, float]`
+        Word tokens with associated frequency.
+
+    `layout_`: `list[tuple[tuple[string, float], int, tuple[int, int], int, color)]]`
+        Encodes the fitted word cloud. For each word, it encodes the string, 
+        normalized frequency, font size, position, orientation, and color.
+        The frequencies are normalized by the most commonly occurring word.
+        The color is in the format of 'rgb(R, G, B).'
+
+    Notes
+    -----
+    Larger canvases with make the code significantly slower. If you need a
+    large word cloud, try a lower canvas size, and set the scale parameter.
+
+    The algorithm might give more weight to the ranking of the words
+    than their actual frequencies, depending on the `max_font_size` and the
+    scaling heuristic.
+    """
+    def __init__(
+        self,
+        language: Literal['TH', 'EN'],
+        model: Optional[Union[KeyedVectors, str]] = None,
+        width: int = 400,
+        height: int = 200,
+        margin: int = 2,
+        scale: float = 1,
+        prefer_horizontal: float = 0.9,
+        color_func: ColorFunc = RandomColorFunc,
+        background_color: Color = 'white',
+        mode: str = "RGB",
+        min_word_length: int = 0,
+        max_words: int = 200,
+        stopwords: Optional[Set[str]] = None,
+        font_path: Optional[str] = None,
+        min_font_size: int = 4,
+        max_font_size: Optional[int] = None,
+        font_step: int = 1,
+        relative_scaling: Union[float, Literal['auto']] = 'auto',
+        regexp: Optional[str] = None,
+        normalize_plurals: Optional[bool] = None,
+        repeat: bool = False,
+        include_numbers: bool = False,
+        collocations: bool = False,
+        collocation_threshold: Optional[int] = None,
+        random_state: Optional[Union[Random, int]] = None
+    ):
+        if language not in ('TH', 'EN'):
+            raise ValueError(f"language must be either 'TH' or 'EN', got {repr(language)}.")
+        self.language: Literal['TH', 'EN'] = language
+
+        if isinstance(model, KeyedVectors):
+            self.model = model
+        elif isinstance(model, str):
+            if language == 'EN':
+                self.model = api.load(model)
+            else:
+                self.model = WordVector(model).get_model()
+        elif language == 'TH':
+            self.model = WordVector("thai2fit_wv").get_model()
+        else:
+            self.model = api.load("glove-wiki-gigaword-50")
+
+        if normalize_plurals is None:
+            self.normalize_plurals = language == 'EN'
+        elif normalize_plurals and language == 'TH':
+            self.normalize_plurals = False
+            print(
+                "WARNING: normalize_plurals is not supported for Thai "
+                "since Thai does not have morphological plurals."
+            )
+        else:
+            self.normalize_plurals = normalize_plurals
+
+        if stopwords is not None:
+            self.stopwords = {w.lower() for w in stopwords}
+        elif language == 'TH':
+            self.stopwords = DEFAULT_TH_STOPWORDS
+        else:
+            self.stopwords = DEFAULT_EN_STOPWORDS
+
+        if collocation_threshold is not None:
+            collocations = True
+        else:
+            collocation_threshold = 30
+        if collocations and language == 'EN':
+            collocations = False
+            print(
+                "WARNING: collocations is not supported for English "
+                "since English word vector models do not contain bigrams."
+            )
+        self.collocations = collocations
+        self.collocation_threshold = collocation_threshold
+
+        if relative_scaling == "auto":
+            if repeat:
+                relative_scaling = 0
+            else:
+                relative_scaling = .5
+        elif relative_scaling < 0 or relative_scaling > 1:
+            raise ValueError(f"relative_scaling needs to be between 0 and 1, got {relative_scaling}.")
+        self.relative_scaling = relative_scaling
+
+        if regexp is not None:
+            self.regexp = re.compile(regexp)
+        elif regexp is None and language == 'EN':
+            self.regexp = re.compile(r"\w[\w']*" if min_word_length <= 1 else r"\w[\w']+")
+        else:
+            self.regexp = None
+
+        if not isinstance(random_state, Random):
+            random_state = Random(random_state)
+        self.random_state = random_state
+
+        self.font_path = font_path or DEFAULT_FONT_PATH
+        self.width = width
+        self.height = height
+        self.margin = margin
+        self.prefer_horizontal = prefer_horizontal
+        self.scale = scale
+        self.max_words = max_words
+        self.min_font_size = min_font_size
+        self.font_step = font_step
+        self.color_func = color_func
+        self.background_color = background_color
+        self.max_font_size = max_font_size
+        self.mode = mode
+        self.repeat = repeat
+        self.include_numbers = include_numbers
+        self.min_word_length = min_word_length
+
+        self.sub_clouds: List[SemanticWordCloud] = []
+        self.layout_: List[Tuple[Tuple[str, float], int, Tuple[int, int], Optional[int], Color]] = []
+
+    def _embed_w2v(
+        self,
+        frequency_dict: Union[Dict[str, int], Dict[str, float]]
+    ) -> List[Tuple[str, NDArray[np.float32]]]:
+        """
+        Parameters
+        ----------
+        `frequency_dict` : `dict[str, int]` | `dict[str, float]`
+            contains words and associated frequency.
+
+        Returns
+        -------
+        List of tuples of word and its word vector: `list[tuple[str, NDArray[float32]]]`
+        """
+        return [
+            (word, self.model[word]) # type: ignore
+            for word in sorted(frequency_dict, key=lambda k: frequency_dict[k], reverse=True)
+                if word in self.model
+        ][:self.max_words]
+
+    def generate_from_frequencies(
+        self,
+        frequency_dict: Union[Dict[str, int], Dict[str, float]],
+        max_font_size: Optional[int] = None,
+        tsne_plot: Optional[Dict[str, Tuple[float, float]]] = None,
+        plot_now: bool = True,
+        random_state: Optional[Union[Random, int]] = None
+    ):
+        """
+        Create a semantic word cloud from words and frequencies.
+
+        Parameters
+        ----------
+        `frequency_dict` : `dict[str, int]`
+            A contains words and associated frequency.
+
+        `max_font_size` : `int` (default=None)
+            Use this font-size instead of self.max_font_size
+
+        `tsne_plot` : `dict[str, tuple[float, float]]` (default=None)
+            A dictionary of word and its coordinates from TSNE plot.
+            If None, a TSNE plot will be generated.
+
+        `plot_now` : `bool` (default=True)
+            Whether to plot the word cloud immediately.
+
+        `random_state` : `random.Random` or `int` (default=None)
+            Random state to be used for random drawing.
+        """
+        if len(frequency_dict) <= 0:
+            raise ValueError(
+                f"We need at least 1 word to plot a word cloud, got {len(frequency_dict)}."
+            )
+
+        if random_state is None:
+            random_state = self.random_state
+        elif not isinstance(random_state, Random):
+            random_state = Random(random_state)
+
+        if tsne_plot is None:
+            tsne_plot = plot_TSNE(
+                self._embed_w2v(frequency_dict),
+                language = self.language,
+                random_state = random_state
+            )
+
+        maxX = 0
+        maxY = 0
+        for ind in tsne_plot.values():
+            if ind[0] > maxX:
+                maxX = ind[0]
+            if ind[1] > maxY:
+                maxY = ind[1]
+        
+        # make sure frequencies are sorted and normalized
+        frequencies = sorted(
+            ((k, v) for k, v in frequency_dict.items() if k in tsne_plot),
+            key=itemgetter(1),
+            reverse=True
+        )
+        # largest entry will be 1
+        max_frequency = float(frequencies[0][1])
+        frequencies = [(word, freq / max_frequency) for word, freq in frequencies]
+
+        height, width = self.height, self.width
+        occupancy = IntegralOccupancyMap(height, width)
+
+        # create image
+        img_grey = Image.new("L", (width, height))
+        draw = ImageDraw.Draw(img_grey)
+        img_array = np.asarray(img_grey)
+
+        font_sizes: List[int] = []
+        positions: List[Tuple[int, int]] = []
+        orientations: List[Optional[int]] = []
+        colors: List[Color] = []
+
+        if max_font_size is None:
+            # if not provided use default font_size
+            max_font_size = self.max_font_size
+
+        if max_font_size is None:
+            # figure out a good font size by trying to draw with
+            # just the first two words
+            if len(frequencies) == 1:
+                # We only have one word. Make it big!
+                font_size = self.height
+            else:
+                self.generate_from_frequencies(
+                    dict(frequencies[:2]),
+                    max_font_size = self.height,
+                    plot_now = False,
+                    tsne_plot = tsne_plot,
+                    random_state = random_state
+                )
+                # find font sizes
+                sizes = [x[1] for x in self.layout_]
+                try:
+                    font_size = int(2 * sizes[0] * sizes[1] / (sizes[0] + sizes[1]))
+                # quick fix for if self.layout_ contains less than 2 values
+                # on very small images it can be empty
+                except IndexError:
+                    try:
+                        font_size = sizes[0]
+                    except IndexError:
+                        raise ValueError(
+                            "Couldn't find space to draw. The Canvas size might be too small."
+                        )
+        else:
+            font_size = max_font_size
+
+        self.words_ = dict(frequencies)
+
+        if self.repeat and len(frequencies) < self.max_words:
+            # pad frequencies with repeating words.
+            times_extend = int(np.ceil(self.max_words / len(frequencies))) - 1
+            # get smallest frequency
+            frequencies_org = list(frequencies)
+            downweight = frequencies[-1][1]
+            for i in range(times_extend):
+                frequencies.extend([
+                    (word, freq * downweight ** (i + 1))
+                    for word, freq in frequencies_org
+                ])
+
+        # start drawing grey image
+        ## edit
+        last_freq = 1.
+        last_font_size = font_size
+        cant_draw: Set[int] = set()
+        for i, (word, freq) in enumerate(frequencies):
+            if freq == 0:
+                continue
+            # select the font size
+            rs = self.relative_scaling
+            if rs != 0:
+                font_size = int(round((rs * (freq / float(last_freq)) + (1 - rs)) * last_font_size))
+            if random_state.random() < self.prefer_horizontal:
+                orientation = None
+            else:
+                orientation = Image.ROTATE_90
+            tried_other_orientation = False
+            while True:
+                # try to find a position
+                font = ImageFont.truetype(self.font_path, font_size)
+                # transpose font optionally
+                transposed_font = ImageFont.TransposedFont(font, orientation=orientation)
+                # get size of resulting text
+                box_size = draw.textsize(word, font=transposed_font)
+
+                # find possible places using integral image:
+                resu = tsne_plot[word]
+                to_mul_x = width / maxX
+                to_mul_y = height / maxY
+                fix_state = (to_mul_x * resu[0], to_mul_y * resu[1])
+                result = occupancy.sample_position(
+                    box_size[1] + self.margin, box_size[0] + self.margin, fix_state
+                )
+                
+                if result is not None or font_size < self.min_font_size:
+                    # either we found a place or font-size went too small
+                    break
+                # if we didn't find a place, make font smaller
+                # but first try to rotate!
+                if not tried_other_orientation and self.prefer_horizontal < 1:
+                    orientation = Image.ROTATE_90
+                    tried_other_orientation = True
+                else:
+                    font_size -= self.font_step
+                    orientation = None
+
+            if font_size < self.min_font_size:
+                # Word became too small, skip to next word
+                cant_draw.add(i)
+                continue
+
+            x, y = np.array(result) + self.margin // 2
+            
+            # actually draw the text
+            draw.text((y, x), word, fill="white", font=transposed_font)
+            positions.append((x, y))
+            orientations.append(orientation)
+            font_sizes.append(font_size)
+            colors.append(
+                self.color_func(
+                    word = word,
+                    font_size = font_size,
+                    position = (x, y),
+                    orientation = orientation,
+                    random_state = random_state,
+                    font_path = self.font_path
+                )
+            )
+
+            # recompute integral image
+            img_array = np.asarray(img_grey)
+            # recompute bottom right
+            occupancy.update(img_array, x, y)
+            last_freq = freq
+            last_font_size = font_size
+
+        self.sub_clouds.clear()
+        self.layout_ = list(zip(
+            [(w, f) for i, (w, f) in enumerate(frequencies) if i not in cant_draw],
+            font_sizes,
+            positions,
+            orientations,
+            colors
+        ))
+
+        if plot_now:
+            self.show()
+
+    def _process_text(self, text: Union[str, List[str]]):
+        """
+        Tokenization, a.k.a. splits a long text into words, eliminates the stopwords.
+
+        Parameters
+        ----------
+        `text` : `str` | `list[str]`
+            The text to be processed.
+
+        Returns
+        -------
+        `words` : `Counter[str]`
+            Word tokens with associated frequency.
+        """
+        # EN is guaranteed to have regexp
+        if self.regexp:
+            if isinstance(text, list):
+                text = '\n'.join(text)
+            words: List[str] = self.regexp.findall(text)
+            # remove 's
+            if self.language == 'EN':
+                words = [
+                    word[:-2] if word.lower().endswith("'s") else word
+                    for word in words
+                ]
+        else:
+            if isinstance(text, str):
+                words = word_tokenize(text)
+            else:
+                words = [word for t in text for word in word_tokenize(t)]
+
+        def is_number(s: str):
+            try:
+                float(s)
+                return True
+            except ValueError:
+                return False
+        # remove numbers
+        if not self.include_numbers:
+            words = [word for word in words if not is_number(word)]
+        # remove short words
+        if self.min_word_length:
+            words = [word for word in words if len(word) >= self.min_word_length]
+
+        if self.collocations:
+            word_counts = unigrams_and_bigrams(
+                words, self.stopwords, self.collocation_threshold
+            )
+        else:
+            # remove stopwords
+            words = [word for word in words if word.lower() not in self.stopwords]
+            if self.language == 'EN':
+                word_counts = process_tokens(words, self.normalize_plurals)
+            else:
+                word_counts = Counter(words)
+
+        return word_counts
+
+    def generate_from_text(
+        self,
+        text: Union[str, List[str]],
+        tsne_plot: Optional[Dict[str, Tuple[float, float]]] = None,
+        kmeans: Optional[int] = None,
+        plot_now: bool = True,
+        random_state: Optional[Union[Random, int]] = None
+    ):
+        """
+        Generate wordcloud from raw natural text.
+        This method calls `process_text` and then either
+        `generate_from_frequencies` or `generate_kmeans_cloud`.
+        If kmeans is not None, the generated sub clouds can be
+        accessed via `sub_clouds` attribute.
+
+        Parameters
+        ----------
+        `text` : `str` | `list[str]`
+            The text to be processed.
+
+        `tsne_plot` : `dict[str, tuple[float, float]]` (default=None)
+            A dictionary of word and its coordinates from TSNE plot.
+            If None, a TSNE plot will be generated.
+            Mutually exclusive with `kmeans`.
+
+        `kmeans` : `int` (default=None)
+            Number of clusters for K-Means algorithm.
+            Mutually exclusive with `tsne_plot`.
+
+        `plot_now` : `bool` (default=True)
+            Whether to plot the word cloud immediately.
+
+        `random_state` : `random.Random` or `int` (default=None)
+            Random state to be used for random drawing.
+        """
+        if tsne_plot is not None and kmeans is not None:
+            raise ValueError("Cannot use both tsne_plot and kmeans at the same time.")
+
+        words = self._process_text(text)
+        if kmeans is not None:
+            if kmeans <= 1:
+                raise ValueError(f'kmeans must be greater than 1, got {kmeans}.')
+            self.generate_kmeans_cloud(
+                frequency_dict = words,
+                n_clusters = kmeans,
+                plot_now = plot_now,
+                random_state = random_state
+            )
+        else:
+            self.generate_from_frequencies(
+                frequency_dict = words,
+                tsne_plot = tsne_plot,
+                plot_now = plot_now,
+                random_state = random_state
+            )
+
+    def _gen_kmeans_frequencies(
+        self,
+        model: List[Tuple[str, NDArray[np.float32]]],
+        frequency_dict: Union[Dict[str, int], Dict[str, float]],
+        n_clusters: int,
+        random_state: Random
+    ):
+        """
+        Parameters
+        ----------
+        `model` : list[tuple[str, NDArray[float32]]]
+            List of tuple of word and its word vectors
+
+        `frequency_dict` : `dict[str, int]` | `dict[str, float]`
+            Words and their associated frequency.
+
+        `n_clusters` : `int`
+            Number of clusters for K-Means algorithm.
+
+        `random_state` : `random.Random` or `int` (default=None)
+            Random state to be used for K-Means algorithm.
+
+        Returns
+        -------
+        `list[tuple[int, list[tuple[str, float]]]]`
+            List of tuple of cluster number and list of tuple of word and its frequency
+        """
+        label = list(map(lambda x: x[0], model))
+        df = DataFrame(data={
+            'word': label,
+            'cluster': kmeans_cluster(
+                model = model,
+                n_clusters = n_clusters,
+                random_state = random_state
+            )
+        })
+        df['word_count'] = df['word'].map(frequency_dict)
+
+        k_means_freq: List[Tuple[int, List[Tuple[str, float]]]] = []        
+        for i in range(n_clusters):
+            clus_i = df.loc[df['cluster'] == i]
+            total = clus_i['word_count'].sum()
+            clus_i_dict: Dict[str, float] = {}
+            for _, row in clus_i.iterrows():
+                clus_i_dict[row['word']] = row['word_count'] / total
+            sorted_dict_i = sorted(clus_i_dict.items(), key=lambda item: item[1], reverse=True)
+
+            lst: List[Tuple[str, float]] = []
+            for k, v in sorted_dict_i:
+                lst.append((k, v))
+            k_means_freq.append((i, lst))
+
+        return k_means_freq
+
+
+    def generate_kmeans_cloud(
+        self,
+        frequency_dict: Union[Dict[str, int], Dict[str, float]],
+        n_clusters: int,
+        plot_now: bool = True,
+        random_state: Optional[Union[Random, int]] = None
+    ):
+        """
+        Generate semantic word cloud using K-Means algorithm.
+        The generated sub clouds can be accessed via `sub_clouds` attribute.
+
+        Parameters
+        ----------
+        `frequency_dict` : `dict[str, int]` | `dict[str, float]`
+            Words and their associated frequency.
+
+        `n_clusters` : `int`
+            Number of clusters for K-Means algorithm.
+
+        `plot_now` : `bool` (default=True)
+            Whether to plot the word cloud immediately.
+
+        `random_state` : `random.Random` or `int` (default=None)
+            Random state to be used for K-Means algorithm.
+        """
+        if random_state is None:
+            random_state = self.random_state
+        elif not isinstance(random_state, Random):
+            random_state = Random(random_state)
+
+        model = self._embed_w2v(frequency_dict)
+        kmeans_freq = self._gen_kmeans_frequencies(
+            model,
+            frequency_dict,
+            n_clusters = n_clusters,
+            random_state = random_state
+        )
+
+        n_vertical = n_horizontal = ceil(sqrt(n_clusters))
+        if (n_vertical - 1) * n_horizontal >= n_clusters:
+            n_vertical -= 1
+
+        self.layout_.clear()
+        self.sub_clouds = [
+            SemanticWordCloud(
+                language = self.language,
+                model = self.model,
+                width = self.width // n_horizontal,
+                height = self.height // n_vertical,
+                margin = self.margin,
+                scale = self.scale,
+                prefer_horizontal = self.prefer_horizontal,
+                color_func = self.color_func,
+                background_color = self.background_color,
+                mode = self.mode,
+                min_word_length = self.min_word_length,
+                max_words = self.max_words,
+                stopwords = self.stopwords,
+                font_path = self.font_path,
+                min_font_size = self.min_font_size,
+                max_font_size = self.max_font_size,
+                font_step = self.font_step,
+                relative_scaling = self.relative_scaling,
+                regexp = self.regexp.pattern if self.regexp else None,
+                normalize_plurals = self.normalize_plurals,
+                repeat = self.repeat,
+                include_numbers = self.include_numbers,
+                collocations = self.collocations,
+                collocation_threshold = self.collocation_threshold,
+                random_state = random_state,
+            ) for _ in range(n_clusters)
+        ]
+
+        for i, cloud in enumerate(self.sub_clouds):
+            topic_words = dict(kmeans_freq[i][1]) # list of (words, freq)
+            cloud.generate_from_frequencies(topic_words, plot_now=False) # set topic
+
+        if plot_now:
+            self.show()
+
+    def show(self):
+        self._check_generated()
+        if self.sub_clouds:
+            n_clusters = len(self.sub_clouds)
+            n_vertical = n_horizontal = ceil(sqrt(n_clusters))
+            if (n_vertical - 1) * n_horizontal >= n_clusters:
+                n_vertical -= 1
+
+            dpi = plt.rcParams['figure.dpi']
+            fig, axes = plt.subplots(
+                n_vertical,
+                n_horizontal,
+                figsize=(self.width / dpi, self.height / dpi),
+                sharex=True,
+                sharey=True
+            )
+            for cloud, ax in zip_longest(self.sub_clouds, axes.flatten()):
+                ax.axhline(y=0, color='black', linewidth=1)
+                ax.axvline(x=0, color='black', linewidth=1)
+                fig.add_subplot(ax)
+                fig.tight_layout(rect=(0, 0.03, 1, 0.95))
+                if cloud is not None:
+                    plt.gca().imshow(cloud, aspect="auto", interpolation="bilinear")
+                plt.gca().axis('off')
+            plt.subplots_adjust(wspace=0, hspace=0)
+            plt.show()
+        else:
+            dpi = plt.rcParams['figure.dpi']
+            plt.style.use('ggplot')
+            plt.figure(figsize=(self.width / dpi, self.height / dpi))
+            plt.imshow(self, interpolation="bilinear")
+            plt.axis('off')
+            plt.show()
+
+    def _check_generated(self):
+        """Check if `layout_` or `sub_clouds` was computed, otherwise raise error."""
+        if not (self.layout_ or self.sub_clouds):
+            raise ValueError("SemanticWordCloud has not been calculated, call generate first.")
+
+    def to_image(self):
+        """Convert to `pillow`'s image."""
+        self._check_generated()
+        if self.sub_clouds:
+            raise ValueError(
+                "Cannot directly convert a SemanticWordCloud with sub clouds to image. "
+                "Call `to_image` individually from a sub cloud instead."
+            )
+
+        height, width = self.height, self.width
+
+        img = Image.new(
+            self.mode,
+            (int(width * self.scale), int(height * self.scale)),
+            self.background_color
+        )
+        draw = ImageDraw.Draw(img)
+        for (word, _), font_size, position, orientation, color in self.layout_:
+            font = ImageFont.truetype(self.font_path, int(font_size * self.scale))
+            transposed_font = ImageFont.TransposedFont(font, orientation=orientation)
+            pos = (int(position[1] * self.scale), int(position[0] * self.scale))
+            draw.text(pos, word, fill=color, font=transposed_font)
+
+        return img
+
+    def recolor(
+        self,
+        color_func: Optional[ColorFunc] = None,
+        plot_now: bool = True,
+        random_state: Optional[Union[Random, int]] = None
+    ):
+        """
+        Recolor existing layout.
+
+        Applying a new coloring is much faster than generating the whole
+        wordcloud.
+
+        Parameters
+        ----------
+        `color_func` : `Callable`
+            Function to generate new colors. If None, self.color_func is used again.
+
+        plot_now : `bool` (default=True)
+            Whether to plot the recolored word cloud immediately.
+    
+        `random_state` : `random.Random` or `int` (default=None)
+            If None, use self.random_state.
+            If not None, a fixed random state is used. If an int is given, this
+            is used as seed for a random.Random state.
+        """
+        if random_state is None:
+            random_state = self.random_state
+        elif not isinstance(random_state, Random):
+            random_state = Random(random_state)
+
+        if color_func is None:
+            color_func = self.color_func
+
+        self._check_generated()
+        if self.sub_clouds:
+            for cloud in self.sub_clouds:
+                cloud.recolor(color_func, plot_now=False, random_state=random_state)
+        else:
+            self.layout_ = [
+                (
+                    word_freq,
+                    font_size,
+                    position,
+                    orientation,
+                    color_func(
+                        word = word_freq[0],
+                        font_size = font_size,
+                        position = position,
+                        orientation = orientation,
+                        random_state = random_state,
+                        font_path = self.font_path
+                    )
+                )
+                for word_freq, font_size, position, orientation, _ in self.layout_
+            ]
+
+        if plot_now:
+            self.show()
+
+    def to_file(self, filename: str):
+        """
+        Export to image file.
+
+        Parameters
+        ----------
+        `filename` : `str`
+            Location to write to.
+        """
+        if self.sub_clouds:
+            filename, extension = path.splitext(filename)
+            for i, cloud in enumerate(self.sub_clouds, start=1):
+                cloud.to_file(filename + '_' + str(i) + extension)
+        else:
+            img = self.to_image()
+            img.save(filename, optimize=True)
+
+    def to_array(self):
+        """
+        Convert to numpy array.
+
+        Returns
+        -------
+        `image` : `NDArray` size (width, height, 3)
+            Word cloud image as numpy matrix.
+        """
+        return np.array(self.to_image())
+
+    def __array__(self):
+        """
+        Convert to numpy array.
+
+        Returns
+        -------
+        `image` : `NDArray` size (width, height, 3)
+            Word cloud image as numpy matrix.
+        """
+        return self.to_array()
+
+    def to_svg(
+        self,
+        embed_font: bool = False,
+        optimize_embedded_font: bool = True,
+        embed_image: bool = False
+    ):
+        """
+        Export to SVG.
+
+        Font is assumed to be available to the SVG reader. Otherwise, text
+        coordinates may produce artifacts when rendered with replacement font.
+        It is also possible to include a subset of the original font in WOFF
+        format using `embed_font` (requires `fontTools`).
+
+        Note that some renderers do not handle glyphs the same way, and may
+        differ from `to_image` result. In particular, Complex Text Layout may
+        not be supported. In this typesetting, the shape or positioning of a
+        grapheme depends on its relation to other graphemes.
+
+        Pillow, since version 4.2.0, supports CTL using ``libraqm``. However,
+        due to dependencies, this feature is not always enabled. Hence, the
+        same rendering differences may appear in ``to_image``. As this
+        rasterized output is used to compute the layout, this also affects the
+        layout generation. Use ``PIL.features.check`` to test availability of
+        ``raqm``.
+
+        Consistant rendering is therefore expected if both Pillow and the SVG
+        renderer have the same support of CTL.
+
+        Parameters
+        ----------
+        `embed_font` : `bool`, (default=False)
+            Whether to include font inside resulting SVG file.
+
+        `optimize_embedded_font` : `bool`, (default=True)
+            Whether to be aggressive when embedding a font, to reduce size. In
+            particular, hinting tables are dropped, which may introduce slight
+            changes to character shapes (w.r.t. `to_image` baseline).
+
+        `embed_image` : `bool`, (default=False)
+            Whether to include rasterized image inside resulting SVG file.
+            Useful for debugging.
+
+        Returns
+        -------
+        `content` : `str`
+            Word cloud image as SVG string
+        """
+
+        # TODO should add option to specify URL for font (i.e. WOFF file)
+
+        # Make sure layout is generated
+        self._check_generated()
+        if self.sub_clouds:
+            raise ValueError(
+                "Cannot directly convert a SemanticWordCloud with sub clouds to SVG. "
+                "Call `to_svg` from a sub cloud individually instead."
+            )
+
+        # Get output size, in pixels
+        height, width = self.height, self.width
+
+        # Get max font size
+        if self.max_font_size is None:
+            max_font_size = max(w[1] for w in self.layout_)
+        else:
+            max_font_size = self.max_font_size
+
+        # Text buffer
+        result: List[str] = []
+
+        # Get font information
+        font = ImageFont.truetype(self.font_path, int(max_font_size * self.scale))
+        raw_font_family, raw_font_style = font.getname()
+        # TODO properly escape/quote this name?
+        font_family = repr(raw_font_family)
+        # TODO better support for uncommon font styles/weights?
+        raw_font_style = raw_font_style.lower()
+        if 'bold' in raw_font_style:
+            font_weight = 'bold'
+        else:
+            font_weight = 'normal'
+        if 'italic' in raw_font_style:
+            font_style = 'italic'
+        elif 'oblique' in raw_font_style:
+            font_style = 'oblique'
+        else:
+            font_style = 'normal'
+
+        # Add header
+        result.append(
+            f'<svg xmlns="http://www.w3.org/2000/svg" width="{width * self.scale}" height="{height * self.scale}">'
+        )
+
+        # Embed font, if requested
+        if embed_font:
+
+            # Import here, to avoid hard dependency on fonttools
+            import fontTools.subset
+            from fontTools.ttLib import TTFont
+
+            # Subset options
+            options = fontTools.subset.Options(
+                # Small impact on character shapes, but reduce size a lot
+                hinting = not optimize_embedded_font,
+                # On small subsets, can improve size
+                desubroutinize = optimize_embedded_font,
+                # Try to be lenient
+                ignore_missing_glyphs = True,
+            )
+
+            # Load and subset font
+            ttf = fontTools.subset.load_font(self.font_path, options)
+            subsetter = fontTools.subset.Subsetter(options)
+            characters = {c for item in self.layout_ for c in item[0][0]}
+            text = ''.join(characters)
+            subsetter.populate(text=text)
+            subsetter.subset(ttf)
+
+            # Export as WOFF
+            # TODO is there a better method, i.e. directly export to WOFF?
+            buffer = BytesIO()
+            ttf.saveXML(buffer)
+            buffer.seek(0)
+            woff = TTFont(flavor='woff')
+            woff.importXML(buffer)
+
+            # Create stylesheet with embedded font face
+            buffer = BytesIO()
+            woff.save(buffer)
+            data = b64encode(buffer.getbuffer()).decode('ascii')
+            url = 'data:application/font-woff;charset=utf-8;base64,' + data
+            result.append(
+                f'<style>@font-face{{font-family:{font_family};font-weight:{font_weight};font-style:{font_style};src:url("{url}")format("woff");}}</style>'
+            )
+
+        # Select global style
+        result.append(
+            f'<style>text{{font-family:{font_family};font-weight:{font_weight};font-style:{font_style};}}</style>'
+        )
+
+        # Add background
+        # if self.background_color is not None: # Should always be True
+        result.append(
+            f'<rect width="100%" height="100%" style="fill:{self.background_color}"></rect>'
+        )
+
+        # Embed image, useful for debug purpose
+        if embed_image:
+            image = self.to_image()
+            data = BytesIO()
+            image.save(data, format='JPEG')
+            data = b64encode(data.getbuffer()).decode('ascii')
+            result.append(
+                f'<image width="100%" height="100%" href="data:image/jpg;base64,{data}"/>'
+            )
+
+        # For each word in layout
+        for (word, _), font_size, (y, x), orientation, color in self.layout_:
+            x *= self.scale
+            y *= self.scale
+
+            # Get text metrics
+            font = ImageFont.truetype(self.font_path, int(font_size * self.scale))
+            (size_x, _), (offset_x, offset_y) = font.font.getsize(word)
+            ascent, _ = font.getmetrics()
+
+            # Compute text bounding box
+            min_x = -offset_x
+            max_x = size_x - offset_x
+            max_y = ascent - offset_y
+
+            # Compute text attributes
+            if orientation == Image.ROTATE_90:
+                x += max_y
+                y += max_x - min_x
+                transform = f'translate({x},{y}) rotate(-90)'
+            else:
+                x += min_x
+                y += max_y
+                transform = f'translate({x},{y})'
+
+            # Create node
+            result.append(
+                f'<text transform="{transform}" font-size="{font_size * self.scale}" style="fill:{color}">{saxutils.escape(word)}</text>'
+            )
+
+        # Complete SVG file
+        result.append('</svg>')
+        return '\n'.join(result)
```

