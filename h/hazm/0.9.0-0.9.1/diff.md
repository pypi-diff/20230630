# Comparing `tmp/hazm-0.9.0.tar.gz` & `tmp/hazm-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazm-0.9.0.tar", max compression
+gzip compressed data, was "hazm-0.9.1.tar", max compression
```

## Comparing `hazm-0.9.0.tar` & `hazm-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1083 2023-05-20 15:46:10.182773 hazm-0.9.0/LICENSE
--rw-r--r--   0        0        0     4452 2023-05-20 15:46:10.182773 hazm-0.9.0/README.md
--rw-r--r--   0        0        0     2480 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/__init__.py
--rwxr-xr-x   0        0        0    11943 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/chunker.py
--rw-r--r--   0        0        0      586 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/__init__.py
--rw-r--r--   0        0        0     4470 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/bijankhan_reader.py
--rw-r--r--   0        0        0    16979 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/dadegan_reader.py
--rw-r--r--   0        0        0     6360 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/degarbayan_reader.py
--rw-r--r--   0        0        0     6136 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/hamshahri_reader.py
--rw-r--r--   0        0        0     1858 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/mirastext_reader.py
--rw-r--r--   0        0        0     1267 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/persian_plain_text_reader.py
--rw-r--r--   0        0        0     3332 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/persica_reader.py
--rw-r--r--   0        0        0    11630 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/peykare_reader.py
--rw-r--r--   0        0        0     4392 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/quran_reader.py
--rw-r--r--   0        0        0     4731 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/sentipers_reader.py
--rw-r--r--   0        0        0     4609 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/tnews_reader.py
--rw-r--r--   0        0        0    14539 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/treebank_reader.py
--rw-r--r--   0        0        0     2733 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/verbvalency_reader.py
--rw-r--r--   0        0        0    64232 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/wiki_extractor.py
--rw-r--r--   0        0        0     3481 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/wikipedia_reader.py
--rw-r--r--   0        0        0      656 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/data/iverbs.dat
--rw-r--r--   0        0        0     5172 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/data/iwords.dat
--rw-r--r--   0        0        0     3664 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/data/stopwords.dat
--rw-r--r--   0        0        0     8328 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/data/verbs.dat
--rw-r--r--   0        0        0  1335405 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/data/words.dat
--rw-r--r--   0        0        0     8559 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/dependency_parser.py
--rw-r--r--   0        0        0    15568 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/embedding.py
--rw-r--r--   0        0        0    36078 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/informal_normalizer.py
--rw-r--r--   0        0        0   107981 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/lemmatizer.py
--rw-r--r--   0        0        0    24507 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/normalizer.py
--rw-r--r--   0        0        0    10011 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/pos_tagger.py
--rw-r--r--   0        0        0     1348 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/sentence_tokenizer.py
--rw-r--r--   0        0        0    17158 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/sequence_tagger.py
--rw-r--r--   0        0        0     2495 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/stemmer.py
--rw-r--r--   0        0        0     2593 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/token_splitter.py
--rw-r--r--   0        0        0     3027 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/utils.py
--rw-r--r--   0        0        0    13819 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/word_tokenizer.py
--rw-r--r--   0        0        0     4160 2023-05-20 15:46:10.258774 hazm-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 hazm-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2556 2023-06-29 06:34:44.278743 hazm-0.9.1/hazm/__init__.py
+-rw-r--r--   0        0        0    12199 2023-06-29 06:34:44.278743 hazm-0.9.1/hazm/chunker.py
+-rw-r--r--   0        0        0      600 2023-06-29 06:34:44.279745 hazm-0.9.1/hazm/corpus_readers/__init__.py
+-rw-r--r--   0        0        0     4603 2023-06-29 06:34:44.280743 hazm-0.9.1/hazm/corpus_readers/bijankhan_reader.py
+-rw-r--r--   0        0        0    17393 2023-06-29 06:34:44.281745 hazm-0.9.1/hazm/corpus_readers/dadegan_reader.py
+-rw-r--r--   0        0        0     6504 2023-06-29 06:34:44.281745 hazm-0.9.1/hazm/corpus_readers/degarbayan_reader.py
+-rw-r--r--   0        0        0     6302 2023-06-29 06:34:44.282742 hazm-0.9.1/hazm/corpus_readers/hamshahri_reader.py
+-rw-r--r--   0        0        0     1910 2023-05-19 17:02:23.654234 hazm-0.9.1/hazm/corpus_readers/mirastext_reader.py
+-rw-r--r--   0        0        0     1307 2023-05-20 09:29:17.536041 hazm-0.9.1/hazm/corpus_readers/persian_plain_text_reader.py
+-rw-r--r--   0        0        0     3419 2023-05-19 17:02:23.657234 hazm-0.9.1/hazm/corpus_readers/persica_reader.py
+-rw-r--r--   0        0        0    11969 2023-06-29 06:34:44.282742 hazm-0.9.1/hazm/corpus_readers/peykare_reader.py
+-rw-r--r--   0        0        0     4495 2023-06-29 06:34:44.283743 hazm-0.9.1/hazm/corpus_readers/quran_reader.py
+-rw-r--r--   0        0        0     4861 2023-06-29 06:34:44.283743 hazm-0.9.1/hazm/corpus_readers/sentipers_reader.py
+-rw-r--r--   0        0        0     4731 2023-05-19 17:02:23.659233 hazm-0.9.1/hazm/corpus_readers/tnews_reader.py
+-rw-r--r--   0        0        0    14949 2023-06-29 06:34:44.284743 hazm-0.9.1/hazm/corpus_readers/treebank_reader.py
+-rw-r--r--   0        0        0     2799 2023-05-19 17:02:23.653233 hazm-0.9.1/hazm/corpus_readers/verbvalency_reader.py
+-rw-r--r--   0        0        0    66091 2023-05-20 08:47:35.344846 hazm-0.9.1/hazm/corpus_readers/wiki_extractor.py
+-rw-r--r--   0        0        0     3579 2023-05-19 17:02:23.651232 hazm-0.9.1/hazm/corpus_readers/wikipedia_reader.py
+-rw-r--r--   0        0        0      682 2023-06-29 06:34:30.160053 hazm-0.9.1/hazm/data/iverbs.dat
+-rw-r--r--   0        0        0     5415 2023-06-29 06:34:30.161054 hazm-0.9.1/hazm/data/iwords.dat
+-rw-r--r--   0        0        0     4053 2023-04-21 06:10:37.576573 hazm-0.9.1/hazm/data/stopwords.dat
+-rw-r--r--   0        0        0     3259 2023-06-29 07:11:56.484742 hazm-0.9.1/hazm/data/verbs.dat
+-rw-r--r--   0        0        0   886268 2023-06-29 06:40:36.368810 hazm-0.9.1/hazm/data/words.dat
+-rw-r--r--   0        0        0     8805 2023-06-29 06:34:44.285743 hazm-0.9.1/hazm/dependency_parser.py
+-rw-r--r--   0        0        0    15980 2023-06-29 06:34:44.286745 hazm-0.9.1/hazm/embedding.py
+-rw-r--r--   0        0        0    36919 2023-06-29 07:20:53.180758 hazm-0.9.1/hazm/informal_normalizer.py
+-rw-r--r--   0        0        0   110303 2023-06-29 06:34:44.287745 hazm-0.9.1/hazm/lemmatizer.py
+-rw-r--r--   0        0        0    25042 2023-06-29 06:34:44.288745 hazm-0.9.1/hazm/normalizer.py
+-rw-r--r--   0        0        0    10216 2023-06-29 06:34:44.289742 hazm-0.9.1/hazm/pos_tagger.py
+-rw-r--r--   0        0        0     1388 2023-05-19 10:59:52.643719 hazm-0.9.1/hazm/sentence_tokenizer.py
+-rw-r--r--   0        0        0    17569 2023-05-24 17:29:45.481776 hazm-0.9.1/hazm/sequence_tagger.py
+-rw-r--r--   0        0        0     2570 2023-05-24 10:34:28.735473 hazm-0.9.1/hazm/stemmer.py
+-rw-r--r--   0        0        0     2659 2023-05-20 09:04:50.521923 hazm-0.9.1/hazm/token_splitter.py
+-rw-r--r--   0        0        0     3133 2023-05-20 09:38:21.938503 hazm-0.9.1/hazm/utils.py
+-rw-r--r--   0        0        0    14149 2023-05-20 09:01:45.137870 hazm-0.9.1/hazm/word_tokenizer.py
+-rw-r--r--   0        0        0     1103 2023-05-05 07:10:08.350612 hazm-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4261 2023-06-29 07:35:28.487269 hazm-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4558 2023-06-29 06:34:44.270745 hazm-0.9.1/README.md
+-rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 hazm-0.9.1/PKG-INFO
```

### Comparing `hazm-0.9.0/LICENSE` & `hazm-0.9.1/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-
-Copyright (c) 2013 Alireza Nourian
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2013 Alireza Nourian
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `hazm-0.9.0/README.md` & `hazm-0.9.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,279 +1,285 @@
-00000000: 2320 4861 7a6d 0a0a 215b 5465 7374 735d  # Hazm..![Tests]
-00000010: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000020: 656c 6473 2e69 6f2f 6769 7468 7562 2f61  elds.io/github/a
-00000030: 6374 696f 6e73 2f77 6f72 6b66 6c6f 772f  ctions/workflow/
-00000040: 7374 6174 7573 2f72 6f73 6861 6e2d 7265  status/roshan-re
-00000050: 7365 6172 6368 2f68 617a 6d2f 7465 7374  search/hazm/test
-00000060: 732e 796d 6c3f 6272 616e 6368 3d6d 6173  s.yml?branch=mas
-00000070: 7465 7229 0a21 5b50 7950 4920 2d20 446f  ter).![PyPI - Do
-00000080: 776e 6c6f 6164 735d 2868 7474 7073 3a2f  wnloads](https:/
-00000090: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000000a0: 6769 7468 7562 2f64 6f77 6e6c 6f61 6473  github/downloads
-000000b0: 2f72 6f73 6861 6e2d 7265 7365 6172 6368  /roshan-research
-000000c0: 2f68 617a 6d2f 746f 7461 6c29 0a21 5b47  /hazm/total).![G
-000000d0: 6974 4875 625d 2868 7474 7073 3a2f 2f69  itHub](https://i
-000000e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-000000f0: 7468 7562 2f6c 6963 656e 7365 2f72 6f73  thub/license/ros
-00000100: 6861 6e2d 7265 7365 6172 6368 2f68 617a  han-research/haz
-00000110: 6d29 0a0a 5079 7468 6f6e 206c 6962 7261  m)..Python libra
-00000120: 7279 2066 6f72 2064 6967 6573 7469 6e67  ry for digesting
-00000130: 2050 6572 7369 616e 2074 6578 742e 0a0a   Persian text...
-00000140: 2d20 5465 7874 2063 6c65 616e 696e 670a  - Text cleaning.
-00000150: 2d20 5365 6e74 656e 6365 2061 6e64 2077  - Sentence and w
-00000160: 6f72 6420 746f 6b65 6e69 7a65 720a 2d20  ord tokenizer.- 
-00000170: 576f 7264 206c 656d 6d61 7469 7a65 720a  Word lemmatizer.
-00000180: 2d20 504f 5320 7461 6767 6572 0a2d 2053  - POS tagger.- S
-00000190: 6861 6c6c 6f77 2070 6172 7365 720a 2d20  hallow parser.- 
-000001a0: 4465 7065 6e64 656e 6379 2070 6172 7365  Dependency parse
-000001b0: 720a 2d20 496e 7465 7266 6163 6573 2066  r.- Interfaces f
-000001c0: 6f72 2050 6572 7369 616e 2063 6f72 706f  or Persian corpo
-000001d0: 7261 0a2d 205b 4e4c 544b 5d28 6874 7470  ra.- [NLTK](http
-000001e0: 3a2f 2f6e 6c74 6b2e 6f72 672f 2920 636f  ://nltk.org/) co
-000001f0: 6d70 6174 6962 6c65 0a2d 2050 7974 686f  mpatible.- Pytho
-00000200: 6e20 332e 382c 2033 2e39 2c20 332e 3130  n 3.8, 3.9, 3.10
-00000210: 2061 6e64 2033 2e31 3120 7375 7070 6f72   and 3.11 suppor
-00000220: 740a 0a23 2320 446f 6375 6d65 6e74 6174  t..## Documentat
-00000230: 696f 6e0a 0a56 6973 6974 2068 7474 7073  ion..Visit https
-00000240: 3a2f 2f72 6f73 6861 6e2d 6169 2e69 722f  ://roshan-ai.ir/
-00000250: 6861 7a6d 2f64 6f63 7320 746f 2076 6965  hazm/docs to vie
-00000260: 7720 7468 6520 6675 6c6c 2064 6f63 756d  w the full docum
-00000270: 656e 7461 7469 6f6e 2e0a 0a23 2320 4d6f  entation...## Mo
-00000280: 6475 6c65 7320 6163 6375 7261 6379 0a0a  dules accuracy..
-00000290: 7c20 2a2a 4d6f 6475 6c65 206e 616d 652a  | **Module name*
-000002a0: 2a20 2020 2020 2020 2020 207c 202a 2a61  *          | **a
-000002b0: 6363 7572 6163 792a 2a20 7c20 207c 0a7c  ccuracy** |  |.|
-000002c0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-000002d0: 2d2d 2d2d 2d2d 2d2d 2d20 7c3a 2d2d 2d2d  --------- |:----
-000002e0: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
-000002f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
-00000300: 7c0a 7c20 2a2a 4c65 6d6d 6174 697a 6572  |.| **Lemmatizer
-00000310: 2a2a 2020 2020 2020 2020 2020 207c 2038  **           | 8
-00000320: 392e 3925 2020 2020 2020 2020 7c20 2020  9.9%        |   
-00000330: 2020 2020 2020 2020 2020 207c 0a7c 202a             |.| *
-00000340: 2a43 6875 6e6b 6572 2a2a 2020 2020 2020  *Chunker**      
-00000350: 2020 2020 2020 2020 7c20 3933 2e34 2520          | 93.4% 
-00000360: 2020 2020 2020 207c 205b 646f 776e 6c6f         | [downlo
-00000370: 6164 2070 7265 2d74 7261 696e 6564 206d  ad pre-trained m
-00000380: 6f64 656c 5d28 6874 7470 733a 2f2f 6472  odel](https://dr
-00000390: 6976 652e 676f 6f67 6c65 2e63 6f6d 2f66  ive.google.com/f
-000003a0: 696c 652f 642f 3177 6442 796b 304c 4842  ile/d/1wdByk0LHB
-000003b0: 5a69 7a6a 6255 7164 4478 6544 4235 4159  ZizjbUqdDxeDB5AY
-000003c0: 4945 6a6e 3449 4b29 2020 2020 2020 2020  IEjn4IK)        
-000003d0: 2020 2020 207c 0a7c 202a 2a50 4f53 5461       |.| **POSTa
-000003e0: 6767 6572 2a2a 2020 2020 2020 2020 2020  gger**          
-000003f0: 2020 7c20 3937 2e32 2520 2020 2020 2020    | 97.2%       
-00000400: 207c 2064 6f77 6e6c 6f61 6420 7072 652d   | download pre-
-00000410: 7472 6169 6e65 6420 6d6f 6465 6c20 2020  trained model   
-00000420: 2020 2020 2020 2020 2020 7c0a 7c20 2a2a            |.| **
-00000430: 504f 5354 6167 6765 7228 556e 6976 6572  POSTagger(Univer
-00000440: 7361 6c29 2a2a 207c 2039 382e 3825 2020  sal)** | 98.8%  
-00000450: 2020 2020 2020 7c20 5b64 6f77 6e6c 6f61        | [downloa
-00000460: 6420 7072 652d 7472 6169 6e65 6420 6d6f  d pre-trained mo
-00000470: 6465 6c5d 2868 7474 7073 3a2f 2f64 7269  del](https://dri
-00000480: 7665 2e67 6f6f 676c 652e 636f 6d2f 6669  ve.google.com/fi
-00000490: 6c65 2f64 2f31 696d 376c 4848 4877 6b37  le/d/1im7lHHHwk7
-000004a0: 6279 424a 4867 6678 7468 7577 5931 2d51  byBJHgfxthuwY1-Q
-000004b0: 4539 3846 4b43 2920 2020 2020 2020 2020  E98FKC)         
-000004c0: 2020 2020 7c0a 7c20 2a2a 4465 7065 6e64      |.| **Depend
-000004d0: 656e 6379 5061 7273 6572 2a2a 2020 2020  encyParser**    
-000004e0: 207c 2039 372e 3125 2020 2020 2020 2020   | 97.1%        
-000004f0: 7c20 5b64 6f77 6e6c 6f61 6420 7072 652d  | [download pre-
-00000500: 7472 6169 6e65 6420 6d6f 6465 6c5d 2868  trained model](h
-00000510: 7474 7073 3a2f 2f64 7269 7665 2e67 6f6f  ttps://drive.goo
-00000520: 676c 652e 636f 6d2f 6669 6c65 2f64 2f31  gle.com/file/d/1
-00000530: 7441 7936 6256 3537 5a58 4743 5263 7871  tAy6bV57ZXGCRcxq
-00000540: 7a4d 4263 7348 656a 7237 3872 524d 3938  zMBcsHejr78rRM98
-00000550: 2920 2020 2020 2020 2020 2020 2020 7c0a  )             |.
-00000560: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-00000570: 6e0a 0a54 6865 206c 6174 6573 7420 7374  n..The latest st
-00000580: 6162 6c65 2076 6572 7369 6f6e 206f 6620  able version of 
-00000590: 4861 7a6d 2063 616e 2062 6520 696e 7374  Hazm can be inst
-000005a0: 616c 6c65 6420 7468 726f 7567 6820 6070  alled through `p
-000005b0: 6970 603a 0a0a 2020 2020 7069 7020 696e  ip`:..    pip in
-000005c0: 7374 616c 6c20 6861 7a6d 0a0a 4275 7420  stall hazm..But 
-000005d0: 666f 7220 7465 7374 696e 6720 6f72 2075  for testing or u
-000005e0: 7369 6e67 2048 617a 6d20 7769 7468 2074  sing Hazm with t
-000005f0: 6865 206c 6174 6573 7420 7570 6461 7465  he latest update
-00000600: 7320 796f 7520 6d61 7920 7573 653a 0a0a  s you may use:..
-00000610: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
-00000620: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000630: 6f6d 2f72 6f73 6861 6e2d 7265 7365 6172  om/roshan-resear
-00000640: 6368 2f68 617a 6d2f 6172 6368 6976 652f  ch/hazm/archive/
-00000650: 6d61 7374 6572 2e7a 6970 202d 2d75 7067  master.zip --upg
-00000660: 7261 6465 0a0a 0a23 2320 5573 6167 650a  rade...## Usage.
-00000670: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2066  .```python.>>> f
-00000680: 726f 6d20 6861 7a6d 2069 6d70 6f72 7420  rom hazm import 
-00000690: 2a0a 0a3e 3e3e 206e 6f72 6d61 6c69 7a65  *..>>> normalize
-000006a0: 7220 3d20 4e6f 726d 616c 697a 6572 2829  r = Normalizer()
-000006b0: 0a3e 3e3e 206e 6f72 6d61 6c69 7a65 722e  .>>> normalizer.
-000006c0: 6e6f 726d 616c 697a 6528 27d8 a7d8 b5d9  normalize('.....
-000006d0: 84d8 a7d8 ad20 d986 d988 d98a d8b3 d987  ..... ..........
-000006e0: 20d9 87d8 a720 d988 20d8 a7d8 b3d8 aad9   .... .. .......
-000006f0: 81d8 a7d8 afd9 8720 d8a7 d8b2 20d9 86db  ....... .... ...
-00000700: 8cd9 85e2 808c d981 d8a7 d8b5 d984 d987  ................
-00000710: 20d9 bed8 b1d8 afd8 a7d8 b2d8 b420 d8b1   ............ ..
-00000720: d8a7 20d8 a2d8 b3d8 a7d9 8620 d985 d98a  .. ........ ....
-00000730: 20d9 83d9 86d8 af27 290a 27d8 a7d8 b5d9   ......').'.....
-00000740: 84d8 a7d8 ad20 d986 d988 db8c d8b3 d987  ..... ..........
-00000750: e280 8cd9 87d8 a720 d988 20d8 a7d8 b3d8  ....... .. .....
-00000760: aad9 81d8 a7d8 afd9 8720 d8a7 d8b2 20d9  ......... .... .
-00000770: 86db 8cd9 85e2 808c d981 d8a7 d8b5 d984  ................
-00000780: d987 20d9 bed8 b1d8 afd8 a7d8 b2d8 b420  .. ............ 
-00000790: d8b1 d8a7 20d8 a2d8 b3d8 a7d9 8620 d985  .... ........ ..
-000007a0: db8c e280 8cda a9d9 86d8 af27 0a0a 3e3e  ...........'..>>
-000007b0: 3e20 7365 6e74 5f74 6f6b 656e 697a 6528  > sent_tokenize(
-000007c0: 27d9 85d8 a720 d987 d985 20d8 a8d8 b1d8  '.... .... .....
-000007d0: a7db 8c20 d988 d8b5 d984 20da a9d8 b1d8  ... ...... .....
-000007e0: afd9 8620 d8a2 d985 d8af db8c d985 2120  ... ..........! 
-000007f0: d988 d984 db8c 20d8 a8d8 b1d8 a7db 8c20  ...... ........ 
-00000800: d9be d8b1 d8af d8a7 d8b2 d8b4 d88c 20d8  .............. .
-00000810: acd8 afd8 a720 d8a8 d987 d8aa d8b1 20d9  ..... ........ .
-00000820: 86db 8cd8 b3d8 aad8 9f27 290a 5b27 d985  .........').['..
-00000830: d8a7 20d9 87d9 8520 d8a8 d8b1 d8a7 db8c  .. .... ........
-00000840: 20d9 88d8 b5d9 8420 daa9 d8b1 d8af d986   ...... ........
-00000850: 20d8 a2d9 85d8 afdb 8cd9 8521 272c 2027   ..........!', '
-00000860: d988 d984 db8c 20d8 a8d8 b1d8 a7db 8c20  ...... ........ 
-00000870: d9be d8b1 d8af d8a7 d8b2 d8b4 d88c 20d8  .............. .
-00000880: acd8 afd8 a720 d8a8 d987 d8aa d8b1 20d9  ..... ........ .
-00000890: 86db 8cd8 b3d8 aad8 9f27 5d0a 3e3e 3e20  .........'].>>> 
-000008a0: 776f 7264 5f74 6f6b 656e 697a 6528 27d9  word_tokenize('.
-000008b0: 88d9 84db 8c20 d8a8 d8b1 d8a7 db8c 20d9  ..... ........ .
-000008c0: bed8 b1d8 afd8 a7d8 b2d8 b4d8 8c20 d8ac  ............. ..
-000008d0: d8af d8a7 20d8 a8d9 87d8 aad8 b120 d986  .... ........ ..
-000008e0: db8c d8b3 d8aa d89f 2729 0a5b 27d9 88d9  ........').['...
-000008f0: 84db 8c27 2c20 27d8 a8d8 b1d8 a7db 8c27  ...', '........'
-00000900: 2c20 27d9 bed8 b1d8 afd8 a7d8 b2d8 b427  , '............'
-00000910: 2c20 27d8 8c27 2c20 27d8 acd8 afd8 a727  , '..', '......'
-00000920: 2c20 27d8 a8d9 87d8 aad8 b127 2c20 27d9  , '........', '.
-00000930: 86db 8cd8 b3d8 aa27 2c20 27d8 9f27 5d0a  .......', '..'].
-00000940: 0a3e 3e3e 2073 7465 6d6d 6572 203d 2053  .>>> stemmer = S
-00000950: 7465 6d6d 6572 2829 0a3e 3e3e 2073 7465  temmer().>>> ste
-00000960: 6d6d 6572 2e73 7465 6d28 27da a9d8 aad8  mmer.stem('.....
-00000970: a7d8 a8e2 808c d987 d8a7 2729 0a27 daa9  ..........').'..
-00000980: d8aa d8a7 d8a8 270a 3e3e 3e20 6c65 6d6d  ......'.>>> lemm
-00000990: 6174 697a 6572 203d 204c 656d 6d61 7469  atizer = Lemmati
-000009a0: 7a65 7228 290a 3e3e 3e20 6c65 6d6d 6174  zer().>>> lemmat
-000009b0: 697a 6572 2e6c 656d 6d61 7469 7a65 2827  izer.lemmatize('
-000009c0: d985 db8c e280 8cd8 b1d9 88d9 8527 290a  .............').
-000009d0: 27d8 b1d9 81d8 aa23 d8b1 d988 270a 0a3e  '......#....'..>
-000009e0: 3e3e 2074 6167 6765 7220 3d20 504f 5354  >> tagger = POST
-000009f0: 6167 6765 7228 6d6f 6465 6c3d 2772 6573  agger(model='res
-00000a00: 6f75 7263 6573 2f70 6f73 5f74 6167 6765  ources/pos_tagge
-00000a10: 722e 6d6f 6465 6c27 290a 3e3e 3e20 7461  r.model').>>> ta
-00000a20: 6767 6572 2e74 6167 2877 6f72 645f 746f  gger.tag(word_to
-00000a30: 6b65 6e69 7a65 2827 d985 d8a7 20d8 a8d8  kenize('.... ...
-00000a40: b3db 8cd8 a7d8 b120 daa9 d8aa d8a7 d8a8  ....... ........
-00000a50: 20d9 85db 8ce2 808c d8ae d988 d8a7 d986   ...............
-00000a60: db8c d985 2729 290a 5b28 27d9 85d8 a727  ....')).[('....'
-00000a70: 2c20 2750 524f 2729 2c20 2827 d8a8 d8b3  , 'PRO'), ('....
-00000a80: db8c d8a7 d8b1 272c 2027 4144 5627 292c  ......', 'ADV'),
-00000a90: 2028 27da a9d8 aad8 a7d8 a827 2c20 274e   ('........', 'N
-00000aa0: 2729 2c20 2827 d985 db8c e280 8cd8 aed9  '), ('..........
-00000ab0: 88d8 a7d9 86db 8cd9 8527 2c20 2756 2729  .........', 'V')
-00000ac0: 5d0a 0a3e 3e3e 2063 6875 6e6b 6572 203d  ]..>>> chunker =
-00000ad0: 2043 6875 6e6b 6572 286d 6f64 656c 3d27   Chunker(model='
-00000ae0: 7265 736f 7572 6365 732f 6368 756e 6b65  resources/chunke
-00000af0: 722e 6d6f 6465 6c27 290a 3e3e 3e20 7461  r.model').>>> ta
-00000b00: 6767 6564 203d 2074 6167 6765 722e 7461  gged = tagger.ta
-00000b10: 6728 776f 7264 5f74 6f6b 656e 697a 6528  g(word_tokenize(
-00000b20: 27da a9d8 aad8 a7d8 a820 d8ae d988 d8a7  '........ ......
-00000b30: d986 d8af d986 20d8 b1d8 a720 d8af d988  ...... .... ....
-00000b40: d8b3 d8aa 20d8 afd8 a7d8 b1db 8cd9 8527  .... ..........'
-00000b50: 2929 0a3e 3e3e 2074 7265 6532 6272 6163  )).>>> tree2brac
-00000b60: 6b65 7473 2863 6875 6e6b 6572 2e70 6172  kets(chunker.par
-00000b70: 7365 2874 6167 6765 6429 290a 275b daa9  se(tagged)).'[..
-00000b80: d8aa d8a7 d8a8 20d8 aed9 88d8 a7d9 86d8  ...... .........
-00000b90: afd9 8620 4e50 5d20 5bd8 b1d8 a720 504f  ... NP] [.... PO
-00000ba0: 5354 505d 205b d8af d988 d8b3 d8aa 20d8  STP] [........ .
-00000bb0: afd8 a7d8 b1db 8cd9 8520 5650 5d27 0a0a  ......... VP]'..
-00000bc0: 3e3e 3e20 7061 7273 6572 203d 2044 6570  >>> parser = Dep
-00000bd0: 656e 6465 6e63 7950 6172 7365 7228 7461  endencyParser(ta
-00000be0: 6767 6572 3d74 6167 6765 722c 206c 656d  gger=tagger, lem
-00000bf0: 6d61 7469 7a65 723d 6c65 6d6d 6174 697a  matizer=lemmatiz
-00000c00: 6572 290a 3e3e 3e20 7061 7273 6572 2e70  er).>>> parser.p
-00000c10: 6172 7365 2877 6f72 645f 746f 6b65 6e69  arse(word_tokeni
-00000c20: 7a65 2827 d8b2 d986 daaf e280 8cd9 87d8  ze('............
-00000c30: a720 d8a8 d8b1 d8a7 db8c 20da a9d9 8720  . ........ .... 
-00000c40: d8a8 d987 20d8 b5d8 afd8 a720 d8af d8b1  .... ...... ....
-00000c50: d985 db8c e280 8cd8 a2db 8cd8 afd8 9f27  ...............'
-00000c60: 2929 0a3c 4465 7065 6e64 656e 6379 4772  )).<DependencyGr
-00000c70: 6170 6820 7769 7468 2038 206e 6f64 6573  aph with 8 nodes
-00000c80: 3e0a 0a60 6060 0a0a 2323 2045 7874 656e  >..```..## Exten
-00000c90: 7369 6f6e 730a 0a4e 6f74 653a 2054 6865  sions..Note: The
-00000ca0: 7365 2061 7265 206e 6f74 206f 6666 6963  se are not offic
-00000cb0: 6961 6c20 7665 7273 696f 6e73 206f 6620  ial versions of 
-00000cc0: 6861 7a6d 2c20 6e6f 7420 7570 746f 6461  hazm, not uptoda
-00000cd0: 7465 206f 6e20 6675 6e63 7469 6f6e 616c  te on functional
-00000ce0: 6974 7920 616e 6420 6172 6520 6e6f 7420  ity and are not 
-00000cf0: 7375 7070 6f72 7465 6420 6279 2052 6f73  supported by Ros
-00000d00: 6861 6e2e 0a0a 2d20 5b2a 2a4a 4861 7a6d  han...- [**JHazm
-00000d10: 2a2a 5d28 6874 7470 733a 2f2f 6769 7468  **](https://gith
-00000d20: 7562 2e63 6f6d 2f6d 6f6a 7461 6261 2d6b  ub.com/mojtaba-k
-00000d30: 6861 6c6c 6173 682f 4a48 617a 6d29 3a20  hallash/JHazm): 
-00000d40: 4120 4a61 7661 2070 6f72 7420 6f66 2048  A Java port of H
-00000d50: 617a 6d0a 2d20 5b2a 2a4e 4861 7a6d 2a2a  azm.- [**NHazm**
-00000d60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000d70: 2e63 6f6d 2f6d 6f6a 7461 6261 2d6b 6861  .com/mojtaba-kha
-00000d80: 6c6c 6173 682f 4e48 617a 6d29 3a20 4120  llash/NHazm): A 
-00000d90: 4323 2070 6f72 7420 6f66 2048 617a 6d0a  C# port of Hazm.
-00000da0: 0a23 2320 436f 6e74 7269 6275 7469 6f6e  .## Contribution
-00000db0: 0a0a 5765 2077 656c 636f 6d65 2061 6e64  ..We welcome and
-00000dc0: 2061 7070 7265 6369 6174 6520 616e 7920   appreciate any 
-00000dd0: 636f 6e74 7269 6275 7469 6f6e 7320 746f  contributions to
-00000de0: 2074 6869 7320 7265 706f 2c20 7375 6368   this repo, such
-00000df0: 2061 7320 6275 6720 7265 706f 7274 732c   as bug reports,
-00000e00: 2066 6561 7475 7265 2072 6571 7565 7374   feature request
-00000e10: 732c 2063 6f64 6520 696d 7072 6f76 656d  s, code improvem
-00000e20: 656e 7473 2c20 646f 6375 6d65 6e74 6174  ents, documentat
-00000e30: 696f 6e20 7570 6461 7465 732c 2065 7463  ion updates, etc
-00000e40: 2e20 506c 6561 7365 2066 6f6c 6c6f 7720  . Please follow 
-00000e50: 7468 6520 5b43 6f6e 7472 6962 7574 696f  the [Contributio
-00000e60: 6e20 6775 6964 656c 696e 655d 282e 2f43  n guideline](./C
-00000e70: 4f4e 5452 4942 5554 494f 4e2e 6d64 2920  ONTRIBUTION.md) 
-00000e80: 7768 656e 2063 6f6e 7472 6962 7574 696e  when contributin
-00000e90: 672e 2059 6f75 2063 616e 206f 7065 6e20  g. You can open 
-00000ea0: 616e 2069 7373 7565 2c20 666f 726b 2074  an issue, fork t
-00000eb0: 6865 2072 6570 6f2c 2077 7269 7465 2079  he repo, write y
-00000ec0: 6f75 7220 636f 6465 2c20 6372 6561 7465  our code, create
-00000ed0: 2061 2070 756c 6c20 7265 7175 6573 7420   a pull request 
-00000ee0: 616e 6420 7761 6974 2066 6f72 2061 2072  and wait for a r
-00000ef0: 6576 6965 7720 616e 6420 6665 6564 6261  eview and feedba
-00000f00: 636b 2e20 5468 616e 6b20 796f 7520 666f  ck. Thank you fo
-00000f10: 7220 796f 7572 2069 6e74 6572 6573 7420  r your interest 
-00000f20: 616e 6420 7375 7070 6f72 7420 696e 2074  and support in t
-00000f30: 6869 7320 7265 706f 210a 0a23 2320 5468  his repo!..## Th
-00000f40: 616e 6b73 0a0a 2323 2320 436f 6465 2063  anks..### Code c
-00000f50: 6f6e 7472 6962 7574 6f72 6573 0a0a 215b  ontributores..![
-00000f60: 416c 745d 2868 7474 7073 3a2f 2f72 6570  Alt](https://rep
-00000f70: 6f62 6561 7473 2e61 7869 6f6d 2e63 6f2f  obeats.axiom.co/
-00000f80: 6170 692f 656d 6265 642f 6165 3432 6264  api/embed/ae42bd
-00000f90: 6131 3538 3739 3136 3435 6431 3433 6333  a158791645d143c3
-00000fa0: 6533 6337 6631 3964 3861 3638 6430 3664  e3c7f19d8a68d06d
-00000fb0: 3038 2e73 7667 2022 5265 706f 6265 6174  08.svg "Repobeat
-00000fc0: 7320 616e 616c 7974 6963 7320 696d 6167  s analytics imag
-00000fd0: 6522 290a 0a3c 6120 6872 6566 3d22 6874  e")..<a href="ht
-00000fe0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ff0: 2f72 6f73 6861 6e2d 7265 7365 6172 6368  /roshan-research
-00001000: 2f68 617a 6d2f 6772 6170 6873 2f63 6f6e  /hazm/graphs/con
-00001010: 7472 6962 7574 6f72 7322 3e0a 2020 3c69  tributors">.  <i
-00001020: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001030: 636f 6e74 7269 622e 726f 636b 732f 696d  contrib.rocks/im
-00001040: 6167 653f 7265 706f 3d72 6f73 6861 6e2d  age?repo=roshan-
-00001050: 7265 7365 6172 6368 2f68 617a 6d22 202f  research/hazm" /
-00001060: 3e0a 3c2f 613e 0a0a 2323 2320 4f74 6865  >.</a>..### Othe
-00001070: 7273 0a0a 2d20 5468 616e 6b73 2074 6f20  rs..- Thanks to 
-00001080: 5b56 6972 6173 7479 6172 5d28 6874 7470  [Virastyar](http
-00001090: 3a2f 2f76 6972 6173 7479 6172 2e69 722f  ://virastyar.ir/
-000010a0: 2920 7072 6f6a 6563 7420 666f 7220 7072  ) project for pr
-000010b0: 6f76 6964 696e 6720 7468 6520 7065 7273  oviding the pers
-000010c0: 6961 6e20 776f 7264 206c 6973 742e 0a0a  ian word list...
-000010d0: 5b21 5b53 7461 7220 4869 7374 6f72 7920  [![Star History 
-000010e0: 4368 6172 745d 2868 7474 7073 3a2f 2f61  Chart](https://a
-000010f0: 7069 2e73 7461 722d 6869 7374 6f72 792e  pi.star-history.
-00001100: 636f 6d2f 7376 673f 7265 706f 733d 726f  com/svg?repos=ro
-00001110: 7368 616e 2d72 6573 6561 7263 682f 6861  shan-research/ha
-00001120: 7a6d 2674 7970 653d 4461 7465 295d 2868  zm&type=Date)](h
-00001130: 7474 7073 3a2f 2f73 7461 722d 6869 7374  ttps://star-hist
-00001140: 6f72 792e 636f 6d2f 2372 6f73 6861 6e2d  ory.com/#roshan-
-00001150: 7265 7365 6172 6368 2f68 617a 6d26 4461  research/hazm&Da
-00001160: 7465 290a                                te).
+00000000: 2320 4861 7a6d 0d0a 0d0a 215b 5465 7374  # Hazm....![Test
+00000010: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
+00000020: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00000030: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000040: 772f 7374 6174 7573 2f72 6f73 6861 6e2d  w/status/roshan-
+00000050: 7265 7365 6172 6368 2f68 617a 6d2f 7465  research/hazm/te
+00000060: 7374 732e 796d 6c3f 6272 616e 6368 3d6d  sts.yml?branch=m
+00000070: 6173 7465 7229 0d0a 215b 5079 5049 202d  aster)..![PyPI -
+00000080: 2044 6f77 6e6c 6f61 6473 5d28 6874 7470   Downloads](http
+00000090: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000000a0: 696f 2f67 6974 6875 622f 646f 776e 6c6f  io/github/downlo
+000000b0: 6164 732f 726f 7368 616e 2d72 6573 6561  ads/roshan-resea
+000000c0: 7263 682f 6861 7a6d 2f74 6f74 616c 290d  rch/hazm/total).
+000000d0: 0a21 5b47 6974 4875 625d 2868 7474 7073  .![GitHub](https
+000000e0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000000f0: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
+00000100: 2f72 6f73 6861 6e2d 7265 7365 6172 6368  /roshan-research
+00000110: 2f68 617a 6d29 0d0a 0d0a 5079 7468 6f6e  /hazm)....Python
+00000120: 206c 6962 7261 7279 2066 6f72 2064 6967   library for dig
+00000130: 6573 7469 6e67 2050 6572 7369 616e 2074  esting Persian t
+00000140: 6578 742e 0d0a 0d0a 2d20 5465 7874 2063  ext.....- Text c
+00000150: 6c65 616e 696e 670d 0a2d 2053 656e 7465  leaning..- Sente
+00000160: 6e63 6520 616e 6420 776f 7264 2074 6f6b  nce and word tok
+00000170: 656e 697a 6572 0d0a 2d20 576f 7264 206c  enizer..- Word l
+00000180: 656d 6d61 7469 7a65 720d 0a2d 2050 4f53  emmatizer..- POS
+00000190: 2074 6167 6765 720d 0a2d 2053 6861 6c6c   tagger..- Shall
+000001a0: 6f77 2070 6172 7365 720d 0a2d 2044 6570  ow parser..- Dep
+000001b0: 656e 6465 6e63 7920 7061 7273 6572 0d0a  endency parser..
+000001c0: 2d20 496e 7465 7266 6163 6573 2066 6f72  - Interfaces for
+000001d0: 2050 6572 7369 616e 2063 6f72 706f 7261   Persian corpora
+000001e0: 0d0a 2d20 5b4e 4c54 4b5d 2868 7474 703a  ..- [NLTK](http:
+000001f0: 2f2f 6e6c 746b 2e6f 7267 2f29 2063 6f6d  //nltk.org/) com
+00000200: 7061 7469 626c 650d 0a2d 2050 7974 686f  patible..- Pytho
+00000210: 6e20 332e 382c 2033 2e39 2c20 332e 3130  n 3.8, 3.9, 3.10
+00000220: 2061 6e64 2033 2e31 3120 7375 7070 6f72   and 3.11 suppor
+00000230: 740d 0a0d 0a23 2320 446f 6375 6d65 6e74  t....## Document
+00000240: 6174 696f 6e0d 0a0d 0a56 6973 6974 2068  ation....Visit h
+00000250: 7474 7073 3a2f 2f72 6f73 6861 6e2d 6169  ttps://roshan-ai
+00000260: 2e69 722f 6861 7a6d 2f64 6f63 7320 746f  .ir/hazm/docs to
+00000270: 2076 6965 7720 7468 6520 6675 6c6c 2064   view the full d
+00000280: 6f63 756d 656e 7461 7469 6f6e 2e0d 0a0d  ocumentation....
+00000290: 0a23 2320 4d6f 6475 6c65 7320 6163 6375  .## Modules accu
+000002a0: 7261 6379 0d0a 0d0a 7c20 2a2a 4d6f 6475  racy....| **Modu
+000002b0: 6c65 206e 616d 652a 2a20 2020 2020 2020  le name**       
+000002c0: 2020 207c 202a 2a61 6363 7572 6163 792a     | **accuracy*
+000002d0: 2a20 7c20 207c 0d0a 7c3a 2d2d 2d2d 2d2d  * |  |..|:------
+000002e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000002f0: 2d2d 207c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  -- |:-----------
+00000300: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
+00000310: 2d2d 2d2d 2d2d 2d2d 3a7c 0d0a 7c20 2a2a  --------:|..| **
+00000320: 4c65 6d6d 6174 697a 6572 2a2a 2020 2020  Lemmatizer**    
+00000330: 2020 2020 2020 207c 2038 392e 3925 2020         | 89.9%  
+00000340: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00000350: 2020 2020 207c 0d0a 7c20 2a2a 4368 756e       |..| **Chun
+00000360: 6b65 722a 2a20 2020 2020 2020 2020 2020  ker**           
+00000370: 2020 207c 2039 332e 3425 2020 2020 2020     | 93.4%      
+00000380: 2020 7c20 5b64 6f77 6e6c 6f61 6420 7072    | [download pr
+00000390: 652d 7472 6169 6e65 6420 6d6f 6465 6c5d  e-trained model]
+000003a0: 2868 7474 7073 3a2f 2f64 7269 7665 2e67  (https://drive.g
+000003b0: 6f6f 676c 652e 636f 6d2f 6669 6c65 2f64  oogle.com/file/d
+000003c0: 2f31 7764 4279 6b30 4c48 425a 697a 6a62  /1wdByk0LHBZizjb
+000003d0: 5571 6444 7865 4442 3541 5949 456a 6e34  UqdDxeDB5AYIEjn4
+000003e0: 494b 2920 2020 2020 2020 2020 2020 2020  IK)             
+000003f0: 7c0d 0a7c 202a 2a50 4f53 5461 6767 6572  |..| **POSTagger
+00000400: 2a2a 2020 2020 2020 2020 2020 2020 7c20  **            | 
+00000410: 3937 2e32 2520 2020 2020 2020 207c 2064  97.2%        | d
+00000420: 6f77 6e6c 6f61 6420 7072 652d 7472 6169  ownload pre-trai
+00000430: 6e65 6420 6d6f 6465 6c20 2020 2020 2020  ned model       
+00000440: 2020 2020 2020 7c0d 0a7c 202a 2a50 4f53        |..| **POS
+00000450: 5461 6767 6572 2855 6e69 7665 7273 616c  Tagger(Universal
+00000460: 292a 2a20 7c20 3938 2e38 2520 2020 2020  )** | 98.8%     
+00000470: 2020 207c 205b 646f 776e 6c6f 6164 2070     | [download p
+00000480: 7265 2d74 7261 696e 6564 206d 6f64 656c  re-trained model
+00000490: 5d28 6874 7470 733a 2f2f 6472 6976 652e  ](https://drive.
+000004a0: 676f 6f67 6c65 2e63 6f6d 2f66 696c 652f  google.com/file/
+000004b0: 642f 3169 6d37 6c48 4848 776b 3762 7942  d/1im7lHHHwk7byB
+000004c0: 4a48 6766 7874 6875 7759 312d 5145 3938  JHgfxthuwY1-QE98
+000004d0: 464b 4329 2020 2020 2020 2020 2020 2020  FKC)            
+000004e0: 207c 0d0a 7c20 2a2a 4465 7065 6e64 656e   |..| **Dependen
+000004f0: 6379 5061 7273 6572 2a2a 2020 2020 207c  cyParser**     |
+00000500: 2039 372e 3125 2020 2020 2020 2020 7c20   97.1%        | 
+00000510: 5b64 6f77 6e6c 6f61 6420 7072 652d 7472  [download pre-tr
+00000520: 6169 6e65 6420 6d6f 6465 6c5d 2868 7474  ained model](htt
+00000530: 7073 3a2f 2f64 7269 7665 2e67 6f6f 676c  ps://drive.googl
+00000540: 652e 636f 6d2f 6669 6c65 2f64 2f31 7441  e.com/file/d/1tA
+00000550: 7936 6256 3537 5a58 4743 5263 7871 7a4d  y6bV57ZXGCRcxqzM
+00000560: 4263 7348 656a 7237 3872 524d 3938 2920  BcsHejr78rRM98) 
+00000570: 2020 2020 2020 2020 2020 2020 7c0d 0a0d              |...
+00000580: 0a0d 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
+00000590: 6f6e 0d0a 0d0a 5468 6520 6c61 7465 7374  on....The latest
+000005a0: 2073 7461 626c 6520 7665 7273 696f 6e20   stable version 
+000005b0: 6f66 2048 617a 6d20 6361 6e20 6265 2069  of Hazm can be i
+000005c0: 6e73 7461 6c6c 6564 2074 6872 6f75 6768  nstalled through
+000005d0: 2060 7069 7060 3a0d 0a0d 0a20 2020 2070   `pip`:....    p
+000005e0: 6970 2069 6e73 7461 6c6c 2068 617a 6d0d  ip install hazm.
+000005f0: 0a0d 0a42 7574 2066 6f72 2074 6573 7469  ...But for testi
+00000600: 6e67 206f 7220 7573 696e 6720 4861 7a6d  ng or using Hazm
+00000610: 2077 6974 6820 7468 6520 6c61 7465 7374   with the latest
+00000620: 2075 7064 6174 6573 2079 6f75 206d 6179   updates you may
+00000630: 2075 7365 3a0d 0a0d 0a20 2020 2070 6970   use:....    pip
+00000640: 2069 6e73 7461 6c6c 2068 7474 7073 3a2f   install https:/
+00000650: 2f67 6974 6875 622e 636f 6d2f 726f 7368  /github.com/rosh
+00000660: 616e 2d72 6573 6561 7263 682f 6861 7a6d  an-research/hazm
+00000670: 2f61 7263 6869 7665 2f6d 6173 7465 722e  /archive/master.
+00000680: 7a69 7020 2d2d 7570 6772 6164 650d 0a0d  zip --upgrade...
+00000690: 0a0d 0a23 2320 5573 6167 650d 0a0d 0a60  ...## Usage....`
+000006a0: 6060 7079 7468 6f6e 0d0a 3e3e 3e20 6672  ``python..>>> fr
+000006b0: 6f6d 2068 617a 6d20 696d 706f 7274 202a  om hazm import *
+000006c0: 0d0a 0d0a 3e3e 3e20 6e6f 726d 616c 697a  ....>>> normaliz
+000006d0: 6572 203d 204e 6f72 6d61 6c69 7a65 7228  er = Normalizer(
+000006e0: 290d 0a3e 3e3e 206e 6f72 6d61 6c69 7a65  )..>>> normalize
+000006f0: 722e 6e6f 726d 616c 697a 6528 27d8 a7d8  r.normalize('...
+00000700: b5d9 84d8 a7d8 ad20 d986 d988 d98a d8b3  ....... ........
+00000710: d987 20d9 87d8 a720 d988 20d8 a7d8 b3d8  .. .... .. .....
+00000720: aad9 81d8 a7d8 afd9 8720 d8a7 d8b2 20d9  ......... .... .
+00000730: 86db 8cd9 85e2 808c d981 d8a7 d8b5 d984  ................
+00000740: d987 20d9 bed8 b1d8 afd8 a7d8 b2d8 b420  .. ............ 
+00000750: d8b1 d8a7 20d8 a2d8 b3d8 a7d9 8620 d985  .... ........ ..
+00000760: d98a 20d9 83d9 86d8 af27 290d 0a27 d8a7  .. ......')..'..
+00000770: d8b5 d984 d8a7 d8ad 20d9 86d9 88db 8cd8  ........ .......
+00000780: b3d9 87e2 808c d987 d8a7 20d9 8820 d8a7  .......... .. ..
+00000790: d8b3 d8aa d981 d8a7 d8af d987 20d8 a7d8  ............ ...
+000007a0: b220 d986 db8c d985 e280 8cd9 81d8 a7d8  . ..............
+000007b0: b5d9 84d9 8720 d9be d8b1 d8af d8a7 d8b2  ..... ..........
+000007c0: d8b4 20d8 b1d8 a720 d8a2 d8b3 d8a7 d986  .. .... ........
+000007d0: 20d9 85db 8ce2 808c daa9 d986 d8af 270d   .............'.
+000007e0: 0a0d 0a3e 3e3e 2073 656e 745f 746f 6b65  ...>>> sent_toke
+000007f0: 6e69 7a65 2827 d985 d8a7 20d9 87d9 8520  nize('.... .... 
+00000800: d8a8 d8b1 d8a7 db8c 20d9 88d8 b5d9 8420  ........ ...... 
+00000810: daa9 d8b1 d8af d986 20d8 a2d9 85d8 afdb  ........ .......
+00000820: 8cd9 8521 20d9 88d9 84db 8c20 d8a8 d8b1  ...! ...... ....
+00000830: d8a7 db8c 20d9 bed8 b1d8 afd8 a7d8 b2d8  .... ...........
+00000840: b4d8 8c20 d8ac d8af d8a7 20d8 a8d9 87d8  ... ...... .....
+00000850: aad8 b120 d986 db8c d8b3 d8aa d89f 2729  ... ..........')
+00000860: 0d0a 5b27 d985 d8a7 20d9 87d9 8520 d8a8  ..['.... .... ..
+00000870: d8b1 d8a7 db8c 20d9 88d8 b5d9 8420 daa9  ...... ...... ..
+00000880: d8b1 d8af d986 20d8 a2d9 85d8 afdb 8cd9  ...... .........
+00000890: 8521 272c 2027 d988 d984 db8c 20d8 a8d8  .!', '...... ...
+000008a0: b1d8 a7db 8c20 d9be d8b1 d8af d8a7 d8b2  ..... ..........
+000008b0: d8b4 d88c 20d8 acd8 afd8 a720 d8a8 d987  .... ...... ....
+000008c0: d8aa d8b1 20d9 86db 8cd8 b3d8 aad8 9f27  .... ..........'
+000008d0: 5d0d 0a3e 3e3e 2077 6f72 645f 746f 6b65  ]..>>> word_toke
+000008e0: 6e69 7a65 2827 d988 d984 db8c 20d8 a8d8  nize('...... ...
+000008f0: b1d8 a7db 8c20 d9be d8b1 d8af d8a7 d8b2  ..... ..........
+00000900: d8b4 d88c 20d8 acd8 afd8 a720 d8a8 d987  .... ...... ....
+00000910: d8aa d8b1 20d9 86db 8cd8 b3d8 aad8 9f27  .... ..........'
+00000920: 290d 0a5b 27d9 88d9 84db 8c27 2c20 27d8  )..['......', '.
+00000930: a8d8 b1d8 a7db 8c27 2c20 27d9 bed8 b1d8  .......', '.....
+00000940: afd8 a7d8 b2d8 b427 2c20 27d8 8c27 2c20  .......', '..', 
+00000950: 27d8 acd8 afd8 a727 2c20 27d8 a8d9 87d8  '......', '.....
+00000960: aad8 b127 2c20 27d9 86db 8cd8 b3d8 aa27  ...', '........'
+00000970: 2c20 27d8 9f27 5d0d 0a0d 0a3e 3e3e 2073  , '..']....>>> s
+00000980: 7465 6d6d 6572 203d 2053 7465 6d6d 6572  temmer = Stemmer
+00000990: 2829 0d0a 3e3e 3e20 7374 656d 6d65 722e  ()..>>> stemmer.
+000009a0: 7374 656d 2827 daa9 d8aa d8a7 d8a8 e280  stem('..........
+000009b0: 8cd9 87d8 a727 290d 0a27 daa9 d8aa d8a7  .....')..'......
+000009c0: d8a8 270d 0a3e 3e3e 206c 656d 6d61 7469  ..'..>>> lemmati
+000009d0: 7a65 7220 3d20 4c65 6d6d 6174 697a 6572  zer = Lemmatizer
+000009e0: 2829 0d0a 3e3e 3e20 6c65 6d6d 6174 697a  ()..>>> lemmatiz
+000009f0: 6572 2e6c 656d 6d61 7469 7a65 2827 d985  er.lemmatize('..
+00000a00: db8c e280 8cd8 b1d9 88d9 8527 290d 0a27  ...........')..'
+00000a10: d8b1 d981 d8aa 23d8 b1d9 8827 0d0a 0d0a  ......#....'....
+00000a20: 3e3e 3e20 7461 6767 6572 203d 2050 4f53  >>> tagger = POS
+00000a30: 5461 6767 6572 286d 6f64 656c 3d27 7265  Tagger(model='re
+00000a40: 736f 7572 6365 732f 706f 735f 7461 6767  sources/pos_tagg
+00000a50: 6572 2e6d 6f64 656c 2729 0d0a 3e3e 3e20  er.model')..>>> 
+00000a60: 7461 6767 6572 2e74 6167 2877 6f72 645f  tagger.tag(word_
+00000a70: 746f 6b65 6e69 7a65 2827 d985 d8a7 20d8  tokenize('.... .
+00000a80: a8d8 b3db 8cd8 a7d8 b120 daa9 d8aa d8a7  ......... ......
+00000a90: d8a8 20d9 85db 8ce2 808c d8ae d988 d8a7  .. .............
+00000aa0: d986 db8c d985 2729 290d 0a5b 2827 d985  ......'))..[('..
+00000ab0: d8a7 272c 2027 5052 4f27 292c 2028 27d8  ..', 'PRO'), ('.
+00000ac0: a8d8 b3db 8cd8 a7d8 b127 2c20 2741 4456  .........', 'ADV
+00000ad0: 2729 2c20 2827 daa9 d8aa d8a7 d8a8 272c  '), ('........',
+00000ae0: 2027 4e27 292c 2028 27d9 85db 8ce2 808c   'N'), ('.......
+00000af0: d8ae d988 d8a7 d986 db8c d985 272c 2027  ............', '
+00000b00: 5627 295d 0d0a 0d0a 3e3e 3e20 6368 756e  V')]....>>> chun
+00000b10: 6b65 7220 3d20 4368 756e 6b65 7228 6d6f  ker = Chunker(mo
+00000b20: 6465 6c3d 2772 6573 6f75 7263 6573 2f63  del='resources/c
+00000b30: 6875 6e6b 6572 2e6d 6f64 656c 2729 0d0a  hunker.model')..
+00000b40: 3e3e 3e20 7461 6767 6564 203d 2074 6167  >>> tagged = tag
+00000b50: 6765 722e 7461 6728 776f 7264 5f74 6f6b  ger.tag(word_tok
+00000b60: 656e 697a 6528 27da a9d8 aad8 a7d8 a820  enize('........ 
+00000b70: d8ae d988 d8a7 d986 d8af d986 20d8 b1d8  ............ ...
+00000b80: a720 d8af d988 d8b3 d8aa 20d8 afd8 a7d8  . ........ .....
+00000b90: b1db 8cd9 8527 2929 0d0a 3e3e 3e20 7472  .....'))..>>> tr
+00000ba0: 6565 3262 7261 636b 6574 7328 6368 756e  ee2brackets(chun
+00000bb0: 6b65 722e 7061 7273 6528 7461 6767 6564  ker.parse(tagged
+00000bc0: 2929 0d0a 275b daa9 d8aa d8a7 d8a8 20d8  ))..'[........ .
+00000bd0: aed9 88d8 a7d9 86d8 afd9 8620 4e50 5d20  ........... NP] 
+00000be0: 5bd8 b1d8 a720 504f 5354 505d 205b d8af  [.... POSTP] [..
+00000bf0: d988 d8b3 d8aa 20d8 afd8 a7d8 b1db 8cd9  ...... .........
+00000c00: 8520 5650 5d27 0d0a 0d0a 3e3e 3e20 7061  . VP]'....>>> pa
+00000c10: 7273 6572 203d 2044 6570 656e 6465 6e63  rser = Dependenc
+00000c20: 7950 6172 7365 7228 7461 6767 6572 3d74  yParser(tagger=t
+00000c30: 6167 6765 722c 206c 656d 6d61 7469 7a65  agger, lemmatize
+00000c40: 723d 6c65 6d6d 6174 697a 6572 290d 0a3e  r=lemmatizer)..>
+00000c50: 3e3e 2070 6172 7365 722e 7061 7273 6528  >> parser.parse(
+00000c60: 776f 7264 5f74 6f6b 656e 697a 6528 27d8  word_tokenize('.
+00000c70: b2d9 86da afe2 808c d987 d8a7 20d8 a8d8  ............ ...
+00000c80: b1d8 a7db 8c20 daa9 d987 20d8 a8d9 8720  ..... .... .... 
+00000c90: d8b5 d8af d8a7 20d8 afd8 b1d9 85db 8ce2  ...... .........
+00000ca0: 808c d8a2 db8c d8af d89f 2729 290d 0a3c  ..........'))..<
+00000cb0: 4465 7065 6e64 656e 6379 4772 6170 6820  DependencyGraph 
+00000cc0: 7769 7468 2038 206e 6f64 6573 3e0d 0a0d  with 8 nodes>...
+00000cd0: 0a60 6060 0d0a 0d0a 2323 2045 7874 656e  .```....## Exten
+00000ce0: 7369 6f6e 730d 0a0d 0a4e 6f74 653a 2054  sions....Note: T
+00000cf0: 6865 7365 2061 7265 206e 6f74 206f 6666  hese are not off
+00000d00: 6963 6961 6c20 7665 7273 696f 6e73 206f  icial versions o
+00000d10: 6620 6861 7a6d 2c20 6e6f 7420 7570 746f  f hazm, not upto
+00000d20: 6461 7465 206f 6e20 6675 6e63 7469 6f6e  date on function
+00000d30: 616c 6974 7920 616e 6420 6172 6520 6e6f  ality and are no
+00000d40: 7420 7375 7070 6f72 7465 6420 6279 2052  t supported by R
+00000d50: 6f73 6861 6e2e 0d0a 0d0a 2d20 5b2a 2a4a  oshan.....- [**J
+00000d60: 4861 7a6d 2a2a 5d28 6874 7470 733a 2f2f  Hazm**](https://
+00000d70: 6769 7468 7562 2e63 6f6d 2f6d 6f6a 7461  github.com/mojta
+00000d80: 6261 2d6b 6861 6c6c 6173 682f 4a48 617a  ba-khallash/JHaz
+00000d90: 6d29 3a20 4120 4a61 7661 2070 6f72 7420  m): A Java port 
+00000da0: 6f66 2048 617a 6d0d 0a2d 205b 2a2a 4e48  of Hazm..- [**NH
+00000db0: 617a 6d2a 2a5d 2868 7474 7073 3a2f 2f67  azm**](https://g
+00000dc0: 6974 6875 622e 636f 6d2f 6d6f 6a74 6162  ithub.com/mojtab
+00000dd0: 612d 6b68 616c 6c61 7368 2f4e 4861 7a6d  a-khallash/NHazm
+00000de0: 293a 2041 2043 2320 706f 7274 206f 6620  ): A C# port of 
+00000df0: 4861 7a6d 0d0a 0d0a 2323 2043 6f6e 7472  Hazm....## Contr
+00000e00: 6962 7574 696f 6e0d 0a0d 0a57 6520 7765  ibution....We we
+00000e10: 6c63 6f6d 6520 616e 6420 6170 7072 6563  lcome and apprec
+00000e20: 6961 7465 2061 6e79 2063 6f6e 7472 6962  iate any contrib
+00000e30: 7574 696f 6e73 2074 6f20 7468 6973 2072  utions to this r
+00000e40: 6570 6f2c 2073 7563 6820 6173 2062 7567  epo, such as bug
+00000e50: 2072 6570 6f72 7473 2c20 6665 6174 7572   reports, featur
+00000e60: 6520 7265 7175 6573 7473 2c20 636f 6465  e requests, code
+00000e70: 2069 6d70 726f 7665 6d65 6e74 732c 2064   improvements, d
+00000e80: 6f63 756d 656e 7461 7469 6f6e 2075 7064  ocumentation upd
+00000e90: 6174 6573 2c20 6574 632e 2050 6c65 6173  ates, etc. Pleas
+00000ea0: 6520 666f 6c6c 6f77 2074 6865 205b 436f  e follow the [Co
+00000eb0: 6e74 7269 6275 7469 6f6e 2067 7569 6465  ntribution guide
+00000ec0: 6c69 6e65 5d28 2e2f 434f 4e54 5249 4255  line](./CONTRIBU
+00000ed0: 5449 4f4e 2e6d 6429 2077 6865 6e20 636f  TION.md) when co
+00000ee0: 6e74 7269 6275 7469 6e67 2e20 596f 7520  ntributing. You 
+00000ef0: 6361 6e20 6f70 656e 2061 6e20 6973 7375  can open an issu
+00000f00: 652c 2066 6f72 6b20 7468 6520 7265 706f  e, fork the repo
+00000f10: 2c20 7772 6974 6520 796f 7572 2063 6f64  , write your cod
+00000f20: 652c 2063 7265 6174 6520 6120 7075 6c6c  e, create a pull
+00000f30: 2072 6571 7565 7374 2061 6e64 2077 6169   request and wai
+00000f40: 7420 666f 7220 6120 7265 7669 6577 2061  t for a review a
+00000f50: 6e64 2066 6565 6462 6163 6b2e 2054 6861  nd feedback. Tha
+00000f60: 6e6b 2079 6f75 2066 6f72 2079 6f75 7220  nk you for your 
+00000f70: 696e 7465 7265 7374 2061 6e64 2073 7570  interest and sup
+00000f80: 706f 7274 2069 6e20 7468 6973 2072 6570  port in this rep
+00000f90: 6f21 0d0a 0d0a 2323 2054 6861 6e6b 730d  o!....## Thanks.
+00000fa0: 0a0d 0a23 2323 2043 6f64 6520 636f 6e74  ...### Code cont
+00000fb0: 7269 6275 746f 7265 730d 0a0d 0a21 5b41  ributores....![A
+00000fc0: 6c74 5d28 6874 7470 733a 2f2f 7265 706f  lt](https://repo
+00000fd0: 6265 6174 732e 6178 696f 6d2e 636f 2f61  beats.axiom.co/a
+00000fe0: 7069 2f65 6d62 6564 2f61 6534 3262 6461  pi/embed/ae42bda
+00000ff0: 3135 3837 3931 3634 3564 3134 3363 3365  158791645d143c3e
+00001000: 3363 3766 3139 6438 6136 3864 3036 6430  3c7f19d8a68d06d0
+00001010: 382e 7376 6720 2252 6570 6f62 6561 7473  8.svg "Repobeats
+00001020: 2061 6e61 6c79 7469 6373 2069 6d61 6765   analytics image
+00001030: 2229 0d0a 0d0a 3c61 2068 7265 663d 2268  ")....<a href="h
+00001040: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001050: 6d2f 726f 7368 616e 2d72 6573 6561 7263  m/roshan-researc
+00001060: 682f 6861 7a6d 2f67 7261 7068 732f 636f  h/hazm/graphs/co
+00001070: 6e74 7269 6275 746f 7273 223e 0d0a 2020  ntributors">..  
+00001080: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00001090: 2f2f 636f 6e74 7269 622e 726f 636b 732f  //contrib.rocks/
+000010a0: 696d 6167 653f 7265 706f 3d72 6f73 6861  image?repo=rosha
+000010b0: 6e2d 7265 7365 6172 6368 2f68 617a 6d22  n-research/hazm"
+000010c0: 202f 3e0d 0a3c 2f61 3e0d 0a0d 0a23 2323   />..</a>....###
+000010d0: 204f 7468 6572 730d 0a0d 0a2d 2054 6861   Others....- Tha
+000010e0: 6e6b 7320 746f 205b 5669 7261 7374 7961  nks to [Virastya
+000010f0: 725d 2868 7474 703a 2f2f 7669 7261 7374  r](http://virast
+00001100: 7961 722e 6972 2f29 2070 726f 6a65 6374  yar.ir/) project
+00001110: 2066 6f72 2070 726f 7669 6469 6e67 2074   for providing t
+00001120: 6865 2070 6572 7369 616e 2077 6f72 6420  he persian word 
+00001130: 6c69 7374 2e0d 0a0d 0a5b 215b 5374 6172  list.....[![Star
+00001140: 2048 6973 746f 7279 2043 6861 7274 5d28   History Chart](
+00001150: 6874 7470 733a 2f2f 6170 692e 7374 6172  https://api.star
+00001160: 2d68 6973 746f 7279 2e63 6f6d 2f73 7667  -history.com/svg
+00001170: 3f72 6570 6f73 3d72 6f73 6861 6e2d 7265  ?repos=roshan-re
+00001180: 7365 6172 6368 2f68 617a 6d26 7479 7065  search/hazm&type
+00001190: 3d44 6174 6529 5d28 6874 7470 733a 2f2f  =Date)](https://
+000011a0: 7374 6172 2d68 6973 746f 7279 2e63 6f6d  star-history.com
+000011b0: 2f23 726f 7368 616e 2d72 6573 6561 7263  /#roshan-researc
+000011c0: 682f 6861 7a6d 2644 6174 6529 0d0a       h/hazm&Date)..
```

### Comparing `hazm-0.9.0/hazm/__init__.py` & `hazm-0.9.1/hazm/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-"""entry point for the package."""
-
-from typing import List
-
-from hazm.utils import default_verbs
-from hazm.utils import default_words
-from hazm.utils import stopwords_list
-from hazm.utils import words_list
-from hazm.utils import maketrans
-from hazm.utils import regex_replace
-from hazm.utils import words_list
-from hazm.utils import NUMBERS
-from hazm.utils import informal_verbs
-from hazm.utils import informal_words
-
-from hazm.sequence_tagger import IOBTagger
-from hazm.sequence_tagger import SequenceTagger
-
-from hazm.pos_tagger import POSTagger
-from hazm.pos_tagger import StanfordPOSTagger
-
-from hazm.stemmer import Stemmer
-from hazm.word_tokenizer import WordTokenizer
-
-from hazm.lemmatizer import Conjugation
-from hazm.lemmatizer import Lemmatizer
-
-from hazm.normalizer import Normalizer
-
-from hazm.chunker import Chunker
-from hazm.chunker import RuleBasedChunker
-from hazm.chunker import tree2brackets
-
-from hazm.sentence_tokenizer import SentenceTokenizer
-
-def sent_tokenize(text: str) -> List[str]:
-    """Sentence Tokenizer."""
-    if not hasattr(sent_tokenize, "tokenizer"):
-        sent_tokenize.tokenizer = SentenceTokenizer()
-    return sent_tokenize.tokenizer.tokenize(text)
-
-
-def word_tokenize(sentence: str) -> List[str]:
-    """Word Tokenizer."""
-    if not hasattr(word_tokenize, "tokenizer"):
-        word_tokenize.tokenizer = WordTokenizer()
-    return word_tokenize.tokenizer.tokenize(sentence)
-
-from hazm.corpus_readers import PeykareReader
-from hazm.corpus_readers import BijankhanReader
-from hazm.corpus_readers import DadeganReader
-from hazm.corpus_readers import DegarbayanReader
-from hazm.corpus_readers import HamshahriReader
-from hazm.corpus_readers import MirasTextReader
-from hazm.corpus_readers import PersicaReader
-from hazm.corpus_readers import QuranReader
-from hazm.corpus_readers import SentiPersReader
-from hazm.corpus_readers import TNewsReader
-from hazm.corpus_readers import TreebankReader
-from hazm.corpus_readers import VerbValencyReader
-from hazm.corpus_readers import WikipediaReader
-from hazm.corpus_readers import persian_plain_text_reader
-
-from hazm.dependency_parser import DependencyParser
-from hazm.dependency_parser import MaltParser
-from hazm.dependency_parser import TurboParser
-
-from hazm.embedding import SentEmbedding
-from hazm.embedding import WordEmbedding
-
-from hazm.informal_normalizer import InformalLemmatizer
-from hazm.informal_normalizer import InformalNormalizer
-
-from hazm.token_splitter import TokenSplitter
-
-
+"""entry point for the package."""
+
+from typing import List
+
+from hazm.utils import default_verbs
+from hazm.utils import default_words
+from hazm.utils import stopwords_list
+from hazm.utils import words_list
+from hazm.utils import maketrans
+from hazm.utils import regex_replace
+from hazm.utils import words_list
+from hazm.utils import NUMBERS
+from hazm.utils import informal_verbs
+from hazm.utils import informal_words
+
+from hazm.sequence_tagger import IOBTagger
+from hazm.sequence_tagger import SequenceTagger
+
+from hazm.pos_tagger import POSTagger
+from hazm.pos_tagger import StanfordPOSTagger
+
+from hazm.stemmer import Stemmer
+from hazm.word_tokenizer import WordTokenizer
+
+from hazm.lemmatizer import Conjugation
+from hazm.lemmatizer import Lemmatizer
+
+from hazm.normalizer import Normalizer
+
+from hazm.chunker import Chunker
+from hazm.chunker import RuleBasedChunker
+from hazm.chunker import tree2brackets
+
+from hazm.sentence_tokenizer import SentenceTokenizer
+
+def sent_tokenize(text: str) -> List[str]:
+    """Sentence Tokenizer."""
+    if not hasattr(sent_tokenize, "tokenizer"):
+        sent_tokenize.tokenizer = SentenceTokenizer()
+    return sent_tokenize.tokenizer.tokenize(text)
+
+
+def word_tokenize(sentence: str) -> List[str]:
+    """Word Tokenizer."""
+    if not hasattr(word_tokenize, "tokenizer"):
+        word_tokenize.tokenizer = WordTokenizer()
+    return word_tokenize.tokenizer.tokenize(sentence)
+
+from hazm.corpus_readers import PeykareReader
+from hazm.corpus_readers import BijankhanReader
+from hazm.corpus_readers import DadeganReader
+from hazm.corpus_readers import DegarbayanReader
+from hazm.corpus_readers import HamshahriReader
+from hazm.corpus_readers import MirasTextReader
+from hazm.corpus_readers import PersicaReader
+from hazm.corpus_readers import QuranReader
+from hazm.corpus_readers import SentiPersReader
+from hazm.corpus_readers import TNewsReader
+from hazm.corpus_readers import TreebankReader
+from hazm.corpus_readers import VerbValencyReader
+from hazm.corpus_readers import WikipediaReader
+from hazm.corpus_readers import persian_plain_text_reader
+
+from hazm.dependency_parser import DependencyParser
+from hazm.dependency_parser import MaltParser
+from hazm.dependency_parser import TurboParser
+
+from hazm.embedding import SentEmbedding
+from hazm.embedding import WordEmbedding
+
+from hazm.informal_normalizer import InformalLemmatizer
+from hazm.informal_normalizer import InformalNormalizer
+
+from hazm.token_splitter import TokenSplitter
+
+
```

### Comparing `hazm-0.9.0/hazm/chunker.py` & `hazm-0.9.1/hazm/chunker.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای تجزیهٔ متن به عبارات اسمی، فعلی و حرف
-اضافه‌ای است. **میزان دقت تجزیه‌گر سطحی در نسخهٔ حاضر ۹۳.۴ درصد [^1] است.**
-[^1]:
-این عدد با انتشار هر نسخه بروزرسانی می‌شود.
-
-"""
-
-from typing import Dict
-from typing import Iterator
-from typing import List
-from typing import Tuple
-from typing import Union
-
-from nltk.chunk import RegexpParser
-from nltk.chunk import conlltags2tree
-from nltk.chunk import tree2conlltags
-
-from hazm import POSTagger
-from hazm import IOBTagger
-
-
-def tree2brackets(tree: str) -> str:
-    """خروجی درختی تابع [parse()][hazm.chunker.Chunker.parse] را به یک ساختار
-    کروشه‌ای تبدیل می‌کند.
-
-    Examples:
-        >>> chunker = Chunker(model='resources/chunker.model')
-        >>> tree=chunker.parse([('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')])
-        >>> print(tree)
-        (S
-          (NP نامه/NOUN,EZ ایشان/PRON)
-          (POSTP را/ADP)
-          (VP دریافت/NOUN داشتم/VERB)
-          ./PUNCT)
-
-        >>> tree2brackets(tree)
-        '[نامه ایشان NP] [را POSTP] [دریافت داشتم VP] .'
-
-    Args:
-        tree: ساختار درختی حاصل از پردزاش تابع parse()
-
-    Returns:
-        رشته‌ای از کروشه‌ها که در هر کروشه جزئی از متن به همراه نوع آن جای گرفته است.
-
-    """
-    s, tag = "", ""
-    for item in tree2conlltags(tree):
-        if item[2][0] in {"B", "O"} and tag:
-            s += tag + "] "
-            tag = ""
-
-        if item[2][0] == "B":
-            tag = item[2].split("-")[1]
-            s += "["
-        s += item[0] + " "
-
-    if tag:
-        s += tag + "] "
-
-    return s.strip()
-
-
-class Chunker(IOBTagger):
-    """این کلاس شامل توابعی برای تقطیع متن، آموزش و ارزیابی مدل است."""
-
-    def __init__(
-        self: "Chunker",
-        model: str = None,
-        data_maker: List[List[Dict]] = None,
-    ) -> None:
-        """constructor."""
-        data_maker = self.data_maker if data_maker is None else data_maker
-        self.posTagger = POSTagger()
-        super().__init__(model, data_maker)
-
-    def data_maker(
-        self: "Chunker",
-        tokens: List[List[Tuple[str, str]]],
-    ) -> List[List[Dict]]:
-        """تابعی که لیستی دو بعدی از کلمات به همراه لیبل را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
-
-        Examples:
-            >>> chunker = Chunker(model = 'resources/chunker.model')
-            >>> chunker.data_maker(tokens = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]])
-            [[{'word': 'من', 'is_first': True, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'من', 'prefix-3': 'من', 'suffix-1': 'ن', 'suffix-2': 'من', 'suffix-3': 'من', 'prev_word': '', 'two_prev_word': '', 'next_word': 'به', 'two_next_word': 'مدرسه', 'is_numeric': False, 'prev_is_numeric': '', 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': '', 'next_is_punc': False, 'pos': 'PRON', 'prev_pos': '', 'next_pos': 'ADP'}, {'word': 'به', 'is_first': False, 'is_last': False, 'prefix-1': 'ب', 'prefix-2': 'به', 'prefix-3': 'به', 'suffix-1': 'ه', 'suffix-2': 'به', 'suffix-3': 'به', 'prev_word': 'من', 'two_prev_word': '.', 'next_word': 'مدرسه', 'two_next_word': 'ایران', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'ADP', 'prev_pos': 'PRON', 'next_pos': 'NOUN,EZ'}, {'word': 'مدرسه', 'is_first': False, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'مد', 'prefix-3': 'مدر', 'suffix-1': 'ه', 'suffix-2': 'سه', 'suffix-3': 'رسه', 'prev_word': 'به', 'two_prev_word': 'من', 'next_word': 'ایران', 'two_next_word': 'رفته_بودم', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'NOUN,EZ', 'prev_pos': 'ADP', 'next_pos': 'NOUN'}, {'word': 'ایران', 'is_first': False, 'is_last': False, 'prefix-1': 'ا', 'prefix-2': 'ای', 'prefix-3': 'ایر', 'suffix-1': 'ن', 'suffix-2': 'ان', 'suffix-3': 'ران', 'prev_word': 'مدرسه', 'two_prev_word': 'به', 'next_word': 'رفته_بودم', 'two_next_word': '.', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'NOUN', 'prev_pos': 'NOUN,EZ', 'next_pos': 'VERB'}, {'word': 'رفته_بودم', 'is_first': False, 'is_last': False, 'prefix-1': 'ر', 'prefix-2': 'رف', 'prefix-3': 'رفت', 'suffix-1': 'م', 'suffix-2': 'دم', 'suffix-3': 'ودم', 'prev_word': 'ایران', 'two_prev_word': 'مدرسه', 'next_word': '.', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': True, 'pos': 'VERB', 'prev_pos': 'NOUN', 'next_pos': 'PUNCT'}, {'word': '.', 'is_first': False, 'is_last': True, 'prefix-1': '.', 'prefix-2': '.', 'prefix-3': '.', 'suffix-1': '.', 'suffix-2': '.', 'suffix-3': '.', 'prev_word': 'رفته_بودم', 'two_prev_word': 'ایران', 'next_word': '', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': '', 'is_punc': True, 'prev_is_punc': False, 'next_is_punc': '', 'pos': 'PUNCT', 'prev_pos': 'VERB', 'next_pos': ''}]]
-
-        Args:
-            tokens: جملاتی که نیاز به تبدیل آن به برداری از ویژگی‌ها است.
-
-        Returns:
-            لیستی از لیستی از دیکشنری‌های بیان‌کننده ویژگی‌های یک کلمه.
-
-        """
-        words = [[word for word, _ in token] for token in tokens]
-        tags = [[tag for _, tag in token] for token in tokens]
-        return [
-            [
-                self.features(words=word_tokens, pos_tags=tag_tokens, index=index)
-                for index in range(len(word_tokens))
-            ]
-            for word_tokens, tag_tokens in zip(words, tags)
-        ]
-
-    def features(
-        self: "Chunker",
-        words: List[str],
-        pos_tags: List[str],
-        index: int,
-    ) -> Dict[str, Union[str, bool]]:
-        """ویژگی‌های کلمه را برمی‌گرداند."""
-        word_features = self.posTagger.features(words, index)
-        word_features.update(
-            {
-                "pos": pos_tags[index],
-                "prev_pos": "" if index == 0 else pos_tags[index - 1],
-                "next_pos": "" if index == len(pos_tags) - 1 else pos_tags[index + 1],
-            },
-        )
-        return word_features
-
-    def train(
-        self: "Chunker",
-        trees: List[str],
-        c1: float = 0.4,
-        c2: float = 0.04,
-        max_iteration: int = 400,
-        verbose: bool = True,
-        file_name: str = "chunker_crf.model",
-        report_duration: bool = True,
-    ) -> None:
-        """از روی درخت ورودی، مدل را آموزش می‌دهد.
-
-        Args:
-            trees: لیستی از درخت‌ها برای آموزش مدل.
-            c1: مقدار L1 regularization.
-            c2: مقدار L2 regularization.
-            max_iteration: تعداد تکرار آموزش بر کل دیتا.
-            verbose: نمایش اطلاعات مربوط به آموزش.
-            file_name: نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
-            report_duration: نمایش گزارشات مربوط به زمان.
-
-        """
-        return super().train(
-            [tree2conlltags(tree) for tree in trees],
-            c1,
-            c2,
-            max_iteration,
-            verbose,
-            file_name,
-            report_duration,
-        )
-
-    def parse(self: "Chunker", sentence: List[Tuple[str, str]]) -> str:
-        """جمله‌ای را در قالب لیستی از تاپل‌های دوتایی [(توکن, نوع), (توکن, نوع), ...]
-        دریافت می‌کند و درخت تقطع‌شدهٔ آن را بر می‌گرداند.
-
-        Examples:
-            >>> chunker = Chunker(model = 'resources/chunker.model')
-            >>> tree = chunker.parse(sentence = [('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')])
-            >>> print(tree)
-            (S
-              (NP نامه/NOUN,EZ ایشان/PRON)
-              (POSTP را/ADP)
-              (VP دریافت/NOUN داشتم/VERB)
-              ./PUNCT)
-
-        Args:
-            sentence: جمله‌ای که باید درخت تقطیع‌شدهٔ آن تولید شود.
-
-        Returns:
-            ساختار درختی حاصل از تقطیع.
-            برای تبدیل این ساختار درختی به یک ساختار کروشه‌ای و قابل‌درک‌تر
-            می‌توانید از تابع `tree2brackets()` استفاده کنید.
-
-        """
-        return conlltags2tree(super().tag(sentence))
-
-    def parse_sents(
-        self: "Chunker",
-        sentences: List[List[Tuple[str, str]]],
-    ) -> Iterator[str]:
-        """جملات ورودی را به‌شکل تقطیع‌شده و در قالب یک برمی‌گرداند.
-
-        Args:
-            sentences: جملات ورودی.
-
-        Yields:
-            یک `Iterator` از جملات تقطیع شده.
-
-        """
-        for conlltagged in super().tag_sents(sentences):
-            yield conlltags2tree(conlltagged)
-
-    def evaluate(self: "Chunker", trees: List[str]) -> float:
-        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
-
-        Examples:
-            >>> chunker = Chunker(model = 'resources/chunker.model')
-            >>> trees = list(chunker.parse_sents([[('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')]]))
-            >>> chunker.evaluate(trees)
-            1.0
-
-        Args:
-            trees: لیست درختانی که با استفاده از آن مدل را ارزیابی می‌کنیم.
-
-        Returns:
-            دقت مدل
-
-        """
-        return super().evaluate([tree2conlltags(tree) for tree in trees])
-
-
-class RuleBasedChunker(RegexpParser):
-    """کلاس RuleBasedChunker.
-
-
-    Examples:
-    >>> chunker = RuleBasedChunker()
-    >>> tree2brackets(chunker.parse([('نامه', 'Ne'), ('۱۰', 'NUMe'), ('فوریه', 'Ne'), ('شما', 'PRO'), ('را', 'POSTP'), ('دریافت', 'N'), ('داشتم', 'V'), ('.', 'PUNC')]))
-    '[نامه ۱۰ فوریه شما NP] [را POSTP] [دریافت داشتم VP] .'
-
-    """
-
-    def __init__(self: "RuleBasedChunker") -> None:
-        """Init."""
-        grammar = r"""
-
-            NP:
-                <P>{<N>}<V>
-
-            VP:
-                <.*[^e]>{<N>?<V>}
-                {<V>}
-
-            ADVP:
-                {<ADVe?><AJ>?}
-
-            ADJP:
-                <.*[^e]>{<AJe?>}
-
-            NP:
-                {<DETe?|Ne?|NUMe?|AJe|PRO|CL|RESe?><DETe?|Ne?|NUMe?|AJe?|PRO|CL|RESe?>*}
-                <N>}{<.*e?>
-
-            ADJP:
-                {<AJe?>}
-
-            POSTP:
-                {<POSTP>}
-
-            PP:
-                {<Pe?>+}
-
-        """
-
-        super().__init__(grammar=grammar)
+"""این ماژول شامل کلاس‌ها و توابعی برای تجزیهٔ متن به عبارات اسمی، فعلی و حرف
+اضافه‌ای است. **میزان دقت تجزیه‌گر سطحی در نسخهٔ حاضر ۹۳.۴ درصد [^1] است.**
+[^1]:
+این عدد با انتشار هر نسخه بروزرسانی می‌شود.
+
+"""
+
+from typing import Dict
+from typing import Iterator
+from typing import List
+from typing import Tuple
+from typing import Union
+
+from nltk.chunk import RegexpParser
+from nltk.chunk import conlltags2tree
+from nltk.chunk import tree2conlltags
+
+from hazm import POSTagger
+from hazm import IOBTagger
+
+
+def tree2brackets(tree: str) -> str:
+    """خروجی درختی تابع [parse()][hazm.chunker.Chunker.parse] را به یک ساختار
+    کروشه‌ای تبدیل می‌کند.
+
+    Examples:
+        >>> chunker = Chunker(model='resources/chunker.model')
+        >>> tree=chunker.parse([('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')])
+        >>> print(tree)
+        (S
+          (NP نامه/NOUN,EZ ایشان/PRON)
+          (POSTP را/ADP)
+          (VP دریافت/NOUN داشتم/VERB)
+          ./PUNCT)
+
+        >>> tree2brackets(tree)
+        '[نامه ایشان NP] [را POSTP] [دریافت داشتم VP] .'
+
+    Args:
+        tree: ساختار درختی حاصل از پردزاش تابع parse()
+
+    Returns:
+        رشته‌ای از کروشه‌ها که در هر کروشه جزئی از متن به همراه نوع آن جای گرفته است.
+
+    """
+    s, tag = "", ""
+    for item in tree2conlltags(tree):
+        if item[2][0] in {"B", "O"} and tag:
+            s += tag + "] "
+            tag = ""
+
+        if item[2][0] == "B":
+            tag = item[2].split("-")[1]
+            s += "["
+        s += item[0] + " "
+
+    if tag:
+        s += tag + "] "
+
+    return s.strip()
+
+
+class Chunker(IOBTagger):
+    """این کلاس شامل توابعی برای تقطیع متن، آموزش و ارزیابی مدل است."""
+
+    def __init__(
+        self: "Chunker",
+        model: str = None,
+        data_maker: List[List[Dict]] = None,
+    ) -> None:
+        """constructor."""
+        data_maker = self.data_maker if data_maker is None else data_maker
+        self.posTagger = POSTagger()
+        super().__init__(model, data_maker)
+
+    def data_maker(
+        self: "Chunker",
+        tokens: List[List[Tuple[str, str]]],
+    ) -> List[List[Dict]]:
+        """تابعی که لیستی دو بعدی از کلمات به همراه لیبل را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
+
+        Examples:
+            >>> chunker = Chunker(model = 'resources/chunker.model')
+            >>> chunker.data_maker(tokens = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]])
+            [[{'word': 'من', 'is_first': True, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'من', 'prefix-3': 'من', 'suffix-1': 'ن', 'suffix-2': 'من', 'suffix-3': 'من', 'prev_word': '', 'two_prev_word': '', 'next_word': 'به', 'two_next_word': 'مدرسه', 'is_numeric': False, 'prev_is_numeric': '', 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': '', 'next_is_punc': False, 'pos': 'PRON', 'prev_pos': '', 'next_pos': 'ADP'}, {'word': 'به', 'is_first': False, 'is_last': False, 'prefix-1': 'ب', 'prefix-2': 'به', 'prefix-3': 'به', 'suffix-1': 'ه', 'suffix-2': 'به', 'suffix-3': 'به', 'prev_word': 'من', 'two_prev_word': '.', 'next_word': 'مدرسه', 'two_next_word': 'ایران', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'ADP', 'prev_pos': 'PRON', 'next_pos': 'NOUN,EZ'}, {'word': 'مدرسه', 'is_first': False, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'مد', 'prefix-3': 'مدر', 'suffix-1': 'ه', 'suffix-2': 'سه', 'suffix-3': 'رسه', 'prev_word': 'به', 'two_prev_word': 'من', 'next_word': 'ایران', 'two_next_word': 'رفته_بودم', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'NOUN,EZ', 'prev_pos': 'ADP', 'next_pos': 'NOUN'}, {'word': 'ایران', 'is_first': False, 'is_last': False, 'prefix-1': 'ا', 'prefix-2': 'ای', 'prefix-3': 'ایر', 'suffix-1': 'ن', 'suffix-2': 'ان', 'suffix-3': 'ران', 'prev_word': 'مدرسه', 'two_prev_word': 'به', 'next_word': 'رفته_بودم', 'two_next_word': '.', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'NOUN', 'prev_pos': 'NOUN,EZ', 'next_pos': 'VERB'}, {'word': 'رفته_بودم', 'is_first': False, 'is_last': False, 'prefix-1': 'ر', 'prefix-2': 'رف', 'prefix-3': 'رفت', 'suffix-1': 'م', 'suffix-2': 'دم', 'suffix-3': 'ودم', 'prev_word': 'ایران', 'two_prev_word': 'مدرسه', 'next_word': '.', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': True, 'pos': 'VERB', 'prev_pos': 'NOUN', 'next_pos': 'PUNCT'}, {'word': '.', 'is_first': False, 'is_last': True, 'prefix-1': '.', 'prefix-2': '.', 'prefix-3': '.', 'suffix-1': '.', 'suffix-2': '.', 'suffix-3': '.', 'prev_word': 'رفته_بودم', 'two_prev_word': 'ایران', 'next_word': '', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': '', 'is_punc': True, 'prev_is_punc': False, 'next_is_punc': '', 'pos': 'PUNCT', 'prev_pos': 'VERB', 'next_pos': ''}]]
+
+        Args:
+            tokens: جملاتی که نیاز به تبدیل آن به برداری از ویژگی‌ها است.
+
+        Returns:
+            لیستی از لیستی از دیکشنری‌های بیان‌کننده ویژگی‌های یک کلمه.
+
+        """
+        words = [[word for word, _ in token] for token in tokens]
+        tags = [[tag for _, tag in token] for token in tokens]
+        return [
+            [
+                self.features(words=word_tokens, pos_tags=tag_tokens, index=index)
+                for index in range(len(word_tokens))
+            ]
+            for word_tokens, tag_tokens in zip(words, tags)
+        ]
+
+    def features(
+        self: "Chunker",
+        words: List[str],
+        pos_tags: List[str],
+        index: int,
+    ) -> Dict[str, Union[str, bool]]:
+        """ویژگی‌های کلمه را برمی‌گرداند."""
+        word_features = self.posTagger.features(words, index)
+        word_features.update(
+            {
+                "pos": pos_tags[index],
+                "prev_pos": "" if index == 0 else pos_tags[index - 1],
+                "next_pos": "" if index == len(pos_tags) - 1 else pos_tags[index + 1],
+            },
+        )
+        return word_features
+
+    def train(
+        self: "Chunker",
+        trees: List[str],
+        c1: float = 0.4,
+        c2: float = 0.04,
+        max_iteration: int = 400,
+        verbose: bool = True,
+        file_name: str = "chunker_crf.model",
+        report_duration: bool = True,
+    ) -> None:
+        """از روی درخت ورودی، مدل را آموزش می‌دهد.
+
+        Args:
+            trees: لیستی از درخت‌ها برای آموزش مدل.
+            c1: مقدار L1 regularization.
+            c2: مقدار L2 regularization.
+            max_iteration: تعداد تکرار آموزش بر کل دیتا.
+            verbose: نمایش اطلاعات مربوط به آموزش.
+            file_name: نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
+            report_duration: نمایش گزارشات مربوط به زمان.
+
+        """
+        return super().train(
+            [tree2conlltags(tree) for tree in trees],
+            c1,
+            c2,
+            max_iteration,
+            verbose,
+            file_name,
+            report_duration,
+        )
+
+    def parse(self: "Chunker", sentence: List[Tuple[str, str]]) -> str:
+        """جمله‌ای را در قالب لیستی از تاپل‌های دوتایی [(توکن, نوع), (توکن, نوع), ...]
+        دریافت می‌کند و درخت تقطع‌شدهٔ آن را بر می‌گرداند.
+
+        Examples:
+            >>> chunker = Chunker(model = 'resources/chunker.model')
+            >>> tree = chunker.parse(sentence = [('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')])
+            >>> print(tree)
+            (S
+              (NP نامه/NOUN,EZ ایشان/PRON)
+              (POSTP را/ADP)
+              (VP دریافت/NOUN داشتم/VERB)
+              ./PUNCT)
+
+        Args:
+            sentence: جمله‌ای که باید درخت تقطیع‌شدهٔ آن تولید شود.
+
+        Returns:
+            ساختار درختی حاصل از تقطیع.
+            برای تبدیل این ساختار درختی به یک ساختار کروشه‌ای و قابل‌درک‌تر
+            می‌توانید از تابع `tree2brackets()` استفاده کنید.
+
+        """
+        return conlltags2tree(super().tag(sentence))
+
+    def parse_sents(
+        self: "Chunker",
+        sentences: List[List[Tuple[str, str]]],
+    ) -> Iterator[str]:
+        """جملات ورودی را به‌شکل تقطیع‌شده و در قالب یک برمی‌گرداند.
+
+        Args:
+            sentences: جملات ورودی.
+
+        Yields:
+            یک `Iterator` از جملات تقطیع شده.
+
+        """
+        for conlltagged in super().tag_sents(sentences):
+            yield conlltags2tree(conlltagged)
+
+    def evaluate(self: "Chunker", trees: List[str]) -> float:
+        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
+
+        Examples:
+            >>> chunker = Chunker(model = 'resources/chunker.model')
+            >>> trees = list(chunker.parse_sents([[('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')]]))
+            >>> chunker.evaluate(trees)
+            1.0
+
+        Args:
+            trees: لیست درختانی که با استفاده از آن مدل را ارزیابی می‌کنیم.
+
+        Returns:
+            دقت مدل
+
+        """
+        return super().evaluate([tree2conlltags(tree) for tree in trees])
+
+
+class RuleBasedChunker(RegexpParser):
+    """کلاس RuleBasedChunker.
+
+
+    Examples:
+    >>> chunker = RuleBasedChunker()
+    >>> tree2brackets(chunker.parse([('نامه', 'Ne'), ('۱۰', 'NUMe'), ('فوریه', 'Ne'), ('شما', 'PRO'), ('را', 'POSTP'), ('دریافت', 'N'), ('داشتم', 'V'), ('.', 'PUNC')]))
+    '[نامه ۱۰ فوریه شما NP] [را POSTP] [دریافت داشتم VP] .'
+
+    """
+
+    def __init__(self: "RuleBasedChunker") -> None:
+        """Init."""
+        grammar = r"""
+
+            NP:
+                <P>{<N>}<V>
+
+            VP:
+                <.*[^e]>{<N>?<V>}
+                {<V>}
+
+            ADVP:
+                {<ADVe?><AJ>?}
+
+            ADJP:
+                <.*[^e]>{<AJe?>}
+
+            NP:
+                {<DETe?|Ne?|NUMe?|AJe|PRO|CL|RESe?><DETe?|Ne?|NUMe?|AJe?|PRO|CL|RESe?>*}
+                <N>}{<.*e?>
+
+            ADJP:
+                {<AJe?>}
+
+            POSTP:
+                {<POSTP>}
+
+            PP:
+                {<Pe?>+}
+
+        """
+
+        super().__init__(grammar=grammar)
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/__init__.py` & `hazm-0.9.1/hazm/corpus_readers/__init__.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""init."""
-from .bijankhan_reader import BijankhanReader
-from .dadegan_reader import DadeganReader
-from .degarbayan_reader import DegarbayanReader
-from .hamshahri_reader import HamshahriReader
-from .mirastext_reader import MirasTextReader
-from .persica_reader import PersicaReader
-from .peykare_reader import PeykareReader
-from .quran_reader import QuranReader
-from .sentipers_reader import SentiPersReader
-from .tnews_reader import TNewsReader
-from .treebank_reader import TreebankReader
-from .verbvalency_reader import VerbValencyReader
-from .wikipedia_reader import WikipediaReader
+"""init."""
+from .bijankhan_reader import BijankhanReader
+from .dadegan_reader import DadeganReader
+from .degarbayan_reader import DegarbayanReader
+from .hamshahri_reader import HamshahriReader
+from .mirastext_reader import MirasTextReader
+from .persica_reader import PersicaReader
+from .peykare_reader import PeykareReader
+from .quran_reader import QuranReader
+from .sentipers_reader import SentiPersReader
+from .tnews_reader import TNewsReader
+from .treebank_reader import TreebankReader
+from .verbvalency_reader import VerbValencyReader
+from .wikipedia_reader import WikipediaReader
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/bijankhan_reader.py` & `hazm-0.9.1/hazm/corpus_readers/bijankhan_reader.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ بی‌جن‌خان است.
-
-[پیکرهٔ
-بی‌جن‌خان](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-
-%D8%A8%DB%8C%E2%80%8C%D8%AC%D9%86%E2%80%8C%D8%AE%D8%A7%D9%86) مجموعه‌ای
-است از متون فارسی شامل بیش از ۲ میلیون و ۶۰۰ هزار کلمه که با ۵۵۰ نوع برچسب POS
-برچسب‌گذاری شده‌اند. این پیکره که در پژوهشکدهٔ پردازش هوشمند علائم تهیه شده است
-همچنین شامل بیش از ۴۳۰۰ تگ موضوعی چون سیاسی، تاریخی و ... برای متون است.
-
-"""
-
-import re
-from pathlib import Path
-from typing import Iterator
-from typing import List
-from typing import Tuple
-
-from hazm import Normalizer
-from .peykare_reader import join_verb_parts
-
-default_pos_map = {
-    "ADJ": "ADJ",
-    "ADJ_CMPR": "ADJ",
-    "ADJ_INO": "ADJ",
-    "ADJ_ORD": "ADJ",
-    "ADJ_SIM": "ADJ",
-    "ADJ_SUP": "ADJ",
-    "ADV": "ADV",
-    "ADV_EXM": "ADV",
-    "ADV_I": "ADV",
-    "ADV_NEGG": "ADV",
-    "ADV_NI": "ADV",
-    "ADV_TIME": "ADV",
-    "AR": "AR",
-    "CON": "CONJ",
-    "DEFAULT": "DEFAULT",
-    "DELM": "PUNC",
-    "DET": "PREP",
-    "IF": "IF",
-    "INT": "INT",
-    "MORP": "MORP",
-    "MQUA": "MQUA",
-    "MS": "MS",
-    "N_PL": "N",
-    "N_SING": "N",
-    "NN": "NN",
-    "NP": "NP",
-    "OH": "OH",
-    "OHH": "OHH",
-    "P": "PREP",
-    "PP": "PP",
-    "PRO": "PR",
-    "PS": "PS",
-    "QUA": "QUA",
-    "SPEC": "SPEC",
-    "V_AUX": "V",
-    "V_IMP": "V",
-    "V_PA": "V",
-    "V_PRE": "V",
-    "V_PRS": "V",
-    "V_SUB": "V",
-}
-
-
-class BijankhanReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ بی‌جن‌خان است.
-
-    Args:
-        bijankhan_file: مسیر فایلِ پیکره.
-        joined_verb_parts: اگر `True‍` باشد افعال چندبخشی را با _ به‌هم می‌چسباند.
-        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
-
-    """
-
-    def __init__(
-        self: "BijankhanReader",
-        bijankhan_file: str,
-        joined_verb_parts: bool = True,
-        pos_map: str = None,
-    ) -> None:
-        """Init."""
-        if pos_map is None:
-            pos_map = default_pos_map
-        self._bijankhan_file = bijankhan_file
-        self._joined_verb_parts = joined_verb_parts
-        self._pos_map = pos_map
-        self._normalizer = Normalizer(correct_spacing=False)
-
-    def _sentences(self: "BijankhanReader") -> Iterator[List[Tuple[str, str]]]:
-        """جملات پیکره را به شکل متن خام برمی‌گرداند.
-
-        Yields:
-            جملهٔ بعدی.
-
-        """
-        sentence = []
-        with Path(self._bijankhan_file).open(encoding="utf-8") as f:
-            length = 2
-            for line in f:
-                parts = re.split("  +", line.strip())
-                if len(parts) == length:
-                    word, tag = parts
-                    if word not in ("#", "*"):
-                        word = self._normalizer.normalize(word)
-                        sentence.append((word if word else "_", tag))
-                    if (
-                        tag == "DELM"
-                        and word in ("#", "*", ".", "؟", "!")
-                        and len(sentence)
-                    ):
-                        yield sentence
-                        sentence = []
-
-    def sents(self: "BijankhanReader") -> Iterator[List[Tuple[str, str]]]:
-        """جملات پیکره را به شکل لیستی از `(توکن،برچسب)`ها برمی‌گرداند..
-
-        Examples:
-            >>> bijankhan = BijankhanReader(bijankhan_file='corpora/bijankhan.txt')
-            >>> next(bijankhan.sents())
-            [('اولین', 'ADJ'), ('سیاره', 'N'), ('خارج', 'ADJ'), ('از', 'PREP'), ('منظومه', 'N'), ('شمسی', 'ADJ'), ('دیده_شد', 'V'), ('.', 'PUNC')]
-
-        Yields:
-            جملهٔ بعدی در قالب لیستی از `(توکن،برچسب)`ها.
-
-        """
-
-        def map_poses(item: Tuple[str, str]) -> Tuple[str, str]:
-            return (item[0], self._pos_map.get(item[1], item[1]))
-
-        for sentence in self._sentences():
-            if self._joined_verb_parts:
-                sentence = join_verb_parts(sentence)
-            yield list(map(map_poses, sentence))
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ بی‌جن‌خان است.
+
+[پیکرهٔ
+بی‌جن‌خان](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-
+%D8%A8%DB%8C%E2%80%8C%D8%AC%D9%86%E2%80%8C%D8%AE%D8%A7%D9%86) مجموعه‌ای
+است از متون فارسی شامل بیش از ۲ میلیون و ۶۰۰ هزار کلمه که با ۵۵۰ نوع برچسب POS
+برچسب‌گذاری شده‌اند. این پیکره که در پژوهشکدهٔ پردازش هوشمند علائم تهیه شده است
+همچنین شامل بیش از ۴۳۰۰ تگ موضوعی چون سیاسی، تاریخی و ... برای متون است.
+
+"""
+
+import re
+from pathlib import Path
+from typing import Iterator
+from typing import List
+from typing import Tuple
+
+from hazm import Normalizer
+from .peykare_reader import join_verb_parts
+
+default_pos_map = {
+    "ADJ": "ADJ",
+    "ADJ_CMPR": "ADJ",
+    "ADJ_INO": "ADJ",
+    "ADJ_ORD": "ADJ",
+    "ADJ_SIM": "ADJ",
+    "ADJ_SUP": "ADJ",
+    "ADV": "ADV",
+    "ADV_EXM": "ADV",
+    "ADV_I": "ADV",
+    "ADV_NEGG": "ADV",
+    "ADV_NI": "ADV",
+    "ADV_TIME": "ADV",
+    "AR": "AR",
+    "CON": "CONJ",
+    "DEFAULT": "DEFAULT",
+    "DELM": "PUNC",
+    "DET": "PREP",
+    "IF": "IF",
+    "INT": "INT",
+    "MORP": "MORP",
+    "MQUA": "MQUA",
+    "MS": "MS",
+    "N_PL": "N",
+    "N_SING": "N",
+    "NN": "NN",
+    "NP": "NP",
+    "OH": "OH",
+    "OHH": "OHH",
+    "P": "PREP",
+    "PP": "PP",
+    "PRO": "PR",
+    "PS": "PS",
+    "QUA": "QUA",
+    "SPEC": "SPEC",
+    "V_AUX": "V",
+    "V_IMP": "V",
+    "V_PA": "V",
+    "V_PRE": "V",
+    "V_PRS": "V",
+    "V_SUB": "V",
+}
+
+
+class BijankhanReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ بی‌جن‌خان است.
+
+    Args:
+        bijankhan_file: مسیر فایلِ پیکره.
+        joined_verb_parts: اگر `True‍` باشد افعال چندبخشی را با _ به‌هم می‌چسباند.
+        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
+
+    """
+
+    def __init__(
+        self: "BijankhanReader",
+        bijankhan_file: str,
+        joined_verb_parts: bool = True,
+        pos_map: str = None,
+    ) -> None:
+        """Init."""
+        if pos_map is None:
+            pos_map = default_pos_map
+        self._bijankhan_file = bijankhan_file
+        self._joined_verb_parts = joined_verb_parts
+        self._pos_map = pos_map
+        self._normalizer = Normalizer(correct_spacing=False)
+
+    def _sentences(self: "BijankhanReader") -> Iterator[List[Tuple[str, str]]]:
+        """جملات پیکره را به شکل متن خام برمی‌گرداند.
+
+        Yields:
+            جملهٔ بعدی.
+
+        """
+        sentence = []
+        with Path(self._bijankhan_file).open(encoding="utf-8") as f:
+            length = 2
+            for line in f:
+                parts = re.split("  +", line.strip())
+                if len(parts) == length:
+                    word, tag = parts
+                    if word not in ("#", "*"):
+                        word = self._normalizer.normalize(word)
+                        sentence.append((word if word else "_", tag))
+                    if (
+                        tag == "DELM"
+                        and word in ("#", "*", ".", "؟", "!")
+                        and len(sentence)
+                    ):
+                        yield sentence
+                        sentence = []
+
+    def sents(self: "BijankhanReader") -> Iterator[List[Tuple[str, str]]]:
+        """جملات پیکره را به شکل لیستی از `(توکن،برچسب)`ها برمی‌گرداند..
+
+        Examples:
+            >>> bijankhan = BijankhanReader(bijankhan_file='corpora/bijankhan.txt')
+            >>> next(bijankhan.sents())
+            [('اولین', 'ADJ'), ('سیاره', 'N'), ('خارج', 'ADJ'), ('از', 'PREP'), ('منظومه', 'N'), ('شمسی', 'ADJ'), ('دیده_شد', 'V'), ('.', 'PUNC')]
+
+        Yields:
+            جملهٔ بعدی در قالب لیستی از `(توکن،برچسب)`ها.
+
+        """
+
+        def map_poses(item: Tuple[str, str]) -> Tuple[str, str]:
+            return (item[0], self._pos_map.get(item[1], item[1]))
+
+        for sentence in self._sentences():
+            if self._joined_verb_parts:
+                sentence = join_verb_parts(sentence)
+            yield list(map(map_poses, sentence))
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/dadegan_reader.py` & `hazm-0.9.1/hazm/corpus_readers/dadegan_reader.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,414 +1,414 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ PerDT است.
-
-PerDT حاوی تعداد قابل‌توجهی جملۀ برچسب‌خورده با اطلاعات نحوی و ساخت‌واژی است.
-
-"""
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import Iterator
-from typing import List
-from typing import Tuple
-from typing import Type
-
-from nltk.parse import DependencyGraph
-from nltk.tree import Tree
-
-
-def coarse_pos_u(tags: List[str], word: str) -> str:
-    """برچسب‌های ریز را به برچسب‌های درشت منطبق با استاندارد جهانی (coarse-grained
-    universal pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_e(['N', 'IANM'], 'امروز')
-        'N'
-
-    """
-    mapping = {
-        "N": "NOUN",
-        "V": "VERB",
-        "ADJ": "ADJ",
-        "ADV": "ADV",
-        "PR": "PRON",
-        "PREM": "DET",
-        "PREP": "ADP",
-        "POSTP": "ADP",
-        "PRENUM": "NUM",
-        "CONJ": "CCONJ",
-        "PUNC": "PUNCT",
-        "SUBR": "SCONJ",
-        "IDEN": "PROPN",
-        "POSTNUM": "NUM",
-        "PSUS": "INTJ",
-        "PART": "PART",
-        "ADR": "INTJ",
-    }
-    pos_mapped = mapping.get(tags[0], "X")
-    if pos_mapped == "PART" and word == "را":
-        return "ADP"
-    if pos_mapped == "PART" and word in ["خوب", "آخر"]:
-        return "ADP"
-    return pos_mapped
-
-
-def coarse_pos_e(tags: List[str], word) -> str:
-    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_e(['N', 'IANM'],'امروز')
-        'N'
-
-    """
-    mapping = {
-        "N": "N",
-        "V": "V",
-        "ADJ": "AJ",
-        "ADV": "ADV",
-        "PR": "PRO",
-        "PREM": "DET",
-        "PREP": "P",
-        "POSTP": "POSTP",
-        "PRENUM": "NUM",
-        "CONJ": "CONJ",
-        "PUNC": "PUNC",
-        "SUBR": "CONJ",
-    }
-    return mapping.get(tags[0], "X") + ("e" if "EZ" in tags else "")
-
-
-def word_nodes(tree: Type[Tree]) -> List[Dict[str, Any]]:
-    """نودها را به صورت مرتب‌شده برمی‌گرداند."""
-    return sorted(tree.nodes.values(), key=lambda node: node["address"])[1:]
-
-
-def node_deps(node: List[Dict[str, Any]]) -> List[Any]:
-    """مقادیر موجود در فیلد deps نود ورودی را برمی‌گرداند."""
-    return sum(list(node["deps"].values()), [])
-
-
-class DadeganReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ PerDT است.
-
-    Args:
-        conll_file: مسیر فایلِ پیکره.
-        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
-
-    """
-
-    def __init__(
-        self: "DadeganReader",
-        conll_file: str,
-        pos_map: str = coarse_pos_e,
-        universal_pos: bool = False,
-    ) -> None:
-        self._conll_file = conll_file
-        if pos_map is None:
-            self._pos_map = lambda tags: ",".join(tags)
-        elif universal_pos:
-            self._pos_map = coarse_pos_u
-        else:
-            self._pos_map = coarse_pos_e
-
-    def _sentences(self: "DadeganReader") -> Iterator[str]:
-        """جملات پیکره را به شکل متن خام برمی‌گرداند.
-
-        Yields:
-            جملهٔ بعدی.
-
-        """
-        with Path(self._conll_file).open(encoding="utf8") as conll_file:
-            text = conll_file.read()
-
-            # refine text
-            text = (
-                text.replace("‌‌", "‌")
-                .replace("\t‌", "\t")
-                .replace("‌\t", "\t")
-                .replace("\t ", "\t")
-                .replace(" \t", "\t")
-                .replace("\r", "")
-                .replace("\u2029", "‌")
-            )
-
-            for item in text.replace(" ", "_").split("\n\n"):
-                if item.strip():
-                    yield item
-
-    def trees(self: "DadeganReader") -> Iterator[Type[Tree]]:
-        """ساختار درختی جملات را برمی‌گرداند.
-
-        Yields:
-            ساختار درختی جملهٔ بعدی.
-
-        """
-        for sentence in self._sentences():
-            tree = DependencyGraph(sentence)
-
-            for node in word_nodes(tree):
-                node["mtag"] = [node["ctag"], node["tag"]]
-
-                if "ezafe" in node["feats"]:
-                    node["mtag"].append("EZ")
-
-                node["mtag"] = self._pos_map(node["mtag"], node["word"])
-
-            yield tree
-
-    def sents(self: "DadeganReader") -> Iterator[List[Tuple[str, str]]]:
-        """لیستی از جملات را برمی‌گرداند.
-
-        هر جمله لیستی از `(توکن، برچسب)`ها است.
-
-        Examples:
-            >>> dadegan = DadeganReader(conll_file='corpora/dadegan.conll')
-            >>> next(dadegan.sents())
-            [('این', 'DET'), ('میهمانی', 'N'), ('به', 'P'), ('منظور', 'Ne'), ('آشنایی', 'Ne'), ('هم‌تیمی‌های', 'Ne'), ('او', 'PRO'), ('با', 'P'), ('غذاهای', 'Ne'), ('ایرانی', 'AJ'), ('ترتیب', 'N'), ('داده_شد', 'V'), ('.', 'PUNC')]
-
-        Yields:
-            جملهٔ بعدی.
-
-        """
-        for tree in self.trees():
-            yield [(node["word"], node["mtag"]) for node in word_nodes(tree)]
-
-    def chunked_trees(self: "DadeganReader") -> Iterator[Type[Tree]]:
-        """درخت وابستگی‌های جملات را برمی‌گرداند.
-
-        Examples:
-            >>> from hazm.chunker import tree2brackets
-            >>> dadegan = DadeganReader(conll_file='corpora/dadegan.conll')
-            >>> tree2brackets(next(dadegan.chunked_trees()))
-            '[این میهمانی NP] [به PP] [منظور آشنایی هم‌تیمی‌های او NP] [با PP] [غذاهای ایرانی NP] [ترتیب داده_شد VP] .'
-
-        Yields:
-            درخت وابستگی‌های جملهٔ بعدی.
-
-        """
-        for tree in self.trees():
-            chunks = []
-            for node in word_nodes(tree):
-                n = node["address"]
-                item = (node["word"], node["mtag"])
-                appended = False
-                if node["ctag"] in {"PREP", "POSTP"}:
-                    for d in node_deps(node):
-                        label = "PP"
-                        if node["ctag"] == "POSTP":
-                            label = "POSTP"
-                        if (
-                            d == n - 1
-                            and type(chunks[-1]) == Tree
-                            and chunks[-1].label() == label
-                        ):
-                            chunks[-1].append(item)
-                            appended = True
-                    if (
-                        node["head"] == n - 1
-                        and len(chunks) > 0
-                        and type(chunks[-1]) == Tree
-                        and chunks[-1].label() == label
-                    ):
-                        chunks[-1].append(item)
-                        appended = True
-                    if not appended:
-                        chunks.append(Tree(label, [item]))
-                elif node["ctag"] in {"PUNC", "CONJ", "SUBR", "PART"}:
-                    if (
-                        item[0]
-                        in {"'", '"', "(", ")", "{", "}", "[", "]", "-", "#", "«", "»"}
-                        and len(chunks) > 0
-                        and type(chunks[-1]) == Tree
-                    ):
-                        for leaf in chunks[-1].leaves():
-                            if leaf[1] == item[1]:
-                                chunks[-1].append(item)
-                                appended = True
-                                break
-                    if appended is not True:
-                        chunks.append(item)
-                elif node["ctag"] in {
-                    "N",
-                    "PREM",
-                    "ADJ",
-                    "PR",
-                    "ADR",
-                    "PRENUM",
-                    "IDEN",
-                    "POSNUM",
-                    "SADV",
-                }:
-                    if node["rel"] in {"MOZ", "NPOSTMOD"}:
-                        if len(chunks) > 0:
-                            if type(chunks[-1]) == Tree:
-                                j = n - len(chunks[-1].leaves())
-                                chunks[-1].append(item)
-                            else:
-                                j = n - 1
-                                treenode = Tree("NP", [chunks.pop(), item])
-                                chunks.append(treenode)
-                            while j > node["head"]:
-                                leaves = chunks.pop().leaves()
-                                if len(chunks) < 1:
-                                    chunks.append(Tree("NP", leaves))
-                                    j -= 1
-                                elif type(chunks[-1]) == Tree:
-                                    j -= len(chunks[-1])
-                                    for leaf in leaves:
-                                        chunks[-1].append(leaf)
-                                else:
-                                    leaves.insert(0, chunks.pop())
-                                    chunks.append(Tree("NP", leaves))
-                                    j -= 1
-                            continue
-                    elif node["rel"] == "POSDEP" and tree.nodes[node["head"]][
-                        "rel"
-                    ] in {"NCONJ", "AJCONJ"}:
-                        conj = tree.nodes[node["head"]]
-                        if tree.nodes[conj["head"]]["rel"] in {
-                            "MOZ",
-                            "NPOSTMOD",
-                            "AJCONJ",
-                            "POSDEP",
-                        }:
-                            label = "NP"
-                            leaves = [item]
-                            j = n - 1
-                            while j >= conj["head"]:
-                                if type(chunks[-1]) is Tree:
-                                    j -= len(chunks[-1].leaves())
-                                    label = chunks[-1].label()
-                                    leaves = chunks.pop().leaves() + leaves
-                                else:
-                                    leaves.insert(0, chunks.pop())
-                                    j -= 1
-                            chunks.append(Tree(label, leaves))
-                            appended = True
-                    elif (
-                        node["head"] == n - 1
-                        and len(chunks) > 0
-                        and type(chunks[-1]) == Tree
-                        and chunks[-1].label() != "PP"
-                    ):
-                        chunks[-1].append(item)
-                        appended = True
-                    elif node["rel"] == "AJCONJ" and tree.nodes[node["head"]][
-                        "rel"
-                    ] in {"NPOSTMOD", "AJCONJ"}:
-                        np_nodes = [item]
-                        label = "ADJP"
-                        i = n - node["head"]
-                        while i > 0:
-                            if type(chunks[-1]) == Tree:
-                                label = chunks[-1].label()
-                                leaves = chunks.pop().leaves()
-                                i -= len(leaves)
-                                np_nodes = leaves + np_nodes
-                            else:
-                                i -= 1
-                                np_nodes.insert(0, chunks.pop())
-                        chunks.append(Tree(label, np_nodes))
-                        appended = True
-                    elif (
-                        node["ctag"] == "ADJ"
-                        and node["rel"] == "POSDEP"
-                        and tree.nodes[node["head"]]["ctag"] != "CONJ"
-                    ):
-                        np_nodes = [item]
-                        i = n - node["head"]
-                        while i > 0:
-                            label = "ADJP"
-                            if type(chunks[-1]) == Tree:
-                                label = chunks[-1].label()
-                                leaves = chunks.pop().leaves()
-                                i -= len(leaves)
-                                np_nodes = leaves + np_nodes
-                            else:
-                                i -= 1
-                                np_nodes.insert(0, chunks.pop())
-                        chunks.append(Tree(label, np_nodes))
-                        appended = True
-                    for d in node_deps(node):
-                        if (
-                            d == n - 1
-                            and type(chunks[-1]) == Tree
-                            and chunks[-1].label() != "PP"
-                            and appended is not True
-                        ):
-                            label = chunks[-1].label()
-                            if node["rel"] == "ADV":
-                                label = "ADVP"
-                            elif label in {"ADJP", "ADVP"}:
-                                if node["ctag"] == "N":
-                                    label = "NP"
-                                elif node["ctag"] == "ADJ":
-                                    label = "ADJP"
-                            leaves = chunks.pop().leaves()
-                            leaves.append(item)
-                            chunks.append(Tree(label, leaves))
-                            appended = True
-                        elif tree.nodes[d]["rel"] == "NPREMOD" and appended is not True:
-                            np_nodes = [item]
-                            i = n - d
-                            while i > 0:
-                                if type(chunks[-1]) == Tree:
-                                    leaves = chunks.pop().leaves()
-                                    i -= len(leaves)
-                                    np_nodes = leaves + np_nodes
-                                else:
-                                    i -= 1
-                                    np_nodes.insert(0, chunks.pop())
-                            chunks.append(Tree("NP", np_nodes))
-                            appended = True
-                    if not appended:
-                        label = "NP"
-                        if node["ctag"] == "ADJ":
-                            label = "ADJP"
-                        elif node["rel"] == "ADV":
-                            label = "ADVP"
-                        chunks.append(Tree(label, [item]))
-                elif node["ctag"] in {"V"}:
-                    appended = False
-                    for d in node_deps(node):
-                        if (
-                            d == n - 1
-                            and type(chunks[-1]) == Tree
-                            and tree.nodes[d]["rel"] in {"NVE", "ENC"}
-                            and appended is not True
-                        ):
-                            leaves = chunks.pop().leaves()
-                            leaves.append(item)
-                            chunks.append(Tree("VP", leaves))
-                            appended = True
-                        elif tree.nodes[d]["rel"] in {"VPRT", "NVE"}:
-                            vp_nodes = [item]
-                            i = n - d
-                            while i > 0:
-                                if type(chunks[-1]) == Tree:
-                                    leaves = chunks.pop().leaves()
-                                    i -= len(leaves)
-                                    vp_nodes = leaves + vp_nodes
-                                else:
-                                    i -= 1
-                                    vp_nodes.insert(0, chunks.pop())
-                            chunks.append(Tree("VP", vp_nodes))
-                            appended = True
-                            break
-                    if not appended:
-                        chunks.append(Tree("VP", [item]))
-                elif node["ctag"] in {"PSUS"}:
-                    if node["rel"] == "ADV":
-                        chunks.append(Tree("ADVP", [item]))
-                    else:
-                        chunks.append(Tree("VP", [item]))
-                elif node["ctag"] in {"ADV", "SADV"}:
-                    appended = False
-                    for d in node_deps(node):
-                        if d == n - 1 and type(chunks[-1]) == Tree:
-                            leaves = chunks.pop().leaves()
-                            leaves.append(item)
-                            chunks.append(Tree("ADVP", leaves))
-                            appended = True
-                    if not appended:
-                        chunks.append(Tree("ADVP", [item]))
-
-            yield Tree("S", chunks)
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ PerDT است.
+
+PerDT حاوی تعداد قابل‌توجهی جملۀ برچسب‌خورده با اطلاعات نحوی و ساخت‌واژی است.
+
+"""
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import Iterator
+from typing import List
+from typing import Tuple
+from typing import Type
+
+from nltk.parse import DependencyGraph
+from nltk.tree import Tree
+
+
+def coarse_pos_u(tags: List[str], word: str) -> str:
+    """برچسب‌های ریز را به برچسب‌های درشت منطبق با استاندارد جهانی (coarse-grained
+    universal pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_e(['N', 'IANM'], 'امروز')
+        'N'
+
+    """
+    mapping = {
+        "N": "NOUN",
+        "V": "VERB",
+        "ADJ": "ADJ",
+        "ADV": "ADV",
+        "PR": "PRON",
+        "PREM": "DET",
+        "PREP": "ADP",
+        "POSTP": "ADP",
+        "PRENUM": "NUM",
+        "CONJ": "CCONJ",
+        "PUNC": "PUNCT",
+        "SUBR": "SCONJ",
+        "IDEN": "PROPN",
+        "POSTNUM": "NUM",
+        "PSUS": "INTJ",
+        "PART": "PART",
+        "ADR": "INTJ",
+    }
+    pos_mapped = mapping.get(tags[0], "X")
+    if pos_mapped == "PART" and word == "را":
+        return "ADP"
+    if pos_mapped == "PART" and word in ["خوب", "آخر"]:
+        return "ADP"
+    return pos_mapped
+
+
+def coarse_pos_e(tags: List[str], word) -> str:
+    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_e(['N', 'IANM'],'امروز')
+        'N'
+
+    """
+    mapping = {
+        "N": "N",
+        "V": "V",
+        "ADJ": "AJ",
+        "ADV": "ADV",
+        "PR": "PRO",
+        "PREM": "DET",
+        "PREP": "P",
+        "POSTP": "POSTP",
+        "PRENUM": "NUM",
+        "CONJ": "CONJ",
+        "PUNC": "PUNC",
+        "SUBR": "CONJ",
+    }
+    return mapping.get(tags[0], "X") + ("e" if "EZ" in tags else "")
+
+
+def word_nodes(tree: Type[Tree]) -> List[Dict[str, Any]]:
+    """نودها را به صورت مرتب‌شده برمی‌گرداند."""
+    return sorted(tree.nodes.values(), key=lambda node: node["address"])[1:]
+
+
+def node_deps(node: List[Dict[str, Any]]) -> List[Any]:
+    """مقادیر موجود در فیلد deps نود ورودی را برمی‌گرداند."""
+    return sum(list(node["deps"].values()), [])
+
+
+class DadeganReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ PerDT است.
+
+    Args:
+        conll_file: مسیر فایلِ پیکره.
+        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
+
+    """
+
+    def __init__(
+        self: "DadeganReader",
+        conll_file: str,
+        pos_map: str = coarse_pos_e,
+        universal_pos: bool = False,
+    ) -> None:
+        self._conll_file = conll_file
+        if pos_map is None:
+            self._pos_map = lambda tags: ",".join(tags)
+        elif universal_pos:
+            self._pos_map = coarse_pos_u
+        else:
+            self._pos_map = coarse_pos_e
+
+    def _sentences(self: "DadeganReader") -> Iterator[str]:
+        """جملات پیکره را به شکل متن خام برمی‌گرداند.
+
+        Yields:
+            جملهٔ بعدی.
+
+        """
+        with Path(self._conll_file).open(encoding="utf8") as conll_file:
+            text = conll_file.read()
+
+            # refine text
+            text = (
+                text.replace("‌‌", "‌")
+                .replace("\t‌", "\t")
+                .replace("‌\t", "\t")
+                .replace("\t ", "\t")
+                .replace(" \t", "\t")
+                .replace("\r", "")
+                .replace("\u2029", "‌")
+            )
+
+            for item in text.replace(" ", "_").split("\n\n"):
+                if item.strip():
+                    yield item
+
+    def trees(self: "DadeganReader") -> Iterator[Type[Tree]]:
+        """ساختار درختی جملات را برمی‌گرداند.
+
+        Yields:
+            ساختار درختی جملهٔ بعدی.
+
+        """
+        for sentence in self._sentences():
+            tree = DependencyGraph(sentence)
+
+            for node in word_nodes(tree):
+                node["mtag"] = [node["ctag"], node["tag"]]
+
+                if "ezafe" in node["feats"]:
+                    node["mtag"].append("EZ")
+
+                node["mtag"] = self._pos_map(node["mtag"], node["word"])
+
+            yield tree
+
+    def sents(self: "DadeganReader") -> Iterator[List[Tuple[str, str]]]:
+        """لیستی از جملات را برمی‌گرداند.
+
+        هر جمله لیستی از `(توکن، برچسب)`ها است.
+
+        Examples:
+            >>> dadegan = DadeganReader(conll_file='corpora/dadegan.conll')
+            >>> next(dadegan.sents())
+            [('این', 'DET'), ('میهمانی', 'N'), ('به', 'P'), ('منظور', 'Ne'), ('آشنایی', 'Ne'), ('هم‌تیمی‌های', 'Ne'), ('او', 'PRO'), ('با', 'P'), ('غذاهای', 'Ne'), ('ایرانی', 'AJ'), ('ترتیب', 'N'), ('داده_شد', 'V'), ('.', 'PUNC')]
+
+        Yields:
+            جملهٔ بعدی.
+
+        """
+        for tree in self.trees():
+            yield [(node["word"], node["mtag"]) for node in word_nodes(tree)]
+
+    def chunked_trees(self: "DadeganReader") -> Iterator[Type[Tree]]:
+        """درخت وابستگی‌های جملات را برمی‌گرداند.
+
+        Examples:
+            >>> from hazm.chunker import tree2brackets
+            >>> dadegan = DadeganReader(conll_file='corpora/dadegan.conll')
+            >>> tree2brackets(next(dadegan.chunked_trees()))
+            '[این میهمانی NP] [به PP] [منظور آشنایی هم‌تیمی‌های او NP] [با PP] [غذاهای ایرانی NP] [ترتیب داده_شد VP] .'
+
+        Yields:
+            درخت وابستگی‌های جملهٔ بعدی.
+
+        """
+        for tree in self.trees():
+            chunks = []
+            for node in word_nodes(tree):
+                n = node["address"]
+                item = (node["word"], node["mtag"])
+                appended = False
+                if node["ctag"] in {"PREP", "POSTP"}:
+                    for d in node_deps(node):
+                        label = "PP"
+                        if node["ctag"] == "POSTP":
+                            label = "POSTP"
+                        if (
+                            d == n - 1
+                            and type(chunks[-1]) == Tree
+                            and chunks[-1].label() == label
+                        ):
+                            chunks[-1].append(item)
+                            appended = True
+                    if (
+                        node["head"] == n - 1
+                        and len(chunks) > 0
+                        and type(chunks[-1]) == Tree
+                        and chunks[-1].label() == label
+                    ):
+                        chunks[-1].append(item)
+                        appended = True
+                    if not appended:
+                        chunks.append(Tree(label, [item]))
+                elif node["ctag"] in {"PUNC", "CONJ", "SUBR", "PART"}:
+                    if (
+                        item[0]
+                        in {"'", '"', "(", ")", "{", "}", "[", "]", "-", "#", "«", "»"}
+                        and len(chunks) > 0
+                        and type(chunks[-1]) == Tree
+                    ):
+                        for leaf in chunks[-1].leaves():
+                            if leaf[1] == item[1]:
+                                chunks[-1].append(item)
+                                appended = True
+                                break
+                    if appended is not True:
+                        chunks.append(item)
+                elif node["ctag"] in {
+                    "N",
+                    "PREM",
+                    "ADJ",
+                    "PR",
+                    "ADR",
+                    "PRENUM",
+                    "IDEN",
+                    "POSNUM",
+                    "SADV",
+                }:
+                    if node["rel"] in {"MOZ", "NPOSTMOD"}:
+                        if len(chunks) > 0:
+                            if type(chunks[-1]) == Tree:
+                                j = n - len(chunks[-1].leaves())
+                                chunks[-1].append(item)
+                            else:
+                                j = n - 1
+                                treenode = Tree("NP", [chunks.pop(), item])
+                                chunks.append(treenode)
+                            while j > node["head"]:
+                                leaves = chunks.pop().leaves()
+                                if len(chunks) < 1:
+                                    chunks.append(Tree("NP", leaves))
+                                    j -= 1
+                                elif type(chunks[-1]) == Tree:
+                                    j -= len(chunks[-1])
+                                    for leaf in leaves:
+                                        chunks[-1].append(leaf)
+                                else:
+                                    leaves.insert(0, chunks.pop())
+                                    chunks.append(Tree("NP", leaves))
+                                    j -= 1
+                            continue
+                    elif node["rel"] == "POSDEP" and tree.nodes[node["head"]][
+                        "rel"
+                    ] in {"NCONJ", "AJCONJ"}:
+                        conj = tree.nodes[node["head"]]
+                        if tree.nodes[conj["head"]]["rel"] in {
+                            "MOZ",
+                            "NPOSTMOD",
+                            "AJCONJ",
+                            "POSDEP",
+                        }:
+                            label = "NP"
+                            leaves = [item]
+                            j = n - 1
+                            while j >= conj["head"]:
+                                if type(chunks[-1]) is Tree:
+                                    j -= len(chunks[-1].leaves())
+                                    label = chunks[-1].label()
+                                    leaves = chunks.pop().leaves() + leaves
+                                else:
+                                    leaves.insert(0, chunks.pop())
+                                    j -= 1
+                            chunks.append(Tree(label, leaves))
+                            appended = True
+                    elif (
+                        node["head"] == n - 1
+                        and len(chunks) > 0
+                        and type(chunks[-1]) == Tree
+                        and chunks[-1].label() != "PP"
+                    ):
+                        chunks[-1].append(item)
+                        appended = True
+                    elif node["rel"] == "AJCONJ" and tree.nodes[node["head"]][
+                        "rel"
+                    ] in {"NPOSTMOD", "AJCONJ"}:
+                        np_nodes = [item]
+                        label = "ADJP"
+                        i = n - node["head"]
+                        while i > 0:
+                            if type(chunks[-1]) == Tree:
+                                label = chunks[-1].label()
+                                leaves = chunks.pop().leaves()
+                                i -= len(leaves)
+                                np_nodes = leaves + np_nodes
+                            else:
+                                i -= 1
+                                np_nodes.insert(0, chunks.pop())
+                        chunks.append(Tree(label, np_nodes))
+                        appended = True
+                    elif (
+                        node["ctag"] == "ADJ"
+                        and node["rel"] == "POSDEP"
+                        and tree.nodes[node["head"]]["ctag"] != "CONJ"
+                    ):
+                        np_nodes = [item]
+                        i = n - node["head"]
+                        while i > 0:
+                            label = "ADJP"
+                            if type(chunks[-1]) == Tree:
+                                label = chunks[-1].label()
+                                leaves = chunks.pop().leaves()
+                                i -= len(leaves)
+                                np_nodes = leaves + np_nodes
+                            else:
+                                i -= 1
+                                np_nodes.insert(0, chunks.pop())
+                        chunks.append(Tree(label, np_nodes))
+                        appended = True
+                    for d in node_deps(node):
+                        if (
+                            d == n - 1
+                            and type(chunks[-1]) == Tree
+                            and chunks[-1].label() != "PP"
+                            and appended is not True
+                        ):
+                            label = chunks[-1].label()
+                            if node["rel"] == "ADV":
+                                label = "ADVP"
+                            elif label in {"ADJP", "ADVP"}:
+                                if node["ctag"] == "N":
+                                    label = "NP"
+                                elif node["ctag"] == "ADJ":
+                                    label = "ADJP"
+                            leaves = chunks.pop().leaves()
+                            leaves.append(item)
+                            chunks.append(Tree(label, leaves))
+                            appended = True
+                        elif tree.nodes[d]["rel"] == "NPREMOD" and appended is not True:
+                            np_nodes = [item]
+                            i = n - d
+                            while i > 0:
+                                if type(chunks[-1]) == Tree:
+                                    leaves = chunks.pop().leaves()
+                                    i -= len(leaves)
+                                    np_nodes = leaves + np_nodes
+                                else:
+                                    i -= 1
+                                    np_nodes.insert(0, chunks.pop())
+                            chunks.append(Tree("NP", np_nodes))
+                            appended = True
+                    if not appended:
+                        label = "NP"
+                        if node["ctag"] == "ADJ":
+                            label = "ADJP"
+                        elif node["rel"] == "ADV":
+                            label = "ADVP"
+                        chunks.append(Tree(label, [item]))
+                elif node["ctag"] in {"V"}:
+                    appended = False
+                    for d in node_deps(node):
+                        if (
+                            d == n - 1
+                            and type(chunks[-1]) == Tree
+                            and tree.nodes[d]["rel"] in {"NVE", "ENC"}
+                            and appended is not True
+                        ):
+                            leaves = chunks.pop().leaves()
+                            leaves.append(item)
+                            chunks.append(Tree("VP", leaves))
+                            appended = True
+                        elif tree.nodes[d]["rel"] in {"VPRT", "NVE"}:
+                            vp_nodes = [item]
+                            i = n - d
+                            while i > 0:
+                                if type(chunks[-1]) == Tree:
+                                    leaves = chunks.pop().leaves()
+                                    i -= len(leaves)
+                                    vp_nodes = leaves + vp_nodes
+                                else:
+                                    i -= 1
+                                    vp_nodes.insert(0, chunks.pop())
+                            chunks.append(Tree("VP", vp_nodes))
+                            appended = True
+                            break
+                    if not appended:
+                        chunks.append(Tree("VP", [item]))
+                elif node["ctag"] in {"PSUS"}:
+                    if node["rel"] == "ADV":
+                        chunks.append(Tree("ADVP", [item]))
+                    else:
+                        chunks.append(Tree("VP", [item]))
+                elif node["ctag"] in {"ADV", "SADV"}:
+                    appended = False
+                    for d in node_deps(node):
+                        if d == n - 1 and type(chunks[-1]) == Tree:
+                            leaves = chunks.pop().leaves()
+                            leaves.append(item)
+                            chunks.append(Tree("ADVP", leaves))
+                            appended = True
+                    if not appended:
+                        chunks.append(Tree("ADVP", [item]))
+
+            yield Tree("S", chunks)
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/degarbayan_reader.py` & `hazm-0.9.1/hazm/corpus_readers/degarbayan_reader.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ دِگَربیان است.
-
-[پیکرهٔ
-دگربیان](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-
-%D8%AF%DA%AF%D8%B1%D8%A8%DB%8C%D8%A7%D9%86) حاوی
-۱۵۲۳ نمونه است که به عنوان نمونه‌های دگربیان نشانه‌گذاری شده‌اند. جملات و
-عبارات
-دگربیان، بیانی متفاوت از مفهومی یکسان هستند. داده‌های این پیکره از خبرگزاری‌ها
-جمع‌آورده شده و در سه دسته‌بندی «دگربیان»، «تقریباً دگربیان» و «نامرتبط» ارائه
-می‌شوند. این داده‌ها با استفاده از همکاری جمعی در پیام‌رسان تلگرام نشانه‌گذاری
-شده است.
-
-"""
-
-
-import os
-import sys
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import Iterator
-from typing import Tuple
-from xml.dom import minidom
-
-
-class DegarbayanReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ دگربیان است.
-
-    Args:
-        root: مسیر فولدر حاوی فایل‌های پیکره
-        corpus_file: فایل اطلاعات پیکره.
-            در صورتی که بخواهید از حالت استاندارد پیکره استفاده کنید نیازی به تغییرِ این فایل نیست.
-        judge_type: این پارامتر دارای دو مقدار `three_class` و `two_class` است.
-            در حالت `three_class` جملات سه برچسب می‌خورند: ۱. `Paraphrase`(دگربیان)
-            ۲. `SemiParaphrase`(تقریباً دگربیان) ۳. `NotParaphrase`(غیر دگربیان). در حالت
-            `two_class` حالت دوم یعنی `SemiParaphrase` هم برچسب `Paraphrase` می‌خورَد.
-        version: شمارهٔ نسخهٔ پیکره
-
-    """
-
-    def __init__(
-        self: "DegarbayanReader",
-        root: str,
-        corpus_file: str = "corpus_pair.xml",
-        judge_type: str = "three_class",
-    ) -> None:
-        self._root = root
-        self._corpus_file = corpus_file
-        self._judge_type = judge_type
-        if judge_type != "three_class" and judge_type != "two_class":
-            self._judge_type = "three_class"
-
-    def docs(self: "DegarbayanReader") -> Iterator[Dict[str, Any]]:
-        """اسناد موجود در پیکره را برمی‌گرداند.
-
-        Yields:
-            سند بعدی.
-
-        """
-
-        def judge_number_to_text(judge: str) -> str:
-            if judge == "1" or (self._judge_type == "two_class" and judge == "0"):
-                return "Paraphrase"
-
-            if judge == "0":
-                return "SemiParaphrase"
-
-            return "NotParaphrase"
-
-        filename = os.path.join(self._root, self._corpus_file)
-        if os.path.exists(filename):
-            try:
-                elements = minidom.parse(filename)
-                for element in elements.getElementsByTagName("Pair"):
-                    pair = {
-                        "id": (
-                            element.getElementsByTagName("PairId")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "news_source1": (
-                            element.getElementsByTagName("NewsSource1")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "news_source2": (
-                            element.getElementsByTagName("NewsSource2")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "news_id1": (
-                            element.getElementsByTagName("NewsId1")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "news_id2": (
-                            element.getElementsByTagName("NewsId2")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "sentence1": (
-                            element.getElementsByTagName("Sentence1")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "sentence2": (
-                            element.getElementsByTagName("Sentence2")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "method_type": (
-                            element.getElementsByTagName("MethodType")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "judge": judge_number_to_text(
-                            element.getElementsByTagName("judge")[0]
-                            .childNodes[0]
-                            .data.strip(),
-                        ),
-                    }
-                    yield pair
-
-            except Exception as e:
-                print("error in reading", filename, e, file=sys.stderr)
-        else:
-            print("error in reading file", filename, e, file=sys.stderr)  # noqa: F821
-            msg = "error in reading file"
-            raise FileNotFoundError(msg, filename)
-
-    def pairs(self: "DegarbayanReader") -> Iterator[Tuple[str, str, str]]:
-        """متن‌های دگربیان را در قالب یک `(متن اصلی، شکل دگربیان، برچسب)` برمی‌گرداند.
-
-        Examples:
-            >>> degarbayan = DegarbayanReader(root='corpora/degarbayan')
-            >>> next(degarbayan.pairs())
-            ('24 نفر نهایی تیم ملی بدون تغییری خاص معرفی شد', 'کی روش 24 بازیکن را به تیم ملی فوتبال دعوت کرد', 'Paraphrase')
-
-        Yields:
-            `متن دگربیان بعدی در قالب یک `(متن اصلی، شکل دگربیان، برچسب).
-
-        """
-        for pair in self.docs():
-            yield pair["sentence1"], pair["sentence2"], pair["judge"]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ دِگَربیان است.
+
+[پیکرهٔ
+دگربیان](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-
+%D8%AF%DA%AF%D8%B1%D8%A8%DB%8C%D8%A7%D9%86) حاوی
+۱۵۲۳ نمونه است که به عنوان نمونه‌های دگربیان نشانه‌گذاری شده‌اند. جملات و
+عبارات
+دگربیان، بیانی متفاوت از مفهومی یکسان هستند. داده‌های این پیکره از خبرگزاری‌ها
+جمع‌آورده شده و در سه دسته‌بندی «دگربیان»، «تقریباً دگربیان» و «نامرتبط» ارائه
+می‌شوند. این داده‌ها با استفاده از همکاری جمعی در پیام‌رسان تلگرام نشانه‌گذاری
+شده است.
+
+"""
+
+
+import os
+import sys
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import Iterator
+from typing import Tuple
+from xml.dom import minidom
+
+
+class DegarbayanReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ دگربیان است.
+
+    Args:
+        root: مسیر فولدر حاوی فایل‌های پیکره
+        corpus_file: فایل اطلاعات پیکره.
+            در صورتی که بخواهید از حالت استاندارد پیکره استفاده کنید نیازی به تغییرِ این فایل نیست.
+        judge_type: این پارامتر دارای دو مقدار `three_class` و `two_class` است.
+            در حالت `three_class` جملات سه برچسب می‌خورند: ۱. `Paraphrase`(دگربیان)
+            ۲. `SemiParaphrase`(تقریباً دگربیان) ۳. `NotParaphrase`(غیر دگربیان). در حالت
+            `two_class` حالت دوم یعنی `SemiParaphrase` هم برچسب `Paraphrase` می‌خورَد.
+        version: شمارهٔ نسخهٔ پیکره
+
+    """
+
+    def __init__(
+        self: "DegarbayanReader",
+        root: str,
+        corpus_file: str = "corpus_pair.xml",
+        judge_type: str = "three_class",
+    ) -> None:
+        self._root = root
+        self._corpus_file = corpus_file
+        self._judge_type = judge_type
+        if judge_type != "three_class" and judge_type != "two_class":
+            self._judge_type = "three_class"
+
+    def docs(self: "DegarbayanReader") -> Iterator[Dict[str, Any]]:
+        """اسناد موجود در پیکره را برمی‌گرداند.
+
+        Yields:
+            سند بعدی.
+
+        """
+
+        def judge_number_to_text(judge: str) -> str:
+            if judge == "1" or (self._judge_type == "two_class" and judge == "0"):
+                return "Paraphrase"
+
+            if judge == "0":
+                return "SemiParaphrase"
+
+            return "NotParaphrase"
+
+        filename = os.path.join(self._root, self._corpus_file)
+        if os.path.exists(filename):
+            try:
+                elements = minidom.parse(filename)
+                for element in elements.getElementsByTagName("Pair"):
+                    pair = {
+                        "id": (
+                            element.getElementsByTagName("PairId")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "news_source1": (
+                            element.getElementsByTagName("NewsSource1")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "news_source2": (
+                            element.getElementsByTagName("NewsSource2")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "news_id1": (
+                            element.getElementsByTagName("NewsId1")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "news_id2": (
+                            element.getElementsByTagName("NewsId2")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "sentence1": (
+                            element.getElementsByTagName("Sentence1")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "sentence2": (
+                            element.getElementsByTagName("Sentence2")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "method_type": (
+                            element.getElementsByTagName("MethodType")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "judge": judge_number_to_text(
+                            element.getElementsByTagName("judge")[0]
+                            .childNodes[0]
+                            .data.strip(),
+                        ),
+                    }
+                    yield pair
+
+            except Exception as e:
+                print("error in reading", filename, e, file=sys.stderr)
+        else:
+            print("error in reading file", filename, e, file=sys.stderr)  # noqa: F821
+            msg = "error in reading file"
+            raise FileNotFoundError(msg, filename)
+
+    def pairs(self: "DegarbayanReader") -> Iterator[Tuple[str, str, str]]:
+        """متن‌های دگربیان را در قالب یک `(متن اصلی، شکل دگربیان، برچسب)` برمی‌گرداند.
+
+        Examples:
+            >>> degarbayan = DegarbayanReader(root='corpora/degarbayan')
+            >>> next(degarbayan.pairs())
+            ('24 نفر نهایی تیم ملی بدون تغییری خاص معرفی شد', 'کی روش 24 بازیکن را به تیم ملی فوتبال دعوت کرد', 'Paraphrase')
+
+        Yields:
+            `متن دگربیان بعدی در قالب یک `(متن اصلی، شکل دگربیان، برچسب).
+
+        """
+        for pair in self.docs():
+            yield pair["sentence1"], pair["sentence2"], pair["judge"]
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/mirastext_reader.py` & `hazm-0.9.1/hazm/corpus_readers/mirastext_reader.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ میراث است.
-
-[پیکرهٔ میراث](https://github.com/miras-tech/MirasText) حاوی ۲,۸۳۵,۴۱۴ خبر از
-۲۵۰ خبرگزاری فارسی است.
-
-"""
-from pathlib import Path
-from typing import Dict
-from typing import Iterator
-
-
-class MirasTextReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ میراث است.
-
-    Args:
-        filename: مسیر فایلِ پیکره.
-
-    """
-
-    def __init__(self: "MirasTextReader", filename: str) -> None:
-        self._filename = filename
-
-    def docs(self: "MirasTextReader") -> Iterator[Dict[str, str]]:
-        """خبرها را برمی‌گرداند.
-
-        Yields:
-            خبر بعدی.
-
-        """
-        for line in Path(self._filename).open(encoding="utf-8"):
-            parts = line.split("***")
-            # todo: extract link, tags, ...
-            yield {"text": parts[0].strip()}
-
-    def texts(self: "MirasTextReader") -> Iterator[str]:
-        """فقط متن خبرها را برمی‌گرداند.
-
-        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با تابع
-        ‍[docs()][hazm.corpus_readers.mirastext_reader.MirasTextReader.docs] و دریافت مقدار
-        پراپرتی `text` نیز می‌توانید همین کار را انجام دهید.
-
-        Examples:
-            >>> mirastext = MirasTextReader(filename='corpora/mirastext.txt')
-            >>> next(mirastext.texts())[:42]  # first 42 characters of fitst text
-            'ایرانی‌ها چقدر از اینترنت استفاده می‌کنند؟'
-
-        Yields:
-            : متنِ خبر بعدی.
-
-        """
-        for doc in self.docs():
-            yield doc["text"]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ میراث است.
+
+[پیکرهٔ میراث](https://github.com/miras-tech/MirasText) حاوی ۲,۸۳۵,۴۱۴ خبر از
+۲۵۰ خبرگزاری فارسی است.
+
+"""
+from pathlib import Path
+from typing import Dict
+from typing import Iterator
+
+
+class MirasTextReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ میراث است.
+
+    Args:
+        filename: مسیر فایلِ پیکره.
+
+    """
+
+    def __init__(self: "MirasTextReader", filename: str) -> None:
+        self._filename = filename
+
+    def docs(self: "MirasTextReader") -> Iterator[Dict[str, str]]:
+        """خبرها را برمی‌گرداند.
+
+        Yields:
+            خبر بعدی.
+
+        """
+        for line in Path(self._filename).open(encoding="utf-8"):
+            parts = line.split("***")
+            # todo: extract link, tags, ...
+            yield {"text": parts[0].strip()}
+
+    def texts(self: "MirasTextReader") -> Iterator[str]:
+        """فقط متن خبرها را برمی‌گرداند.
+
+        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با تابع
+        ‍[docs()][hazm.corpus_readers.mirastext_reader.MirasTextReader.docs] و دریافت مقدار
+        پراپرتی `text` نیز می‌توانید همین کار را انجام دهید.
+
+        Examples:
+            >>> mirastext = MirasTextReader(filename='corpora/mirastext.txt')
+            >>> next(mirastext.texts())[:42]  # first 42 characters of fitst text
+            'ایرانی‌ها چقدر از اینترنت استفاده می‌کنند؟'
+
+        Yields:
+            : متنِ خبر بعدی.
+
+        """
+        for doc in self.docs():
+            yield doc["text"]
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/persian_plain_text_reader.py` & `hazm-0.9.1/hazm/corpus_readers/persian_plain_text_reader.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""این ماژول، پیکره‌های متنی خام را می‌خواند."""
-from typing import Any
-from typing import Callable
-from typing import List
-
-from nltk.corpus import PlaintextCorpusReader
-from nltk.corpus.reader import StreamBackedCorpusView
-from nltk.corpus.reader import read_blankline_block
-
-from hazm import SentenceTokenizer
-from hazm import WordTokenizer
-
-
-class PersianPlainTextReader(PlaintextCorpusReader):
-    """Reader for corpora that consist of plaintext documents.  Paragraphs
-    are assumed to be split using blank lines.  Sentences and words can
-    be tokenized using the default tokenizers, or by custom tokenizers
-    specificed as parameters to the constructor.
-
-    """
-
-    CorpusView = StreamBackedCorpusView
-
-    def __init__(
-        self: "PersianPlainTextReader",
-        root: str,
-        fileids: List,
-        word_tokenizer: Callable = WordTokenizer.tokenize,
-        sent_tokenizer: Callable = SentenceTokenizer.tokenize,
-        para_block_reader: Callable = read_blankline_block,
-        encoding: str = "utf8",
-    ) -> None:
-        super().__init__(
-            root,
-            fileids,
-            word_tokenizer,
-            sent_tokenizer,
-            para_block_reader,
-            encoding,
-        )
+"""این ماژول، پیکره‌های متنی خام را می‌خواند."""
+from typing import Any
+from typing import Callable
+from typing import List
+
+from nltk.corpus import PlaintextCorpusReader
+from nltk.corpus.reader import StreamBackedCorpusView
+from nltk.corpus.reader import read_blankline_block
+
+from hazm import SentenceTokenizer
+from hazm import WordTokenizer
+
+
+class PersianPlainTextReader(PlaintextCorpusReader):
+    """Reader for corpora that consist of plaintext documents.  Paragraphs
+    are assumed to be split using blank lines.  Sentences and words can
+    be tokenized using the default tokenizers, or by custom tokenizers
+    specificed as parameters to the constructor.
+
+    """
+
+    CorpusView = StreamBackedCorpusView
+
+    def __init__(
+        self: "PersianPlainTextReader",
+        root: str,
+        fileids: List,
+        word_tokenizer: Callable = WordTokenizer.tokenize,
+        sent_tokenizer: Callable = SentenceTokenizer.tokenize,
+        para_block_reader: Callable = read_blankline_block,
+        encoding: str = "utf8",
+    ) -> None:
+        super().__init__(
+            root,
+            fileids,
+            word_tokenizer,
+            sent_tokenizer,
+            para_block_reader,
+            encoding,
+        )
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/persica_reader.py` & `hazm-0.9.1/hazm/corpus_readers/persica_reader.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ پرسیکا است.
-
-[پیکرهٔ پرسیکا](https://www.peykaregan.ir/dataset/%D9%BE%D8%B1%D8%B3%DB%8C%DA%A
-9%D8%A7-%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-%D9%85%D8%AA%D9%88%D9%86-
-%D8%AE%D8%A8%D8%B1%DB%8C) حاوی
-خبرهای برگرفته از خبرگزاری ایسنا در یازده دستهٔ ورزشی، اقتصادی، فرهنگی، مذهبی،
-تاریخی، سیاسی، علمی، اجتماعی، آموزشی، حقوق قضایی و بهداشت است. روی این داده‌ها
-پیش‌پردازش‌هایی صورت شده و آمادهٔ استفاده در کاربردهای مختلف پردازش زبان طبیعی
-و
-داده‌کاوی است.
-
-"""
-from pathlib import Path
-from typing import Dict
-from typing import Iterator
-
-
-class PersicaReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ پرسیکا است.
-
-    Args:
-        csv_file: مسیر فایلِ پیکره با پسوند csv.
-
-    """
-
-    def __init__(self: "PersicaReader", csv_file: str) -> None:
-        self._csv_file = csv_file
-
-    def docs(self: "PersicaReader") -> Iterator[Dict[str, str]]:
-        """خبرها را برمی‌گرداند.
-
-        هر خبر، شی‌ای متشکل از این پارامتر است:
-
-        - شناسه (`id`)
-        - عنوان (`title`)
-        - متن (`text`)
-        - تاریخ (`date`)
-        - زمان (`time`)
-        - دستهٔ اصلی (`category`)
-        - دستهٔ فرعی (`category2`)
-
-        Examples:
-            >>> persica = PersicaReader('corpora/persica.csv')
-            >>> next(persica.docs())['id']
-            843656
-
-        Yields:
-            خبر بعدی.
-
-        """
-        lines = []
-        for current_line in Path(self._csv_file).open(encoding="utf-8-sig"):
-            current_line = current_line.strip()
-            if current_line:
-                if current_line.endswith(","):
-                    lines.append(current_line[:-1])
-                else:
-                    lines.append(current_line)
-                    yield {
-                        "id": int(lines[0]),
-                        "title": lines[1],
-                        "text": lines[2],
-                        "date": lines[3],
-                        "time": lines[4],
-                        "category": lines[5],
-                        "category2": lines[6],
-                    }
-                    lines = []
-
-    def texts(self: "PersicaReader") -> Iterator[str]:
-        """فقط متن خبرها را برمی‌گرداند.
-
-        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با همان تابع
-        ‍[docs()][hazm.corpus_readers.persica_reader.PersicaReader.docs] و دریافت مقدار پراپرتی
-        `text` نیز می‌توانید همین کار را انجام دهید.
-
-        Examples:
-            >>> persica = PersicaReader('corpora/persica.csv')
-            >>> next(persica.texts()).startswith('وزير علوم در جمع استادان نمونه كشور گفت')
-            True
-
-        Yields:
-            متنِ خبر بعدی.
-
-        """
-        for doc in self.docs():
-            yield doc["text"]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ پرسیکا است.
+
+[پیکرهٔ پرسیکا](https://www.peykaregan.ir/dataset/%D9%BE%D8%B1%D8%B3%DB%8C%DA%A
+9%D8%A7-%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-%D9%85%D8%AA%D9%88%D9%86-
+%D8%AE%D8%A8%D8%B1%DB%8C) حاوی
+خبرهای برگرفته از خبرگزاری ایسنا در یازده دستهٔ ورزشی، اقتصادی، فرهنگی، مذهبی،
+تاریخی، سیاسی، علمی، اجتماعی، آموزشی، حقوق قضایی و بهداشت است. روی این داده‌ها
+پیش‌پردازش‌هایی صورت شده و آمادهٔ استفاده در کاربردهای مختلف پردازش زبان طبیعی
+و
+داده‌کاوی است.
+
+"""
+from pathlib import Path
+from typing import Dict
+from typing import Iterator
+
+
+class PersicaReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ پرسیکا است.
+
+    Args:
+        csv_file: مسیر فایلِ پیکره با پسوند csv.
+
+    """
+
+    def __init__(self: "PersicaReader", csv_file: str) -> None:
+        self._csv_file = csv_file
+
+    def docs(self: "PersicaReader") -> Iterator[Dict[str, str]]:
+        """خبرها را برمی‌گرداند.
+
+        هر خبر، شی‌ای متشکل از این پارامتر است:
+
+        - شناسه (`id`)
+        - عنوان (`title`)
+        - متن (`text`)
+        - تاریخ (`date`)
+        - زمان (`time`)
+        - دستهٔ اصلی (`category`)
+        - دستهٔ فرعی (`category2`)
+
+        Examples:
+            >>> persica = PersicaReader('corpora/persica.csv')
+            >>> next(persica.docs())['id']
+            843656
+
+        Yields:
+            خبر بعدی.
+
+        """
+        lines = []
+        for current_line in Path(self._csv_file).open(encoding="utf-8-sig"):
+            current_line = current_line.strip()
+            if current_line:
+                if current_line.endswith(","):
+                    lines.append(current_line[:-1])
+                else:
+                    lines.append(current_line)
+                    yield {
+                        "id": int(lines[0]),
+                        "title": lines[1],
+                        "text": lines[2],
+                        "date": lines[3],
+                        "time": lines[4],
+                        "category": lines[5],
+                        "category2": lines[6],
+                    }
+                    lines = []
+
+    def texts(self: "PersicaReader") -> Iterator[str]:
+        """فقط متن خبرها را برمی‌گرداند.
+
+        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با همان تابع
+        ‍[docs()][hazm.corpus_readers.persica_reader.PersicaReader.docs] و دریافت مقدار پراپرتی
+        `text` نیز می‌توانید همین کار را انجام دهید.
+
+        Examples:
+            >>> persica = PersicaReader('corpora/persica.csv')
+            >>> next(persica.texts()).startswith('وزير علوم در جمع استادان نمونه كشور گفت')
+            True
+
+        Yields:
+            متنِ خبر بعدی.
+
+        """
+        for doc in self.docs():
+            yield doc["text"]
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/peykare_reader.py` & `hazm-0.9.1/hazm/corpus_readers/peykare_reader.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ Peykare است.
-
-[peykare پیکرهٔ](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%
-87-%D9%85%D8%AA%D9%86%DB%8C-%D8%B2%D8%A8%D8%A7%D9%86-
-%D9%81%D8%A7%D8%B1%D8%B3%DB%8C)
-جموعه‌ای از متون نوشتاری و گفتاری رسمی زبان فارسی است که از منابع واقعی همچون
-روزنامه‌ها، سایت‌ها و مستنداتِ از قبل تایپ‌شده، جمع‌آوری شده، تصحیح گردیده و
-برچسب خورده است. حجم این دادگان حدوداً ۱۰۰ میلیون کلمه است و از منابع مختلف
-تهیه
-گردیده و دارای تنوع بسیار زیادی است. ۱۰ میلیون کلمه از این پیکره با استفاده از
-۸۸۲ برچسب نحوی-معنایی به صورت دستی توسط دانشجویان رشتهٔ زبان‌شناسی برچسب‌دهی
-شده‌اند و هر پرونده بر حسب موضوع و منبع آن طبقه‌بندی شده است. این پیکره که توسط
-پژوهشکده پردازش هوشمند علائم تهیه شده است، برای استفاده در آموزش مدل زبانی و
-سایر پروژه‌های مربوط به پردازش زبان طبیعی مناسب است.
-
-"""
-
-
-import codecs
-import os
-from pathlib import Path
-from typing import Any
-from typing import Iterator
-from typing import List
-from typing import Tuple
-
-from hazm.normalizer import Normalizer
-from hazm.word_tokenizer import WordTokenizer
-
-
-def coarse_pos_u(tags: List[str], word: str) -> List[str]:
-    """برچسب‌های ریز را به برچسب‌های درشت منطبق با استاندارد جهانی (coarse-grained
-    universal pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_u(['N','COM','SING'], 'الجزیره')
-        'NOUN'
-
-    Args:
-        tags: لیست برچسب‌های ریز.
-        word: برچسبی که می‌خواهید به برچسب جهانی تبدیل شود.
-
-    Returns:
-        لیست برچسب‌های درشت جهانی.
-
-    """
-    map_pos_to_upos = {
-        "N": "NOUN",
-        "V": "VERB",
-        "AJ": "ADJ",
-        "ADV": "ADV",
-        "PRO": "PRON",
-        "DET": "DET",
-        "P": "ADP",
-        "POSTP": "ADP",
-        "NUM": "NUM",
-        "CONJ": "CCONJ",
-        "PUNC": "PUNCT",
-        "CL": "NOUN",
-        "INT": "INTJ",
-        "RES": "NOUN",
-    }
-    sconj_list = {
-        "که",
-        "تا",
-        "گرچه",
-        "اگرچه",
-        "چرا",
-        "زیرا",
-        "اگر",
-        "چون",
-        "چراکه",
-        "هرچند",
-        "وگرنه",
-        "چنانچه",
-        "والا",
-        "هرچه",
-        "ولو",
-        "مگر",
-        "پس",
-        "چو",
-        "چه",
-        "بنابراین",
-        "وقتی",
-        "والّا",
-        "انگاری",
-        "هرچندكه",
-        "درنتيجه",
-        "اگه",
-        "ازآنجاكه",
-        "گر",
-        "وگر",
-        "وقتيكه",
-        "تااينكه",
-        "زمانيكه",
-    }
-    num_adj_list = {
-        "نخست",
-        "دوم",
-        "اول",
-        "پنجم",
-        "آخر",
-        "يازدهم",
-        "نهم",
-        "چهارم",
-        "ششم",
-        "پانزدهم",
-        "دوازدهم",
-        "هشتم",
-        "صدم",
-        "هفتم",
-        "هفدهم",
-        "آخرين",
-        "سيزدهم",
-        "يكم",
-        "بيستم",
-        "ويكم",
-        "دوسوم",
-        "شانزدهم",
-        "هجدهم",
-        "چهاردهم",
-        "ششصدم",
-        "ميليونيم",
-        "وهفتم",
-        "يازدهمين",
-        "هيجدهمين",
-        "واپسين",
-        "چهلم",
-        "هزارم",
-        "وپنجم",
-        "هيجدهم",
-        "ميلياردم",
-        "ميليونيوم",
-        "تريليونيوم",
-        "چهارپنجم",
-        "دهگانه",
-        "ميليونم",
-        "اوّل",
-        "سوّم",
-    }
-    try:
-        old_pos = list(
-            set(tags)
-            & {
-                "N",
-                "V",
-                "AJ",
-                "ADV",
-                "PRO",
-                "DET",
-                "P",
-                "POSTP",
-                "NUM",
-                "CONJ",
-                "PUNC",
-                "CL",
-                "INT",
-                "RES",
-            },
-        )[0]
-        if old_pos == "CONJ" and word in sconj_list:
-            return "SCONJ"
-        if old_pos == "NUM" and word in num_adj_list:
-            return "ADJ" + (",EZ" if "EZ" in tags else "")
-        return map_pos_to_upos[old_pos] + (",EZ" if "EZ" in tags else "")
-    except:
-        return "NOUN"
-
-
-def coarse_pos_e(tags: List[str], word) -> List[str]:
-    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_e(['N','COM','SING'],'الجزیره')
-        'N'
-
-    Args:
-        tags: لیست برچسب‌های ریز.
-
-    Returns:
-        لیست برچسب‌های درشت.
-
-    """
-    try:
-        return list(
-            set(tags)
-            & {
-                "N",
-                "V",
-                "AJ",
-                "ADV",
-                "PRO",
-                "DET",
-                "P",
-                "POSTP",
-                "NUM",
-                "CONJ",
-                "PUNC",
-                "CL",
-                "INT",
-                "RES",
-            },
-        )[0] + (",EZ" if "EZ" in tags else "")
-    except:
-        return "N"
-
-
-def join_verb_parts(sentence: List[Tuple[str, str]]) -> List[Tuple[str, str]]:
-    """جمله را در قالب لیستی از `(توکن، برچسب)‌`ها می‌گیرد و توکن‌های مربوط به
-    افعال چندبخشی را با کاراکتر زیرخط (_) به هم می‌چسباند.
-
-    Examples:
-        >>> join_verb_parts([('اولین', 'AJ'), ('سیاره', 'Ne'), ('خارج', 'AJ'), ('از', 'P'), ('منظومه', 'Ne'), ('شمسی', 'AJ'), ('دیده', 'AJ'), ('شد', 'V'), ('.', 'PUNC')])
-        [('اولین', 'AJ'), ('سیاره', 'Ne'), ('خارج', 'AJ'), ('از', 'P'), ('منظومه', 'Ne'), ('شمسی', 'AJ'), ('دیده_شد', 'V'), ('.', 'PUNC')]
-
-    Args:
-        sentence: جمله در قالب لیستی از `(توکن، برچسب)`ها.
-
-    Returns:
-        لیستی از `(توکن، برچسب)`ها که در آن افعال چندبخشی در قالب یک توکن با کاراکتر زیرخط به هم چسبانده شده‌اند.
-
-    """
-    if not hasattr(join_verb_parts, "tokenizer"):
-        join_verb_parts.tokenizer = WordTokenizer()
-    before_verbs, after_verbs, verbe = (
-        join_verb_parts.tokenizer.before_verbs,
-        join_verb_parts.tokenizer.after_verbs,
-        join_verb_parts.tokenizer.verbe,
-    )
-
-    result = [("", "")]
-    for word in reversed(sentence):
-        if word[0] in before_verbs or (
-            result[-1][0] in after_verbs and word[0] in verbe
-        ):
-            result[-1] = (word[0] + "_" + result[-1][0], result[-1][1])
-        else:
-            result.append(word)
-    return list(reversed(result[1:]))
-
-
-class PeykareReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ Peykare است.
-
-    Args:
-        root: آدرس فولدر حاوی فایل‌های پیکره.
-        joined_verb_parts: اگر `True‍` باشد افعال چندقسمتی به‌شکل چسبیده‌به‌هم برگردانده_می‌شود.
-        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
-
-    """
-
-    def __init__(
-        self: "PeykareReader",
-        root: str,
-        joined_verb_parts: bool = True,
-        pos_map: str = coarse_pos_e,
-        universal_pos: bool = False,
-    ) -> None:
-        self._root = root
-        if pos_map is None:
-            self._pos_map = lambda tags: ",".join(tags)
-        elif universal_pos:
-            self._pos_map = coarse_pos_u
-        else:
-            self._pos_map = coarse_pos_e
-        self._joined_verb_parts = joined_verb_parts
-        self._normalizer = Normalizer(correct_spacing=False)
-
-    def docs(self: "PeykareReader") -> Iterator[str]:
-        """اسناد را به شکل متن خام برمی‌گرداند.
-
-        Yields:
-            متن خام سند بعدی.
-
-        """
-        for root, _, files in os.walk(self._root):
-            for name in sorted(files):
-                with codecs.open(
-                    Path(root) / name,
-                    encoding="windows-1256",
-                ) as peykare_file:
-                    text = peykare_file.read()
-                    if text:
-                        yield text
-
-    def doc_to_sents(
-        self: "PeykareReader", document: str,
-    ) -> Iterator[List[Tuple[str, str]]]:
-        """سند ورودی را به لیستی از جملات تبدیل می‌کند.
-
-        هر جمله لیستی از `(کلمه, برچسب)`ها است.
-
-        Args:
-            document: سندی که باید تبدیل شود.
-
-        Yields:
-            `ها جملهٔ بعدی در قالب لیستی از `(کلمه، برچسب).
-
-        """
-        sentence = []
-        for line in document.split("\r\n"):
-            if not line:
-                continue
-
-            parts = line.split(" ")
-            tags, word = parts[3], self._normalizer.normalize("‌".join(parts[4:]))
-
-            if word and word != "#":
-                sentence.append((word, tags))
-
-            if parts[2] == "PUNC" and word in {"#", ".", "؟", "!"}:
-                if len(sentence) > 1:
-                    yield sentence
-                sentence = []
-
-    def sents(self: "PeykareReader") -> Iterator[List[Tuple[str, str]]]:
-        """جملات پیکره را در قالب لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> peykare = PeykareReader(root='corpora/peykare')
-            >>> next(peykare.sents())
-            [('دیرزمانی', 'N'), ('از', 'P'), ('راه\u200cاندازی', 'N,EZ'), ('شبکه\u200cی', 'N,EZ'), ('خبر', 'N,EZ'), ('الجزیره', 'N'), ('نمی\u200cگذرد', 'V'), ('،', 'PUNC'), ('اما', 'CONJ'), ('این', 'DET'), ('شبکه\u200cی', 'N,EZ'), ('خبری', 'AJ,EZ'), ('عربی', 'N'), ('بسیار', 'ADV'), ('سریع', 'ADV'), ('توانسته', 'V'), ('در', 'P'), ('میان', 'N,EZ'), ('شبکه\u200cهای', 'N,EZ'), ('عظیم', 'AJ,EZ'), ('خبری', 'AJ'), ('و', 'CONJ'), ('بنگاه\u200cهای', 'N,EZ'), ('چندرسانه\u200cای', 'AJ,EZ'), ('دنیا', 'N'), ('خودی', 'N'), ('نشان', 'N'), ('دهد', 'V'), ('.', 'PUNC')]
-
-        Yields:
-            جملهٔ بعدی در قالب لیستی از `(توکن، برچسب)`ها.
-
-        """
-
-        # >>> peykare = PeykareReader(root='corpora/peykare', joined_verb_parts=False, pos_map=None)
-        # >>> next(peykare.sents())
-        def map_pos(item: str) -> Tuple:
-            return (item[0], self._pos_map(item[1].split(","), item[0]))
-
-        for document in self.docs():
-            for sentence in self.doc_to_sents(document):
-                if self._joined_verb_parts:
-                    sentence = join_verb_parts(sentence)
-
-                yield list(map(map_pos, sentence))
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ Peykare است.
+
+[peykare پیکرهٔ](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%
+87-%D9%85%D8%AA%D9%86%DB%8C-%D8%B2%D8%A8%D8%A7%D9%86-
+%D9%81%D8%A7%D8%B1%D8%B3%DB%8C)
+جموعه‌ای از متون نوشتاری و گفتاری رسمی زبان فارسی است که از منابع واقعی همچون
+روزنامه‌ها، سایت‌ها و مستنداتِ از قبل تایپ‌شده، جمع‌آوری شده، تصحیح گردیده و
+برچسب خورده است. حجم این دادگان حدوداً ۱۰۰ میلیون کلمه است و از منابع مختلف
+تهیه
+گردیده و دارای تنوع بسیار زیادی است. ۱۰ میلیون کلمه از این پیکره با استفاده از
+۸۸۲ برچسب نحوی-معنایی به صورت دستی توسط دانشجویان رشتهٔ زبان‌شناسی برچسب‌دهی
+شده‌اند و هر پرونده بر حسب موضوع و منبع آن طبقه‌بندی شده است. این پیکره که توسط
+پژوهشکده پردازش هوشمند علائم تهیه شده است، برای استفاده در آموزش مدل زبانی و
+سایر پروژه‌های مربوط به پردازش زبان طبیعی مناسب است.
+
+"""
+
+
+import codecs
+import os
+from pathlib import Path
+from typing import Any
+from typing import Iterator
+from typing import List
+from typing import Tuple
+
+from hazm.normalizer import Normalizer
+from hazm.word_tokenizer import WordTokenizer
+
+
+def coarse_pos_u(tags: List[str], word: str) -> List[str]:
+    """برچسب‌های ریز را به برچسب‌های درشت منطبق با استاندارد جهانی (coarse-grained
+    universal pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_u(['N','COM','SING'], 'الجزیره')
+        'NOUN'
+
+    Args:
+        tags: لیست برچسب‌های ریز.
+        word: برچسبی که می‌خواهید به برچسب جهانی تبدیل شود.
+
+    Returns:
+        لیست برچسب‌های درشت جهانی.
+
+    """
+    map_pos_to_upos = {
+        "N": "NOUN",
+        "V": "VERB",
+        "AJ": "ADJ",
+        "ADV": "ADV",
+        "PRO": "PRON",
+        "DET": "DET",
+        "P": "ADP",
+        "POSTP": "ADP",
+        "NUM": "NUM",
+        "CONJ": "CCONJ",
+        "PUNC": "PUNCT",
+        "CL": "NOUN",
+        "INT": "INTJ",
+        "RES": "NOUN",
+    }
+    sconj_list = {
+        "که",
+        "تا",
+        "گرچه",
+        "اگرچه",
+        "چرا",
+        "زیرا",
+        "اگر",
+        "چون",
+        "چراکه",
+        "هرچند",
+        "وگرنه",
+        "چنانچه",
+        "والا",
+        "هرچه",
+        "ولو",
+        "مگر",
+        "پس",
+        "چو",
+        "چه",
+        "بنابراین",
+        "وقتی",
+        "والّا",
+        "انگاری",
+        "هرچندكه",
+        "درنتيجه",
+        "اگه",
+        "ازآنجاكه",
+        "گر",
+        "وگر",
+        "وقتيكه",
+        "تااينكه",
+        "زمانيكه",
+    }
+    num_adj_list = {
+        "نخست",
+        "دوم",
+        "اول",
+        "پنجم",
+        "آخر",
+        "يازدهم",
+        "نهم",
+        "چهارم",
+        "ششم",
+        "پانزدهم",
+        "دوازدهم",
+        "هشتم",
+        "صدم",
+        "هفتم",
+        "هفدهم",
+        "آخرين",
+        "سيزدهم",
+        "يكم",
+        "بيستم",
+        "ويكم",
+        "دوسوم",
+        "شانزدهم",
+        "هجدهم",
+        "چهاردهم",
+        "ششصدم",
+        "ميليونيم",
+        "وهفتم",
+        "يازدهمين",
+        "هيجدهمين",
+        "واپسين",
+        "چهلم",
+        "هزارم",
+        "وپنجم",
+        "هيجدهم",
+        "ميلياردم",
+        "ميليونيوم",
+        "تريليونيوم",
+        "چهارپنجم",
+        "دهگانه",
+        "ميليونم",
+        "اوّل",
+        "سوّم",
+    }
+    try:
+        old_pos = list(
+            set(tags)
+            & {
+                "N",
+                "V",
+                "AJ",
+                "ADV",
+                "PRO",
+                "DET",
+                "P",
+                "POSTP",
+                "NUM",
+                "CONJ",
+                "PUNC",
+                "CL",
+                "INT",
+                "RES",
+            },
+        )[0]
+        if old_pos == "CONJ" and word in sconj_list:
+            return "SCONJ"
+        if old_pos == "NUM" and word in num_adj_list:
+            return "ADJ" + (",EZ" if "EZ" in tags else "")
+        return map_pos_to_upos[old_pos] + (",EZ" if "EZ" in tags else "")
+    except:
+        return "NOUN"
+
+
+def coarse_pos_e(tags: List[str], word) -> List[str]:
+    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_e(['N','COM','SING'],'الجزیره')
+        'N'
+
+    Args:
+        tags: لیست برچسب‌های ریز.
+
+    Returns:
+        لیست برچسب‌های درشت.
+
+    """
+    try:
+        return list(
+            set(tags)
+            & {
+                "N",
+                "V",
+                "AJ",
+                "ADV",
+                "PRO",
+                "DET",
+                "P",
+                "POSTP",
+                "NUM",
+                "CONJ",
+                "PUNC",
+                "CL",
+                "INT",
+                "RES",
+            },
+        )[0] + (",EZ" if "EZ" in tags else "")
+    except:
+        return "N"
+
+
+def join_verb_parts(sentence: List[Tuple[str, str]]) -> List[Tuple[str, str]]:
+    """جمله را در قالب لیستی از `(توکن، برچسب)‌`ها می‌گیرد و توکن‌های مربوط به
+    افعال چندبخشی را با کاراکتر زیرخط (_) به هم می‌چسباند.
+
+    Examples:
+        >>> join_verb_parts([('اولین', 'AJ'), ('سیاره', 'Ne'), ('خارج', 'AJ'), ('از', 'P'), ('منظومه', 'Ne'), ('شمسی', 'AJ'), ('دیده', 'AJ'), ('شد', 'V'), ('.', 'PUNC')])
+        [('اولین', 'AJ'), ('سیاره', 'Ne'), ('خارج', 'AJ'), ('از', 'P'), ('منظومه', 'Ne'), ('شمسی', 'AJ'), ('دیده_شد', 'V'), ('.', 'PUNC')]
+
+    Args:
+        sentence: جمله در قالب لیستی از `(توکن، برچسب)`ها.
+
+    Returns:
+        لیستی از `(توکن، برچسب)`ها که در آن افعال چندبخشی در قالب یک توکن با کاراکتر زیرخط به هم چسبانده شده‌اند.
+
+    """
+    if not hasattr(join_verb_parts, "tokenizer"):
+        join_verb_parts.tokenizer = WordTokenizer()
+    before_verbs, after_verbs, verbe = (
+        join_verb_parts.tokenizer.before_verbs,
+        join_verb_parts.tokenizer.after_verbs,
+        join_verb_parts.tokenizer.verbe,
+    )
+
+    result = [("", "")]
+    for word in reversed(sentence):
+        if word[0] in before_verbs or (
+            result[-1][0] in after_verbs and word[0] in verbe
+        ):
+            result[-1] = (word[0] + "_" + result[-1][0], result[-1][1])
+        else:
+            result.append(word)
+    return list(reversed(result[1:]))
+
+
+class PeykareReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ Peykare است.
+
+    Args:
+        root: آدرس فولدر حاوی فایل‌های پیکره.
+        joined_verb_parts: اگر `True‍` باشد افعال چندقسمتی به‌شکل چسبیده‌به‌هم برگردانده_می‌شود.
+        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
+
+    """
+
+    def __init__(
+        self: "PeykareReader",
+        root: str,
+        joined_verb_parts: bool = True,
+        pos_map: str = coarse_pos_e,
+        universal_pos: bool = False,
+    ) -> None:
+        self._root = root
+        if pos_map is None:
+            self._pos_map = lambda tags: ",".join(tags)
+        elif universal_pos:
+            self._pos_map = coarse_pos_u
+        else:
+            self._pos_map = coarse_pos_e
+        self._joined_verb_parts = joined_verb_parts
+        self._normalizer = Normalizer(correct_spacing=False)
+
+    def docs(self: "PeykareReader") -> Iterator[str]:
+        """اسناد را به شکل متن خام برمی‌گرداند.
+
+        Yields:
+            متن خام سند بعدی.
+
+        """
+        for root, _, files in os.walk(self._root):
+            for name in sorted(files):
+                with codecs.open(
+                    Path(root) / name,
+                    encoding="windows-1256",
+                ) as peykare_file:
+                    text = peykare_file.read()
+                    if text:
+                        yield text
+
+    def doc_to_sents(
+        self: "PeykareReader", document: str,
+    ) -> Iterator[List[Tuple[str, str]]]:
+        """سند ورودی را به لیستی از جملات تبدیل می‌کند.
+
+        هر جمله لیستی از `(کلمه, برچسب)`ها است.
+
+        Args:
+            document: سندی که باید تبدیل شود.
+
+        Yields:
+            `ها جملهٔ بعدی در قالب لیستی از `(کلمه، برچسب).
+
+        """
+        sentence = []
+        for line in document.split("\r\n"):
+            if not line:
+                continue
+
+            parts = line.split(" ")
+            tags, word = parts[3], self._normalizer.normalize("‌".join(parts[4:]))
+
+            if word and word != "#":
+                sentence.append((word, tags))
+
+            if parts[2] == "PUNC" and word in {"#", ".", "؟", "!"}:
+                if len(sentence) > 1:
+                    yield sentence
+                sentence = []
+
+    def sents(self: "PeykareReader") -> Iterator[List[Tuple[str, str]]]:
+        """جملات پیکره را در قالب لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> peykare = PeykareReader(root='corpora/peykare')
+            >>> next(peykare.sents())
+            [('دیرزمانی', 'N'), ('از', 'P'), ('راه\u200cاندازی', 'N,EZ'), ('شبکه\u200cی', 'N,EZ'), ('خبر', 'N,EZ'), ('الجزیره', 'N'), ('نمی\u200cگذرد', 'V'), ('،', 'PUNC'), ('اما', 'CONJ'), ('این', 'DET'), ('شبکه\u200cی', 'N,EZ'), ('خبری', 'AJ,EZ'), ('عربی', 'N'), ('بسیار', 'ADV'), ('سریع', 'ADV'), ('توانسته', 'V'), ('در', 'P'), ('میان', 'N,EZ'), ('شبکه\u200cهای', 'N,EZ'), ('عظیم', 'AJ,EZ'), ('خبری', 'AJ'), ('و', 'CONJ'), ('بنگاه\u200cهای', 'N,EZ'), ('چندرسانه\u200cای', 'AJ,EZ'), ('دنیا', 'N'), ('خودی', 'N'), ('نشان', 'N'), ('دهد', 'V'), ('.', 'PUNC')]
+
+        Yields:
+            جملهٔ بعدی در قالب لیستی از `(توکن، برچسب)`ها.
+
+        """
+
+        # >>> peykare = PeykareReader(root='corpora/peykare', joined_verb_parts=False, pos_map=None)
+        # >>> next(peykare.sents())
+        def map_pos(item: str) -> Tuple:
+            return (item[0], self._pos_map(item[1].split(","), item[0]))
+
+        for document in self.docs():
+            for sentence in self.doc_to_sents(document):
+                if self._joined_verb_parts:
+                    sentence = join_verb_parts(sentence)
+
+                yield list(map(map_pos, sentence))
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/quran_reader.py` & `hazm-0.9.1/hazm/corpus_readers/quran_reader.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ Quranic Arabic است.
-
-پیکرهٔ [Quranic Arabic](https://corpus.quran.com/) شامل قواعد نحوی و اطلاعات
-ریخت‌شناسی تک‌تک کلمات قرآن کریم است.
-
-"""
-from pathlib import Path
-from typing import Dict
-from typing import Iterator
-from typing import List
-from typing import Tuple
-
-from hazm.utils import maketrans
-
-buckwalter_transliteration = maketrans(
-    "'>&<}AbptvjHxd*rzs$SDTZEg_fqklmnhwYyFNKaui~o^#`{:@\"[;,.!-+%]",
-    "\u0621\u0623\u0624\u0625\u0626\u0627\u0628\u0629\u062a\u062b\u062c\u062d\u062e\u062f\u0630\u0631\u0632\u0633\u0634\u0635\u0636\u0637\u0638\u0639\u063a\u0640\u0641\u0642\u0643\u0644\u0645\u0646\u0647\u0648\u0649\u064a\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652\u0653\u0654\u0670\u0671\u06dc\u06df\u06e0\u06e2\u06e3\u06e5\u06e6\u06e8\u06ea\u06eb\u06ec\u06ed",
-)
-
-
-class QuranReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ Quranic Arabic است.
-
-    Args:
-        quran_file: مسیر فایلِ پیکره
-
-    """
-
-    def __init__(self: "QuranReader", quran_file: str) -> None:
-        self._quran_file = quran_file
-
-    def parts(self: "QuranReader") -> Iterator[Dict[str, str]]:
-        """اجزای متن قرآن را به‌همراه اطلاعات نحوی‌شان برمی‌گرداند.
-
-        یک جزء لزوماً یک کلمه نیست؛ مثلاً واژهٔ «الرحمن» از دو جزء «ال» و «رحمن» تشکیل
-        شده است.
-
-        Examples:
-            >>> parts=QuranReader(quran_file='corpora/quranic_corpus_morphology.txt').parts()
-            >>> print(next(parts))
-            {'loc': (1, 1, 1, 1), 'text': 'بِ', 'tag': 'P'}
-            >>> print(next(parts))
-            {'loc': (1, 1, 1, 2), 'text': 'سْمِ', 'tag': 'N', 'lem': 'ٱسْم', 'root': 'سمو'}
-            >>> print(next(parts))
-            {'loc': (1, 1, 2, 1), 'text': 'ٱللَّهِ', 'tag': 'PN', 'lem': 'ٱللَّه', 'root': 'اله'}
-
-        Yields:
-            جزء بعدی متن قرآن.
-
-        """
-        for line in Path(self._quran_file).open(encoding="utf8"):
-            if not line.startswith("("):
-                continue
-            parts = line.strip().split("\t")
-
-            part = {
-                "loc": eval(parts[0].replace(":", ",")),
-                "text": parts[1].translate(buckwalter_transliteration),
-                "tag": parts[2],
-            }
-
-            features = parts[3].split("|")
-            for feature in features:
-                if feature.startswith("LEM:"):
-                    part["lem"] = feature[4:].translate(buckwalter_transliteration)
-                elif feature.startswith("ROOT:"):
-                    part["root"] = feature[5:].translate(buckwalter_transliteration)
-            yield part
-
-    def words(
-        self: "QuranReader",
-    ) -> Iterator[Tuple[str, str, str, str, str, List[Dict[str, str]]]]:
-        """اطلاعات صرفی کلمات قرآن را برمی‌گرداند.
-
-        Examples:
-            >>> words=QuranReader(quran_file='corpora/quranic_corpus_morphology.txt').words()
-            >>> print(next(words))
-            ('1.1.1', 'بِسْمِ', 'ٱسْم', 'سمو', 'P-N', [{'text': 'بِ', 'tag': 'P'}, {'text': 'سْمِ', 'tag': 'N', 'lem': 'ٱسْم', 'root': 'سمو'}])
-
-        Yields:
-            اطلاعات صرفی کلمهٔ بعدی قرآن.
-
-        """
-
-        def word_item(location: Tuple[int], parts: List[Dict]) -> str:
-            text = "".join([part["text"] for part in parts])
-            tag = "-".join([part["tag"] for part in parts])
-            lem = "-".join([part["lem"] for part in parts if "lem" in part])
-            root = "-".join([part["root"] for part in parts if "root" in part])
-            return ".".join(map(str, location)), text, lem, root, tag, parts
-
-        last_location = (0, 0, 0, 0)
-        items = []
-        for part in self.parts():
-            if last_location[:3] == part["loc"][:3]:
-                items.append(part)
-            else:
-                if items:
-                    yield word_item(last_location[:3], items)
-                items = [part]
-            last_location = part["loc"]
-            del part["loc"]
-        yield word_item(last_location[:3], items)
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ Quranic Arabic است.
+
+پیکرهٔ [Quranic Arabic](https://corpus.quran.com/) شامل قواعد نحوی و اطلاعات
+ریخت‌شناسی تک‌تک کلمات قرآن کریم است.
+
+"""
+from pathlib import Path
+from typing import Dict
+from typing import Iterator
+from typing import List
+from typing import Tuple
+
+from hazm.utils import maketrans
+
+buckwalter_transliteration = maketrans(
+    "'>&<}AbptvjHxd*rzs$SDTZEg_fqklmnhwYyFNKaui~o^#`{:@\"[;,.!-+%]",
+    "\u0621\u0623\u0624\u0625\u0626\u0627\u0628\u0629\u062a\u062b\u062c\u062d\u062e\u062f\u0630\u0631\u0632\u0633\u0634\u0635\u0636\u0637\u0638\u0639\u063a\u0640\u0641\u0642\u0643\u0644\u0645\u0646\u0647\u0648\u0649\u064a\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652\u0653\u0654\u0670\u0671\u06dc\u06df\u06e0\u06e2\u06e3\u06e5\u06e6\u06e8\u06ea\u06eb\u06ec\u06ed",
+)
+
+
+class QuranReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ Quranic Arabic است.
+
+    Args:
+        quran_file: مسیر فایلِ پیکره
+
+    """
+
+    def __init__(self: "QuranReader", quran_file: str) -> None:
+        self._quran_file = quran_file
+
+    def parts(self: "QuranReader") -> Iterator[Dict[str, str]]:
+        """اجزای متن قرآن را به‌همراه اطلاعات نحوی‌شان برمی‌گرداند.
+
+        یک جزء لزوماً یک کلمه نیست؛ مثلاً واژهٔ «الرحمن» از دو جزء «ال» و «رحمن» تشکیل
+        شده است.
+
+        Examples:
+            >>> parts=QuranReader(quran_file='corpora/quranic_corpus_morphology.txt').parts()
+            >>> print(next(parts))
+            {'loc': (1, 1, 1, 1), 'text': 'بِ', 'tag': 'P'}
+            >>> print(next(parts))
+            {'loc': (1, 1, 1, 2), 'text': 'سْمِ', 'tag': 'N', 'lem': 'ٱسْم', 'root': 'سمو'}
+            >>> print(next(parts))
+            {'loc': (1, 1, 2, 1), 'text': 'ٱللَّهِ', 'tag': 'PN', 'lem': 'ٱللَّه', 'root': 'اله'}
+
+        Yields:
+            جزء بعدی متن قرآن.
+
+        """
+        for line in Path(self._quran_file).open(encoding="utf8"):
+            if not line.startswith("("):
+                continue
+            parts = line.strip().split("\t")
+
+            part = {
+                "loc": eval(parts[0].replace(":", ",")),
+                "text": parts[1].translate(buckwalter_transliteration),
+                "tag": parts[2],
+            }
+
+            features = parts[3].split("|")
+            for feature in features:
+                if feature.startswith("LEM:"):
+                    part["lem"] = feature[4:].translate(buckwalter_transliteration)
+                elif feature.startswith("ROOT:"):
+                    part["root"] = feature[5:].translate(buckwalter_transliteration)
+            yield part
+
+    def words(
+        self: "QuranReader",
+    ) -> Iterator[Tuple[str, str, str, str, str, List[Dict[str, str]]]]:
+        """اطلاعات صرفی کلمات قرآن را برمی‌گرداند.
+
+        Examples:
+            >>> words=QuranReader(quran_file='corpora/quranic_corpus_morphology.txt').words()
+            >>> print(next(words))
+            ('1.1.1', 'بِسْمِ', 'ٱسْم', 'سمو', 'P-N', [{'text': 'بِ', 'tag': 'P'}, {'text': 'سْمِ', 'tag': 'N', 'lem': 'ٱسْم', 'root': 'سمو'}])
+
+        Yields:
+            اطلاعات صرفی کلمهٔ بعدی قرآن.
+
+        """
+
+        def word_item(location: Tuple[int], parts: List[Dict]) -> str:
+            text = "".join([part["text"] for part in parts])
+            tag = "-".join([part["tag"] for part in parts])
+            lem = "-".join([part["lem"] for part in parts if "lem" in part])
+            root = "-".join([part["root"] for part in parts if "root" in part])
+            return ".".join(map(str, location)), text, lem, root, tag, parts
+
+        last_location = (0, 0, 0, 0)
+        items = []
+        for part in self.parts():
+            if last_location[:3] == part["loc"][:3]:
+                items.append(part)
+            else:
+                if items:
+                    yield word_item(last_location[:3], items)
+                items = [part]
+            last_location = part["loc"]
+            del part["loc"]
+        yield word_item(last_location[:3], items)
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/sentipers_reader.py` & `hazm-0.9.1/hazm/corpus_readers/sentipers_reader.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ سِنتی‌پِرِس است.
-
-سِنتی‌پرس شامل مجموعه‌ای از متون فارسی با برچسب‌های معنایی است.
-
-"""
-
-
-import itertools
-import os
-import sys
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import Iterator
-from xml.dom import minidom
-
-
-class SentiPersReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ سِنتی‌پِرِس است.
-
-    Args:
-        root: مسیر فولدر حاوی فایل‌های پیکره
-
-    """
-
-    def __init__(self: "SentiPersReader", root: str) -> None:
-        self._root = root
-
-    def docs(self: "SentiPersReader") -> Iterator[Dict[str, Any]]:
-        """متن‌های فارسی را در قالب یک برمی‌گرداند.
-
-        هر متن شامل این فیلدهاست:
-
-        - عنوان (Title)
-        - نوع (Type)
-        - نظرات (comments)
-
-        فیلد `comments `خودش شامل این فیلدهاست:
-
-        - شناسه (id)
-        - نوع (type)
-        - نویسنده (author)
-        - ارزش (value)
-        - جملات (sentences)
-
-        Yields:
-            متن بعدی.
-
-        """
-
-        def element_sentences(element: str) -> Iterator[Dict]:
-            for sentence in element.getElementsByTagName("Sentence"):
-                yield {
-                    "text": sentence.childNodes[0].data,
-                    "id": sentence.getAttribute("ID"),
-                    "value": (
-                        int(sentence.getAttribute("Value"))
-                        if comment.getAttribute("Value")
-                        else None
-                    ),
-                }
-
-        for root, _dirs, files in os.walk(self._root):
-            for filename in sorted(files):
-                try:
-                    elements = minidom.parse(os.path.join(root, filename))
-
-                    product = elements.getElementsByTagName("Product")[0]
-                    doc = {
-                        "Title": product.getAttribute("Title"),
-                        "Type": product.getAttribute("Type"),
-                        "comments": [],
-                    }
-
-                    for child in product.childNodes:
-                        if child.nodeName in {
-                            "Voters",
-                            "Performance",
-                            "Capability",
-                            "Production_Quality",
-                            "Ergonomics",
-                            "Purchase_Value",
-                        }:
-                            value = child.getAttribute("Value")
-                            doc[child.nodeName] = (
-                                float(value) if "." in value else int(value)
-                            )
-
-                    for comment in itertools.chain(
-                        elements.getElementsByTagName("Opinion"),
-                        elements.getElementsByTagName("Criticism"),
-                    ):
-                        doc["comments"].append(
-                            {
-                                "id": comment.getAttribute("ID"),
-                                "type": comment.nodeName,
-                                "author": comment.getAttribute("Holder").strip(),
-                                "value": (
-                                    int(comment.getAttribute("Value"))
-                                    if comment.getAttribute("Value")
-                                    else None
-                                ),
-                                "sentences": list(element_sentences(comment)),
-                            },
-                        )
-
-                    # todo: Accessories, Features, Review, Advantages, Tags, Keywords, Index
-
-                    yield doc
-
-                except Exception as e:
-                    print("error in reading", filename, e, file=sys.stderr)
-
-    def comments(self: "SentiPersReader") -> Iterator[str]:
-        """نظرات مربوط به متن را برمی‌گرداند.
-
-        Examples:
-            >>> sentipers = SentiPersReader(root='corpora/sentipers')
-            >>> next(sentipers.comments())[0][1]
-            'بيشتر مناسب است براي کساني که به دنبال تنوع هستند و در همه چيز نو گرايي دارند .'
-
-        Yields:
-            نظر بعدی.
-
-        """
-        for doc in self.docs():
-            yield [
-                [sentence["text"] for sentence in text]
-                for text in [comment["sentences"] for comment in doc["comments"]]
-            ]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ سِنتی‌پِرِس است.
+
+سِنتی‌پرس شامل مجموعه‌ای از متون فارسی با برچسب‌های معنایی است.
+
+"""
+
+
+import itertools
+import os
+import sys
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import Iterator
+from xml.dom import minidom
+
+
+class SentiPersReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ سِنتی‌پِرِس است.
+
+    Args:
+        root: مسیر فولدر حاوی فایل‌های پیکره
+
+    """
+
+    def __init__(self: "SentiPersReader", root: str) -> None:
+        self._root = root
+
+    def docs(self: "SentiPersReader") -> Iterator[Dict[str, Any]]:
+        """متن‌های فارسی را در قالب یک برمی‌گرداند.
+
+        هر متن شامل این فیلدهاست:
+
+        - عنوان (Title)
+        - نوع (Type)
+        - نظرات (comments)
+
+        فیلد `comments `خودش شامل این فیلدهاست:
+
+        - شناسه (id)
+        - نوع (type)
+        - نویسنده (author)
+        - ارزش (value)
+        - جملات (sentences)
+
+        Yields:
+            متن بعدی.
+
+        """
+
+        def element_sentences(element: str) -> Iterator[Dict]:
+            for sentence in element.getElementsByTagName("Sentence"):
+                yield {
+                    "text": sentence.childNodes[0].data,
+                    "id": sentence.getAttribute("ID"),
+                    "value": (
+                        int(sentence.getAttribute("Value"))
+                        if comment.getAttribute("Value")
+                        else None
+                    ),
+                }
+
+        for root, _dirs, files in os.walk(self._root):
+            for filename in sorted(files):
+                try:
+                    elements = minidom.parse(os.path.join(root, filename))
+
+                    product = elements.getElementsByTagName("Product")[0]
+                    doc = {
+                        "Title": product.getAttribute("Title"),
+                        "Type": product.getAttribute("Type"),
+                        "comments": [],
+                    }
+
+                    for child in product.childNodes:
+                        if child.nodeName in {
+                            "Voters",
+                            "Performance",
+                            "Capability",
+                            "Production_Quality",
+                            "Ergonomics",
+                            "Purchase_Value",
+                        }:
+                            value = child.getAttribute("Value")
+                            doc[child.nodeName] = (
+                                float(value) if "." in value else int(value)
+                            )
+
+                    for comment in itertools.chain(
+                        elements.getElementsByTagName("Opinion"),
+                        elements.getElementsByTagName("Criticism"),
+                    ):
+                        doc["comments"].append(
+                            {
+                                "id": comment.getAttribute("ID"),
+                                "type": comment.nodeName,
+                                "author": comment.getAttribute("Holder").strip(),
+                                "value": (
+                                    int(comment.getAttribute("Value"))
+                                    if comment.getAttribute("Value")
+                                    else None
+                                ),
+                                "sentences": list(element_sentences(comment)),
+                            },
+                        )
+
+                    # todo: Accessories, Features, Review, Advantages, Tags, Keywords, Index
+
+                    yield doc
+
+                except Exception as e:
+                    print("error in reading", filename, e, file=sys.stderr)
+
+    def comments(self: "SentiPersReader") -> Iterator[str]:
+        """نظرات مربوط به متن را برمی‌گرداند.
+
+        Examples:
+            >>> sentipers = SentiPersReader(root='corpora/sentipers')
+            >>> next(sentipers.comments())[0][1]
+            'بيشتر مناسب است براي کساني که به دنبال تنوع هستند و در همه چيز نو گرايي دارند .'
+
+        Yields:
+            نظر بعدی.
+
+        """
+        for doc in self.docs():
+            yield [
+                [sentence["text"] for sentence in text]
+                for text in [comment["sentences"] for comment in doc["comments"]]
+            ]
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/treebank_reader.py` & `hazm-0.9.1/hazm/corpus_readers/treebank_reader.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,410 +1,410 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ تری‌بانک است.
-
-پیکرهٔ تری‌بانک حاوی هزاران جملهٔ برچسب‌خورده با اطلاعات نحوی و ساخت‌واژی است.
-
-"""
-
-
-import os
-import re
-import sys
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import Iterator
-from typing import List
-from typing import Tuple
-from xml.dom import minidom
-
-from nltk.tree import Tree
-
-from ..word_tokenizer import WordTokenizer
-
-
-def coarse_pos_e(tags: List[str]) -> List[str]:
-    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_e(['Nasp---', 'pers', 'prop'])
-        'N'
-
-    Args:
-        tags: لیست برچسب‌های ریز.
-
-    Returns:
-        لیست برچسب‌های درشت.
-
-    """
-    mapping = {
-        "N": "N",
-        "V": "V",
-        "A": "AJ",
-        "D": "ADV",
-        "Z": "PRO",
-        "T": "DET",
-        "E": "P",
-        "P": "POSTP",
-        "U": "NUM",
-        "J": "CONJ",
-        "O": "PUNC",
-        "R": "RES",
-        "L": "CL",
-        "I": "INT",
-    }
-    try:
-        if tags[0][0] == "C":
-            if "pronominal" in tags:
-                tags[0] = "Z"
-            elif "verb" in tags:
-                tags[0] = "V"
-            elif "prep" in tags:
-                tags[0] = "E"
-            elif "adv" in tags:
-                tags[0] = "D"
-            elif "det" in tags:
-                tags[0] = "T"
-        return mapping[tags[0][0]] + ("e" if "ezafe" in tags else "")
-    except Exception:
-        return ""
-
-
-class TreebankReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ تری‌بانک است.
-
-    Args:
-        root: مسیر فولدر حاوی فایل‌های پیکره
-        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
-        join_clitics: اگر `True‍` باشد واژه‌بست‌ها را به کلمهٔ مادر می‌چسباند.
-        join_verb_parts: اگر `True` باشد افعال چندبخشی را با _ به هم می‌چسباند.
-
-    """
-
-    def __init__(
-        self: "TreebankReader",
-        root: str,
-        pos_map: str = coarse_pos_e,
-        join_clitics: bool = False,
-        join_verb_parts: bool = False,
-    ) -> None:
-        self._root = root
-        self._pos_map = pos_map if pos_map else lambda tags: ",".join(tags)
-        self._join_clitics = join_clitics
-        self._join_verb_parts = join_verb_parts
-        self._tokenizer = WordTokenizer()
-
-    def docs(self: "TreebankReader") -> Iterator[Any]:
-        """اسناد موجود در پیکره را برمی‌گرداند.
-
-        Yields:
-            سند بعدی.
-
-        """
-        for root, _dirs, files in os.walk(self._root):
-            for name in sorted(files):
-                try:
-                    with Path.open(
-                        Path(root) / name,
-                        encoding="utf8",
-                    ) as treebank_file:
-                        raw = re.sub(r"\n *", "", treebank_file.read())
-                        yield minidom.parseString(raw.encode("utf8"))
-                except Exception as e:
-                    print("error in reading", name, e, file=sys.stderr)
-
-    def trees(self: "TreebankReader") -> Iterator[str]:
-        """ساختارهای درختی موجود در پیکره را برمی‌گرداند.
-
-        Examples:
-            >>> treebank = TreebankReader(root='corpora/treebank')
-            >>> print(next(treebank.trees()))
-            (S
-            (VPS
-                    (NPC (N دنیای/Ne) (MN (N آدولف/N) (N بورن/N)))
-                    (VPC
-                    (NPC (N دنیای/Ne) (NPA (N اتفاقات/Ne) (ADJ رویایی/AJ)))
-                    (V است/V)))
-            (PUNC ./PUNC))
-
-        Yields:
-            ساختار درختی بعدی.
-
-        """
-
-        def traverse(node: str) -> Tree:
-            def extract_tags(w: str):
-                pos = [w.getAttribute("lc") if w.getAttribute("lc") else None]
-                if w.getAttribute("clitic") in {
-                    "ezafe",
-                    "pronominal",
-                    "verb",
-                    "prep",
-                    "adv",
-                    "det",
-                }:
-                    pos.append(w.getAttribute("clitic"))
-                if w.getAttribute("ne_sort"):
-                    pos.append(w.getAttribute("ne_sort"))
-                if w.getAttribute("n_type"):
-                    pos.append(w.getAttribute("n_type"))
-                if w.getAttribute("ya_type"):
-                    pos.append(w.getAttribute("ya_type"))
-                if w.getAttribute("ke_type"):
-                    pos.append(w.getAttribute("ke_type"))
-                if w.getAttribute("type"):
-                    pos.append(w.getAttribute("type"))
-                if w.getAttribute("kind"):
-                    pos.append(w.getAttribute("kind"))
-                return pos
-
-            def clitic_join(tree: Tree, clitic: Dict):
-                if type(tree[-1]) == Tree:
-                    return clitic_join(tree[-1], clitic)
-
-                if clitic[0][0][0] == "ا":
-                    clitic[0] = ("‌" + clitic[0][0], clitic[0][1])
-                tree[-1] = (tree[-1][0] + clitic[0][0], clitic[0][1])
-                tree.set_label("CLITICS")
-                return None
-
-            if not len(node.childNodes):
-                return None
-            first = node.childNodes[0]
-
-            if first.nodeName == "w":
-                pos = extract_tags(first)
-                return Tree(
-                    node.nodeName,
-                    [
-                        (self._pos_map(pos),),
-                    ],
-                )
-            childs = node.childNodes[2:] if node.tagName == "S" else node.childNodes
-            for child in childs:
-                if not len(child.childNodes):
-                    childs.remove(child)
-            tree = Tree(node.tagName, list(map(traverse, childs)))
-            if (
-                self._join_clitics
-                and len(tree) > 1
-                and type(tree[1]) == Tree
-                and tree[1].label() == "CLITIC"
-                and tree[1][0][1] not in {"P", "V"}
-            ):
-                clitic = tree[-1]
-                tree = Tree(tree.label(), list(tree[0]))
-                clitic_join(tree, clitic)
-            if (
-                self._join_verb_parts
-                and len(tree) > 1
-                and type(tree[1]) == Tree
-                and type(tree[0]) == Tree
-                and tree[0].label() == "AUX"
-                and tree[0][0][0] in self._tokenizer.before_verbs
-            ):
-                tree[1][0] = (tree[0][0][0] + " " + tree[1][0][0], tree[1][0][1])
-                tree.remove(tree[0])
-            if (
-                self._join_verb_parts
-                and len(tree.leaves()) > 1
-                and tree.leaves()[-1][0] in self._tokenizer.after_verbs
-                and tree.leaves()[-2][0] in self._tokenizer.verbe
-            ):
-                tree[1][0] = (
-                    tree[0].leaves()[-1][0] + " " + tree[1][0][0],
-                    tree[1][0][1],
-                )
-                path = tree.leaf_treeposition(len(tree.leaves()) - 2)
-                removingtree = tree
-                while len(path) > 2:
-                    removingtree = removingtree[path[0]]
-                    path = path[1:]
-                removingtree.remove(Tree(tree.pos()[-2][1], [tree.pos()[-2][0]]))
-            if (
-                self._join_verb_parts
-                and len(tree.leaves()) > 1
-                and tree.leaves()[-1][0] in self._tokenizer.after_verbs
-                and tree.leaves()[-2][0] in self._tokenizer.verbe
-            ):
-                tree[1][0] = (
-                    tree[0].leaves()[-1][0] + " " + tree[1][0][0],
-                    tree[1][0][1],
-                )
-                path = tree.leaf_treeposition(len(tree.leaves()) - 2)
-                removingtree = tree
-                while len(path) > 2:
-                    removingtree = removingtree[path[0]]
-                    path = path[1:]
-                removingtree.remove(Tree(tree.pos()[-2][1], [tree.pos()[-2][0]]))
-            return tree
-
-        for doc in self.docs():
-            for s in doc.getElementsByTagName("S"):
-                traverse(s)
-                yield traverse(s)
-
-    def sents(self: "TreebankReader") -> Iterator[List[Tuple[str, str]]]:
-        """جملات را به شکل مجموعه‌ای از `(توکن،برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> treebank = TreebankReader(root='corpora/treebank')
-            >>> next(treebank.sents())
-            [('دنیای', 'Ne'), ('آدولف', 'N'), ('بورن', 'N'), ('دنیای', 'Ne'), ('اتفاقات', 'Ne'), ('رویایی', 'AJ'), ('است', 'V'), ('.', 'PUNC')]
-
-        Yields:
-            جملهٔ بعدی.
-
-        """
-        for tree in self.trees():
-            yield tree.leaves()
-
-    def chunked_trees(self: "TreebankReader") -> Iterator[str]:
-        """ساختار درختی را به شکل تقطیع شده برمی‌گرداند.
-
-        Examples:
-            >>> from .Chunker import tree2brackets
-            >>> treebank = TreebankReader(root='corpora/treebank')
-            >>> tree2brackets(next(treebank.chunked_trees()))
-            '[دنیای آدولف بورن NP] [دنیای اتفاقات رویایی NP] [است VP] .'
-
-        Yields:
-            درخت تقطیع شدهٔ بعدی.
-
-        """
-
-        def collapse(node, label):
-            return Tree(label, [Tree(pos[1], [pos[0]]) for pos in node.pos()])
-
-        def traverse(node, parent, chunks):
-            label = node.label()
-
-            if label.count("-nid") > 0:
-                label = label.replace("-nid", "")
-            if label.count("-nid") > 0:
-                label = label.replace("-nid", "")
-            if label.count("-DiscA") > 0:
-                label = label.replace("-DiscA", "")
-
-            if label in {"CLITIC", "CLITICS"}:
-                if node[0][1] == "V":
-                    label = "V"
-                elif node[0][1] == "P":
-                    label = "PREP"
-                elif node[0][1] == "DET":
-                    label = "DET"
-                elif node[0][1] == "ADV":
-                    label = "ADV"
-                elif node[0][1] == "PRO":
-                    label = "PRON"
-
-            if label in {"CONJ", "PUNC"} and len(node) == 1:
-                chunks.append(node)
-                return
-
-            if label == "PPC" and len(node) == 1:
-                chunks.append(Tree("PP", [node[0]]))
-                return
-
-            if label == "PREP":
-                chunks.append(Tree("PP", [node]))
-                return
-
-            if label == "PostP":
-                chunks.append(Tree("POSTP", [node]))
-                return
-
-            for leaf in node.pos():
-                if leaf[1] in {"PUNC", "CONJ", "PREP", "PostP"}:
-                    for i in range(len(node)):
-                        traverse(node[i], node, chunks)
-                    return
-
-            if label == "NPA" and parent.label() in {"CPC", "PPC"}:
-                chunks.append(collapse(node, "NP"))
-                return
-
-            if label == "NPA" and len(node) >= 1 and node[0].label() == "ADV":
-                chunks.append(collapse(node, "NP"))
-                return
-
-            if label in {
-                "NPC",
-                "N",
-                "INFV",
-                "DPA",
-                "CLASS",
-                "DPC",
-                "DEM",
-                "INTJ",
-                "MN",
-                "PRON",
-                "DET",
-                "NUM",
-                "RES",
-            }:
-                chunks.append(collapse(node, "NP"))
-                return
-
-            if (
-                label == "NPA"
-                and len(node) >= 2
-                and (
-                    node[0].label() == "ADJ"
-                    and node[1].label() == "NPC"
-                    or node[0].label() in {"N", "PRON"}
-                    and node[1].label() in {"ADJ", "ADJPA", "N"}
-                    or node[0].label() == "NUM"
-                    and node[1].label() in {"N", "NPC", "MN", "NUM"}
-                    or node[0].label() in {"N", "NPC", "MN"}
-                    and node[1].label() == "NUM"
-                    or node[0].label() == "NPC"
-                    and node[1].label() == "ADJ"
-                    or node[0].label() == "NPA"
-                    and node[1].label() != "NPC"
-                    or node[1].label() == "NPA"
-                    and node[0].label() != "NPC"
-                )
-            ):
-                chunks.append(collapse(node, "NP"))
-                return
-
-            if label == "DPC" and len(node) >= 2:
-                chunkable = True
-                for leaf in node[1].pos():
-                    if leaf[1] in {"PUNC", "CONJ", "PREP", "PostP"}:
-                        chunkable = False
-                if node[1].label() in {"N", "NPA", "NPC"} and chunkable:
-                    chunks.append(collapse(node, "NP"))
-                    return
-
-            if label == "DPA" and len(node) >= 2 and node[1].label() == "ADV":
-                chunks.append(collapse(node, "ADVP"))
-                return
-
-            if label in {"MV", "V", "AUX", "PPARV"}:
-                chunks.append(Tree("VP", [node]))
-                return
-
-            if label in {"ADJ", "ADJPC", "MADJ", "ADVPA"}:
-                chunks.append(Tree("ADJP", [node]))
-                return
-
-            if label in {"ADV", "MADV", "ADVPC"}:
-                chunks.append(Tree("ADVP", [node]))
-                return
-
-            if type(node[0]) != Tree:
-                chunks.append(node)
-                return
-
-            for i in range(len(node)):
-                traverse(node[i], node, chunks)
-
-        for tree in self.trees():
-            chunks = []
-            traverse(tree, None, chunks)
-            for i in range(len(chunks)):
-                if chunks[i].label() in {"PUNC", "CONJ"}:
-                    chunks[i] = chunks[i][0]
-                else:
-                    chunks[i] = Tree(chunks[i].label(), chunks[i].leaves())
-            yield Tree("S", chunks)
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ تری‌بانک است.
+
+پیکرهٔ تری‌بانک حاوی هزاران جملهٔ برچسب‌خورده با اطلاعات نحوی و ساخت‌واژی است.
+
+"""
+
+
+import os
+import re
+import sys
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import Iterator
+from typing import List
+from typing import Tuple
+from xml.dom import minidom
+
+from nltk.tree import Tree
+
+from ..word_tokenizer import WordTokenizer
+
+
+def coarse_pos_e(tags: List[str]) -> List[str]:
+    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_e(['Nasp---', 'pers', 'prop'])
+        'N'
+
+    Args:
+        tags: لیست برچسب‌های ریز.
+
+    Returns:
+        لیست برچسب‌های درشت.
+
+    """
+    mapping = {
+        "N": "N",
+        "V": "V",
+        "A": "AJ",
+        "D": "ADV",
+        "Z": "PRO",
+        "T": "DET",
+        "E": "P",
+        "P": "POSTP",
+        "U": "NUM",
+        "J": "CONJ",
+        "O": "PUNC",
+        "R": "RES",
+        "L": "CL",
+        "I": "INT",
+    }
+    try:
+        if tags[0][0] == "C":
+            if "pronominal" in tags:
+                tags[0] = "Z"
+            elif "verb" in tags:
+                tags[0] = "V"
+            elif "prep" in tags:
+                tags[0] = "E"
+            elif "adv" in tags:
+                tags[0] = "D"
+            elif "det" in tags:
+                tags[0] = "T"
+        return mapping[tags[0][0]] + ("e" if "ezafe" in tags else "")
+    except Exception:
+        return ""
+
+
+class TreebankReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ تری‌بانک است.
+
+    Args:
+        root: مسیر فولدر حاوی فایل‌های پیکره
+        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
+        join_clitics: اگر `True‍` باشد واژه‌بست‌ها را به کلمهٔ مادر می‌چسباند.
+        join_verb_parts: اگر `True` باشد افعال چندبخشی را با _ به هم می‌چسباند.
+
+    """
+
+    def __init__(
+        self: "TreebankReader",
+        root: str,
+        pos_map: str = coarse_pos_e,
+        join_clitics: bool = False,
+        join_verb_parts: bool = False,
+    ) -> None:
+        self._root = root
+        self._pos_map = pos_map if pos_map else lambda tags: ",".join(tags)
+        self._join_clitics = join_clitics
+        self._join_verb_parts = join_verb_parts
+        self._tokenizer = WordTokenizer()
+
+    def docs(self: "TreebankReader") -> Iterator[Any]:
+        """اسناد موجود در پیکره را برمی‌گرداند.
+
+        Yields:
+            سند بعدی.
+
+        """
+        for root, _dirs, files in os.walk(self._root):
+            for name in sorted(files):
+                try:
+                    with Path.open(
+                        Path(root) / name,
+                        encoding="utf8",
+                    ) as treebank_file:
+                        raw = re.sub(r"\n *", "", treebank_file.read())
+                        yield minidom.parseString(raw.encode("utf8"))
+                except Exception as e:
+                    print("error in reading", name, e, file=sys.stderr)
+
+    def trees(self: "TreebankReader") -> Iterator[str]:
+        """ساختارهای درختی موجود در پیکره را برمی‌گرداند.
+
+        Examples:
+            >>> treebank = TreebankReader(root='corpora/treebank')
+            >>> print(next(treebank.trees()))
+            (S
+            (VPS
+                    (NPC (N دنیای/Ne) (MN (N آدولف/N) (N بورن/N)))
+                    (VPC
+                    (NPC (N دنیای/Ne) (NPA (N اتفاقات/Ne) (ADJ رویایی/AJ)))
+                    (V است/V)))
+            (PUNC ./PUNC))
+
+        Yields:
+            ساختار درختی بعدی.
+
+        """
+
+        def traverse(node: str) -> Tree:
+            def extract_tags(w: str):
+                pos = [w.getAttribute("lc") if w.getAttribute("lc") else None]
+                if w.getAttribute("clitic") in {
+                    "ezafe",
+                    "pronominal",
+                    "verb",
+                    "prep",
+                    "adv",
+                    "det",
+                }:
+                    pos.append(w.getAttribute("clitic"))
+                if w.getAttribute("ne_sort"):
+                    pos.append(w.getAttribute("ne_sort"))
+                if w.getAttribute("n_type"):
+                    pos.append(w.getAttribute("n_type"))
+                if w.getAttribute("ya_type"):
+                    pos.append(w.getAttribute("ya_type"))
+                if w.getAttribute("ke_type"):
+                    pos.append(w.getAttribute("ke_type"))
+                if w.getAttribute("type"):
+                    pos.append(w.getAttribute("type"))
+                if w.getAttribute("kind"):
+                    pos.append(w.getAttribute("kind"))
+                return pos
+
+            def clitic_join(tree: Tree, clitic: Dict):
+                if type(tree[-1]) == Tree:
+                    return clitic_join(tree[-1], clitic)
+
+                if clitic[0][0][0] == "ا":
+                    clitic[0] = ("‌" + clitic[0][0], clitic[0][1])
+                tree[-1] = (tree[-1][0] + clitic[0][0], clitic[0][1])
+                tree.set_label("CLITICS")
+                return None
+
+            if not len(node.childNodes):
+                return None
+            first = node.childNodes[0]
+
+            if first.nodeName == "w":
+                pos = extract_tags(first)
+                return Tree(
+                    node.nodeName,
+                    [
+                        (self._pos_map(pos),),
+                    ],
+                )
+            childs = node.childNodes[2:] if node.tagName == "S" else node.childNodes
+            for child in childs:
+                if not len(child.childNodes):
+                    childs.remove(child)
+            tree = Tree(node.tagName, list(map(traverse, childs)))
+            if (
+                self._join_clitics
+                and len(tree) > 1
+                and type(tree[1]) == Tree
+                and tree[1].label() == "CLITIC"
+                and tree[1][0][1] not in {"P", "V"}
+            ):
+                clitic = tree[-1]
+                tree = Tree(tree.label(), list(tree[0]))
+                clitic_join(tree, clitic)
+            if (
+                self._join_verb_parts
+                and len(tree) > 1
+                and type(tree[1]) == Tree
+                and type(tree[0]) == Tree
+                and tree[0].label() == "AUX"
+                and tree[0][0][0] in self._tokenizer.before_verbs
+            ):
+                tree[1][0] = (tree[0][0][0] + " " + tree[1][0][0], tree[1][0][1])
+                tree.remove(tree[0])
+            if (
+                self._join_verb_parts
+                and len(tree.leaves()) > 1
+                and tree.leaves()[-1][0] in self._tokenizer.after_verbs
+                and tree.leaves()[-2][0] in self._tokenizer.verbe
+            ):
+                tree[1][0] = (
+                    tree[0].leaves()[-1][0] + " " + tree[1][0][0],
+                    tree[1][0][1],
+                )
+                path = tree.leaf_treeposition(len(tree.leaves()) - 2)
+                removingtree = tree
+                while len(path) > 2:
+                    removingtree = removingtree[path[0]]
+                    path = path[1:]
+                removingtree.remove(Tree(tree.pos()[-2][1], [tree.pos()[-2][0]]))
+            if (
+                self._join_verb_parts
+                and len(tree.leaves()) > 1
+                and tree.leaves()[-1][0] in self._tokenizer.after_verbs
+                and tree.leaves()[-2][0] in self._tokenizer.verbe
+            ):
+                tree[1][0] = (
+                    tree[0].leaves()[-1][0] + " " + tree[1][0][0],
+                    tree[1][0][1],
+                )
+                path = tree.leaf_treeposition(len(tree.leaves()) - 2)
+                removingtree = tree
+                while len(path) > 2:
+                    removingtree = removingtree[path[0]]
+                    path = path[1:]
+                removingtree.remove(Tree(tree.pos()[-2][1], [tree.pos()[-2][0]]))
+            return tree
+
+        for doc in self.docs():
+            for s in doc.getElementsByTagName("S"):
+                traverse(s)
+                yield traverse(s)
+
+    def sents(self: "TreebankReader") -> Iterator[List[Tuple[str, str]]]:
+        """جملات را به شکل مجموعه‌ای از `(توکن،برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> treebank = TreebankReader(root='corpora/treebank')
+            >>> next(treebank.sents())
+            [('دنیای', 'Ne'), ('آدولف', 'N'), ('بورن', 'N'), ('دنیای', 'Ne'), ('اتفاقات', 'Ne'), ('رویایی', 'AJ'), ('است', 'V'), ('.', 'PUNC')]
+
+        Yields:
+            جملهٔ بعدی.
+
+        """
+        for tree in self.trees():
+            yield tree.leaves()
+
+    def chunked_trees(self: "TreebankReader") -> Iterator[str]:
+        """ساختار درختی را به شکل تقطیع شده برمی‌گرداند.
+
+        Examples:
+            >>> from .Chunker import tree2brackets
+            >>> treebank = TreebankReader(root='corpora/treebank')
+            >>> tree2brackets(next(treebank.chunked_trees()))
+            '[دنیای آدولف بورن NP] [دنیای اتفاقات رویایی NP] [است VP] .'
+
+        Yields:
+            درخت تقطیع شدهٔ بعدی.
+
+        """
+
+        def collapse(node, label):
+            return Tree(label, [Tree(pos[1], [pos[0]]) for pos in node.pos()])
+
+        def traverse(node, parent, chunks):
+            label = node.label()
+
+            if label.count("-nid") > 0:
+                label = label.replace("-nid", "")
+            if label.count("-nid") > 0:
+                label = label.replace("-nid", "")
+            if label.count("-DiscA") > 0:
+                label = label.replace("-DiscA", "")
+
+            if label in {"CLITIC", "CLITICS"}:
+                if node[0][1] == "V":
+                    label = "V"
+                elif node[0][1] == "P":
+                    label = "PREP"
+                elif node[0][1] == "DET":
+                    label = "DET"
+                elif node[0][1] == "ADV":
+                    label = "ADV"
+                elif node[0][1] == "PRO":
+                    label = "PRON"
+
+            if label in {"CONJ", "PUNC"} and len(node) == 1:
+                chunks.append(node)
+                return
+
+            if label == "PPC" and len(node) == 1:
+                chunks.append(Tree("PP", [node[0]]))
+                return
+
+            if label == "PREP":
+                chunks.append(Tree("PP", [node]))
+                return
+
+            if label == "PostP":
+                chunks.append(Tree("POSTP", [node]))
+                return
+
+            for leaf in node.pos():
+                if leaf[1] in {"PUNC", "CONJ", "PREP", "PostP"}:
+                    for i in range(len(node)):
+                        traverse(node[i], node, chunks)
+                    return
+
+            if label == "NPA" and parent.label() in {"CPC", "PPC"}:
+                chunks.append(collapse(node, "NP"))
+                return
+
+            if label == "NPA" and len(node) >= 1 and node[0].label() == "ADV":
+                chunks.append(collapse(node, "NP"))
+                return
+
+            if label in {
+                "NPC",
+                "N",
+                "INFV",
+                "DPA",
+                "CLASS",
+                "DPC",
+                "DEM",
+                "INTJ",
+                "MN",
+                "PRON",
+                "DET",
+                "NUM",
+                "RES",
+            }:
+                chunks.append(collapse(node, "NP"))
+                return
+
+            if (
+                label == "NPA"
+                and len(node) >= 2
+                and (
+                    node[0].label() == "ADJ"
+                    and node[1].label() == "NPC"
+                    or node[0].label() in {"N", "PRON"}
+                    and node[1].label() in {"ADJ", "ADJPA", "N"}
+                    or node[0].label() == "NUM"
+                    and node[1].label() in {"N", "NPC", "MN", "NUM"}
+                    or node[0].label() in {"N", "NPC", "MN"}
+                    and node[1].label() == "NUM"
+                    or node[0].label() == "NPC"
+                    and node[1].label() == "ADJ"
+                    or node[0].label() == "NPA"
+                    and node[1].label() != "NPC"
+                    or node[1].label() == "NPA"
+                    and node[0].label() != "NPC"
+                )
+            ):
+                chunks.append(collapse(node, "NP"))
+                return
+
+            if label == "DPC" and len(node) >= 2:
+                chunkable = True
+                for leaf in node[1].pos():
+                    if leaf[1] in {"PUNC", "CONJ", "PREP", "PostP"}:
+                        chunkable = False
+                if node[1].label() in {"N", "NPA", "NPC"} and chunkable:
+                    chunks.append(collapse(node, "NP"))
+                    return
+
+            if label == "DPA" and len(node) >= 2 and node[1].label() == "ADV":
+                chunks.append(collapse(node, "ADVP"))
+                return
+
+            if label in {"MV", "V", "AUX", "PPARV"}:
+                chunks.append(Tree("VP", [node]))
+                return
+
+            if label in {"ADJ", "ADJPC", "MADJ", "ADVPA"}:
+                chunks.append(Tree("ADJP", [node]))
+                return
+
+            if label in {"ADV", "MADV", "ADVPC"}:
+                chunks.append(Tree("ADVP", [node]))
+                return
+
+            if type(node[0]) != Tree:
+                chunks.append(node)
+                return
+
+            for i in range(len(node)):
+                traverse(node[i], node, chunks)
+
+        for tree in self.trees():
+            chunks = []
+            traverse(tree, None, chunks)
+            for i in range(len(chunks)):
+                if chunks[i].label() in {"PUNC", "CONJ"}:
+                    chunks[i] = chunks[i][0]
+                else:
+                    chunks[i] = Tree(chunks[i].label(), chunks[i].leaves())
+            yield Tree("S", chunks)
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/verbvalency_reader.py` & `hazm-0.9.1/hazm/corpus_readers/verbvalency_reader.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ ظرفیت نحوی افعال فارسی
-است.
-
-پیکرهٔ ظرفیت نحوی افعال فارسی مجموعه‌ای است حاوی اطلاعات مربوط به ظرفیت نحوی
-بیش
-از ۴۵۰۰ فعل در زبان فارسی. در این فرهنگ، متمم‌های اجباری و اختیاری انواع
-فعل‌های
-ساده، مرکب، پیشوندی و عبارات فعلی مشخص شده است. فراوانی فعل‌های مرکب در زبان
-فارسی، نیاز به فرهنگ ظرفیت فعل را در این زبان دوچندان می‌نماید. چرا که شناخت
-فعل‌های مرکب چه از لحاظ انسانی و چه از لحاظ پردازشی کاری دشوار‌تر از شناخت
-فعل‌های ساده است و به همین خاطر فراهم آوردن فهرستی از فعل‌های زبان (که شامل
-فعل‌های مرکب نیز می‌شود) به همراه ساخت‌های ظرفیتی افعال، کمکی شایان برای کارهای
-پردازشی است. از سوی دیگر، بر اساس نظریه وابستگی، ساخت بنیادین جمله را می‌توان
-از
-روی ساخت ظرفیتی فعل جمله به دست آورد و به همین دلیل بر اهمیت دانستن ساخت‌های
-ظرفیتی فعل در متن‌های زبانی افزوده می‌شود.
-
-"""
-
-
-from collections import namedtuple
-from pathlib import Path
-from typing import Iterator
-
-Verb = namedtuple(
-    "Verb",
-    (
-        "past_light_verb",
-        "present_light_verb",
-        "prefix",
-        "nonverbal_element",
-        "preposition",
-        "valency",
-    ),
-)
-
-
-class VerbValencyReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ ظرفیت نحوی افعال فارسی است.
-
-    Args:
-        valency_file: مسیر فایلِ پیکره.
-
-    """
-
-    def __init__(
-        self: "VerbValencyReader", valency_file: str = "corpora/valency.txt",
-    ) -> None:
-        self._valency_file = valency_file
-
-    def verbs(self: "VerbValencyReader") -> Iterator[Verb]:
-        """افعال پیکره را برمی‌گرداند.
-
-        Yields:
-            فعل بعدی.
-
-        """
-        with Path.open(self._valency_file, encoding="utf-8") as valency_file:
-            for line in valency_file:
-                if "بن ماضی" in line:
-                    continue
-
-                line = line.strip().replace("-\t", "\t")
-                parts = line.split("\t")
-                if len(parts) == 6:
-                    yield Verb(*parts)
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ ظرفیت نحوی افعال فارسی
+است.
+
+پیکرهٔ ظرفیت نحوی افعال فارسی مجموعه‌ای است حاوی اطلاعات مربوط به ظرفیت نحوی
+بیش
+از ۴۵۰۰ فعل در زبان فارسی. در این فرهنگ، متمم‌های اجباری و اختیاری انواع
+فعل‌های
+ساده، مرکب، پیشوندی و عبارات فعلی مشخص شده است. فراوانی فعل‌های مرکب در زبان
+فارسی، نیاز به فرهنگ ظرفیت فعل را در این زبان دوچندان می‌نماید. چرا که شناخت
+فعل‌های مرکب چه از لحاظ انسانی و چه از لحاظ پردازشی کاری دشوار‌تر از شناخت
+فعل‌های ساده است و به همین خاطر فراهم آوردن فهرستی از فعل‌های زبان (که شامل
+فعل‌های مرکب نیز می‌شود) به همراه ساخت‌های ظرفیتی افعال، کمکی شایان برای کارهای
+پردازشی است. از سوی دیگر، بر اساس نظریه وابستگی، ساخت بنیادین جمله را می‌توان
+از
+روی ساخت ظرفیتی فعل جمله به دست آورد و به همین دلیل بر اهمیت دانستن ساخت‌های
+ظرفیتی فعل در متن‌های زبانی افزوده می‌شود.
+
+"""
+
+
+from collections import namedtuple
+from pathlib import Path
+from typing import Iterator
+
+Verb = namedtuple(
+    "Verb",
+    (
+        "past_light_verb",
+        "present_light_verb",
+        "prefix",
+        "nonverbal_element",
+        "preposition",
+        "valency",
+    ),
+)
+
+
+class VerbValencyReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ ظرفیت نحوی افعال فارسی است.
+
+    Args:
+        valency_file: مسیر فایلِ پیکره.
+
+    """
+
+    def __init__(
+        self: "VerbValencyReader", valency_file: str = "corpora/valency.txt",
+    ) -> None:
+        self._valency_file = valency_file
+
+    def verbs(self: "VerbValencyReader") -> Iterator[Verb]:
+        """افعال پیکره را برمی‌گرداند.
+
+        Yields:
+            فعل بعدی.
+
+        """
+        with Path.open(self._valency_file, encoding="utf-8") as valency_file:
+            for line in valency_file:
+                if "بن ماضی" in line:
+                    continue
+
+                line = line.strip().replace("-\t", "\t")
+                parts = line.split("\t")
+                if len(parts) == 6:
+                    yield Verb(*parts)
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/wiki_extractor.py` & `hazm-0.9.1/hazm/corpus_readers/wiki_extractor.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,1859 +1,1859 @@
-# -*- coding: utf-8 -*-
-
-# =============================================================================
-#  Copyright (c) 2020. Giuseppe Attardi (attardi@di.unipi.it).
-# =============================================================================
-#  This file is part of Tanl.
-#
-#  Tanl is free software; you can redistribute it and/or modify it
-#  under the terms of the GNU Affero General Public License, version 3,
-#  as published by the Free Software Foundation.
-#
-#  Tanl is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Affero General Public License for more details.
-#
-#  You should have received a copy of the GNU Affero General Public License
-#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-# =============================================================================
-
-import re
-import html
-import json
-from itertools import zip_longest
-from urllib.parse import quote as urlencode
-from html.entities import name2codepoint
-import logging
-import time
-
-# ----------------------------------------------------------------------
-
-# match tail after wikilink
-tailRE = re.compile('\w+')
-syntaxhighlight = re.compile('&lt;syntaxhighlight .*?&gt;(.*?)&lt;/syntaxhighlight&gt;', re.DOTALL)
-
-## PARAMS ####################################################################
-
-##
-# Defined in <siteinfo>
-# We include as default Template, when loading external template file.
-knownNamespaces = set(['Template'])
-
-##
-# Drop these elements from article text
-#
-discardElements = [
-    'gallery', 'timeline', 'noinclude', 'pre',
-    'table', 'tr', 'td', 'th', 'caption', 'div',
-    'form', 'input', 'select', 'option', 'textarea',
-    'ul', 'li', 'ol', 'dl', 'dt', 'dd', 'menu', 'dir',
-    'ref', 'references', 'img', 'imagemap', 'source', 'small'
-]
-
-##
-# Recognize only these namespaces
-# w: Internal links to the Wikipedia
-# wiktionary: Wiki dictionary
-# wikt: shortcut for Wiktionary
-#
-acceptedNamespaces = ['w', 'wiktionary', 'wikt']
-
-
-def get_url(urlbase, uid):
-    return "%s?curid=%s" % (urlbase, uid)
-
-
-# ======================================================================
-
-
-def clean(extractor, text, expand_templates=False, html_safe=True):
-    """
-    Transforms wiki markup. If the command line flag --escapedoc is set then the text is also escaped
-    @see https://www.mediawiki.org/wiki/Help:Formatting
-    :param extractor: the Extractor t use.
-    :param text: the text to clean.
-    :param expand_templates: whether to perform template expansion.
-    :param html_safe: whether to convert reserved HTML characters to entities.
-    @return: the cleaned text.
-    """
-
-    if expand_templates:
-        # expand templates
-        # See: http://www.mediawiki.org/wiki/Help:Templates
-        text = extractor.expandTemplates(text)
-    else:
-        # Drop transclusions (template, parser functions)
-        text = dropNested(text, r'{{', r'}}')
-
-    # Drop tables
-    text = dropNested(text, r'{\|', r'\|}')
-
-    # replace external links
-    text = replaceExternalLinks(text)
-
-    # replace internal links
-    text = replaceInternalLinks(text)
-
-    # drop MagicWords behavioral switches
-    text = magicWordsRE.sub('', text)
-
-    # ############### Process HTML ###############
-
-    # turn into HTML, except for the content of <syntaxhighlight>
-    res = ''
-    cur = 0
-    for m in syntaxhighlight.finditer(text):
-        end = m.end()
-        res += unescape(text[cur:m.start()]) + m.group(1)
-        cur = end
-    text = res + unescape(text[cur:])
-
-    # Handle bold/italic/quote
-    if extractor.HtmlFormatting:
-        text = bold_italic.sub(r'<b>\1</b>', text)
-        text = bold.sub(r'<b>\1</b>', text)
-        text = italic.sub(r'<i>\1</i>', text)
-    else:
-        text = bold_italic.sub(r'\1', text)
-        text = bold.sub(r'\1', text)
-        text = italic_quote.sub(r'"\1"', text)
-        text = italic.sub(r'"\1"', text)
-        text = quote_quote.sub(r'"\1"', text)
-    # residuals of unbalanced quotes
-    text = text.replace("'''", '').replace("''", '"')
-
-    # Collect spans
-
-    spans = []
-    # Drop HTML comments
-    for m in comment.finditer(text):
-        spans.append((m.start(), m.end()))
-
-    # Drop self-closing tags
-    for pattern in selfClosing_tag_patterns:
-        for m in pattern.finditer(text):
-            spans.append((m.start(), m.end()))
-
-    # Drop ignored tags
-    for left, right in ignored_tag_patterns:
-        for m in left.finditer(text):
-            spans.append((m.start(), m.end()))
-        for m in right.finditer(text):
-            spans.append((m.start(), m.end()))
-
-    # Bulk remove all spans
-    text = dropSpans(spans, text)
-
-    # Drop discarded elements
-    for tag in discardElements:
-        text = dropNested(text, r'<\s*%s\b[^>/]*>' % tag, r'<\s*/\s*%s>' % tag)
-
-    if not extractor.HtmlFormatting:
-        # Turn into text what is left (&amp;nbsp;) and <syntaxhighlight>
-        text = unescape(text)
-
-    # Expand placeholders
-    for pattern, placeholder in placeholder_tag_patterns:
-        index = 1
-        for match in pattern.finditer(text):
-            text = text.replace(match.group(), '%s_%d' % (placeholder, index))
-            index += 1
-
-    text = text.replace('<<', u'«').replace('>>', u'»')
-
-    #############################################
-
-    # Cleanup text
-    text = text.replace('\t', ' ')
-    text = spaces.sub(' ', text)
-    text = dots.sub('...', text)
-    text = re.sub(u' (,:\.\)\]»)', r'\1', text)
-    text = re.sub(u'(\[\(«) ', r'\1', text)
-    text = re.sub(r'\n\W+?\n', '\n', text, flags=re.U)  # lines with only punctuations
-    text = text.replace(',,', ',').replace(',.', '.')
-    if html_safe:
-        text = html.escape(text, quote=False)
-    return text
-
-
-# skip level 1, it is page name level
-section = re.compile(r'(==+)\s*(.*?)\s*\1')
-
-listOpen = {'*': '<ul>', '#': '<ol>', ';': '<dl>', ':': '<dl>'}
-listClose = {'*': '</ul>', '#': '</ol>', ';': '</dl>', ':': '</dl>'}
-listItem = {'*': '<li>%s</li>', '#': '<li>%s</<li>', ';': '<dt>%s</dt>',
-            ':': '<dd>%s</dd>'}
-
-
-def compact(text, mark_headers=False):
-    """Deal with headers, lists, empty sections, residuals of tables.
-    :param text: convert to HTML
-    """
-
-    page = []  # list of paragraph
-    headers = {}  # Headers for unfilled sections
-    emptySection = False  # empty sections are discarded
-    listLevel = ''  # nesting of lists
-
-    for line in text.split('\n'):
-
-        if not line:
-            if len(listLevel):    # implies Extractor.HtmlFormatting
-                for c in reversed(listLevel):
-                    page.append(listClose[c])
-                    listLevel = ''
-            continue
-
-        # Handle section titles
-        m = section.match(line)
-        if m:
-            title = m.group(2)
-            lev = len(m.group(1))
-            if Extractor.HtmlFormatting:
-                page.append("<h%d>%s</h%d>" % (lev, title, lev))
-            if title and title[-1] not in '!?':
-                title += '.'
-
-            if mark_headers:
-                title = "## " + title
-
-            headers[lev] = title
-            # drop previous headers
-            headers = { k:v for k,v in headers.items() if k <= lev }
-            emptySection = True
-            continue
-        # Handle page title
-        if line.startswith('++'):
-            title = line[2:-2]
-            if title:
-                if title[-1] not in '!?':
-                    title += '.'
-                page.append(title)
-        # handle indents
-        elif line[0] == ':':
-            page.append(line.lstrip(':'))
-        # handle lists
-        # @see https://www.mediawiki.org/wiki/Help:Formatting
-        elif line[0] in '*#;':
-            if Extractor.HtmlFormatting:
-                # close extra levels
-                l = 0
-                for c in listLevel:
-                    if l < len(line) and c != line[l]:
-                        for extra in reversed(listLevel[l:]):
-                            page.append(listClose[extra])
-                        listLevel = listLevel[:l]
-                        break
-                    l += 1
-                if l < len(line) and line[l] in '*#;:':
-                    # add new level (only one, no jumps)
-                    # FIXME: handle jumping levels
-                    type = line[l]
-                    page.append(listOpen[type])
-                    listLevel += type
-                    line = line[l+1:].strip()
-                else:
-                    # continue on same level
-                    type = line[l-1]
-                    line = line[l:].strip()
-                page.append(listItem[type] % line)
-            else:
-                continue
-        elif len(listLevel):    # implies Extractor.HtmlFormatting
-            for c in reversed(listLevel):
-                page.append(listClose[c])
-            listLevel = []
-
-        # Drop residuals of lists
-        elif line[0] in '{|' or line[-1] == '}':
-            continue
-        # Drop irrelevant lines
-        elif (line[0] == '(' and line[-1] == ')') or line.strip('.-') == '':
-            continue
-        elif len(headers):
-            if Extractor.keepSections:
-                items = sorted(headers.items())
-                for (i, v) in items:
-                    page.append(v)
-            headers.clear()
-            page.append(line)  # first line
-            emptySection = False
-        elif not emptySection:
-            page.append(line)
-            # dangerous
-            # # Drop preformatted
-            # elif line[0] == ' ':
-            #     continue
-
-    return page
-
-
-# ----------------------------------------------------------------------
-
-def dropNested(text, openDelim, closeDelim):
-    """
-    A matching function for nested expressions, e.g. namespaces and tables.
-    """
-    openRE = re.compile(openDelim, re.IGNORECASE)
-    closeRE = re.compile(closeDelim, re.IGNORECASE)
-    # partition text in separate blocks { } { }
-    spans = []  # pairs (s, e) for each partition
-    nest = 0  # nesting level
-    start = openRE.search(text, 0)
-    if not start:
-        return text
-    end = closeRE.search(text, start.end())
-    next = start
-    while end:
-        next = openRE.search(text, next.end())
-        if not next:  # termination
-            while nest:  # close all pending
-                nest -= 1
-                end0 = closeRE.search(text, end.end())
-                if end0:
-                    end = end0
-                else:
-                    break
-            spans.append((start.start(), end.end()))
-            break
-        while end.end() < next.start():
-            # { } {
-            if nest:
-                nest -= 1
-                # try closing more
-                last = end.end()
-                end = closeRE.search(text, end.end())
-                if not end:  # unbalanced
-                    if spans:
-                        span = (spans[0][0], last)
-                    else:
-                        span = (start.start(), last)
-                    spans = [span]
-                    break
-            else:
-                spans.append((start.start(), end.end()))
-                # advance start, find next close
-                start = next
-                end = closeRE.search(text, next.end())
-                break  # { }
-        if next != start:
-            # { { }
-            nest += 1
-    # collect text outside partitions
-    return dropSpans(spans, text)
-
-
-def dropSpans(spans, text):
-    """
-    Drop from text the blocks identified in :param spans:, possibly nested.
-    """
-    spans.sort()
-    res = ''
-    offset = 0
-    for s, e in spans:
-        if offset <= s:  # handle nesting
-            if offset < s:
-                res += text[offset:s]
-            offset = e
-    res += text[offset:]
-    return res
-
-
-# ----------------------------------------------------------------------
-# External links
-
-# from: https://doc.wikimedia.org/mediawiki-core/master/php/DefaultSettings_8php_source.html
-
-wgUrlProtocols = [
-    'bitcoin:', 'ftp://', 'ftps://', 'geo:', 'git://', 'gopher://', 'http://',
-    'https://', 'irc://', 'ircs://', 'magnet:', 'mailto:', 'mms://', 'news:',
-    'nntp://', 'redis://', 'sftp://', 'sip:', 'sips:', 'sms:', 'ssh://',
-    'svn://', 'tel:', 'telnet://', 'urn:', 'worldwind://', 'xmpp:', '//'
-]
-
-# from: https://doc.wikimedia.org/mediawiki-core/master/php/Parser_8php_source.html
-
-# Constants needed for external link processing
-# Everything except bracket, space, or control characters
-# \p{Zs} is unicode 'separator, space' category. It covers the space 0x20
-# as well as U+3000 is IDEOGRAPHIC SPACE for bug 19052
-EXT_LINK_URL_CLASS = r'[^][<>"\x00-\x20\x7F\s]'
-ExtLinkBracketedRegex = re.compile(
-    '(?i)\[((' + '|'.join(wgUrlProtocols) + ')' + EXT_LINK_URL_CLASS + r'+)\s*([^\]\x00-\x08\x0a-\x1F]*?)\]',
-    re.S | re.U)
-EXT_IMAGE_REGEX = re.compile(
-    r"""(?i)^(http://|https://)([^][<>"\x00-\x20\x7F\s]+)
-    /([A-Za-z0-9_.,~%\-+&;#*?!=()@\x80-\xFF]+)\.(gif|png|jpg|jpeg)$""",
-    re.X | re.S | re.U)
-
-
-def replaceExternalLinks(text):
-    s = ''
-    cur = 0
-    for m in ExtLinkBracketedRegex.finditer(text):
-        s += text[cur:m.start()]
-        cur = m.end()
-
-        url = m.group(1)
-        label = m.group(3)
-
-        # # The characters '<' and '>' (which were escaped by
-        # # removeHTMLtags()) should not be included in
-        # # URLs, per RFC 2396.
-        # m2 = re.search('&(lt|gt);', url)
-        # if m2:
-        #     link = url[m2.end():] + ' ' + link
-        #     url = url[0:m2.end()]
-
-        # If the link text is an image URL, replace it with an <img> tag
-        # This happened by accident in the original parser, but some people used it extensively
-        m = EXT_IMAGE_REGEX.match(label)
-        if m:
-            label = makeExternalImage(label)
-
-        # Use the encoded URL
-        # This means that users can paste URLs directly into the text
-        # Funny characters like ö aren't valid in URLs anyway
-        # This was changed in August 2004
-        s += makeExternalLink(url, label)  # + trail
-
-    return s + text[cur:]
-
-
-def makeExternalLink(url, anchor):
-    """Function applied to wikiLinks"""
-    if Extractor.keepLinks:
-        return '<a href="%s">%s</a>' % (urlencode(url), anchor)
-    else:
-        return anchor
-
-
-def makeExternalImage(url, alt=''):
-    if Extractor.keepLinks:
-        return '<img src="%s" alt="%s">' % (url, alt)
-    else:
-        return alt
-
-
-# ----------------------------------------------------------------------
-# WikiLinks
-# See https://www.mediawiki.org/wiki/Help:Links#Internal_links
-
-# Can be nested [[File:..|..[[..]]..|..]], [[Category:...]], etc.
-# Also: [[Help:IPA for Catalan|[andora]]]
-
-
-def replaceInternalLinks(text):
-    """
-    Replaces external links of the form:
-    [[title |...|label]]trail
-
-    with title concatenated with trail, when present, e.g. 's' for plural.
-    """
-    # call this after removal of external links, so we need not worry about
-    # triple closing ]]].
-    cur = 0
-    res = ''
-    for s, e in findBalanced(text, ['[['], [']]']):
-        m = tailRE.match(text, e)
-        if m:
-            trail = m.group(0)
-            end = m.end()
-        else:
-            trail = ''
-            end = e
-        inner = text[s + 2:e - 2]
-        # find first |
-        pipe = inner.find('|')
-        if pipe < 0:
-            title = inner
-            label = title
-        else:
-            title = inner[:pipe].rstrip()
-            # find last |
-            curp = pipe + 1
-            for s1, e1 in findBalanced(inner, ['[['], [']]']):
-                last = inner.rfind('|', curp, s1)
-                if last >= 0:
-                    pipe = last  # advance
-                curp = e1
-            label = inner[pipe + 1:].strip()
-        res += text[cur:s] + makeInternalLink(title, label) + trail
-        cur = end
-    return res + text[cur:]
-
-
-def makeInternalLink(title, label):
-    colon = title.find(':')
-    if colon > 0 and title[:colon] not in acceptedNamespaces:
-        return ''
-    if colon == 0:
-        # drop also :File:
-        colon2 = title.find(':', colon + 1)
-        if colon2 > 1 and title[colon + 1:colon2] not in acceptedNamespaces:
-            return ''
-    if Extractor.keepLinks:
-        return '<a href="%s">%s</a>' % (urlencode(title), label)
-    else:
-        return label
-
-
-# ----------------------------------------------------------------------
-# variables
-
-
-class MagicWords():
-
-    """
-    One copy in each Extractor.
-
-    @see https://doc.wikimedia.org/mediawiki-core/master/php/MagicWord_8php_source.html
-    """
-    names = [
-        '!',
-        'currentmonth',
-        'currentmonth1',
-        'currentmonthname',
-        'currentmonthnamegen',
-        'currentmonthabbrev',
-        'currentday',
-        'currentday2',
-        'currentdayname',
-        'currentyear',
-        'currenttime',
-        'currenthour',
-        'localmonth',
-        'localmonth1',
-        'localmonthname',
-        'localmonthnamegen',
-        'localmonthabbrev',
-        'localday',
-        'localday2',
-        'localdayname',
-        'localyear',
-        'localtime',
-        'localhour',
-        'numberofarticles',
-        'numberoffiles',
-        'numberofedits',
-        'articlepath',
-        'pageid',
-        'sitename',
-        'server',
-        'servername',
-        'scriptpath',
-        'stylepath',
-        'pagename',
-        'pagenamee',
-        'fullpagename',
-        'fullpagenamee',
-        'namespace',
-        'namespacee',
-        'namespacenumber',
-        'currentweek',
-        'currentdow',
-        'localweek',
-        'localdow',
-        'revisionid',
-        'revisionday',
-        'revisionday2',
-        'revisionmonth',
-        'revisionmonth1',
-        'revisionyear',
-        'revisiontimestamp',
-        'revisionuser',
-        'revisionsize',
-        'subpagename',
-        'subpagenamee',
-        'talkspace',
-        'talkspacee',
-        'subjectspace',
-        'subjectspacee',
-        'talkpagename',
-        'talkpagenamee',
-        'subjectpagename',
-        'subjectpagenamee',
-        'numberofusers',
-        'numberofactiveusers',
-        'numberofpages',
-        'currentversion',
-        'rootpagename',
-        'rootpagenamee',
-        'basepagename',
-        'basepagenamee',
-        'currenttimestamp',
-        'localtimestamp',
-        'directionmark',
-        'contentlanguage',
-        'numberofadmins',
-        'cascadingsources',
-    ]
-
-    def __init__(self):
-        self.values = {'!': '|'}
-
-    def __getitem__(self, name):
-        return self.values.get(name)
-
-    def __setitem__(self, name, value):
-        self.values[name] = value
-
-    switches = (
-        '__NOTOC__',
-        '__FORCETOC__',
-        '__TOC__',
-        '__TOC__',
-        '__NEWSECTIONLINK__',
-        '__NONEWSECTIONLINK__',
-        '__NOGALLERY__',
-        '__HIDDENCAT__',
-        '__NOCONTENTCONVERT__',
-        '__NOCC__',
-        '__NOTITLECONVERT__',
-        '__NOTC__',
-        '__START__',
-        '__END__',
-        '__INDEX__',
-        '__NOINDEX__',
-        '__STATICREDIRECT__',
-        '__DISAMBIG__'
-    )
-
-
-magicWordsRE = re.compile('|'.join(MagicWords.switches))
-
-
-# =========================================================================
-#
-# MediaWiki Markup Grammar
-# https://www.mediawiki.org/wiki/Preprocessor_ABNF
-
-# xml-char = %x9 / %xA / %xD / %x20-D7FF / %xE000-FFFD / %x10000-10FFFF
-# sptab = SP / HTAB
-
-# ; everything except ">" (%x3E)
-# attr-char = %x9 / %xA / %xD / %x20-3D / %x3F-D7FF / %xE000-FFFD / %x10000-10FFFF
-
-# literal         = *xml-char
-# title           = wikitext-L3
-# part-name       = wikitext-L3
-# part-value      = wikitext-L3
-# part            = ( part-name "=" part-value ) / ( part-value )
-# parts           = [ title *( "|" part ) ]
-# tplarg          = "{{{" parts "}}}"
-# template        = "{{" parts "}}"
-# link            = "[[" wikitext-L3 "]]"
-
-# comment         = "<!--" literal "-->"
-# unclosed-comment = "<!--" literal END
-# ; the + in the line-eating-comment rule was absent between MW 1.12 and MW 1.22
-# line-eating-comment = LF LINE-START *SP +( comment *SP ) LINE-END
-
-# attr            = *attr-char
-# nowiki-element  = "<nowiki" attr ( "/>" / ( ">" literal ( "</nowiki>" / END ) ) )
-
-# wikitext-L2     = heading / wikitext-L3 / *wikitext-L2
-# wikitext-L3     = literal / template / tplarg / link / comment /
-#                   line-eating-comment / unclosed-comment / xmlish-element /
-#                   *wikitext-L3
-
-# ------------------------------------------------------------------------------
-
-selfClosingTags = ('br', 'hr', 'nobr', 'ref', 'references', 'nowiki')
-
-# These tags are dropped, keeping their content.
-# handle 'a' separately, depending on keepLinks
-ignoredTags = (
-    'abbr', 'b', 'big', 'blockquote', 'center', 'cite', 'div', 'em',
-    'font', 'h1', 'h2', 'h3', 'h4', 'hiero', 'i', 'kbd', 'nowiki',
-    'p', 'plaintext', 's', 'span', 'strike', 'strong',
-    'sub', 'sup', 'tt', 'u', 'var'
-)
-
-placeholder_tags = {'math': 'formula', 'code': 'codice'}
-
-
-def normalizeTitle(title):
-    """Normalize title"""
-    # remove leading/trailing whitespace and underscores
-    title = title.strip(' _')
-    # replace sequences of whitespace and underscore chars with a single space
-    title = re.sub(r'[\s_]+', ' ', title)
-
-    m = re.match(r'([^:]*):(\s*)(\S(?:.*))', title)
-    if m:
-        prefix = m.group(1)
-        if m.group(2):
-            optionalWhitespace = ' '
-        else:
-            optionalWhitespace = ''
-        rest = m.group(3)
-
-        ns = normalizeNamespace(prefix)
-        if ns in knownNamespaces:
-            # If the prefix designates a known namespace, then it might be
-            # followed by optional whitespace that should be removed to get
-            # the canonical page name
-            # (e.g., "Category:  Births" should become "Category:Births").
-            title = ns + ":" + ucfirst(rest)
-        else:
-            # No namespace, just capitalize first letter.
-            # If the part before the colon is not a known namespace, then we
-            # must not remove the space after the colon (if any), e.g.,
-            # "3001: The_Final_Odyssey" != "3001:The_Final_Odyssey".
-            # However, to get the canonical page name we must contract multiple
-            # spaces into one, because
-            # "3001:   The_Final_Odyssey" != "3001: The_Final_Odyssey".
-            title = ucfirst(prefix) + ":" + optionalWhitespace + ucfirst(rest)
-    else:
-        # no namespace, just capitalize first letter
-        title = ucfirst(title)
-    return title
-
-
-def unescape(text):
-    """
-    Removes HTML or XML character references and entities from a text string.
-
-    :param text The HTML (or XML) source text.
-    :return The plain text, as a Unicode string, if necessary.
-    """
-
-    def fixup(m):
-        text = m.group(0)
-        code = m.group(1)
-        try:
-            if text[1] == "#":  # character reference
-                if text[2] == "x":
-                    return chr(int(code[1:], 16))
-                else:
-                    return chr(int(code))
-            else:  # named entity
-                return chr(name2codepoint[code])
-        except:
-            return text  # leave as is
-
-    return re.sub("&#?(\w+);", fixup, text)
-
-
-# Match HTML comments
-# The buggy template {{Template:T}} has a comment terminating with just "->"
-comment = re.compile(r'<!--.*?-->', re.DOTALL)
-
-# Match ignored tags
-ignored_tag_patterns = []
-
-
-def ignoreTag(tag):
-    left = re.compile(r'<%s\b.*?>' % tag, re.IGNORECASE | re.DOTALL)  # both <ref> and <reference>
-    right = re.compile(r'</\s*%s>' % tag, re.IGNORECASE)
-    ignored_tag_patterns.append((left, right))
-
-
-def resetIgnoredTags():
-    global ignored_tag_patterns
-    ignored_tag_patterns = []
-
-
-for tag in ignoredTags:
-    ignoreTag(tag)
-
-# Match selfClosing HTML tags
-selfClosing_tag_patterns = [
-    re.compile(r'<\s*%s\b[^>]*/\s*>' % tag, re.DOTALL | re.IGNORECASE) for tag in selfClosingTags
-]
-
-# Match HTML placeholder tags
-placeholder_tag_patterns = [
-    (re.compile(r'<\s*%s(\s*| [^>]+?)>.*?<\s*/\s*%s\s*>' % (tag, tag), re.DOTALL | re.IGNORECASE),
-     repl) for tag, repl in placeholder_tags.items()
-]
-
-# Match preformatted lines
-preformatted = re.compile(r'^ .*?$')
-
-# Match external links (space separates second optional parameter)
-externalLink = re.compile(r'\[\w+[^ ]*? (.*?)]')
-externalLinkNoAnchor = re.compile(r'\[\w+[&\]]*\]')
-
-# Matches bold/italic
-bold_italic = re.compile(r"'''''(.*?)'''''")
-bold = re.compile(r"'''(.*?)'''")
-italic_quote = re.compile(r"''\"([^\"]*?)\"''")
-italic = re.compile(r"''(.*?)''")
-quote_quote = re.compile(r'""([^"]*?)""')
-
-# Matches space
-spaces = re.compile(r' {2,}')
-
-# Matches dots
-dots = re.compile(r'\.{4,}')
-
-# ======================================================================
-
-class Template(list):
-    """
-    A Template is a list of TemplateText or TemplateArgs
-    """
-
-    @classmethod
-    def parse(cls, body):
-        tpl = Template()
-        # we must handle nesting, s.a.
-        # {{{1|{{PAGENAME}}}
-        # {{{italics|{{{italic|}}}
-        # {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|
-        #
-        start = 0
-        for s,e in findMatchingBraces(body, 3):
-            tpl.append(TemplateText(body[start:s]))
-            tpl.append(TemplateArg(body[s+3:e-3]))
-            start = e
-        tpl.append(TemplateText(body[start:])) # leftover
-        return tpl
-
-    def subst(self, params, extractor, depth=0):
-        # We perform parameter substitutions recursively.
-        # We also limit the maximum number of iterations to avoid too long or
-        # even endless loops (in case of malformed input).
-
-        # :see: http://meta.wikimedia.org/wiki/Help:Expansion#Distinction_between_variables.2C_parser_functions.2C_and_templates
-        #
-        # Parameter values are assigned to parameters in two (?) passes.
-        # Therefore a parameter name in a template can depend on the value of
-        # another parameter of the same template, regardless of the order in
-        # which they are specified in the template call, for example, using
-        # Template:ppp containing "{{{{{{p}}}}}}", {{ppp|p=q|q=r}} and even
-        # {{ppp|q=r|p=q}} gives r, but using Template:tvvv containing
-        # "{{{{{{{{{p}}}}}}}}}", {{tvvv|p=q|q=r|r=s}} gives s.
-
-        logging.debug('subst tpl (%d, %d) %s', len(extractor.frame), depth, self)
-
-        if depth > extractor.maxParameterRecursionLevels:
-            extractor.recursion_exceeded_3_errs += 1
-            return ''
-
-        return ''.join([tpl.subst(params, extractor, depth) for tpl in self])
-
-    def __str__(self):
-        return ''.join([str(x) for x in self])
-
-
-class TemplateText(str):
-    """Fixed text of template"""
-
-    def subst(self, params, extractor, depth):
-        return self
-
-
-class TemplateArg():
-    """
-    parameter to a template.
-    Has a name and a default value, both of which are Templates.
-    """
-    def __init__(self, parameter):
-        """
-        :param parameter: the parts of a tplarg.
-        """
-        # the parameter name itself might contain templates, e.g.:
-        #   appointe{{#if:{{{appointer14|}}}|r|d}}14|
-        #   4|{{{{{subst|}}}CURRENTYEAR}}
-
-        # any parts in a tplarg after the first (the parameter default) are
-        # ignored, and an equals sign in the first part is treated as plain text.
-        #logging.debug('TemplateArg %s', parameter)
-
-        parts = splitParts(parameter)
-        self.name = Template.parse(parts[0])
-        if len(parts) > 1:
-            # This parameter has a default value
-            self.default = Template.parse(parts[1])
-        else:
-            self.default = None
-
-    def __str__(self):
-        if self.default:
-            return '{{{%s|%s}}}' % (self.name, self.default)
-        else:
-            return '{{{%s}}}' % self.name
-
-    def subst(self, params, extractor, depth):
-        """
-        Substitute value for this argument from dict :param params:
-        Use :param extractor: to evaluate expressions for name and default.
-        Limit substitution to the maximun :param depth:.
-        """
-        # the parameter name itself might contain templates, e.g.:
-        # appointe{{#if:{{{appointer14|}}}|r|d}}14|
-        paramName = self.name.subst(params, extractor, depth+1)
-        paramName = extractor.expandTemplates(paramName)
-        res = ''
-        if paramName in params:
-            res = params[paramName]  # use parameter value specified in template invocation
-        elif self.default:            # use the default value
-            defaultValue = self.default.subst(params, extractor, depth+1)
-            res =  extractor.expandTemplates(defaultValue)
-        #logging.debug('subst arg %d %s -> %s' % (depth, paramName, res))
-        return res
-
-
-# ======================================================================
-
-substWords = 'subst:|safesubst:'
-
-
-class Extractor():
-    """
-    An extraction task on a article.
-    """
-    ##
-    # Whether to preserve links in output
-    keepLinks = False
-
-    ##
-    # Whether to preserve section titles
-    keepSections = True
-
-    ##
-    # Whether to output text with HTML formatting elements in <doc> files.
-    HtmlFormatting = False
-
-    ##
-    # Whether to produce json instead of the default <doc> output format.
-    toJson = False
-
-    ##
-    # Obtained from TemplateNamespace
-    templatePrefix = ''
-
-    def __init__(self, id, revid, urlbase, title, page):
-        """
-        :param page: a list of lines.
-        """
-        self.id = id
-        self.revid = revid
-        self.url = get_url(urlbase, id)
-        self.title = title
-        self.page = page
-        self.magicWords = MagicWords()
-        self.frame = []
-        self.recursion_exceeded_1_errs = 0  # template recursion within expandTemplates()
-        self.recursion_exceeded_2_errs = 0  # template recursion within expandTemplate()
-        self.recursion_exceeded_3_errs = 0  # parameter recursion
-        self.template_title_errs = 0
-
-    def clean_text(self, text, mark_headers=False, expand_templates=True,
-                   html_safe=True):
-        """
-        :param mark_headers: True to distinguish headers from paragraphs
-          e.g. "## Section 1"
-        """
-        self.magicWords['namespace'] = self.title[:max(0, self.title.find(":"))]
-        #self.magicWords['namespacenumber'] = '0' # for article,
-        self.magicWords['pagename'] = self.title
-        self.magicWords['fullpagename'] = self.title
-        self.magicWords['currentyear'] = time.strftime('%Y')
-        self.magicWords['currentmonth'] = time.strftime('%m')
-        self.magicWords['currentday'] = time.strftime('%d')
-        self.magicWords['currenthour'] = time.strftime('%H')
-        self.magicWords['currenttime'] = time.strftime('%H:%M:%S')
-
-        text = clean(self, text, expand_templates=expand_templates,
-                     html_safe=html_safe)
-
-        text = compact(text, mark_headers=mark_headers)
-        return text
-
-    def extract(self, out, html_safe=True):
-        """
-        :param out: a memory file.
-        :param html_safe: whether to escape HTML entities.
-        """
-        logging.debug("%s\t%s", self.id, self.title)
-        text = ''.join(self.page)
-        text = self.clean_text(text, html_safe=html_safe)
-
-        if self.to_json:
-            json_data = {
-		'id': self.id,
-                'revid': self.revid,
-                'url': self.url,
-                'title': self.title,
-                'text': "\n".join(text)
-            }
-            out_str = json.dumps(json_data)
-            out.write(out_str)
-            out.write('\n')
-        else:
-            header = '<doc id="%s" url="%s" title="%s">\n' % (self.id, self.url, self.title)
-            # Separate header from text with a newline.
-            header += self.title + '\n\n'
-            footer = "\n</doc>\n"
-            out.write(header)
-            out.write('\n'.join(text))
-            out.write('\n')
-            out.write(footer)
-
-        errs = (self.template_title_errs,
-                self.recursion_exceeded_1_errs,
-                self.recursion_exceeded_2_errs,
-                self.recursion_exceeded_3_errs)
-        if any(errs):
-            logging.warn("Template errors in article '%s' (%s): title(%d) recursion(%d, %d, %d)",
-                         self.title, self.id, *errs)
-
-    # ----------------------------------------------------------------------
-    # Expand templates
-
-    maxTemplateRecursionLevels = 30
-    maxParameterRecursionLevels = 16
-
-    # check for template beginning
-    reOpen = re.compile('(?<!{){{(?!{)', re.DOTALL)
-
-    def expandTemplates(self, wikitext):
-        """
-        :param wikitext: the text to be expanded.
-
-        Templates are frequently nested. Occasionally, parsing mistakes may
-        cause template insertion to enter an infinite loop, for instance when
-        trying to instantiate Template:Country
-
-        {{country_{{{1}}}|{{{2}}}|{{{2}}}|size={{{size|}}}|name={{{name|}}}}}
-
-        which is repeatedly trying to insert template 'country_', which is
-        again resolved to Template:Country. The straightforward solution of
-        keeping track of templates that were already inserted for the current
-        article would not work, because the same template may legally be used
-        more than once, with different parameters in different parts of the
-        article.  Therefore, we limit the number of iterations of nested
-        template inclusion.
-
-        """
-        # Test template expansion at:
-        # https://en.wikipedia.org/wiki/Special:ExpandTemplates
-
-        res = ''
-        if len(self.frame) >= self.maxTemplateRecursionLevels:
-            self.recursion_exceeded_1_errs += 1
-            return res
-
-        # logging.debug('<expandTemplates ' + str(len(self.frame)))
-
-        cur = 0
-        # look for matching {{...}}
-        for s, e in findMatchingBraces(wikitext, 2):
-            res += wikitext[cur:s] + self.expandTemplate(wikitext[s + 2:e - 2])
-            cur = e
-        # leftover
-        res += wikitext[cur:]
-        # logging.debug('   expandTemplates> %d %s', len(self.frame), res)
-        return res
-
-    def templateParams(self, parameters):
-        """
-        Build a dictionary with positional or name key to expanded parameters.
-        :param parameters: the parts[1:] of a template, i.e. all except the title.
-        """
-        templateParams = {}
-
-        if not parameters:
-            return templateParams
-        logging.debug('<templateParams: %s', '|'.join(parameters))
-
-        # Parameters can be either named or unnamed. In the latter case, their
-        # name is defined by their ordinal position (1, 2, 3, ...).
-
-        unnamedParameterCounter = 0
-
-        # It's legal for unnamed parameters to be skipped, in which case they
-        # will get default values (if available) during actual instantiation.
-        # That is {{template_name|a||c}} means parameter 1 gets
-        # the value 'a', parameter 2 value is not defined, and parameter 3 gets
-        # the value 'c'.  This case is correctly handled by function 'split',
-        # and does not require any special handling.
-        for param in parameters:
-            # Spaces before or after a parameter value are normally ignored,
-            # UNLESS the parameter contains a link (to prevent possible gluing
-            # the link to the following text after template substitution)
-
-            # Parameter values may contain "=" symbols, hence the parameter
-            # name extends up to the first such symbol.
-
-            # It is legal for a parameter to be specified several times, in
-            # which case the last assignment takes precedence. Example:
-            # "{{t|a|b|c|2=B}}" is equivalent to "{{t|a|B|c}}".
-            # Therefore, we don't check if the parameter has been assigned a
-            # value before, because anyway the last assignment should override
-            # any previous ones.
-            # FIXME: Don't use DOTALL here since parameters may be tags with
-            # attributes, e.g. <div class="templatequotecite">
-            # Parameters may span several lines, like:
-            # {{Reflist|colwidth=30em|refs=
-            # &lt;ref name=&quot;Goode&quot;&gt;Title&lt;/ref&gt;
-
-            # The '=' might occurr within an HTML attribute:
-            #   "&lt;ref name=value"
-            # but we stop at first.
-
-            # The '=' might occurr within quotes:
-            # ''''<span lang="pt-pt" xml:lang="pt-pt">cénicas</span>'''
-
-            m = re.match(" *([^=']*?) *=(.*)", param, re.DOTALL)
-            if m:
-                # This is a named parameter.  This case also handles parameter
-                # assignments like "2=xxx", where the number of an unnamed
-                # parameter ("2") is specified explicitly - this is handled
-                # transparently.
-
-                parameterName = m.group(1).strip()
-                parameterValue = m.group(2)
-
-                if ']]' not in parameterValue:  # if the value does not contain a link, trim whitespace
-                    parameterValue = parameterValue.strip()
-                templateParams[parameterName] = parameterValue
-            else:
-                # this is an unnamed parameter
-                unnamedParameterCounter += 1
-
-                if ']]' not in param:  # if the value does not contain a link, trim whitespace
-                    param = param.strip()
-                templateParams[str(unnamedParameterCounter)] = param
-        logging.debug('   templateParams> %s', '|'.join(templateParams.values()))
-        return templateParams
-
-    def expandTemplate(self, body):
-        """Expands template invocation.
-        :param body: the parts of a template.
-
-        :see http://meta.wikimedia.org/wiki/Help:Expansion for an explanation
-        of the process.
-
-        See in particular: Expansion of names and values
-        http://meta.wikimedia.org/wiki/Help:Expansion#Expansion_of_names_and_values
-
-        For most parser functions all names and values are expanded,
-        regardless of what is relevant for the result. The branching functions
-        (#if, #ifeq, #iferror, #ifexist, #ifexpr, #switch) are exceptions.
-
-        All names in a template call are expanded, and the titles of the
-        tplargs in the template body, after which it is determined which
-        values must be expanded, and for which tplargs in the template body
-        the first part (default).
-
-        In the case of a tplarg, any parts beyond the first are never
-        expanded.  The possible name and the value of the first part is
-        expanded if the title does not match a name in the template call.
-
-        :see code for braceSubstitution at
-        https://doc.wikimedia.org/mediawiki-core/master/php/html/Parser_8php_source.html#3397:
-
-        """
-
-        # template        = "{{" parts "}}"
-
-        # Templates and tplargs are decomposed in the same way, with pipes as
-        # separator, even though eventually any parts in a tplarg after the first
-        # (the parameter default) are ignored, and an equals sign in the first
-        # part is treated as plain text.
-        # Pipes inside inner templates and tplargs, or inside double rectangular
-        # brackets within the template or tplargs are not taken into account in
-        # this decomposition.
-        # The first part is called title, the other parts are simply called parts.
-
-        # If a part has one or more equals signs in it, the first equals sign
-        # determines the division into name = value. Equals signs inside inner
-        # templates and tplargs, or inside double rectangular brackets within the
-        # part are not taken into account in this decomposition. Parts without
-        # equals sign are indexed 1, 2, .., given as attribute in the <name> tag.
-
-        if len(self.frame) >= self.maxTemplateRecursionLevels:
-            self.recursion_exceeded_2_errs += 1
-            # logging.debug('   INVOCATION> %d %s', len(self.frame), body)
-            return ''
-
-        logging.debug('INVOCATION %d %s', len(self.frame), body)
-
-        parts = splitParts(body)
-        # title is the portion before the first |
-        logging.debug('TITLE %s', parts[0].strip())
-        title = self.expandTemplates(parts[0].strip())
-
-        # SUBST
-        # Apply the template tag to parameters without
-        # substituting into them, e.g.
-        # {{subst:t|a{{{p|q}}}b}} gives the wikitext start-a{{{p|q}}}b-end
-        # @see https://www.mediawiki.org/wiki/Manual:Substitution#Partial_substitution
-        subst = False
-        if re.match(substWords, title, re.IGNORECASE):
-            title = re.sub(substWords, '', title, 1, re.IGNORECASE)
-            subst = True
-
-        if title.lower() in self.magicWords.values:
-            return self.magicWords[title.lower()]
-
-        # Parser functions
-        # The first argument is everything after the first colon.
-        # It has been evaluated above.
-        colon = title.find(':')
-        if colon > 1:
-            funct = title[:colon]
-            parts[0] = title[colon + 1:].strip()  # side-effect (parts[0] not used later)
-            # arguments after first are not evaluated
-            ret = callParserFunction(funct, parts, self.frame)
-            return self.expandTemplates(ret)
-
-        title = fullyQualifiedTemplateTitle(title)
-        if not title:
-            self.template_title_errs += 1
-            return ''
-
-        redirected = redirects.get(title)
-        if redirected:
-            title = redirected
-
-        # get the template
-        if title in templateCache:
-            template = templateCache[title]
-        elif title in templates:
-            template = Template.parse(templates[title])
-            # add it to cache
-            templateCache[title] = template
-            del templates[title]
-        else:
-            # The page being included could not be identified
-            return ''
-
-        # logging.debug('TEMPLATE %s: %s', title, template)
-
-        # tplarg          = "{{{" parts "}}}"
-        # parts           = [ title *( "|" part ) ]
-        # part            = ( part-name "=" part-value ) / ( part-value )
-        # part-name       = wikitext-L3
-        # part-value      = wikitext-L3
-        # wikitext-L3     = literal / template / tplarg / link / comment /
-        #                   line-eating-comment / unclosed-comment /
-        #           	    xmlish-element / *wikitext-L3
-
-        # A tplarg may contain other parameters as well as templates, e.g.:
-        #   {{{text|{{{quote|{{{1|{{error|Error: No text given}}}}}}}}}}}
-        # hence no simple RE like this would work:
-        #   '{{{((?:(?!{{{).)*?)}}}'
-        # We must use full CF parsing.
-
-        # the parameter name itself might be computed, e.g.:
-        #   {{{appointe{{#if:{{{appointer14|}}}|r|d}}14|}}}
-
-        # Because of the multiple uses of double-brace and triple-brace
-        # syntax, expressions can sometimes be ambiguous.
-        # Precedence rules specifed here:
-        # http://www.mediawiki.org/wiki/Preprocessor_ABNF#Ideal_precedence
-        # resolve ambiguities like this:
-        #   {{{{ }}}} -> { {{{ }}} }
-        #   {{{{{ }}}}} -> {{ {{{ }}} }}
-        #
-        # :see: https://en.wikipedia.org/wiki/Help:Template#Handling_parameters
-
-        params = parts[1:]
-
-        if not subst:
-            # Evaluate parameters, since they may contain templates, including
-            # the symbol "=".
-            # {{#ifexpr: {{{1}}} = 1 }}
-            params = [self.expandTemplates(p) for p in params]
-
-        # build a dict of name-values for the parameter values
-        params = self.templateParams(params)
-
-        # Perform parameter substitution
-        # extend frame before subst, since there may be recursion in default
-        # parameter value, e.g. {{OTRS|celebrative|date=April 2015}} in article
-        # 21637542 in enwiki.
-        self.frame.append((title, params))
-        instantiated = template.subst(params, self)
-        # logging.debug('instantiated %d %s', len(self.frame), instantiated)
-        value = self.expandTemplates(instantiated)
-        self.frame.pop()
-        # logging.debug('   INVOCATION> %s %d %s', title, len(self.frame), value)
-        return value
-
-
-# ----------------------------------------------------------------------
-# parameter handling
-
-
-def splitParts(paramsList):
-    """
-    :param paramsList: the parts of a template or tplarg.
-
-    Split template parameters at the separator "|".
-    separator "=".
-
-    Template parameters often contain URLs, internal links, text or even
-    template expressions, since we evaluate templates outside in.
-    This is required for cases like:
-      {{#if: {{{1}}} | {{lc:{{{1}}} | "parameter missing"}}
-    Parameters are separated by "|" symbols. However, we
-    cannot simply split the string on "|" symbols, since these
-    also appear inside templates and internal links, e.g.
-
-     {{if:|
-      |{{#if:the president|
-           |{{#if:|
-               [[Category:Hatnote templates|A{{PAGENAME}}]]
-            }}
-       }}
-     }}
-
-    We split parts at the "|" symbols that are not inside any pair
-    {{{...}}}, {{...}}, [[...]], {|...|}.
-    """
-
-    # Must consider '[' as normal in expansion of Template:EMedicine2:
-    # #ifeq: ped|article|[http://emedicine.medscape.com/article/180-overview|[http://www.emedicine.com/ped/topic180.htm#{{#if: |section~}}
-    # as part of:
-    # {{#ifeq: ped|article|[http://emedicine.medscape.com/article/180-overview|[http://www.emedicine.com/ped/topic180.htm#{{#if: |section~}}}} ped/180{{#if: |~}}]
-
-    # should handle both tpl arg like:
-    #    4|{{{{{subst|}}}CURRENTYEAR}}
-    # and tpl parameters like:
-    #    ||[[Category:People|{{#if:A|A|{{PAGENAME}}}}]]
-
-    sep = '|'
-    parameters = []
-    cur = 0
-    for s, e in findMatchingBraces(paramsList):
-        par = paramsList[cur:s].split(sep)
-        if par:
-            if parameters:
-                # portion before | belongs to previous parameter
-                parameters[-1] += par[0]
-                if len(par) > 1:
-                    # rest are new parameters
-                    parameters.extend(par[1:])
-            else:
-                parameters = par
-        elif not parameters:
-            parameters = ['']  # create first param
-        # add span to last previous parameter
-        parameters[-1] += paramsList[s:e]
-        cur = e
-    # leftover
-    par = paramsList[cur:].split(sep)
-    if par:
-        if parameters:
-            # portion before | belongs to previous parameter
-            parameters[-1] += par[0]
-            if len(par) > 1:
-                # rest are new parameters
-                parameters.extend(par[1:])
-        else:
-            parameters = par
-
-    # logging.debug('splitParts %s %s\nparams: %s', sep, paramsList, str(parameters))
-    return parameters
-
-
-def findMatchingBraces(text, ldelim=0):
-    """
-    :param ldelim: number of braces to match. 0 means match [[]], {{}} and {{{}}}.
-    """
-    # Parsing is done with respect to pairs of double braces {{..}} delimiting
-    # a template, and pairs of triple braces {{{..}}} delimiting a tplarg.
-    # If double opening braces are followed by triple closing braces or
-    # conversely, this is taken as delimiting a template, with one left-over
-    # brace outside it, taken as plain text. For any pattern of braces this
-    # defines a set of templates and tplargs such that any two are either
-    # separate or nested (not overlapping).
-
-    # Unmatched double rectangular closing brackets can be in a template or
-    # tplarg, but unmatched double rectangular opening brackets cannot.
-    # Unmatched double or triple closing braces inside a pair of
-    # double rectangular brackets are treated as plain text.
-    # Other formulation: in ambiguity between template or tplarg on one hand,
-    # and a link on the other hand, the structure with the rightmost opening
-    # takes precedence, even if this is the opening of a link without any
-    # closing, so not producing an actual link.
-
-    # In the case of more than three opening braces the last three are assumed
-    # to belong to a tplarg, unless there is no matching triple of closing
-    # braces, in which case the last two opening braces are are assumed to
-    # belong to a template.
-
-    # We must skip individual { like in:
-    #   {{#ifeq: {{padleft:|1|}} | { | | &nbsp;}}
-    # We must resolve ambiguities like this:
-    #   {{{{ }}}} -> { {{{ }}} }
-    #   {{{{{ }}}}} -> {{ {{{ }}} }}
-    #   {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|...}}
-
-    # Handle:
-    #   {{{{{|safesubst:}}}#Invoke:String|replace|{{{1|{{{{{|safesubst:}}}PAGENAME}}}}}|%s+%([^%(]-%)$||plain=false}}
-    # as well as expressions with stray }:
-    #   {{{link|{{ucfirst:{{{1}}}}}} interchange}}}
-
-    if ldelim:  # 2-3
-        reOpen = re.compile('[{]{%d,}' % ldelim)  # at least ldelim
-        reNext = re.compile('[{]{2,}|}{2,}')  # at least 2 open or close bracces
-    else:
-        reOpen = re.compile('{{2,}|\[{2,}')
-        reNext = re.compile('{{2,}|}{2,}|\[{2,}|]{2,}')  # at least 2
-
-    cur = 0
-    while True:
-        m1 = reOpen.search(text, cur)
-        if not m1:
-            return
-        lmatch = m1.end() - m1.start()
-        if m1.group()[0] == '{':
-            stack = [lmatch]  # stack of opening braces lengths
-        else:
-            stack = [-lmatch]  # negative means [
-        end = m1.end()
-        while True:
-            m2 = reNext.search(text, end)
-            if not m2:
-                return  # unbalanced
-            end = m2.end()
-            brac = m2.group()[0]
-            lmatch = m2.end() - m2.start()
-
-            if brac == '{':
-                stack.append(lmatch)
-            elif brac == '}':
-                while stack:
-                    openCount = stack.pop()  # opening span
-                    if openCount == 0:  # illegal unmatched [[
-                        continue
-                    if lmatch >= openCount:
-                        lmatch -= openCount
-                        if lmatch <= 1:  # either close or stray }
-                            break
-                    else:
-                        # put back unmatched
-                        stack.append(openCount - lmatch)
-                        break
-                if not stack:
-                    yield m1.start(), end - lmatch
-                    cur = end
-                    break
-                elif len(stack) == 1 and 0 < stack[0] < ldelim:
-                    # ambiguous {{{{{ }}} }}
-                    yield m1.start() + stack[0], end
-                    cur = end
-                    break
-            elif brac == '[':  # [[
-                stack.append(-lmatch)
-            else:  # ]]
-                while stack and stack[-1] < 0:  # matching [[
-                    openCount = -stack.pop()
-                    if lmatch >= openCount:
-                        lmatch -= openCount
-                        if lmatch <= 1:  # either close or stray ]
-                            break
-                    else:
-                        # put back unmatched (negative)
-                        stack.append(lmatch - openCount)
-                        break
-                if not stack:
-                    yield m1.start(), end - lmatch
-                    cur = end
-                    break
-                # unmatched ]] are discarded
-                cur = end
-
-
-def findBalanced(text, openDelim, closeDelim):
-    """
-    Assuming that text contains a properly balanced expression using
-    :param openDelim: as opening delimiters and
-    :param closeDelim: as closing delimiters.
-    :return: an iterator producing pairs (start, end) of start and end
-    positions in text containing a balanced expression.
-    """
-    openPat = '|'.join([re.escape(x) for x in openDelim])
-    # patter for delimiters expected after each opening delimiter
-    afterPat = {o: re.compile(openPat + '|' + c, re.DOTALL) for o, c in zip(openDelim, closeDelim)}
-    stack = []
-    start = 0
-    cur = 0
-    # end = len(text)
-    startSet = False
-    startPat = re.compile(openPat)
-    nextPat = startPat
-    while True:
-        next = nextPat.search(text, cur)
-        if not next:
-            return
-        if not startSet:
-            start = next.start()
-            startSet = True
-        delim = next.group(0)
-        if delim in openDelim:
-            stack.append(delim)
-            nextPat = afterPat[delim]
-        else:
-            opening = stack.pop()
-            # assert opening == openDelim[closeDelim.index(next.group(0))]
-            if stack:
-                nextPat = afterPat[stack[-1]]
-            else:
-                yield start, next.end()
-                nextPat = startPat
-                start = next.end()
-                startSet = False
-        cur = next.end()
-
-# ----------------------------------------------------------------------
-# parser functions utilities
-
-
-def ucfirst(string):
-    """:return: a string with just its first character uppercase
-    We can't use title() since it coverts all words.
-    """
-    if string:
-        if len(string) > 1:
-            return string[0].upper() + string[1:]
-        else:
-            return string.upper()
-    else:
-        return ''
-
-
-def lcfirst(string):
-    """:return: a string with its first character lowercase"""
-    if string:
-        if len(string) > 1:
-            return string[0].lower() + string[1:]
-        else:
-            return string.lower()
-    else:
-        return ''
-
-
-def fullyQualifiedTemplateTitle(templateTitle):
-    """
-    Determine the namespace of the page being included through the template
-    mechanism
-    """
-    if templateTitle.startswith(':'):
-        # Leading colon by itself implies main namespace, so strip this colon
-        return ucfirst(templateTitle[1:])
-    else:
-        m = re.match('([^:]*)(:.*)', templateTitle)
-        if m:
-            # colon found but not in the first position - check if it
-            # designates a known namespace
-            prefix = normalizeNamespace(m.group(1))
-            if prefix in knownNamespaces:
-                return prefix + ucfirst(m.group(2))
-    # The title of the page being included is NOT in the main namespace and
-    # lacks any other explicit designation of the namespace - therefore, it
-    # is resolved to the Template namespace (that's the default for the
-    # template inclusion mechanism).
-
-    # This is a defense against pages whose title only contains UTF-8 chars
-    # that are reduced to an empty string. Right now I can think of one such
-    # case - <C2><A0> which represents the non-breaking space.
-    # In this particular case, this page is a redirect to [[Non-nreaking
-    # space]], but having in the system a redirect page with an empty title
-    # causes numerous problems, so we'll live happier without it.
-    if templateTitle:
-        return Extractor.templatePrefix + ucfirst(templateTitle)
-    else:
-        return ''  # caller may log as error
-
-
-def normalizeNamespace(ns):
-    return ucfirst(ns)
-
-
-# ----------------------------------------------------------------------
-# Parser functions
-# see http://www.mediawiki.org/wiki/Help:Extension:ParserFunctions
-# https://github.com/Wikia/app/blob/dev/extensions/ParserFunctions/ParserFunctions_body.php
-
-
-class Infix():
-
-    """Infix operators.
-    The calling sequence for the infix is:
-      x |op| y
-    """
-
-    def __init__(self, function):
-        self.function = function
-
-    def __ror__(self, other):
-        return Infix(lambda x, self=self, other=other: self.function(other, x))
-
-    def __or__(self, other):
-        return self.function(other)
-
-    def __rlshift__(self, other):
-        return Infix(lambda x, self=self, other=other: self.function(other, x))
-
-    def __rshift__(self, other):
-        return self.function(other)
-
-    def __call__(self, value1, value2):
-        return self.function(value1, value2)
-
-
-ROUND = Infix(lambda x, y: round(x, y))
-
-
-def sharp_expr(expr):
-    try:
-        expr = re.sub('=', '==', expr)
-        expr = re.sub('mod', '%', expr)
-        expr = re.sub('\bdiv\b', '/', expr)
-        expr = re.sub('\bround\b', '|ROUND|', expr)
-        return str(eval(expr))
-    except:
-        return '<span class="error"></span>'
-
-
-def sharp_if(testValue, valueIfTrue, valueIfFalse=None, *args):
-    # In theory, we should evaluate the first argument here,
-    # but it was evaluated while evaluating part[0] in expandTemplate().
-    if testValue.strip():
-        # The {{#if:}} function is an if-then-else construct.
-        # The applied condition is: "The condition string is non-empty".
-        valueIfTrue = valueIfTrue.strip()
-        if valueIfTrue:
-            return valueIfTrue
-    elif valueIfFalse:
-        return valueIfFalse.strip()
-    return ""
-
-
-def sharp_ifeq(lvalue, rvalue, valueIfTrue, valueIfFalse=None, *args):
-    rvalue = rvalue.strip()
-    if rvalue:
-        # lvalue is always defined
-        if lvalue.strip() == rvalue:
-            # The {{#ifeq:}} function is an if-then-else construct. The
-            # applied condition is "is rvalue equal to lvalue". Note that this
-            # does only string comparison while MediaWiki implementation also
-            # supports numerical comparissons.
-
-            if valueIfTrue:
-                return valueIfTrue.strip()
-        else:
-            if valueIfFalse:
-                return valueIfFalse.strip()
-    return ""
-
-
-def sharp_iferror(test, then='', Else=None, *args):
-    if re.match('<(?:strong|span|p|div)\s(?:[^\s>]*\s+)*?class="(?:[^"\s>]*\s+)*?error(?:\s[^">]*)?"', test):
-        return then
-    elif Else is None:
-        return test.strip()
-    else:
-        return Else.strip()
-
-
-def sharp_switch(primary, *params):
-    # FIXME: we don't support numeric expressions in primary
-
-    # {{#switch: comparison string
-    #  | case1 = result1
-    #  | case2
-    #  | case4 = result2
-    #  | 1 | case5 = result3
-    #  | #default = result4
-    # }}
-
-    primary = primary.strip()
-    found = False  # for fall through cases
-    default = None
-    rvalue = None
-    lvalue = ''
-    for param in params:
-        # handle cases like:
-        #  #default = [http://www.perseus.tufts.edu/hopper/text?doc=Perseus...]
-        pair = param.split('=', 1)
-        lvalue = pair[0].strip()
-        rvalue = None
-        if len(pair) > 1:
-            # got "="
-            rvalue = pair[1].strip()
-            # check for any of multiple values pipe separated
-            if found or primary in [v.strip() for v in lvalue.split('|')]:
-                # Found a match, return now
-                return rvalue
-            elif lvalue == '#default':
-                default = rvalue
-            rvalue = None  # avoid defaulting to last case
-        elif lvalue == primary:
-            # If the value matches, set a flag and continue
-            found = True
-    # Default case
-    # Check if the last item had no = sign, thus specifying the default case
-    if rvalue is not None:
-        return lvalue
-    elif default is not None:
-        return default
-    return ''
-
-
-# Extension Scribuntu
-def sharp_invoke(module, function, frame):
-    functions = modules.get(module)
-    if functions:
-        funct = functions.get(function)
-        if funct:
-            # find parameters in frame whose title is the one of the original
-            # template invocation
-            templateTitle = fullyQualifiedTemplateTitle(function)
-            if not templateTitle:
-                logging.warn("Template with empty title")
-            pair = next((x for x in frame if x[0] == templateTitle), None)
-            if pair:
-                params = pair[1]
-                # extract positional args
-                params = [params.get(str(i + 1)) for i in range(len(params))]
-                return funct(*params)
-            else:
-                return funct()
-    return ''
-
-
-parserFunctions = {
-
-    '#expr': sharp_expr,
-
-    '#if': sharp_if,
-
-    '#ifeq': sharp_ifeq,
-
-    '#iferror': sharp_iferror,
-
-    '#ifexpr': lambda *args: '',  # not supported
-
-    '#ifexist': lambda *args: '',  # not supported
-
-    '#rel2abs': lambda *args: '',  # not supported
-
-    '#switch': sharp_switch,
-
-    '# language': lambda *args: '',  # not supported
-
-    '#time': lambda *args: '',  # not supported
-
-    '#timel': lambda *args: '',  # not supported
-
-    '#titleparts': lambda *args: '',  # not supported
-
-    # This function is used in some pages to construct links
-    # http://meta.wikimedia.org/wiki/Help:URL
-    'urlencode': lambda string, *rest: urlencode(string),
-
-    'lc': lambda string, *rest: string.lower() if string else '',
-
-    'lcfirst': lambda string, *rest: lcfirst(string),
-
-    'uc': lambda string, *rest: string.upper() if string else '',
-
-    'ucfirst': lambda string, *rest: ucfirst(string),
-
-    'int': lambda string, *rest: str(int(string)),
-
-    'padleft': lambda char, width, string: string.ljust(char, int(pad)), # CHECK_ME
-
-}
-
-
-def callParserFunction(functionName, args, frame):
-    """
-    Parser functions have similar syntax as templates, except that
-    the first argument is everything after the first colon.
-    :param functionName: nameof the parser function
-    :param args: the arguments to the function
-    :return: the result of the invocation, None in case of failure.
-
-    http://meta.wikimedia.org/wiki/Help:ParserFunctions
-    """
-
-    try:
-        if functionName == '#invoke':
-            # special handling of frame
-            ret = sharp_invoke(args[0].strip(), args[1].strip(), frame)
-            # logging.debug('parserFunction> %s %s', args[1], ret)
-            return ret
-        if functionName in parserFunctions:
-            ret = parserFunctions[functionName](*args)
-            # logging.debug('parserFunction> %s(%s) %s', functionName, args, ret)
-            return ret
-    except:
-        return ""  # FIXME: fix errors
-
-    return ""
-
-
-# ----------------------------------------------------------------------
-# Extract Template definition
-
-reNoinclude = re.compile(r'<noinclude>(?:.*?)</noinclude>', re.DOTALL)
-reIncludeonly = re.compile(r'<includeonly>|</includeonly>', re.DOTALL)
-
-# These are built before spawning processes, hence they are shared.
-templates = {}
-redirects = {}
-# cache of parser templates
-# FIXME: sharing this with a Manager slows down.
-templateCache = {}
-
-
-def define_template(title, page):
-    """
-    Adds a template defined in the :param page:.
-    @see https://en.wikipedia.org/wiki/Help:Template#Noinclude.2C_includeonly.2C_and_onlyinclude
-    """
-    global templates
-    global redirects
-
-    # title = normalizeTitle(title)
-
-    # check for redirects
-    m = re.match('#REDIRECT.*?\[\[([^\]]*)]]', page[0], re.IGNORECASE)
-    if m:
-        redirects[title] = m.group(1)  # normalizeTitle(m.group(1))
-        return
-
-    text = unescape(''.join(page))
-
-    # We're storing template text for future inclusion, therefore,
-    # remove all <noinclude> text and keep all <includeonly> text
-    # (but eliminate <includeonly> tags per se).
-    # However, if <onlyinclude> ... </onlyinclude> parts are present,
-    # then only keep them and discard the rest of the template body.
-    # This is because using <onlyinclude> on a text fragment is
-    # equivalent to enclosing it in <includeonly> tags **AND**
-    # enclosing all the rest of the template body in <noinclude> tags.
-
-    # remove comments
-    text = comment.sub('', text)
-
-    # eliminate <noinclude> fragments
-    text = reNoinclude.sub('', text)
-    # eliminate unterminated <noinclude> elements
-    text = re.sub(r'<noinclude\s*>.*$', '', text, flags=re.DOTALL)
-    text = re.sub(r'<noinclude/>', '', text)
-
-    onlyincludeAccumulator = ''
-    for m in re.finditer('<onlyinclude>(.*?)</onlyinclude>', text, re.DOTALL):
-        onlyincludeAccumulator += m.group(1)
-    if onlyincludeAccumulator:
-        text = onlyincludeAccumulator
-    else:
-        text = reIncludeonly.sub('', text)
-
-    if text:
-        if title in templates and templates[title] != text:
-            logging.warn('Redefining: %s', title)
-        templates[title] = text
+# -*- coding: utf-8 -*-
+
+# =============================================================================
+#  Copyright (c) 2020. Giuseppe Attardi (attardi@di.unipi.it).
+# =============================================================================
+#  This file is part of Tanl.
+#
+#  Tanl is free software; you can redistribute it and/or modify it
+#  under the terms of the GNU Affero General Public License, version 3,
+#  as published by the Free Software Foundation.
+#
+#  Tanl is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Affero General Public License for more details.
+#
+#  You should have received a copy of the GNU Affero General Public License
+#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# =============================================================================
+
+import re
+import html
+import json
+from itertools import zip_longest
+from urllib.parse import quote as urlencode
+from html.entities import name2codepoint
+import logging
+import time
+
+# ----------------------------------------------------------------------
+
+# match tail after wikilink
+tailRE = re.compile('\w+')
+syntaxhighlight = re.compile('&lt;syntaxhighlight .*?&gt;(.*?)&lt;/syntaxhighlight&gt;', re.DOTALL)
+
+## PARAMS ####################################################################
+
+##
+# Defined in <siteinfo>
+# We include as default Template, when loading external template file.
+knownNamespaces = set(['Template'])
+
+##
+# Drop these elements from article text
+#
+discardElements = [
+    'gallery', 'timeline', 'noinclude', 'pre',
+    'table', 'tr', 'td', 'th', 'caption', 'div',
+    'form', 'input', 'select', 'option', 'textarea',
+    'ul', 'li', 'ol', 'dl', 'dt', 'dd', 'menu', 'dir',
+    'ref', 'references', 'img', 'imagemap', 'source', 'small'
+]
+
+##
+# Recognize only these namespaces
+# w: Internal links to the Wikipedia
+# wiktionary: Wiki dictionary
+# wikt: shortcut for Wiktionary
+#
+acceptedNamespaces = ['w', 'wiktionary', 'wikt']
+
+
+def get_url(urlbase, uid):
+    return "%s?curid=%s" % (urlbase, uid)
+
+
+# ======================================================================
+
+
+def clean(extractor, text, expand_templates=False, html_safe=True):
+    """
+    Transforms wiki markup. If the command line flag --escapedoc is set then the text is also escaped
+    @see https://www.mediawiki.org/wiki/Help:Formatting
+    :param extractor: the Extractor t use.
+    :param text: the text to clean.
+    :param expand_templates: whether to perform template expansion.
+    :param html_safe: whether to convert reserved HTML characters to entities.
+    @return: the cleaned text.
+    """
+
+    if expand_templates:
+        # expand templates
+        # See: http://www.mediawiki.org/wiki/Help:Templates
+        text = extractor.expandTemplates(text)
+    else:
+        # Drop transclusions (template, parser functions)
+        text = dropNested(text, r'{{', r'}}')
+
+    # Drop tables
+    text = dropNested(text, r'{\|', r'\|}')
+
+    # replace external links
+    text = replaceExternalLinks(text)
+
+    # replace internal links
+    text = replaceInternalLinks(text)
+
+    # drop MagicWords behavioral switches
+    text = magicWordsRE.sub('', text)
+
+    # ############### Process HTML ###############
+
+    # turn into HTML, except for the content of <syntaxhighlight>
+    res = ''
+    cur = 0
+    for m in syntaxhighlight.finditer(text):
+        end = m.end()
+        res += unescape(text[cur:m.start()]) + m.group(1)
+        cur = end
+    text = res + unescape(text[cur:])
+
+    # Handle bold/italic/quote
+    if extractor.HtmlFormatting:
+        text = bold_italic.sub(r'<b>\1</b>', text)
+        text = bold.sub(r'<b>\1</b>', text)
+        text = italic.sub(r'<i>\1</i>', text)
+    else:
+        text = bold_italic.sub(r'\1', text)
+        text = bold.sub(r'\1', text)
+        text = italic_quote.sub(r'"\1"', text)
+        text = italic.sub(r'"\1"', text)
+        text = quote_quote.sub(r'"\1"', text)
+    # residuals of unbalanced quotes
+    text = text.replace("'''", '').replace("''", '"')
+
+    # Collect spans
+
+    spans = []
+    # Drop HTML comments
+    for m in comment.finditer(text):
+        spans.append((m.start(), m.end()))
+
+    # Drop self-closing tags
+    for pattern in selfClosing_tag_patterns:
+        for m in pattern.finditer(text):
+            spans.append((m.start(), m.end()))
+
+    # Drop ignored tags
+    for left, right in ignored_tag_patterns:
+        for m in left.finditer(text):
+            spans.append((m.start(), m.end()))
+        for m in right.finditer(text):
+            spans.append((m.start(), m.end()))
+
+    # Bulk remove all spans
+    text = dropSpans(spans, text)
+
+    # Drop discarded elements
+    for tag in discardElements:
+        text = dropNested(text, r'<\s*%s\b[^>/]*>' % tag, r'<\s*/\s*%s>' % tag)
+
+    if not extractor.HtmlFormatting:
+        # Turn into text what is left (&amp;nbsp;) and <syntaxhighlight>
+        text = unescape(text)
+
+    # Expand placeholders
+    for pattern, placeholder in placeholder_tag_patterns:
+        index = 1
+        for match in pattern.finditer(text):
+            text = text.replace(match.group(), '%s_%d' % (placeholder, index))
+            index += 1
+
+    text = text.replace('<<', u'«').replace('>>', u'»')
+
+    #############################################
+
+    # Cleanup text
+    text = text.replace('\t', ' ')
+    text = spaces.sub(' ', text)
+    text = dots.sub('...', text)
+    text = re.sub(u' (,:\.\)\]»)', r'\1', text)
+    text = re.sub(u'(\[\(«) ', r'\1', text)
+    text = re.sub(r'\n\W+?\n', '\n', text, flags=re.U)  # lines with only punctuations
+    text = text.replace(',,', ',').replace(',.', '.')
+    if html_safe:
+        text = html.escape(text, quote=False)
+    return text
+
+
+# skip level 1, it is page name level
+section = re.compile(r'(==+)\s*(.*?)\s*\1')
+
+listOpen = {'*': '<ul>', '#': '<ol>', ';': '<dl>', ':': '<dl>'}
+listClose = {'*': '</ul>', '#': '</ol>', ';': '</dl>', ':': '</dl>'}
+listItem = {'*': '<li>%s</li>', '#': '<li>%s</<li>', ';': '<dt>%s</dt>',
+            ':': '<dd>%s</dd>'}
+
+
+def compact(text, mark_headers=False):
+    """Deal with headers, lists, empty sections, residuals of tables.
+    :param text: convert to HTML
+    """
+
+    page = []  # list of paragraph
+    headers = {}  # Headers for unfilled sections
+    emptySection = False  # empty sections are discarded
+    listLevel = ''  # nesting of lists
+
+    for line in text.split('\n'):
+
+        if not line:
+            if len(listLevel):    # implies Extractor.HtmlFormatting
+                for c in reversed(listLevel):
+                    page.append(listClose[c])
+                    listLevel = ''
+            continue
+
+        # Handle section titles
+        m = section.match(line)
+        if m:
+            title = m.group(2)
+            lev = len(m.group(1))
+            if Extractor.HtmlFormatting:
+                page.append("<h%d>%s</h%d>" % (lev, title, lev))
+            if title and title[-1] not in '!?':
+                title += '.'
+
+            if mark_headers:
+                title = "## " + title
+
+            headers[lev] = title
+            # drop previous headers
+            headers = { k:v for k,v in headers.items() if k <= lev }
+            emptySection = True
+            continue
+        # Handle page title
+        if line.startswith('++'):
+            title = line[2:-2]
+            if title:
+                if title[-1] not in '!?':
+                    title += '.'
+                page.append(title)
+        # handle indents
+        elif line[0] == ':':
+            page.append(line.lstrip(':'))
+        # handle lists
+        # @see https://www.mediawiki.org/wiki/Help:Formatting
+        elif line[0] in '*#;':
+            if Extractor.HtmlFormatting:
+                # close extra levels
+                l = 0
+                for c in listLevel:
+                    if l < len(line) and c != line[l]:
+                        for extra in reversed(listLevel[l:]):
+                            page.append(listClose[extra])
+                        listLevel = listLevel[:l]
+                        break
+                    l += 1
+                if l < len(line) and line[l] in '*#;:':
+                    # add new level (only one, no jumps)
+                    # FIXME: handle jumping levels
+                    type = line[l]
+                    page.append(listOpen[type])
+                    listLevel += type
+                    line = line[l+1:].strip()
+                else:
+                    # continue on same level
+                    type = line[l-1]
+                    line = line[l:].strip()
+                page.append(listItem[type] % line)
+            else:
+                continue
+        elif len(listLevel):    # implies Extractor.HtmlFormatting
+            for c in reversed(listLevel):
+                page.append(listClose[c])
+            listLevel = []
+
+        # Drop residuals of lists
+        elif line[0] in '{|' or line[-1] == '}':
+            continue
+        # Drop irrelevant lines
+        elif (line[0] == '(' and line[-1] == ')') or line.strip('.-') == '':
+            continue
+        elif len(headers):
+            if Extractor.keepSections:
+                items = sorted(headers.items())
+                for (i, v) in items:
+                    page.append(v)
+            headers.clear()
+            page.append(line)  # first line
+            emptySection = False
+        elif not emptySection:
+            page.append(line)
+            # dangerous
+            # # Drop preformatted
+            # elif line[0] == ' ':
+            #     continue
+
+    return page
+
+
+# ----------------------------------------------------------------------
+
+def dropNested(text, openDelim, closeDelim):
+    """
+    A matching function for nested expressions, e.g. namespaces and tables.
+    """
+    openRE = re.compile(openDelim, re.IGNORECASE)
+    closeRE = re.compile(closeDelim, re.IGNORECASE)
+    # partition text in separate blocks { } { }
+    spans = []  # pairs (s, e) for each partition
+    nest = 0  # nesting level
+    start = openRE.search(text, 0)
+    if not start:
+        return text
+    end = closeRE.search(text, start.end())
+    next = start
+    while end:
+        next = openRE.search(text, next.end())
+        if not next:  # termination
+            while nest:  # close all pending
+                nest -= 1
+                end0 = closeRE.search(text, end.end())
+                if end0:
+                    end = end0
+                else:
+                    break
+            spans.append((start.start(), end.end()))
+            break
+        while end.end() < next.start():
+            # { } {
+            if nest:
+                nest -= 1
+                # try closing more
+                last = end.end()
+                end = closeRE.search(text, end.end())
+                if not end:  # unbalanced
+                    if spans:
+                        span = (spans[0][0], last)
+                    else:
+                        span = (start.start(), last)
+                    spans = [span]
+                    break
+            else:
+                spans.append((start.start(), end.end()))
+                # advance start, find next close
+                start = next
+                end = closeRE.search(text, next.end())
+                break  # { }
+        if next != start:
+            # { { }
+            nest += 1
+    # collect text outside partitions
+    return dropSpans(spans, text)
+
+
+def dropSpans(spans, text):
+    """
+    Drop from text the blocks identified in :param spans:, possibly nested.
+    """
+    spans.sort()
+    res = ''
+    offset = 0
+    for s, e in spans:
+        if offset <= s:  # handle nesting
+            if offset < s:
+                res += text[offset:s]
+            offset = e
+    res += text[offset:]
+    return res
+
+
+# ----------------------------------------------------------------------
+# External links
+
+# from: https://doc.wikimedia.org/mediawiki-core/master/php/DefaultSettings_8php_source.html
+
+wgUrlProtocols = [
+    'bitcoin:', 'ftp://', 'ftps://', 'geo:', 'git://', 'gopher://', 'http://',
+    'https://', 'irc://', 'ircs://', 'magnet:', 'mailto:', 'mms://', 'news:',
+    'nntp://', 'redis://', 'sftp://', 'sip:', 'sips:', 'sms:', 'ssh://',
+    'svn://', 'tel:', 'telnet://', 'urn:', 'worldwind://', 'xmpp:', '//'
+]
+
+# from: https://doc.wikimedia.org/mediawiki-core/master/php/Parser_8php_source.html
+
+# Constants needed for external link processing
+# Everything except bracket, space, or control characters
+# \p{Zs} is unicode 'separator, space' category. It covers the space 0x20
+# as well as U+3000 is IDEOGRAPHIC SPACE for bug 19052
+EXT_LINK_URL_CLASS = r'[^][<>"\x00-\x20\x7F\s]'
+ExtLinkBracketedRegex = re.compile(
+    '(?i)\[((' + '|'.join(wgUrlProtocols) + ')' + EXT_LINK_URL_CLASS + r'+)\s*([^\]\x00-\x08\x0a-\x1F]*?)\]',
+    re.S | re.U)
+EXT_IMAGE_REGEX = re.compile(
+    r"""(?i)^(http://|https://)([^][<>"\x00-\x20\x7F\s]+)
+    /([A-Za-z0-9_.,~%\-+&;#*?!=()@\x80-\xFF]+)\.(gif|png|jpg|jpeg)$""",
+    re.X | re.S | re.U)
+
+
+def replaceExternalLinks(text):
+    s = ''
+    cur = 0
+    for m in ExtLinkBracketedRegex.finditer(text):
+        s += text[cur:m.start()]
+        cur = m.end()
+
+        url = m.group(1)
+        label = m.group(3)
+
+        # # The characters '<' and '>' (which were escaped by
+        # # removeHTMLtags()) should not be included in
+        # # URLs, per RFC 2396.
+        # m2 = re.search('&(lt|gt);', url)
+        # if m2:
+        #     link = url[m2.end():] + ' ' + link
+        #     url = url[0:m2.end()]
+
+        # If the link text is an image URL, replace it with an <img> tag
+        # This happened by accident in the original parser, but some people used it extensively
+        m = EXT_IMAGE_REGEX.match(label)
+        if m:
+            label = makeExternalImage(label)
+
+        # Use the encoded URL
+        # This means that users can paste URLs directly into the text
+        # Funny characters like ö aren't valid in URLs anyway
+        # This was changed in August 2004
+        s += makeExternalLink(url, label)  # + trail
+
+    return s + text[cur:]
+
+
+def makeExternalLink(url, anchor):
+    """Function applied to wikiLinks"""
+    if Extractor.keepLinks:
+        return '<a href="%s">%s</a>' % (urlencode(url), anchor)
+    else:
+        return anchor
+
+
+def makeExternalImage(url, alt=''):
+    if Extractor.keepLinks:
+        return '<img src="%s" alt="%s">' % (url, alt)
+    else:
+        return alt
+
+
+# ----------------------------------------------------------------------
+# WikiLinks
+# See https://www.mediawiki.org/wiki/Help:Links#Internal_links
+
+# Can be nested [[File:..|..[[..]]..|..]], [[Category:...]], etc.
+# Also: [[Help:IPA for Catalan|[andora]]]
+
+
+def replaceInternalLinks(text):
+    """
+    Replaces external links of the form:
+    [[title |...|label]]trail
+
+    with title concatenated with trail, when present, e.g. 's' for plural.
+    """
+    # call this after removal of external links, so we need not worry about
+    # triple closing ]]].
+    cur = 0
+    res = ''
+    for s, e in findBalanced(text, ['[['], [']]']):
+        m = tailRE.match(text, e)
+        if m:
+            trail = m.group(0)
+            end = m.end()
+        else:
+            trail = ''
+            end = e
+        inner = text[s + 2:e - 2]
+        # find first |
+        pipe = inner.find('|')
+        if pipe < 0:
+            title = inner
+            label = title
+        else:
+            title = inner[:pipe].rstrip()
+            # find last |
+            curp = pipe + 1
+            for s1, e1 in findBalanced(inner, ['[['], [']]']):
+                last = inner.rfind('|', curp, s1)
+                if last >= 0:
+                    pipe = last  # advance
+                curp = e1
+            label = inner[pipe + 1:].strip()
+        res += text[cur:s] + makeInternalLink(title, label) + trail
+        cur = end
+    return res + text[cur:]
+
+
+def makeInternalLink(title, label):
+    colon = title.find(':')
+    if colon > 0 and title[:colon] not in acceptedNamespaces:
+        return ''
+    if colon == 0:
+        # drop also :File:
+        colon2 = title.find(':', colon + 1)
+        if colon2 > 1 and title[colon + 1:colon2] not in acceptedNamespaces:
+            return ''
+    if Extractor.keepLinks:
+        return '<a href="%s">%s</a>' % (urlencode(title), label)
+    else:
+        return label
+
+
+# ----------------------------------------------------------------------
+# variables
+
+
+class MagicWords():
+
+    """
+    One copy in each Extractor.
+
+    @see https://doc.wikimedia.org/mediawiki-core/master/php/MagicWord_8php_source.html
+    """
+    names = [
+        '!',
+        'currentmonth',
+        'currentmonth1',
+        'currentmonthname',
+        'currentmonthnamegen',
+        'currentmonthabbrev',
+        'currentday',
+        'currentday2',
+        'currentdayname',
+        'currentyear',
+        'currenttime',
+        'currenthour',
+        'localmonth',
+        'localmonth1',
+        'localmonthname',
+        'localmonthnamegen',
+        'localmonthabbrev',
+        'localday',
+        'localday2',
+        'localdayname',
+        'localyear',
+        'localtime',
+        'localhour',
+        'numberofarticles',
+        'numberoffiles',
+        'numberofedits',
+        'articlepath',
+        'pageid',
+        'sitename',
+        'server',
+        'servername',
+        'scriptpath',
+        'stylepath',
+        'pagename',
+        'pagenamee',
+        'fullpagename',
+        'fullpagenamee',
+        'namespace',
+        'namespacee',
+        'namespacenumber',
+        'currentweek',
+        'currentdow',
+        'localweek',
+        'localdow',
+        'revisionid',
+        'revisionday',
+        'revisionday2',
+        'revisionmonth',
+        'revisionmonth1',
+        'revisionyear',
+        'revisiontimestamp',
+        'revisionuser',
+        'revisionsize',
+        'subpagename',
+        'subpagenamee',
+        'talkspace',
+        'talkspacee',
+        'subjectspace',
+        'subjectspacee',
+        'talkpagename',
+        'talkpagenamee',
+        'subjectpagename',
+        'subjectpagenamee',
+        'numberofusers',
+        'numberofactiveusers',
+        'numberofpages',
+        'currentversion',
+        'rootpagename',
+        'rootpagenamee',
+        'basepagename',
+        'basepagenamee',
+        'currenttimestamp',
+        'localtimestamp',
+        'directionmark',
+        'contentlanguage',
+        'numberofadmins',
+        'cascadingsources',
+    ]
+
+    def __init__(self):
+        self.values = {'!': '|'}
+
+    def __getitem__(self, name):
+        return self.values.get(name)
+
+    def __setitem__(self, name, value):
+        self.values[name] = value
+
+    switches = (
+        '__NOTOC__',
+        '__FORCETOC__',
+        '__TOC__',
+        '__TOC__',
+        '__NEWSECTIONLINK__',
+        '__NONEWSECTIONLINK__',
+        '__NOGALLERY__',
+        '__HIDDENCAT__',
+        '__NOCONTENTCONVERT__',
+        '__NOCC__',
+        '__NOTITLECONVERT__',
+        '__NOTC__',
+        '__START__',
+        '__END__',
+        '__INDEX__',
+        '__NOINDEX__',
+        '__STATICREDIRECT__',
+        '__DISAMBIG__'
+    )
+
+
+magicWordsRE = re.compile('|'.join(MagicWords.switches))
+
+
+# =========================================================================
+#
+# MediaWiki Markup Grammar
+# https://www.mediawiki.org/wiki/Preprocessor_ABNF
+
+# xml-char = %x9 / %xA / %xD / %x20-D7FF / %xE000-FFFD / %x10000-10FFFF
+# sptab = SP / HTAB
+
+# ; everything except ">" (%x3E)
+# attr-char = %x9 / %xA / %xD / %x20-3D / %x3F-D7FF / %xE000-FFFD / %x10000-10FFFF
+
+# literal         = *xml-char
+# title           = wikitext-L3
+# part-name       = wikitext-L3
+# part-value      = wikitext-L3
+# part            = ( part-name "=" part-value ) / ( part-value )
+# parts           = [ title *( "|" part ) ]
+# tplarg          = "{{{" parts "}}}"
+# template        = "{{" parts "}}"
+# link            = "[[" wikitext-L3 "]]"
+
+# comment         = "<!--" literal "-->"
+# unclosed-comment = "<!--" literal END
+# ; the + in the line-eating-comment rule was absent between MW 1.12 and MW 1.22
+# line-eating-comment = LF LINE-START *SP +( comment *SP ) LINE-END
+
+# attr            = *attr-char
+# nowiki-element  = "<nowiki" attr ( "/>" / ( ">" literal ( "</nowiki>" / END ) ) )
+
+# wikitext-L2     = heading / wikitext-L3 / *wikitext-L2
+# wikitext-L3     = literal / template / tplarg / link / comment /
+#                   line-eating-comment / unclosed-comment / xmlish-element /
+#                   *wikitext-L3
+
+# ------------------------------------------------------------------------------
+
+selfClosingTags = ('br', 'hr', 'nobr', 'ref', 'references', 'nowiki')
+
+# These tags are dropped, keeping their content.
+# handle 'a' separately, depending on keepLinks
+ignoredTags = (
+    'abbr', 'b', 'big', 'blockquote', 'center', 'cite', 'div', 'em',
+    'font', 'h1', 'h2', 'h3', 'h4', 'hiero', 'i', 'kbd', 'nowiki',
+    'p', 'plaintext', 's', 'span', 'strike', 'strong',
+    'sub', 'sup', 'tt', 'u', 'var'
+)
+
+placeholder_tags = {'math': 'formula', 'code': 'codice'}
+
+
+def normalizeTitle(title):
+    """Normalize title"""
+    # remove leading/trailing whitespace and underscores
+    title = title.strip(' _')
+    # replace sequences of whitespace and underscore chars with a single space
+    title = re.sub(r'[\s_]+', ' ', title)
+
+    m = re.match(r'([^:]*):(\s*)(\S(?:.*))', title)
+    if m:
+        prefix = m.group(1)
+        if m.group(2):
+            optionalWhitespace = ' '
+        else:
+            optionalWhitespace = ''
+        rest = m.group(3)
+
+        ns = normalizeNamespace(prefix)
+        if ns in knownNamespaces:
+            # If the prefix designates a known namespace, then it might be
+            # followed by optional whitespace that should be removed to get
+            # the canonical page name
+            # (e.g., "Category:  Births" should become "Category:Births").
+            title = ns + ":" + ucfirst(rest)
+        else:
+            # No namespace, just capitalize first letter.
+            # If the part before the colon is not a known namespace, then we
+            # must not remove the space after the colon (if any), e.g.,
+            # "3001: The_Final_Odyssey" != "3001:The_Final_Odyssey".
+            # However, to get the canonical page name we must contract multiple
+            # spaces into one, because
+            # "3001:   The_Final_Odyssey" != "3001: The_Final_Odyssey".
+            title = ucfirst(prefix) + ":" + optionalWhitespace + ucfirst(rest)
+    else:
+        # no namespace, just capitalize first letter
+        title = ucfirst(title)
+    return title
+
+
+def unescape(text):
+    """
+    Removes HTML or XML character references and entities from a text string.
+
+    :param text The HTML (or XML) source text.
+    :return The plain text, as a Unicode string, if necessary.
+    """
+
+    def fixup(m):
+        text = m.group(0)
+        code = m.group(1)
+        try:
+            if text[1] == "#":  # character reference
+                if text[2] == "x":
+                    return chr(int(code[1:], 16))
+                else:
+                    return chr(int(code))
+            else:  # named entity
+                return chr(name2codepoint[code])
+        except:
+            return text  # leave as is
+
+    return re.sub("&#?(\w+);", fixup, text)
+
+
+# Match HTML comments
+# The buggy template {{Template:T}} has a comment terminating with just "->"
+comment = re.compile(r'<!--.*?-->', re.DOTALL)
+
+# Match ignored tags
+ignored_tag_patterns = []
+
+
+def ignoreTag(tag):
+    left = re.compile(r'<%s\b.*?>' % tag, re.IGNORECASE | re.DOTALL)  # both <ref> and <reference>
+    right = re.compile(r'</\s*%s>' % tag, re.IGNORECASE)
+    ignored_tag_patterns.append((left, right))
+
+
+def resetIgnoredTags():
+    global ignored_tag_patterns
+    ignored_tag_patterns = []
+
+
+for tag in ignoredTags:
+    ignoreTag(tag)
+
+# Match selfClosing HTML tags
+selfClosing_tag_patterns = [
+    re.compile(r'<\s*%s\b[^>]*/\s*>' % tag, re.DOTALL | re.IGNORECASE) for tag in selfClosingTags
+]
+
+# Match HTML placeholder tags
+placeholder_tag_patterns = [
+    (re.compile(r'<\s*%s(\s*| [^>]+?)>.*?<\s*/\s*%s\s*>' % (tag, tag), re.DOTALL | re.IGNORECASE),
+     repl) for tag, repl in placeholder_tags.items()
+]
+
+# Match preformatted lines
+preformatted = re.compile(r'^ .*?$')
+
+# Match external links (space separates second optional parameter)
+externalLink = re.compile(r'\[\w+[^ ]*? (.*?)]')
+externalLinkNoAnchor = re.compile(r'\[\w+[&\]]*\]')
+
+# Matches bold/italic
+bold_italic = re.compile(r"'''''(.*?)'''''")
+bold = re.compile(r"'''(.*?)'''")
+italic_quote = re.compile(r"''\"([^\"]*?)\"''")
+italic = re.compile(r"''(.*?)''")
+quote_quote = re.compile(r'""([^"]*?)""')
+
+# Matches space
+spaces = re.compile(r' {2,}')
+
+# Matches dots
+dots = re.compile(r'\.{4,}')
+
+# ======================================================================
+
+class Template(list):
+    """
+    A Template is a list of TemplateText or TemplateArgs
+    """
+
+    @classmethod
+    def parse(cls, body):
+        tpl = Template()
+        # we must handle nesting, s.a.
+        # {{{1|{{PAGENAME}}}
+        # {{{italics|{{{italic|}}}
+        # {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|
+        #
+        start = 0
+        for s,e in findMatchingBraces(body, 3):
+            tpl.append(TemplateText(body[start:s]))
+            tpl.append(TemplateArg(body[s+3:e-3]))
+            start = e
+        tpl.append(TemplateText(body[start:])) # leftover
+        return tpl
+
+    def subst(self, params, extractor, depth=0):
+        # We perform parameter substitutions recursively.
+        # We also limit the maximum number of iterations to avoid too long or
+        # even endless loops (in case of malformed input).
+
+        # :see: http://meta.wikimedia.org/wiki/Help:Expansion#Distinction_between_variables.2C_parser_functions.2C_and_templates
+        #
+        # Parameter values are assigned to parameters in two (?) passes.
+        # Therefore a parameter name in a template can depend on the value of
+        # another parameter of the same template, regardless of the order in
+        # which they are specified in the template call, for example, using
+        # Template:ppp containing "{{{{{{p}}}}}}", {{ppp|p=q|q=r}} and even
+        # {{ppp|q=r|p=q}} gives r, but using Template:tvvv containing
+        # "{{{{{{{{{p}}}}}}}}}", {{tvvv|p=q|q=r|r=s}} gives s.
+
+        logging.debug('subst tpl (%d, %d) %s', len(extractor.frame), depth, self)
+
+        if depth > extractor.maxParameterRecursionLevels:
+            extractor.recursion_exceeded_3_errs += 1
+            return ''
+
+        return ''.join([tpl.subst(params, extractor, depth) for tpl in self])
+
+    def __str__(self):
+        return ''.join([str(x) for x in self])
+
+
+class TemplateText(str):
+    """Fixed text of template"""
+
+    def subst(self, params, extractor, depth):
+        return self
+
+
+class TemplateArg():
+    """
+    parameter to a template.
+    Has a name and a default value, both of which are Templates.
+    """
+    def __init__(self, parameter):
+        """
+        :param parameter: the parts of a tplarg.
+        """
+        # the parameter name itself might contain templates, e.g.:
+        #   appointe{{#if:{{{appointer14|}}}|r|d}}14|
+        #   4|{{{{{subst|}}}CURRENTYEAR}}
+
+        # any parts in a tplarg after the first (the parameter default) are
+        # ignored, and an equals sign in the first part is treated as plain text.
+        #logging.debug('TemplateArg %s', parameter)
+
+        parts = splitParts(parameter)
+        self.name = Template.parse(parts[0])
+        if len(parts) > 1:
+            # This parameter has a default value
+            self.default = Template.parse(parts[1])
+        else:
+            self.default = None
+
+    def __str__(self):
+        if self.default:
+            return '{{{%s|%s}}}' % (self.name, self.default)
+        else:
+            return '{{{%s}}}' % self.name
+
+    def subst(self, params, extractor, depth):
+        """
+        Substitute value for this argument from dict :param params:
+        Use :param extractor: to evaluate expressions for name and default.
+        Limit substitution to the maximun :param depth:.
+        """
+        # the parameter name itself might contain templates, e.g.:
+        # appointe{{#if:{{{appointer14|}}}|r|d}}14|
+        paramName = self.name.subst(params, extractor, depth+1)
+        paramName = extractor.expandTemplates(paramName)
+        res = ''
+        if paramName in params:
+            res = params[paramName]  # use parameter value specified in template invocation
+        elif self.default:            # use the default value
+            defaultValue = self.default.subst(params, extractor, depth+1)
+            res =  extractor.expandTemplates(defaultValue)
+        #logging.debug('subst arg %d %s -> %s' % (depth, paramName, res))
+        return res
+
+
+# ======================================================================
+
+substWords = 'subst:|safesubst:'
+
+
+class Extractor():
+    """
+    An extraction task on a article.
+    """
+    ##
+    # Whether to preserve links in output
+    keepLinks = False
+
+    ##
+    # Whether to preserve section titles
+    keepSections = True
+
+    ##
+    # Whether to output text with HTML formatting elements in <doc> files.
+    HtmlFormatting = False
+
+    ##
+    # Whether to produce json instead of the default <doc> output format.
+    toJson = False
+
+    ##
+    # Obtained from TemplateNamespace
+    templatePrefix = ''
+
+    def __init__(self, id, revid, urlbase, title, page):
+        """
+        :param page: a list of lines.
+        """
+        self.id = id
+        self.revid = revid
+        self.url = get_url(urlbase, id)
+        self.title = title
+        self.page = page
+        self.magicWords = MagicWords()
+        self.frame = []
+        self.recursion_exceeded_1_errs = 0  # template recursion within expandTemplates()
+        self.recursion_exceeded_2_errs = 0  # template recursion within expandTemplate()
+        self.recursion_exceeded_3_errs = 0  # parameter recursion
+        self.template_title_errs = 0
+
+    def clean_text(self, text, mark_headers=False, expand_templates=True,
+                   html_safe=True):
+        """
+        :param mark_headers: True to distinguish headers from paragraphs
+          e.g. "## Section 1"
+        """
+        self.magicWords['namespace'] = self.title[:max(0, self.title.find(":"))]
+        #self.magicWords['namespacenumber'] = '0' # for article,
+        self.magicWords['pagename'] = self.title
+        self.magicWords['fullpagename'] = self.title
+        self.magicWords['currentyear'] = time.strftime('%Y')
+        self.magicWords['currentmonth'] = time.strftime('%m')
+        self.magicWords['currentday'] = time.strftime('%d')
+        self.magicWords['currenthour'] = time.strftime('%H')
+        self.magicWords['currenttime'] = time.strftime('%H:%M:%S')
+
+        text = clean(self, text, expand_templates=expand_templates,
+                     html_safe=html_safe)
+
+        text = compact(text, mark_headers=mark_headers)
+        return text
+
+    def extract(self, out, html_safe=True):
+        """
+        :param out: a memory file.
+        :param html_safe: whether to escape HTML entities.
+        """
+        logging.debug("%s\t%s", self.id, self.title)
+        text = ''.join(self.page)
+        text = self.clean_text(text, html_safe=html_safe)
+
+        if self.to_json:
+            json_data = {
+		'id': self.id,
+                'revid': self.revid,
+                'url': self.url,
+                'title': self.title,
+                'text': "\n".join(text)
+            }
+            out_str = json.dumps(json_data)
+            out.write(out_str)
+            out.write('\n')
+        else:
+            header = '<doc id="%s" url="%s" title="%s">\n' % (self.id, self.url, self.title)
+            # Separate header from text with a newline.
+            header += self.title + '\n\n'
+            footer = "\n</doc>\n"
+            out.write(header)
+            out.write('\n'.join(text))
+            out.write('\n')
+            out.write(footer)
+
+        errs = (self.template_title_errs,
+                self.recursion_exceeded_1_errs,
+                self.recursion_exceeded_2_errs,
+                self.recursion_exceeded_3_errs)
+        if any(errs):
+            logging.warn("Template errors in article '%s' (%s): title(%d) recursion(%d, %d, %d)",
+                         self.title, self.id, *errs)
+
+    # ----------------------------------------------------------------------
+    # Expand templates
+
+    maxTemplateRecursionLevels = 30
+    maxParameterRecursionLevels = 16
+
+    # check for template beginning
+    reOpen = re.compile('(?<!{){{(?!{)', re.DOTALL)
+
+    def expandTemplates(self, wikitext):
+        """
+        :param wikitext: the text to be expanded.
+
+        Templates are frequently nested. Occasionally, parsing mistakes may
+        cause template insertion to enter an infinite loop, for instance when
+        trying to instantiate Template:Country
+
+        {{country_{{{1}}}|{{{2}}}|{{{2}}}|size={{{size|}}}|name={{{name|}}}}}
+
+        which is repeatedly trying to insert template 'country_', which is
+        again resolved to Template:Country. The straightforward solution of
+        keeping track of templates that were already inserted for the current
+        article would not work, because the same template may legally be used
+        more than once, with different parameters in different parts of the
+        article.  Therefore, we limit the number of iterations of nested
+        template inclusion.
+
+        """
+        # Test template expansion at:
+        # https://en.wikipedia.org/wiki/Special:ExpandTemplates
+
+        res = ''
+        if len(self.frame) >= self.maxTemplateRecursionLevels:
+            self.recursion_exceeded_1_errs += 1
+            return res
+
+        # logging.debug('<expandTemplates ' + str(len(self.frame)))
+
+        cur = 0
+        # look for matching {{...}}
+        for s, e in findMatchingBraces(wikitext, 2):
+            res += wikitext[cur:s] + self.expandTemplate(wikitext[s + 2:e - 2])
+            cur = e
+        # leftover
+        res += wikitext[cur:]
+        # logging.debug('   expandTemplates> %d %s', len(self.frame), res)
+        return res
+
+    def templateParams(self, parameters):
+        """
+        Build a dictionary with positional or name key to expanded parameters.
+        :param parameters: the parts[1:] of a template, i.e. all except the title.
+        """
+        templateParams = {}
+
+        if not parameters:
+            return templateParams
+        logging.debug('<templateParams: %s', '|'.join(parameters))
+
+        # Parameters can be either named or unnamed. In the latter case, their
+        # name is defined by their ordinal position (1, 2, 3, ...).
+
+        unnamedParameterCounter = 0
+
+        # It's legal for unnamed parameters to be skipped, in which case they
+        # will get default values (if available) during actual instantiation.
+        # That is {{template_name|a||c}} means parameter 1 gets
+        # the value 'a', parameter 2 value is not defined, and parameter 3 gets
+        # the value 'c'.  This case is correctly handled by function 'split',
+        # and does not require any special handling.
+        for param in parameters:
+            # Spaces before or after a parameter value are normally ignored,
+            # UNLESS the parameter contains a link (to prevent possible gluing
+            # the link to the following text after template substitution)
+
+            # Parameter values may contain "=" symbols, hence the parameter
+            # name extends up to the first such symbol.
+
+            # It is legal for a parameter to be specified several times, in
+            # which case the last assignment takes precedence. Example:
+            # "{{t|a|b|c|2=B}}" is equivalent to "{{t|a|B|c}}".
+            # Therefore, we don't check if the parameter has been assigned a
+            # value before, because anyway the last assignment should override
+            # any previous ones.
+            # FIXME: Don't use DOTALL here since parameters may be tags with
+            # attributes, e.g. <div class="templatequotecite">
+            # Parameters may span several lines, like:
+            # {{Reflist|colwidth=30em|refs=
+            # &lt;ref name=&quot;Goode&quot;&gt;Title&lt;/ref&gt;
+
+            # The '=' might occurr within an HTML attribute:
+            #   "&lt;ref name=value"
+            # but we stop at first.
+
+            # The '=' might occurr within quotes:
+            # ''''<span lang="pt-pt" xml:lang="pt-pt">cénicas</span>'''
+
+            m = re.match(" *([^=']*?) *=(.*)", param, re.DOTALL)
+            if m:
+                # This is a named parameter.  This case also handles parameter
+                # assignments like "2=xxx", where the number of an unnamed
+                # parameter ("2") is specified explicitly - this is handled
+                # transparently.
+
+                parameterName = m.group(1).strip()
+                parameterValue = m.group(2)
+
+                if ']]' not in parameterValue:  # if the value does not contain a link, trim whitespace
+                    parameterValue = parameterValue.strip()
+                templateParams[parameterName] = parameterValue
+            else:
+                # this is an unnamed parameter
+                unnamedParameterCounter += 1
+
+                if ']]' not in param:  # if the value does not contain a link, trim whitespace
+                    param = param.strip()
+                templateParams[str(unnamedParameterCounter)] = param
+        logging.debug('   templateParams> %s', '|'.join(templateParams.values()))
+        return templateParams
+
+    def expandTemplate(self, body):
+        """Expands template invocation.
+        :param body: the parts of a template.
+
+        :see http://meta.wikimedia.org/wiki/Help:Expansion for an explanation
+        of the process.
+
+        See in particular: Expansion of names and values
+        http://meta.wikimedia.org/wiki/Help:Expansion#Expansion_of_names_and_values
+
+        For most parser functions all names and values are expanded,
+        regardless of what is relevant for the result. The branching functions
+        (#if, #ifeq, #iferror, #ifexist, #ifexpr, #switch) are exceptions.
+
+        All names in a template call are expanded, and the titles of the
+        tplargs in the template body, after which it is determined which
+        values must be expanded, and for which tplargs in the template body
+        the first part (default).
+
+        In the case of a tplarg, any parts beyond the first are never
+        expanded.  The possible name and the value of the first part is
+        expanded if the title does not match a name in the template call.
+
+        :see code for braceSubstitution at
+        https://doc.wikimedia.org/mediawiki-core/master/php/html/Parser_8php_source.html#3397:
+
+        """
+
+        # template        = "{{" parts "}}"
+
+        # Templates and tplargs are decomposed in the same way, with pipes as
+        # separator, even though eventually any parts in a tplarg after the first
+        # (the parameter default) are ignored, and an equals sign in the first
+        # part is treated as plain text.
+        # Pipes inside inner templates and tplargs, or inside double rectangular
+        # brackets within the template or tplargs are not taken into account in
+        # this decomposition.
+        # The first part is called title, the other parts are simply called parts.
+
+        # If a part has one or more equals signs in it, the first equals sign
+        # determines the division into name = value. Equals signs inside inner
+        # templates and tplargs, or inside double rectangular brackets within the
+        # part are not taken into account in this decomposition. Parts without
+        # equals sign are indexed 1, 2, .., given as attribute in the <name> tag.
+
+        if len(self.frame) >= self.maxTemplateRecursionLevels:
+            self.recursion_exceeded_2_errs += 1
+            # logging.debug('   INVOCATION> %d %s', len(self.frame), body)
+            return ''
+
+        logging.debug('INVOCATION %d %s', len(self.frame), body)
+
+        parts = splitParts(body)
+        # title is the portion before the first |
+        logging.debug('TITLE %s', parts[0].strip())
+        title = self.expandTemplates(parts[0].strip())
+
+        # SUBST
+        # Apply the template tag to parameters without
+        # substituting into them, e.g.
+        # {{subst:t|a{{{p|q}}}b}} gives the wikitext start-a{{{p|q}}}b-end
+        # @see https://www.mediawiki.org/wiki/Manual:Substitution#Partial_substitution
+        subst = False
+        if re.match(substWords, title, re.IGNORECASE):
+            title = re.sub(substWords, '', title, 1, re.IGNORECASE)
+            subst = True
+
+        if title.lower() in self.magicWords.values:
+            return self.magicWords[title.lower()]
+
+        # Parser functions
+        # The first argument is everything after the first colon.
+        # It has been evaluated above.
+        colon = title.find(':')
+        if colon > 1:
+            funct = title[:colon]
+            parts[0] = title[colon + 1:].strip()  # side-effect (parts[0] not used later)
+            # arguments after first are not evaluated
+            ret = callParserFunction(funct, parts, self.frame)
+            return self.expandTemplates(ret)
+
+        title = fullyQualifiedTemplateTitle(title)
+        if not title:
+            self.template_title_errs += 1
+            return ''
+
+        redirected = redirects.get(title)
+        if redirected:
+            title = redirected
+
+        # get the template
+        if title in templateCache:
+            template = templateCache[title]
+        elif title in templates:
+            template = Template.parse(templates[title])
+            # add it to cache
+            templateCache[title] = template
+            del templates[title]
+        else:
+            # The page being included could not be identified
+            return ''
+
+        # logging.debug('TEMPLATE %s: %s', title, template)
+
+        # tplarg          = "{{{" parts "}}}"
+        # parts           = [ title *( "|" part ) ]
+        # part            = ( part-name "=" part-value ) / ( part-value )
+        # part-name       = wikitext-L3
+        # part-value      = wikitext-L3
+        # wikitext-L3     = literal / template / tplarg / link / comment /
+        #                   line-eating-comment / unclosed-comment /
+        #           	    xmlish-element / *wikitext-L3
+
+        # A tplarg may contain other parameters as well as templates, e.g.:
+        #   {{{text|{{{quote|{{{1|{{error|Error: No text given}}}}}}}}}}}
+        # hence no simple RE like this would work:
+        #   '{{{((?:(?!{{{).)*?)}}}'
+        # We must use full CF parsing.
+
+        # the parameter name itself might be computed, e.g.:
+        #   {{{appointe{{#if:{{{appointer14|}}}|r|d}}14|}}}
+
+        # Because of the multiple uses of double-brace and triple-brace
+        # syntax, expressions can sometimes be ambiguous.
+        # Precedence rules specifed here:
+        # http://www.mediawiki.org/wiki/Preprocessor_ABNF#Ideal_precedence
+        # resolve ambiguities like this:
+        #   {{{{ }}}} -> { {{{ }}} }
+        #   {{{{{ }}}}} -> {{ {{{ }}} }}
+        #
+        # :see: https://en.wikipedia.org/wiki/Help:Template#Handling_parameters
+
+        params = parts[1:]
+
+        if not subst:
+            # Evaluate parameters, since they may contain templates, including
+            # the symbol "=".
+            # {{#ifexpr: {{{1}}} = 1 }}
+            params = [self.expandTemplates(p) for p in params]
+
+        # build a dict of name-values for the parameter values
+        params = self.templateParams(params)
+
+        # Perform parameter substitution
+        # extend frame before subst, since there may be recursion in default
+        # parameter value, e.g. {{OTRS|celebrative|date=April 2015}} in article
+        # 21637542 in enwiki.
+        self.frame.append((title, params))
+        instantiated = template.subst(params, self)
+        # logging.debug('instantiated %d %s', len(self.frame), instantiated)
+        value = self.expandTemplates(instantiated)
+        self.frame.pop()
+        # logging.debug('   INVOCATION> %s %d %s', title, len(self.frame), value)
+        return value
+
+
+# ----------------------------------------------------------------------
+# parameter handling
+
+
+def splitParts(paramsList):
+    """
+    :param paramsList: the parts of a template or tplarg.
+
+    Split template parameters at the separator "|".
+    separator "=".
+
+    Template parameters often contain URLs, internal links, text or even
+    template expressions, since we evaluate templates outside in.
+    This is required for cases like:
+      {{#if: {{{1}}} | {{lc:{{{1}}} | "parameter missing"}}
+    Parameters are separated by "|" symbols. However, we
+    cannot simply split the string on "|" symbols, since these
+    also appear inside templates and internal links, e.g.
+
+     {{if:|
+      |{{#if:the president|
+           |{{#if:|
+               [[Category:Hatnote templates|A{{PAGENAME}}]]
+            }}
+       }}
+     }}
+
+    We split parts at the "|" symbols that are not inside any pair
+    {{{...}}}, {{...}}, [[...]], {|...|}.
+    """
+
+    # Must consider '[' as normal in expansion of Template:EMedicine2:
+    # #ifeq: ped|article|[http://emedicine.medscape.com/article/180-overview|[http://www.emedicine.com/ped/topic180.htm#{{#if: |section~}}
+    # as part of:
+    # {{#ifeq: ped|article|[http://emedicine.medscape.com/article/180-overview|[http://www.emedicine.com/ped/topic180.htm#{{#if: |section~}}}} ped/180{{#if: |~}}]
+
+    # should handle both tpl arg like:
+    #    4|{{{{{subst|}}}CURRENTYEAR}}
+    # and tpl parameters like:
+    #    ||[[Category:People|{{#if:A|A|{{PAGENAME}}}}]]
+
+    sep = '|'
+    parameters = []
+    cur = 0
+    for s, e in findMatchingBraces(paramsList):
+        par = paramsList[cur:s].split(sep)
+        if par:
+            if parameters:
+                # portion before | belongs to previous parameter
+                parameters[-1] += par[0]
+                if len(par) > 1:
+                    # rest are new parameters
+                    parameters.extend(par[1:])
+            else:
+                parameters = par
+        elif not parameters:
+            parameters = ['']  # create first param
+        # add span to last previous parameter
+        parameters[-1] += paramsList[s:e]
+        cur = e
+    # leftover
+    par = paramsList[cur:].split(sep)
+    if par:
+        if parameters:
+            # portion before | belongs to previous parameter
+            parameters[-1] += par[0]
+            if len(par) > 1:
+                # rest are new parameters
+                parameters.extend(par[1:])
+        else:
+            parameters = par
+
+    # logging.debug('splitParts %s %s\nparams: %s', sep, paramsList, str(parameters))
+    return parameters
+
+
+def findMatchingBraces(text, ldelim=0):
+    """
+    :param ldelim: number of braces to match. 0 means match [[]], {{}} and {{{}}}.
+    """
+    # Parsing is done with respect to pairs of double braces {{..}} delimiting
+    # a template, and pairs of triple braces {{{..}}} delimiting a tplarg.
+    # If double opening braces are followed by triple closing braces or
+    # conversely, this is taken as delimiting a template, with one left-over
+    # brace outside it, taken as plain text. For any pattern of braces this
+    # defines a set of templates and tplargs such that any two are either
+    # separate or nested (not overlapping).
+
+    # Unmatched double rectangular closing brackets can be in a template or
+    # tplarg, but unmatched double rectangular opening brackets cannot.
+    # Unmatched double or triple closing braces inside a pair of
+    # double rectangular brackets are treated as plain text.
+    # Other formulation: in ambiguity between template or tplarg on one hand,
+    # and a link on the other hand, the structure with the rightmost opening
+    # takes precedence, even if this is the opening of a link without any
+    # closing, so not producing an actual link.
+
+    # In the case of more than three opening braces the last three are assumed
+    # to belong to a tplarg, unless there is no matching triple of closing
+    # braces, in which case the last two opening braces are are assumed to
+    # belong to a template.
+
+    # We must skip individual { like in:
+    #   {{#ifeq: {{padleft:|1|}} | { | | &nbsp;}}
+    # We must resolve ambiguities like this:
+    #   {{{{ }}}} -> { {{{ }}} }
+    #   {{{{{ }}}}} -> {{ {{{ }}} }}
+    #   {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|...}}
+
+    # Handle:
+    #   {{{{{|safesubst:}}}#Invoke:String|replace|{{{1|{{{{{|safesubst:}}}PAGENAME}}}}}|%s+%([^%(]-%)$||plain=false}}
+    # as well as expressions with stray }:
+    #   {{{link|{{ucfirst:{{{1}}}}}} interchange}}}
+
+    if ldelim:  # 2-3
+        reOpen = re.compile('[{]{%d,}' % ldelim)  # at least ldelim
+        reNext = re.compile('[{]{2,}|}{2,}')  # at least 2 open or close bracces
+    else:
+        reOpen = re.compile('{{2,}|\[{2,}')
+        reNext = re.compile('{{2,}|}{2,}|\[{2,}|]{2,}')  # at least 2
+
+    cur = 0
+    while True:
+        m1 = reOpen.search(text, cur)
+        if not m1:
+            return
+        lmatch = m1.end() - m1.start()
+        if m1.group()[0] == '{':
+            stack = [lmatch]  # stack of opening braces lengths
+        else:
+            stack = [-lmatch]  # negative means [
+        end = m1.end()
+        while True:
+            m2 = reNext.search(text, end)
+            if not m2:
+                return  # unbalanced
+            end = m2.end()
+            brac = m2.group()[0]
+            lmatch = m2.end() - m2.start()
+
+            if brac == '{':
+                stack.append(lmatch)
+            elif brac == '}':
+                while stack:
+                    openCount = stack.pop()  # opening span
+                    if openCount == 0:  # illegal unmatched [[
+                        continue
+                    if lmatch >= openCount:
+                        lmatch -= openCount
+                        if lmatch <= 1:  # either close or stray }
+                            break
+                    else:
+                        # put back unmatched
+                        stack.append(openCount - lmatch)
+                        break
+                if not stack:
+                    yield m1.start(), end - lmatch
+                    cur = end
+                    break
+                elif len(stack) == 1 and 0 < stack[0] < ldelim:
+                    # ambiguous {{{{{ }}} }}
+                    yield m1.start() + stack[0], end
+                    cur = end
+                    break
+            elif brac == '[':  # [[
+                stack.append(-lmatch)
+            else:  # ]]
+                while stack and stack[-1] < 0:  # matching [[
+                    openCount = -stack.pop()
+                    if lmatch >= openCount:
+                        lmatch -= openCount
+                        if lmatch <= 1:  # either close or stray ]
+                            break
+                    else:
+                        # put back unmatched (negative)
+                        stack.append(lmatch - openCount)
+                        break
+                if not stack:
+                    yield m1.start(), end - lmatch
+                    cur = end
+                    break
+                # unmatched ]] are discarded
+                cur = end
+
+
+def findBalanced(text, openDelim, closeDelim):
+    """
+    Assuming that text contains a properly balanced expression using
+    :param openDelim: as opening delimiters and
+    :param closeDelim: as closing delimiters.
+    :return: an iterator producing pairs (start, end) of start and end
+    positions in text containing a balanced expression.
+    """
+    openPat = '|'.join([re.escape(x) for x in openDelim])
+    # patter for delimiters expected after each opening delimiter
+    afterPat = {o: re.compile(openPat + '|' + c, re.DOTALL) for o, c in zip(openDelim, closeDelim)}
+    stack = []
+    start = 0
+    cur = 0
+    # end = len(text)
+    startSet = False
+    startPat = re.compile(openPat)
+    nextPat = startPat
+    while True:
+        next = nextPat.search(text, cur)
+        if not next:
+            return
+        if not startSet:
+            start = next.start()
+            startSet = True
+        delim = next.group(0)
+        if delim in openDelim:
+            stack.append(delim)
+            nextPat = afterPat[delim]
+        else:
+            opening = stack.pop()
+            # assert opening == openDelim[closeDelim.index(next.group(0))]
+            if stack:
+                nextPat = afterPat[stack[-1]]
+            else:
+                yield start, next.end()
+                nextPat = startPat
+                start = next.end()
+                startSet = False
+        cur = next.end()
+
+# ----------------------------------------------------------------------
+# parser functions utilities
+
+
+def ucfirst(string):
+    """:return: a string with just its first character uppercase
+    We can't use title() since it coverts all words.
+    """
+    if string:
+        if len(string) > 1:
+            return string[0].upper() + string[1:]
+        else:
+            return string.upper()
+    else:
+        return ''
+
+
+def lcfirst(string):
+    """:return: a string with its first character lowercase"""
+    if string:
+        if len(string) > 1:
+            return string[0].lower() + string[1:]
+        else:
+            return string.lower()
+    else:
+        return ''
+
+
+def fullyQualifiedTemplateTitle(templateTitle):
+    """
+    Determine the namespace of the page being included through the template
+    mechanism
+    """
+    if templateTitle.startswith(':'):
+        # Leading colon by itself implies main namespace, so strip this colon
+        return ucfirst(templateTitle[1:])
+    else:
+        m = re.match('([^:]*)(:.*)', templateTitle)
+        if m:
+            # colon found but not in the first position - check if it
+            # designates a known namespace
+            prefix = normalizeNamespace(m.group(1))
+            if prefix in knownNamespaces:
+                return prefix + ucfirst(m.group(2))
+    # The title of the page being included is NOT in the main namespace and
+    # lacks any other explicit designation of the namespace - therefore, it
+    # is resolved to the Template namespace (that's the default for the
+    # template inclusion mechanism).
+
+    # This is a defense against pages whose title only contains UTF-8 chars
+    # that are reduced to an empty string. Right now I can think of one such
+    # case - <C2><A0> which represents the non-breaking space.
+    # In this particular case, this page is a redirect to [[Non-nreaking
+    # space]], but having in the system a redirect page with an empty title
+    # causes numerous problems, so we'll live happier without it.
+    if templateTitle:
+        return Extractor.templatePrefix + ucfirst(templateTitle)
+    else:
+        return ''  # caller may log as error
+
+
+def normalizeNamespace(ns):
+    return ucfirst(ns)
+
+
+# ----------------------------------------------------------------------
+# Parser functions
+# see http://www.mediawiki.org/wiki/Help:Extension:ParserFunctions
+# https://github.com/Wikia/app/blob/dev/extensions/ParserFunctions/ParserFunctions_body.php
+
+
+class Infix():
+
+    """Infix operators.
+    The calling sequence for the infix is:
+      x |op| y
+    """
+
+    def __init__(self, function):
+        self.function = function
+
+    def __ror__(self, other):
+        return Infix(lambda x, self=self, other=other: self.function(other, x))
+
+    def __or__(self, other):
+        return self.function(other)
+
+    def __rlshift__(self, other):
+        return Infix(lambda x, self=self, other=other: self.function(other, x))
+
+    def __rshift__(self, other):
+        return self.function(other)
+
+    def __call__(self, value1, value2):
+        return self.function(value1, value2)
+
+
+ROUND = Infix(lambda x, y: round(x, y))
+
+
+def sharp_expr(expr):
+    try:
+        expr = re.sub('=', '==', expr)
+        expr = re.sub('mod', '%', expr)
+        expr = re.sub('\bdiv\b', '/', expr)
+        expr = re.sub('\bround\b', '|ROUND|', expr)
+        return str(eval(expr))
+    except:
+        return '<span class="error"></span>'
+
+
+def sharp_if(testValue, valueIfTrue, valueIfFalse=None, *args):
+    # In theory, we should evaluate the first argument here,
+    # but it was evaluated while evaluating part[0] in expandTemplate().
+    if testValue.strip():
+        # The {{#if:}} function is an if-then-else construct.
+        # The applied condition is: "The condition string is non-empty".
+        valueIfTrue = valueIfTrue.strip()
+        if valueIfTrue:
+            return valueIfTrue
+    elif valueIfFalse:
+        return valueIfFalse.strip()
+    return ""
+
+
+def sharp_ifeq(lvalue, rvalue, valueIfTrue, valueIfFalse=None, *args):
+    rvalue = rvalue.strip()
+    if rvalue:
+        # lvalue is always defined
+        if lvalue.strip() == rvalue:
+            # The {{#ifeq:}} function is an if-then-else construct. The
+            # applied condition is "is rvalue equal to lvalue". Note that this
+            # does only string comparison while MediaWiki implementation also
+            # supports numerical comparissons.
+
+            if valueIfTrue:
+                return valueIfTrue.strip()
+        else:
+            if valueIfFalse:
+                return valueIfFalse.strip()
+    return ""
+
+
+def sharp_iferror(test, then='', Else=None, *args):
+    if re.match('<(?:strong|span|p|div)\s(?:[^\s>]*\s+)*?class="(?:[^"\s>]*\s+)*?error(?:\s[^">]*)?"', test):
+        return then
+    elif Else is None:
+        return test.strip()
+    else:
+        return Else.strip()
+
+
+def sharp_switch(primary, *params):
+    # FIXME: we don't support numeric expressions in primary
+
+    # {{#switch: comparison string
+    #  | case1 = result1
+    #  | case2
+    #  | case4 = result2
+    #  | 1 | case5 = result3
+    #  | #default = result4
+    # }}
+
+    primary = primary.strip()
+    found = False  # for fall through cases
+    default = None
+    rvalue = None
+    lvalue = ''
+    for param in params:
+        # handle cases like:
+        #  #default = [http://www.perseus.tufts.edu/hopper/text?doc=Perseus...]
+        pair = param.split('=', 1)
+        lvalue = pair[0].strip()
+        rvalue = None
+        if len(pair) > 1:
+            # got "="
+            rvalue = pair[1].strip()
+            # check for any of multiple values pipe separated
+            if found or primary in [v.strip() for v in lvalue.split('|')]:
+                # Found a match, return now
+                return rvalue
+            elif lvalue == '#default':
+                default = rvalue
+            rvalue = None  # avoid defaulting to last case
+        elif lvalue == primary:
+            # If the value matches, set a flag and continue
+            found = True
+    # Default case
+    # Check if the last item had no = sign, thus specifying the default case
+    if rvalue is not None:
+        return lvalue
+    elif default is not None:
+        return default
+    return ''
+
+
+# Extension Scribuntu
+def sharp_invoke(module, function, frame):
+    functions = modules.get(module)
+    if functions:
+        funct = functions.get(function)
+        if funct:
+            # find parameters in frame whose title is the one of the original
+            # template invocation
+            templateTitle = fullyQualifiedTemplateTitle(function)
+            if not templateTitle:
+                logging.warn("Template with empty title")
+            pair = next((x for x in frame if x[0] == templateTitle), None)
+            if pair:
+                params = pair[1]
+                # extract positional args
+                params = [params.get(str(i + 1)) for i in range(len(params))]
+                return funct(*params)
+            else:
+                return funct()
+    return ''
+
+
+parserFunctions = {
+
+    '#expr': sharp_expr,
+
+    '#if': sharp_if,
+
+    '#ifeq': sharp_ifeq,
+
+    '#iferror': sharp_iferror,
+
+    '#ifexpr': lambda *args: '',  # not supported
+
+    '#ifexist': lambda *args: '',  # not supported
+
+    '#rel2abs': lambda *args: '',  # not supported
+
+    '#switch': sharp_switch,
+
+    '# language': lambda *args: '',  # not supported
+
+    '#time': lambda *args: '',  # not supported
+
+    '#timel': lambda *args: '',  # not supported
+
+    '#titleparts': lambda *args: '',  # not supported
+
+    # This function is used in some pages to construct links
+    # http://meta.wikimedia.org/wiki/Help:URL
+    'urlencode': lambda string, *rest: urlencode(string),
+
+    'lc': lambda string, *rest: string.lower() if string else '',
+
+    'lcfirst': lambda string, *rest: lcfirst(string),
+
+    'uc': lambda string, *rest: string.upper() if string else '',
+
+    'ucfirst': lambda string, *rest: ucfirst(string),
+
+    'int': lambda string, *rest: str(int(string)),
+
+    'padleft': lambda char, width, string: string.ljust(char, int(pad)), # CHECK_ME
+
+}
+
+
+def callParserFunction(functionName, args, frame):
+    """
+    Parser functions have similar syntax as templates, except that
+    the first argument is everything after the first colon.
+    :param functionName: nameof the parser function
+    :param args: the arguments to the function
+    :return: the result of the invocation, None in case of failure.
+
+    http://meta.wikimedia.org/wiki/Help:ParserFunctions
+    """
+
+    try:
+        if functionName == '#invoke':
+            # special handling of frame
+            ret = sharp_invoke(args[0].strip(), args[1].strip(), frame)
+            # logging.debug('parserFunction> %s %s', args[1], ret)
+            return ret
+        if functionName in parserFunctions:
+            ret = parserFunctions[functionName](*args)
+            # logging.debug('parserFunction> %s(%s) %s', functionName, args, ret)
+            return ret
+    except:
+        return ""  # FIXME: fix errors
+
+    return ""
+
+
+# ----------------------------------------------------------------------
+# Extract Template definition
+
+reNoinclude = re.compile(r'<noinclude>(?:.*?)</noinclude>', re.DOTALL)
+reIncludeonly = re.compile(r'<includeonly>|</includeonly>', re.DOTALL)
+
+# These are built before spawning processes, hence they are shared.
+templates = {}
+redirects = {}
+# cache of parser templates
+# FIXME: sharing this with a Manager slows down.
+templateCache = {}
+
+
+def define_template(title, page):
+    """
+    Adds a template defined in the :param page:.
+    @see https://en.wikipedia.org/wiki/Help:Template#Noinclude.2C_includeonly.2C_and_onlyinclude
+    """
+    global templates
+    global redirects
+
+    # title = normalizeTitle(title)
+
+    # check for redirects
+    m = re.match('#REDIRECT.*?\[\[([^\]]*)]]', page[0], re.IGNORECASE)
+    if m:
+        redirects[title] = m.group(1)  # normalizeTitle(m.group(1))
+        return
+
+    text = unescape(''.join(page))
+
+    # We're storing template text for future inclusion, therefore,
+    # remove all <noinclude> text and keep all <includeonly> text
+    # (but eliminate <includeonly> tags per se).
+    # However, if <onlyinclude> ... </onlyinclude> parts are present,
+    # then only keep them and discard the rest of the template body.
+    # This is because using <onlyinclude> on a text fragment is
+    # equivalent to enclosing it in <includeonly> tags **AND**
+    # enclosing all the rest of the template body in <noinclude> tags.
+
+    # remove comments
+    text = comment.sub('', text)
+
+    # eliminate <noinclude> fragments
+    text = reNoinclude.sub('', text)
+    # eliminate unterminated <noinclude> elements
+    text = re.sub(r'<noinclude\s*>.*$', '', text, flags=re.DOTALL)
+    text = re.sub(r'<noinclude/>', '', text)
+
+    onlyincludeAccumulator = ''
+    for m in re.finditer('<onlyinclude>(.*?)</onlyinclude>', text, re.DOTALL):
+        onlyincludeAccumulator += m.group(1)
+    if onlyincludeAccumulator:
+        text = onlyincludeAccumulator
+    else:
+        text = reIncludeonly.sub('', text)
+
+    if text:
+        if title in templates and templates[title] != text:
+            logging.warn('Redefining: %s', title)
+        templates[title] = text
```

### Comparing `hazm-0.9.0/hazm/corpus_readers/wikipedia_reader.py` & `hazm-0.9.1/hazm/corpus_readers/wikipedia_reader.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ ویکی‌پدیا است.
-
-[پیکرهٔ ویکی‌پدیا](http://download.wikimedia.org/fawiki/latest/fawiki-latest-
-pages-articles.xml.bz2) پیکرهٔ
-عظیمی مشتمل بر تمام مقالات ویکی‌پدیای فارسی است که هر دوماه یکبار بروزرسانی
-می‌شود. برای کسب اطلاعات بیشتر دربارهٔ این پیکره می‌توانید به [صفحهٔ اصلی
-آن](https://dumps.wikimedia.org/backup-index.html) مراجعه کنید.
-
-"""
-
-
-import os
-import re
-import subprocess
-from pathlib import Path
-from typing import Dict
-from typing import Iterator
-
-
-class WikipediaReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ ویکی‌پدیا است.
-
-    Args:
-        fawiki_dump: مسیر فولدر حاوی فایل‌های پیکره.
-        n_jobs: تعداد هسته‌های پردازنده برای پردازش موازی.
-
-    """
-
-    def __init__(self: "WikipediaReader", fawiki_dump: str, n_jobs: int = 2) -> None:
-        self.fawiki_dump = fawiki_dump
-        self.wiki_extractor = Path(__file__).parent / "wiki_extractor.py"
-        self.n_jobs = n_jobs
-
-    def docs(self: "WikipediaReader") -> Iterator[Dict[str, str]]:
-        """مقالات را برمی‌گرداند.
-
-        هر مقاله، شی‌ای متشکل از چند پارامتر است:
-
-        - شناسه (id)،
-        - عنوان (title)،
-        - متن (text)،
-        - نسخهٔ وب (date)،
-        - آدرس صفحه (url).
-
-        Examples:
-            >>> wikipedia = WikipediaReader('corpora/wikipedia.csv')
-            >>> next(wikipedia.docs())['id']
-
-        Yields:
-            مقالهٔ بعدی.
-
-        """
-        proc = subprocess.Popen(
-            [
-                "python",
-                self.wiki_extractor,
-                "--no-templates",
-                "--processes",
-                str(self.n_jobs),
-                "--output",
-                "-",
-                self.fawiki_dump,
-            ],
-            stdout=subprocess.PIPE,
-        )
-        doc_pattern = re.compile(r'<doc id="(\d+)" url="([^\"]+)" title="([^\"]+)">')
-
-        doc = []
-        for line in iter(proc.stdout.readline, b""):
-            line = line.strip().decode("utf8")
-            if line:
-                doc.append(line)
-
-            if line == "</doc>":
-                del doc[1]
-                id, url, title = doc_pattern.match(doc[0]).groups()  # noqa: A001
-                html = "\n".join(doc[1:-1])
-
-                yield {"id": id, "url": url, "title": title, "html": html, "text": html}
-                doc = []
-
-    def texts(self: "WikipediaReader") -> Iterator[str]:
-        """فقط متن مقالات را برمی‌گرداند.
-
-        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با همان تابع
-        ‍[docs()][hazm.corpus_readers.wikipedia_reader.WikipediaReader.docs] و دریافت مقدار
-        پراپرتی `text` نیز می‌توانید همین کار را انجام دهید.
-
-        Examples:
-            >>> wikipedia = WikipediaReader('corpora/wikipedia.csv')
-            >>> next(wikipedia.texts())[:30]
-
-        Yields:
-            متنِ مقالهٔ بعدی.
-
-        """
-        for doc in self.docs():
-            yield doc["text"]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ ویکی‌پدیا است.
+
+[پیکرهٔ ویکی‌پدیا](http://download.wikimedia.org/fawiki/latest/fawiki-latest-
+pages-articles.xml.bz2) پیکرهٔ
+عظیمی مشتمل بر تمام مقالات ویکی‌پدیای فارسی است که هر دوماه یکبار بروزرسانی
+می‌شود. برای کسب اطلاعات بیشتر دربارهٔ این پیکره می‌توانید به [صفحهٔ اصلی
+آن](https://dumps.wikimedia.org/backup-index.html) مراجعه کنید.
+
+"""
+
+
+import os
+import re
+import subprocess
+from pathlib import Path
+from typing import Dict
+from typing import Iterator
+
+
+class WikipediaReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ ویکی‌پدیا است.
+
+    Args:
+        fawiki_dump: مسیر فولدر حاوی فایل‌های پیکره.
+        n_jobs: تعداد هسته‌های پردازنده برای پردازش موازی.
+
+    """
+
+    def __init__(self: "WikipediaReader", fawiki_dump: str, n_jobs: int = 2) -> None:
+        self.fawiki_dump = fawiki_dump
+        self.wiki_extractor = Path(__file__).parent / "wiki_extractor.py"
+        self.n_jobs = n_jobs
+
+    def docs(self: "WikipediaReader") -> Iterator[Dict[str, str]]:
+        """مقالات را برمی‌گرداند.
+
+        هر مقاله، شی‌ای متشکل از چند پارامتر است:
+
+        - شناسه (id)،
+        - عنوان (title)،
+        - متن (text)،
+        - نسخهٔ وب (date)،
+        - آدرس صفحه (url).
+
+        Examples:
+            >>> wikipedia = WikipediaReader('corpora/wikipedia.csv')
+            >>> next(wikipedia.docs())['id']
+
+        Yields:
+            مقالهٔ بعدی.
+
+        """
+        proc = subprocess.Popen(
+            [
+                "python",
+                self.wiki_extractor,
+                "--no-templates",
+                "--processes",
+                str(self.n_jobs),
+                "--output",
+                "-",
+                self.fawiki_dump,
+            ],
+            stdout=subprocess.PIPE,
+        )
+        doc_pattern = re.compile(r'<doc id="(\d+)" url="([^\"]+)" title="([^\"]+)">')
+
+        doc = []
+        for line in iter(proc.stdout.readline, b""):
+            line = line.strip().decode("utf8")
+            if line:
+                doc.append(line)
+
+            if line == "</doc>":
+                del doc[1]
+                id, url, title = doc_pattern.match(doc[0]).groups()  # noqa: A001
+                html = "\n".join(doc[1:-1])
+
+                yield {"id": id, "url": url, "title": title, "html": html, "text": html}
+                doc = []
+
+    def texts(self: "WikipediaReader") -> Iterator[str]:
+        """فقط متن مقالات را برمی‌گرداند.
+
+        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با همان تابع
+        ‍[docs()][hazm.corpus_readers.wikipedia_reader.WikipediaReader.docs] و دریافت مقدار
+        پراپرتی `text` نیز می‌توانید همین کار را انجام دهید.
+
+        Examples:
+            >>> wikipedia = WikipediaReader('corpora/wikipedia.csv')
+            >>> next(wikipedia.texts())[:30]
+
+        Yields:
+            متنِ مقالهٔ بعدی.
+
+        """
+        for doc in self.docs():
+            yield doc["text"]
```

### Comparing `hazm-0.9.0/hazm/dependency_parser.py` & `hazm-0.9.1/hazm/dependency_parser.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,246 +1,246 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای شناساییِ وابستگی‌های دستوری متن است.
-
-**میزان دقت
-این ماژول در نسخهٔ حاضر ۹۷.۱ درصد [^1] است.**
-[^1]:
-این عدد با انتشار هر نسخه بروزرسانی می‌شود
-"""
-
-
-import os
-import tempfile
-from pathlib import Path
-from typing import List
-from typing import Tuple
-from typing import Type
-
-from nltk.parse import DependencyGraph
-from nltk.parse.api import ParserI
-from nltk.parse.malt import MaltParser
-
-
-class MaltParser(MaltParser):
-    """این کلاس شامل توابعی برای شناسایی وابستگی‌های دستوری است.
-
-    Args:
-        tagger: نام تابع `POS Tagger`.
-        lemmatizer: نام کلاس ریشه‌یاب.
-        working_dir: محل ذخیره‌سازی `maltparser‍`.
-        model_file: آدرس مدلِ از پیش آموزش دیده با پسوند `mco`.
-
-    """
-
-    def __init__(
-        self: "MaltParser",
-        tagger: str,
-        lemmatizer: str,
-        working_dir: str = "resources",
-        model_file: str = "langModel.mco",  # Don't rename this file
-    ) -> None:
-        self.tagger = tagger
-        self.working_dir = working_dir
-        self.mco = model_file
-        self._malt_bin = os.path.join(working_dir, "malt.jar")
-        self.lemmatize = (
-            lemmatizer.lemmatize if lemmatizer else lambda w, t: "_"
-        )
-
-    def parse_sents(self: "MaltParser", sentences: str, verbose: bool = False) -> str:
-        """گراف وابستگی را برمی‌گرداند.
-
-        Args:
-            sentences: جملاتی که باید گراف وابستگی آن‌ها استخراج شود.
-            verbose: اگر `True` باشد وابستگی‌های بیشتری را برمی‌گرداند.
-
-        Returns:
-            گراف وابستگی.
-
-        """
-        tagged_sentences = self.tagger.tag_sents(sentences)
-        return self.parse_tagged_sents(tagged_sentences, verbose)
-
-    def parse_tagged_sents(
-        self: "MaltParser",
-        sentences: List[List[Tuple[str, str]]],
-        verbose: bool = False,
-    ) -> str:
-        """گراف وابستگی‌ها را برای جملات ورودی برمی‌گرداند.
-
-        Args:
-            sentences: جملاتی که باید گراف وابستگی‌های آن استخراج شود.
-            verbose: اگر `True` باشد وابستگی‌های بیشتری را برمی‌گرداند..
-
-        Returns:
-            گراف وابستگی جملات.
-
-        Raises:
-            Exception: در صورت بروز خطا یک اکسپشن عمومی صادر می‌شود.
-
-        """
-        input_file = tempfile.NamedTemporaryFile(
-            prefix="malt_input.conll",
-            dir=self.working_dir,
-            delete=False,
-        )
-        output_file = tempfile.NamedTemporaryFile(
-            prefix="malt_output.conll",
-            dir=self.working_dir,
-            delete=False,
-        )
-
-        try:
-            for sentence in sentences:
-                for i, (word, tag) in enumerate(sentence, start=1):
-                    word = word.strip()
-                    if not word:
-                        word = "_"
-                    input_file.write(
-                        (
-                            "\t".join(
-                                [
-                                    str(i),
-                                    word.replace(" ", "_"),
-                                    self.lemmatize(word, tag).replace(" ", "_"),
-                                    tag,
-                                    tag,
-                                    "_",
-                                    "0",
-                                    "ROOT",
-                                    "_",
-                                    "_",
-                                    "\n",
-                                ],
-                            )
-                        ).encode("utf8"),
-                    )
-                input_file.write(b"\n\n")
-            input_file.close()
-
-            cmd = [
-                "java",
-                "-jar",
-                self._malt_bin,
-                "-w",
-                self.working_dir,
-                "-c",
-                self.mco,
-                "-i",
-                input_file.name,
-                "-o",
-                output_file.name,
-                "-m",
-                "parse",
-            ]
-            if self._execute(cmd, verbose) != 0:
-                raise Exception("MaltParser parsing failed: %s" % " ".join(cmd))
-
-            return (
-                DependencyGraph(item)
-                for item in open(output_file.name, encoding="utf8").read().split("\n\n")
-                if item.strip()
-            )
-
-        finally:
-            input_file.close()
-            os.remove(input_file.name)
-            output_file.close()
-            os.remove(output_file.name)
-
-
-class TurboParser(ParserI):
-    """interfaces [TurboParser](http://www.ark.cs.cmu.edu/TurboParser/) which you must
-    manually install.
-
-    """
-
-    def __init__(self: "TurboParser", tagger, lemmatizer: str, model_file: str) -> None:
-        self.tagger = tagger
-        self.lemmatize = (
-            lemmatizer.lemmatize if lemmatizer else lambda w, t: "_"
-        )
-
-        import turboparser
-
-        self._pturboparser = turboparser.PTurboParser()
-        self.interface = self._pturboparser.create_parser()
-        self.interface.load_parser_model(model_file)
-
-    def parse_sents(
-        self: "TurboParser",
-        sentences: List[List[Tuple[str, str]]],
-    ) -> Type[DependencyGraph]:
-        """parse_sents."""
-        tagged_sentences = self.tagger.tag_sents(sentences)
-        return self.tagged_parse_sents(tagged_sentences)
-
-    def tagged_parse_sents(
-        self: "TurboParser",
-        sentences: List[List[Tuple[str, str]]],
-    ) -> Type[DependencyGraph]:
-        """tagged_parse_sents."""
-        input_file = tempfile.NamedTemporaryFile(
-            prefix="turbo_input.conll",
-            dir="resources",
-            delete=False,
-        )
-        output_file = tempfile.NamedTemporaryFile(
-            prefix="turbo_output.conll",
-            dir="resources",
-            delete=False,
-        )
-
-        try:
-            for sentence in sentences:
-                for i, (word, tag) in enumerate(sentence, start=1):
-                    word = word.strip()
-                    if not word:
-                        word = "_"
-                    input_file.write(
-                        (
-                            "\t".join(
-                                [
-                                    str(i),
-                                    word.replace(" ", "_"),
-                                    self.lemmatize(word, tag).replace(" ", "_"),
-                                    tag,
-                                    tag,
-                                    "_",
-                                    "0",
-                                    "ROOT",
-                                    "_",
-                                    "_",
-                                    "\n",
-                                ],
-                            )
-                        ).encode("utf8"),
-                    )
-                input_file.write(b"\n")
-            input_file.close()
-
-            self.interface.parse(input_file.name, output_file.name)
-
-            return (
-                DependencyGraph(item, cell_extractor=lambda cells: cells[1:8])
-                for item in open(output_file.name, encoding="utf8").read().split("\n\n")
-                if item.strip()
-            )
-
-        finally:
-            input_file.close()
-            os.remove(input_file.name)
-            output_file.close()
-            os.remove(output_file.name)
-
-
-class DependencyParser(MaltParser):
-    """این کلاس شامل توابعی برای شناسایی وابستگی‌های دستوری است.
-
-    این کلاس تمام توابع خود را از کلاس
-    [MaltParser][hazm.dependency_parser.MaltParser] به ارث می‌برد.
-
-    Examples:
-        >>> from hazm import POSTagger, Lemmatizer, DependencyParser
-        >>> parser = DependencyParser(tagger=POSTagger(model='resources/pos_tagger.model'), lemmatizer=Lemmatizer())
-        >>> parser.parse(['من', 'به', 'مدرسه', 'رفته بودم', '.']).tree().pprint()
-        (من (به (مدرسه (رفته_بودم .))))
-    """
+"""این ماژول شامل کلاس‌ها و توابعی برای شناساییِ وابستگی‌های دستوری متن است.
+
+**میزان دقت
+این ماژول در نسخهٔ حاضر ۹۷.۱ درصد [^1] است.**
+[^1]:
+این عدد با انتشار هر نسخه بروزرسانی می‌شود
+"""
+
+
+import os
+import tempfile
+from pathlib import Path
+from typing import List
+from typing import Tuple
+from typing import Type
+
+from nltk.parse import DependencyGraph
+from nltk.parse.api import ParserI
+from nltk.parse.malt import MaltParser
+
+
+class MaltParser(MaltParser):
+    """این کلاس شامل توابعی برای شناسایی وابستگی‌های دستوری است.
+
+    Args:
+        tagger: نام تابع `POS Tagger`.
+        lemmatizer: نام کلاس ریشه‌یاب.
+        working_dir: محل ذخیره‌سازی `maltparser‍`.
+        model_file: آدرس مدلِ از پیش آموزش دیده با پسوند `mco`.
+
+    """
+
+    def __init__(
+        self: "MaltParser",
+        tagger: str,
+        lemmatizer: str,
+        working_dir: str = "resources",
+        model_file: str = "langModel.mco",  # Don't rename this file
+    ) -> None:
+        self.tagger = tagger
+        self.working_dir = working_dir
+        self.mco = model_file
+        self._malt_bin = os.path.join(working_dir, "malt.jar")
+        self.lemmatize = (
+            lemmatizer.lemmatize if lemmatizer else lambda w, t: "_"
+        )
+
+    def parse_sents(self: "MaltParser", sentences: str, verbose: bool = False) -> str:
+        """گراف وابستگی را برمی‌گرداند.
+
+        Args:
+            sentences: جملاتی که باید گراف وابستگی آن‌ها استخراج شود.
+            verbose: اگر `True` باشد وابستگی‌های بیشتری را برمی‌گرداند.
+
+        Returns:
+            گراف وابستگی.
+
+        """
+        tagged_sentences = self.tagger.tag_sents(sentences)
+        return self.parse_tagged_sents(tagged_sentences, verbose)
+
+    def parse_tagged_sents(
+        self: "MaltParser",
+        sentences: List[List[Tuple[str, str]]],
+        verbose: bool = False,
+    ) -> str:
+        """گراف وابستگی‌ها را برای جملات ورودی برمی‌گرداند.
+
+        Args:
+            sentences: جملاتی که باید گراف وابستگی‌های آن استخراج شود.
+            verbose: اگر `True` باشد وابستگی‌های بیشتری را برمی‌گرداند..
+
+        Returns:
+            گراف وابستگی جملات.
+
+        Raises:
+            Exception: در صورت بروز خطا یک اکسپشن عمومی صادر می‌شود.
+
+        """
+        input_file = tempfile.NamedTemporaryFile(
+            prefix="malt_input.conll",
+            dir=self.working_dir,
+            delete=False,
+        )
+        output_file = tempfile.NamedTemporaryFile(
+            prefix="malt_output.conll",
+            dir=self.working_dir,
+            delete=False,
+        )
+
+        try:
+            for sentence in sentences:
+                for i, (word, tag) in enumerate(sentence, start=1):
+                    word = word.strip()
+                    if not word:
+                        word = "_"
+                    input_file.write(
+                        (
+                            "\t".join(
+                                [
+                                    str(i),
+                                    word.replace(" ", "_"),
+                                    self.lemmatize(word, tag).replace(" ", "_"),
+                                    tag,
+                                    tag,
+                                    "_",
+                                    "0",
+                                    "ROOT",
+                                    "_",
+                                    "_",
+                                    "\n",
+                                ],
+                            )
+                        ).encode("utf8"),
+                    )
+                input_file.write(b"\n\n")
+            input_file.close()
+
+            cmd = [
+                "java",
+                "-jar",
+                self._malt_bin,
+                "-w",
+                self.working_dir,
+                "-c",
+                self.mco,
+                "-i",
+                input_file.name,
+                "-o",
+                output_file.name,
+                "-m",
+                "parse",
+            ]
+            if self._execute(cmd, verbose) != 0:
+                raise Exception("MaltParser parsing failed: %s" % " ".join(cmd))
+
+            return (
+                DependencyGraph(item)
+                for item in open(output_file.name, encoding="utf8").read().split("\n\n")
+                if item.strip()
+            )
+
+        finally:
+            input_file.close()
+            os.remove(input_file.name)
+            output_file.close()
+            os.remove(output_file.name)
+
+
+class TurboParser(ParserI):
+    """interfaces [TurboParser](http://www.ark.cs.cmu.edu/TurboParser/) which you must
+    manually install.
+
+    """
+
+    def __init__(self: "TurboParser", tagger, lemmatizer: str, model_file: str) -> None:
+        self.tagger = tagger
+        self.lemmatize = (
+            lemmatizer.lemmatize if lemmatizer else lambda w, t: "_"
+        )
+
+        import turboparser
+
+        self._pturboparser = turboparser.PTurboParser()
+        self.interface = self._pturboparser.create_parser()
+        self.interface.load_parser_model(model_file)
+
+    def parse_sents(
+        self: "TurboParser",
+        sentences: List[List[Tuple[str, str]]],
+    ) -> Type[DependencyGraph]:
+        """parse_sents."""
+        tagged_sentences = self.tagger.tag_sents(sentences)
+        return self.tagged_parse_sents(tagged_sentences)
+
+    def tagged_parse_sents(
+        self: "TurboParser",
+        sentences: List[List[Tuple[str, str]]],
+    ) -> Type[DependencyGraph]:
+        """tagged_parse_sents."""
+        input_file = tempfile.NamedTemporaryFile(
+            prefix="turbo_input.conll",
+            dir="resources",
+            delete=False,
+        )
+        output_file = tempfile.NamedTemporaryFile(
+            prefix="turbo_output.conll",
+            dir="resources",
+            delete=False,
+        )
+
+        try:
+            for sentence in sentences:
+                for i, (word, tag) in enumerate(sentence, start=1):
+                    word = word.strip()
+                    if not word:
+                        word = "_"
+                    input_file.write(
+                        (
+                            "\t".join(
+                                [
+                                    str(i),
+                                    word.replace(" ", "_"),
+                                    self.lemmatize(word, tag).replace(" ", "_"),
+                                    tag,
+                                    tag,
+                                    "_",
+                                    "0",
+                                    "ROOT",
+                                    "_",
+                                    "_",
+                                    "\n",
+                                ],
+                            )
+                        ).encode("utf8"),
+                    )
+                input_file.write(b"\n")
+            input_file.close()
+
+            self.interface.parse(input_file.name, output_file.name)
+
+            return (
+                DependencyGraph(item, cell_extractor=lambda cells: cells[1:8])
+                for item in open(output_file.name, encoding="utf8").read().split("\n\n")
+                if item.strip()
+            )
+
+        finally:
+            input_file.close()
+            os.remove(input_file.name)
+            output_file.close()
+            os.remove(output_file.name)
+
+
+class DependencyParser(MaltParser):
+    """این کلاس شامل توابعی برای شناسایی وابستگی‌های دستوری است.
+
+    این کلاس تمام توابع خود را از کلاس
+    [MaltParser][hazm.dependency_parser.MaltParser] به ارث می‌برد.
+
+    Examples:
+        >>> from hazm import POSTagger, Lemmatizer, DependencyParser
+        >>> parser = DependencyParser(tagger=POSTagger(model='resources/pos_tagger.model'), lemmatizer=Lemmatizer())
+        >>> parser.parse(['من', 'به', 'مدرسه', 'رفته بودم', '.']).tree().pprint()
+        (من (به (مدرسه (رفته_بودم .))))
+    """
```

### Comparing `hazm-0.9.0/hazm/embedding.py` & `hazm-0.9.1/hazm/embedding.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,412 +1,412 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای تبدیل کلمه یا متن به برداری از اعداد است."""
-import multiprocessing
-import os
-import warnings
-from pathlib import Path
-from typing import Any
-from typing import Iterator
-from typing import List
-from typing import Tuple
-from typing import Type
-
-from gensim.models import Doc2Vec
-from gensim.models import KeyedVectors
-from gensim.models import fasttext
-from gensim.models.doc2vec import TaggedDocument
-from gensim.scripts.glove2word2vec import glove2word2vec
-from gensim.test.utils import datapath
-from numpy import ndarray
-
-from hazm import Normalizer
-
-from hazm import word_tokenize
-
-supported_embeddings = ["fasttext", "keyedvector", "glove"]
-
-
-class WordEmbedding:
-    """این کلاس شامل توابعی برای تبدیل کلمه به برداری از اعداد است.
-
-    Args:
-        model_type: نوع امبدینگ که می‌تواند یکی از مقادیر ‍`fasttext`, `keyedvector`, `glove` باشد.
-        model_path: مسیر فایل امبدینگ.
-
-    """
-
-    def __init__(
-        self: "WordEmbedding",
-        model_type: str,
-        model_path: str = None,
-    ) -> None:
-        if model_type not in supported_embeddings:
-            msg = (
-                f'Model type "{model_type}" is not supported! Please choose from'
-                f" {supported_embeddings}"
-            )
-            raise KeyError(
-                msg,
-            )
-        self.model_type = model_type
-        if model_path:
-            self.load_model(model_path)
-
-    def load_model(self: "WordEmbedding", model_path: str) -> None:
-        """فایل امبدینگ را بارگزاری می‌کند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
-            >>> wordEmbedding.load_model('resources/cc.fa.300.bin')
-
-        Args:
-            model_path: مسیر فایل امبدینگ.
-
-        """
-        if self.model_type == "fasttext":
-            self.model = fasttext.load_facebook_model(model_path).wv
-        elif self.model_type == "keyedvector":
-            if model_path.endswith("bin"):
-                self.model = KeyedVectors.load_word2vec_format(model_path, binary=True)
-            else:
-                self.model = KeyedVectors.load_word2vec_format(model_path)
-        elif self.model_type == "glove":
-            word2vec_addr = str(model_path) + "_word2vec_format.vec"
-            if not Path.exists(word2vec_addr):
-                _ = glove2word2vec(model_path, word2vec_addr)
-            self.model = KeyedVectors.load_word2vec_format(word2vec_addr)
-            self.model_type = "keyedvector"
-        else:
-            msg = (
-                f"{self.model_type} not supported! Please choose from"
-                f" {supported_embeddings}"
-            )
-            raise KeyError(
-                msg,
-            )
-
-    def train(
-        self: "WordEmbedding",
-        dataset_path: str,
-        workers: int = multiprocessing.cpu_count() - 1,  # noqa: B008
-        vector_size: int = 200,
-        epochs: int = 10,
-        fasttext_type: str = "skipgram",
-        dest_path: str = None,
-    ) -> None:
-        """یک فایل امبدینگ از نوع fasttext ترین می‌کند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
-            >>> wordEmbedding.train(dataset_path = 'dataset.txt', worker = 4, vector_size = 300, epochs = 30, fasttext_type = 'cbow', dest_path = 'fasttext_model')
-
-        Args:
-            dataset_path: مسیر فایل متنی.
-            workers: تعداد هسته درگیر برای ترین مدل.
-            vector_size: طول وکتور خروجی به ازای هر کلمه.
-            epochs: تعداد تکرار ترین بر روی کل دیتا.
-            fasttext_type: نوع fasttext مورد نظر برای ترین که میتواند یکی از مقادیر skipgram یا cbow را داشته باشد.
-            dest_path: مسیر مورد نظر برای ذخیره فایل امبدینگ.
-
-        """
-        if self.model_type != "fasttext":
-            self.model = "fasttext"
-            warnings.warn(
-                (
-                    "this function is for training fasttext models only and"
-                    f" {self.model_type} is not supported"
-                ),
-                stacklevel=2,
-            )
-
-        fasttext_model_types = ["cbow", "skipgram"]
-        if fasttext_type not in fasttext_model_types:
-            msg = (
-                f'Model type "{fasttext_type}" is not supported! Please choose from'
-                f" {fasttext_model_types}"
-            )
-            raise KeyError(
-                msg,
-            )
-
-        workers = 1 if workers == 0 else workers
-
-        model = fasttext.train_unsupervised(
-            dataset_path,
-            model=fasttext_type,
-            dim=vector_size,
-            epoch=epochs,
-            thread=workers,
-        )
-
-        self.model = model.wv
-
-        print("Model trained.")
-
-        if dest_path is not None:
-            model.save_model(dest_path)
-            print("Model saved.")
-
-    def __getitem__(self: "WordEmbedding", word: str) -> str:
-        """__getitem__."""
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.model[word]
-
-    def doesnt_match(self: "WordEmbedding", words: List[str]) -> str:
-        """لیستی از کلمات را دریافت می‌کند و کلمهٔ نامرتبط را برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.doesnt_match(['سلام' ,'درود' ,'خداحافظ' ,'پنجره'])
-            'پنجره'
-            >>> wordEmbedding.doesnt_match(['ساعت' ,'پلنگ' ,'شیر'])
-            'ساعت'
-
-        Args:
-            words: لیست کلمات.
-
-        Returns:
-            کلمهٔ نامرتبط.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.model.doesnt_match(words)
-
-    def similarity(self: "WordEmbedding", word1: str, word2: str) -> float:
-        """میزان شباهت دو کلمه را برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.similarity('ایران', 'آلمان')
-            0.44988164
-            >>> wordEmbedding.similarity('ایران', 'پنجره')
-            0.08837362
-
-        Args:
-            word1: کلمهٔ اول
-            word2: کلمهٔ دوم
-
-        Returns:
-            میزان شباهت دو کلمه.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return float(str(self.model.similarity(word1, word2)))
-
-    def get_vocab(self: "WordEmbedding") -> List[str]:
-        """لیستی از کلمات موجود در فایل امبدینگ را برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.get_vocab()
-            ['،', 'در', '.', 'و', ...]
-
-        Returns:
-            لیست کلمات موجود در فایل امبدینگ.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.model.index_to_key
-
-    def nearest_words(
-        self: "WordEmbedding",
-        word: str,
-        topn: int = 5,
-    ) -> List[Tuple[str, str]]:
-        """کلمات مرتبط با یک واژه را به همراه میزان ارتباط آن برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.nearest_words('ایران', topn = 5)
-            [('ايران', 0.657148540019989'), (جمهوری', 0.6470394134521484'), (آمریکا', 0.635792076587677'), (اسلامی', 0.6354473233222961'), (کشور', 0.6339613795280457')]
-
-        Args:
-            word: کلمه‌ای که می‌خواهید واژگان مرتبط با آن را بدانید.
-            topn: تعداد کلمات مرتبطی که می‌خواهید برگردانده شود.
-
-        Returns:
-            لیستی از تاپل‌های [`کلمهٔ مرتبط`, `میزان ارتباط`].
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.model.most_similar(word, topn=topn)
-
-    def get_normal_vector(self: "WordEmbedding", word: str) -> Type[ndarray]:
-        """بردار امبدینگ نرمالایزشدهٔ کلمه ورودی را برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.get_normal_vector('سرباز')
-            array([ 8.99544358e-03,  2.76231226e-02, -1.06164828e-01, ..., -9.45233554e-02, -7.59726465e-02, -8.96625668e-02], dtype=float32)
-
-        Args:
-            word: کلمه‌ای که می‌خواهید بردار متناظر با آن را بدانید.
-
-        Returns:
-            لیست بردار نرمالایزشدهٔ مرتبط با کلمهٔ ورودی.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-
-        return self.model.get_vector(word=word, norm=True)
-
-
-class SentEmbedding:
-    """این کلاس شامل توابعی برای تبدیل جمله به برداری از اعداد است.
-
-    Args:
-        model_path: مسیر فایل امبدینگ.
-
-    """
-
-    def __init__(self: "SentEmbedding", model_path: str = None) -> None:
-        if model_path:
-            self.load_model(model_path)
-
-    def load_model(self: "SentEmbedding", model_path: str) -> None:
-        """فایل امبدینگ را بارگذاری می‌کند.
-
-        Examples:
-            >>> sentEmbedding = SentEmbedding()
-            >>> sentEmbedding.load_model('sent2vec_model_path')
-
-        Args:
-            model_path: مسیر فایل امبدینگ.
-
-        """
-        self.model = Doc2Vec.load(model_path)
-
-    def train(
-        self: "SentEmbedding",
-        dataset_path: str,
-        min_count: int = 5,
-        workers: int = multiprocessing.cpu_count() - 1,  # noqa: B008
-        windows: int = 5,
-        vector_size: int = 300,
-        epochs: int = 10,
-        dest_path: str = None,
-    ) -> None:
-        """یک فایل امبدینگ doc2vec ترین می‌کند.
-
-        Examples:
-            >>> sentEmbedding = SentEmbedding()
-            >>> sentEmbedding.train(dataset_path = 'dataset.txt', min_count = 10, worker = 6, windows = 3, vector_size = 250, epochs = 35, dest_path = 'doc2vec_model')
-
-        Args:
-            dataset_path: مسیر فایل متنی.
-            min_count: مینیموم دفعات تکرار یک کلمه برای حضور آن در لیست کلمات امبدینگ.
-            workers: تعداد هسته درگیر برای ترین مدل.
-            windows: طول پنجره برای لحاظ کلمات اطراف یک کلمه در ترین آن.
-            vector_size: طول وکتور خروجی به ازای هر جمله.
-            epochs: تعداد تکرار ترین بر روی کل دیتا.
-            dest_path: مسیر مورد نظر برای ذخیره فایل امبدینگ.
-
-        """
-        workers = 1 if workers == 0 else workers
-
-        doc = SentenceEmbeddingCorpus(dataset_path)
-
-        model = Doc2Vec(
-            min_count=min_count,
-            window=windows,
-            vector_size=vector_size,
-            workers=workers,
-        )
-        model.build_vocab(doc)
-        model.train(doc, total_examples=model.corpus_count, epochs=epochs)
-
-        self.model = model
-
-        print("Model trained.")
-
-        if dest_path is not None:
-            model.save(dest_path)
-            print("Model saved.")
-
-    def __getitem__(self: "SentEmbedding", sent: str) -> Type[ndarray]:
-        """__getitem__."""
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.get_sentence_vector(sent)
-
-    def get_sentence_vector(self: "SentEmbedding", sent: str) -> str:
-        """جمله‌ای را دریافت می‌کند و بردار امبدینگ متناظر با آن را برمی‌گرداند.
-
-        Examples:
-            >>> sentEmbedding = SentEmbedding(sent_embedding_file)
-            >>> sentEmbedding.get_sentence_vector('این متن به برداری متناظر با خودش تبدیل خواهد شد')
-            array([-0.28460968,  0.04566888, -0.00979532, ..., -0.4701098 , -0.3010612 , -0.18577948], dtype=float32)
-
-        Args:
-            sent: جمله‌ای که می‌خواهید بردار امبیدنگ آن را دریافت کنید.
-
-        Returns:
-            لیست بردار مرتبط با جملهٔ ورودی.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-
-        tokenized_sent = word_tokenize(sent)
-        return self.model.infer_vector(tokenized_sent)
-
-    def similarity(self: "SentEmbedding", sent1: str, sent2: str) -> float:
-        """میزان شباهت دو جمله را برمی‌گرداند.
-
-        Examples:
-            >>> sentEmbedding = SentEmbedding(sent_embedding_file)
-            >>> sentEmbedding.similarity('شیر حیوانی وحشی است', 'پلنگ از دیگر جانوران درنده است')
-            0.8748713
-            >>> sentEmbedding.similarity('هضم یک محصول پردازش متن فارسی است', 'شیر حیوانی وحشی است')
-            0.2379288
-
-        Args:
-            sent1: جملهٔ اول.
-            sent2: جملهٔ دوم.
-
-        Returns:
-            میزان شباهت دو جمله که عددی بین `0` و`1` است.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-
-        return float(
-            str(
-                self.model.similarity_unseen_docs(
-                    word_tokenize(sent1),
-                    word_tokenize(sent2),
-                ),
-            ),
-        )
-
-
-class SentenceEmbeddingCorpus:
-    """SentenceEmbeddingCorpus."""
-
-    def __init__(self: "SentenceEmbeddingCorpus", data_path: str) -> None:
-        """__init__."""
-        self.data_path = data_path
-
-    def __iter__(self: "SentenceEmbeddingCorpus") -> Iterator[TaggedDocument]:
-        """__iter__."""
-        corpus_path = datapath(self.data_path)
-        
-        for i, list_of_words in enumerate(Path.open(corpus_path)):
-            yield TaggedDocument(
-                word_tokenize(Normalizer().normalize(list_of_words)),
-                [i],
-            )
+"""این ماژول شامل کلاس‌ها و توابعی برای تبدیل کلمه یا متن به برداری از اعداد است."""
+import multiprocessing
+import os
+import warnings
+from pathlib import Path
+from typing import Any
+from typing import Iterator
+from typing import List
+from typing import Tuple
+from typing import Type
+
+from gensim.models import Doc2Vec
+from gensim.models import KeyedVectors
+from gensim.models import fasttext
+from gensim.models.doc2vec import TaggedDocument
+from gensim.scripts.glove2word2vec import glove2word2vec
+from gensim.test.utils import datapath
+from numpy import ndarray
+
+from hazm import Normalizer
+
+from hazm import word_tokenize
+
+supported_embeddings = ["fasttext", "keyedvector", "glove"]
+
+
+class WordEmbedding:
+    """این کلاس شامل توابعی برای تبدیل کلمه به برداری از اعداد است.
+
+    Args:
+        model_type: نوع امبدینگ که می‌تواند یکی از مقادیر ‍`fasttext`, `keyedvector`, `glove` باشد.
+        model_path: مسیر فایل امبدینگ.
+
+    """
+
+    def __init__(
+        self: "WordEmbedding",
+        model_type: str,
+        model_path: str = None,
+    ) -> None:
+        if model_type not in supported_embeddings:
+            msg = (
+                f'Model type "{model_type}" is not supported! Please choose from'
+                f" {supported_embeddings}"
+            )
+            raise KeyError(
+                msg,
+            )
+        self.model_type = model_type
+        if model_path:
+            self.load_model(model_path)
+
+    def load_model(self: "WordEmbedding", model_path: str) -> None:
+        """فایل امبدینگ را بارگزاری می‌کند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('resources/cc.fa.300.bin')
+
+        Args:
+            model_path: مسیر فایل امبدینگ.
+
+        """
+        if self.model_type == "fasttext":
+            self.model = fasttext.load_facebook_model(model_path).wv
+        elif self.model_type == "keyedvector":
+            if model_path.endswith("bin"):
+                self.model = KeyedVectors.load_word2vec_format(model_path, binary=True)
+            else:
+                self.model = KeyedVectors.load_word2vec_format(model_path)
+        elif self.model_type == "glove":
+            word2vec_addr = str(model_path) + "_word2vec_format.vec"
+            if not Path.exists(word2vec_addr):
+                _ = glove2word2vec(model_path, word2vec_addr)
+            self.model = KeyedVectors.load_word2vec_format(word2vec_addr)
+            self.model_type = "keyedvector"
+        else:
+            msg = (
+                f"{self.model_type} not supported! Please choose from"
+                f" {supported_embeddings}"
+            )
+            raise KeyError(
+                msg,
+            )
+
+    def train(
+        self: "WordEmbedding",
+        dataset_path: str,
+        workers: int = multiprocessing.cpu_count() - 1,  # noqa: B008
+        vector_size: int = 200,
+        epochs: int = 10,
+        fasttext_type: str = "skipgram",
+        dest_path: str = None,
+    ) -> None:
+        """یک فایل امبدینگ از نوع fasttext ترین می‌کند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.train(dataset_path = 'dataset.txt', worker = 4, vector_size = 300, epochs = 30, fasttext_type = 'cbow', dest_path = 'fasttext_model')
+
+        Args:
+            dataset_path: مسیر فایل متنی.
+            workers: تعداد هسته درگیر برای ترین مدل.
+            vector_size: طول وکتور خروجی به ازای هر کلمه.
+            epochs: تعداد تکرار ترین بر روی کل دیتا.
+            fasttext_type: نوع fasttext مورد نظر برای ترین که میتواند یکی از مقادیر skipgram یا cbow را داشته باشد.
+            dest_path: مسیر مورد نظر برای ذخیره فایل امبدینگ.
+
+        """
+        if self.model_type != "fasttext":
+            self.model = "fasttext"
+            warnings.warn(
+                (
+                    "this function is for training fasttext models only and"
+                    f" {self.model_type} is not supported"
+                ),
+                stacklevel=2,
+            )
+
+        fasttext_model_types = ["cbow", "skipgram"]
+        if fasttext_type not in fasttext_model_types:
+            msg = (
+                f'Model type "{fasttext_type}" is not supported! Please choose from'
+                f" {fasttext_model_types}"
+            )
+            raise KeyError(
+                msg,
+            )
+
+        workers = 1 if workers == 0 else workers
+
+        model = fasttext.train_unsupervised(
+            dataset_path,
+            model=fasttext_type,
+            dim=vector_size,
+            epoch=epochs,
+            thread=workers,
+        )
+
+        self.model = model.wv
+
+        print("Model trained.")
+
+        if dest_path is not None:
+            model.save_model(dest_path)
+            print("Model saved.")
+
+    def __getitem__(self: "WordEmbedding", word: str) -> str:
+        """__getitem__."""
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.model[word]
+
+    def doesnt_match(self: "WordEmbedding", words: List[str]) -> str:
+        """لیستی از کلمات را دریافت می‌کند و کلمهٔ نامرتبط را برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
+            >>> wordEmbedding.doesnt_match(['سلام' ,'درود' ,'خداحافظ' ,'پنجره'])
+            'پنجره'
+            >>> wordEmbedding.doesnt_match(['ساعت' ,'پلنگ' ,'شیر'])
+            'ساعت'
+
+        Args:
+            words: لیست کلمات.
+
+        Returns:
+            کلمهٔ نامرتبط.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.model.doesnt_match(words)
+
+    def similarity(self: "WordEmbedding", word1: str, word2: str) -> float:
+        """میزان شباهت دو کلمه را برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
+            >>> wordEmbedding.similarity('ایران', 'آلمان')
+            0.44988164
+            >>> wordEmbedding.similarity('ایران', 'پنجره')
+            0.08837362
+
+        Args:
+            word1: کلمهٔ اول
+            word2: کلمهٔ دوم
+
+        Returns:
+            میزان شباهت دو کلمه.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return float(str(self.model.similarity(word1, word2)))
+
+    def get_vocab(self: "WordEmbedding") -> List[str]:
+        """لیستی از کلمات موجود در فایل امبدینگ را برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
+            >>> wordEmbedding.get_vocab()
+            ['،', 'در', '.', 'و', ...]
+
+        Returns:
+            لیست کلمات موجود در فایل امبدینگ.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.model.index_to_key
+
+    def nearest_words(
+        self: "WordEmbedding",
+        word: str,
+        topn: int = 5,
+    ) -> List[Tuple[str, str]]:
+        """کلمات مرتبط با یک واژه را به همراه میزان ارتباط آن برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
+            >>> wordEmbedding.nearest_words('ایران', topn = 5)
+            [('ايران', 0.657148540019989'), (جمهوری', 0.6470394134521484'), (آمریکا', 0.635792076587677'), (اسلامی', 0.6354473233222961'), (کشور', 0.6339613795280457')]
+
+        Args:
+            word: کلمه‌ای که می‌خواهید واژگان مرتبط با آن را بدانید.
+            topn: تعداد کلمات مرتبطی که می‌خواهید برگردانده شود.
+
+        Returns:
+            لیستی از تاپل‌های [`کلمهٔ مرتبط`, `میزان ارتباط`].
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.model.most_similar(word, topn=topn)
+
+    def get_normal_vector(self: "WordEmbedding", word: str) -> Type[ndarray]:
+        """بردار امبدینگ نرمالایزشدهٔ کلمه ورودی را برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
+            >>> wordEmbedding.get_normal_vector('سرباز')
+            array([ 8.99544358e-03,  2.76231226e-02, -1.06164828e-01, ..., -9.45233554e-02, -7.59726465e-02, -8.96625668e-02], dtype=float32)
+
+        Args:
+            word: کلمه‌ای که می‌خواهید بردار متناظر با آن را بدانید.
+
+        Returns:
+            لیست بردار نرمالایزشدهٔ مرتبط با کلمهٔ ورودی.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+
+        return self.model.get_vector(word=word, norm=True)
+
+
+class SentEmbedding:
+    """این کلاس شامل توابعی برای تبدیل جمله به برداری از اعداد است.
+
+    Args:
+        model_path: مسیر فایل امبدینگ.
+
+    """
+
+    def __init__(self: "SentEmbedding", model_path: str = None) -> None:
+        if model_path:
+            self.load_model(model_path)
+
+    def load_model(self: "SentEmbedding", model_path: str) -> None:
+        """فایل امبدینگ را بارگذاری می‌کند.
+
+        Examples:
+            >>> sentEmbedding = SentEmbedding()
+            >>> sentEmbedding.load_model('sent2vec_model_path')
+
+        Args:
+            model_path: مسیر فایل امبدینگ.
+
+        """
+        self.model = Doc2Vec.load(model_path)
+
+    def train(
+        self: "SentEmbedding",
+        dataset_path: str,
+        min_count: int = 5,
+        workers: int = multiprocessing.cpu_count() - 1,  # noqa: B008
+        windows: int = 5,
+        vector_size: int = 300,
+        epochs: int = 10,
+        dest_path: str = None,
+    ) -> None:
+        """یک فایل امبدینگ doc2vec ترین می‌کند.
+
+        Examples:
+            >>> sentEmbedding = SentEmbedding()
+            >>> sentEmbedding.train(dataset_path = 'dataset.txt', min_count = 10, worker = 6, windows = 3, vector_size = 250, epochs = 35, dest_path = 'doc2vec_model')
+
+        Args:
+            dataset_path: مسیر فایل متنی.
+            min_count: مینیموم دفعات تکرار یک کلمه برای حضور آن در لیست کلمات امبدینگ.
+            workers: تعداد هسته درگیر برای ترین مدل.
+            windows: طول پنجره برای لحاظ کلمات اطراف یک کلمه در ترین آن.
+            vector_size: طول وکتور خروجی به ازای هر جمله.
+            epochs: تعداد تکرار ترین بر روی کل دیتا.
+            dest_path: مسیر مورد نظر برای ذخیره فایل امبدینگ.
+
+        """
+        workers = 1 if workers == 0 else workers
+
+        doc = SentenceEmbeddingCorpus(dataset_path)
+
+        model = Doc2Vec(
+            min_count=min_count,
+            window=windows,
+            vector_size=vector_size,
+            workers=workers,
+        )
+        model.build_vocab(doc)
+        model.train(doc, total_examples=model.corpus_count, epochs=epochs)
+
+        self.model = model
+
+        print("Model trained.")
+
+        if dest_path is not None:
+            model.save(dest_path)
+            print("Model saved.")
+
+    def __getitem__(self: "SentEmbedding", sent: str) -> Type[ndarray]:
+        """__getitem__."""
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.get_sentence_vector(sent)
+
+    def get_sentence_vector(self: "SentEmbedding", sent: str) -> str:
+        """جمله‌ای را دریافت می‌کند و بردار امبدینگ متناظر با آن را برمی‌گرداند.
+
+        Examples:
+            >>> sentEmbedding = SentEmbedding(sent_embedding_file)
+            >>> sentEmbedding.get_sentence_vector('این متن به برداری متناظر با خودش تبدیل خواهد شد')
+            array([-0.28460968,  0.04566888, -0.00979532, ..., -0.4701098 , -0.3010612 , -0.18577948], dtype=float32)
+
+        Args:
+            sent: جمله‌ای که می‌خواهید بردار امبیدنگ آن را دریافت کنید.
+
+        Returns:
+            لیست بردار مرتبط با جملهٔ ورودی.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+
+        tokenized_sent = word_tokenize(sent)
+        return self.model.infer_vector(tokenized_sent)
+
+    def similarity(self: "SentEmbedding", sent1: str, sent2: str) -> float:
+        """میزان شباهت دو جمله را برمی‌گرداند.
+
+        Examples:
+            >>> sentEmbedding = SentEmbedding(sent_embedding_file)
+            >>> sentEmbedding.similarity('شیر حیوانی وحشی است', 'پلنگ از دیگر جانوران درنده است')
+            0.8748713
+            >>> sentEmbedding.similarity('هضم یک محصول پردازش متن فارسی است', 'شیر حیوانی وحشی است')
+            0.2379288
+
+        Args:
+            sent1: جملهٔ اول.
+            sent2: جملهٔ دوم.
+
+        Returns:
+            میزان شباهت دو جمله که عددی بین `0` و`1` است.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+
+        return float(
+            str(
+                self.model.similarity_unseen_docs(
+                    word_tokenize(sent1),
+                    word_tokenize(sent2),
+                ),
+            ),
+        )
+
+
+class SentenceEmbeddingCorpus:
+    """SentenceEmbeddingCorpus."""
+
+    def __init__(self: "SentenceEmbeddingCorpus", data_path: str) -> None:
+        """__init__."""
+        self.data_path = data_path
+
+    def __iter__(self: "SentenceEmbeddingCorpus") -> Iterator[TaggedDocument]:
+        """__iter__."""
+        corpus_path = datapath(self.data_path)
+        
+        for i, list_of_words in enumerate(Path.open(corpus_path)):
+            yield TaggedDocument(
+                word_tokenize(Normalizer().normalize(list_of_words)),
+                [i],
+            )
```

### Comparing `hazm-0.9.0/hazm/informal_normalizer.py` & `hazm-0.9.1/hazm/informal_normalizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,856 +1,856 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای نرمال‌سازی متن‌های محاوره‌ای است."""
-
-
-import re
-from pathlib import Path
-from typing import List
-
-from hazm import Lemmatizer
-from hazm import Normalizer
-from hazm import SentenceTokenizer
-from hazm import Stemmer
-from hazm import NUMBERS
-from hazm import informal_verbs
-from hazm import informal_words
-from hazm import WordTokenizer
-from hazm import default_verbs
-
-
-class InformalNormalizer(Normalizer):
-    """این کلاس شامل توابعی برای نرمال‌سازی متن‌های محاوره‌ای است.
-
-    Args:
-        verb_file: فایل حاوی افعال محاوره‌ای.
-        word_file: فایل حاوی کلمات محاوره‌ای.
-        seperation_flag: اگر `True` باشد و در بخشی از متن به فاصله نیاز بود آن فاصله درج می‌شود.
-        **kargs: پارامترهای نامدارِ اختیاری
-
-    """
-
-    def __init__(
-        self: "InformalNormalizer",
-        verb_file: str = informal_verbs,
-        word_file: str = informal_words,
-        seperation_flag: bool = False,
-        **kargs: str,
-    ) -> None:
-        self.seperation_flag = seperation_flag
-        self.lemmatizer = Lemmatizer()
-        self.ilemmatizer = InformalLemmatizer()
-        self.stemmer = Stemmer()
-        super().__init__(**kargs)
-
-        self.sent_tokenizer = SentenceTokenizer()
-        self.word_tokenizer = WordTokenizer()
-
-        with Path.open(verb_file, encoding="utf8") as vf:
-            self.pastVerbs = {}
-            self.presentVerbs = {}
-            for f, i, _flag in [x.strip().split(" ", 2) for x in vf]:
-                splitedf = f.split("#")
-                self.presentVerbs.update({i: splitedf[1]})
-                self.pastVerbs.update({splitedf[0]: splitedf[0]})
-        with Path.open(default_verbs, encoding="utf8") as vf:
-            for f, i in [x.strip().split("#", 2) for x in vf]:
-                self.presentVerbs.update({i: i})
-                self.pastVerbs.update({f: f})
-
-        def informal_to_formal_conjucation(i, f, flag):
-            iv = self.informal_conjugations(i)
-            fv = self.lemmatizer.conjugation.get_all(f)
-            res = {}
-            if flag:
-                for i, j in zip(iv, fv[48:]):
-                    res[i] = j
-                    if "‌" in i:
-                        res[i.replace("‌", "")] = j
-                        res[i.replace("‌", " ")] = j
-                    if i.endswith("ین"):
-                        res[i[:-1] + "د"] = j
-            else:
-                for i, j in zip(iv[8:], fv[56:]):
-                    res[i] = j
-                    if "‌" in i:
-                        res[i.replace("‌", "")] = j
-                        res[i.replace("‌", " ")] = j
-                    if i.endswith("ین"):
-                        res[i[:-1] + "د"] = j
-
-            return res
-
-        with Path.open(verb_file, encoding="utf8") as vf:
-            self.iverb_map = {}
-            for f, i, flag in [x.strip().split(" ", 2) for x in vf]:
-                self.iverb_map.update(informal_to_formal_conjucation(i, f, flag))
-
-        with Path.open(word_file, encoding="utf8") as wf:
-            self.iword_map = dict([x.strip().split(" ", 1) for x in wf])
-
-        self.words = set()
-        if self.seperation_flag:
-            self.words.update(list(self.iword_map.keys()))
-            self.words.update(list(self.iword_map.values()))
-            self.words.update(list(self.iverb_map.keys()))
-            self.words.update(list(self.iverb_map.values()))
-            self.words.update(self.lemmatizer.words)
-            self.words.update(list(self.lemmatizer.verbs.keys()))
-            self.words.update(list(self.lemmatizer.verbs.values()))
-
-    def split_token_words(self: "InformalNormalizer", token: str) -> str:
-        """هرجایی در متن فاصله نیاز بود قرار می‌دهد.
-
-        متأسفانه در برخی از متن‌ها، به بهانهٔ صرفه‌جویی در زمان یا از سرِ تنبلی،
-        فاصله‌گذاری‌ها درست رعایت نمی‌شود. مثلاً جملهٔ «تو را دوست دارم.» به این
-        شکل نوشته می‌شود: «تورادوست دارم.» این تابع فواصل ضروری را در متن
-        ایجاد می‌کند و آن را به شکل صحیح برمی‌گرداند.
-
-        Args:
-            token: توکنی که باید فاصله‌گذاری شود.
-
-        Returns:
-            توکنی با فاصله‌گذاری صحیح.
-
-        """
-
-        def shekan(token):
-            res = [""]
-            for i in token:
-                res[-1] += i
-                if i in {"ا", "د", "ذ", "ر", "ز", "ژ", "و", *list(NUMBERS)}:
-                    res.append("")
-            while "" in res:
-                res.remove("")
-            return res
-
-        def perm(lst):
-            if len(lst) > 1:
-                up = perm(lst[1:])
-            else:
-                return [lst]
-            res = []
-            for i in up:
-                res.append([lst[0], *i])
-                res.append([lst[0] + i[0]] + i[1:])
-            res.sort(key=len)
-            return res
-
-        token = re.sub(r"(.)\1{2,}", r"\1", token)
-        ps = perm(shekan(token))
-        for c in ps:
-            if {self.ilemmatizer.lemmatize(x) for x in c}.issubset(self.words):
-                return " ".join(c)
-        return token
-
-    def normalized_word(self: "InformalNormalizer", word: str) -> List[str]:
-        """اشکال مختلف نرمالایزشدهٔ کلمه را برمی‌گرداند.
-
-        Examples:
-            >>> normalizer = InformalNormalizer()
-            >>> normalizer.normalized_word('می‌رم')
-            ['می‌روم', 'می‌رم']
-
-        Args:
-            word: کلمه‌ای که باید نرمال‌سازی شود.
-
-        Returns:
-            اشکال نرمالایزشدهٔ کلمه.
-
-        """
-        # >>> normalizer = InformalNormalizer(seperation_flag=True)
-        # >>> normalizer.normalized_word('صداوسیماجمهوری')
-
-        def analyze_word(word):
-            end_words_list = [
-                "هاست",
-                "هایی",
-                "هایم",
-                "ترین",
-                "ایی",
-                "انی",
-                "شان",
-                "شون",
-                "است",
-                "تان",
-                "تون",
-                "مان",
-                "مون",
-                "هام",
-                "هاش",
-                "های",
-                "طور",
-                "ها",
-                "تر",
-                "ئی",
-                "یی",
-                "یم",
-                "ام",
-                "ای",
-                "ان",
-                "هم",
-                "رو",
-                "یت",
-                "ه",
-                "ی",
-                "ش",
-                "و",
-                "ا",
-                "ت",
-                "م",
-            ]
-
-            return_list = []
-
-            collection_of_word_and_suffix = []
-
-            found_early = False
-
-            mid_word_condidate = []
-
-            if word.endswith(("\u200c", "\u200e")):
-                word = word[:-1]
-
-            if word in self.lemmatizer.words or word in self.iword_map:
-                if word in self.lemmatizer.words:
-                    collection_of_word_and_suffix.append({"word": word, "suffix": []})
-                if word in self.iword_map:
-                    collection_of_word_and_suffix.append(
-                        {"word": self.iword_map[word], "suffix": []},
-                    )
-                found_early = True
-
-            if not found_early:
-                for endword in end_words_list:
-                    if word.endswith(endword):
-                        sliceword = word[: -1 * len(endword)]
-                        if (
-                            sliceword in self.lemmatizer.words
-                            or sliceword in self.iword_map
-                        ):
-                            if sliceword in self.lemmatizer.words:
-                                collection_of_word_and_suffix.append(
-                                    {"word": sliceword, "suffix": [endword]},
-                                )
-                            if sliceword in self.iword_map:
-                                collection_of_word_and_suffix.append(
-                                    {
-                                        "word": self.iword_map[sliceword],
-                                        "suffix": [endword],
-                                    },
-                                )
-                        else:
-                            mid_word_condidate.append(sliceword)
-                            mid_word_condidate.append([endword])
-
-                for endword in end_words_list:
-                    for i in range(len(mid_word_condidate) - 1):
-                        if i % 2 == 1:
-                            continue
-                        midword = mid_word_condidate[i]
-                        mid_word_end_word_list = mid_word_condidate[i + 1]
-                        if midword.endswith(endword):
-                            sliceword = midword[: -1 * len(endword)]
-                            if (
-                                sliceword in self.lemmatizer.words
-                                or sliceword in self.iword_map
-                            ):
-                                if sliceword in self.lemmatizer.words:
-                                    collection_of_word_and_suffix.append(
-                                        {
-                                            "word": sliceword,
-                                            "suffix": [
-                                                endword,
-                                                *mid_word_end_word_list,
-                                            ],
-                                        },
-                                    )
-                                if sliceword in self.iword_map:
-                                    collection_of_word_and_suffix.append(
-                                        {
-                                            "word": self.iword_map[sliceword],
-                                            "suffix": [
-                                                endword,
-                                                *mid_word_end_word_list,
-                                            ],
-                                        },
-                                    )
-
-            for i in range(len(collection_of_word_and_suffix)):
-                new_possible_word_list = append_suffix_to_word(
-                    collection_of_word_and_suffix[i],
-                )
-                for j in range(len(new_possible_word_list)):
-                    new_possible_word = new_possible_word_list[j]
-                    if new_possible_word not in return_list:
-                        return_list.append(new_possible_word)
-
-            return return_list
-
-        def analyze_verb_word(word):
-            if word in self.pastVerbs:
-                word = self.pastVerbs[word]
-                return [word]
-
-            if word in self.iword_map:
-                return []
-
-            if word in self.lemmatizer.words:
-                if word[-1] == "ن":
-                    None  # noqa: B018
-                else:
-                    return []
-
-            return_list = []
-
-            collection_of_verb_list = []
-
-            end_verb_list = [
-                "یم",
-                "دم",
-                "دیم",
-                "ید",
-                "دی",
-                "دید",
-                "ند",
-                "دن",
-                "دند",
-                "ین",
-                "دین",
-                "ست",
-                "ستم",
-                "ستی",
-                "ستیم",
-                "ستید",
-                "ستند",
-                "ستن",
-                "م",
-                "ی",
-                "ه",
-                "د",
-                "ن",
-            ]
-
-            for endverb in end_verb_list:
-                if word.endswith(endverb):
-                    if endverb == "ین":
-                        collection_of_verb_list.append(
-                            {"word": word[:-2], "suffix": "ید"},
-                        )
-                    elif endverb == "ستن":
-                        collection_of_verb_list.append(
-                            {"word": word[:-3], "suffix": "ستند"},
-                        )
-                    elif endverb == "ن":
-                        collection_of_verb_list.append(
-                            {"word": word[:-1], "suffix": "ن"},
-                        )
-                        collection_of_verb_list.append(
-                            {"word": word[:-1], "suffix": "ند"},
-                        )
-                    elif endverb == "ه":
-                        if len(word) > 1:
-                            if word[-2] != "د":
-                                collection_of_verb_list.append(
-                                    {"word": word[:-1], "suffix": "د"},
-                                )
-                            collection_of_verb_list.append(
-                                {"word": word[:-1], "suffix": "ه"},
-                            )
-                        else:
-                            collection_of_verb_list.append(
-                                {"word": word[:-1], "suffix": "ه"},
-                            )
-                    else:
-                        collection_of_verb_list.append(
-                            {
-                                "word": word[: -1 * len(endverb)],
-                                "suffix": endverb,
-                            },
-                        )
-            collection_of_verb_list.append({"word": word, "suffix": ""})
-            collection_of_verb_list_2 = []
-            for i in range(len(collection_of_verb_list)):
-                mainword = collection_of_verb_list[i]["word"]
-                collection_of_verb_list[i]["preffix"] = ""
-                if mainword.startswith("بر"):
-                    modified_word = mainword[2:]
-                    new_main_word = ""
-                    if modified_word.startswith("نمی"):
-                        collection_of_verb_list[i]["preffix"] = "برنمی"
-                        new_main_word = modified_word[3:]
-                    elif modified_word.startswith("می"):
-                        collection_of_verb_list[i]["preffix"] = "برمی"
-                        new_main_word = modified_word[2:]
-                    elif modified_word.startswith("ن"):
-                        collection_of_verb_list[i]["preffix"] = "برن"
-                        new_main_word = modified_word[1:]
-                    elif modified_word.startswith("بی"):
-                        collection_of_verb_list[i]["preffix"] = "بربی"
-                        new_main_word = modified_word[2:]
-                    elif modified_word.startswith("ب"):
-                        collection_of_verb_list[i]["preffix"] = "برب"
-                        new_main_word = modified_word[1:]
-                    else:
-                        collection_of_verb_list[i]["preffix"] = "بر"
-                        new_main_word = modified_word
-                        collection_of_verb_list_2.append(
-                            {
-                                "word": mainword,
-                                "preffix": "",
-                                "suffix": collection_of_verb_list[i]["suffix"],
-                            },
-                        )
-
-                    if new_main_word:
-                        collection_of_verb_list[i]["word"] = new_main_word
-                elif mainword.startswith("نمی"):
-                    collection_of_verb_list[i]["preffix"] = "نمی"
-                    collection_of_verb_list[i]["word"] = mainword[3:]
-                elif mainword.startswith("می"):
-                    collection_of_verb_list[i]["preffix"] = "می"
-                    collection_of_verb_list[i]["word"] = mainword[2:]
-                elif mainword.startswith("ن"):
-                    collection_of_verb_list[i]["preffix"] = "ن"
-                    collection_of_verb_list[i]["word"] = mainword[1:]
-                    collection_of_verb_list_2.append(
-                        {
-                            "word": mainword,
-                            "preffix": "",
-                            "suffix": collection_of_verb_list[i]["suffix"],
-                        },
-                    )
-
-                elif mainword.startswith("بی"):
-                    collection_of_verb_list[i]["preffix"] = "بی"
-                    collection_of_verb_list[i]["word"] = mainword[2:]
-                elif mainword.startswith("ب"):
-                    collection_of_verb_list[i]["preffix"] = "ب"
-                    collection_of_verb_list[i]["word"] = mainword[1:]
-                    collection_of_verb_list_2.append(
-                        {
-                            "word": mainword,
-                            "preffix": "",
-                            "suffix": collection_of_verb_list[i]["suffix"],
-                        },
-                    )
-
-            for i in range(len(collection_of_verb_list_2)):
-                collection_of_verb_list.append(collection_of_verb_list_2[i])
-
-            collection_of_real_verb_list = []
-            for i in range(len(collection_of_verb_list)):
-                mainword = collection_of_verb_list[i]["word"]
-                if mainword.startswith(("\u200c", "\u200e")):
-                    mainword = mainword[1:]
-
-                mainword2 = None
-                if mainword.startswith("ا"):
-                    mainword2 = "آ" + mainword[1:]
-                if mainword in self.pastVerbs:
-                    collection_of_verb_list[i]["word"] = self.pastVerbs[mainword]
-                    collection_of_real_verb_list.append(collection_of_verb_list[i])
-                if mainword in self.presentVerbs:
-                    collection_of_verb_list[i]["word"] = self.presentVerbs[mainword]
-                    collection_of_real_verb_list.append(collection_of_verb_list[i])
-                if mainword2 is not None and not (
-                    collection_of_verb_list[i]["preffix"] == "بربی"
-                    or collection_of_verb_list[i]["preffix"] == "بی"
-                ):
-                    if mainword2 in self.pastVerbs:
-                        collection_of_verb_list[i]["word"] = self.pastVerbs[mainword2]
-                        collection_of_real_verb_list.append(collection_of_verb_list[i])
-                    if mainword2 in self.presentVerbs:
-                        collection_of_verb_list[i]["word"] = self.presentVerbs[
-                            mainword2
-                        ]
-                        collection_of_real_verb_list.append(collection_of_verb_list[i])
-
-            for i in range(len(collection_of_real_verb_list)):
-                preffix = collection_of_real_verb_list[i]["preffix"]
-                suffix = collection_of_real_verb_list[i]["suffix"]
-                mainword = collection_of_real_verb_list[i]["word"]
-                returnword = preffix
-                if preffix.endswith("می"):
-                    returnword += "‌"
-                returnword += mainword
-                returnword += suffix
-                if mainword and returnword not in return_list:
-                    return_list.append(returnword)
-
-            return return_list
-
-        def append_suffix_to_word(one_collection_of_word_and_suffix):
-            mainword = one_collection_of_word_and_suffix["word"]
-            suffix_list = one_collection_of_word_and_suffix["suffix"]
-            adhesive_alphabet = {
-                "ب": "ب",
-                "پ": "پ",
-                "ت": "ت",
-                "ث": "ث",
-                "ج": "ج",
-                "چ": "چ",
-                "ح": "ح",
-                "خ": "خ",
-                "س": "س",
-                "ش": "ش",
-                "ص": "ص",
-                "ض": "ض",
-                "ع": "ع",
-                "غ": "غ",
-                "ف": "ف",
-                "ق": "ق",
-                "ک": "ک",
-                "گ": "گ",
-                "ل": "ل",
-                "م": "م",
-                "ن": "ن",
-                "ه": "ه",
-                "ی": "ی",
-            }
-            return_list = []
-            returnword = mainword
-            return_word2 = None
-            return_word3 = None
-            if len(suffix_list) == 0:
-                return [returnword]
-            if len(suffix_list) > 1:
-                if suffix_list[0] == "ه" and suffix_list[1] == "ا":
-                    suffix_list[0] = "ها"
-                    suffix_list.remove(suffix_list[1])
-                if suffix_list[0] == "ه" and suffix_list[1] == "است":
-                    suffix_list[0] = "هاست"
-                    suffix_list.remove(suffix_list[1])
-                if suffix_list[0] == "ت" and suffix_list[1] == "ا":
-                    suffix_list[0] = "تا"
-                    suffix_list.remove(suffix_list[1])
-            for i in range(len(suffix_list)):
-                if suffix_list[i] == "شون":
-                    returnword += "شان"
-                elif suffix_list[i] == "تون":
-                    returnword += "تان"
-                elif suffix_list[i] == "مون":
-                    returnword += "مان"
-                elif suffix_list[i] == "هام":
-                    try:
-                        adhesive_alphabet[returnword[-1]]
-                        returnword += "‌"
-                    except:
-                        None  # noqa: B018
-                    returnword += "هایم"
-                elif suffix_list[i] == "ها":  # noqa: SIM114
-                    try:
-                        adhesive_alphabet[returnword[-1]]
-                        returnword += "‌"
-                    except:
-                        None  # noqa: B018
-                    returnword += "ها"
-                elif (
-                    suffix_list[i] == "ا"
-                    and suffix_list[len(suffix_list) - 1] == "ا"
-                    and not returnword.endswith("ه")
-                ):
-                    try:
-                        adhesive_alphabet[returnword[-1]]
-                        returnword += "‌"
-                    except:
-                        None  # noqa: B018
-                    returnword += "ها"
-                elif suffix_list[i] == "و" and suffix_list[len(suffix_list) - 1] == "و":
-                    return_word2 = returnword
-                    return_word2 += " و"
-                    returnword += " را"
-
-                elif (
-                    suffix_list[i] == "رو" and suffix_list[len(suffix_list) - 1] == "رو"
-                ):
-                    returnword += " را"
-
-                elif suffix_list[i] == "ه" and suffix_list[len(suffix_list) - 1] == "ه":
-                    return_word2 = returnword
-                    return_word2 += "ه"
-                    return_word3 = returnword
-                    return_word3 += " است"
-                    returnword += "ه است"
-                else:
-                    returnword += suffix_list[i]
-            return_list.append(returnword)
-            if return_word2 is not None:
-                return_list.append(return_word2)
-            if return_word3 is not None:
-                return_list.append(return_word3)
-            return return_list
-
-        def straight_forward_result(word):
-            straight_forward_dic = {
-                "ب": ["به"],
-                "ک": ["که"],
-                "آن": ["آن"],
-                "می‌آید": ["می‌آید"],
-                "میاید": ["می‌آید"],
-                "می‌آیم": ["می‌آیم"],
-                "میایم": ["می‌آیم"],
-                "نمی‌آید": ["نمی‌آید"],
-                "نمیاید": ["نمی‌آید"],
-                "نمی‌آیم": ["نمی‌آیم"],
-                "نمیایم": ["نمی‌آیم"],
-                "برمی‌آید": ["برمی‌آید"],
-                "برمیاید": ["برمی‌آید"],
-                "برمی‌آیم": ["برمی‌آیم"],
-                "برمیایم": ["برمی‌آیم"],
-                "برنمی‌آید": ["برنمی‌آید"],
-                "برنمیاید": ["برنمی‌آید"],
-                "برنمی‌آیم": ["برنمی‌آیم"],
-                "برنمیایم": ["برنمی‌آیم"],
-                "منظوره": ["منظوره"],
-                "بدن": ["بدن"],
-                "میا": ["میا"],
-                "نیس": ["نیست"],
-                "فک": ["فکر"],
-                "برام": ["برایم"],
-                "آ": ["آ"],
-                "آی": ["آی"],
-                "این": ["این"],
-                "است": ["است"],
-                "ان": ["ان"],
-                "اند": ["اند"],
-                "میان": ["میان"],
-                "گردن": ["گردن"],
-                "اینهمه": ["اینهمه"],
-                "آنهمه": ["آنهمه"],
-                "الیه": ["الیه"],
-                "غرغره": ["غرغره"],
-                "لیله": ["لیله"],
-                "بزرگانه": ["بزرگانه"],
-                "پرستانه": ["پرستانه"],
-                "ام": ["ام"],
-                "بادی": ["بادی"],
-                "نان": ["نان"],
-                "باورم": ["باورم"],
-                "اوه": ["اوه"],
-                "چقد": ["چقدر"],
-                "چو": ["چون"],
-                "هس": ["هست"],
-                "اومدند": ["آمدند"],
-                "ش": ["اش"],
-                "بش": ["بهش"],
-                "ازت": ["از تو"],
-                "رو": ["را", "رو"],
-                "پایتون": ["پایتون"],
-                "اردن": ["اردن"],
-                "دست": ["دست"],
-                "دستی": ["دستی"],
-                "دستم": ["دستم"],
-                "دین": ["دین"],
-                "شین": ["شین"],
-                "سراتو": ["سراتو"],
-                "فالو": ["فالو"],
-                "هرجا": ["هرجا"],
-                "میدان": ["میدان"],
-                "میدون": ["میدان"],
-                "کفا": ["کفا"],
-                "ویا": ["و یا"],
-                "نشد": ["نشد"],
-                "شو": ["شو"],
-                "مشیا": ["مشیا"],
-                "پلاسما": ["پلاسما"],
-                "فیلیمو": ["فیلیمو"],
-                "پاشو": ["پاشو"],
-                "میر": ["میر"],
-                "بارم": ["بار هم", "بارم"],
-                "برند": ["برند"],
-                "کنه": ["کند"],
-                "بتونه": ["بتواند"],
-                "باشه": ["باشد"],
-                "بخوان": ["بخوان"],
-                "بدم": ["بدم"],
-                "برم": ["برم"],
-                "بده": ["بده"],
-                "نده": ["نده"],
-                "شهرو": ["شهرو"],
-                "شیرو": ["شیرو"],
-                "نگذاشته": ["نگذاشته"],
-                "نگرفته": ["نگرفته"],
-                "نمیشناخته": ["نمی‌شناخته"],
-                "نمی‌شناخته": ["نمی‌شناخته"],
-                "بشین": ["بشین"],
-                "هارو": ["ها را"],
-                "مارو": ["ما را"],
-                "میاومد": ["می‌آمد"],
-                "می‌اومد": ["می‌آمد"],
-                "میخواسته": ["می‌خواسته"],
-                "می‌خواسته": ["می‌خواسته"],
-                "نمیخواسته": ["نمی‌خواسته"],
-                "نمی‌خواسته": ["نمی‌خواسته"],
-                "میتوانسته": ["می‌توانسته"],
-                "می‌توانسته": ["می‌توانسته"],
-                "میرفته": ["می‌رفته"],
-                "می‌رفته": ["می‌رفته"],
-                "نشین": ["نشین"],
-                "انا": ["انا"],
-                "خونی": ["خونی"],
-                "خون": ["خون"],
-                "یالا": ["یالا"],
-                "میخواند": ["می‌خواند"],
-                "می‌خواند": ["می‌خواند"],
-                "نمیخواند": ["نمی‌خواند"],
-                "نمی‌خواند": ["نمی‌خواند"],
-                "میده": ["می‌دهد"],
-                "می‌ده": ["می‌دهد"],
-                "میشه": ["می‌شود"],
-                "می‌شه": ["می‌شود"],
-                "میشد": ["می‌شد"],
-                "می‌شد": ["می‌شد"],
-                "میشدم": ["می‌شدم"],
-                "می‌شدم": ["می‌شدم"],
-                "نمیشد": ["نمی‌شد"],
-                "نمی‌شد": ["نمی‌شد"],
-                "بردم": ["بردم"],
-                "بره": ["بره", "برود"],
-                "شم": ["بشوم"],
-                "اوست": ["اوست"],
-                "بیا": ["بیا"],
-                "نیا": ["نیا"],
-                "میاد": ["می‌آید"],
-                "نشدی": ["نشدی"],
-                "بخواند": ["بخواند"],
-                "سیا": ["سیا"],
-                "میدید": ["می‌دید"],
-                "می‌دید": ["می‌دید"],
-                "وا": ["وا"],
-                "برگشته": ["برگشته"],
-                "میخواست": ["می‌خواست"],
-                "می‌خواست": ["می‌خواست"],
-            }
-            try:
-                return straight_forward_dic[word]
-            except:
-                return []
-
-        straight_forward_words = straight_forward_result(word)
-        if len(straight_forward_words) > 0:
-            return straight_forward_words
-
-        verb_words_list = analyze_verb_word(word)
-        if len(verb_words_list) > 0:
-            return verb_words_list
-        possible_words = analyze_word(word)
-
-        mainword = word
-        if mainword in possible_words:
-            possible_words.remove(mainword)
-            possible_words.append(mainword)
-        elif len(possible_words) == 0:
-            possible_words.append(mainword)
-
-        return possible_words
-
-    def normalize(self: "InformalNormalizer", text: str) -> List[List[List[str]]]:
-        """متن محاوره‌ای را به متن فارسی معیار تبدیل می‌کند.
-
-        Examples:
-            >>> normalizer = InformalNormalizer()
-            >>> normalizer.normalize('بابا یه شغل مناسب واسه بچه هام پیدا کردن که به جایی برنمیخوره !')
-            [[['بابا'], ['یک'], ['شغل'], ['مناسب'], ['برای'], ['بچه'], ['هایم'], ['پیدا'], ['کردن', 'کردند'], ['که'], ['به'], ['جایی'], ['برنمی\u200cخورد', 'برنمی\u200cخوره'], ['!']]]
-            >>> normalizer = InformalNormalizer()
-            >>> normalizer.normalize('اجازه بدیم همسرمون در جمع خانواده‌اش احساس آزادی کنه و فکر نکنه که ما دائم هواسمون بهش هست .')
-            [[['اجازه'], ['بدهیم'], ['همسرمان'], ['در'], ['جمع'], ['خانواده\u200cاش'], ['احساس'], ['آزادی'], ['کند'], ['و'], ['فکر'], ['نکند', 'نکنه'], ['که'], ['ما'], ['دائم'], ['حواسمان'], ['بهش'], ['هست'], ['.']]]
-
-        Args:
-            text: متن محاوره‌ای که باید تبدیل به متن فارسی معیار شود.
-
-        Returns:
-           متن فارسی معیار.
-
-        """
-        text = super().normalize(text)
-        sents = [
-            self.word_tokenizer.tokenize(sentence)
-            for sentence in self.sent_tokenizer.tokenize(text)
-        ]
-
-        return [[self.normalized_word(word) for word in sent] for sent in sents]
-
-    def informal_conjugations(self: "InformalNormalizer", verb: str) -> List[str]:
-        """صورت‌های صرفی فعل را در شکل محاوره‌ای تولید می‌کند.
-
-        Args:
-            verb: فعلی که باید صرف شود.
-
-        Returns:
-            صورت‌های صرفی فعل.
-
-        """
-        ends = ["م", "ی", "", "یم", "ین", "ن"]
-        present_simples = [verb + end for end in ends]
-        if verb.endswith("ا"):
-            present_simples[2] = verb + "د"
-        else:
-            present_simples[2] = verb + "ه"
-        present_not_simples = ["ن" + item for item in present_simples]
-        present_imperfects = ["می‌" + item for item in present_simples]
-        present_not_imperfects = ["ن" + item for item in present_imperfects]
-        present_subjunctives = [
-            item if item.startswith("ب") else "ب" + item for item in present_simples
-        ]
-        present_not_subjunctives = ["ن" + item for item in present_simples]
-        return (
-            present_simples
-            + present_not_simples
-            + present_imperfects
-            + present_not_imperfects
-            + present_subjunctives
-            + present_not_subjunctives
-        )
-
-
-class InformalLemmatizer(Lemmatizer):
-    """این کلاس شامل توابعی برای نرمال‌سازی متن‌های محاوره‌ای است."""
-
-    def __init__(self: "InformalNormalizer", **kargs: str) -> None:
-        """__init__."""
-        super().__init__(**kargs)
-
-        temp = []
-        self.words = set(self.words.keys())
-        for word in self.words:
-            if word.endswith("ً"):
-                temp.append(word[:-1])
-
-        self.words.update(temp)
-
-        temp = {}
-        for verb in self.verbs:
-            if verb.endswith("د"):
-                temp[verb[:-1] + "ن"] = self.verbs[verb]
-
-        self.verbs.update(temp)
-
-        with Path.open(informal_verbs, encoding="utf8") as vf:
-            for f, i, _flag in [x.strip().split(" ", 2) for x in vf]:
-                self.verbs.update({x: f for x in self.iconjugations(i)})
-
-        with Path.open(informal_words, encoding="utf8") as wf:
-            self.words.update([x.strip().split(" ", 1)[0] for x in wf])
-
-    def iconjugations(self: "InformalNormalizer", verb: str):
-        """iconjugations."""
-        ends = ["م", "ی", "", "یم", "ین", "ن"]
-        present_simples = [verb + end for end in ends]
-        if verb.endswith("ا"):
-            present_simples[2] = verb + "د"
-        else:
-            present_simples[2] = verb + "ه"
-        present_not_simples = ["ن" + item for item in present_simples]
-        present_imperfects = ["می‌" + item for item in present_simples]
-        present_not_imperfects = ["ن" + item for item in present_imperfects]
-        present_subjunctives = [
-            item if item.startswith("ب") else "ب" + item for item in present_simples
-        ]
-        present_not_subjunctives = ["ن" + item for item in present_simples]
-        return (
-            present_simples
-            + present_not_simples
-            + present_imperfects
-            + present_not_imperfects
-            + present_subjunctives
-            + present_not_subjunctives
-        )
+"""این ماژول شامل کلاس‌ها و توابعی برای نرمال‌سازی متن‌های محاوره‌ای است."""
+
+
+import re
+from pathlib import Path
+from typing import List
+
+from hazm import Lemmatizer
+from hazm import Normalizer
+from hazm import SentenceTokenizer
+from hazm import Stemmer
+from hazm import NUMBERS
+from hazm import informal_verbs
+from hazm import informal_words
+from hazm import WordTokenizer
+from hazm import default_verbs
+
+
+class InformalNormalizer(Normalizer):
+    """این کلاس شامل توابعی برای نرمال‌سازی متن‌های محاوره‌ای است.
+
+    Args:
+        verb_file: فایل حاوی افعال محاوره‌ای.
+        word_file: فایل حاوی کلمات محاوره‌ای.
+        seperation_flag: اگر `True` باشد و در بخشی از متن به فاصله نیاز بود آن فاصله درج می‌شود.
+        **kargs: پارامترهای نامدارِ اختیاری
+
+    """
+
+    def __init__(
+        self: "InformalNormalizer",
+        verb_file: str = informal_verbs,
+        word_file: str = informal_words,
+        seperation_flag: bool = False,
+        **kargs: str,
+    ) -> None:
+        self.seperation_flag = seperation_flag
+        self.lemmatizer = Lemmatizer()
+        self.ilemmatizer = InformalLemmatizer()
+        self.stemmer = Stemmer()
+        super().__init__(**kargs)
+
+        self.sent_tokenizer = SentenceTokenizer()
+        self.word_tokenizer = WordTokenizer()
+
+        with Path.open(verb_file, encoding="utf8") as vf:
+            self.pastVerbs = {}
+            self.presentVerbs = {}
+            for f, i, _flag in [x.strip().split(" ", 2) for x in vf]:
+                splitedf = f.split("#")
+                self.presentVerbs.update({i: splitedf[1]})
+                self.pastVerbs.update({splitedf[0]: splitedf[0]})
+        with Path.open(default_verbs, encoding="utf8") as vf:
+            for f, i in [x.strip().split("#", 2) for x in vf]:
+                self.presentVerbs.update({i: i})
+                self.pastVerbs.update({f: f})
+
+        def informal_to_formal_conjucation(i, f, flag):
+            iv = self.informal_conjugations(i)
+            fv = self.lemmatizer.conjugation.get_all(f)
+            res = {}
+            if flag:
+                for i, j in zip(iv, fv[48:]):
+                    res[i] = j
+                    if "‌" in i:
+                        res[i.replace("‌", "")] = j
+                        res[i.replace("‌", " ")] = j
+                    if i.endswith("ین"):
+                        res[i[:-1] + "د"] = j
+            else:
+                for i, j in zip(iv[8:], fv[56:]):
+                    res[i] = j
+                    if "‌" in i:
+                        res[i.replace("‌", "")] = j
+                        res[i.replace("‌", " ")] = j
+                    if i.endswith("ین"):
+                        res[i[:-1] + "د"] = j
+
+            return res
+
+        with Path.open(verb_file, encoding="utf8") as vf:
+            self.iverb_map = {}
+            for f, i, flag in [x.strip().split(" ", 2) for x in vf]:
+                self.iverb_map.update(informal_to_formal_conjucation(i, f, flag))
+
+        with Path.open(word_file, encoding="utf8") as wf:
+            self.iword_map = dict([x.strip().split(" ", 1) for x in wf])
+
+        self.words = set()
+        if self.seperation_flag:
+            self.words.update(list(self.iword_map.keys()))
+            self.words.update(list(self.iword_map.values()))
+            self.words.update(list(self.iverb_map.keys()))
+            self.words.update(list(self.iverb_map.values()))
+            self.words.update(self.lemmatizer.words)
+            self.words.update(list(self.lemmatizer.verbs.keys()))
+            self.words.update(list(self.lemmatizer.verbs.values()))
+
+    def split_token_words(self: "InformalNormalizer", token: str) -> str:
+        """هرجایی در متن فاصله نیاز بود قرار می‌دهد.
+
+        متأسفانه در برخی از متن‌ها، به بهانهٔ صرفه‌جویی در زمان یا از سرِ تنبلی،
+        فاصله‌گذاری‌ها درست رعایت نمی‌شود. مثلاً جملهٔ «تو را دوست دارم.» به این
+        شکل نوشته می‌شود: «تورادوست دارم.» این تابع فواصل ضروری را در متن
+        ایجاد می‌کند و آن را به شکل صحیح برمی‌گرداند.
+
+        Args:
+            token: توکنی که باید فاصله‌گذاری شود.
+
+        Returns:
+            توکنی با فاصله‌گذاری صحیح.
+
+        """
+
+        def shekan(token):
+            res = [""]
+            for i in token:
+                res[-1] += i
+                if i in {"ا", "د", "ذ", "ر", "ز", "ژ", "و", *list(NUMBERS)}:
+                    res.append("")
+            while "" in res:
+                res.remove("")
+            return res
+
+        def perm(lst):
+            if len(lst) > 1:
+                up = perm(lst[1:])
+            else:
+                return [lst]
+            res = []
+            for i in up:
+                res.append([lst[0], *i])
+                res.append([lst[0] + i[0]] + i[1:])
+            res.sort(key=len)
+            return res
+
+        token = re.sub(r"(.)\1{2,}", r"\1", token)
+        ps = perm(shekan(token))
+        for c in ps:
+            if {self.ilemmatizer.lemmatize(x) for x in c}.issubset(self.words):
+                return " ".join(c)
+        return token
+
+    def normalized_word(self: "InformalNormalizer", word: str) -> List[str]:
+        """اشکال مختلف نرمالایزشدهٔ کلمه را برمی‌گرداند.
+
+        Examples:
+            >>> normalizer = InformalNormalizer()
+            >>> normalizer.normalized_word('می‌رم')
+            ['می‌روم']
+
+        Args:
+            word: کلمه‌ای که باید نرمال‌سازی شود.
+
+        Returns:
+            اشکال نرمالایزشدهٔ کلمه.
+
+        """
+        # >>> normalizer = InformalNormalizer(seperation_flag=True)
+        # >>> normalizer.normalized_word('صداوسیماجمهوری')
+
+        def analyze_word(word):
+            end_words_list = [
+                "هاست",
+                "هایی",
+                "هایم",
+                "ترین",
+                "ایی",
+                "انی",
+                "شان",
+                "شون",
+                "است",
+                "تان",
+                "تون",
+                "مان",
+                "مون",
+                "هام",
+                "هاش",
+                "های",
+                "طور",
+                "ها",
+                "تر",
+                "ئی",
+                "یی",
+                "یم",
+                "ام",
+                "ای",
+                "ان",
+                "هم",
+                "رو",
+                "یت",
+                "ه",
+                "ی",
+                "ش",
+                "و",
+                "ا",
+                "ت",
+                "م",
+            ]
+
+            return_list = []
+
+            collection_of_word_and_suffix = []
+
+            found_early = False
+
+            mid_word_condidate = []
+
+            if word.endswith(("\u200c", "\u200e")):
+                word = word[:-1]
+
+            if word in self.lemmatizer.words or word in self.iword_map:
+                if word in self.lemmatizer.words:
+                    collection_of_word_and_suffix.append({"word": word, "suffix": []})
+                if word in self.iword_map:
+                    collection_of_word_and_suffix.append(
+                        {"word": self.iword_map[word], "suffix": []},
+                    )
+                found_early = True
+
+            if not found_early:
+                for endword in end_words_list:
+                    if word.endswith(endword):
+                        sliceword = word[: -1 * len(endword)]
+                        if (
+                            sliceword in self.lemmatizer.words
+                            or sliceword in self.iword_map
+                        ):
+                            if sliceword in self.lemmatizer.words:
+                                collection_of_word_and_suffix.append(
+                                    {"word": sliceword, "suffix": [endword]},
+                                )
+                            if sliceword in self.iword_map:
+                                collection_of_word_and_suffix.append(
+                                    {
+                                        "word": self.iword_map[sliceword],
+                                        "suffix": [endword],
+                                    },
+                                )
+                        else:
+                            mid_word_condidate.append(sliceword)
+                            mid_word_condidate.append([endword])
+
+                for endword in end_words_list:
+                    for i in range(len(mid_word_condidate) - 1):
+                        if i % 2 == 1:
+                            continue
+                        midword = mid_word_condidate[i]
+                        mid_word_end_word_list = mid_word_condidate[i + 1]
+                        if midword.endswith(endword):
+                            sliceword = midword[: -1 * len(endword)]
+                            if (
+                                sliceword in self.lemmatizer.words
+                                or sliceword in self.iword_map
+                            ):
+                                if sliceword in self.lemmatizer.words:
+                                    collection_of_word_and_suffix.append(
+                                        {
+                                            "word": sliceword,
+                                            "suffix": [
+                                                endword,
+                                                *mid_word_end_word_list,
+                                            ],
+                                        },
+                                    )
+                                if sliceword in self.iword_map:
+                                    collection_of_word_and_suffix.append(
+                                        {
+                                            "word": self.iword_map[sliceword],
+                                            "suffix": [
+                                                endword,
+                                                *mid_word_end_word_list,
+                                            ],
+                                        },
+                                    )
+
+            for i in range(len(collection_of_word_and_suffix)):
+                new_possible_word_list = append_suffix_to_word(
+                    collection_of_word_and_suffix[i],
+                )
+                for j in range(len(new_possible_word_list)):
+                    new_possible_word = new_possible_word_list[j]
+                    if new_possible_word not in return_list:
+                        return_list.append(new_possible_word)
+
+            return return_list
+
+        def analyze_verb_word(word):
+            if word in self.pastVerbs:
+                word = self.pastVerbs[word]
+                return [word]
+
+            if word in self.iword_map:
+                return []
+
+            if word in self.lemmatizer.words:
+                if word[-1] == "ن":
+                    None  # noqa: B018
+                else:
+                    return []
+
+            return_list = []
+
+            collection_of_verb_list = []
+
+            end_verb_list = [
+                "یم",
+                "دم",
+                "دیم",
+                "ید",
+                "دی",
+                "دید",
+                "ند",
+                "دن",
+                "دند",
+                "ین",
+                "دین",
+                "ست",
+                "ستم",
+                "ستی",
+                "ستیم",
+                "ستید",
+                "ستند",
+                "ستن",
+                "م",
+                "ی",
+                "ه",
+                "د",
+                "ن",
+            ]
+
+            for endverb in end_verb_list:
+                if word.endswith(endverb):
+                    if endverb == "ین":
+                        collection_of_verb_list.append(
+                            {"word": word[:-2], "suffix": "ید"},
+                        )
+                    elif endverb == "ستن":
+                        collection_of_verb_list.append(
+                            {"word": word[:-3], "suffix": "ستند"},
+                        )
+                    elif endverb == "ن":
+                        collection_of_verb_list.append(
+                            {"word": word[:-1], "suffix": "ن"},
+                        )
+                        collection_of_verb_list.append(
+                            {"word": word[:-1], "suffix": "ند"},
+                        )
+                    elif endverb == "ه":
+                        if len(word) > 1:
+                            if word[-2] != "د":
+                                collection_of_verb_list.append(
+                                    {"word": word[:-1], "suffix": "د"},
+                                )
+                            collection_of_verb_list.append(
+                                {"word": word[:-1], "suffix": "ه"},
+                            )
+                        else:
+                            collection_of_verb_list.append(
+                                {"word": word[:-1], "suffix": "ه"},
+                            )
+                    else:
+                        collection_of_verb_list.append(
+                            {
+                                "word": word[: -1 * len(endverb)],
+                                "suffix": endverb,
+                            },
+                        )
+            collection_of_verb_list.append({"word": word, "suffix": ""})
+            collection_of_verb_list_2 = []
+            for i in range(len(collection_of_verb_list)):
+                mainword = collection_of_verb_list[i]["word"]
+                collection_of_verb_list[i]["preffix"] = ""
+                if mainword.startswith("بر"):
+                    modified_word = mainword[2:]
+                    new_main_word = ""
+                    if modified_word.startswith("نمی"):
+                        collection_of_verb_list[i]["preffix"] = "برنمی"
+                        new_main_word = modified_word[3:]
+                    elif modified_word.startswith("می"):
+                        collection_of_verb_list[i]["preffix"] = "برمی"
+                        new_main_word = modified_word[2:]
+                    elif modified_word.startswith("ن"):
+                        collection_of_verb_list[i]["preffix"] = "برن"
+                        new_main_word = modified_word[1:]
+                    elif modified_word.startswith("بی"):
+                        collection_of_verb_list[i]["preffix"] = "بربی"
+                        new_main_word = modified_word[2:]
+                    elif modified_word.startswith("ب"):
+                        collection_of_verb_list[i]["preffix"] = "برب"
+                        new_main_word = modified_word[1:]
+                    else:
+                        collection_of_verb_list[i]["preffix"] = "بر"
+                        new_main_word = modified_word
+                        collection_of_verb_list_2.append(
+                            {
+                                "word": mainword,
+                                "preffix": "",
+                                "suffix": collection_of_verb_list[i]["suffix"],
+                            },
+                        )
+
+                    if new_main_word:
+                        collection_of_verb_list[i]["word"] = new_main_word
+                elif mainword.startswith("نمی"):
+                    collection_of_verb_list[i]["preffix"] = "نمی"
+                    collection_of_verb_list[i]["word"] = mainword[3:]
+                elif mainword.startswith("می"):
+                    collection_of_verb_list[i]["preffix"] = "می"
+                    collection_of_verb_list[i]["word"] = mainword[2:]
+                elif mainword.startswith("ن"):
+                    collection_of_verb_list[i]["preffix"] = "ن"
+                    collection_of_verb_list[i]["word"] = mainword[1:]
+                    collection_of_verb_list_2.append(
+                        {
+                            "word": mainword,
+                            "preffix": "",
+                            "suffix": collection_of_verb_list[i]["suffix"],
+                        },
+                    )
+
+                elif mainword.startswith("بی"):
+                    collection_of_verb_list[i]["preffix"] = "بی"
+                    collection_of_verb_list[i]["word"] = mainword[2:]
+                elif mainword.startswith("ب"):
+                    collection_of_verb_list[i]["preffix"] = "ب"
+                    collection_of_verb_list[i]["word"] = mainword[1:]
+                    collection_of_verb_list_2.append(
+                        {
+                            "word": mainword,
+                            "preffix": "",
+                            "suffix": collection_of_verb_list[i]["suffix"],
+                        },
+                    )
+
+            for i in range(len(collection_of_verb_list_2)):
+                collection_of_verb_list.append(collection_of_verb_list_2[i])
+
+            collection_of_real_verb_list = []
+            for i in range(len(collection_of_verb_list)):
+                mainword = collection_of_verb_list[i]["word"]
+                if mainword.startswith(("\u200c", "\u200e")):
+                    mainword = mainword[1:]
+
+                mainword2 = None
+                if mainword.startswith("ا"):
+                    mainword2 = "آ" + mainword[1:]
+                if mainword in self.pastVerbs:
+                    collection_of_verb_list[i]["word"] = self.pastVerbs[mainword]
+                    collection_of_real_verb_list.append(collection_of_verb_list[i])
+                if mainword in self.presentVerbs:
+                    collection_of_verb_list[i]["word"] = self.presentVerbs[mainword]
+                    collection_of_real_verb_list.append(collection_of_verb_list[i])
+                if mainword2 is not None and not (
+                    collection_of_verb_list[i]["preffix"] == "بربی"
+                    or collection_of_verb_list[i]["preffix"] == "بی"
+                ):
+                    if mainword2 in self.pastVerbs:
+                        collection_of_verb_list[i]["word"] = self.pastVerbs[mainword2]
+                        collection_of_real_verb_list.append(collection_of_verb_list[i])
+                    if mainword2 in self.presentVerbs:
+                        collection_of_verb_list[i]["word"] = self.presentVerbs[
+                            mainword2
+                        ]
+                        collection_of_real_verb_list.append(collection_of_verb_list[i])
+
+            for i in range(len(collection_of_real_verb_list)):
+                preffix = collection_of_real_verb_list[i]["preffix"]
+                suffix = collection_of_real_verb_list[i]["suffix"]
+                mainword = collection_of_real_verb_list[i]["word"]
+                returnword = preffix
+                if preffix.endswith("می"):
+                    returnword += "‌"
+                returnword += mainword
+                returnword += suffix
+                if mainword and returnword not in return_list:
+                    return_list.append(returnword)
+
+            return return_list
+
+        def append_suffix_to_word(one_collection_of_word_and_suffix):
+            mainword = one_collection_of_word_and_suffix["word"]
+            suffix_list = one_collection_of_word_and_suffix["suffix"]
+            adhesive_alphabet = {
+                "ب": "ب",
+                "پ": "پ",
+                "ت": "ت",
+                "ث": "ث",
+                "ج": "ج",
+                "چ": "چ",
+                "ح": "ح",
+                "خ": "خ",
+                "س": "س",
+                "ش": "ش",
+                "ص": "ص",
+                "ض": "ض",
+                "ع": "ع",
+                "غ": "غ",
+                "ف": "ف",
+                "ق": "ق",
+                "ک": "ک",
+                "گ": "گ",
+                "ل": "ل",
+                "م": "م",
+                "ن": "ن",
+                "ه": "ه",
+                "ی": "ی",
+            }
+            return_list = []
+            returnword = mainword
+            return_word2 = None
+            return_word3 = None
+            if len(suffix_list) == 0:
+                return [returnword]
+            if len(suffix_list) > 1:
+                if suffix_list[0] == "ه" and suffix_list[1] == "ا":
+                    suffix_list[0] = "ها"
+                    suffix_list.remove(suffix_list[1])
+                if suffix_list[0] == "ه" and suffix_list[1] == "است":
+                    suffix_list[0] = "هاست"
+                    suffix_list.remove(suffix_list[1])
+                if suffix_list[0] == "ت" and suffix_list[1] == "ا":
+                    suffix_list[0] = "تا"
+                    suffix_list.remove(suffix_list[1])
+            for i in range(len(suffix_list)):
+                if suffix_list[i] == "شون":
+                    returnword += "شان"
+                elif suffix_list[i] == "تون":
+                    returnword += "تان"
+                elif suffix_list[i] == "مون":
+                    returnword += "مان"
+                elif suffix_list[i] == "هام":
+                    try:
+                        adhesive_alphabet[returnword[-1]]
+                        returnword += "‌"
+                    except:
+                        None  # noqa: B018
+                    returnword += "هایم"
+                elif suffix_list[i] == "ها":  # noqa: SIM114
+                    try:
+                        adhesive_alphabet[returnword[-1]]
+                        returnword += "‌"
+                    except:
+                        None  # noqa: B018
+                    returnword += "ها"
+                elif (
+                    suffix_list[i] == "ا"
+                    and suffix_list[len(suffix_list) - 1] == "ا"
+                    and not returnword.endswith("ه")
+                ):
+                    try:
+                        adhesive_alphabet[returnword[-1]]
+                        returnword += "‌"
+                    except:
+                        None  # noqa: B018
+                    returnword += "ها"
+                elif suffix_list[i] == "و" and suffix_list[len(suffix_list) - 1] == "و":
+                    return_word2 = returnword
+                    return_word2 += " و"
+                    returnword += " را"
+
+                elif (
+                    suffix_list[i] == "رو" and suffix_list[len(suffix_list) - 1] == "رو"
+                ):
+                    returnword += " را"
+
+                elif suffix_list[i] == "ه" and suffix_list[len(suffix_list) - 1] == "ه":
+                    return_word2 = returnword
+                    return_word2 += "ه"
+                    return_word3 = returnword
+                    return_word3 += " است"
+                    returnword += "ه است"
+                else:
+                    returnword += suffix_list[i]
+            return_list.append(returnword)
+            if return_word2 is not None:
+                return_list.append(return_word2)
+            if return_word3 is not None:
+                return_list.append(return_word3)
+            return return_list
+
+        def straight_forward_result(word):
+            straight_forward_dic = {
+                "ب": ["به"],
+                "ک": ["که"],
+                "آن": ["آن"],
+                "می‌آید": ["می‌آید"],
+                "میاید": ["می‌آید"],
+                "می‌آیم": ["می‌آیم"],
+                "میایم": ["می‌آیم"],
+                "نمی‌آید": ["نمی‌آید"],
+                "نمیاید": ["نمی‌آید"],
+                "نمی‌آیم": ["نمی‌آیم"],
+                "نمیایم": ["نمی‌آیم"],
+                "برمی‌آید": ["برمی‌آید"],
+                "برمیاید": ["برمی‌آید"],
+                "برمی‌آیم": ["برمی‌آیم"],
+                "برمیایم": ["برمی‌آیم"],
+                "برنمی‌آید": ["برنمی‌آید"],
+                "برنمیاید": ["برنمی‌آید"],
+                "برنمی‌آیم": ["برنمی‌آیم"],
+                "برنمیایم": ["برنمی‌آیم"],
+                "منظوره": ["منظوره"],
+                "بدن": ["بدن"],
+                "میا": ["میا"],
+                "نیس": ["نیست"],
+                "فک": ["فکر"],
+                "برام": ["برایم"],
+                "آ": ["آ"],
+                "آی": ["آی"],
+                "این": ["این"],
+                "است": ["است"],
+                "ان": ["ان"],
+                "اند": ["اند"],
+                "میان": ["میان"],
+                "گردن": ["گردن"],
+                "اینهمه": ["اینهمه"],
+                "آنهمه": ["آنهمه"],
+                "الیه": ["الیه"],
+                "غرغره": ["غرغره"],
+                "لیله": ["لیله"],
+                "بزرگانه": ["بزرگانه"],
+                "پرستانه": ["پرستانه"],
+                "ام": ["ام"],
+                "بادی": ["بادی"],
+                "نان": ["نان"],
+                "باورم": ["باورم"],
+                "اوه": ["اوه"],
+                "چقد": ["چقدر"],
+                "چو": ["چون"],
+                "هس": ["هست"],
+                "اومدند": ["آمدند"],
+                "ش": ["اش"],
+                "بش": ["بهش"],
+                "ازت": ["از تو"],
+                "رو": ["را", "رو"],
+                "پایتون": ["پایتون"],
+                "اردن": ["اردن"],
+                "دست": ["دست"],
+                "دستی": ["دستی"],
+                "دستم": ["دستم"],
+                "دین": ["دین"],
+                "شین": ["شین"],
+                "سراتو": ["سراتو"],
+                "فالو": ["فالو"],
+                "هرجا": ["هرجا"],
+                "میدان": ["میدان"],
+                "میدون": ["میدان"],
+                "کفا": ["کفا"],
+                "ویا": ["و یا"],
+                "نشد": ["نشد"],
+                "شو": ["شو"],
+                "مشیا": ["مشیا"],
+                "پلاسما": ["پلاسما"],
+                "فیلیمو": ["فیلیمو"],
+                "پاشو": ["پاشو"],
+                "میر": ["میر"],
+                "بارم": ["بار هم", "بارم"],
+                "برند": ["برند"],
+                "کنه": ["کند"],
+                "بتونه": ["بتواند"],
+                "باشه": ["باشد"],
+                "بخوان": ["بخوان"],
+                "بدم": ["بدم"],
+                "برم": ["برم"],
+                "بده": ["بده"],
+                "نده": ["نده"],
+                "شهرو": ["شهرو"],
+                "شیرو": ["شیرو"],
+                "نگذاشته": ["نگذاشته"],
+                "نگرفته": ["نگرفته"],
+                "نمیشناخته": ["نمی‌شناخته"],
+                "نمی‌شناخته": ["نمی‌شناخته"],
+                "بشین": ["بشین"],
+                "هارو": ["ها را"],
+                "مارو": ["ما را"],
+                "میاومد": ["می‌آمد"],
+                "می‌اومد": ["می‌آمد"],
+                "میخواسته": ["می‌خواسته"],
+                "می‌خواسته": ["می‌خواسته"],
+                "نمیخواسته": ["نمی‌خواسته"],
+                "نمی‌خواسته": ["نمی‌خواسته"],
+                "میتوانسته": ["می‌توانسته"],
+                "می‌توانسته": ["می‌توانسته"],
+                "میرفته": ["می‌رفته"],
+                "می‌رفته": ["می‌رفته"],
+                "نشین": ["نشین"],
+                "انا": ["انا"],
+                "خونی": ["خونی"],
+                "خون": ["خون"],
+                "یالا": ["یالا"],
+                "میخواند": ["می‌خواند"],
+                "می‌خواند": ["می‌خواند"],
+                "نمیخواند": ["نمی‌خواند"],
+                "نمی‌خواند": ["نمی‌خواند"],
+                "میده": ["می‌دهد"],
+                "می‌ده": ["می‌دهد"],
+                "میشه": ["می‌شود"],
+                "می‌شه": ["می‌شود"],
+                "میشد": ["می‌شد"],
+                "می‌شد": ["می‌شد"],
+                "میشدم": ["می‌شدم"],
+                "می‌شدم": ["می‌شدم"],
+                "نمیشد": ["نمی‌شد"],
+                "نمی‌شد": ["نمی‌شد"],
+                "بردم": ["بردم"],
+                "بره": ["بره", "برود"],
+                "شم": ["بشوم"],
+                "اوست": ["اوست"],
+                "بیا": ["بیا"],
+                "نیا": ["نیا"],
+                "میاد": ["می‌آید"],
+                "نشدی": ["نشدی"],
+                "بخواند": ["بخواند"],
+                "سیا": ["سیا"],
+                "میدید": ["می‌دید"],
+                "می‌دید": ["می‌دید"],
+                "وا": ["وا"],
+                "برگشته": ["برگشته"],
+                "میخواست": ["می‌خواست"],
+                "می‌خواست": ["می‌خواست"],
+            }
+            try:
+                return straight_forward_dic[word]
+            except:
+                return []
+
+        straight_forward_words = straight_forward_result(word)
+        if len(straight_forward_words) > 0:
+            return straight_forward_words
+
+        verb_words_list = analyze_verb_word(word)
+        if len(verb_words_list) > 0:
+            return verb_words_list
+        possible_words = analyze_word(word)
+
+        mainword = word
+        if mainword in possible_words:
+            possible_words.remove(mainword)
+            possible_words.append(mainword)
+        elif len(possible_words) == 0:
+            possible_words.append(mainword)
+
+        return possible_words
+
+    def normalize(self: "InformalNormalizer", text: str) -> List[List[List[str]]]:
+        """متن محاوره‌ای را به متن فارسی معیار تبدیل می‌کند.
+
+        Examples:
+            >>> normalizer = InformalNormalizer()
+            >>> normalizer.normalize('بابا یه شغل مناسب واسه بچه هام پیدا کردن که به جایی برنمیخوره !')
+            [[['بابا'], ['یک'], ['شغل'], ['مناسب'], ['برای'], ['بچه'], ['هایم'], ['پیدا'], ['کردن', 'کردند'], ['که'], ['به'], ['جایی'], ['برنمی\u200cخورد', 'برنمی\u200cخوره'], ['!']]]
+            >>> normalizer = InformalNormalizer()
+            >>> normalizer.normalize('اجازه بدیم همسرمون در جمع خانواده‌اش احساس آزادی کنه و فکر نکنه که ما دائم هواسمون بهش هست .')
+            [[['اجازه'], ['بدهیم'], ['همسرمان'], ['در'], ['جمع'], ['خانواده\u200cاش'], ['احساس'], ['آزادی'], ['کند'], ['و'], ['فکر'], ['نکند', 'نکنه'], ['که'], ['ما'], ['دائم'], ['حواسمان'], ['بهش'], ['هست'], ['.']]]
+
+        Args:
+            text: متن محاوره‌ای که باید تبدیل به متن فارسی معیار شود.
+
+        Returns:
+           متن فارسی معیار.
+
+        """
+        text = super().normalize(text)
+        sents = [
+            self.word_tokenizer.tokenize(sentence)
+            for sentence in self.sent_tokenizer.tokenize(text)
+        ]
+
+        return [[self.normalized_word(word) for word in sent] for sent in sents]
+
+    def informal_conjugations(self: "InformalNormalizer", verb: str) -> List[str]:
+        """صورت‌های صرفی فعل را در شکل محاوره‌ای تولید می‌کند.
+
+        Args:
+            verb: فعلی که باید صرف شود.
+
+        Returns:
+            صورت‌های صرفی فعل.
+
+        """
+        ends = ["م", "ی", "", "یم", "ین", "ن"]
+        present_simples = [verb + end for end in ends]
+        if verb.endswith("ا"):
+            present_simples[2] = verb + "د"
+        else:
+            present_simples[2] = verb + "ه"
+        present_not_simples = ["ن" + item for item in present_simples]
+        present_imperfects = ["می‌" + item for item in present_simples]
+        present_not_imperfects = ["ن" + item for item in present_imperfects]
+        present_subjunctives = [
+            item if item.startswith("ب") else "ب" + item for item in present_simples
+        ]
+        present_not_subjunctives = ["ن" + item for item in present_simples]
+        return (
+            present_simples
+            + present_not_simples
+            + present_imperfects
+            + present_not_imperfects
+            + present_subjunctives
+            + present_not_subjunctives
+        )
+
+
+class InformalLemmatizer(Lemmatizer):
+    """این کلاس شامل توابعی برای نرمال‌سازی متن‌های محاوره‌ای است."""
+
+    def __init__(self: "InformalNormalizer", **kargs: str) -> None:
+        """__init__."""
+        super().__init__(**kargs)
+
+        temp = []
+        self.words = set(self.words.keys())
+        for word in self.words:
+            if word.endswith("ً"):
+                temp.append(word[:-1])
+
+        self.words.update(temp)
+
+        temp = {}
+        for verb in self.verbs:
+            if verb.endswith("د"):
+                temp[verb[:-1] + "ن"] = self.verbs[verb]
+
+        self.verbs.update(temp)
+
+        with Path.open(informal_verbs, encoding="utf8") as vf:
+            for f, i, _flag in [x.strip().split(" ", 2) for x in vf]:
+                self.verbs.update({x: f for x in self.iconjugations(i)})
+
+        with Path.open(informal_words, encoding="utf8") as wf:
+            self.words.update([x.strip().split(" ", 1)[0] for x in wf])
+
+    def iconjugations(self: "InformalNormalizer", verb: str):
+        """iconjugations."""
+        ends = ["م", "ی", "", "یم", "ین", "ن"]
+        present_simples = [verb + end for end in ends]
+        if verb.endswith("ا"):
+            present_simples[2] = verb + "د"
+        else:
+            present_simples[2] = verb + "ه"
+        present_not_simples = ["ن" + item for item in present_simples]
+        present_imperfects = ["می‌" + item for item in present_simples]
+        present_not_imperfects = ["ن" + item for item in present_imperfects]
+        present_subjunctives = [
+            item if item.startswith("ب") else "ب" + item for item in present_simples
+        ]
+        present_not_subjunctives = ["ن" + item for item in present_simples]
+        return (
+            present_simples
+            + present_not_simples
+            + present_imperfects
+            + present_not_imperfects
+            + present_subjunctives
+            + present_not_subjunctives
+        )
```

### Comparing `hazm-0.9.0/hazm/lemmatizer.py` & `hazm-0.9.1/hazm/lemmatizer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,2322 +1,2322 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای ریشه‌یابی کلمات است.
-
-فرق بین [Lemmatizer](./lemmatizer.md) و [Stemmer](./stemmer.md) این است که
-اِستمر درکی از معنای کلمه ندارد و صرفاً براساس حذف برخی از پسوندهای ساده تلاش
-می‌کند ریشهٔ کلمه را بیابد؛ بنابراین ممکن است در ریشه‌یابیِ برخی از کلمات نتایج
-نادرستی ارائه دهد؛ اما لماتایزر براساس لیستی از کلمات مرجع به همراه ریشهٔ آن
-این
-کار را انجام می‌دهد و نتایج دقیق‌تری ارائه می‌دهد. البته هزینهٔ این دقت، سرعتِ
-کمتر در ریشه‌یابی است.
-
-**میزان دقت
-لماتایزر در نسخهٔ حاضر ۸۹.۹ درصد [^1] است.**
-[^1]:
-این عدد با انتشار هر نسخه بروزرسانی می‌شود
-
-"""
-
-
-from typing import List
-
-from hazm import Stemmer
-from hazm import default_verbs
-from hazm import default_words
-from hazm import WordTokenizer
-
-
-class Lemmatizer:
-    """این کلاس شامل توابعی برای ریشه‌یابی کلمات است.
-
-    Args:
-        words_file: ریشه‌یابی کلمات از روی این فایل صورت
-            می‌گیرد. هضم به صورت پیش‌فرض فایلی برای این منظور در نظر گرفته است؛ با
-            این حال شما می‌توانید فایل موردنظر خود را معرفی کنید. برای آگاهی از
-            ساختار این فایل به فایل پیش‌فرض مراجعه کنید.
-        verbs_file: اشکال صرفی فعل از روی این فایل ساخته
-            می‌شود. هضم به صورت پیش‌فرض فایلی برای این منظور در نظر گرفته است؛ با
-            این حال شما می‌توانید فایل موردنظر خود را معرفی کنید. برای آگاهی از
-            ساختار این فایل به فایل پیش‌فرض مراجعه کنید.
-        joined_verb_parts: اگر `True` باشد افعال چندبخشی را با کاراکتر زیرخط به هم می‌چسباند.
-
-    """
-
-    def __init__(
-        self: "Lemmatizer",
-        words_file: str = default_words,
-        verbs_file: str = default_verbs,
-        joined_verb_parts: bool = True,
-    ) -> None:
-        self.words_file = words_file
-        self.verbs = {}
-        self.stemmer = Stemmer()
-        self.conjugation = Conjugation()
-
-        tokenizer = WordTokenizer(words_file=default_words, verbs_file=verbs_file)
-        self.words = tokenizer.words
-
-        if verbs_file:
-            self.verbs["است"] = "#است"
-            for verb in tokenizer.verbs:
-                for tense in self.conjugation.get_all(verb):
-                    self.verbs[tense] = verb
-            if joined_verb_parts:
-                for verb in tokenizer.verbs:
-                    bon = verb.split("#")[0]
-                    for after_verb in tokenizer.after_verbs:
-                        self.verbs[bon + "ه_" + after_verb] = verb
-                        self.verbs["ن" + bon + "ه_" + after_verb] = verb
-                    for before_verb in tokenizer.before_verbs:
-                        self.verbs[before_verb + "_" + bon] = verb
-
-    def lemmatize(self: "Lemmatizer", word: str, pos: str = "") -> str:
-        """ریشهٔ کلمه را پیدا می‌کند.
-
-        پارامتر `pos` نوع کلمه است: (اسم، فعل، صفت و ...) و به این خاطر لازم
-        است که می‌تواند روی ریشه‌یابی کلمات اثر بگذارد؛ مثلاً واژهٔ «اجتماعی» در
-        جایگاه صفت (او یک فرد اجتماعی است)، ریشه‌اش همان «اجتماعی» می‌شود ولی
-        همین واژه در جایگاه اسم (اجتماعی از مردم)، ریشه‌اش می‌شود «اجتماع».
-
-        Examples:
-            >>> lemmatizer = Lemmatizer()
-            >>> lemmatizer.lemmatize('کتاب‌ها')
-            'کتاب'
-            >>> lemmatizer.lemmatize('آتشفشان')
-            'آتشفشان'
-            >>> lemmatizer.lemmatize('می‌روم')
-            'رفت#رو'
-            >>> lemmatizer.lemmatize('گفته_شده_است')
-            'گفت#گو'
-            >>> lemmatizer.lemmatize('نچشیده_است')
-            'چشید#چش'
-            >>> lemmatizer.lemmatize('مردم', pos='N')
-            'مردم'
-            >>> lemmatizer.lemmatize('اجتماعی', pos='AJ')
-            'اجتماعی'
-
-        Args:
-            word: کلمه‌ای که باید پردازش شود.
-            pos: نوع کلمه. این پارامتر سه مقدار `V` (فعل) و `AJ` (صفت) و `PRO` (ضمیر) را می‌پذیرد.
-
-        Returns:
-            ریشهٔ کلمه
-
-        """
-        if not pos and word in self.words:
-            return word
-
-        if (not pos or pos == "V") and word in self.verbs:
-            return self.verbs[word]
-
-        if pos.startswith("AJ") and word[-1] == "ی":
-            return word
-
-        if pos == "PRO":
-            return word
-
-        if word in self.words:
-            return word
-
-        stem = self.stemmer.stem(word)
-        if stem and stem in self.words:
-            return stem
-
-        return word
-
-
-class Conjugation:
-    """این کلاس دارای توابعی برای صرف‌کردن افعال است."""
-
-    def perfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ مطلق صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.perfective_past('دید')
-            ['دیدم', 'دیدی', 'دید', 'دیدیم', 'دیدید', 'دیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-            صورت‌های صرفی فعل در زمان گذشتهٔ مطلق.
-        """
-        return [ri + x for x in ["م", "ی", "", "یم", "ید", "ند"]]
-
-    def negative_perfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ مطلق به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_perfective_past('دید')
-            ['ندیدم', 'ندیدی', 'ندید', 'ندیدیم', 'ندیدید', 'ندیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.perfective_past(ri)]
-
-    def passive_perfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ مطلق در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_perfective_past('دید')
-            ['دیده شدم', 'دیده شدی', 'دیده شد', 'دیده شدیم', 'دیده شدید', 'دیده شدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.perfective_past("شد")]
-
-    def negative_passive_perfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_perfective_past('دید')
-            ['دیده نشدم', 'دیده نشدی', 'دیده نشد', 'دیده نشدیم', 'دیده نشدید', 'دیده نشدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_perfective_past("شد")]
-
-    def imperfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_past('دید')
-            ['می‌دیدم', 'می‌دیدی', 'می‌دید', 'می‌دیدیم', 'می‌دیدید', 'می‌دیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پایا.
-        """
-        return ["می‌" + x for x in self.perfective_past(ri)]
-
-    def negative_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_past('دید')
-            ['نمی‌دیدم', 'نمی‌دیدی', 'نمی‌دید', 'نمی‌دیدیم', 'نمی‌دیدید', 'نمی‌دیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_past(ri)]
-
-    def passive_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_past('دید')
-            ['دیده می‌شدم', 'دیده می‌شدی', 'دیده می‌شد', 'دیده می‌شدیم', 'دیده می‌شدید', 'دیده می‌شدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_past("شد")]
-
-    def negative_passive_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_past('دید')
-            ['دیده نمی‌شدم', 'دیده نمی‌شدی', 'دیده نمی‌شد', 'دیده نمی‌شدیم', 'دیده نمی‌شدید', 'دیده نمی‌شدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_past("شد")]
-
-    def past_progresive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_progresive('دید')
-            ['داشتم می‌دیدم', 'داشتی می‌دیدی', 'داشت می‌دید', 'داشتیم می‌دیدیم', 'داشتید می‌دیدید', 'داشتند می‌دیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(self.perfective_past("داشت"), self.imperfective_past(ri))
-        ]
-
-    def passive_past_progresive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_progresive('دید')
-            ['داشتم دیده می‌شدم', 'داشتی دیده می‌شدی', 'داشت دیده می‌شد', 'داشتیم دیده می‌شدیم', 'داشتید دیده می‌شدید', 'داشتند دیده می‌شدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_past("داشت"),
-                self.passive_imperfective_past(ri),
-            )
-        ]
-
-    def present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.present_perfect('دید')
-            ['دیده‌ام', 'دیده‌ای', 'دیده است', 'دیده', 'دیده‌ایم', 'دیده‌اید', 'دیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل.
-        """
-        return [ri + x for x in ["ه‌ام", "ه‌ای", "ه است", "ه", "ه‌ایم", "ه‌اید", "ه‌اند"]]
-
-    def negative_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_present_perfect('دید')
-            ['ندیده‌ام', 'ندیده‌ای', 'ندیده است', 'ندیده', 'ندیده‌ایم', 'ندیده‌اید', 'ندیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.present_perfect(ri)]
-
-    def subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_present_perfect('دید')
-            ['دیده باشم', 'دیده باشی', 'دیده باشد', 'دیده باشیم', 'دیده باشید', 'دیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی.
-        """
-        return [ri + "ه " + x for x in self.perfective_present("باش")]
-
-    def negative_subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_present_perfect('دید')
-            ['ندیده باشم', 'ندیده باشی', 'ندیده باشد', 'ندیده باشیم', 'ندیده باشید', 'ندیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.subjunctive_present_perfect(ri)]
-
-    def grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه دستوری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.grammatical_present_perfect('دید')
-            ['دیده باشم', 'دیده باش', 'دیده باشد', 'دیده باشیم', 'دیده باشید', 'دیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری.
-        """
-        return [
-            ri + "ه " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def negative_grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه دستوری به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_grammatical_present_perfect('دید')
-            ['ندیده باشم', 'ندیده باش', 'ندیده باشد', 'ندیده باشیم', 'ندیده باشید', 'ندیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری به‌شکل منفی.
-        """
-        return [
-            "ن" + ri + "ه " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def passive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_present_perfect('دید')
-            ['دیده شده‌ام', 'دیده شده‌ای', 'دیده شده است', 'دیده شده', 'دیده شده‌ایم', 'دیده شده‌اید', 'دیده شده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.present_perfect("شد")]
-
-    def negative_passive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_present_perfect('دید')
-            ['دیده نشده‌ام', 'دیده نشده‌ای', 'دیده نشده است', 'دیده نشده', 'دیده نشده‌ایم', 'دیده نشده‌اید', 'دیده نشده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_present_perfect("شد")]
-
-    def passive_subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_present_perfect('دید')
-            ['دیده شده باشم', 'دیده شده باشی', 'دیده شده باشد', 'دیده شده باشیم', 'دیده شده باشید', 'دیده شده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.subjunctive_present_perfect("شد")]
-
-    def negative_passive_subjunctive_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_present_perfect('دید')
-            ['دیده نشده باشم', 'دیده نشده باشی', 'دیده نشده باشد', 'دیده نشده باشیم', 'دیده نشده باشید', 'دیده نشده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_subjunctive_present_perfect("شد")]
-
-    def passive_grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه دستوری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_grammatical_present_perfect('دید')
-            ['دیده شده باشم', 'دیده شده باش', 'دیده شده باشد', 'دیده شده باشیم', 'دیده شده باشید', 'دیده شده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری در حالت مجهول.
-        """
-        return [
-            ri + "ه شده " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def negative_passive_grammatical_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_grammatical_present_perfect('دید')
-            ['دیده نشده باشم', 'دیده نشده باش', 'دیده نشده باشد', 'دیده نشده باشیم', 'دیده نشده باشید', 'دیده نشده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه نشده " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def imperfective_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_present_perfect('دید')
-            ['می‌دیده‌ام', 'می‌دیده‌ای', 'می‌دیده است', 'می‌دیده', 'می‌دیده‌ایم', 'می‌دیده‌اید', 'می‌دیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا.
-        """
-        return ["می‌" + x for x in self.present_perfect(ri)]
-
-    def negative_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_present_perfect('دید')
-            ['نمی‌دیده‌ام', 'نمی‌دیده‌ای', 'نمی‌دیده است', 'نمی‌دیده', 'نمی‌دیده‌ایم', 'نمی‌دیده‌اید', 'نمی‌دیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_present_perfect(ri)]
-
-    def subjunctive_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_imperfective_present_perfect('دید')
-            ['می‌دیده باشم', 'می‌دیده باشی', 'می‌دیده باشد', 'می‌دیده باشیم', 'می‌دیده باشید', 'می‌دیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی.
-        """
-        return ["می‌" + x for x in self.subjunctive_present_perfect(ri)]
-
-    def negative_subjunctive_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_imperfective_present_perfect('دید')
-            ['نمی‌دیده باشم', 'نمی‌دیده باشی', 'نمی‌دیده باشد', 'نمی‌دیده باشیم', 'نمی‌دیده باشید', 'نمی‌دیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.subjunctive_imperfective_present_perfect(ri)]
-
-    def passive_imperfective_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_present_perfect('دید')
-            ['دیده می‌شده‌ام', 'دیده می‌شده‌ای', 'دیده می‌شده است', 'دیده می‌شده', 'دیده می‌شده‌ایم', 'دیده می‌شده‌اید', 'دیده می‌شده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_present_perfect("شد")]
-
-    def negative_passive_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_present_perfect('دید')
-            ['دیده نمی‌شده‌ام', 'دیده نمی‌شده‌ای', 'دیده نمی‌شده است', 'دیده نمی‌شده', 'دیده نمی‌شده‌ایم', 'دیده نمی‌شده‌اید', 'دیده نمی‌شده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_present_perfect("شد")]
-
-    def passive_subjunctive_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_imperfective_present_perfect('دید')
-            ['دیده می‌شده باشم', 'دیده می‌شده باشی', 'دیده می‌شده باشد', 'دیده می‌شده باشیم', 'دیده می‌شده باشید', 'دیده می‌شده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی در حالت مجهول.
-        """
-        return [
-            ri + "ه " + x for x in self.subjunctive_imperfective_present_perfect("شد")
-        ]
-
-    def negative_passive_subjunctive_imperfective_present_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_imperfective_present_perfect('دید')
-            ['دیده نمی‌شده باشم', 'دیده نمی‌شده باشی', 'دیده نمی‌شده باشد', 'دیده نمی‌شده باشیم', 'دیده نمی‌شده باشید', 'دیده نمی‌شده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x
-            for x in self.negative_subjunctive_imperfective_present_perfect("شد")
-        ]
-
-    def present_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.present_perfect_progressive('دید')
-            ['داشته‌ام می‌دیده‌ام', 'داشته‌ای می‌دیده‌ای', 'داشته است می‌دیده است', 'داشته می‌دیده', 'داشته‌ایم می‌دیده‌ایم', 'داشته‌اید می‌دیده‌اید', 'داشته‌اند می‌دیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.present_perfect("داشت"),
-                self.imperfective_present_perfect(ri),
-            )
-        ]
-
-    def passive_present_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_present_perfect_progressive('دید')
-            ['داشته‌ام دیده می‌شده‌ام', 'داشته‌ای دیده می‌شده‌ای', 'داشته است دیده می‌شده است', 'داشته دیده می‌شده', 'داشته‌ایم دیده می‌شده‌ایم', 'داشته‌اید دیده می‌شده‌اید', 'داشته‌اند دیده می‌شده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.present_perfect("داشت"),
-                self.passive_imperfective_present_perfect(ri),
-            )
-        ]
-
-    def past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_precedent('دید')
-            ['دیده بودم', 'دیده بودی', 'دیده بود', 'دیده بودیم', 'دیده بودید', 'دیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین.
-        """
-        return [ri + "ه " + x for x in self.perfective_past("بود")]
-
-    def negative_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_past_precedent('دید')
-            ['ندیده بودم', 'ندیده بودی', 'ندیده بود', 'ندیده بودیم', 'ندیده بودید', 'ندیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.past_precedent(ri)]
-
-    def passive_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_precedent('دید')
-            ['دیده شده بودم', 'دیده شده بودی', 'دیده شده بود', 'دیده شده بودیم', 'دیده شده بودید', 'دیده شده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.past_precedent("شد")]
-
-    def negative_passive_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_past_precedent('دید')
-            ['دیده نشده بودم', 'دیده نشده بودی', 'دیده نشده بود', 'دیده نشده بودیم', 'دیده نشده بودید', 'دیده نشده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_past_precedent("شد")]
-
-    def imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_past_precedent('دید')
-            ['می‌دیده بودم', 'می‌دیده بودی', 'می‌دیده بود', 'می‌دیده بودیم', 'می‌دیده بودید', 'می‌دیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا.
-        """
-        return ["می‌" + x for x in self.past_precedent(ri)]
-
-    def negative_imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_past_precedent('دید')
-            ['نمی‌دیده بودم', 'نمی‌دیده بودی', 'نمی‌دیده بود', 'نمی‌دیده بودیم', 'نمی‌دیده بودید', 'نمی‌دیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_past_precedent(ri)]
-
-    def passive_imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_past_precedent('دید')
-            ['دیده می‌شده بودم', 'دیده می‌شده بودی', 'دیده می‌شده بود', 'دیده می‌شده بودیم', 'دیده می‌شده بودید', 'دیده می‌شده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_past_precedent("شد")]
-
-    def negative_passive_imperfective_past_precedent(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_past_precedent('دید')
-            ['دیده نمی‌شده بودم', 'دیده نمی‌شده بودی', 'دیده نمی‌شده بود', 'دیده نمی‌شده بودیم', 'دیده نمی‌شده بودید', 'دیده نمی‌شده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_past_precedent("شد")]
-
-    def past_precedent_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_precedent_progressive('دید')
-            ['داشتم می‌دیده بودم', 'داشتی می‌دیده بودی', 'داشت می‌دیده بود', 'داشتیم می‌دیده بودیم', 'داشتید می‌دیده بودید', 'داشتند می‌دیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_past("داشت"),
-                self.imperfective_past_precedent(ri),
-            )
-        ]
-
-    def passive_past_precedent_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_precedent_progressive('دید')
-            ['داشتم دیده می‌شده بودم', 'داشتی دیده می‌شده بودی', 'داشت دیده می‌شده بود', 'داشتیم دیده می‌شده بودیم', 'داشتید دیده می‌شده بودید', 'داشتند دیده می‌شده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_past("داشت"),
-                self.passive_imperfective_past_precedent(ri),
-            )
-        ]
-
-    def past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_precedent_perfect('دید')
-            ['دیده بوده‌ام', 'دیده بوده‌ای', 'دیده بوده است', 'دیده بوده', 'دیده بوده‌ایم', 'دیده بوده‌اید', 'دیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل.
-        """
-        return [ri + "ه " + x for x in self.present_perfect("بود")]
-
-    def negative_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_past_precedent_perfect('دید')
-            ['ندیده بوده‌ام', 'ندیده بوده‌ای', 'ندیده بوده است', 'ندیده بوده', 'ندیده بوده‌ایم', 'ندیده بوده‌اید', 'ندیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.past_precedent_perfect(ri)]
-
-    def subjunctive_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_past_precedent_perfect('دید')
-            ['دیده بوده باشم', 'دیده بوده باشی', 'دیده بوده باشد', 'دیده بوده باشیم', 'دیده بوده باشید', 'دیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی.
-        """
-        return [ri + "ه " + x for x in self.subjunctive_present_perfect("بود")]
-
-    def negative_subjunctive_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_past_precedent_perfect('دید')
-            ['ندیده بوده باشم', 'ندیده بوده باشی', 'ندیده بوده باشد', 'ندیده بوده باشیم', 'ندیده بوده باشید', 'ندیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.subjunctive_past_precedent_perfect(ri)]
-
-    def grammatical_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.grammatical_past_precedent_perfect('دید')
-            ['دیده بوده باشم', 'دیده بوده باش', 'دیده بوده باشد', 'دیده بوده باشیم', 'دیده بوده باشید', 'دیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری.
-        """
-        return [
-            ri + "ه بوده " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def negative_grammatical_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_grammatical_past_precedent_perfect('دید')
-            ['ندیده بوده باشم', 'ندیده بوده باش', 'ندیده بوده باشد', 'ندیده بوده باشیم', 'ندیده بوده باشید', 'ندیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.grammatical_past_precedent_perfect(ri)]
-
-    def passive_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_precedent_perfect('دید')
-            ['دیده شده بوده‌ام', 'دیده شده بوده‌ای', 'دیده شده بوده است', 'دیده شده بوده', 'دیده شده بوده‌ایم', 'دیده شده بوده‌اید', 'دیده شده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.past_precedent_perfect("شد")]
-
-    def negative_passive_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_past_precedent_perfect('دید')
-            ['دیده نشده بوده‌ام', 'دیده نشده بوده‌ای', 'دیده نشده بوده است', 'دیده نشده بوده', 'دیده نشده بوده‌ایم', 'دیده نشده بوده‌اید', 'دیده نشده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_past_precedent_perfect("شد")]
-
-    def passive_subjunctive_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_past_precedent_perfect('دید')
-            ['دیده شده بوده باشم', 'دیده شده بوده باشی', 'دیده شده بوده باشد', 'دیده شده بوده باشیم', 'دیده شده بوده باشید', 'دیده شده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.subjunctive_past_precedent_perfect("شد")]
-
-    def negative_passive_subjunctive_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_past_precedent_perfect('دید')
-            ['دیده نشده بوده باشم', 'دیده نشده بوده باشی', 'دیده نشده بوده باشد', 'دیده نشده بوده باشیم', 'دیده نشده بوده باشید', 'دیده نشده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + "ن" + x for x in self.subjunctive_past_precedent_perfect("شد")
-        ]
-
-    def passive_grammatical_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_grammatical_past_precedent_perfect('دید')
-            ['دیده شده بوده باشم', 'دیده شده بوده باش', 'دیده شده بوده باشد', 'دیده شده بوده باشیم', 'دیده شده بوده باشید', 'دیده شده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.grammatical_past_precedent_perfect("شد")]
-
-    def negative_passive_grammatical_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_grammatical_past_precedent_perfect('دید')
-            ['دیده نشده بوده باشم', 'دیده نشده بوده باش', 'دیده نشده بوده باشد', 'دیده نشده بوده باشیم', 'دیده نشده بوده باشید', 'دیده نشده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x
-            for x in self.negative_grammatical_past_precedent_perfect("شد")
-        ]
-
-    def imperfective_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_past_precedent_perfect('دید')
-            ['می‌دیده بوده‌ام', 'می‌دیده بوده‌ای', 'می‌دیده بوده است', 'می‌دیده بوده', 'می‌دیده بوده‌ایم', 'می‌دیده بوده‌اید', 'می‌دیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا.
-        """
-        return ["می‌" + x for x in self.past_precedent_perfect(ri)]
-
-    def negative_imperfective_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_past_precedent_perfect('دید')
-            ['نمی‌دیده بوده‌ام', 'نمی‌دیده بوده‌ای', 'نمی‌دیده بوده است', 'نمی‌دیده بوده', 'نمی‌دیده بوده‌ایم', 'نمی‌دیده بوده‌اید', 'نمی‌دیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_past_precedent_perfect(ri)]
-
-    def subjunctive_imperfective_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_imperfective_past_precedent_perfect('دید')
-            ['می‌دیده بوده باشم', 'می‌دیده بوده باشی', 'می‌دیده بوده باشد', 'می‌دیده بوده باشیم', 'می‌دیده بوده باشید', 'می‌دیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی.
-        """
-        return ["می‌" + x for x in self.subjunctive_past_precedent_perfect(ri)]
-
-    def negative_subjunctive_imperfective_past_precedent_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_imperfective_past_precedent_perfect('دید')
-            ['نمی‌دیده بوده باشم', 'نمی‌دیده بوده باشی', 'نمی‌دیده بوده باشد', 'نمی‌دیده بوده باشیم', 'نمی‌دیده بوده باشید', 'نمی‌دیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی به‌شکل منفی.
-        """
-        return [
-            "ن" + x for x in self.subjunctive_imperfective_past_precedent_perfect(ri)
-        ]
-
-    def passive_imperfective_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_past_precedent_perfect('دید')
-            ['دیده می‌شده بوده‌ام', 'دیده می‌شده بوده‌ای', 'دیده می‌شده بوده است', 'دیده می‌شده بوده', 'دیده می‌شده بوده‌ایم', 'دیده می‌شده بوده‌اید', 'دیده می‌شده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_past_precedent_perfect("شد")]
-
-    def negative_passive_imperfective_past_precedent_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_past_precedent_perfect('دید')
-            ['دیده نمی‌شده بوده‌ام', 'دیده نمی‌شده بوده‌ای', 'دیده نمی‌شده بوده است', 'دیده نمی‌شده بوده', 'دیده نمی‌شده بوده‌ایم', 'دیده نمی‌شده بوده‌اید', 'دیده نمی‌شده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x
-            for x in self.negative_imperfective_past_precedent_perfect("شد")
-        ]
-
-    def passive_subjunctive_imperfective_past_precedent_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_imperfective_past_precedent_perfect('دید')
-            ['دیده می‌شده بوده باشم', 'دیده می‌شده بوده باشی', 'دیده می‌شده بوده باشد', 'دیده می‌شده بوده باشیم', 'دیده می‌شده بوده باشید', 'دیده می‌شده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول.
-        """
-        return [
-            ri + "ه " + x
-            for x in self.subjunctive_imperfective_past_precedent_perfect("شد")
-        ]
-
-    def negative_passive_subjunctive_imperfective_past_precedent_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_imperfective_past_precedent_perfect('دید')
-            ['دیده نمی‌شده بوده باشم', 'دیده نمی‌شده بوده باشی', 'دیده نمی‌شده بوده باشد', 'دیده نمی‌شده بوده باشیم', 'دیده نمی‌شده بوده باشید', 'دیده نمی‌شده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + "ن" + x
-            for x in self.subjunctive_imperfective_past_precedent_perfect("شد")
-        ]
-
-    def past_precedent_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_precedent_perfect_progressive('دید')
-            ['داشته‌ام می‌دیده بوده‌ام', 'داشته‌ای می‌دیده بوده‌ای', 'داشته است می‌دیده بوده است', 'داشته می‌دیده بوده', 'داشته‌ایم می‌دیده بوده‌ایم', 'داشته‌اید می‌دیده بوده‌اید', 'داشته‌اند می‌دیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.present_perfect("داشت"),
-                self.imperfective_past_precedent_perfect(ri),
-            )
-        ]
-
-    def passive_past_precedent_perfect_progressive(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_precedent_perfect_progressive('دید')
-            ['داشته‌ام دیده می‌شده بوده‌ام', 'داشته‌ای دیده می‌شده بوده‌ای', 'داشته است دیده می‌شده بوده است', 'داشته دیده می‌شده بوده', 'داشته‌ایم دیده می‌شده بوده‌ایم', 'داشته‌اید دیده می‌شده بوده‌اید', 'داشته‌اند دیده می‌شده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.present_perfect("داشت"),
-                self.passive_imperfective_past_precedent_perfect(ri),
-            )
-        ]
-
-    def perfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال مطلق صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.perfective_present('بین')
-            ['بینم', 'بینی', 'بیند', 'بینیم', 'بینید', 'بینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق.
-        """
-        return [rii + x for x in ["م", "ی", "د", "یم", "ید", "ند"]]
-
-    def negative_perfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال مطلق به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_perfective_present('بین')
-            ['نبینم', 'نبینی', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.perfective_present(rii)]
-
-    def subjunctive_perfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_perfective_present('بین')
-            ['ببینم', 'ببینی', 'ببیند', 'ببینیم', 'ببینید', 'ببینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی.
-        """
-        return ["ب" + x for x in self.perfective_present(rii)]
-
-    def negative_subjunctive_perfective_present(
-        self: "Conjugation", rii: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_perfective_present('بین')
-            ['نبینم', 'نبینی', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.perfective_present(rii)]
-
-    def grammatical_perfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه دستوری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.grammatical_perfective_present('بین')
-            ['ببینم', 'ببین', 'ببیند', 'ببینیم', 'ببینید', 'ببینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری.
-        """
-        return [
-            "ببین" if x == "ببینی" else x
-            for x in self.subjunctive_perfective_present(rii)
-        ]
-
-    def negative_grammatical_perfective_present(
-        self: "Conjugation", rii: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه دستوری به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_grammatical_perfective_present('بین')
-            ['نبینم', 'نبین', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری به‌شکل منفی.
-        """
-        return [
-            "ن" + ("بین" if x == "بینی" else x) for x in self.perfective_present(rii)
-        ]
-
-    def passive_perfective_present(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال مطلق در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_perfective_present('دید')
-            ['دیده شوم', 'دیده شوی', 'دیده شود', 'دیده شویم', 'دیده شوید', 'دیده شوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.perfective_present("شو")]
-
-    def negative_passive_perfective_present(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_perfective_present('دید')
-            ['دیده نشوم', 'دیده نشوی', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_perfective_present("شو")]
-
-    def passive_subjunctive_perfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_perfective_present('دید')
-            ['دیده بشوم', 'دیده بشوی', 'دیده بشود', 'دیده بشویم', 'دیده بشوید', 'دیده بشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.subjunctive_perfective_present("شو")]
-
-    def negative_passive_subjunctive_perfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_perfective_present('دید')
-            ['دیده نشوم', 'دیده نشوی', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x for x in self.negative_subjunctive_perfective_present("شو")
-        ]
-
-    def passive_grammatical_perfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه دستوری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_grammatical_perfective_present('دید')
-            ['دیده بشوم', 'دیده بشو', 'دیده بشود', 'دیده بشویم', 'دیده بشوید', 'دیده بشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری در حالت مجهول.
-        """
-        return [
-            ri + "ه " + ("بشو" if x == "بشوی" else x)
-            for x in self.grammatical_perfective_present("شو")
-        ]
-
-    def negative_passive_grammatical_perfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_grammatical_perfective_present('دید')
-            ['دیده نشوم', 'دیده نشو', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + ("نشو" if x == "نشوی" else x)
-            for x in self.negative_grammatical_perfective_present("شو")
-        ]
-
-    def imperfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_present('بین')
-            ['می‌بینم', 'می‌بینی', 'می‌بیند', 'می‌بینیم', 'می‌بینید', 'می‌بینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال پایا.
-        """
-        return ["می‌" + x for x in self.perfective_present(rii)]
-
-    def negative_imperfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_present('بین')
-            ['نمی‌بینم', 'نمی‌بینی', 'نمی‌بیند', 'نمی‌بینیم', 'نمی‌بینید', 'نمی‌بینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_present(rii)]
-
-    def passive_imperfective_present(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_present('دید')
-            ['دیده می‌شوم', 'دیده می‌شوی', 'دیده می‌شود', 'دیده می‌شویم', 'دیده می‌شوید', 'دیده می‌شوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_present("شو")]
-
-    def negative_passive_imperfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_present('دید')
-            ['دیده نمی‌شوم', 'دیده نمی‌شوی', 'دیده نمی‌شود', 'دیده نمی‌شویم', 'دیده نمی‌شوید', 'دیده نمی‌شوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_present("شو")]
-
-    def present_progressive(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.present_progressive('بین')
-            ['دارم می‌بینم', 'داری می‌بینی', 'دارد می‌بیند', 'داریم می‌بینیم', 'دارید می‌بینید', 'دارند می‌بینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_present("دار"),
-                self.imperfective_present(rii),
-            )
-        ]
-
-    def passive_present_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_present_progressive('دید')
-            ['دارم دیده می‌شوم', 'داری دیده می‌شوی', 'دارد دیده می‌شود', 'داریم دیده می‌شویم', 'دارید دیده می‌شوید', 'دارند دیده می‌شوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_present("دار"),
-                self.passive_imperfective_present(ri),
-            )
-        ]
-
-    def perfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ مطلق صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.perfective_future('دید')
-            ['خواهم دید', 'خواهی دید', 'خواهد دید', 'خواهیم دید', 'خواهید دید', 'خواهند دید']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ مطلق.
-        """
-        return [x + " " + ri for x in self.perfective_present("خواه")]
-
-    def negative_perfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ مطلق به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_perfective_future('دید')
-            ['نخواهم دید', 'نخواهی دید', 'نخواهد دید', 'نخواهیم دید', 'نخواهید دید', 'نخواهند دید']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ مطلق به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.perfective_future(ri)]
-
-    def passive_perfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ مطلق در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_perfective_future('دید')
-            ['دیده خواهم شد', 'دیده خواهی شد', 'دیده خواهد شد', 'دیده خواهیم شد', 'دیده خواهید شد', 'دیده خواهند شد']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ مطلق در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.perfective_future("شد")]
-
-    def negative_passive_perfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_perfective_future('دید')
-            ['دیده نخواهم شد', 'دیده نخواهی شد', 'دیده نخواهد شد', 'دیده نخواهیم شد', 'دیده نخواهید شد', 'دیده نخواهند شد']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ مطلق در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_perfective_future("شد")]
-
-    def imperfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_future('دید')
-            ['می‌خواهم دید', 'می‌خواهی دید', 'می‌خواهد دید', 'می‌خواهیم دید', 'می‌خواهید دید', 'می‌خواهند دید']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پایا.
-        """
-        return ["می‌" + x for x in self.perfective_future(ri)]
-
-    def negative_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_future('دید')
-            ['نمی‌خواهم دید', 'نمی‌خواهی دید', 'نمی‌خواهد دید', 'نمی‌خواهیم دید', 'نمی‌خواهید دید', 'نمی‌خواهند دید']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_future(ri)]
-
-    def passive_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_future('دید')
-            ['دیده می‌خواهم شد', 'دیده می‌خواهی شد', 'دیده می‌خواهد شد', 'دیده می‌خواهیم شد', 'دیده می‌خواهید شد', 'دیده می‌خواهند شد']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_future("شد")]
-
-    def negative_passive_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_future('دید')
-            ['دیده نمی‌خواهم شد', 'دیده نمی‌خواهی شد', 'دیده نمی‌خواهد شد', 'دیده نمی‌خواهیم شد', 'دیده نمی‌خواهید شد', 'دیده نمی‌خواهند شد']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_future("شد")]
-
-    def future_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.future_precedent('دید')
-            ['دیده خواهم بود', 'دیده خواهی بود', 'دیده خواهد بود', 'دیده خواهیم بود', 'دیده خواهید بود', 'دیده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین.
-        """
-        return [ri + "ه " + x for x in self.perfective_future("بود")]
-
-    def negative_future_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_future_precedent('دید')
-            ['ندیده خواهم بود', 'ندیده خواهی بود', 'ندیده خواهد بود', 'ندیده خواهیم بود', 'ندیده خواهید بود', 'ندیده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.future_precedent(ri)]
-
-    def passive_future_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_future_precedent('دید')
-            ['دیده شده خواهم بود', 'دیده شده خواهی بود', 'دیده شده خواهد بود', 'دیده شده خواهیم بود', 'دیده شده خواهید بود', 'دیده شده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.future_precedent("شد")]
-
-    def negative_passive_future_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_future_precedent('دید')
-            ['دیده نشده خواهم بود', 'دیده نشده خواهی بود', 'دیده نشده خواهد بود', 'دیده نشده خواهیم بود', 'دیده نشده خواهید بود', 'دیده نشده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_future_precedent("شد")]
-
-    def future_precedent_imperfective(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.future_precedent_imperfective('دید')
-            ['می‌دیده خواهم بود', 'می‌دیده خواهی بود', 'می‌دیده خواهد بود', 'می‌دیده خواهیم بود', 'می‌دیده خواهید بود', 'می‌دیده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا.
-        """
-        return ["می‌" + x for x in self.future_precedent(ri)]
-
-    def negative_future_precedent_imperfective(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_future_precedent_imperfective('دید')
-            ['نمی‌دیده خواهم بود', 'نمی‌دیده خواهی بود', 'نمی‌دیده خواهد بود', 'نمی‌دیده خواهیم بود', 'نمی‌دیده خواهید بود', 'نمی‌دیده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.future_precedent_imperfective(ri)]
-
-    def passive_future_precedent_imperfective(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_future_precedent_imperfective('دید')
-            ['دیده می‌شده خواهم بود', 'دیده می‌شده خواهی بود', 'دیده می‌شده خواهد بود', 'دیده می‌شده خواهیم بود', 'دیده می‌شده خواهید بود', 'دیده می‌شده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.future_precedent_imperfective("شد")]
-
-    def negative_passive_future_precedent_imperfective(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_future_precedent_imperfective('دید')
-            ['دیده نمی‌شده خواهم بود', 'دیده نمی‌شده خواهی بود', 'دیده نمی‌شده خواهد بود', 'دیده نمی‌شده خواهیم بود', 'دیده نمی‌شده خواهید بود', 'دیده نمی‌شده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x for x in self.negative_future_precedent_imperfective("شد")
-        ]
-
-    def get(self: "Conjugation", verb, negative=False, passive=False) -> List[str]:
-        """صورت‌های صرفی فعل را برمی‌گرداند.
-
-        Args:
-            verb (str): فعلی که باید صرف شود. به‌صورت بن ماضی#بن مضارع؛ مانند: دید#بین.
-            negative (bool, optional): اگر `True` باشد صورت‌های صرفی منفی را برمی‌گرداند.
-            passive (bool, optional): اگر `True` باشد صورت‌های صرفی مجهول را برمی‌گرداند.
-
-        Returns:
-            (List(str)): صورت‌های صرفی فعل.
-        """
-        ri, rii = verb.split("#")
-        infinitive = [ri + "ن"]
-        result = [infinitive]
-
-        if negative and passive:
-            result.append(self.negative_passive_perfective_past(ri))
-            result.append(self.negative_passive_imperfective_past(ri))
-            result.append(self.negative_passive_present_perfect(ri))
-            result.append(self.negative_passive_subjunctive_present_perfect(ri))
-            result.append(self.negative_passive_grammatical_present_perfect(ri))
-            result.append(self.negative_passive_imperfective_present_perfect(ri))
-            result.append(
-                self.negative_passive_subjunctive_imperfective_present_perfect(ri),
-            )
-            result.append(self.negative_passive_past_precedent(ri))
-            result.append(self.negative_passive_imperfective_past_precedent(ri))
-            result.append(self.negative_passive_past_precedent_perfect(ri))
-            result.append(self.negative_passive_subjunctive_past_precedent_perfect(ri))
-            result.append(self.negative_passive_grammatical_past_precedent_perfect(ri))
-            result.append(self.negative_passive_imperfective_past_precedent_perfect(ri))
-            result.append(
-                self.negative_passive_subjunctive_imperfective_past_precedent_perfect(
-                    ri,
-                ),
-            )
-            result.append(self.negative_passive_perfective_present(ri))
-            result.append(self.negative_passive_subjunctive_perfective_present(ri))
-            result.append(self.negative_passive_grammatical_perfective_present(ri))
-            result.append(self.negative_passive_imperfective_present(ri))
-            result.append(self.negative_passive_perfective_future(ri))
-            result.append(self.negative_passive_imperfective_future(ri))
-            result.append(self.negative_passive_future_precedent(ri))
-            result.append(self.negative_passive_future_precedent_imperfective(ri))
-
-        elif passive and not negative:
-            result.append(self.passive_perfective_past(ri))
-            result.append(self.passive_imperfective_past(ri))
-            result.append(self.passive_past_progresive(ri))
-            result.append(self.passive_present_perfect(ri))
-            result.append(self.passive_subjunctive_present_perfect(ri))
-            result.append(self.passive_grammatical_present_perfect(ri))
-            result.append(self.passive_imperfective_present_perfect(ri))
-            result.append(self.passive_subjunctive_imperfective_present_perfect(ri))
-            result.append(self.passive_present_perfect_progressive(ri))
-            result.append(self.passive_past_precedent(ri))
-            result.append(self.passive_imperfective_past_precedent(ri))
-            result.append(self.passive_past_precedent_progressive(ri))
-            result.append(self.passive_past_precedent_perfect(ri))
-            result.append(self.passive_subjunctive_past_precedent_perfect(ri))
-            result.append(self.passive_grammatical_past_precedent_perfect(ri))
-            result.append(self.passive_imperfective_past_precedent_perfect(ri))
-            result.append(
-                self.passive_subjunctive_imperfective_past_precedent_perfect(ri),
-            )
-            result.append(self.passive_past_precedent_perfect_progressive(ri))
-            result.append(self.passive_perfective_present(ri))
-            result.append(self.passive_subjunctive_perfective_present(ri))
-            result.append(self.passive_grammatical_perfective_present(ri))
-            result.append(self.passive_imperfective_present(ri))
-            result.append(self.passive_present_progressive(ri))
-            result.append(self.passive_perfective_future(ri))
-            result.append(self.passive_imperfective_future(ri))
-            result.append(self.passive_future_precedent(ri))
-            result.append(self.passive_future_precedent_imperfective(ri))
-
-        elif negative and not passive:
-            result.append(self.negative_perfective_past(ri))
-            result.append(self.negative_imperfective_past(ri))
-            result.append(self.negative_present_perfect(ri))
-            result.append(self.negative_subjunctive_present_perfect(ri))
-            result.append(self.negative_grammatical_present_perfect(ri))
-            result.append(self.negative_imperfective_present_perfect(ri))
-            result.append(self.negative_subjunctive_imperfective_present_perfect(ri))
-            result.append(self.negative_past_precedent(ri))
-            result.append(self.negative_imperfective_past_precedent(ri))
-            result.append(self.negative_past_precedent_perfect(ri))
-            result.append(self.negative_subjunctive_past_precedent_perfect(ri))
-            result.append(self.negative_grammatical_past_precedent_perfect(ri))
-            result.append(self.negative_imperfective_past_precedent_perfect(ri))
-            result.append(
-                self.negative_subjunctive_imperfective_past_precedent_perfect(ri),
-            )
-            result.append(self.negative_perfective_present(rii))
-            result.append(self.negative_subjunctive_perfective_present(rii))
-            result.append(self.negative_grammatical_perfective_present(rii))
-            result.append(self.negative_imperfective_present(rii))
-            result.append(self.negative_perfective_future(ri))
-            result.append(self.negative_imperfective_future(ri))
-            result.append(self.negative_future_precedent(ri))
-            result.append(self.negative_future_precedent_imperfective(ri))
-
-        elif not negative and not passive:
-            result.append(self.perfective_past(ri))
-            result.append(self.imperfective_past(ri))
-            result.append(self.past_progresive(ri))
-            result.append(self.present_perfect(ri))
-            result.append(self.subjunctive_present_perfect(ri))
-            result.append(self.grammatical_present_perfect(ri))
-            result.append(self.imperfective_present_perfect(ri))
-            result.append(self.subjunctive_imperfective_present_perfect(ri))
-            result.append(self.present_perfect_progressive(ri))
-            result.append(self.past_precedent(ri))
-            result.append(self.imperfective_past_precedent(ri))
-            result.append(self.past_precedent_progressive(ri))
-            result.append(self.past_precedent_perfect(ri))
-            result.append(self.subjunctive_past_precedent_perfect(ri))
-            result.append(self.grammatical_past_precedent_perfect(ri))
-            result.append(self.imperfective_past_precedent_perfect(ri))
-            result.append(self.subjunctive_imperfective_past_precedent_perfect(ri))
-            result.append(self.past_precedent_perfect_progressive(ri))
-            result.append(self.perfective_present(rii))
-            result.append(self.subjunctive_perfective_present(rii))
-            result.append(self.grammatical_perfective_present(rii))
-            result.append(self.imperfective_present(rii))
-            result.append(self.present_progressive(rii))
-            result.append(self.perfective_future(ri))
-            result.append(self.imperfective_future(ri))
-            result.append(self.future_precedent(ri))
-            result.append(self.future_precedent_imperfective(ri))
-
-        return sum(result, [])
-
-    def get_all(self: "Conjugation", verb: str) -> List[str]:
-        """تمام صورت‌های صرفی فعل را در وجوه اخباری، التزامی، دستوری و در اشکال منفی و مثبت و مجهول برمی‌گرداند.
-
-        Args:
-            verb (str): فعلی که باید صرف شود. به‌صورت بن ماضی#بن مضارع؛ مانند: دید#بین.
-
-        Returns:
-             لیست تمام صورت‌های صرفی فعل.
-        """
-        ri, rii = verb.split("#")
-        infinitive = [ri + "ن"]
-        result = [infinitive]
-
-        # گذشتهٔ مطلق
-        result.append(self.perfective_past(ri))
-
-        # گذشتهٔ مطلق منفی
-        result.append(self.negative_perfective_past(ri))
-
-        # گذشتهٔ مطلق مجهول
-        result.append(self.passive_perfective_past(ri))
-
-        # گذشتهٔ مطلق مجهول منفی
-        result.append(self.negative_passive_perfective_past(ri))
-
-        # گذشتهٔ پایا
-        result.append(self.imperfective_past(ri))
-
-        # گذشتهٔ پایای منفی
-        result.append(self.negative_imperfective_past(ri))
-
-        # گذشتهٔ پایای مجهول
-        result.append(self.passive_imperfective_past(ri))
-
-        # گذشتهٔ پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_past(ri))
-
-        # گذشتهٔ استمراری
-        result.append(self.past_progresive(ri))
-
-        # گذشتهٔ استمراری مجهول
-        result.append(self.passive_past_progresive(ri))
-
-        # حال کامل
-        result.append(self.present_perfect(ri))
-
-        # حال کامل منفی
-        result.append(self.negative_present_perfect(ri))
-
-        # حال کامل التزامی
-        result.append(self.subjunctive_present_perfect(ri))
-
-        # حال کامل التزامی منفی
-        result.append(self.negative_subjunctive_present_perfect(ri))
-
-        # حال کامل دستوری
-        result.append(self.grammatical_present_perfect(ri))
-
-        # حال کامل دستوری منفی
-        result.append(self.negative_grammatical_present_perfect(ri))
-
-        # حال کامل مجهول
-        result.append(self.passive_present_perfect(ri))
-
-        # حال کامل مجهول منفی
-        result.append(self.negative_passive_present_perfect(ri))
-
-        # حال کامل التزامی مجهول
-        result.append(self.passive_subjunctive_present_perfect(ri))
-
-        # حال کامل التزامی مجهول منفی
-        result.append(self.negative_passive_subjunctive_present_perfect(ri))
-
-        # حال کامل دستوری مجهول
-        result.append(self.passive_grammatical_present_perfect(ri))
-
-        # حال کامل دستوری مجهول منفی
-        result.append(self.negative_passive_grammatical_present_perfect(ri))
-
-        # حال کامل پایا
-        result.append(self.imperfective_present_perfect(ri))
-
-        # حال کامل پایای منفی
-        result.append(self.negative_imperfective_present_perfect(ri))
-
-        # حال کامل پایای التزامی
-        result.append(self.subjunctive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای التزامی منفی
-        result.append(self.negative_subjunctive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای مجهول
-        result.append(self.passive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای التزامی مجهول
-        result.append(self.passive_subjunctive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای التزامی مجهول منفی
-        result.append(
-            self.negative_passive_subjunctive_imperfective_present_perfect(ri),
-        )
-
-        # حال کامل استمراری
-        result.append(self.present_perfect_progressive(ri))
-
-        # حال کامل استمراری مجهول
-        result.append(self.passive_present_perfect_progressive(ri))
-
-        # گذشتهٔ پیشین
-        result.append(self.past_precedent(ri))
-
-        # گذشتهٔ پیشین منفی
-        result.append(self.negative_past_precedent(ri))
-
-        # گذشتهٔ پیشین مجهول
-        result.append(self.passive_past_precedent(ri))
-
-        # گذشتهٔ پیشین مجهول منفی
-        result.append(self.negative_passive_past_precedent(ri))
-
-        # گذشتهٔ پیشین پایا
-        result.append(self.imperfective_past_precedent(ri))
-
-        # گذشتهٔ پیشین پایای منفی
-        result.append(self.negative_imperfective_past_precedent(ri))
-
-        # گذشتهٔ پیشین پایای مجهول
-        result.append(self.passive_imperfective_past_precedent(ri))
-
-        # گذشتهٔ پیشین پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_past_precedent(ri))
-
-        # گذشتهٔ پیشین استمراری
-        result.append(self.past_precedent_progressive(ri))
-
-        # گذشتهٔ پیشین استمراری مجهول
-        result.append(self.passive_past_precedent_progressive(ri))
-
-        # گذشتهٔ پیشین کامل
-        result.append(self.past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل منفی
-        result.append(self.negative_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل التزامی
-        result.append(self.subjunctive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل التزامی منفی
-        result.append(self.negative_subjunctive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل دستوری
-        result.append(self.grammatical_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل دستوری منفی
-        result.append(self.negative_grammatical_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل مجهول
-        result.append(self.passive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل مجهول منفی
-        result.append(self.negative_passive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل التزامی مجهول
-        result.append(self.passive_subjunctive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل التزامی مجهول منفی
-        result.append(self.negative_passive_subjunctive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشن کامل دستوری مجهول
-        result.append(self.passive_grammatical_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل دستوری مجهول منفی
-        result.append(self.negative_passive_grammatical_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایا
-        result.append(self.imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای منفی
-        result.append(self.negative_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای التزامی
-        result.append(self.subjunctive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای التزامی منفی
-        result.append(self.negative_subjunctive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای مجهول
-        result.append(self.passive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای التزامی مجهول
-        result.append(self.passive_subjunctive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای التزامی مجهول منفی
-        result.append(
-            self.negative_passive_subjunctive_imperfective_past_precedent_perfect(ri),
-        )
-
-        # گذشتهٔ پیشین کامل استمراری
-        result.append(self.past_precedent_perfect_progressive(ri))
-
-        # گذشتهٔ پیشین کامل استمراری مجهول
-        result.append(self.passive_past_precedent_perfect_progressive(ri))
-
-        # حال مطلق
-        result.append(self.perfective_present(rii))
-
-        # حال مطلق منفی
-        result.append(self.negative_perfective_present(rii))
-
-        # حال مطلق التزامی
-        result.append(self.subjunctive_perfective_present(rii))
-
-        # حال مطلق التزامی منفی
-        result.append(self.negative_subjunctive_perfective_present(rii))
-
-        # حال مطلق دستوری
-        result.append(self.grammatical_perfective_present(rii))
-
-        # حال مطلق دستوری منفی
-        result.append(self.negative_grammatical_perfective_present(rii))
-
-        # حال مطلق مجهول
-        result.append(self.passive_perfective_present(ri))
-
-        # حال مطلق مجهول منفی
-        result.append(self.negative_passive_perfective_present(ri))
-
-        # حال مطلق التزامی مجهول
-        result.append(self.passive_subjunctive_perfective_present(ri))
-
-        # حال مطلق التزامی مجهول منفی
-        result.append(self.negative_passive_subjunctive_perfective_present(ri))
-
-        # حال مطلق دستوری مجهول
-        result.append(self.passive_grammatical_perfective_present(ri))
-
-        # حال مطلق دستوری مجهول منفی
-        result.append(self.negative_passive_grammatical_perfective_present(ri))
-
-        # حال پایا
-        result.append(self.imperfective_present(rii))
-
-        # حال پایای منفی
-        result.append(self.negative_imperfective_present(rii))
-
-        # حال پایای مجهول
-        result.append(self.passive_imperfective_present(ri))
-
-        # حال پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_present(ri))
-
-        # حال استمراری
-        result.append(self.present_progressive(rii))
-
-        # حال استمراری مجهول
-        result.append(self.passive_present_progressive(ri))
-
-        # آیندهٔ مطلق
-        result.append(self.perfective_future(ri))
-
-        # آیندهٔ مطلق منفی
-        result.append(self.negative_perfective_future(ri))
-
-        # آیندهٔ مطلق مجهول
-        result.append(self.passive_perfective_future(ri))
-
-        # آیندهٔ مطلق مجهول منفی
-        result.append(self.negative_passive_perfective_future(ri))
-
-        # آیندهٔ پایا
-        result.append(self.imperfective_future(ri))
-
-        # آیندهٔ پایای منفی
-        result.append(self.negative_imperfective_future(ri))
-
-        # آیندهٔ پایای مجهول
-        result.append(self.passive_imperfective_future(ri))
-
-        # آیندهٔ پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_future(ri))
-
-        # آیندهٔ پیشین
-        result.append(self.future_precedent(ri))
-
-        # آیندهٔ پیشین منفی
-        result.append(self.negative_future_precedent(ri))
-
-        # آیندهٔ پیشین مجهول
-        result.append(self.passive_future_precedent(ri))
-
-        # آیندهٔ پیشین مجهول منفی
-        result.append(self.negative_passive_future_precedent(ri))
-
-        # آیندهٔ پیشین پایا
-        result.append(self.future_precedent_imperfective(ri))
-
-        # آیندهٔ پیشین پایای منفی
-        result.append(self.negative_future_precedent_imperfective(ri))
-
-        # آیندهٔ پیشین پایای مجهول
-        result.append(self.passive_future_precedent_imperfective(ri))
-
-        # آیندهٔ پیشین پایای مجهول منفی
-        result.append(self.negative_passive_future_precedent_imperfective(ri))
-
-        return sum(result, [])
+"""این ماژول شامل کلاس‌ها و توابعی برای ریشه‌یابی کلمات است.
+
+فرق بین [Lemmatizer](./lemmatizer.md) و [Stemmer](./stemmer.md) این است که
+اِستمر درکی از معنای کلمه ندارد و صرفاً براساس حذف برخی از پسوندهای ساده تلاش
+می‌کند ریشهٔ کلمه را بیابد؛ بنابراین ممکن است در ریشه‌یابیِ برخی از کلمات نتایج
+نادرستی ارائه دهد؛ اما لماتایزر براساس لیستی از کلمات مرجع به همراه ریشهٔ آن
+این
+کار را انجام می‌دهد و نتایج دقیق‌تری ارائه می‌دهد. البته هزینهٔ این دقت، سرعتِ
+کمتر در ریشه‌یابی است.
+
+**میزان دقت
+لماتایزر در نسخهٔ حاضر ۸۹.۹ درصد [^1] است.**
+[^1]:
+این عدد با انتشار هر نسخه بروزرسانی می‌شود
+
+"""
+
+
+from typing import List
+
+from hazm import Stemmer
+from hazm import default_verbs
+from hazm import default_words
+from hazm import WordTokenizer
+
+
+class Lemmatizer:
+    """این کلاس شامل توابعی برای ریشه‌یابی کلمات است.
+
+    Args:
+        words_file: ریشه‌یابی کلمات از روی این فایل صورت
+            می‌گیرد. هضم به صورت پیش‌فرض فایلی برای این منظور در نظر گرفته است؛ با
+            این حال شما می‌توانید فایل موردنظر خود را معرفی کنید. برای آگاهی از
+            ساختار این فایل به فایل پیش‌فرض مراجعه کنید.
+        verbs_file: اشکال صرفی فعل از روی این فایل ساخته
+            می‌شود. هضم به صورت پیش‌فرض فایلی برای این منظور در نظر گرفته است؛ با
+            این حال شما می‌توانید فایل موردنظر خود را معرفی کنید. برای آگاهی از
+            ساختار این فایل به فایل پیش‌فرض مراجعه کنید.
+        joined_verb_parts: اگر `True` باشد افعال چندبخشی را با کاراکتر زیرخط به هم می‌چسباند.
+
+    """
+
+    def __init__(
+        self: "Lemmatizer",
+        words_file: str = default_words,
+        verbs_file: str = default_verbs,
+        joined_verb_parts: bool = True,
+    ) -> None:
+        self.words_file = words_file
+        self.verbs = {}
+        self.stemmer = Stemmer()
+        self.conjugation = Conjugation()
+
+        tokenizer = WordTokenizer(words_file=default_words, verbs_file=verbs_file)
+        self.words = tokenizer.words
+
+        if verbs_file:
+            self.verbs["است"] = "#است"
+            for verb in tokenizer.verbs:
+                for tense in self.conjugation.get_all(verb):
+                    self.verbs[tense] = verb
+            if joined_verb_parts:
+                for verb in tokenizer.verbs:
+                    bon = verb.split("#")[0]
+                    for after_verb in tokenizer.after_verbs:
+                        self.verbs[bon + "ه_" + after_verb] = verb
+                        self.verbs["ن" + bon + "ه_" + after_verb] = verb
+                    for before_verb in tokenizer.before_verbs:
+                        self.verbs[before_verb + "_" + bon] = verb
+
+    def lemmatize(self: "Lemmatizer", word: str, pos: str = "") -> str:
+        """ریشهٔ کلمه را پیدا می‌کند.
+
+        پارامتر `pos` نوع کلمه است: (اسم، فعل، صفت و ...) و به این خاطر لازم
+        است که می‌تواند روی ریشه‌یابی کلمات اثر بگذارد؛ مثلاً واژهٔ «اجتماعی» در
+        جایگاه صفت (او یک فرد اجتماعی است)، ریشه‌اش همان «اجتماعی» می‌شود ولی
+        همین واژه در جایگاه اسم (اجتماعی از مردم)، ریشه‌اش می‌شود «اجتماع».
+
+        Examples:
+            >>> lemmatizer = Lemmatizer()
+            >>> lemmatizer.lemmatize('کتاب‌ها')
+            'کتاب'
+            >>> lemmatizer.lemmatize('آتشفشان')
+            'آتشفشان'
+            >>> lemmatizer.lemmatize('می‌روم')
+            'رفت#رو'
+            >>> lemmatizer.lemmatize('گفته_شده_است')
+            'گفت#گو'
+            >>> lemmatizer.lemmatize('نچشیده_است')
+            'چشید#چش'
+            >>> lemmatizer.lemmatize('مردم', pos='N')
+            'مردم'
+            >>> lemmatizer.lemmatize('اجتماعی', pos='AJ')
+            'اجتماعی'
+
+        Args:
+            word: کلمه‌ای که باید پردازش شود.
+            pos: نوع کلمه. این پارامتر سه مقدار `V` (فعل) و `AJ` (صفت) و `PRO` (ضمیر) را می‌پذیرد.
+
+        Returns:
+            ریشهٔ کلمه
+
+        """
+        if not pos and word in self.words:
+            return word
+
+        if (not pos or pos == "V") and word in self.verbs:
+            return self.verbs[word]
+
+        if pos.startswith("AJ") and word[-1] == "ی":
+            return word
+
+        if pos == "PRO":
+            return word
+
+        if word in self.words:
+            return word
+
+        stem = self.stemmer.stem(word)
+        if stem and stem in self.words:
+            return stem
+
+        return word
+
+
+class Conjugation:
+    """این کلاس دارای توابعی برای صرف‌کردن افعال است."""
+
+    def perfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ مطلق صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.perfective_past('دید')
+            ['دیدم', 'دیدی', 'دید', 'دیدیم', 'دیدید', 'دیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+            صورت‌های صرفی فعل در زمان گذشتهٔ مطلق.
+        """
+        return [ri + x for x in ["م", "ی", "", "یم", "ید", "ند"]]
+
+    def negative_perfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ مطلق به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_perfective_past('دید')
+            ['ندیدم', 'ندیدی', 'ندید', 'ندیدیم', 'ندیدید', 'ندیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.perfective_past(ri)]
+
+    def passive_perfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ مطلق در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_perfective_past('دید')
+            ['دیده شدم', 'دیده شدی', 'دیده شد', 'دیده شدیم', 'دیده شدید', 'دیده شدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.perfective_past("شد")]
+
+    def negative_passive_perfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_perfective_past('دید')
+            ['دیده نشدم', 'دیده نشدی', 'دیده نشد', 'دیده نشدیم', 'دیده نشدید', 'دیده نشدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_perfective_past("شد")]
+
+    def imperfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_past('دید')
+            ['می‌دیدم', 'می‌دیدی', 'می‌دید', 'می‌دیدیم', 'می‌دیدید', 'می‌دیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پایا.
+        """
+        return ["می‌" + x for x in self.perfective_past(ri)]
+
+    def negative_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_past('دید')
+            ['نمی‌دیدم', 'نمی‌دیدی', 'نمی‌دید', 'نمی‌دیدیم', 'نمی‌دیدید', 'نمی‌دیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_past(ri)]
+
+    def passive_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_past('دید')
+            ['دیده می‌شدم', 'دیده می‌شدی', 'دیده می‌شد', 'دیده می‌شدیم', 'دیده می‌شدید', 'دیده می‌شدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_past("شد")]
+
+    def negative_passive_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_past('دید')
+            ['دیده نمی‌شدم', 'دیده نمی‌شدی', 'دیده نمی‌شد', 'دیده نمی‌شدیم', 'دیده نمی‌شدید', 'دیده نمی‌شدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_past("شد")]
+
+    def past_progresive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_progresive('دید')
+            ['داشتم می‌دیدم', 'داشتی می‌دیدی', 'داشت می‌دید', 'داشتیم می‌دیدیم', 'داشتید می‌دیدید', 'داشتند می‌دیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(self.perfective_past("داشت"), self.imperfective_past(ri))
+        ]
+
+    def passive_past_progresive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_progresive('دید')
+            ['داشتم دیده می‌شدم', 'داشتی دیده می‌شدی', 'داشت دیده می‌شد', 'داشتیم دیده می‌شدیم', 'داشتید دیده می‌شدید', 'داشتند دیده می‌شدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_past("داشت"),
+                self.passive_imperfective_past(ri),
+            )
+        ]
+
+    def present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.present_perfect('دید')
+            ['دیده‌ام', 'دیده‌ای', 'دیده است', 'دیده', 'دیده‌ایم', 'دیده‌اید', 'دیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل.
+        """
+        return [ri + x for x in ["ه‌ام", "ه‌ای", "ه است", "ه", "ه‌ایم", "ه‌اید", "ه‌اند"]]
+
+    def negative_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_present_perfect('دید')
+            ['ندیده‌ام', 'ندیده‌ای', 'ندیده است', 'ندیده', 'ندیده‌ایم', 'ندیده‌اید', 'ندیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.present_perfect(ri)]
+
+    def subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_present_perfect('دید')
+            ['دیده باشم', 'دیده باشی', 'دیده باشد', 'دیده باشیم', 'دیده باشید', 'دیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی.
+        """
+        return [ri + "ه " + x for x in self.perfective_present("باش")]
+
+    def negative_subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_present_perfect('دید')
+            ['ندیده باشم', 'ندیده باشی', 'ندیده باشد', 'ندیده باشیم', 'ندیده باشید', 'ندیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.subjunctive_present_perfect(ri)]
+
+    def grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه دستوری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.grammatical_present_perfect('دید')
+            ['دیده باشم', 'دیده باش', 'دیده باشد', 'دیده باشیم', 'دیده باشید', 'دیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری.
+        """
+        return [
+            ri + "ه " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def negative_grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه دستوری به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_grammatical_present_perfect('دید')
+            ['ندیده باشم', 'ندیده باش', 'ندیده باشد', 'ندیده باشیم', 'ندیده باشید', 'ندیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری به‌شکل منفی.
+        """
+        return [
+            "ن" + ri + "ه " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def passive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_present_perfect('دید')
+            ['دیده شده‌ام', 'دیده شده‌ای', 'دیده شده است', 'دیده شده', 'دیده شده‌ایم', 'دیده شده‌اید', 'دیده شده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.present_perfect("شد")]
+
+    def negative_passive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_present_perfect('دید')
+            ['دیده نشده‌ام', 'دیده نشده‌ای', 'دیده نشده است', 'دیده نشده', 'دیده نشده‌ایم', 'دیده نشده‌اید', 'دیده نشده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_present_perfect("شد")]
+
+    def passive_subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_present_perfect('دید')
+            ['دیده شده باشم', 'دیده شده باشی', 'دیده شده باشد', 'دیده شده باشیم', 'دیده شده باشید', 'دیده شده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.subjunctive_present_perfect("شد")]
+
+    def negative_passive_subjunctive_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_present_perfect('دید')
+            ['دیده نشده باشم', 'دیده نشده باشی', 'دیده نشده باشد', 'دیده نشده باشیم', 'دیده نشده باشید', 'دیده نشده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_subjunctive_present_perfect("شد")]
+
+    def passive_grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه دستوری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_grammatical_present_perfect('دید')
+            ['دیده شده باشم', 'دیده شده باش', 'دیده شده باشد', 'دیده شده باشیم', 'دیده شده باشید', 'دیده شده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری در حالت مجهول.
+        """
+        return [
+            ri + "ه شده " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def negative_passive_grammatical_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_grammatical_present_perfect('دید')
+            ['دیده نشده باشم', 'دیده نشده باش', 'دیده نشده باشد', 'دیده نشده باشیم', 'دیده نشده باشید', 'دیده نشده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه نشده " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def imperfective_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_present_perfect('دید')
+            ['می‌دیده‌ام', 'می‌دیده‌ای', 'می‌دیده است', 'می‌دیده', 'می‌دیده‌ایم', 'می‌دیده‌اید', 'می‌دیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا.
+        """
+        return ["می‌" + x for x in self.present_perfect(ri)]
+
+    def negative_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_present_perfect('دید')
+            ['نمی‌دیده‌ام', 'نمی‌دیده‌ای', 'نمی‌دیده است', 'نمی‌دیده', 'نمی‌دیده‌ایم', 'نمی‌دیده‌اید', 'نمی‌دیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_present_perfect(ri)]
+
+    def subjunctive_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_imperfective_present_perfect('دید')
+            ['می‌دیده باشم', 'می‌دیده باشی', 'می‌دیده باشد', 'می‌دیده باشیم', 'می‌دیده باشید', 'می‌دیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی.
+        """
+        return ["می‌" + x for x in self.subjunctive_present_perfect(ri)]
+
+    def negative_subjunctive_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_imperfective_present_perfect('دید')
+            ['نمی‌دیده باشم', 'نمی‌دیده باشی', 'نمی‌دیده باشد', 'نمی‌دیده باشیم', 'نمی‌دیده باشید', 'نمی‌دیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.subjunctive_imperfective_present_perfect(ri)]
+
+    def passive_imperfective_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_present_perfect('دید')
+            ['دیده می‌شده‌ام', 'دیده می‌شده‌ای', 'دیده می‌شده است', 'دیده می‌شده', 'دیده می‌شده‌ایم', 'دیده می‌شده‌اید', 'دیده می‌شده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_present_perfect("شد")]
+
+    def negative_passive_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_present_perfect('دید')
+            ['دیده نمی‌شده‌ام', 'دیده نمی‌شده‌ای', 'دیده نمی‌شده است', 'دیده نمی‌شده', 'دیده نمی‌شده‌ایم', 'دیده نمی‌شده‌اید', 'دیده نمی‌شده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_present_perfect("شد")]
+
+    def passive_subjunctive_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_imperfective_present_perfect('دید')
+            ['دیده می‌شده باشم', 'دیده می‌شده باشی', 'دیده می‌شده باشد', 'دیده می‌شده باشیم', 'دیده می‌شده باشید', 'دیده می‌شده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی در حالت مجهول.
+        """
+        return [
+            ri + "ه " + x for x in self.subjunctive_imperfective_present_perfect("شد")
+        ]
+
+    def negative_passive_subjunctive_imperfective_present_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_imperfective_present_perfect('دید')
+            ['دیده نمی‌شده باشم', 'دیده نمی‌شده باشی', 'دیده نمی‌شده باشد', 'دیده نمی‌شده باشیم', 'دیده نمی‌شده باشید', 'دیده نمی‌شده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x
+            for x in self.negative_subjunctive_imperfective_present_perfect("شد")
+        ]
+
+    def present_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.present_perfect_progressive('دید')
+            ['داشته‌ام می‌دیده‌ام', 'داشته‌ای می‌دیده‌ای', 'داشته است می‌دیده است', 'داشته می‌دیده', 'داشته‌ایم می‌دیده‌ایم', 'داشته‌اید می‌دیده‌اید', 'داشته‌اند می‌دیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.present_perfect("داشت"),
+                self.imperfective_present_perfect(ri),
+            )
+        ]
+
+    def passive_present_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_present_perfect_progressive('دید')
+            ['داشته‌ام دیده می‌شده‌ام', 'داشته‌ای دیده می‌شده‌ای', 'داشته است دیده می‌شده است', 'داشته دیده می‌شده', 'داشته‌ایم دیده می‌شده‌ایم', 'داشته‌اید دیده می‌شده‌اید', 'داشته‌اند دیده می‌شده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.present_perfect("داشت"),
+                self.passive_imperfective_present_perfect(ri),
+            )
+        ]
+
+    def past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_precedent('دید')
+            ['دیده بودم', 'دیده بودی', 'دیده بود', 'دیده بودیم', 'دیده بودید', 'دیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین.
+        """
+        return [ri + "ه " + x for x in self.perfective_past("بود")]
+
+    def negative_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_past_precedent('دید')
+            ['ندیده بودم', 'ندیده بودی', 'ندیده بود', 'ندیده بودیم', 'ندیده بودید', 'ندیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.past_precedent(ri)]
+
+    def passive_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_precedent('دید')
+            ['دیده شده بودم', 'دیده شده بودی', 'دیده شده بود', 'دیده شده بودیم', 'دیده شده بودید', 'دیده شده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.past_precedent("شد")]
+
+    def negative_passive_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_past_precedent('دید')
+            ['دیده نشده بودم', 'دیده نشده بودی', 'دیده نشده بود', 'دیده نشده بودیم', 'دیده نشده بودید', 'دیده نشده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_past_precedent("شد")]
+
+    def imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_past_precedent('دید')
+            ['می‌دیده بودم', 'می‌دیده بودی', 'می‌دیده بود', 'می‌دیده بودیم', 'می‌دیده بودید', 'می‌دیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا.
+        """
+        return ["می‌" + x for x in self.past_precedent(ri)]
+
+    def negative_imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_past_precedent('دید')
+            ['نمی‌دیده بودم', 'نمی‌دیده بودی', 'نمی‌دیده بود', 'نمی‌دیده بودیم', 'نمی‌دیده بودید', 'نمی‌دیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_past_precedent(ri)]
+
+    def passive_imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_past_precedent('دید')
+            ['دیده می‌شده بودم', 'دیده می‌شده بودی', 'دیده می‌شده بود', 'دیده می‌شده بودیم', 'دیده می‌شده بودید', 'دیده می‌شده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_past_precedent("شد")]
+
+    def negative_passive_imperfective_past_precedent(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_past_precedent('دید')
+            ['دیده نمی‌شده بودم', 'دیده نمی‌شده بودی', 'دیده نمی‌شده بود', 'دیده نمی‌شده بودیم', 'دیده نمی‌شده بودید', 'دیده نمی‌شده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_past_precedent("شد")]
+
+    def past_precedent_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_precedent_progressive('دید')
+            ['داشتم می‌دیده بودم', 'داشتی می‌دیده بودی', 'داشت می‌دیده بود', 'داشتیم می‌دیده بودیم', 'داشتید می‌دیده بودید', 'داشتند می‌دیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_past("داشت"),
+                self.imperfective_past_precedent(ri),
+            )
+        ]
+
+    def passive_past_precedent_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_precedent_progressive('دید')
+            ['داشتم دیده می‌شده بودم', 'داشتی دیده می‌شده بودی', 'داشت دیده می‌شده بود', 'داشتیم دیده می‌شده بودیم', 'داشتید دیده می‌شده بودید', 'داشتند دیده می‌شده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_past("داشت"),
+                self.passive_imperfective_past_precedent(ri),
+            )
+        ]
+
+    def past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_precedent_perfect('دید')
+            ['دیده بوده‌ام', 'دیده بوده‌ای', 'دیده بوده است', 'دیده بوده', 'دیده بوده‌ایم', 'دیده بوده‌اید', 'دیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل.
+        """
+        return [ri + "ه " + x for x in self.present_perfect("بود")]
+
+    def negative_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_past_precedent_perfect('دید')
+            ['ندیده بوده‌ام', 'ندیده بوده‌ای', 'ندیده بوده است', 'ندیده بوده', 'ندیده بوده‌ایم', 'ندیده بوده‌اید', 'ندیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.past_precedent_perfect(ri)]
+
+    def subjunctive_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_past_precedent_perfect('دید')
+            ['دیده بوده باشم', 'دیده بوده باشی', 'دیده بوده باشد', 'دیده بوده باشیم', 'دیده بوده باشید', 'دیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی.
+        """
+        return [ri + "ه " + x for x in self.subjunctive_present_perfect("بود")]
+
+    def negative_subjunctive_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_past_precedent_perfect('دید')
+            ['ندیده بوده باشم', 'ندیده بوده باشی', 'ندیده بوده باشد', 'ندیده بوده باشیم', 'ندیده بوده باشید', 'ندیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.subjunctive_past_precedent_perfect(ri)]
+
+    def grammatical_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.grammatical_past_precedent_perfect('دید')
+            ['دیده بوده باشم', 'دیده بوده باش', 'دیده بوده باشد', 'دیده بوده باشیم', 'دیده بوده باشید', 'دیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری.
+        """
+        return [
+            ri + "ه بوده " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def negative_grammatical_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_grammatical_past_precedent_perfect('دید')
+            ['ندیده بوده باشم', 'ندیده بوده باش', 'ندیده بوده باشد', 'ندیده بوده باشیم', 'ندیده بوده باشید', 'ندیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.grammatical_past_precedent_perfect(ri)]
+
+    def passive_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_precedent_perfect('دید')
+            ['دیده شده بوده‌ام', 'دیده شده بوده‌ای', 'دیده شده بوده است', 'دیده شده بوده', 'دیده شده بوده‌ایم', 'دیده شده بوده‌اید', 'دیده شده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.past_precedent_perfect("شد")]
+
+    def negative_passive_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_past_precedent_perfect('دید')
+            ['دیده نشده بوده‌ام', 'دیده نشده بوده‌ای', 'دیده نشده بوده است', 'دیده نشده بوده', 'دیده نشده بوده‌ایم', 'دیده نشده بوده‌اید', 'دیده نشده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_past_precedent_perfect("شد")]
+
+    def passive_subjunctive_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_past_precedent_perfect('دید')
+            ['دیده شده بوده باشم', 'دیده شده بوده باشی', 'دیده شده بوده باشد', 'دیده شده بوده باشیم', 'دیده شده بوده باشید', 'دیده شده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.subjunctive_past_precedent_perfect("شد")]
+
+    def negative_passive_subjunctive_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_past_precedent_perfect('دید')
+            ['دیده نشده بوده باشم', 'دیده نشده بوده باشی', 'دیده نشده بوده باشد', 'دیده نشده بوده باشیم', 'دیده نشده بوده باشید', 'دیده نشده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + "ن" + x for x in self.subjunctive_past_precedent_perfect("شد")
+        ]
+
+    def passive_grammatical_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_grammatical_past_precedent_perfect('دید')
+            ['دیده شده بوده باشم', 'دیده شده بوده باش', 'دیده شده بوده باشد', 'دیده شده بوده باشیم', 'دیده شده بوده باشید', 'دیده شده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.grammatical_past_precedent_perfect("شد")]
+
+    def negative_passive_grammatical_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_grammatical_past_precedent_perfect('دید')
+            ['دیده نشده بوده باشم', 'دیده نشده بوده باش', 'دیده نشده بوده باشد', 'دیده نشده بوده باشیم', 'دیده نشده بوده باشید', 'دیده نشده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x
+            for x in self.negative_grammatical_past_precedent_perfect("شد")
+        ]
+
+    def imperfective_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_past_precedent_perfect('دید')
+            ['می‌دیده بوده‌ام', 'می‌دیده بوده‌ای', 'می‌دیده بوده است', 'می‌دیده بوده', 'می‌دیده بوده‌ایم', 'می‌دیده بوده‌اید', 'می‌دیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا.
+        """
+        return ["می‌" + x for x in self.past_precedent_perfect(ri)]
+
+    def negative_imperfective_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_past_precedent_perfect('دید')
+            ['نمی‌دیده بوده‌ام', 'نمی‌دیده بوده‌ای', 'نمی‌دیده بوده است', 'نمی‌دیده بوده', 'نمی‌دیده بوده‌ایم', 'نمی‌دیده بوده‌اید', 'نمی‌دیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_past_precedent_perfect(ri)]
+
+    def subjunctive_imperfective_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_imperfective_past_precedent_perfect('دید')
+            ['می‌دیده بوده باشم', 'می‌دیده بوده باشی', 'می‌دیده بوده باشد', 'می‌دیده بوده باشیم', 'می‌دیده بوده باشید', 'می‌دیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی.
+        """
+        return ["می‌" + x for x in self.subjunctive_past_precedent_perfect(ri)]
+
+    def negative_subjunctive_imperfective_past_precedent_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_imperfective_past_precedent_perfect('دید')
+            ['نمی‌دیده بوده باشم', 'نمی‌دیده بوده باشی', 'نمی‌دیده بوده باشد', 'نمی‌دیده بوده باشیم', 'نمی‌دیده بوده باشید', 'نمی‌دیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی به‌شکل منفی.
+        """
+        return [
+            "ن" + x for x in self.subjunctive_imperfective_past_precedent_perfect(ri)
+        ]
+
+    def passive_imperfective_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_past_precedent_perfect('دید')
+            ['دیده می‌شده بوده‌ام', 'دیده می‌شده بوده‌ای', 'دیده می‌شده بوده است', 'دیده می‌شده بوده', 'دیده می‌شده بوده‌ایم', 'دیده می‌شده بوده‌اید', 'دیده می‌شده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_past_precedent_perfect("شد")]
+
+    def negative_passive_imperfective_past_precedent_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_past_precedent_perfect('دید')
+            ['دیده نمی‌شده بوده‌ام', 'دیده نمی‌شده بوده‌ای', 'دیده نمی‌شده بوده است', 'دیده نمی‌شده بوده', 'دیده نمی‌شده بوده‌ایم', 'دیده نمی‌شده بوده‌اید', 'دیده نمی‌شده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x
+            for x in self.negative_imperfective_past_precedent_perfect("شد")
+        ]
+
+    def passive_subjunctive_imperfective_past_precedent_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_imperfective_past_precedent_perfect('دید')
+            ['دیده می‌شده بوده باشم', 'دیده می‌شده بوده باشی', 'دیده می‌شده بوده باشد', 'دیده می‌شده بوده باشیم', 'دیده می‌شده بوده باشید', 'دیده می‌شده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول.
+        """
+        return [
+            ri + "ه " + x
+            for x in self.subjunctive_imperfective_past_precedent_perfect("شد")
+        ]
+
+    def negative_passive_subjunctive_imperfective_past_precedent_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_imperfective_past_precedent_perfect('دید')
+            ['دیده نمی‌شده بوده باشم', 'دیده نمی‌شده بوده باشی', 'دیده نمی‌شده بوده باشد', 'دیده نمی‌شده بوده باشیم', 'دیده نمی‌شده بوده باشید', 'دیده نمی‌شده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + "ن" + x
+            for x in self.subjunctive_imperfective_past_precedent_perfect("شد")
+        ]
+
+    def past_precedent_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_precedent_perfect_progressive('دید')
+            ['داشته‌ام می‌دیده بوده‌ام', 'داشته‌ای می‌دیده بوده‌ای', 'داشته است می‌دیده بوده است', 'داشته می‌دیده بوده', 'داشته‌ایم می‌دیده بوده‌ایم', 'داشته‌اید می‌دیده بوده‌اید', 'داشته‌اند می‌دیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.present_perfect("داشت"),
+                self.imperfective_past_precedent_perfect(ri),
+            )
+        ]
+
+    def passive_past_precedent_perfect_progressive(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_precedent_perfect_progressive('دید')
+            ['داشته‌ام دیده می‌شده بوده‌ام', 'داشته‌ای دیده می‌شده بوده‌ای', 'داشته است دیده می‌شده بوده است', 'داشته دیده می‌شده بوده', 'داشته‌ایم دیده می‌شده بوده‌ایم', 'داشته‌اید دیده می‌شده بوده‌اید', 'داشته‌اند دیده می‌شده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.present_perfect("داشت"),
+                self.passive_imperfective_past_precedent_perfect(ri),
+            )
+        ]
+
+    def perfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال مطلق صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.perfective_present('بین')
+            ['بینم', 'بینی', 'بیند', 'بینیم', 'بینید', 'بینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق.
+        """
+        return [rii + x for x in ["م", "ی", "د", "یم", "ید", "ند"]]
+
+    def negative_perfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال مطلق به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_perfective_present('بین')
+            ['نبینم', 'نبینی', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.perfective_present(rii)]
+
+    def subjunctive_perfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_perfective_present('بین')
+            ['ببینم', 'ببینی', 'ببیند', 'ببینیم', 'ببینید', 'ببینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی.
+        """
+        return ["ب" + x for x in self.perfective_present(rii)]
+
+    def negative_subjunctive_perfective_present(
+        self: "Conjugation", rii: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_perfective_present('بین')
+            ['نبینم', 'نبینی', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.perfective_present(rii)]
+
+    def grammatical_perfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه دستوری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.grammatical_perfective_present('بین')
+            ['ببینم', 'ببین', 'ببیند', 'ببینیم', 'ببینید', 'ببینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری.
+        """
+        return [
+            "ببین" if x == "ببینی" else x
+            for x in self.subjunctive_perfective_present(rii)
+        ]
+
+    def negative_grammatical_perfective_present(
+        self: "Conjugation", rii: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه دستوری به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_grammatical_perfective_present('بین')
+            ['نبینم', 'نبین', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری به‌شکل منفی.
+        """
+        return [
+            "ن" + ("بین" if x == "بینی" else x) for x in self.perfective_present(rii)
+        ]
+
+    def passive_perfective_present(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال مطلق در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_perfective_present('دید')
+            ['دیده شوم', 'دیده شوی', 'دیده شود', 'دیده شویم', 'دیده شوید', 'دیده شوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.perfective_present("شو")]
+
+    def negative_passive_perfective_present(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_perfective_present('دید')
+            ['دیده نشوم', 'دیده نشوی', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_perfective_present("شو")]
+
+    def passive_subjunctive_perfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_perfective_present('دید')
+            ['دیده بشوم', 'دیده بشوی', 'دیده بشود', 'دیده بشویم', 'دیده بشوید', 'دیده بشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.subjunctive_perfective_present("شو")]
+
+    def negative_passive_subjunctive_perfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_perfective_present('دید')
+            ['دیده نشوم', 'دیده نشوی', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x for x in self.negative_subjunctive_perfective_present("شو")
+        ]
+
+    def passive_grammatical_perfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه دستوری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_grammatical_perfective_present('دید')
+            ['دیده بشوم', 'دیده بشو', 'دیده بشود', 'دیده بشویم', 'دیده بشوید', 'دیده بشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری در حالت مجهول.
+        """
+        return [
+            ri + "ه " + ("بشو" if x == "بشوی" else x)
+            for x in self.grammatical_perfective_present("شو")
+        ]
+
+    def negative_passive_grammatical_perfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_grammatical_perfective_present('دید')
+            ['دیده نشوم', 'دیده نشو', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + ("نشو" if x == "نشوی" else x)
+            for x in self.negative_grammatical_perfective_present("شو")
+        ]
+
+    def imperfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_present('بین')
+            ['می‌بینم', 'می‌بینی', 'می‌بیند', 'می‌بینیم', 'می‌بینید', 'می‌بینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال پایا.
+        """
+        return ["می‌" + x for x in self.perfective_present(rii)]
+
+    def negative_imperfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_present('بین')
+            ['نمی‌بینم', 'نمی‌بینی', 'نمی‌بیند', 'نمی‌بینیم', 'نمی‌بینید', 'نمی‌بینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_present(rii)]
+
+    def passive_imperfective_present(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_present('دید')
+            ['دیده می‌شوم', 'دیده می‌شوی', 'دیده می‌شود', 'دیده می‌شویم', 'دیده می‌شوید', 'دیده می‌شوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_present("شو")]
+
+    def negative_passive_imperfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_present('دید')
+            ['دیده نمی‌شوم', 'دیده نمی‌شوی', 'دیده نمی‌شود', 'دیده نمی‌شویم', 'دیده نمی‌شوید', 'دیده نمی‌شوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_present("شو")]
+
+    def present_progressive(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.present_progressive('بین')
+            ['دارم می‌بینم', 'داری می‌بینی', 'دارد می‌بیند', 'داریم می‌بینیم', 'دارید می‌بینید', 'دارند می‌بینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_present("دار"),
+                self.imperfective_present(rii),
+            )
+        ]
+
+    def passive_present_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_present_progressive('دید')
+            ['دارم دیده می‌شوم', 'داری دیده می‌شوی', 'دارد دیده می‌شود', 'داریم دیده می‌شویم', 'دارید دیده می‌شوید', 'دارند دیده می‌شوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_present("دار"),
+                self.passive_imperfective_present(ri),
+            )
+        ]
+
+    def perfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ مطلق صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.perfective_future('دید')
+            ['خواهم دید', 'خواهی دید', 'خواهد دید', 'خواهیم دید', 'خواهید دید', 'خواهند دید']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ مطلق.
+        """
+        return [x + " " + ri for x in self.perfective_present("خواه")]
+
+    def negative_perfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ مطلق به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_perfective_future('دید')
+            ['نخواهم دید', 'نخواهی دید', 'نخواهد دید', 'نخواهیم دید', 'نخواهید دید', 'نخواهند دید']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ مطلق به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.perfective_future(ri)]
+
+    def passive_perfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ مطلق در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_perfective_future('دید')
+            ['دیده خواهم شد', 'دیده خواهی شد', 'دیده خواهد شد', 'دیده خواهیم شد', 'دیده خواهید شد', 'دیده خواهند شد']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ مطلق در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.perfective_future("شد")]
+
+    def negative_passive_perfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_perfective_future('دید')
+            ['دیده نخواهم شد', 'دیده نخواهی شد', 'دیده نخواهد شد', 'دیده نخواهیم شد', 'دیده نخواهید شد', 'دیده نخواهند شد']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ مطلق در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_perfective_future("شد")]
+
+    def imperfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_future('دید')
+            ['می‌خواهم دید', 'می‌خواهی دید', 'می‌خواهد دید', 'می‌خواهیم دید', 'می‌خواهید دید', 'می‌خواهند دید']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پایا.
+        """
+        return ["می‌" + x for x in self.perfective_future(ri)]
+
+    def negative_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_future('دید')
+            ['نمی‌خواهم دید', 'نمی‌خواهی دید', 'نمی‌خواهد دید', 'نمی‌خواهیم دید', 'نمی‌خواهید دید', 'نمی‌خواهند دید']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_future(ri)]
+
+    def passive_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_future('دید')
+            ['دیده می‌خواهم شد', 'دیده می‌خواهی شد', 'دیده می‌خواهد شد', 'دیده می‌خواهیم شد', 'دیده می‌خواهید شد', 'دیده می‌خواهند شد']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_future("شد")]
+
+    def negative_passive_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_future('دید')
+            ['دیده نمی‌خواهم شد', 'دیده نمی‌خواهی شد', 'دیده نمی‌خواهد شد', 'دیده نمی‌خواهیم شد', 'دیده نمی‌خواهید شد', 'دیده نمی‌خواهند شد']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_future("شد")]
+
+    def future_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.future_precedent('دید')
+            ['دیده خواهم بود', 'دیده خواهی بود', 'دیده خواهد بود', 'دیده خواهیم بود', 'دیده خواهید بود', 'دیده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین.
+        """
+        return [ri + "ه " + x for x in self.perfective_future("بود")]
+
+    def negative_future_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_future_precedent('دید')
+            ['ندیده خواهم بود', 'ندیده خواهی بود', 'ندیده خواهد بود', 'ندیده خواهیم بود', 'ندیده خواهید بود', 'ندیده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.future_precedent(ri)]
+
+    def passive_future_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_future_precedent('دید')
+            ['دیده شده خواهم بود', 'دیده شده خواهی بود', 'دیده شده خواهد بود', 'دیده شده خواهیم بود', 'دیده شده خواهید بود', 'دیده شده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.future_precedent("شد")]
+
+    def negative_passive_future_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_future_precedent('دید')
+            ['دیده نشده خواهم بود', 'دیده نشده خواهی بود', 'دیده نشده خواهد بود', 'دیده نشده خواهیم بود', 'دیده نشده خواهید بود', 'دیده نشده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_future_precedent("شد")]
+
+    def future_precedent_imperfective(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.future_precedent_imperfective('دید')
+            ['می‌دیده خواهم بود', 'می‌دیده خواهی بود', 'می‌دیده خواهد بود', 'می‌دیده خواهیم بود', 'می‌دیده خواهید بود', 'می‌دیده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا.
+        """
+        return ["می‌" + x for x in self.future_precedent(ri)]
+
+    def negative_future_precedent_imperfective(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_future_precedent_imperfective('دید')
+            ['نمی‌دیده خواهم بود', 'نمی‌دیده خواهی بود', 'نمی‌دیده خواهد بود', 'نمی‌دیده خواهیم بود', 'نمی‌دیده خواهید بود', 'نمی‌دیده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.future_precedent_imperfective(ri)]
+
+    def passive_future_precedent_imperfective(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_future_precedent_imperfective('دید')
+            ['دیده می‌شده خواهم بود', 'دیده می‌شده خواهی بود', 'دیده می‌شده خواهد بود', 'دیده می‌شده خواهیم بود', 'دیده می‌شده خواهید بود', 'دیده می‌شده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.future_precedent_imperfective("شد")]
+
+    def negative_passive_future_precedent_imperfective(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_future_precedent_imperfective('دید')
+            ['دیده نمی‌شده خواهم بود', 'دیده نمی‌شده خواهی بود', 'دیده نمی‌شده خواهد بود', 'دیده نمی‌شده خواهیم بود', 'دیده نمی‌شده خواهید بود', 'دیده نمی‌شده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x for x in self.negative_future_precedent_imperfective("شد")
+        ]
+
+    def get(self: "Conjugation", verb, negative=False, passive=False) -> List[str]:
+        """صورت‌های صرفی فعل را برمی‌گرداند.
+
+        Args:
+            verb (str): فعلی که باید صرف شود. به‌صورت بن ماضی#بن مضارع؛ مانند: دید#بین.
+            negative (bool, optional): اگر `True` باشد صورت‌های صرفی منفی را برمی‌گرداند.
+            passive (bool, optional): اگر `True` باشد صورت‌های صرفی مجهول را برمی‌گرداند.
+
+        Returns:
+            (List(str)): صورت‌های صرفی فعل.
+        """
+        ri, rii = verb.split("#")
+        infinitive = [ri + "ن"]
+        result = [infinitive]
+
+        if negative and passive:
+            result.append(self.negative_passive_perfective_past(ri))
+            result.append(self.negative_passive_imperfective_past(ri))
+            result.append(self.negative_passive_present_perfect(ri))
+            result.append(self.negative_passive_subjunctive_present_perfect(ri))
+            result.append(self.negative_passive_grammatical_present_perfect(ri))
+            result.append(self.negative_passive_imperfective_present_perfect(ri))
+            result.append(
+                self.negative_passive_subjunctive_imperfective_present_perfect(ri),
+            )
+            result.append(self.negative_passive_past_precedent(ri))
+            result.append(self.negative_passive_imperfective_past_precedent(ri))
+            result.append(self.negative_passive_past_precedent_perfect(ri))
+            result.append(self.negative_passive_subjunctive_past_precedent_perfect(ri))
+            result.append(self.negative_passive_grammatical_past_precedent_perfect(ri))
+            result.append(self.negative_passive_imperfective_past_precedent_perfect(ri))
+            result.append(
+                self.negative_passive_subjunctive_imperfective_past_precedent_perfect(
+                    ri,
+                ),
+            )
+            result.append(self.negative_passive_perfective_present(ri))
+            result.append(self.negative_passive_subjunctive_perfective_present(ri))
+            result.append(self.negative_passive_grammatical_perfective_present(ri))
+            result.append(self.negative_passive_imperfective_present(ri))
+            result.append(self.negative_passive_perfective_future(ri))
+            result.append(self.negative_passive_imperfective_future(ri))
+            result.append(self.negative_passive_future_precedent(ri))
+            result.append(self.negative_passive_future_precedent_imperfective(ri))
+
+        elif passive and not negative:
+            result.append(self.passive_perfective_past(ri))
+            result.append(self.passive_imperfective_past(ri))
+            result.append(self.passive_past_progresive(ri))
+            result.append(self.passive_present_perfect(ri))
+            result.append(self.passive_subjunctive_present_perfect(ri))
+            result.append(self.passive_grammatical_present_perfect(ri))
+            result.append(self.passive_imperfective_present_perfect(ri))
+            result.append(self.passive_subjunctive_imperfective_present_perfect(ri))
+            result.append(self.passive_present_perfect_progressive(ri))
+            result.append(self.passive_past_precedent(ri))
+            result.append(self.passive_imperfective_past_precedent(ri))
+            result.append(self.passive_past_precedent_progressive(ri))
+            result.append(self.passive_past_precedent_perfect(ri))
+            result.append(self.passive_subjunctive_past_precedent_perfect(ri))
+            result.append(self.passive_grammatical_past_precedent_perfect(ri))
+            result.append(self.passive_imperfective_past_precedent_perfect(ri))
+            result.append(
+                self.passive_subjunctive_imperfective_past_precedent_perfect(ri),
+            )
+            result.append(self.passive_past_precedent_perfect_progressive(ri))
+            result.append(self.passive_perfective_present(ri))
+            result.append(self.passive_subjunctive_perfective_present(ri))
+            result.append(self.passive_grammatical_perfective_present(ri))
+            result.append(self.passive_imperfective_present(ri))
+            result.append(self.passive_present_progressive(ri))
+            result.append(self.passive_perfective_future(ri))
+            result.append(self.passive_imperfective_future(ri))
+            result.append(self.passive_future_precedent(ri))
+            result.append(self.passive_future_precedent_imperfective(ri))
+
+        elif negative and not passive:
+            result.append(self.negative_perfective_past(ri))
+            result.append(self.negative_imperfective_past(ri))
+            result.append(self.negative_present_perfect(ri))
+            result.append(self.negative_subjunctive_present_perfect(ri))
+            result.append(self.negative_grammatical_present_perfect(ri))
+            result.append(self.negative_imperfective_present_perfect(ri))
+            result.append(self.negative_subjunctive_imperfective_present_perfect(ri))
+            result.append(self.negative_past_precedent(ri))
+            result.append(self.negative_imperfective_past_precedent(ri))
+            result.append(self.negative_past_precedent_perfect(ri))
+            result.append(self.negative_subjunctive_past_precedent_perfect(ri))
+            result.append(self.negative_grammatical_past_precedent_perfect(ri))
+            result.append(self.negative_imperfective_past_precedent_perfect(ri))
+            result.append(
+                self.negative_subjunctive_imperfective_past_precedent_perfect(ri),
+            )
+            result.append(self.negative_perfective_present(rii))
+            result.append(self.negative_subjunctive_perfective_present(rii))
+            result.append(self.negative_grammatical_perfective_present(rii))
+            result.append(self.negative_imperfective_present(rii))
+            result.append(self.negative_perfective_future(ri))
+            result.append(self.negative_imperfective_future(ri))
+            result.append(self.negative_future_precedent(ri))
+            result.append(self.negative_future_precedent_imperfective(ri))
+
+        elif not negative and not passive:
+            result.append(self.perfective_past(ri))
+            result.append(self.imperfective_past(ri))
+            result.append(self.past_progresive(ri))
+            result.append(self.present_perfect(ri))
+            result.append(self.subjunctive_present_perfect(ri))
+            result.append(self.grammatical_present_perfect(ri))
+            result.append(self.imperfective_present_perfect(ri))
+            result.append(self.subjunctive_imperfective_present_perfect(ri))
+            result.append(self.present_perfect_progressive(ri))
+            result.append(self.past_precedent(ri))
+            result.append(self.imperfective_past_precedent(ri))
+            result.append(self.past_precedent_progressive(ri))
+            result.append(self.past_precedent_perfect(ri))
+            result.append(self.subjunctive_past_precedent_perfect(ri))
+            result.append(self.grammatical_past_precedent_perfect(ri))
+            result.append(self.imperfective_past_precedent_perfect(ri))
+            result.append(self.subjunctive_imperfective_past_precedent_perfect(ri))
+            result.append(self.past_precedent_perfect_progressive(ri))
+            result.append(self.perfective_present(rii))
+            result.append(self.subjunctive_perfective_present(rii))
+            result.append(self.grammatical_perfective_present(rii))
+            result.append(self.imperfective_present(rii))
+            result.append(self.present_progressive(rii))
+            result.append(self.perfective_future(ri))
+            result.append(self.imperfective_future(ri))
+            result.append(self.future_precedent(ri))
+            result.append(self.future_precedent_imperfective(ri))
+
+        return sum(result, [])
+
+    def get_all(self: "Conjugation", verb: str) -> List[str]:
+        """تمام صورت‌های صرفی فعل را در وجوه اخباری، التزامی، دستوری و در اشکال منفی و مثبت و مجهول برمی‌گرداند.
+
+        Args:
+            verb (str): فعلی که باید صرف شود. به‌صورت بن ماضی#بن مضارع؛ مانند: دید#بین.
+
+        Returns:
+             لیست تمام صورت‌های صرفی فعل.
+        """
+        ri, rii = verb.split("#")
+        infinitive = [ri + "ن"]
+        result = [infinitive]
+
+        # گذشتهٔ مطلق
+        result.append(self.perfective_past(ri))
+
+        # گذشتهٔ مطلق منفی
+        result.append(self.negative_perfective_past(ri))
+
+        # گذشتهٔ مطلق مجهول
+        result.append(self.passive_perfective_past(ri))
+
+        # گذشتهٔ مطلق مجهول منفی
+        result.append(self.negative_passive_perfective_past(ri))
+
+        # گذشتهٔ پایا
+        result.append(self.imperfective_past(ri))
+
+        # گذشتهٔ پایای منفی
+        result.append(self.negative_imperfective_past(ri))
+
+        # گذشتهٔ پایای مجهول
+        result.append(self.passive_imperfective_past(ri))
+
+        # گذشتهٔ پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_past(ri))
+
+        # گذشتهٔ استمراری
+        result.append(self.past_progresive(ri))
+
+        # گذشتهٔ استمراری مجهول
+        result.append(self.passive_past_progresive(ri))
+
+        # حال کامل
+        result.append(self.present_perfect(ri))
+
+        # حال کامل منفی
+        result.append(self.negative_present_perfect(ri))
+
+        # حال کامل التزامی
+        result.append(self.subjunctive_present_perfect(ri))
+
+        # حال کامل التزامی منفی
+        result.append(self.negative_subjunctive_present_perfect(ri))
+
+        # حال کامل دستوری
+        result.append(self.grammatical_present_perfect(ri))
+
+        # حال کامل دستوری منفی
+        result.append(self.negative_grammatical_present_perfect(ri))
+
+        # حال کامل مجهول
+        result.append(self.passive_present_perfect(ri))
+
+        # حال کامل مجهول منفی
+        result.append(self.negative_passive_present_perfect(ri))
+
+        # حال کامل التزامی مجهول
+        result.append(self.passive_subjunctive_present_perfect(ri))
+
+        # حال کامل التزامی مجهول منفی
+        result.append(self.negative_passive_subjunctive_present_perfect(ri))
+
+        # حال کامل دستوری مجهول
+        result.append(self.passive_grammatical_present_perfect(ri))
+
+        # حال کامل دستوری مجهول منفی
+        result.append(self.negative_passive_grammatical_present_perfect(ri))
+
+        # حال کامل پایا
+        result.append(self.imperfective_present_perfect(ri))
+
+        # حال کامل پایای منفی
+        result.append(self.negative_imperfective_present_perfect(ri))
+
+        # حال کامل پایای التزامی
+        result.append(self.subjunctive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای التزامی منفی
+        result.append(self.negative_subjunctive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای مجهول
+        result.append(self.passive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای التزامی مجهول
+        result.append(self.passive_subjunctive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای التزامی مجهول منفی
+        result.append(
+            self.negative_passive_subjunctive_imperfective_present_perfect(ri),
+        )
+
+        # حال کامل استمراری
+        result.append(self.present_perfect_progressive(ri))
+
+        # حال کامل استمراری مجهول
+        result.append(self.passive_present_perfect_progressive(ri))
+
+        # گذشتهٔ پیشین
+        result.append(self.past_precedent(ri))
+
+        # گذشتهٔ پیشین منفی
+        result.append(self.negative_past_precedent(ri))
+
+        # گذشتهٔ پیشین مجهول
+        result.append(self.passive_past_precedent(ri))
+
+        # گذشتهٔ پیشین مجهول منفی
+        result.append(self.negative_passive_past_precedent(ri))
+
+        # گذشتهٔ پیشین پایا
+        result.append(self.imperfective_past_precedent(ri))
+
+        # گذشتهٔ پیشین پایای منفی
+        result.append(self.negative_imperfective_past_precedent(ri))
+
+        # گذشتهٔ پیشین پایای مجهول
+        result.append(self.passive_imperfective_past_precedent(ri))
+
+        # گذشتهٔ پیشین پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_past_precedent(ri))
+
+        # گذشتهٔ پیشین استمراری
+        result.append(self.past_precedent_progressive(ri))
+
+        # گذشتهٔ پیشین استمراری مجهول
+        result.append(self.passive_past_precedent_progressive(ri))
+
+        # گذشتهٔ پیشین کامل
+        result.append(self.past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل منفی
+        result.append(self.negative_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل التزامی
+        result.append(self.subjunctive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل التزامی منفی
+        result.append(self.negative_subjunctive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل دستوری
+        result.append(self.grammatical_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل دستوری منفی
+        result.append(self.negative_grammatical_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل مجهول
+        result.append(self.passive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل مجهول منفی
+        result.append(self.negative_passive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل التزامی مجهول
+        result.append(self.passive_subjunctive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل التزامی مجهول منفی
+        result.append(self.negative_passive_subjunctive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشن کامل دستوری مجهول
+        result.append(self.passive_grammatical_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل دستوری مجهول منفی
+        result.append(self.negative_passive_grammatical_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایا
+        result.append(self.imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای منفی
+        result.append(self.negative_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای التزامی
+        result.append(self.subjunctive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای التزامی منفی
+        result.append(self.negative_subjunctive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای مجهول
+        result.append(self.passive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای التزامی مجهول
+        result.append(self.passive_subjunctive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای التزامی مجهول منفی
+        result.append(
+            self.negative_passive_subjunctive_imperfective_past_precedent_perfect(ri),
+        )
+
+        # گذشتهٔ پیشین کامل استمراری
+        result.append(self.past_precedent_perfect_progressive(ri))
+
+        # گذشتهٔ پیشین کامل استمراری مجهول
+        result.append(self.passive_past_precedent_perfect_progressive(ri))
+
+        # حال مطلق
+        result.append(self.perfective_present(rii))
+
+        # حال مطلق منفی
+        result.append(self.negative_perfective_present(rii))
+
+        # حال مطلق التزامی
+        result.append(self.subjunctive_perfective_present(rii))
+
+        # حال مطلق التزامی منفی
+        result.append(self.negative_subjunctive_perfective_present(rii))
+
+        # حال مطلق دستوری
+        result.append(self.grammatical_perfective_present(rii))
+
+        # حال مطلق دستوری منفی
+        result.append(self.negative_grammatical_perfective_present(rii))
+
+        # حال مطلق مجهول
+        result.append(self.passive_perfective_present(ri))
+
+        # حال مطلق مجهول منفی
+        result.append(self.negative_passive_perfective_present(ri))
+
+        # حال مطلق التزامی مجهول
+        result.append(self.passive_subjunctive_perfective_present(ri))
+
+        # حال مطلق التزامی مجهول منفی
+        result.append(self.negative_passive_subjunctive_perfective_present(ri))
+
+        # حال مطلق دستوری مجهول
+        result.append(self.passive_grammatical_perfective_present(ri))
+
+        # حال مطلق دستوری مجهول منفی
+        result.append(self.negative_passive_grammatical_perfective_present(ri))
+
+        # حال پایا
+        result.append(self.imperfective_present(rii))
+
+        # حال پایای منفی
+        result.append(self.negative_imperfective_present(rii))
+
+        # حال پایای مجهول
+        result.append(self.passive_imperfective_present(ri))
+
+        # حال پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_present(ri))
+
+        # حال استمراری
+        result.append(self.present_progressive(rii))
+
+        # حال استمراری مجهول
+        result.append(self.passive_present_progressive(ri))
+
+        # آیندهٔ مطلق
+        result.append(self.perfective_future(ri))
+
+        # آیندهٔ مطلق منفی
+        result.append(self.negative_perfective_future(ri))
+
+        # آیندهٔ مطلق مجهول
+        result.append(self.passive_perfective_future(ri))
+
+        # آیندهٔ مطلق مجهول منفی
+        result.append(self.negative_passive_perfective_future(ri))
+
+        # آیندهٔ پایا
+        result.append(self.imperfective_future(ri))
+
+        # آیندهٔ پایای منفی
+        result.append(self.negative_imperfective_future(ri))
+
+        # آیندهٔ پایای مجهول
+        result.append(self.passive_imperfective_future(ri))
+
+        # آیندهٔ پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_future(ri))
+
+        # آیندهٔ پیشین
+        result.append(self.future_precedent(ri))
+
+        # آیندهٔ پیشین منفی
+        result.append(self.negative_future_precedent(ri))
+
+        # آیندهٔ پیشین مجهول
+        result.append(self.passive_future_precedent(ri))
+
+        # آیندهٔ پیشین مجهول منفی
+        result.append(self.negative_passive_future_precedent(ri))
+
+        # آیندهٔ پیشین پایا
+        result.append(self.future_precedent_imperfective(ri))
+
+        # آیندهٔ پیشین پایای منفی
+        result.append(self.negative_future_precedent_imperfective(ri))
+
+        # آیندهٔ پیشین پایای مجهول
+        result.append(self.passive_future_precedent_imperfective(ri))
+
+        # آیندهٔ پیشین پایای مجهول منفی
+        result.append(self.negative_passive_future_precedent_imperfective(ri))
+
+        return sum(result, [])
```

### Comparing `hazm-0.9.0/hazm/normalizer.py` & `hazm-0.9.1/hazm/normalizer.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,535 +1,535 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای نرمال‌سازی متن است."""
-
-
-import re
-from typing import List
-
-from hazm import Lemmatizer
-from hazm import maketrans
-from hazm import regex_replace
-from hazm import WordTokenizer
-
-
-class Normalizer:
-    """این کلاس شامل توابعی برای نرمال‌سازی متن است.
-
-    Args:
-        correct_spacing: اگر `True‍` فاصله‌گذاری‌ها را در متن، نشانه‌های سجاوندی و پیشوندها و پسوندها اصلاح می‌کند.
-        remove_diacritics: اگر `True` باشد اعرابِ حروف را حذف می‌کند.
-        remove_specials_chars: اگر `True` باشد برخی از کاراکترها و نشانه‌های خاص را که کاربردی در پردازش متن ندارند حذف می‌کند.
-        decrease_repeated_chars: اگر `True` باشد تکرارهای بیش از ۲ بار را به ۲ بار کاهش می‌دهد. مثلاً «سلاممم» را به «سلامم» تبدیل می‌کند.
-        persian_style: اگر `True` باشد اصلاحات مخصوص زبان فارسی را انجام می‌دهد؛ مثلاً جایگزین‌کردن کوتیشن با گیومه.
-        persian_numbers: اگر `True` باشد ارقام انگلیسی را با فارسی جایگزین می‌کند.
-        unicodes_replacement: اگر `True` باشد برخی از کاراکترهای یونیکد را با معادل نرمال‌شدهٔ آن جایگزین می‌کند.
-        seperate_mi: اگر `True` باشد پیشوند «می» و «نمی» را در افعال جدا می‌کند.
-
-    """
-
-    def __init__(
-        self: "Normalizer",
-        correct_spacing: bool = True,
-        remove_diacritics: bool = True,
-        remove_specials_chars: bool = True,
-        decrease_repeated_chars: bool = True,
-        persian_style: bool = True,
-        persian_numbers: bool = True,
-        unicodes_replacement: bool = True,
-        seperate_mi: bool = True,
-    ) -> None:
-        self._correct_spacing = correct_spacing
-        self._remove_diacritics = remove_diacritics
-        self._remove_specials_chars = remove_specials_chars
-        self._decrease_repeated_chars = decrease_repeated_chars
-        self._persian_style = persian_style
-        self._persian_number = persian_numbers
-        self._unicodes_replacement = unicodes_replacement
-        self._seperate_mi = seperate_mi
-
-        self.translation_src = "ؠػػؽؾؿكيٮٯٷٸٹٺٻټٽٿڀځٵٶٷٸٹٺٻټٽٿڀځڂڅڇڈډڊڋڌڍڎڏڐڑڒړڔڕږڗڙښڛڜڝڞڟڠڡڢڣڤڥڦڧڨڪګڬڭڮڰڱڲڳڴڵڶڷڸڹںڻڼڽھڿہۂۃۄۅۆۇۈۉۊۋۏۍێېۑےۓەۮۯۺۻۼۿݐݑݒݓݔݕݖݗݘݙݚݛݜݝݞݟݠݡݢݣݤݥݦݧݨݩݪݫݬݭݮݯݰݱݲݳݴݵݶݷݸݹݺݻݼݽݾݿࢠࢡࢢࢣࢤࢥࢦࢧࢨࢩࢪࢫࢮࢯࢰࢱࢬࢲࢳࢴࢶࢷࢸࢹࢺࢻࢼࢽﭐﭑﭒﭓﭔﭕﭖﭗﭘﭙﭚﭛﭜﭝﭞﭟﭠﭡﭢﭣﭤﭥﭦﭧﭨﭩﭮﭯﭰﭱﭲﭳﭴﭵﭶﭷﭸﭹﭺﭻﭼﭽﭾﭿﮀﮁﮂﮃﮄﮅﮆﮇﮈﮉﮊﮋﮌﮍﮎﮏﮐﮑﮒﮓﮔﮕﮖﮗﮘﮙﮚﮛﮜﮝﮞﮟﮠﮡﮢﮣﮤﮥﮦﮧﮨﮩﮪﮫﮬﮭﮮﮯﮰﮱﺀﺁﺃﺄﺅﺆﺇﺈﺉﺊﺋﺌﺍﺎﺏﺐﺑﺒﺕﺖﺗﺘﺙﺚﺛﺜﺝﺞﺟﺠﺡﺢﺣﺤﺥﺦﺧﺨﺩﺪﺫﺬﺭﺮﺯﺰﺱﺲﺳﺴﺵﺶﺷﺸﺹﺺﺻﺼﺽﺾﺿﻀﻁﻂﻃﻄﻅﻆﻇﻈﻉﻊﻋﻌﻍﻎﻏﻐﻑﻒﻓﻔﻕﻖﻗﻘﻙﻚﻛﻜﻝﻞﻟﻠﻡﻢﻣﻤﻥﻦﻧﻨﻩﻪﻫﻬﻭﻮﻯﻰﻱﻲﻳﻴىكي“” "
-        self.translation_dst = (
-            'یککیییکیبقویتتبتتتبحاوویتتبتتتبحححچدددددددددررررررررسسسصصطعففففففققکککککگگگگگللللنننننهچهههوووووووووییییییهدرشضغهبببببببححددرسعععففکککممنننلررسححسرحاایییووییحسسکببجطفقلمییرودصگویزعکبپتریفقنااببببپپپپببببتتتتتتتتتتتتففففححححححححچچچچچچچچددددددددژژررککککگگگگگگگگگگگگننننننههههههههههییییءاااووااییییااببببتتتتثثثثججججححححخخخخددذذررززسسسسششششصصصصضضضضططططظظظظععععغغغغففففققققککککللللممممننننههههوویییییییکی"" '
-        )
-
-        if self._correct_spacing or self._decrease_repeated_chars:
-            self.tokenizer = WordTokenizer(join_verb_parts=False)
-            self.words = self.tokenizer.words
-
-        if self._persian_number:
-            self.number_translation_src = "0123456789%٠١٢٣٤٥٦٧٨٩"
-            self.number_translation_dst = "۰۱۲۳۴۵۶۷۸۹٪۰۱۲۳۴۵۶۷۸۹"
-
-        if self._correct_spacing:
-            self.suffixes = {
-                "ی",
-                "ای",
-                "ها",
-                "های",
-                "تر",
-                "تری",
-                "ترین",
-                "گر",
-                "گری",
-                "ام",
-                "ات",
-                "اش",
-            }
-
-            self.extra_space_patterns = [
-                (r" {2,}", " "),  # remove extra spaces
-                (r"\n{3,}", "\n\n"),  # remove extra newlines
-                (r"\u200c{2,}", "\u200c"),  # remove extra ZWNJs
-                (r"\u200c{1,} ", " "),  # remove unneded ZWNJs before space
-                (r" \u200c{1,}", " "),  # remove unneded ZWNJs after space
-                (r"\b\u200c*\B", ""),  # remove unneded ZWNJs at the beginning of words
-                (r"\B\u200c*\b", ""),  # remove unneded ZWNJs at the end of words
-                (r"[ـ\r]", ""),  # remove keshide, carriage returns
-            ]
-
-            punc_after, punc_before = r"\.:!،؛؟»\]\)\}", r"«\[\(\{"
-
-            self.punctuation_spacing_patterns = [
-                # remove space before and after quotation
-                ('" ([^\n"]+) "', r'"\1"'),
-                (" ([" + punc_after + "])", r"\1"),  # remove space before
-                ("([" + punc_before + "]) ", r"\1"),  # remove space after
-                # put space after . and :
-                (
-                    "([" + punc_after[:3] + "])([^ " + punc_after + r"\d۰۱۲۳۴۵۶۷۸۹])",
-                    r"\1 \2",
-                ),
-                (
-                    "([" + punc_after[3:] + "])([^ " + punc_after + "])",
-                    r"\1 \2",
-                ),  # put space after
-                (
-                    "([^ " + punc_before + "])([" + punc_before + "])",
-                    r"\1 \2",
-                ),  # put space before
-                # put space after number; e.g., به طول ۹متر -> به طول ۹ متر
-                (r"(\d)([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])", r"\1 \2"),
-                # put space after number; e.g., به طول۹ -> به طول ۹
-                (r"([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])(\d)", r"\1 \2"),
-            ]
-
-            self.affix_spacing_patterns = [
-                (r"([^ ]ه) ی ", r"\1‌ی "),  # fix ی space
-                (r"(^| )(ن?می) ", r"\1\2‌"),  # put zwnj after می, نمی
-                # put zwnj before تر, تری, ترین, گر, گری, ها, های
-                (
-                    r"(?<=[^\n\d "
-                    + punc_after
-                    + punc_before
-                    + "]{2}) (تر(ین?)?|گری?|های?)(?=[ \n"
-                    + punc_after
-                    + punc_before
-                    + "]|$)",
-                    r"‌\1",
-                ),
-                # join ام, ایم, اش, اند, ای, اید, ات
-                (
-                    r"([^ ]ه) (ا(م|یم|ش|ند|ی|ید|ت))(?=[ \n" + punc_after + "]|$)",
-                    r"\1‌\2",
-                ),
-                # شنبهها => شنبه‌ها
-                ("(ه)(ها)", r"\1‌\2"),
-            ]
-
-        if self._persian_style:
-            self.persian_style_patterns = [
-                ('"([^\n"]+)"', r"«\1»"),  # replace quotation with gyoome
-                (r"([\d+])\.([\d+])", r"\1٫\2"),  # replace dot with momayez
-                (r" ?\.\.\.", " …"),  # replace 3 dots
-            ]
-
-        if self._decrease_repeated_chars:
-            self.more_than_two_repeat_pattern = (
-                r"([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])\1{2,}"
-            )
-            self.repeated_chars_pattern = (
-                r"[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]*"
-                + self.more_than_two_repeat_pattern
-                + "[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]*"
-            )
-
-        if self._remove_diacritics:
-            self.diacritics_patterns = [
-                # remove FATHATAN, DAMMATAN, KASRATAN, FATHA, DAMMA, KASRA, SHADDA, SUKUN
-                ("[\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652]", ""),
-            ]
-
-        if self._remove_specials_chars:
-            self.specials_chars_patterns = [
-                # Remove almoast all arabic unicode superscript and subscript characters in the ranges of 00600-06FF, 08A0-08FF, FB50-FDFF, and FE70-FEFF
-                (
-                    "[\u0605\u0653\u0654\u0655\u0656\u0657\u0658\u0659\u065a\u065b\u065c\u065d\u065e\u065f\u0670\u0610\u0611\u0612\u0613\u0614\u0615\u0616\u0618\u0619\u061a\u061e\u06d4\u06d6\u06d7\u06d8\u06d9\u06da\u06db\u06dc\u06dd\u06de\u06df\u06e0\u06e1\u06e2\u06e3\u06e4\u06e5\u06e6\u06e7\u06e8\u06e9\u06ea\u06eb\u06ec\u06ed\u06fd\u06fe\u08ad\u08d4\u08d5\u08d6\u08d7\u08d8\u08d9\u08da\u08db\u08dc\u08dd\u08de\u08df\u08e0\u08e1\u08e2\u08e3\u08e4\u08e5\u08e6\u08e7\u08e8\u08e9\u08ea\u08eb\u08ec\u08ed\u08ee\u08ef\u08f0\u08f1\u08f2\u08f3\u08f4\u08f5\u08f6\u08f7\u08f8\u08f9\u08fa\u08fb\u08fc\u08fd\u08fe\u08ff\ufbb2\ufbb3\ufbb4\ufbb5\ufbb6\ufbb7\ufbb8\ufbb9\ufbba\ufbbb\ufbbc\ufbbd\ufbbe\ufbbf\ufbc0\ufbc1\ufc5e\ufc5f\ufc60\ufc61\ufc62\ufc63\ufcf2\ufcf3\ufcf4\ufd3e\ufd3f\ufe70\ufe71\ufe72\ufe76\ufe77\ufe78\ufe79\ufe7a\ufe7b\ufe7c\ufe7d\ufe7e\ufe7f\ufdfa\ufdfb]",
-                    "",
-                ),
-            ]
-
-        if self._seperate_mi:
-            self.verbs = Lemmatizer(joined_verb_parts=False).verbs
-            self.joint_mi_patterns = r"\bن?می[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]+"
-
-        if self._unicodes_replacement:
-            self.replacements = [
-                ("﷽", "بسم الله الرحمن الرحیم"),
-                ("﷼", "ریال"),
-                ("(ﷰ|ﷹ)", "صلی"),
-                ("ﷲ", "الله"),
-                ("ﷳ", "اکبر"),
-                ("ﷴ", "محمد"),
-                ("ﷵ", "صلعم"),
-                ("ﷶ", "رسول"),
-                ("ﷷ", "علیه"),
-                ("ﷸ", "وسلم"),
-                ("ﻵ|ﻶ|ﻷ|ﻸ|ﻹ|ﻺ|ﻻ|ﻼ", "لا"),
-            ]
-
-    def normalize(self: "Normalizer", text: str) -> str:
-        """متن را نرمال‌سازی می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.normalize('اِعلاممممم کَرد : « زمین لرزه ای به بُزرگیِ 6 دهم ریشتر ...»')
-            'اعلام کرد: «زمین‌لرزه‌ای به بزرگی ۶ دهم ریشتر …»'
-            >>> normalizer.normalize('')
-            ''
-
-        Args:
-            text: متنی که باید نرمال‌سازی شود.
-
-        Returns:
-            متنِ نرمال‌سازی‌شده.
-
-        """
-        translations = maketrans(self.translation_src, self.translation_dst)
-        text = text.translate(translations)
-
-        if self._persian_style:
-            text = self.persian_style(text)
-
-        if self._persian_number:
-            text = self.persian_number(text)
-
-        if self._remove_diacritics:
-            text = self.remove_diacritics(text)
-
-        if self._correct_spacing:
-            text = self.correct_spacing(text)
-
-        if self._unicodes_replacement:
-            text = self.unicodes_replacement(text)
-
-        if self._remove_specials_chars:
-            text = self.remove_specials_chars(text)
-
-        if self._decrease_repeated_chars:
-            text = self.decrease_repeated_chars(text)
-
-        if self._seperate_mi:
-            text = self.seperate_mi(text)
-
-        return text
-
-    def correct_spacing(self: "Normalizer", text: str) -> str:
-        """فاصله‌گذاری‌ها را در پیشوندها و پسوندها اصلاح می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.correct_spacing("سلام   دنیا")
-            'سلام دنیا'
-            >>> normalizer.correct_spacing("به طول ۹متر و عرض۶")
-            'به طول ۹ متر و عرض ۶'
-            >>> normalizer.correct_spacing("کاروان‌‌سرا")
-            'کاروان‌سرا'
-            >>> normalizer.correct_spacing("‌سلام‌ به ‌همه‌")
-            'سلام به همه'
-            >>> normalizer.correct_spacing("سلام دنیـــا")
-            'سلام دنیا'
-            >>> normalizer.correct_spacing("جمعهها که کار نمی کنم مطالعه می کنم")
-            'جمعه‌ها که کار نمی‌کنم مطالعه می‌کنم'
-            >>> normalizer.correct_spacing(' "سلام به همه"   ')
-            '"سلام به همه"'
-            >>> normalizer.correct_spacing('')
-            ''
-
-        Args:
-            text (str): متنی که باید فاصله‌گذاری‌های آن اصلاح شود.
-
-        Returns:
-            (str): متنی با فاصله‌گذاری‌های اصلاح‌شده.
-
-
-        """
-        text = regex_replace(self.extra_space_patterns, text)
-
-        lines = text.split("\n")
-        result = []
-        for line in lines:
-            tokens = self.tokenizer.tokenize(line)
-            spaced_tokens = self.token_spacing(tokens)
-            line = " ".join(spaced_tokens)
-            result.append(line)
-
-        text = "\n".join(result)
-
-        text = regex_replace(self.affix_spacing_patterns, text)
-        text = regex_replace(self.punctuation_spacing_patterns, text)
-
-        return text
-
-    def remove_diacritics(self: "Normalizer", text: str) -> str:
-        """اِعراب را از متن حذف می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.remove_diacritics('حَذفِ اِعراب')
-            'حذف اعراب'
-            >>> normalizer.remove_diacritics('آمدند')
-            'آمدند'
-            >>> normalizer.remove_diacritics('متن بدون اعراب')
-            'متن بدون اعراب'
-            >>> normalizer.remove_diacritics('')
-            ''
-
-        Args:
-            text: متنی که باید اعراب آن حذف شود.
-
-        Returns:
-            متنی بدون اعراب.
-
-        """
-        return regex_replace(self.diacritics_patterns, text)
-
-    def remove_specials_chars(self: "Normalizer", text: str) -> str:
-        """برخی از کاراکترها و نشانه‌های خاص را که کاربردی در پردازش متن ندارند حذف
-        می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.remove_specials_chars('پیامبر اکرم ﷺ')
-            'پیامبر اکرم '
-
-        Args:
-            text: متنی که باید کاراکترها و نشانه‌های اضافهٔ آن حذف شود.
-
-        Returns:
-            متنی بدون کاراکترها و نشانه‌های اضافه.
-
-        """
-        return regex_replace(self.specials_chars_patterns, text)
-
-    def decrease_repeated_chars(self: "Normalizer", text: str) -> str:
-        """تکرارهای زائد حروف را در کلماتی مثل سلامممممم حذف می‌کند و در مواردی که
-        نمی‌تواند تشخیص دهد دست کم به دو تکرار کاهش می‌دهد.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.decrease_repeated_chars('سلامممم به همه')
-            'سلام به همه'
-            >>> normalizer.decrease_repeated_chars('سلامم به همه')
-            'سلامم به همه'
-            >>> normalizer.decrease_repeated_chars('سلامم را برسان')
-            'سلامم را برسان'
-            >>> normalizer.decrease_repeated_chars('سلاممم را برسان')
-            'سلام را برسان'
-            >>> normalizer.decrease_repeated_chars('')
-            ''
-
-        Args:
-            text: متنی که باید تکرارهای زائد آن حذف شود.
-
-        Returns:
-            متنی بدون کاراکترهای زائد یا حداقل با دو تکرار.
-
-        """
-        matches = re.finditer(self.repeated_chars_pattern, text)
-
-        for m in matches:
-            word = m.group()
-            if word not in self.words:
-                no_repeat = re.sub(self.more_than_two_repeat_pattern, r"\1", word)
-                two_repeat = re.sub(self.more_than_two_repeat_pattern, r"\1\1", word)
-
-                if (no_repeat in self.words) != (two_repeat in self.words):
-                    r = no_repeat if no_repeat in self.words else two_repeat
-                    text = text.replace(word, r)
-                else:
-                    text = text.replace(word, two_repeat)
-
-        return text
-
-    def persian_style(self: "Normalizer", text: str) -> str:
-        """برخی از حروف و نشانه‌ها را با حروف و نشانه‌های فارسی جایگزین می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.persian_style('"نرمال‌سازی"')
-            '«نرمال‌سازی»'
-            >>> normalizer.persian_style('و ...')
-            'و …'
-            >>> normalizer.persian_style('10.450')
-            '10٫450'
-            >>> normalizer.persian_style('')
-            ''
-
-        Args:
-            text: متنی که باید حروف و نشانه‌های آن با حروف و نشانه‌های فارسی جایگزین شود.
-
-        Returns:
-            متنی با حروف و نشانه‌های فارسی‌سازی شده.
-
-        """
-        return regex_replace(self.persian_style_patterns, text)
-
-    def persian_number(self: "Normalizer", text: str) -> str:
-        """اعداد لاتین و علامت % را با معادل فارسی آن جایگزین می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.persian_number('5 درصد')
-            '۵ درصد'
-            >>> normalizer.persian_number('۵ درصد')
-            '۵ درصد'
-            >>> normalizer.persian_number('')
-            ''
-
-        Args:
-            text: متنی که باید اعداد لاتین و علامت % آن با معادل فارسی جایگزین شود.
-
-        Returns:
-            متنی با اعداد و علامت ٪ فارسی.
-
-        """
-        translations = maketrans(
-            self.number_translation_src,
-            self.number_translation_dst,
-        )
-        return text.translate(translations)
-
-    def unicodes_replacement(self: "Normalizer", text: str) -> str:
-        """برخی از کاراکترهای خاص یونیکد را با معادلِ نرمال آن جایگزین می‌کند. غالباً
-        این کار فقط در مواردی صورت می‌گیرد که یک کلمه در قالب یک کاراکتر یونیکد تعریف
-        شده است.
-
-        **فهرست این کاراکترها و نسخهٔ جایگزین آن:**
-
-        |کاراکتر|نسخهٔ جایگزین|
-        |--------|------------------|
-        |﷽|بسم الله الرحمن الرحیم|
-        |﷼|ریال|
-        |ﷰ، ﷹ|صلی|
-        |ﷲ|الله|
-        |ﷳ|اکبر|
-        |ﷴ|محمد|
-        |ﷵ|صلعم|
-        |ﷶ|رسول|
-        |ﷷ|علیه|
-        |ﷸ|وسلم|
-        |ﻵ، ﻶ، ﻷ، ﻸ، ﻹ، ﻺ، ﻻ، ﻼ|لا|
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.remove_specials_chars('پیامبر اکرم ﷺ')
-            'پیامبر اکرم '
-            >>> normalizer.remove_specials_chars('')
-            ''
-
-        Args:
-            text: متنی که باید برخی از کاراکترهای یونیکد آن (جدول بالا)، با شکل استاندارد، جایگزین شود.
-
-        Returns:
-            متنی که برخی از کاراکترهای یونیکد آن با شکل استاندارد جایگزین شده است.
-
-        """
-        for old, new in self.replacements:
-            text = re.sub(old, new, text)
-
-        return text
-
-    def seperate_mi(self: "Normalizer", text: str) -> str:
-        """پیشوند «می» و «نمی» را در افعال جدا کرده و با نیم‌فاصله می‌چسباند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.seperate_mi('نمیدانم چه میگفت')
-            'نمی‌دانم چه می‌گفت'
-            >>> normalizer.seperate_mi('میز')
-            'میز'
-            >>> normalizer.seperate_mi('')
-            ''
-
-
-        Args:
-            text: متنی که باید پیشوند «می» و «نمی» در آن جدا شود.
-
-        Returns:
-            متنی با «می» و «نمی» جدا شده.
-
-        """
-        matches = re.findall(r"\bن?می[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]+", text)
-        for m in matches:
-            r = re.sub("^(ن?می)", r"\1‌", m)
-            if r in self.verbs:
-                text = text.replace(m, r)
-
-        return text
-
-    def token_spacing(self: "Normalizer", tokens: List[str]) -> List[str]:
-        """توکن‌های ورودی را به فهرستی از توکن‌های نرمال‌سازی شده تبدیل می‌کند.
-        در این فرایند ممکن است برخی از توکن‌ها به یکدیگر بچسبند؛
-        برای مثال: `['زمین', 'لرزه', 'ای']` تبدیل می‌شود به: `['زمین‌لرزه‌ای']`.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.token_spacing(['کتاب', 'ها'])
-            ['کتاب‌ها']
-            >>> normalizer.token_spacing(['او', 'می', 'رود'])
-            ['او', 'می‌رود']
-            >>> normalizer.token_spacing(['ماه', 'می', 'سال', 'جدید'])
-            ['ماه', 'می', 'سال', 'جدید']
-            >>> normalizer.token_spacing(['اخلال', 'گر'])
-            ['اخلال‌گر']
-            >>> normalizer.token_spacing(['زمین', 'لرزه', 'ای'])
-            ['زمین‌لرزه‌ای']
-            >>> normalizer.token_spacing([])
-            []
-
-        Args:
-            tokens: توکن‌هایی که باید نرمال‌سازی شود.
-
-        Returns:
-            لیستی از توکن‌های نرمال‌سازی شده به شکل `[token1, token2, ...]`.
-
-        """
-        # >>> normalizer.token_spacing(['پرداخت', 'شده', 'است'])
-
-        result = []
-        for t, token in enumerate(tokens):
-            joined = False
-
-            if result:
-                token_pair = result[-1] + "‌" + token
-                if (
-                    token_pair in self.verbs
-                    or token_pair in self.words
-                    and self.words[token_pair][0] > 0
-                ):
-                    joined = True
-
-                    if (
-                        t < len(tokens) - 1
-                        and token + "_" + tokens[t + 1] in self.verbs
-                    ):
-                        joined = False
-
-                elif token in self.suffixes and result[-1] in self.words:
-                    joined = True
-
-            if joined:
-                result.pop()
-                result.append(token_pair)
-            else:
-                result.append(token)
-
-        return result
+"""این ماژول شامل کلاس‌ها و توابعی برای نرمال‌سازی متن است."""
+
+
+import re
+from typing import List
+
+from hazm import Lemmatizer
+from hazm import maketrans
+from hazm import regex_replace
+from hazm import WordTokenizer
+
+
+class Normalizer:
+    """این کلاس شامل توابعی برای نرمال‌سازی متن است.
+
+    Args:
+        correct_spacing: اگر `True‍` فاصله‌گذاری‌ها را در متن، نشانه‌های سجاوندی و پیشوندها و پسوندها اصلاح می‌کند.
+        remove_diacritics: اگر `True` باشد اعرابِ حروف را حذف می‌کند.
+        remove_specials_chars: اگر `True` باشد برخی از کاراکترها و نشانه‌های خاص را که کاربردی در پردازش متن ندارند حذف می‌کند.
+        decrease_repeated_chars: اگر `True` باشد تکرارهای بیش از ۲ بار را به ۲ بار کاهش می‌دهد. مثلاً «سلاممم» را به «سلامم» تبدیل می‌کند.
+        persian_style: اگر `True` باشد اصلاحات مخصوص زبان فارسی را انجام می‌دهد؛ مثلاً جایگزین‌کردن کوتیشن با گیومه.
+        persian_numbers: اگر `True` باشد ارقام انگلیسی را با فارسی جایگزین می‌کند.
+        unicodes_replacement: اگر `True` باشد برخی از کاراکترهای یونیکد را با معادل نرمال‌شدهٔ آن جایگزین می‌کند.
+        seperate_mi: اگر `True` باشد پیشوند «می» و «نمی» را در افعال جدا می‌کند.
+
+    """
+
+    def __init__(
+        self: "Normalizer",
+        correct_spacing: bool = True,
+        remove_diacritics: bool = True,
+        remove_specials_chars: bool = True,
+        decrease_repeated_chars: bool = True,
+        persian_style: bool = True,
+        persian_numbers: bool = True,
+        unicodes_replacement: bool = True,
+        seperate_mi: bool = True,
+    ) -> None:
+        self._correct_spacing = correct_spacing
+        self._remove_diacritics = remove_diacritics
+        self._remove_specials_chars = remove_specials_chars
+        self._decrease_repeated_chars = decrease_repeated_chars
+        self._persian_style = persian_style
+        self._persian_number = persian_numbers
+        self._unicodes_replacement = unicodes_replacement
+        self._seperate_mi = seperate_mi
+
+        self.translation_src = "ؠػػؽؾؿكيٮٯٷٸٹٺٻټٽٿڀځٵٶٷٸٹٺٻټٽٿڀځڂڅڇڈډڊڋڌڍڎڏڐڑڒړڔڕږڗڙښڛڜڝڞڟڠڡڢڣڤڥڦڧڨڪګڬڭڮڰڱڲڳڴڵڶڷڸڹںڻڼڽھڿہۂۃۄۅۆۇۈۉۊۋۏۍێېۑےۓەۮۯۺۻۼۿݐݑݒݓݔݕݖݗݘݙݚݛݜݝݞݟݠݡݢݣݤݥݦݧݨݩݪݫݬݭݮݯݰݱݲݳݴݵݶݷݸݹݺݻݼݽݾݿࢠࢡࢢࢣࢤࢥࢦࢧࢨࢩࢪࢫࢮࢯࢰࢱࢬࢲࢳࢴࢶࢷࢸࢹࢺࢻࢼࢽﭐﭑﭒﭓﭔﭕﭖﭗﭘﭙﭚﭛﭜﭝﭞﭟﭠﭡﭢﭣﭤﭥﭦﭧﭨﭩﭮﭯﭰﭱﭲﭳﭴﭵﭶﭷﭸﭹﭺﭻﭼﭽﭾﭿﮀﮁﮂﮃﮄﮅﮆﮇﮈﮉﮊﮋﮌﮍﮎﮏﮐﮑﮒﮓﮔﮕﮖﮗﮘﮙﮚﮛﮜﮝﮞﮟﮠﮡﮢﮣﮤﮥﮦﮧﮨﮩﮪﮫﮬﮭﮮﮯﮰﮱﺀﺁﺃﺄﺅﺆﺇﺈﺉﺊﺋﺌﺍﺎﺏﺐﺑﺒﺕﺖﺗﺘﺙﺚﺛﺜﺝﺞﺟﺠﺡﺢﺣﺤﺥﺦﺧﺨﺩﺪﺫﺬﺭﺮﺯﺰﺱﺲﺳﺴﺵﺶﺷﺸﺹﺺﺻﺼﺽﺾﺿﻀﻁﻂﻃﻄﻅﻆﻇﻈﻉﻊﻋﻌﻍﻎﻏﻐﻑﻒﻓﻔﻕﻖﻗﻘﻙﻚﻛﻜﻝﻞﻟﻠﻡﻢﻣﻤﻥﻦﻧﻨﻩﻪﻫﻬﻭﻮﻯﻰﻱﻲﻳﻴىكي“” "
+        self.translation_dst = (
+            'یککیییکیبقویتتبتتتبحاوویتتبتتتبحححچدددددددددررررررررسسسصصطعففففففققکککککگگگگگللللنننننهچهههوووووووووییییییهدرشضغهبببببببححددرسعععففکککممنننلررسححسرحاایییووییحسسکببجطفقلمییرودصگویزعکبپتریفقنااببببپپپپببببتتتتتتتتتتتتففففححححححححچچچچچچچچددددددددژژررککککگگگگگگگگگگگگننننننههههههههههییییءاااووااییییااببببتتتتثثثثججججححححخخخخددذذررززسسسسششششصصصصضضضضططططظظظظععععغغغغففففققققککککللللممممننننههههوویییییییکی"" '
+        )
+
+        if self._correct_spacing or self._decrease_repeated_chars:
+            self.tokenizer = WordTokenizer(join_verb_parts=False)
+            self.words = self.tokenizer.words
+
+        if self._persian_number:
+            self.number_translation_src = "0123456789%٠١٢٣٤٥٦٧٨٩"
+            self.number_translation_dst = "۰۱۲۳۴۵۶۷۸۹٪۰۱۲۳۴۵۶۷۸۹"
+
+        if self._correct_spacing:
+            self.suffixes = {
+                "ی",
+                "ای",
+                "ها",
+                "های",
+                "تر",
+                "تری",
+                "ترین",
+                "گر",
+                "گری",
+                "ام",
+                "ات",
+                "اش",
+            }
+
+            self.extra_space_patterns = [
+                (r" {2,}", " "),  # remove extra spaces
+                (r"\n{3,}", "\n\n"),  # remove extra newlines
+                (r"\u200c{2,}", "\u200c"),  # remove extra ZWNJs
+                (r"\u200c{1,} ", " "),  # remove unneded ZWNJs before space
+                (r" \u200c{1,}", " "),  # remove unneded ZWNJs after space
+                (r"\b\u200c*\B", ""),  # remove unneded ZWNJs at the beginning of words
+                (r"\B\u200c*\b", ""),  # remove unneded ZWNJs at the end of words
+                (r"[ـ\r]", ""),  # remove keshide, carriage returns
+            ]
+
+            punc_after, punc_before = r"\.:!،؛؟»\]\)\}", r"«\[\(\{"
+
+            self.punctuation_spacing_patterns = [
+                # remove space before and after quotation
+                ('" ([^\n"]+) "', r'"\1"'),
+                (" ([" + punc_after + "])", r"\1"),  # remove space before
+                ("([" + punc_before + "]) ", r"\1"),  # remove space after
+                # put space after . and :
+                (
+                    "([" + punc_after[:3] + "])([^ " + punc_after + r"\d۰۱۲۳۴۵۶۷۸۹])",
+                    r"\1 \2",
+                ),
+                (
+                    "([" + punc_after[3:] + "])([^ " + punc_after + "])",
+                    r"\1 \2",
+                ),  # put space after
+                (
+                    "([^ " + punc_before + "])([" + punc_before + "])",
+                    r"\1 \2",
+                ),  # put space before
+                # put space after number; e.g., به طول ۹متر -> به طول ۹ متر
+                (r"(\d)([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])", r"\1 \2"),
+                # put space after number; e.g., به طول۹ -> به طول ۹
+                (r"([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])(\d)", r"\1 \2"),
+            ]
+
+            self.affix_spacing_patterns = [
+                (r"([^ ]ه) ی ", r"\1‌ی "),  # fix ی space
+                (r"(^| )(ن?می) ", r"\1\2‌"),  # put zwnj after می, نمی
+                # put zwnj before تر, تری, ترین, گر, گری, ها, های
+                (
+                    r"(?<=[^\n\d "
+                    + punc_after
+                    + punc_before
+                    + "]{2}) (تر(ین?)?|گری?|های?)(?=[ \n"
+                    + punc_after
+                    + punc_before
+                    + "]|$)",
+                    r"‌\1",
+                ),
+                # join ام, ایم, اش, اند, ای, اید, ات
+                (
+                    r"([^ ]ه) (ا(م|یم|ش|ند|ی|ید|ت))(?=[ \n" + punc_after + "]|$)",
+                    r"\1‌\2",
+                ),
+                # شنبهها => شنبه‌ها
+                ("(ه)(ها)", r"\1‌\2"),
+            ]
+
+        if self._persian_style:
+            self.persian_style_patterns = [
+                ('"([^\n"]+)"', r"«\1»"),  # replace quotation with gyoome
+                (r"([\d+])\.([\d+])", r"\1٫\2"),  # replace dot with momayez
+                (r" ?\.\.\.", " …"),  # replace 3 dots
+            ]
+
+        if self._decrease_repeated_chars:
+            self.more_than_two_repeat_pattern = (
+                r"([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])\1{2,}"
+            )
+            self.repeated_chars_pattern = (
+                r"[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]*"
+                + self.more_than_two_repeat_pattern
+                + "[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]*"
+            )
+
+        if self._remove_diacritics:
+            self.diacritics_patterns = [
+                # remove FATHATAN, DAMMATAN, KASRATAN, FATHA, DAMMA, KASRA, SHADDA, SUKUN
+                ("[\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652]", ""),
+            ]
+
+        if self._remove_specials_chars:
+            self.specials_chars_patterns = [
+                # Remove almoast all arabic unicode superscript and subscript characters in the ranges of 00600-06FF, 08A0-08FF, FB50-FDFF, and FE70-FEFF
+                (
+                    "[\u0605\u0653\u0654\u0655\u0656\u0657\u0658\u0659\u065a\u065b\u065c\u065d\u065e\u065f\u0670\u0610\u0611\u0612\u0613\u0614\u0615\u0616\u0618\u0619\u061a\u061e\u06d4\u06d6\u06d7\u06d8\u06d9\u06da\u06db\u06dc\u06dd\u06de\u06df\u06e0\u06e1\u06e2\u06e3\u06e4\u06e5\u06e6\u06e7\u06e8\u06e9\u06ea\u06eb\u06ec\u06ed\u06fd\u06fe\u08ad\u08d4\u08d5\u08d6\u08d7\u08d8\u08d9\u08da\u08db\u08dc\u08dd\u08de\u08df\u08e0\u08e1\u08e2\u08e3\u08e4\u08e5\u08e6\u08e7\u08e8\u08e9\u08ea\u08eb\u08ec\u08ed\u08ee\u08ef\u08f0\u08f1\u08f2\u08f3\u08f4\u08f5\u08f6\u08f7\u08f8\u08f9\u08fa\u08fb\u08fc\u08fd\u08fe\u08ff\ufbb2\ufbb3\ufbb4\ufbb5\ufbb6\ufbb7\ufbb8\ufbb9\ufbba\ufbbb\ufbbc\ufbbd\ufbbe\ufbbf\ufbc0\ufbc1\ufc5e\ufc5f\ufc60\ufc61\ufc62\ufc63\ufcf2\ufcf3\ufcf4\ufd3e\ufd3f\ufe70\ufe71\ufe72\ufe76\ufe77\ufe78\ufe79\ufe7a\ufe7b\ufe7c\ufe7d\ufe7e\ufe7f\ufdfa\ufdfb]",
+                    "",
+                ),
+            ]
+
+        if self._seperate_mi:
+            self.verbs = Lemmatizer(joined_verb_parts=False).verbs
+            self.joint_mi_patterns = r"\bن?می[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]+"
+
+        if self._unicodes_replacement:
+            self.replacements = [
+                ("﷽", "بسم الله الرحمن الرحیم"),
+                ("﷼", "ریال"),
+                ("(ﷰ|ﷹ)", "صلی"),
+                ("ﷲ", "الله"),
+                ("ﷳ", "اکبر"),
+                ("ﷴ", "محمد"),
+                ("ﷵ", "صلعم"),
+                ("ﷶ", "رسول"),
+                ("ﷷ", "علیه"),
+                ("ﷸ", "وسلم"),
+                ("ﻵ|ﻶ|ﻷ|ﻸ|ﻹ|ﻺ|ﻻ|ﻼ", "لا"),
+            ]
+
+    def normalize(self: "Normalizer", text: str) -> str:
+        """متن را نرمال‌سازی می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.normalize('اِعلاممممم کَرد : « زمین لرزه ای به بُزرگیِ 6 دهم ریشتر ...»')
+            'اعلام کرد: «زمین‌لرزه‌ای به بزرگی ۶ دهم ریشتر …»'
+            >>> normalizer.normalize('')
+            ''
+
+        Args:
+            text: متنی که باید نرمال‌سازی شود.
+
+        Returns:
+            متنِ نرمال‌سازی‌شده.
+
+        """
+        translations = maketrans(self.translation_src, self.translation_dst)
+        text = text.translate(translations)
+
+        if self._persian_style:
+            text = self.persian_style(text)
+
+        if self._persian_number:
+            text = self.persian_number(text)
+
+        if self._remove_diacritics:
+            text = self.remove_diacritics(text)
+
+        if self._correct_spacing:
+            text = self.correct_spacing(text)
+
+        if self._unicodes_replacement:
+            text = self.unicodes_replacement(text)
+
+        if self._remove_specials_chars:
+            text = self.remove_specials_chars(text)
+
+        if self._decrease_repeated_chars:
+            text = self.decrease_repeated_chars(text)
+
+        if self._seperate_mi:
+            text = self.seperate_mi(text)
+
+        return text
+
+    def correct_spacing(self: "Normalizer", text: str) -> str:
+        """فاصله‌گذاری‌ها را در پیشوندها و پسوندها اصلاح می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.correct_spacing("سلام   دنیا")
+            'سلام دنیا'
+            >>> normalizer.correct_spacing("به طول ۹متر و عرض۶")
+            'به طول ۹ متر و عرض ۶'
+            >>> normalizer.correct_spacing("کاروان‌‌سرا")
+            'کاروان‌سرا'
+            >>> normalizer.correct_spacing("‌سلام‌ به ‌همه‌")
+            'سلام به همه'
+            >>> normalizer.correct_spacing("سلام دنیـــا")
+            'سلام دنیا'
+            >>> normalizer.correct_spacing("جمعهها که کار نمی کنم مطالعه می کنم")
+            'جمعه‌ها که کار نمی‌کنم مطالعه می‌کنم'
+            >>> normalizer.correct_spacing(' "سلام به همه"   ')
+            '"سلام به همه"'
+            >>> normalizer.correct_spacing('')
+            ''
+
+        Args:
+            text (str): متنی که باید فاصله‌گذاری‌های آن اصلاح شود.
+
+        Returns:
+            (str): متنی با فاصله‌گذاری‌های اصلاح‌شده.
+
+
+        """
+        text = regex_replace(self.extra_space_patterns, text)
+
+        lines = text.split("\n")
+        result = []
+        for line in lines:
+            tokens = self.tokenizer.tokenize(line)
+            spaced_tokens = self.token_spacing(tokens)
+            line = " ".join(spaced_tokens)
+            result.append(line)
+
+        text = "\n".join(result)
+
+        text = regex_replace(self.affix_spacing_patterns, text)
+        text = regex_replace(self.punctuation_spacing_patterns, text)
+
+        return text
+
+    def remove_diacritics(self: "Normalizer", text: str) -> str:
+        """اِعراب را از متن حذف می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.remove_diacritics('حَذفِ اِعراب')
+            'حذف اعراب'
+            >>> normalizer.remove_diacritics('آمدند')
+            'آمدند'
+            >>> normalizer.remove_diacritics('متن بدون اعراب')
+            'متن بدون اعراب'
+            >>> normalizer.remove_diacritics('')
+            ''
+
+        Args:
+            text: متنی که باید اعراب آن حذف شود.
+
+        Returns:
+            متنی بدون اعراب.
+
+        """
+        return regex_replace(self.diacritics_patterns, text)
+
+    def remove_specials_chars(self: "Normalizer", text: str) -> str:
+        """برخی از کاراکترها و نشانه‌های خاص را که کاربردی در پردازش متن ندارند حذف
+        می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.remove_specials_chars('پیامبر اکرم ﷺ')
+            'پیامبر اکرم '
+
+        Args:
+            text: متنی که باید کاراکترها و نشانه‌های اضافهٔ آن حذف شود.
+
+        Returns:
+            متنی بدون کاراکترها و نشانه‌های اضافه.
+
+        """
+        return regex_replace(self.specials_chars_patterns, text)
+
+    def decrease_repeated_chars(self: "Normalizer", text: str) -> str:
+        """تکرارهای زائد حروف را در کلماتی مثل سلامممممم حذف می‌کند و در مواردی که
+        نمی‌تواند تشخیص دهد دست کم به دو تکرار کاهش می‌دهد.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.decrease_repeated_chars('سلامممم به همه')
+            'سلام به همه'
+            >>> normalizer.decrease_repeated_chars('سلامم به همه')
+            'سلامم به همه'
+            >>> normalizer.decrease_repeated_chars('سلامم را برسان')
+            'سلامم را برسان'
+            >>> normalizer.decrease_repeated_chars('سلاممم را برسان')
+            'سلام را برسان'
+            >>> normalizer.decrease_repeated_chars('')
+            ''
+
+        Args:
+            text: متنی که باید تکرارهای زائد آن حذف شود.
+
+        Returns:
+            متنی بدون کاراکترهای زائد یا حداقل با دو تکرار.
+
+        """
+        matches = re.finditer(self.repeated_chars_pattern, text)
+
+        for m in matches:
+            word = m.group()
+            if word not in self.words:
+                no_repeat = re.sub(self.more_than_two_repeat_pattern, r"\1", word)
+                two_repeat = re.sub(self.more_than_two_repeat_pattern, r"\1\1", word)
+
+                if (no_repeat in self.words) != (two_repeat in self.words):
+                    r = no_repeat if no_repeat in self.words else two_repeat
+                    text = text.replace(word, r)
+                else:
+                    text = text.replace(word, two_repeat)
+
+        return text
+
+    def persian_style(self: "Normalizer", text: str) -> str:
+        """برخی از حروف و نشانه‌ها را با حروف و نشانه‌های فارسی جایگزین می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.persian_style('"نرمال‌سازی"')
+            '«نرمال‌سازی»'
+            >>> normalizer.persian_style('و ...')
+            'و …'
+            >>> normalizer.persian_style('10.450')
+            '10٫450'
+            >>> normalizer.persian_style('')
+            ''
+
+        Args:
+            text: متنی که باید حروف و نشانه‌های آن با حروف و نشانه‌های فارسی جایگزین شود.
+
+        Returns:
+            متنی با حروف و نشانه‌های فارسی‌سازی شده.
+
+        """
+        return regex_replace(self.persian_style_patterns, text)
+
+    def persian_number(self: "Normalizer", text: str) -> str:
+        """اعداد لاتین و علامت % را با معادل فارسی آن جایگزین می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.persian_number('5 درصد')
+            '۵ درصد'
+            >>> normalizer.persian_number('۵ درصد')
+            '۵ درصد'
+            >>> normalizer.persian_number('')
+            ''
+
+        Args:
+            text: متنی که باید اعداد لاتین و علامت % آن با معادل فارسی جایگزین شود.
+
+        Returns:
+            متنی با اعداد و علامت ٪ فارسی.
+
+        """
+        translations = maketrans(
+            self.number_translation_src,
+            self.number_translation_dst,
+        )
+        return text.translate(translations)
+
+    def unicodes_replacement(self: "Normalizer", text: str) -> str:
+        """برخی از کاراکترهای خاص یونیکد را با معادلِ نرمال آن جایگزین می‌کند. غالباً
+        این کار فقط در مواردی صورت می‌گیرد که یک کلمه در قالب یک کاراکتر یونیکد تعریف
+        شده است.
+
+        **فهرست این کاراکترها و نسخهٔ جایگزین آن:**
+
+        |کاراکتر|نسخهٔ جایگزین|
+        |--------|------------------|
+        |﷽|بسم الله الرحمن الرحیم|
+        |﷼|ریال|
+        |ﷰ، ﷹ|صلی|
+        |ﷲ|الله|
+        |ﷳ|اکبر|
+        |ﷴ|محمد|
+        |ﷵ|صلعم|
+        |ﷶ|رسول|
+        |ﷷ|علیه|
+        |ﷸ|وسلم|
+        |ﻵ، ﻶ، ﻷ، ﻸ، ﻹ، ﻺ، ﻻ، ﻼ|لا|
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.remove_specials_chars('پیامبر اکرم ﷺ')
+            'پیامبر اکرم '
+            >>> normalizer.remove_specials_chars('')
+            ''
+
+        Args:
+            text: متنی که باید برخی از کاراکترهای یونیکد آن (جدول بالا)، با شکل استاندارد، جایگزین شود.
+
+        Returns:
+            متنی که برخی از کاراکترهای یونیکد آن با شکل استاندارد جایگزین شده است.
+
+        """
+        for old, new in self.replacements:
+            text = re.sub(old, new, text)
+
+        return text
+
+    def seperate_mi(self: "Normalizer", text: str) -> str:
+        """پیشوند «می» و «نمی» را در افعال جدا کرده و با نیم‌فاصله می‌چسباند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.seperate_mi('نمیدانم چه میگفت')
+            'نمی‌دانم چه می‌گفت'
+            >>> normalizer.seperate_mi('میز')
+            'میز'
+            >>> normalizer.seperate_mi('')
+            ''
+
+
+        Args:
+            text: متنی که باید پیشوند «می» و «نمی» در آن جدا شود.
+
+        Returns:
+            متنی با «می» و «نمی» جدا شده.
+
+        """
+        matches = re.findall(r"\bن?می[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]+", text)
+        for m in matches:
+            r = re.sub("^(ن?می)", r"\1‌", m)
+            if r in self.verbs:
+                text = text.replace(m, r)
+
+        return text
+
+    def token_spacing(self: "Normalizer", tokens: List[str]) -> List[str]:
+        """توکن‌های ورودی را به فهرستی از توکن‌های نرمال‌سازی شده تبدیل می‌کند.
+        در این فرایند ممکن است برخی از توکن‌ها به یکدیگر بچسبند؛
+        برای مثال: `['زمین', 'لرزه', 'ای']` تبدیل می‌شود به: `['زمین‌لرزه‌ای']`.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.token_spacing(['کتاب', 'ها'])
+            ['کتاب‌ها']
+            >>> normalizer.token_spacing(['او', 'می', 'رود'])
+            ['او', 'می‌رود']
+            >>> normalizer.token_spacing(['ماه', 'می', 'سال', 'جدید'])
+            ['ماه', 'می', 'سال', 'جدید']
+            >>> normalizer.token_spacing(['اخلال', 'گر'])
+            ['اخلال‌گر']
+            >>> normalizer.token_spacing(['زمین', 'لرزه', 'ای'])
+            ['زمین‌لرزه‌ای']
+            >>> normalizer.token_spacing([])
+            []
+
+        Args:
+            tokens: توکن‌هایی که باید نرمال‌سازی شود.
+
+        Returns:
+            لیستی از توکن‌های نرمال‌سازی شده به شکل `[token1, token2, ...]`.
+
+        """
+        # >>> normalizer.token_spacing(['پرداخت', 'شده', 'است'])
+
+        result = []
+        for t, token in enumerate(tokens):
+            joined = False
+
+            if result:
+                token_pair = result[-1] + "‌" + token
+                if (
+                    token_pair in self.verbs
+                    or token_pair in self.words
+                    and self.words[token_pair][0] > 0
+                ):
+                    joined = True
+
+                    if (
+                        t < len(tokens) - 1
+                        and token + "_" + tokens[t + 1] in self.verbs
+                    ):
+                        joined = False
+
+                elif token in self.suffixes and result[-1] in self.words:
+                    joined = True
+
+            if joined:
+                result.pop()
+                result.append(token_pair)
+            else:
+                result.append(token)
+
+        return result
```

### Comparing `hazm-0.9.0/hazm/pos_tagger.py` & `hazm-0.9.1/hazm/pos_tagger.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای برچسب‌گذاری توکن‌هاست.
-
- **میزان دقت
-برچسب‌زنی در نسخهٔ حاضر ۹۷.۲ درصد [^1] است.**
-[^1]:
-این عدد با انتشار هر نسخه بروزرسانی می‌شود.
-
-"""
-
-from nltk.tag import stanford
-
-from hazm import SequenceTagger
-
-punctuation_list = [
-    '"',
-    "#",
-    "(",
-    ")",
-    "*",
-    ",",
-    "-",
-    ".",
-    "/",
-    ":",
-    "[",
-    "]",
-    "«",
-    "»",
-    "،",
-    ";",
-    "?",
-    "!",
-]
-
-
-class POSTagger(SequenceTagger):
-    """این کلاس‌ها شامل توابعی برای برچسب‌گذاری توکن‌هاست. **میزان دقت برچسب‌زنی در
-    نسخهٔ حاضر ۹۷.۲ درصد [^1] است.** این کلاس تمام توابع خود را از کلاس
-    [SequenceTagger][hazm.sequence_tagger.SequenceTagger] به ارث می‌برد.
-    [^1]:
-    این عدد با انتشار هر نسخه بروزرسانی می‌شود.
-
-    """
-
-    def __init__(
-        self: "POSTagger", model=None, data_maker=None, universal_tag=False,
-    ) -> None:
-        data_maker = self.data_maker if data_maker is None else data_maker
-        self.__is_universal = universal_tag
-        super().__init__(model, data_maker)
-
-    def __universal_converter(self: "POSTagger", tagged_list):
-        return [(word, tag.split(",")[0]) for word, tag in tagged_list]
-
-    def __is_punc(self: "POSTagger", word):
-        return word in punctuation_list
-
-    def data_maker(self: "POSTagger", tokens):
-        """تابعی که لیستی از لیستی از کلمات توکنایز شده را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
-
-        Examples:
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model')
-            >>> posTagger.data_maker(tokens = [['دلم', 'اینجا', 'مانده‌است', '.']])
-            [[{'word': 'دلم', 'is_first': True, 'is_last': False, 'prefix-1': 'د', 'prefix-2': 'دل', 'prefix-3': 'دلم', 'suffix-1': 'م', 'suffix-2': 'لم', 'suffix-3': 'دلم', 'prev_word': '', 'two_prev_word': '', 'next_word': 'اینجا', 'two_next_word': 'مانده\u200cاست', 'is_numeric': False, 'prev_is_numeric': '', 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': '', 'next_is_punc': False}, {'word': 'اینجا', 'is_first': False, 'is_last': False, 'prefix-1': 'ا', 'prefix-2': 'ای', 'prefix-3': 'این', 'suffix-1': 'ا', 'suffix-2': 'جا', 'suffix-3': 'نجا', 'prev_word': 'دلم', 'two_prev_word': '.', 'next_word': 'مانده\u200cاست', 'two_next_word': '.', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False}, {'word': 'مانده\u200cاست', 'is_first': False, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'ما', 'prefix-3': 'مان', 'suffix-1': 'ت', 'suffix-2': 'ست', 'suffix-3': 'است', 'prev_word': 'اینجا', 'two_prev_word': 'دلم', 'next_word': '.', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': True}, {'word': '.', 'is_first': False, 'is_last': True, 'prefix-1': '.', 'prefix-2': '.', 'prefix-3': '.', 'suffix-1': '.', 'suffix-2': '.', 'suffix-3': '.', 'prev_word': 'مانده\u200cاست', 'two_prev_word': 'اینجا', 'next_word': '', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': '', 'is_punc': True, 'prev_is_punc': False, 'next_is_punc': ''}]]
-
-        Args:
-            tokens (List[List[str]]): جملاتی که نیاز به تبدیل آن به برداری از ویژگی‌ها است.
-
-        Returns:
-            List(List(Dict())): لیستی از لیستی از دیکشنری‌های بیان‌کننده ویژگی‌های یک کلمه.
-        """
-        return [
-            [self.features(token, index) for index in range(len(token))]
-            for token in tokens
-        ]
-
-    def features(self: "POSTagger", sentence, index):
-        """features."""
-        return {
-            "word": sentence[index],
-            "is_first": index == 0,
-            "is_last": index == len(sentence) - 1,
-            # *ix
-            "prefix-1": sentence[index][0],
-            "prefix-2": sentence[index][:2],
-            "prefix-3": sentence[index][:3],
-            "suffix-1": sentence[index][-1],
-            "suffix-2": sentence[index][-2:],
-            "suffix-3": sentence[index][-3:],
-            # word
-            "prev_word": "" if index == 0 else sentence[index - 1],
-            "two_prev_word": "" if index == 0 else sentence[index - 2],
-            "next_word": "" if index == len(sentence) - 1 else sentence[index + 1],
-            "two_next_word": (
-                ""
-                if (index == len(sentence) - 1 or index == len(sentence) - 2)
-                else sentence[index + 2]
-            ),
-            # digit
-            "is_numeric": sentence[index].isdigit(),
-            "prev_is_numeric": "" if index == 0 else sentence[index - 1].isdigit(),
-            "next_is_numeric": (
-                "" if index == len(sentence) - 1 else sentence[index + 1].isdigit()
-            ),
-            # punc
-            "is_punc": self.__is_punc(sentence[index]),
-            "prev_is_punc": "" if index == 0 else self.__is_punc(sentence[index - 1]),
-            "next_is_punc": (
-                ""
-                if index == len(sentence) - 1
-                else self.__is_punc(sentence[index + 1])
-            ),
-        }
-
-    def tag(self: "POSTagger", tokens):
-        """یک جمله را در قالب لیستی از توکن‌ها دریافت می‌کند و در خروجی لیستی از
-        `(توکن، برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model')
-            >>> posTagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
-            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
-
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model', universal_tag = True)
-            >>> posTagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
-            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
-
-        Args:
-            tokens (List[str]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[Tuple[str,str]]): ‌لیستی از `(توکن، برچسب)`ها.
-
-        """
-        tagged_token = super().tag(tokens)
-        return (
-            self.__universal_converter(tagged_token)
-            if self.__is_universal
-            else tagged_token
-        )
-
-    def tag_sents(self: "POSTagger", sentences):
-        """جملات را در قالب لیستی از توکن‌ها دریافت می‌کند
-        و در خروجی، لیستی از لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
-
-        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
-
-        Examples:
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model')
-            >>> posTagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
-            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
-
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model', universal_tag = True)
-            >>> posTagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
-            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
-
-        Args:
-            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، برچسب)`ها.
-                    هر لیست از `(توکن،برچسب)`ها مربوط به یک جمله است.
-
-        """
-        tagged_sents = super().tag_sents(sentences)
-        return (
-            [self.__universal_converter(tagged_sent) for tagged_sent in tagged_sents]
-            if self.__is_universal
-            else tagged_sents
-        )
-
-
-class StanfordPOSTagger(stanford.StanfordPOSTagger):
-    """StanfordPOSTagger."""
-
-    def __init__(
-        self: "StanfordPOSTagger",
-        model_filename: "str",
-        path_to_jar: str,
-        *args,
-        **kwargs,
-    ) -> None:
-        self._SEPARATOR = "/"
-        super(stanford.StanfordPOSTagger, self).__init__(
-            model_filename=model_filename,
-            path_to_jar=path_to_jar,
-            *args,  # noqa: B026
-            **kwargs,
-        )
-
-    def tag(self: "StanfordPOSTagger", tokens):
-        """tag.
-
-        Examples:
-            >>> tagger = StanfordPOSTagger(model_filename='resources/persian.tagger', path_to_jar='resources/stanford_postagger.jar')
-            >>> tagger.tag(['من', 'به', 'مدرسه', 'رفته_بودم', '.'])
-            [('من', 'PRO'), ('به', 'P'), ('مدرسه', 'N'), ('رفته_بودم', 'V'), ('.', 'PUNC')]
-
-        """
-        return self.tag_sents([tokens])[0]
-
-    def tag_sents(self: "StanfordPOSTagger", sentences):
-        """tag_sents."""
-        refined = ([w.replace(" ", "_") for w in s] for s in sentences)
-        return super(stanford.StanfordPOSTagger, self).tag_sents(refined)
+"""این ماژول شامل کلاس‌ها و توابعی برای برچسب‌گذاری توکن‌هاست.
+
+ **میزان دقت
+برچسب‌زنی در نسخهٔ حاضر ۹۷.۲ درصد [^1] است.**
+[^1]:
+این عدد با انتشار هر نسخه بروزرسانی می‌شود.
+
+"""
+
+from nltk.tag import stanford
+
+from hazm import SequenceTagger
+
+punctuation_list = [
+    '"',
+    "#",
+    "(",
+    ")",
+    "*",
+    ",",
+    "-",
+    ".",
+    "/",
+    ":",
+    "[",
+    "]",
+    "«",
+    "»",
+    "،",
+    ";",
+    "?",
+    "!",
+]
+
+
+class POSTagger(SequenceTagger):
+    """این کلاس‌ها شامل توابعی برای برچسب‌گذاری توکن‌هاست. **میزان دقت برچسب‌زنی در
+    نسخهٔ حاضر ۹۷.۲ درصد [^1] است.** این کلاس تمام توابع خود را از کلاس
+    [SequenceTagger][hazm.sequence_tagger.SequenceTagger] به ارث می‌برد.
+    [^1]:
+    این عدد با انتشار هر نسخه بروزرسانی می‌شود.
+
+    """
+
+    def __init__(
+        self: "POSTagger", model=None, data_maker=None, universal_tag=False,
+    ) -> None:
+        data_maker = self.data_maker if data_maker is None else data_maker
+        self.__is_universal = universal_tag
+        super().__init__(model, data_maker)
+
+    def __universal_converter(self: "POSTagger", tagged_list):
+        return [(word, tag.split(",")[0]) for word, tag in tagged_list]
+
+    def __is_punc(self: "POSTagger", word):
+        return word in punctuation_list
+
+    def data_maker(self: "POSTagger", tokens):
+        """تابعی که لیستی از لیستی از کلمات توکنایز شده را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
+
+        Examples:
+            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model')
+            >>> posTagger.data_maker(tokens = [['دلم', 'اینجا', 'مانده‌است', '.']])
+            [[{'word': 'دلم', 'is_first': True, 'is_last': False, 'prefix-1': 'د', 'prefix-2': 'دل', 'prefix-3': 'دلم', 'suffix-1': 'م', 'suffix-2': 'لم', 'suffix-3': 'دلم', 'prev_word': '', 'two_prev_word': '', 'next_word': 'اینجا', 'two_next_word': 'مانده\u200cاست', 'is_numeric': False, 'prev_is_numeric': '', 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': '', 'next_is_punc': False}, {'word': 'اینجا', 'is_first': False, 'is_last': False, 'prefix-1': 'ا', 'prefix-2': 'ای', 'prefix-3': 'این', 'suffix-1': 'ا', 'suffix-2': 'جا', 'suffix-3': 'نجا', 'prev_word': 'دلم', 'two_prev_word': '.', 'next_word': 'مانده\u200cاست', 'two_next_word': '.', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False}, {'word': 'مانده\u200cاست', 'is_first': False, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'ما', 'prefix-3': 'مان', 'suffix-1': 'ت', 'suffix-2': 'ست', 'suffix-3': 'است', 'prev_word': 'اینجا', 'two_prev_word': 'دلم', 'next_word': '.', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': True}, {'word': '.', 'is_first': False, 'is_last': True, 'prefix-1': '.', 'prefix-2': '.', 'prefix-3': '.', 'suffix-1': '.', 'suffix-2': '.', 'suffix-3': '.', 'prev_word': 'مانده\u200cاست', 'two_prev_word': 'اینجا', 'next_word': '', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': '', 'is_punc': True, 'prev_is_punc': False, 'next_is_punc': ''}]]
+
+        Args:
+            tokens (List[List[str]]): جملاتی که نیاز به تبدیل آن به برداری از ویژگی‌ها است.
+
+        Returns:
+            List(List(Dict())): لیستی از لیستی از دیکشنری‌های بیان‌کننده ویژگی‌های یک کلمه.
+        """
+        return [
+            [self.features(token, index) for index in range(len(token))]
+            for token in tokens
+        ]
+
+    def features(self: "POSTagger", sentence, index):
+        """features."""
+        return {
+            "word": sentence[index],
+            "is_first": index == 0,
+            "is_last": index == len(sentence) - 1,
+            # *ix
+            "prefix-1": sentence[index][0],
+            "prefix-2": sentence[index][:2],
+            "prefix-3": sentence[index][:3],
+            "suffix-1": sentence[index][-1],
+            "suffix-2": sentence[index][-2:],
+            "suffix-3": sentence[index][-3:],
+            # word
+            "prev_word": "" if index == 0 else sentence[index - 1],
+            "two_prev_word": "" if index == 0 else sentence[index - 2],
+            "next_word": "" if index == len(sentence) - 1 else sentence[index + 1],
+            "two_next_word": (
+                ""
+                if (index == len(sentence) - 1 or index == len(sentence) - 2)
+                else sentence[index + 2]
+            ),
+            # digit
+            "is_numeric": sentence[index].isdigit(),
+            "prev_is_numeric": "" if index == 0 else sentence[index - 1].isdigit(),
+            "next_is_numeric": (
+                "" if index == len(sentence) - 1 else sentence[index + 1].isdigit()
+            ),
+            # punc
+            "is_punc": self.__is_punc(sentence[index]),
+            "prev_is_punc": "" if index == 0 else self.__is_punc(sentence[index - 1]),
+            "next_is_punc": (
+                ""
+                if index == len(sentence) - 1
+                else self.__is_punc(sentence[index + 1])
+            ),
+        }
+
+    def tag(self: "POSTagger", tokens):
+        """یک جمله را در قالب لیستی از توکن‌ها دریافت می‌کند و در خروجی لیستی از
+        `(توکن، برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model')
+            >>> posTagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
+            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
+
+            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model', universal_tag = True)
+            >>> posTagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
+            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
+
+        Args:
+            tokens (List[str]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[Tuple[str,str]]): ‌لیستی از `(توکن، برچسب)`ها.
+
+        """
+        tagged_token = super().tag(tokens)
+        return (
+            self.__universal_converter(tagged_token)
+            if self.__is_universal
+            else tagged_token
+        )
+
+    def tag_sents(self: "POSTagger", sentences):
+        """جملات را در قالب لیستی از توکن‌ها دریافت می‌کند
+        و در خروجی، لیستی از لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
+
+        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
+
+        Examples:
+            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model')
+            >>> posTagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
+            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
+
+            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model', universal_tag = True)
+            >>> posTagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
+            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
+
+        Args:
+            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، برچسب)`ها.
+                    هر لیست از `(توکن،برچسب)`ها مربوط به یک جمله است.
+
+        """
+        tagged_sents = super().tag_sents(sentences)
+        return (
+            [self.__universal_converter(tagged_sent) for tagged_sent in tagged_sents]
+            if self.__is_universal
+            else tagged_sents
+        )
+
+
+class StanfordPOSTagger(stanford.StanfordPOSTagger):
+    """StanfordPOSTagger."""
+
+    def __init__(
+        self: "StanfordPOSTagger",
+        model_filename: "str",
+        path_to_jar: str,
+        *args,
+        **kwargs,
+    ) -> None:
+        self._SEPARATOR = "/"
+        super(stanford.StanfordPOSTagger, self).__init__(
+            model_filename=model_filename,
+            path_to_jar=path_to_jar,
+            *args,  # noqa: B026
+            **kwargs,
+        )
+
+    def tag(self: "StanfordPOSTagger", tokens):
+        """tag.
+
+        Examples:
+            >>> tagger = StanfordPOSTagger(model_filename='resources/persian.tagger', path_to_jar='resources/stanford_postagger.jar')
+            >>> tagger.tag(['من', 'به', 'مدرسه', 'رفته_بودم', '.'])
+            [('من', 'PRO'), ('به', 'P'), ('مدرسه', 'N'), ('رفته_بودم', 'V'), ('.', 'PUNC')]
+
+        """
+        return self.tag_sents([tokens])[0]
+
+    def tag_sents(self: "StanfordPOSTagger", sentences):
+        """tag_sents."""
+        refined = ([w.replace(" ", "_") for w in s] for s in sentences)
+        return super(stanford.StanfordPOSTagger, self).tag_sents(refined)
```

### Comparing `hazm-0.9.0/hazm/sentence_tokenizer.py` & `hazm-0.9.1/hazm/sentence_tokenizer.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای استخراج جملاتِ متن است.
-
-برای استخراج کلمات از تابع [WordTokenizer()][hazm.WordTokenizer] استفاده کنید.
-
-"""
-
-
-import re
-from typing import List
-
-from nltk.tokenize.api import TokenizerI
-
-
-class SentenceTokenizer(TokenizerI):
-    """این کلاس شامل توابعی برای استخراج جملاتِ متن است."""
-
-    def __init__(self: "SentenceTokenizer") -> None:
-        self.pattern = re.compile(r"([!.?⸮؟]+)[ \n]+")
-
-    def tokenize(self: "SentenceTokenizer", text: str) -> List[str]:
-        """متن ورودی را به جملات سازندهٔ آن می‌شِکند.
-
-        Examples:
-            >>> tokenizer = SentenceTokenizer()
-            >>> tokenizer.tokenize('جدا کردن ساده است. تقریبا البته!')
-            ['جدا کردن ساده است.', 'تقریبا البته!']
-
-        Args:
-            text: متنی که باید جملات آن استخراج شود.
-
-        Returns:
-            فهرست جملات استخراج‌شده.
-
-        """
-        text = self.pattern.sub(r"\1\n\n", text)
-        return [
-            sentence.replace("\n", " ").strip()
-            for sentence in text.split("\n\n")
-            if sentence.strip()
-        ]
+"""این ماژول شامل کلاس‌ها و توابعی برای استخراج جملاتِ متن است.
+
+برای استخراج کلمات از تابع [WordTokenizer()][hazm.WordTokenizer] استفاده کنید.
+
+"""
+
+
+import re
+from typing import List
+
+from nltk.tokenize.api import TokenizerI
+
+
+class SentenceTokenizer(TokenizerI):
+    """این کلاس شامل توابعی برای استخراج جملاتِ متن است."""
+
+    def __init__(self: "SentenceTokenizer") -> None:
+        self.pattern = re.compile(r"([!.?⸮؟]+)[ \n]+")
+
+    def tokenize(self: "SentenceTokenizer", text: str) -> List[str]:
+        """متن ورودی را به جملات سازندهٔ آن می‌شِکند.
+
+        Examples:
+            >>> tokenizer = SentenceTokenizer()
+            >>> tokenizer.tokenize('جدا کردن ساده است. تقریبا البته!')
+            ['جدا کردن ساده است.', 'تقریبا البته!']
+
+        Args:
+            text: متنی که باید جملات آن استخراج شود.
+
+        Returns:
+            فهرست جملات استخراج‌شده.
+
+        """
+        text = self.pattern.sub(r"\1\n\n", text)
+        return [
+            sentence.replace("\n", " ").strip()
+            for sentence in text.split("\n\n")
+            if sentence.strip()
+        ]
```

### Comparing `hazm-0.9.0/hazm/sequence_tagger.py` & `hazm-0.9.1/hazm/sequence_tagger.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,411 +1,411 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای برچسب‌گذاری توکن‌هاست."""
-
-import time
-from typing import List
-from typing import Tuple
-
-import numpy as np
-from pycrfsuite import Tagger
-from pycrfsuite import Trainer
-from sklearn.metrics import accuracy_score
-
-
-def features(sent, index):
-    """فهرست فیچرها را برمی‌گرداند."""
-    return {
-        "word": sent[index],
-        "is_first": index == 0,
-        "is_last": index == len(sent),
-        "is_num": sent[index].isdigit(),
-        "prev_word": sent[index - 1] if index != 0 else "",
-        "next_word": sent[index + 1] if index != len(sent) - 1 else "",
-    }
-
-
-def data_maker(tokens):
-    """تابع دیتا میکر."""
-    return [[features(sent, index) for index in range(len(sent))] for sent in tokens]
-
-
-def iob_features(words, pos_tags, index):
-    """تابع iob_features."""
-    word_features = features(words, index)
-    word_features.update(
-        {
-            "pos": pos_tags[index],
-            "prev_pos": "" if index == 0 else pos_tags[index - 1],
-            "next_pos": "" if index == len(pos_tags) - 1 else pos_tags[index + 1],
-        },
-    )
-    return word_features
-
-
-def iob_data_maker(tokens):
-    """تابع iob_data_maker."""
-    words = [[word for word, _ in token] for token in tokens]
-    tags = [[tag for _, tag in token] for token in tokens]
-    return [
-        [
-            iob_features(words=word_tokens, pos_taggs=tag_tokens, index=index)
-            for index in range(len(word_tokens))
-        ]
-        for word_tokens, tag_tokens in zip(words, tags)
-    ]
-
-
-class SequenceTagger:
-    """این کلاس شامل توابعی برای برچسب‌گذاری توکن‌ها است. این کلاس در نقش یک
-    wrapper برای کتابخانهٔ [python-crfsuite](https://python-crfsuite.readthedocs.io/en/latest/) است.
-
-    Args:
-        model (str, optional): مسیر فایل tagger.
-        data_maker (function, optional): تابعی که لیستی دو بعدی از کلمات توکنایز شده را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
-    """
-
-    def __init__(self: "SequenceTagger", model=None, data_maker=data_maker) -> None:
-        if model is not None:
-            self.load_model(model)
-        else:
-            self.model = None
-        self.data_maker = data_maker
-
-    def __add_label(self: "SequenceTagger", sentence, tags):
-        return [(word, tag) for word, tag in zip(sentence, tags)]
-
-    def __tag(self: "SequenceTagger", tokens):
-        return self.__add_label(tokens, self.model.tag(self.data_maker([tokens])[0]))
-
-    def __train(
-        self: "SequenceTagger", x, y, args, verbose, file_name, report_duration,
-    ):
-        trainer = Trainer(verbose=verbose)
-        trainer.set_params(args)
-
-        for xseq, yseq in zip(x, y):
-            trainer.append(xseq, yseq)
-
-        start_time = time.time()
-        trainer.train(file_name)
-        end_time = time.time()
-
-        if report_duration:
-            print(f"training time: {(end_time - start_time):.2f} sec")
-
-        self.load_model(file_name)
-
-    def __evaluate(self: "SequenceTagger", gold_labels, predicted_labels):
-        gold_labels = np.concatenate(gold_labels)
-        predicted_labels = np.concatenate(predicted_labels)
-        return float(accuracy_score(gold_labels, predicted_labels))
-
-    def load_model(self: "SequenceTagger", model):
-        """فایل تگر را بارگزاری می‌کند.
-
-        Examples:
-            >>> tagger = SequenceTagger()
-            >>> tagger.load_model(model = 'tagger.model')
-
-        Args:
-            model (str): مسیر فایل تگر.
-
-        """
-        tagger = Tagger()
-        tagger.open(model)
-        self.model = tagger
-
-    def tag(self: "SequenceTagger", tokens):
-        """یک جمله را در قالب لیستی از توکن‌ها دریافت می‌کند و در خروجی لیستی از
-        `(توکن، برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> tagger = SequenceTagger(model = 'tagger.model')
-            >>> tagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
-            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
-
-        Args:
-            tokens (List[str]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[Tuple[str,str]]): ‌لیستی از `(توکن، برچسب)`ها.
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        return self.__tag(tokens)
-
-    def tag_sents(self: "SequenceTagger", sentences):
-        """جملات را در قالب لیستی از توکن‌ها دریافت می‌کند
-        و در خروجی، لیستی از لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
-
-        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
-
-        Examples:
-            >>> tagger = SequenceTagger(model = 'tagger.model')
-            >>> tagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
-            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
-
-        Args:
-            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، برچسب)`ها.
-                    هر لیست از `(توکن،برچسب)`ها مربوط به یک جمله است.
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        return [self.__tag(tokens) for tokens in sentences]
-
-    def train(
-        self: "SequenceTagger",
-        tagged_list,
-        c1=0.4,
-        c2=0.04,
-        max_iteration=400,
-        verbose=True,
-        file_name="crf.model",
-        report_duration=True,
-    ):
-        """لیستی از جملات را می‌گیرد و بر اساس آن مدل را آموزش می‌دهد.
-
-        هر جمله، لیستی از `(توکن، برچسب)`هاست.
-
-        Examples:
-            >>> tagger = SequenceTagger()
-            >>> tagger.train(tagged_list = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'tagger.model', report_duration = True)
-            Feature generation
-            type: CRF1d
-            feature.minfreq: 0.000000
-            feature.possible_states: 0
-            feature.possible_transitions: 1
-            0....1....2....3....4....5....6....7....8....9....10
-            Number of features: 150
-            Seconds required: 0.001
-            ...
-            Writing feature references for attributes
-            Seconds required: 0.000
-
-            training time: 0.01 sec
-
-        Args:
-            tagged_list (List[{List[Tuple[str,str]]]): جملاتی که مدل از روی آن‌ها آموزش می‌بیند.
-            c1 (float): مقدار L1 regularization.
-            c2 (float): مقدار L2 regularization.
-            max_iteration (int): تعداد تکرار آموزش بر کل دیتا.
-            verbose (boolean): نمایش اطلاعات مربوط به آموزش.
-            file_name (str): نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
-            report_duration (boolean): نمایش گزارشات مربوط به زمان.
-
-        """
-        x = self.data_maker(
-            [[x for x, _ in tagged_sent] for tagged_sent in tagged_list],
-        )
-        y = [[y for _, y in tagged_sent] for tagged_sent in tagged_list]
-
-        args = {
-            "c1": c1,
-            "c2": c2,
-            "max_iterations": max_iteration,
-            "feature.possible_transitions": True,
-        }
-
-        self.__train(x, y, args, verbose, file_name, report_duration)
-
-    def save_model(self: "SequenceTagger", filename):
-        """مدل تهیه‌شده توسط تابع [train()][hazm.sequence_tagger.SequenceTagger.train]
-        را ذخیره می‌کند.
-
-        Examples:
-            >>> tagger = SequenceTagger()
-            >>> tagger.train(tagged_list = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'tagger.model', report_duration = True)
-            >>> tagger.save_model(file_name = 'new_tagger.model')
-
-        Args:
-            filename (str): نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        self.model.dump(filename)
-
-    def evaluate(
-        self: "SequenceTagger", tagged_sent: List[List[Tuple[str, str]]],
-    ) -> float:
-        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
-
-        Examples:
-            >>> tagger = SequenceTagger(model = 'tagger.model')
-            >>> tagger.evaluate([[('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')]])
-            1.0
-
-
-        Args:
-            tagged_sent: جملات لیبل‌داری که با استفاده از آن مدل را ارزیابی می‌کنیم.
-
-        Returns:
-            دقت مدل
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        def extract_labels(tagged_list):
-            return [[label for _, label in sent] for sent in tagged_list]
-
-        tokens = [[word for word, _ in sent] for sent in tagged_sent]
-        predicted_tagged_sent = self.tag_sents(tokens)
-        return self.__evaluate(
-            extract_labels(tagged_sent),
-            extract_labels(predicted_tagged_sent),
-        )
-
-
-class IOBTagger(SequenceTagger):
-    """IOBTagger."""
-
-    def __init__(self: "SequenceTagger", model=None, data_maker=iob_data_maker) -> None:
-        super().__init__(model, data_maker)
-
-    def __iob_format(self: "SequenceTagger", tagged_data, chunk_tags):
-        return [
-            (token[0], token[1], chunk_tag[1])
-            for token, chunk_tag in zip(tagged_data, chunk_tags)
-        ]
-
-    def tag(self: "SequenceTagger", tagged_data):
-        """یک جمله را در قالب لیستی از توکن‌ها و تگ‌ها دریافت می‌کند و در خروجی لیستی از
-        `(توکن، تگ، برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> iobTagger = IOBTagger(model = 'tagger.model')
-            >>> iobTagger.tag(tagged_data = [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')])
-            [('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]
-
-        Args:
-            tagged_data (List[Tuple[str, str]]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[Tuple[str, str, str]]): ‌لیستی از `(توکن، تگ، برچسب)`ها.
-
-        """
-        chunk_tags = super().tag(tagged_data)
-        return self.__iob_format(tagged_data, chunk_tags)
-
-    def tag_sents(self: "SequenceTagger", sentences):
-        """جملات را در قالب لیستی لیستی از توکن‌ها و تگ‌ها دریافت می‌کند
-        و در خروجی، لیستی از لیستی از `(توکن، تگ، برچسب)`ها برمی‌گرداند.
-
-        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
-
-        Examples:
-            >>> iobTagger = IOBTagger(model = 'tagger.model')
-            >>> iobTagger.tag_sents(tagged_data = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]])
-            [[('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]]
-
-        Args:
-            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، تگ، برچسب)`ها.
-                    هر لیست از `(توکن، تگ، برچسب)`ها مربوط به یک جمله است.
-
-        """
-        chunk_tags = super().tag_sents(sentences)
-        return [
-            self.__iob_format(tagged_data, chunks)
-            for tagged_data, chunks in zip(sentences, chunk_tags)
-        ]
-
-    def train(
-        self: "SequenceTagger",
-        tagged_list: List[List[Tuple[str, str, str]]],
-        c1: float = 0.4,
-        c2: float = 0.04,
-        max_iteration: int = 400,
-        verbose: True = True,
-        file_name: str = "crf.model",
-        report_duration=True,
-    ):
-        """لیستی از جملات را می‌گیرد و بر اساس آن مدل را آموزش می‌دهد.
-
-        هر جمله، لیستی از `(توکن، تگ، برچسب)`هاست.
-
-        Examples:
-            >>> iobTagger = IOBTagger()
-            >>> iobTagger.train(tagged_list = [[('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'newIOBTagger.model', report_duration = True)
-            Feature generation
-            type: CRF1d
-            feature.minfreq: 0.000000
-            feature.possible_states: 0
-            feature.possible_transitions: 1
-            0....1....2....3....4....5....6....7....8....9....10
-            Number of features: 150
-            Seconds required: 0.001
-            ...
-            Writing feature references for attributes
-            Seconds required: 0.000
-
-            training time: 0.01 sec
-
-        Args:
-            tagged_list: جملاتی که مدل از روی آن‌ها آموزش می‌بیند.
-            c1: مقدار L1 regularization.
-            c2: مقدار L2 regularization.
-            max_iteration: تعداد تکرار آموزش بر کل دیتا.
-            verbose: نمایش اطلاعات مربوط به آموزش.
-            file_name: نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
-            report_duration: نمایش گزارشات مربوط به زمان.
-
-        """
-        tagged_list = [
-            [((word, tag), chunk) for word, tag, chunk in tagged_sent]
-            for tagged_sent in tagged_list
-        ]
-        return super().train(
-            tagged_list,
-            c1,
-            c2,
-            max_iteration,
-            verbose,
-            file_name,
-            report_duration,
-        )
-
-    def evaluate(
-        self: "SequenceTagger", tagged_sent: List[List[Tuple[str, str, str]]],
-    ) -> float:
-        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
-
-        Examples:
-            >>> iobTagger = IOBTagger(model = 'tagger.model')
-            >>> iobTagger.evaluate([[('نامه', 'NOUN,EZ', 'B-NP'), ('ایشان', 'PRON', 'I-NP'), ('را', 'ADP', 'B-POSTP'), ('دریافت', 'NOUN', 'B-VP'), ('داشتم', 'VERB', 'I-VP'), ('.', 'PUNCT', 'O')]])
-            1.0
-
-
-        Args:
-            tagged_sent: جملات لیبل‌داری که با استفاده از آن مدل را ارزیابی می‌کنیم.
-
-        Returns:
-            دقت مدل
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        def extract_labels(tagged_list):
-            return [[token[-1] for token in sent] for sent in tagged_list]
-
-        tokens = [[token[:-1] for token in sent] for sent in tagged_sent]
-        predicted_tagged_sent = self.tag_sents(tokens)
-        return super()._SequenceTagger__evaluate(
-            extract_labels(tagged_sent),
-            extract_labels(predicted_tagged_sent),
-        )
+"""این ماژول شامل کلاس‌ها و توابعی برای برچسب‌گذاری توکن‌هاست."""
+
+import time
+from typing import List
+from typing import Tuple
+
+import numpy as np
+from pycrfsuite import Tagger
+from pycrfsuite import Trainer
+from sklearn.metrics import accuracy_score
+
+
+def features(sent, index):
+    """فهرست فیچرها را برمی‌گرداند."""
+    return {
+        "word": sent[index],
+        "is_first": index == 0,
+        "is_last": index == len(sent),
+        "is_num": sent[index].isdigit(),
+        "prev_word": sent[index - 1] if index != 0 else "",
+        "next_word": sent[index + 1] if index != len(sent) - 1 else "",
+    }
+
+
+def data_maker(tokens):
+    """تابع دیتا میکر."""
+    return [[features(sent, index) for index in range(len(sent))] for sent in tokens]
+
+
+def iob_features(words, pos_tags, index):
+    """تابع iob_features."""
+    word_features = features(words, index)
+    word_features.update(
+        {
+            "pos": pos_tags[index],
+            "prev_pos": "" if index == 0 else pos_tags[index - 1],
+            "next_pos": "" if index == len(pos_tags) - 1 else pos_tags[index + 1],
+        },
+    )
+    return word_features
+
+
+def iob_data_maker(tokens):
+    """تابع iob_data_maker."""
+    words = [[word for word, _ in token] for token in tokens]
+    tags = [[tag for _, tag in token] for token in tokens]
+    return [
+        [
+            iob_features(words=word_tokens, pos_taggs=tag_tokens, index=index)
+            for index in range(len(word_tokens))
+        ]
+        for word_tokens, tag_tokens in zip(words, tags)
+    ]
+
+
+class SequenceTagger:
+    """این کلاس شامل توابعی برای برچسب‌گذاری توکن‌ها است. این کلاس در نقش یک
+    wrapper برای کتابخانهٔ [python-crfsuite](https://python-crfsuite.readthedocs.io/en/latest/) است.
+
+    Args:
+        model (str, optional): مسیر فایل tagger.
+        data_maker (function, optional): تابعی که لیستی دو بعدی از کلمات توکنایز شده را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
+    """
+
+    def __init__(self: "SequenceTagger", model=None, data_maker=data_maker) -> None:
+        if model is not None:
+            self.load_model(model)
+        else:
+            self.model = None
+        self.data_maker = data_maker
+
+    def __add_label(self: "SequenceTagger", sentence, tags):
+        return [(word, tag) for word, tag in zip(sentence, tags)]
+
+    def __tag(self: "SequenceTagger", tokens):
+        return self.__add_label(tokens, self.model.tag(self.data_maker([tokens])[0]))
+
+    def __train(
+        self: "SequenceTagger", x, y, args, verbose, file_name, report_duration,
+    ):
+        trainer = Trainer(verbose=verbose)
+        trainer.set_params(args)
+
+        for xseq, yseq in zip(x, y):
+            trainer.append(xseq, yseq)
+
+        start_time = time.time()
+        trainer.train(file_name)
+        end_time = time.time()
+
+        if report_duration:
+            print(f"training time: {(end_time - start_time):.2f} sec")
+
+        self.load_model(file_name)
+
+    def __evaluate(self: "SequenceTagger", gold_labels, predicted_labels):
+        gold_labels = np.concatenate(gold_labels)
+        predicted_labels = np.concatenate(predicted_labels)
+        return float(accuracy_score(gold_labels, predicted_labels))
+
+    def load_model(self: "SequenceTagger", model):
+        """فایل تگر را بارگزاری می‌کند.
+
+        Examples:
+            >>> tagger = SequenceTagger()
+            >>> tagger.load_model(model = 'tagger.model')
+
+        Args:
+            model (str): مسیر فایل تگر.
+
+        """
+        tagger = Tagger()
+        tagger.open(model)
+        self.model = tagger
+
+    def tag(self: "SequenceTagger", tokens):
+        """یک جمله را در قالب لیستی از توکن‌ها دریافت می‌کند و در خروجی لیستی از
+        `(توکن، برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> tagger = SequenceTagger(model = 'tagger.model')
+            >>> tagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
+            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
+
+        Args:
+            tokens (List[str]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[Tuple[str,str]]): ‌لیستی از `(توکن، برچسب)`ها.
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        return self.__tag(tokens)
+
+    def tag_sents(self: "SequenceTagger", sentences):
+        """جملات را در قالب لیستی از توکن‌ها دریافت می‌کند
+        و در خروجی، لیستی از لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
+
+        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
+
+        Examples:
+            >>> tagger = SequenceTagger(model = 'tagger.model')
+            >>> tagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
+            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
+
+        Args:
+            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، برچسب)`ها.
+                    هر لیست از `(توکن،برچسب)`ها مربوط به یک جمله است.
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        return [self.__tag(tokens) for tokens in sentences]
+
+    def train(
+        self: "SequenceTagger",
+        tagged_list,
+        c1=0.4,
+        c2=0.04,
+        max_iteration=400,
+        verbose=True,
+        file_name="crf.model",
+        report_duration=True,
+    ):
+        """لیستی از جملات را می‌گیرد و بر اساس آن مدل را آموزش می‌دهد.
+
+        هر جمله، لیستی از `(توکن، برچسب)`هاست.
+
+        Examples:
+            >>> tagger = SequenceTagger()
+            >>> tagger.train(tagged_list = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'tagger.model', report_duration = True)
+            Feature generation
+            type: CRF1d
+            feature.minfreq: 0.000000
+            feature.possible_states: 0
+            feature.possible_transitions: 1
+            0....1....2....3....4....5....6....7....8....9....10
+            Number of features: 150
+            Seconds required: 0.001
+            ...
+            Writing feature references for attributes
+            Seconds required: 0.000
+
+            training time: 0.01 sec
+
+        Args:
+            tagged_list (List[{List[Tuple[str,str]]]): جملاتی که مدل از روی آن‌ها آموزش می‌بیند.
+            c1 (float): مقدار L1 regularization.
+            c2 (float): مقدار L2 regularization.
+            max_iteration (int): تعداد تکرار آموزش بر کل دیتا.
+            verbose (boolean): نمایش اطلاعات مربوط به آموزش.
+            file_name (str): نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
+            report_duration (boolean): نمایش گزارشات مربوط به زمان.
+
+        """
+        x = self.data_maker(
+            [[x for x, _ in tagged_sent] for tagged_sent in tagged_list],
+        )
+        y = [[y for _, y in tagged_sent] for tagged_sent in tagged_list]
+
+        args = {
+            "c1": c1,
+            "c2": c2,
+            "max_iterations": max_iteration,
+            "feature.possible_transitions": True,
+        }
+
+        self.__train(x, y, args, verbose, file_name, report_duration)
+
+    def save_model(self: "SequenceTagger", filename):
+        """مدل تهیه‌شده توسط تابع [train()][hazm.sequence_tagger.SequenceTagger.train]
+        را ذخیره می‌کند.
+
+        Examples:
+            >>> tagger = SequenceTagger()
+            >>> tagger.train(tagged_list = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'tagger.model', report_duration = True)
+            >>> tagger.save_model(file_name = 'new_tagger.model')
+
+        Args:
+            filename (str): نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        self.model.dump(filename)
+
+    def evaluate(
+        self: "SequenceTagger", tagged_sent: List[List[Tuple[str, str]]],
+    ) -> float:
+        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
+
+        Examples:
+            >>> tagger = SequenceTagger(model = 'tagger.model')
+            >>> tagger.evaluate([[('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')]])
+            1.0
+
+
+        Args:
+            tagged_sent: جملات لیبل‌داری که با استفاده از آن مدل را ارزیابی می‌کنیم.
+
+        Returns:
+            دقت مدل
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        def extract_labels(tagged_list):
+            return [[label for _, label in sent] for sent in tagged_list]
+
+        tokens = [[word for word, _ in sent] for sent in tagged_sent]
+        predicted_tagged_sent = self.tag_sents(tokens)
+        return self.__evaluate(
+            extract_labels(tagged_sent),
+            extract_labels(predicted_tagged_sent),
+        )
+
+
+class IOBTagger(SequenceTagger):
+    """IOBTagger."""
+
+    def __init__(self: "SequenceTagger", model=None, data_maker=iob_data_maker) -> None:
+        super().__init__(model, data_maker)
+
+    def __iob_format(self: "SequenceTagger", tagged_data, chunk_tags):
+        return [
+            (token[0], token[1], chunk_tag[1])
+            for token, chunk_tag in zip(tagged_data, chunk_tags)
+        ]
+
+    def tag(self: "SequenceTagger", tagged_data):
+        """یک جمله را در قالب لیستی از توکن‌ها و تگ‌ها دریافت می‌کند و در خروجی لیستی از
+        `(توکن، تگ، برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> iobTagger = IOBTagger(model = 'tagger.model')
+            >>> iobTagger.tag(tagged_data = [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')])
+            [('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]
+
+        Args:
+            tagged_data (List[Tuple[str, str]]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[Tuple[str, str, str]]): ‌لیستی از `(توکن، تگ، برچسب)`ها.
+
+        """
+        chunk_tags = super().tag(tagged_data)
+        return self.__iob_format(tagged_data, chunk_tags)
+
+    def tag_sents(self: "SequenceTagger", sentences):
+        """جملات را در قالب لیستی لیستی از توکن‌ها و تگ‌ها دریافت می‌کند
+        و در خروجی، لیستی از لیستی از `(توکن، تگ، برچسب)`ها برمی‌گرداند.
+
+        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
+
+        Examples:
+            >>> iobTagger = IOBTagger(model = 'tagger.model')
+            >>> iobTagger.tag_sents(tagged_data = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]])
+            [[('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]]
+
+        Args:
+            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، تگ، برچسب)`ها.
+                    هر لیست از `(توکن، تگ، برچسب)`ها مربوط به یک جمله است.
+
+        """
+        chunk_tags = super().tag_sents(sentences)
+        return [
+            self.__iob_format(tagged_data, chunks)
+            for tagged_data, chunks in zip(sentences, chunk_tags)
+        ]
+
+    def train(
+        self: "SequenceTagger",
+        tagged_list: List[List[Tuple[str, str, str]]],
+        c1: float = 0.4,
+        c2: float = 0.04,
+        max_iteration: int = 400,
+        verbose: True = True,
+        file_name: str = "crf.model",
+        report_duration=True,
+    ):
+        """لیستی از جملات را می‌گیرد و بر اساس آن مدل را آموزش می‌دهد.
+
+        هر جمله، لیستی از `(توکن، تگ، برچسب)`هاست.
+
+        Examples:
+            >>> iobTagger = IOBTagger()
+            >>> iobTagger.train(tagged_list = [[('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'newIOBTagger.model', report_duration = True)
+            Feature generation
+            type: CRF1d
+            feature.minfreq: 0.000000
+            feature.possible_states: 0
+            feature.possible_transitions: 1
+            0....1....2....3....4....5....6....7....8....9....10
+            Number of features: 150
+            Seconds required: 0.001
+            ...
+            Writing feature references for attributes
+            Seconds required: 0.000
+
+            training time: 0.01 sec
+
+        Args:
+            tagged_list: جملاتی که مدل از روی آن‌ها آموزش می‌بیند.
+            c1: مقدار L1 regularization.
+            c2: مقدار L2 regularization.
+            max_iteration: تعداد تکرار آموزش بر کل دیتا.
+            verbose: نمایش اطلاعات مربوط به آموزش.
+            file_name: نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
+            report_duration: نمایش گزارشات مربوط به زمان.
+
+        """
+        tagged_list = [
+            [((word, tag), chunk) for word, tag, chunk in tagged_sent]
+            for tagged_sent in tagged_list
+        ]
+        return super().train(
+            tagged_list,
+            c1,
+            c2,
+            max_iteration,
+            verbose,
+            file_name,
+            report_duration,
+        )
+
+    def evaluate(
+        self: "SequenceTagger", tagged_sent: List[List[Tuple[str, str, str]]],
+    ) -> float:
+        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
+
+        Examples:
+            >>> iobTagger = IOBTagger(model = 'tagger.model')
+            >>> iobTagger.evaluate([[('نامه', 'NOUN,EZ', 'B-NP'), ('ایشان', 'PRON', 'I-NP'), ('را', 'ADP', 'B-POSTP'), ('دریافت', 'NOUN', 'B-VP'), ('داشتم', 'VERB', 'I-VP'), ('.', 'PUNCT', 'O')]])
+            1.0
+
+
+        Args:
+            tagged_sent: جملات لیبل‌داری که با استفاده از آن مدل را ارزیابی می‌کنیم.
+
+        Returns:
+            دقت مدل
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        def extract_labels(tagged_list):
+            return [[token[-1] for token in sent] for sent in tagged_list]
+
+        tokens = [[token[:-1] for token in sent] for sent in tagged_sent]
+        predicted_tagged_sent = self.tag_sents(tokens)
+        return super()._SequenceTagger__evaluate(
+            extract_labels(tagged_sent),
+            extract_labels(predicted_tagged_sent),
+        )
```

### Comparing `hazm-0.9.0/hazm/stemmer.py` & `hazm-0.9.1/hazm/stemmer.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای ریشه‌یابی کلمات است.
-
-فرق بین [Lemmatizer](./lemmatizer.md) و [Stemmer](./stemmer.md) این است که
-اِستمر درکی از معنای کلمه ندارد و صرفاً براساس حذف برخی از پسوندهای ساده تلاش
-می‌کند ریشهٔ کلمه را بیابد؛ بنابراین ممکن است در ریشه‌یابیِ برخی از کلمات نتایج
-نادرستی ارائه دهد؛ اما لماتایزر براساس لیستی از کلمات مرجع به همراه ریشهٔ آن
-این
-کار را انجام می‌دهد و نتایج دقیق‌تری ارائه می‌دهد. البته هزینهٔ این دقت، سرعتِ
-کمتر در ریشه‌یابی است.
-
-"""
-
-
-from nltk.stem.api import StemmerI
-
-
-class Stemmer(StemmerI):
-    """این کلاس شامل توابعی برای ریشه‌یابی کلمات است."""
-
-    def __init__(self: "Stemmer") -> None:
-        self.ends = [
-            "ات",
-            "ان",
-            "ترین",
-            "تر",
-            "م",
-            "ت",
-            "ش",
-            "یی",
-            "ی",
-            "ها",
-            "ٔ",
-            "‌ا",
-            "‌",
-        ]
-
-    def stem(self: "Stemmer", word: str) -> str:
-        """ریشهٔ کلمه را پیدا می‌کند.
-
-        Examples:
-            >>> stemmer = Stemmer()
-            >>> stemmer.stem('کتابی')
-            'کتاب'
-            >>> stemmer.stem('کتاب‌ها')
-            'کتاب'
-            >>> stemmer.stem('کتاب‌هایی')
-            'کتاب'
-            >>> stemmer.stem('کتابهایشان')
-            'کتاب'
-            >>> stemmer.stem('اندیشه‌اش')
-            'اندیشه'
-            >>> stemmer.stem('خانۀ')
-            'خانه'
-            >>> stemmer.stem('محبوب‌ترین‌ها')
-            'محبوب'
-
-        Args:
-            word: کلمه‌ای که باید ریشهٔ آن پیدا شود.
-
-        Returns:
-            ریشهٔ کلمه.
-
-        """
-        if word.endswith("ۀ"):
-            word = word[:-1] + "ه"
-
-        else:
-            iteration = len(self.ends)
-            while iteration:
-                for end in self.ends:
-                    if word.endswith(end):
-                        word = word[: -len(end)]
-                iteration -= 1
-
-        return word
+"""این ماژول شامل کلاس‌ها و توابعی برای ریشه‌یابی کلمات است.
+
+فرق بین [Lemmatizer](./lemmatizer.md) و [Stemmer](./stemmer.md) این است که
+اِستمر درکی از معنای کلمه ندارد و صرفاً براساس حذف برخی از پسوندهای ساده تلاش
+می‌کند ریشهٔ کلمه را بیابد؛ بنابراین ممکن است در ریشه‌یابیِ برخی از کلمات نتایج
+نادرستی ارائه دهد؛ اما لماتایزر براساس لیستی از کلمات مرجع به همراه ریشهٔ آن
+این
+کار را انجام می‌دهد و نتایج دقیق‌تری ارائه می‌دهد. البته هزینهٔ این دقت، سرعتِ
+کمتر در ریشه‌یابی است.
+
+"""
+
+
+from nltk.stem.api import StemmerI
+
+
+class Stemmer(StemmerI):
+    """این کلاس شامل توابعی برای ریشه‌یابی کلمات است."""
+
+    def __init__(self: "Stemmer") -> None:
+        self.ends = [
+            "ات",
+            "ان",
+            "ترین",
+            "تر",
+            "م",
+            "ت",
+            "ش",
+            "یی",
+            "ی",
+            "ها",
+            "ٔ",
+            "‌ا",
+            "‌",
+        ]
+
+    def stem(self: "Stemmer", word: str) -> str:
+        """ریشهٔ کلمه را پیدا می‌کند.
+
+        Examples:
+            >>> stemmer = Stemmer()
+            >>> stemmer.stem('کتابی')
+            'کتاب'
+            >>> stemmer.stem('کتاب‌ها')
+            'کتاب'
+            >>> stemmer.stem('کتاب‌هایی')
+            'کتاب'
+            >>> stemmer.stem('کتابهایشان')
+            'کتاب'
+            >>> stemmer.stem('اندیشه‌اش')
+            'اندیشه'
+            >>> stemmer.stem('خانۀ')
+            'خانه'
+            >>> stemmer.stem('محبوب‌ترین‌ها')
+            'محبوب'
+
+        Args:
+            word: کلمه‌ای که باید ریشهٔ آن پیدا شود.
+
+        Returns:
+            ریشهٔ کلمه.
+
+        """
+        if word.endswith("ۀ"):
+            word = word[:-1] + "ه"
+
+        else:
+            iteration = len(self.ends)
+            while iteration:
+                for end in self.ends:
+                    if word.endswith(end):
+                        word = word[: -len(end)]
+                iteration -= 1
+
+        return word
```

### Comparing `hazm-0.9.0/hazm/token_splitter.py` & `hazm-0.9.1/hazm/token_splitter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای تجزیه توکن به دو توکن کوچکتر است."""
-
-
-from typing import List
-from typing import Tuple
-
-from hazm import Lemmatizer
-
-
-class TokenSplitter:
-    """این کلاس شامل توابعی برای تجزیه توکن به دو توکن کوچکتر است."""
-
-    def __init__(self: "TokenSplitter") -> None:
-        self.lemmatizer = Lemmatizer()
-        self.lemmatize = self.lemmatizer.lemmatize
-        self.words = self.lemmatizer.words
-
-    def split_token_words(self: "TokenSplitter", token: str) -> List[Tuple[str, str]]:
-        """توکنِ ورودی را به دو توکن کوچکتر تجزیه می‌کند.
-
-        اگر توکن به بیش از یک روش قابل تجزیه باشد همهٔ حالت‌های ممکن را
-        برمی‌گرداند؛ مثلاً «داستان‌سرا» هم می‌توان به `['داستان', 'سرا']` تجزیه
-        شود و هم می‌تواند به `['داستان‌سرا',]` شکسته شود؛ پس هر دو را
-        برمی‌گرداند: `[('داستان', 'سرا'), ('داستان‌سرا',)]`.
-
-        Examples:
-            >>> splitter = TokenSplitter()
-            >>> splitter.split_token_words('صداوسیماجمهوری')
-            [('صداوسیما', 'جمهوری')]
-            >>> splitter.split_token_words('صداو')
-            [('صد', 'او'), ('صدا', 'و')]
-            >>> splitter.split_token_words('داستان‌سرا')
-            [('داستان', 'سرا'), ('داستان‌سرا',)]
-            >>> splitter.split_token_words('دستان‌سرا')
-            [('دستان', 'سرا')]
-
-        Args:
-            token: توکنی که باید پردازش شود.
-
-        Returns:
-            <dir-rtl>لیستی از `[(توکن, توکن), (توکن, توکن), …]`ها.</dir-rtl>
-
-        """
-        # >>> splitter.split_token_words('شهرموشها')
-
-        candidates = []
-        if "‌" in token:
-            candidates.append(tuple(token.split("‌")))
-
-        splits = [
-            (token[:s], token[s:])
-            for s in range(1, len(token))
-            if token[s - 1] != "‌" and token[s] != "‌"
-        ] + [(token,)]
-        candidates.extend(
-            list(
-                filter(
-                    lambda tokens: set(map(self.lemmatize, tokens)).issubset(
-                        self.words,
-                    ),
-                    splits,
-                ),
-            ),
-        )
-
-        return candidates
+"""این ماژول شامل کلاس‌ها و توابعی برای تجزیه توکن به دو توکن کوچکتر است."""
+
+
+from typing import List
+from typing import Tuple
+
+from hazm import Lemmatizer
+
+
+class TokenSplitter:
+    """این کلاس شامل توابعی برای تجزیه توکن به دو توکن کوچکتر است."""
+
+    def __init__(self: "TokenSplitter") -> None:
+        self.lemmatizer = Lemmatizer()
+        self.lemmatize = self.lemmatizer.lemmatize
+        self.words = self.lemmatizer.words
+
+    def split_token_words(self: "TokenSplitter", token: str) -> List[Tuple[str, str]]:
+        """توکنِ ورودی را به دو توکن کوچکتر تجزیه می‌کند.
+
+        اگر توکن به بیش از یک روش قابل تجزیه باشد همهٔ حالت‌های ممکن را
+        برمی‌گرداند؛ مثلاً «داستان‌سرا» هم می‌توان به `['داستان', 'سرا']` تجزیه
+        شود و هم می‌تواند به `['داستان‌سرا',]` شکسته شود؛ پس هر دو را
+        برمی‌گرداند: `[('داستان', 'سرا'), ('داستان‌سرا',)]`.
+
+        Examples:
+            >>> splitter = TokenSplitter()
+            >>> splitter.split_token_words('صداوسیماجمهوری')
+            [('صداوسیما', 'جمهوری')]
+            >>> splitter.split_token_words('صداو')
+            [('صد', 'او'), ('صدا', 'و')]
+            >>> splitter.split_token_words('داستان‌سرا')
+            [('داستان', 'سرا'), ('داستان‌سرا',)]
+            >>> splitter.split_token_words('دستان‌سرا')
+            [('دستان', 'سرا')]
+
+        Args:
+            token: توکنی که باید پردازش شود.
+
+        Returns:
+            <dir-rtl>لیستی از `[(توکن, توکن), (توکن, توکن), …]`ها.</dir-rtl>
+
+        """
+        # >>> splitter.split_token_words('شهرموشها')
+
+        candidates = []
+        if "‌" in token:
+            candidates.append(tuple(token.split("‌")))
+
+        splits = [
+            (token[:s], token[s:])
+            for s in range(1, len(token))
+            if token[s - 1] != "‌" and token[s] != "‌"
+        ] + [(token,)]
+        candidates.extend(
+            list(
+                filter(
+                    lambda tokens: set(map(self.lemmatize, tokens)).issubset(
+                        self.words,
+                    ),
+                    splits,
+                ),
+            ),
+        )
+
+        return candidates
```

### Comparing `hazm-0.9.0/hazm/utils.py` & `hazm-0.9.1/hazm/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-"""این ماژول شامل کلاس‌ها و توابع کمکی است."""
-
-import re
-from os import path
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Tuple
-
-data_path = Path(__file__).parent / "data"
-
-default_words = Path(data_path) / "words.dat"
-default_stopwords = Path(data_path) / "stopwords.dat"
-default_verbs = Path(data_path) / "verbs.dat"
-informal_words = Path(data_path) / "iwords.dat"
-informal_verbs = Path(data_path) / "iverbs.dat"
-
-NUMBERS = "۰۱۲۳۴۵۶۷۸۹"
-
-
-def maketrans(a: str, b: str) -> Dict[int, Any]:
-    """هر یک از حروف رشتهٔ a را به یک حرف در رشتهٔ b مپ می‌کند."""
-    return {ord(a): b for a, b in zip(a, b)}
-
-
-def words_list(
-    words_file: str = default_words,
-) -> List[Tuple[str, int, Tuple[str]]]:
-    """لیست کلمات را برمی‌گرداند.
-
-    Examples:
-        >>> from hazm.utils import words_list
-        >>> words_list()[1]
-        ('آب', 549005877, ('N', 'AJ'))
-
-    Args:
-        words_file: مسیر فایل حاوی کلمات.
-
-    Returns:
-        فهرست کلمات.
-
-    """
-    with Path.open(words_file, encoding="utf-8") as words_file:
-        items = [line.strip().split("\t") for line in words_file]
-        return [
-            (item[0], int(item[1]), tuple(item[2].split(",")))
-            for item in items
-            if len(item) == 3
-        ]
-
-
-def stopwords_list(stopwords_file: str = default_stopwords) -> List[str]:
-    """لیست ایست‌واژه‌ها را برمی‌گرداند.
-
-    Examples:
-        >>> from hazm.utils import stopwords_list
-        >>> stopwords_list()[:4]
-        ['آخرین', 'آقای', 'آمد', 'آمده']
-
-    Args:
-        stopwords_file: مسیر فایل حاوی ایست‌واژه‌ها.
-
-    Returns:
-        فهرست ایست‌واژه‌ها.
-
-    """
-    with Path.open(stopwords_file, encoding="utf8") as stopwords_file:
-        return sorted({w.strip() for w in stopwords_file})
-
-
-def verbs_list() -> List[str]:
-    """لیست افعال را برمی‌گرداند."""
-    with Path.open(default_verbs, encoding="utf8") as verbs_file:
-        lst = []
-        for line in verbs_file:
-            lst.append(line.strip())
-        return lst
-
-
-def past_roots() -> str:
-    """لیست بن‌های گذشته را برمی‌گرداند."""
-    roots = ""
-    for verb in verbs_list():
-        split = verb.split("#")
-        roots += split[0] + "|"
-
-    return roots[:-1]
-
-
-def present_roots() -> str:
-    """لیست بن‌های مضارع را برمی‌گرداند."""
-    roots = ""
-    for verb in verbs_list():
-        split = verb.split("#")
-        roots += split[1] + "|"
-
-    return roots[:-1]
-
-
-def regex_replace(patterns: str, text: str) -> str:
-    """الگوی ریجکس را یافته و با متن داده شده جایگزین می‌کند."""
-    for pattern, repl in patterns:
-        text = re.sub(pattern, repl, text)
-    return text
-
+"""این ماژول شامل کلاس‌ها و توابع کمکی است."""
+
+import re
+from os import path
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Tuple
+
+data_path = Path(__file__).parent / "data"
+
+default_words = Path(data_path) / "words.dat"
+default_stopwords = Path(data_path) / "stopwords.dat"
+default_verbs = Path(data_path) / "verbs.dat"
+informal_words = Path(data_path) / "iwords.dat"
+informal_verbs = Path(data_path) / "iverbs.dat"
+
+NUMBERS = "۰۱۲۳۴۵۶۷۸۹"
+
+
+def maketrans(a: str, b: str) -> Dict[int, Any]:
+    """هر یک از حروف رشتهٔ a را به یک حرف در رشتهٔ b مپ می‌کند."""
+    return {ord(a): b for a, b in zip(a, b)}
+
+
+def words_list(
+    words_file: str = default_words,
+) -> List[Tuple[str, int, Tuple[str]]]:
+    """لیست کلمات را برمی‌گرداند.
+
+    Examples:
+        >>> from hazm.utils import words_list
+        >>> words_list()[1]
+        ('آب', 549005877, ('N', 'AJ'))
+
+    Args:
+        words_file: مسیر فایل حاوی کلمات.
+
+    Returns:
+        فهرست کلمات.
+
+    """
+    with Path.open(words_file, encoding="utf-8") as words_file:
+        items = [line.strip().split("\t") for line in words_file]
+        return [
+            (item[0], int(item[1]), tuple(item[2].split(",")))
+            for item in items
+            if len(item) == 3
+        ]
+
+
+def stopwords_list(stopwords_file: str = default_stopwords) -> List[str]:
+    """لیست ایست‌واژه‌ها را برمی‌گرداند.
+
+    Examples:
+        >>> from hazm.utils import stopwords_list
+        >>> stopwords_list()[:4]
+        ['آخرین', 'آقای', 'آمد', 'آمده']
+
+    Args:
+        stopwords_file: مسیر فایل حاوی ایست‌واژه‌ها.
+
+    Returns:
+        فهرست ایست‌واژه‌ها.
+
+    """
+    with Path.open(stopwords_file, encoding="utf8") as stopwords_file:
+        return sorted({w.strip() for w in stopwords_file})
+
+
+def verbs_list() -> List[str]:
+    """لیست افعال را برمی‌گرداند."""
+    with Path.open(default_verbs, encoding="utf8") as verbs_file:
+        lst = []
+        for line in verbs_file:
+            lst.append(line.strip())
+        return lst
+
+
+def past_roots() -> str:
+    """لیست بن‌های گذشته را برمی‌گرداند."""
+    roots = ""
+    for verb in verbs_list():
+        split = verb.split("#")
+        roots += split[0] + "|"
+
+    return roots[:-1]
+
+
+def present_roots() -> str:
+    """لیست بن‌های مضارع را برمی‌گرداند."""
+    roots = ""
+    for verb in verbs_list():
+        split = verb.split("#")
+        roots += split[1] + "|"
+
+    return roots[:-1]
+
+
+def regex_replace(patterns: str, text: str) -> str:
+    """الگوی ریجکس را یافته و با متن داده شده جایگزین می‌کند."""
+    for pattern, repl in patterns:
+        text = re.sub(pattern, repl, text)
+    return text
+
```

### Comparing `hazm-0.9.0/PKG-INFO` & `hazm-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hazm
-Version: 0.9.0
+Version: 0.9.1
 Summary: Persian NLP Toolkit
 Home-page: https://roshan-ai.ir/hazm/
 License: MIT
 Keywords: nlp,persian nlp,persian
 Author: Roshan
 Author-email: salam@roshan-ai.com
 Maintainer: Roshan
```

