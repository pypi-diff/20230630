# Comparing `tmp/mmct-1.1.1.tar.gz` & `tmp/mmct-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/christian/mmct/dist/tmpk7liv30j/mmct-1.1.1.tar", last modified: Fri Apr 23 20:13:31 2021, max compression
+gzip compressed data, was "mmct-1.1.3.tar", last modified: Fri Jun 30 19:24:25 2023, max compression
```

## Comparing `mmct-1.1.1.tar` & `mmct-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2021-04-23 20:13:31.513814 mmct-1.1.1/
--rw-rw-r--   0 christian  (1000) christian  (1000)     1083 2021-04-10 14:11:09.000000 mmct-1.1.1/LICENSE
--rw-rw-r--   0 christian  (1000) christian  (1000)     4570 2021-04-23 20:13:31.513814 mmct-1.1.1/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)     3713 2021-04-23 20:13:04.000000 mmct-1.1.1/README.md
--rw-rw-r--   0 christian  (1000) christian  (1000)      104 2021-04-17 20:55:56.000000 mmct-1.1.1/pyproject.toml
--rw-rw-r--   0 christian  (1000) christian  (1000)      612 2021-04-23 20:13:31.513814 mmct-1.1.1/setup.cfg
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2021-04-23 20:13:31.513814 mmct-1.1.1/src/
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2021-04-23 20:13:31.513814 mmct-1.1.1/src/mmct/
--rw-rw-r--   0 christian  (1000) christian  (1000)       43 2021-04-17 20:55:56.000000 mmct-1.1.1/src/mmct/__init__.py
--rw-rw-r--   0 christian  (1000) christian  (1000)      762 2021-04-23 20:13:04.000000 mmct-1.1.1/src/mmct/stat.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     3008 2021-04-23 20:13:04.000000 mmct-1.1.1/src/mmct/tester.py
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2021-04-23 20:13:31.513814 mmct-1.1.1/src/mmct.egg-info/
--rw-rw-r--   0 christian  (1000) christian  (1000)     4570 2021-04-23 20:13:31.000000 mmct-1.1.1/src/mmct.egg-info/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)      265 2021-04-23 20:13:31.000000 mmct-1.1.1/src/mmct.egg-info/SOURCES.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)        1 2021-04-23 20:13:31.000000 mmct-1.1.1/src/mmct.egg-info/dependency_links.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)        5 2021-04-23 20:13:31.000000 mmct-1.1.1/src/mmct.egg-info/top_level.txt
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2021-04-23 20:13:31.513814 mmct-1.1.1/test/
--rw-rw-r--   0 christian  (1000) christian  (1000)     1659 2021-04-23 20:13:04.000000 mmct-1.1.1/test/test_stat.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     3696 2021-04-23 20:13:04.000000 mmct-1.1.1/test/test_tester.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2023-06-30 19:24:25.148250 mmct-1.1.3/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1083 2023-06-30 14:48:20.000000 mmct-1.1.3/LICENSE
+-rw-rw-r--   0 christian  (1000) christian  (1000)     3066 2023-06-30 19:24:25.148250 mmct-1.1.3/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2555 2023-06-30 19:01:05.000000 mmct-1.1.3/README.md
+-rw-rw-r--   0 christian  (1000) christian  (1000)      520 2023-06-30 14:48:20.000000 mmct-1.1.3/pyproject.toml
+-rw-rw-r--   0 christian  (1000) christian  (1000)      851 2023-06-30 19:24:25.148250 mmct-1.1.3/setup.cfg
+-rw-rw-r--   0 christian  (1000) christian  (1000)       66 2023-06-30 14:48:20.000000 mmct-1.1.3/setup.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2023-06-30 19:24:25.148250 mmct-1.1.3/src/
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2023-06-30 19:24:25.148250 mmct-1.1.3/src/mmct/
+-rw-rw-r--   0 christian  (1000) christian  (1000)       28 2023-06-30 14:48:20.000000 mmct-1.1.3/src/mmct/__init__.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2880 2023-06-30 19:01:05.000000 mmct-1.1.3/src/mmct/core.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2023-06-30 19:24:25.148250 mmct-1.1.3/src/mmct.egg-info/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     3066 2023-06-30 19:24:25.000000 mmct-1.1.3/src/mmct.egg-info/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)      266 2023-06-30 19:24:25.000000 mmct-1.1.3/src/mmct.egg-info/SOURCES.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)        1 2023-06-30 19:24:25.000000 mmct-1.1.3/src/mmct.egg-info/dependency_links.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)       96 2023-06-30 19:24:25.000000 mmct-1.1.3/src/mmct.egg-info/requires.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)        5 2023-06-30 19:24:25.000000 mmct-1.1.3/src/mmct.egg-info/top_level.txt
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2023-06-30 19:24:25.148250 mmct-1.1.3/test/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2080 2023-06-30 19:01:05.000000 mmct-1.1.3/test/test_core.py
```

### Comparing `mmct-1.1.1/LICENSE` & `mmct-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mmct-1.1.1/README.md` & `mmct-1.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,61 @@
+Metadata-Version: 2.1
+Name: mmct
+Version: 1.1.3
+Summary: Multinomial Monte Carlo testing
+Home-page: https://github.com/cwand/mmct
+Author: Chris Walther Andersen
+Author-email: cvvand@gmail.com
+Project-URL: Bug Tracker, https://github.com/cwand/mmct/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
 # mmct
 
 Provides functionality for performing multinomial tests using monte carlo simulation
 
-## Background
-
-This library contain python code that can be used to test whether a given set of observations are likely to be drawn from a multinomial distribution with a given set of parameters \(probabilities for each case\). Specifically, let X = \(x1,x2,...,xk\), where xi is the number of times we observed outcome i. We want to test whether X is taken from a multinomial distribution with probabilities p1, p2,...,pk, where p1,+p2+...+pk = 1. As is standard we quantify the test with a p-value, i.e. the probability of, by pure randomness, to get a result that is as bad or worse than X.
+![Tests](https://github.com/cwand/mmct/actions/workflows/tests.yml/badge.svg)
 
-To measure what we mean by "as bad or worse" we use the log-likelihood ratio, LLR (default), or the multinomial probability function. This is explained in the context of multinomial tests in an equivalent package for the R programming language [here](https://cran.r-project.org/web/packages/XNomial/vignettes/XNomial.html). Basically, a variable that _exactly_ follows the hypothesised distribution will get a LLR of 0. Any other distribution will have an LLR smaller than 0, with more unlikely distributions getting smaller and smaller. E.g., rolling three times with a fair dice you could roll two ones and a six. That would get you an LLR of -3.47. Rolling three ones would score an LLR of -5.38.
-
-In order to perform the test we generate a bunch of random samples from the null-hypothesis distribution, each with the same number of total observations as the item under test \(N = x1+x2+...+xk\). We order all of these random samples according to their log-likelihood ratio, LLR and compare with the LLR of the item under test. The p-value is simply the fraction of the random samples with an LLR smaller than that of the item under test.
+## Background
 
-The library is inspired by [met](https://pypi.org/project/met/), which achieve the same objective as mmct, but does so by painstakingly enumerating every possible case for the given multinomial distribution and calculating the p-value exactly. While this is certainly preferable, it becomes very slow very quickly, so for performing many tests or tests with a large parameter space, a monte carlo approximation may be good enough. As already mentioned, mmct has also drawn inspiration from the [XNomial](https://cran.r-project.org/web/packages/XNomial/vignettes/XNomial.html) package, which performs an identical task in the R programming language.
+This library contain python code that can be used to test whether a given set of observations are
+likely to be drawn from a multinomial distribution with a given set of parameters (probabilities
+for each case). The test is done using Monte Carlo methods. A bunch of random samples from the
+hypothesised distribution is drawn and the probability of each sample is calculated.  These are all
+compared to the probability of the sample under test. The p-value of the null-hypothesis (that the 
+sample comes from the distribution) is simply the fraction of random samples with probability
+smaller than the sample under test.
+
+The library is inspired by [met](https://pypi.org/project/met/), which achieve the same objective
+as mmct, but does so by painstakingly enumerating every possible case for the given multinomial
+distribution and calculating the p-value exactly. While this is certainly preferable, it becomes
+very slow very quickly, so for performing many tests or tests with a large parameter space, a
+monte carlo approximation may be good enough. mmct has also drawn inspiration
+from the [XNomial](https://cran.r-project.org/web/packages/XNomial/vignettes/XNomial.html) package,
+which performs an identical task in the R programming language.
 
 ## Usage
 
 The package is most easlily installed via pip:
 
 ```text
 pip install mmct
 ```
 
-The source code is also available on GitHub and is free for use and modification: [mmct on GitHub](https://github.com/cwand/mmct/)
+The source code is also available on GitHub and is free for use and modification:
+[mmct on GitHub](https://github.com/cwand/mmct/)
 
-When the package has been installed, a test can be performed following the example below, in which we test whether a set of dice rolls could have been generated from rolling two fair dice 20 times and adding the eyes:
+When the package has been installed, a test can be performed following the example below, in which
+we test whether a set of dice rolls could have been generated from rolling two fair dice 20 times
+and adding the eyes:
 
 ```text
 import mmct
 import numpy as np
 #     Eyes    2  3  4  5  6  7  8  9 10 11 12
 x = np.array([0, 0, 2, 4, 5, 2, 3, 1, 0, 1, 2])
 # Hypothsised probabilities:
@@ -34,10 +63,10 @@
 # Initialise tester:
 t = mmct.mt_tester() # Use the multithreaded tester class
 # Set number of Monte Carlo samples to generate
 t.n_samples = 100000
 pval = t.do_test(x,p)
 ```
 
-The result of the test will of course vary \(unless the random simulator is seeded\), but should in general result in a p-value around 0.31, i.e. we cannot reject the hypothesis that the numbers above are taken from a fair dice rolling \(which they actually are\).
-
-For more in-depth explanation and code documentation, see the [GitHub Pages](https://cwand.github.io/mmct/)
+The result of the test will of course vary (unless the random simulator is seeded), but should in
+general result in a p-value around 0.34, i.e. we cannot reject the hypothesis that the numbers
+above are taken from a fair dice rolling (which they actually are).
```

### Comparing `mmct-1.1.1/setup.cfg` & `mmct-1.1.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mmct
-version = 1.1.1
+version = 1.1.3
 author = Chris Walther Andersen
 author_email = cvvand@gmail.com
 description = Multinomial Monte Carlo testing
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cwand/mmct
 project_urls = 
@@ -13,17 +13,35 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
-packages = find:
-python_requires = >=3.6
+packages = mmct
+install_requires = 
+	numpy>=1.20
+	scipy>=1.7
+python_requires = >=3.8
 
 [options.packages.find]
 where = src
 
+[options.extras_require]
+testing = 
+	pytest>=6.0
+	pytest-cov>=2.0
+	mypy>=0.910
+	flake8>=3.9
+	tox>=3.24
+
+[options.package_data]
+mmct = py.typed
+
+[flake8]
+max-line-length = 100
+ignore = W191,E128
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

