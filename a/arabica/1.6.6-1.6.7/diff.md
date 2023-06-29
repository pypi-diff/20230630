# Comparing `tmp/arabica-1.6.6.tar.gz` & `tmp/arabica-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.6.6.tar", last modified: Thu Jun 29 20:11:21 2023, max compression
+gzip compressed data, was "arabica-1.6.7.tar", last modified: Thu Jun 29 22:45:36 2023, max compression
```

## Comparing `arabica-1.6.6.tar` & `arabica-1.6.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:11:21.373956 arabica-1.6.6/
--rw-rw-rw-   0        0        0       39 2023-06-29 19:51:45.000000 arabica-1.6.6/LICENSE
--rw-rw-rw-   0        0        0     7856 2023-06-29 20:11:21.373956 arabica-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     7051 2023-06-29 20:05:24.000000 arabica-1.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 20:11:21.360312 arabica-1.6.6/arabica/
--rw-rw-rw-   0        0        0      105 2023-06-29 20:10:39.000000 arabica-1.6.6/arabica/__init__.py
--rw-rw-rw-   0        0        0    11892 2023-06-22 16:47:25.000000 arabica-1.6.6/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    31618 2023-06-29 18:51:09.000000 arabica-1.6.6/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.6/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.6/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.6/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.6/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.6/arabica/preprocess.py
--rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.6/arabica/sentiment.py
--rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.6/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:11:21.360312 arabica-1.6.6/arabica.egg-info/
--rw-rw-rw-   0        0        0     7856 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-29 20:11:21.000000 arabica-1.6.6/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      559 2023-06-29 20:10:39.000000 arabica-1.6.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 20:11:21.373956 arabica-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1154 2023-06-29 20:10:39.000000 arabica-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:45:36.838075 arabica-1.6.7/
+-rw-rw-rw-   0        0        0       39 2023-06-29 19:51:45.000000 arabica-1.6.7/LICENSE
+-rw-rw-rw-   0        0        0     7815 2023-06-29 22:45:36.838075 arabica-1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7012 2023-06-29 22:20:39.000000 arabica-1.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 22:45:36.838075 arabica-1.6.7/arabica/
+-rw-rw-rw-   0        0        0      105 2023-06-29 22:43:08.000000 arabica-1.6.7/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11892 2023-06-22 16:47:25.000000 arabica-1.6.7/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    31618 2023-06-29 18:51:09.000000 arabica-1.6.7/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.7/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.7/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.7/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.7/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.7/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.7/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.7/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:45:36.838075 arabica-1.6.7/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7815 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      557 2023-06-29 22:44:49.000000 arabica-1.6.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:45:36.838075 arabica-1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-06-29 22:44:49.000000 arabica-1.6.7/setup.py
```

### Comparing `arabica-1.6.6/PKG-INFO` & `arabica-1.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, !=3.11
+Requires-Python: >3.9, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arabica
 **Python package for exploratory text data analysis**
 
 Text data is often recorded as a time series with significant variability over time. Some examples of time-series text data include Twitter tweets, research article metadata, product reviews, and newspaper headlines. Arabica makes exploratory analysis of these time-series text datasets simple by providing:
@@ -38,15 +38,15 @@
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
 * **European-style**: *DD/MM/YYYY* (2013-31-12, 09-Feb-2009, 2013-31-12 11:46:17, etc.) date and datetime formats.
 
 
 ## Installation
 
-Arabica requires [Python 3.8 - 3.10](https://www.python.org/downloads/), [NLTK](http://www.nltk.org) - stop words removal,
+Arabica requires **Python 3.10**, [NLTK](http://www.nltk.org) - stop words removal,
 [cleantext](https://pypi.org/project/cleantext/#description) - text cleaning, [wordcloud](https://pypi.org/project/wordcloud) - word cloud visualization,
 [plotnine](https://pypi.org/project/plotnine) - heatmaps and line graphs, [matplotlib](https://pypi.org/project/matplotlib/) - word clouds and graphical operations,
 [vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, [finvader](https://pypi.org/project/finvader) - financial sentiment analysis,
 and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
 
 To install using pip, use:
```

### Comparing `arabica-1.6.6/README.md` & `arabica-1.6.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
 * **European-style**: *DD/MM/YYYY* (2013-31-12, 09-Feb-2009, 2013-31-12 11:46:17, etc.) date and datetime formats.
 
 
 ## Installation
 
-Arabica requires [Python 3.8 - 3.10](https://www.python.org/downloads/), [NLTK](http://www.nltk.org) - stop words removal,
+Arabica requires **Python 3.10**, [NLTK](http://www.nltk.org) - stop words removal,
 [cleantext](https://pypi.org/project/cleantext/#description) - text cleaning, [wordcloud](https://pypi.org/project/wordcloud) - word cloud visualization,
 [plotnine](https://pypi.org/project/plotnine) - heatmaps and line graphs, [matplotlib](https://pypi.org/project/matplotlib/) - word clouds and graphical operations,
 [vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, [finvader](https://pypi.org/project/finvader) - financial sentiment analysis,
 and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
 
 To install using pip, use:
```

### Comparing `arabica-1.6.6/arabica/arabica_freq.py` & `arabica-1.6.7/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.6/arabica/cappuccino.py` & `arabica-1.6.7/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.6/arabica/clean_ngram.py` & `arabica-1.6.7/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.6/arabica/coffee_break.py` & `arabica-1.6.7/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.6/arabica/group.py` & `arabica-1.6.7/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.6/arabica/preprocess.py` & `arabica-1.6.7/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.6/arabica/sentiment.py` & `arabica-1.6.7/arabica/sentiment.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.6/arabica.egg-info/PKG-INFO` & `arabica-1.6.7/arabica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, !=3.11
+Requires-Python: >3.9, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arabica
 **Python package for exploratory text data analysis**
 
 Text data is often recorded as a time series with significant variability over time. Some examples of time-series text data include Twitter tweets, research article metadata, product reviews, and newspaper headlines. Arabica makes exploratory analysis of these time-series text datasets simple by providing:
@@ -38,15 +38,15 @@
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
 * **European-style**: *DD/MM/YYYY* (2013-31-12, 09-Feb-2009, 2013-31-12 11:46:17, etc.) date and datetime formats.
 
 
 ## Installation
 
-Arabica requires [Python 3.8 - 3.10](https://www.python.org/downloads/), [NLTK](http://www.nltk.org) - stop words removal,
+Arabica requires **Python 3.10**, [NLTK](http://www.nltk.org) - stop words removal,
 [cleantext](https://pypi.org/project/cleantext/#description) - text cleaning, [wordcloud](https://pypi.org/project/wordcloud) - word cloud visualization,
 [plotnine](https://pypi.org/project/plotnine) - heatmaps and line graphs, [matplotlib](https://pypi.org/project/matplotlib/) - word clouds and graphical operations,
 [vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, [finvader](https://pypi.org/project/finvader) - financial sentiment analysis,
 and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
 
 To install using pip, use:
```

### Comparing `arabica-1.6.6/pyproject.toml` & `arabica-1.6.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 [project]
 name = "arabica"
-version = "1.6.6"
+version = "1.6.7"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.8, !=3.11"
+requires-python = ">3.9, <3.11"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `arabica-1.6.6/setup.py` & `arabica-1.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.6.6",
+        version="1.6.7",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
-        python_requires='>=3.8, !=3.11',
+        python_requires='>3.9, <3.11',
         install_requires = ['pandas == 1.4.0',
                             'nltk == 3.6.2',
                             'regex == 2022.10.31',
                             'finvader',
                             'matplotlib == 3.6.0',
                             'matplotlib-inline == 0.1.6',
                             'plotnine == 0.10.1',
```

