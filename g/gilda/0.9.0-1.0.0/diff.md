# Comparing `tmp/gilda-0.9.0.tar.gz` & `tmp/gilda-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gilda-0.9.0.tar", last modified: Tue Apr 26 22:56:11 2022, max compression
+gzip compressed data, was "gilda-1.0.0.tar", last modified: Fri Jun 30 15:08:32 2023, max compression
```

## Comparing `gilda-0.9.0.tar` & `gilda-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,60 @@
-drwxr-xr-x   0 ben        (504) staff       (20)        0 2022-04-26 22:56:11.096759 gilda-0.9.0/
--rw-r--r--   0 ben        (504) staff       (20)     1346 2021-02-10 19:17:08.000000 gilda-0.9.0/LICENSE
--rw-r--r--   0 ben        (504) staff       (20)      129 2021-02-10 19:17:08.000000 gilda-0.9.0/MANIFEST.in
--rw-r--r--   0 ben        (504) staff       (20)     6044 2022-04-26 22:56:11.096406 gilda-0.9.0/PKG-INFO
--rw-r--r--   0 ben        (504) staff       (20)     4405 2022-04-26 22:20:20.000000 gilda-0.9.0/README.md
-drwxr-xr-x   0 ben        (504) staff       (20)        0 2022-04-26 22:56:11.070291 gilda-0.9.0/doc/
--rw-r--r--   0 ben        (504) staff       (20)      634 2021-02-10 19:17:08.000000 gilda-0.9.0/doc/Makefile
--rw-r--r--   0 ben        (504) staff       (20)     5502 2022-04-26 22:20:20.000000 gilda-0.9.0/doc/conf.py
--rw-r--r--   0 ben        (504) staff       (20)      341 2022-04-26 22:20:20.000000 gilda-0.9.0/doc/index.rst
--rw-r--r--   0 ben        (504) staff       (20)      795 2021-02-10 19:17:08.000000 gilda-0.9.0/doc/make.bat
-drwxr-xr-x   0 ben        (504) staff       (20)        0 2022-04-26 22:56:11.071502 gilda-0.9.0/doc/modules/
--rw-r--r--   0 ben        (504) staff       (20)      452 2021-02-10 19:17:08.000000 gilda-0.9.0/doc/modules/index.rst
--rw-r--r--   0 ben        (504) staff       (20)      124 2022-04-26 22:20:20.000000 gilda-0.9.0/doc/requirements.txt
-drwxr-xr-x   0 ben        (504) staff       (20)        0 2022-04-26 22:56:11.075286 gilda-0.9.0/gilda/
--rw-r--r--   0 ben        (504) staff       (20)      521 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/__init__.py
--rw-r--r--   0 ben        (504) staff       (20)     7250 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/api.py
-drwxr-xr-x   0 ben        (504) staff       (20)        0 2022-04-26 22:56:11.081214 gilda-0.9.0/gilda/app/
--rw-r--r--   0 ben        (504) staff       (20)      338 2021-02-10 19:17:08.000000 gilda-0.9.0/gilda/app/__init__.py
--rw-r--r--   0 ben        (504) staff       (20)       59 2021-09-05 00:38:55.000000 gilda-0.9.0/gilda/app/__main__.py
--rw-r--r--   0 ben        (504) staff       (20)    11525 2022-04-14 20:13:56.000000 gilda-0.9.0/gilda/app/app.py
--rw-r--r--   0 ben        (504) staff       (20)    28879 2022-04-14 20:13:56.000000 gilda-0.9.0/gilda/generate_terms.py
--rwxr-xr-x   0 ben        (504) staff       (20)     1584 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/greek_alphabet.py
--rw-r--r--   0 ben        (504) staff       (20)    23848 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/grounder.py
--rw-r--r--   0 ben        (504) staff       (20)     7377 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/process.py
-drwxr-xr-x   0 ben        (504) staff       (20)        0 2022-04-26 22:56:11.087943 gilda-0.9.0/gilda/resources/
--rw-r--r--   0 ben        (504) staff       (20)     2845 2022-04-14 20:13:56.000000 gilda-0.9.0/gilda/resources/__init__.py
--rw-r--r--   0 ben        (504) staff       (20)      130 2021-09-05 00:38:55.000000 gilda-0.9.0/gilda/resources/__main__.py
--rw-r--r--   0 ben        (504) staff       (20)    29081 2021-02-10 19:17:08.000000 gilda-0.9.0/gilda/resources/mesh_ambig_mappings.tsv
--rw-r--r--   0 ben        (504) staff       (20)   362152 2021-02-10 19:17:08.000000 gilda-0.9.0/gilda/resources/mesh_mappings.tsv
--rw-r--r--   0 ben        (504) staff       (20)     8564 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/scorer.py
--rw-r--r--   0 ben        (504) staff       (20)     4834 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/term.py
-drwxr-xr-x   0 ben        (504) staff       (20)        0 2022-04-26 22:56:11.095686 gilda-0.9.0/gilda/tests/
--rw-r--r--   0 ben        (504) staff       (20)       47 2021-02-10 19:17:08.000000 gilda-0.9.0/gilda/tests/__init__.py
--rw-r--r--   0 ben        (504) staff       (20)     2022 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/tests/test_api.py
--rw-r--r--   0 ben        (504) staff       (20)     2380 2022-04-14 20:13:56.000000 gilda-0.9.0/gilda/tests/test_app.py
--rw-r--r--   0 ben        (504) staff       (20)     5321 2022-04-14 20:13:56.000000 gilda-0.9.0/gilda/tests/test_generate_terms.py
--rw-r--r--   0 ben        (504) staff       (20)     7188 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/tests/test_grounder.py
--rw-r--r--   0 ben        (504) staff       (20)     1306 2022-04-14 20:13:56.000000 gilda-0.9.0/gilda/tests/test_process.py
--rw-r--r--   0 ben        (504) staff       (20)     1566 2021-02-10 19:17:08.000000 gilda-0.9.0/gilda/tests/test_scorer.py
--rw-r--r--   0 ben        (504) staff       (20)     1238 2022-04-26 22:20:20.000000 gilda-0.9.0/gilda/tests/test_term.py
-drwxr-xr-x   0 ben        (504) staff       (20)        0 2022-04-26 22:56:11.077802 gilda-0.9.0/gilda.egg-info/
--rw-r--r--   0 ben        (504) staff       (20)     6044 2022-04-26 22:56:10.000000 gilda-0.9.0/gilda.egg-info/PKG-INFO
--rw-r--r--   0 ben        (504) staff       (20)      860 2022-04-26 22:56:10.000000 gilda-0.9.0/gilda.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (504) staff       (20)        1 2022-04-26 22:56:10.000000 gilda-0.9.0/gilda.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (504) staff       (20)       42 2022-04-26 22:56:10.000000 gilda-0.9.0/gilda.egg-info/entry_points.txt
--rw-r--r--   0 ben        (504) staff       (20)      255 2022-04-26 22:56:10.000000 gilda-0.9.0/gilda.egg-info/requires.txt
--rw-r--r--   0 ben        (504) staff       (20)        6 2022-04-26 22:56:10.000000 gilda-0.9.0/gilda.egg-info/top_level.txt
--rw-r--r--   0 ben        (504) staff       (20)       38 2022-04-26 22:56:11.096849 gilda-0.9.0/setup.cfg
--rw-r--r--   0 ben        (504) staff       (20)     2138 2022-04-26 22:20:20.000000 gilda-0.9.0/setup.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-06-30 15:08:32.821639 gilda-1.0.0/
+-rw-r--r--   0 ben        (503) staff       (20)     1346 2021-02-10 19:17:08.000000 gilda-1.0.0/LICENSE
+-rw-r--r--   0 ben        (503) staff       (20)      155 2023-06-30 15:07:59.000000 gilda-1.0.0/MANIFEST.in
+-rw-r--r--   0 ben        (503) staff       (20)     7161 2023-06-30 15:08:32.821428 gilda-1.0.0/PKG-INFO
+-rw-r--r--   0 ben        (503) staff       (20)     6428 2023-06-30 15:07:59.000000 gilda-1.0.0/README.md
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-06-30 15:08:32.816637 gilda-1.0.0/doc/
+-rw-r--r--   0 ben        (503) staff       (20)      634 2021-02-10 19:17:08.000000 gilda-1.0.0/doc/Makefile
+-rw-r--r--   0 ben        (503) staff       (20)     5514 2023-06-30 15:07:59.000000 gilda-1.0.0/doc/conf.py
+-rw-r--r--   0 ben        (503) staff       (20)      341 2022-04-26 22:20:20.000000 gilda-1.0.0/doc/index.rst
+-rw-r--r--   0 ben        (503) staff       (20)      795 2021-02-10 19:17:08.000000 gilda-1.0.0/doc/make.bat
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-06-30 15:08:32.816745 gilda-1.0.0/doc/modules/
+-rw-r--r--   0 ben        (503) staff       (20)      674 2023-06-30 15:07:59.000000 gilda-1.0.0/doc/modules/index.rst
+-rw-r--r--   0 ben        (503) staff       (20)      128 2023-06-30 15:07:59.000000 gilda-1.0.0/doc/requirements.txt
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-06-30 15:08:32.817882 gilda-1.0.0/gilda/
+-rw-r--r--   0 ben        (503) staff       (20)      738 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)     8713 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/api.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-06-30 15:08:32.818888 gilda-1.0.0/gilda/app/
+-rw-r--r--   0 ben        (503) staff       (20)      412 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/app/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)       59 2021-09-05 00:38:55.000000 gilda-1.0.0/gilda/app/__main__.py
+-rw-r--r--   0 ben        (503) staff       (20)    14523 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/app/app.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-06-30 15:08:32.819434 gilda-1.0.0/gilda/app/templates/
+-rw-r--r--   0 ben        (503) staff       (20)     6737 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/app/templates/base.html
+-rw-r--r--   0 ben        (503) staff       (20)       92 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/app/templates/home.html
+-rw-r--r--   0 ben        (503) staff       (20)     2235 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/app/templates/matches.html
+-rw-r--r--   0 ben        (503) staff       (20)       96 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/app/templates/ner_home.html
+-rw-r--r--   0 ben        (503) staff       (20)     1838 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/app/templates/ner_matches.html
+-rw-r--r--   0 ben        (503) staff       (20)    28308 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/generate_terms.py
+-rwxr-xr-x   0 ben        (503) staff       (20)     1584 2022-04-26 22:20:20.000000 gilda-1.0.0/gilda/greek_alphabet.py
+-rw-r--r--   0 ben        (503) staff       (20)    26932 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/grounder.py
+-rw-r--r--   0 ben        (503) staff       (20)     6734 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/ner.py
+-rw-r--r--   0 ben        (503) staff       (20)     2782 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/pandas_utils.py
+-rw-r--r--   0 ben        (503) staff       (20)     7755 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/process.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-06-30 15:08:32.820201 gilda-1.0.0/gilda/resources/
+-rw-r--r--   0 ben        (503) staff       (20)     2846 2022-06-21 14:02:33.000000 gilda-1.0.0/gilda/resources/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)      130 2021-09-05 00:38:55.000000 gilda-1.0.0/gilda/resources/__main__.py
+-rw-r--r--   0 ben        (503) staff       (20)    29081 2021-02-10 19:17:08.000000 gilda-1.0.0/gilda/resources/mesh_ambig_mappings.tsv
+-rw-r--r--   0 ben        (503) staff       (20)   362152 2021-02-10 19:17:08.000000 gilda-1.0.0/gilda/resources/mesh_mappings.tsv
+-rw-r--r--   0 ben        (503) staff       (20)     3331 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/resources/sqlite_adapter.py
+-rw-r--r--   0 ben        (503) staff       (20)     8205 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/scorer.py
+-rw-r--r--   0 ben        (503) staff       (20)     6495 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/term.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-06-30 15:08:32.821272 gilda-1.0.0/gilda/tests/
+-rw-r--r--   0 ben        (503) staff       (20)       47 2021-02-10 19:17:08.000000 gilda-1.0.0/gilda/tests/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)     2022 2022-04-26 22:20:20.000000 gilda-1.0.0/gilda/tests/test_api.py
+-rw-r--r--   0 ben        (503) staff       (20)     2488 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/tests/test_app.py
+-rw-r--r--   0 ben        (503) staff       (20)     5846 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/tests/test_generate_terms.py
+-rw-r--r--   0 ben        (503) staff       (20)     8004 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/tests/test_grounder.py
+-rw-r--r--   0 ben        (503) staff       (20)     2294 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/tests/test_ner.py
+-rw-r--r--   0 ben        (503) staff       (20)      543 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/tests/test_pandas_utils.py
+-rw-r--r--   0 ben        (503) staff       (20)     1644 2023-06-30 15:07:59.000000 gilda-1.0.0/gilda/tests/test_process.py
+-rw-r--r--   0 ben        (503) staff       (20)     1566 2021-02-10 19:17:08.000000 gilda-1.0.0/gilda/tests/test_scorer.py
+-rw-r--r--   0 ben        (503) staff       (20)     1238 2022-04-26 22:20:20.000000 gilda-1.0.0/gilda/tests/test_term.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-06-30 15:08:32.818569 gilda-1.0.0/gilda.egg-info/
+-rw-r--r--   0 ben        (503) staff       (20)     7161 2023-06-30 15:08:32.000000 gilda-1.0.0/gilda.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (503) staff       (20)     1150 2023-06-30 15:08:32.000000 gilda-1.0.0/gilda.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (503) staff       (20)        1 2023-06-30 15:08:32.000000 gilda-1.0.0/gilda.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (503) staff       (20)       41 2023-06-30 15:08:32.000000 gilda-1.0.0/gilda.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (503) staff       (20)      275 2023-06-30 15:08:32.000000 gilda-1.0.0/gilda.egg-info/requires.txt
+-rw-r--r--   0 ben        (503) staff       (20)        6 2023-06-30 15:08:32.000000 gilda-1.0.0/gilda.egg-info/top_level.txt
+-rw-r--r--   0 ben        (503) staff       (20)       38 2023-06-30 15:08:32.821678 gilda-1.0.0/setup.cfg
+-rw-r--r--   0 ben        (503) staff       (20)     2188 2023-06-30 15:07:59.000000 gilda-1.0.0/setup.py
```

### Comparing `gilda-0.9.0/LICENSE` & `gilda-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gilda-0.9.0/PKG-INFO` & `gilda-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,132 +1,165 @@
-Metadata-Version: 2.1
-Name: gilda
-Version: 0.9.0
-Summary: Grounding for biomedical entities with contextual disambiguation
-Home-page: https://github.com/indralab/gilda
-Author: Benjamin M. Gyori, Harvard Medical School
-Author-email: benjamin_gyori@hms.harvard.edu
-License: UNKNOWN
-Description: # Gilda: Grounding Integrating Learned Disambiguation
-        [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
-        [![Build](https://github.com/indralab/gilda/actions/workflows/tests.yml/badge.svg)](https://github.com/indralab/gilda/actions)
-        [![Documentation](https://readthedocs.org/projects/gilda/badge/?version=latest)](https://gilda.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/gilda.svg)](https://badge.fury.io/py/gilda)
-        
-        Gilda is a Python package and REST service that grounds (i.e., finds
-        appropriate identifiers in namespaces for) named entities in biomedical text.
-        
-        ## Installation
-        Gilda is deployed as a web service at http://grounding.indra.bio/ (see
-        Usage instructions below), however, it can also be used locally as a Python
-        package.
-        
-        The recommended method to install Gilda is through PyPI as
-        ```bash
-        pip install gilda
-        ```
-        Note that Gilda uses a single large resource file for grounding, which is
-        automatically downloaded into the `~/.data/gilda/<version>` folder during
-        runtime (see [pystow](https://github.com/cthoyt/pystow#%EF%B8%8F-configuration) for options to
-        configure the location of this folder).
-        
-        Given some additional dependencies, the grounding resource file can
-        also be regenerated locally by running `python -m gilda.generate_terms`.
-        
-        ## Documentation and notebooks
-        Documentation for Gilda is available [here](https://gilda.readthedocs.io).
-        We also provide several interactive Jupyter notebooks to help use and customize Gilda:
-        - [This notebook](https://github.com/indralab/gilda/blob/master/notebooks/gilda_introduction.ipynb) provides an interactive tutorial for using Gilda.
-        - [This notebook](https://github.com/indralab/gilda/blob/master/notebooks/custom_grounders.ipynb) shows several examples of how Gilda can be instantiated with custom
-        grounding resources.
-        - [This notebook](https://github.com/indralab/gilda/blob/master/models/model_training.ipynb) provides interactive sample code for training
-        new disambiguation models.
-        
-        ## Usage
-        Gilda can either be used as a REST web service or used programmatically
-        via its Python API. An introduction Jupyter notebook for using Gilda
-        is available at
-        https://github.com/indralab/gilda/blob/master/notebooks/gilda_introduction.ipynb
-        
-        ### Use as a Python package
-        For using Gilda as a Python package, the documentation at
-        http://gilda.readthedocs.org provides detailed descriptions of each module of
-        Gilda and their usage. A basic usage example is as follows
-        
-        ```python
-        import gilda
-        scored_matches = gilda.ground('ER', context='Calcium is released from the ER.')
-        ```
-        
-        ### Use as a web service
-        The REST service accepts POST requests with a JSON header on the /ground
-        endpoint. There is a public REST service running at http://grounding.indra.bio
-        but the service can also be run locally as
-        
-        ```bash
-        python -m gilda.app
-        ```
-        which, by default, launches the server at `localhost:8001` (for local usage
-        replace the URL in the examples below with this address).
-        
-        Below is an example request using `curl`:
-        
-        ```bash
-        curl -X POST -H "Content-Type: application/json" -d '{"text": "kras"}' http://grounding.indra.bio/ground
-        ```
-        
-        The same request using Python's request package would be as follows:
-        
-        ```python
-        import requests
-        requests.post('http://grounding.indra.bio/ground', json={'text': 'kras'})
-        ```
-        
-        ## Run web service with Docker
-        
-        After cloning the repository locally, you can build and run a Docker image
-        of Gilda using the following commands:
-        
-        ```shell
-        $ docker build -t gilda:latest .
-        $ docker run -d -p 8001:8001 gilda:latest
-        ```
-        
-        Alternatively, you can use `docker-compose` to do both the initial build and
-        run the container based on the `docker-compose.yml` configuration:
-        
-        ```shell
-        $ docker-compose up
-        ```
-        
-        ## Citation
-        
-        ```bibtex
-        @article{gyori2021gilda,
-          author = {Gyori, Benjamin M and Hoyt, Charles Tapley and Steppi, Albert},
-          doi = {10.1101/2021.09.10.459803},
-          journal = {bioRxiv},
-          publisher = {Cold Spring Harbor Laboratory},
-          title = {{Gilda: biomedical entity text normalization with machine-learned disambiguation as a service}},
-          url = {https://www.biorxiv.org/content/10.1101/2021.09.10.459803v1},
-          year = {2021}
-        }
-        ```
-        
-        ## Funding
-        The development of Gilda was funded under the DARPA Communicating with Computers
-        program (ARO grant W911NF-15-1-0544) and the DARPA Young Faculty Award
-        (ARO grant W911NF-20-1-0255).
-        
-Keywords: nlp,biology
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: terms
-Provides-Extra: benchmarks
-Provides-Extra: docs
+# Gilda: Grounding Integrating Learned Disambiguation
+[![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
+[![Build](https://github.com/indralab/gilda/actions/workflows/tests.yml/badge.svg)](https://github.com/indralab/gilda/actions)
+[![Documentation](https://readthedocs.org/projects/gilda/badge/?version=latest)](https://gilda.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/gilda.svg)](https://badge.fury.io/py/gilda)
+[![DOI](https://img.shields.io/badge/DOI-10.1093/bioadv/vbac034-green.svg)](https://doi.org/10.1093/bioadv/vbac034)
+
+Gilda is a Python package and REST service that grounds (i.e., finds
+appropriate identifiers in namespaces for) named entities in biomedical text.
+
+Gyori BM, Hoyt CT, Steppi A (2022). Gilda: biomedical entity text normalization with machine-learned disambiguation as a service. Bioinformatics Advances, 2022; vbac034 [https://doi.org/10.1093/bioadv/vbac034](https://doi.org/10.1093/bioadv/vbac034).
+
+## Installation
+Gilda is deployed as a web service at http://grounding.indra.bio/ (see
+Usage instructions below), however, it can also be used locally as a Python
+package.
+
+The recommended method to install Gilda is through PyPI as
+```bash
+pip install gilda
+```
+Note that Gilda uses a single large resource file for grounding, which is
+automatically downloaded into the `~/.data/gilda/<version>` folder during
+runtime (see [pystow](https://github.com/cthoyt/pystow#%EF%B8%8F%EF%B8%8F-configuration) for options to
+configure the location of this folder).
+
+Given some additional dependencies, the grounding resource file can
+also be regenerated locally by running `python -m gilda.generate_terms`.
+
+## Documentation and notebooks
+Documentation for Gilda is available [here](https://gilda.readthedocs.io).
+We also provide several interactive Jupyter notebooks to help use and customize Gilda:
+- [Gilda Introduction](https://github.com/indralab/gilda/blob/master/notebooks/gilda_introduction.ipynb) provides an interactive tutorial for using Gilda.
+- [Custom Grounders](https://github.com/indralab/gilda/blob/master/notebooks/custom_grounders.ipynb) shows several examples of how Gilda can be instantiated with custom
+grounding resources.
+- [Model Training](https://github.com/indralab/gilda/blob/master/models/model_training.ipynb) provides interactive sample code for training
+new disambiguation models.
+
+## Usage
+Gilda can either be used as a REST web service or used programmatically
+via its Python API. An introduction Jupyter notebook for using Gilda
+is available at
+https://github.com/indralab/gilda/blob/master/notebooks/gilda_introduction.ipynb
+
+### Use as a Python package
+For using Gilda as a Python package, the documentation at
+http://gilda.readthedocs.org provides detailed descriptions of each module of
+Gilda and their usage. A basic usage example for named entity normalization (NEN),
+or _grounding_ is as follows:
+
+```python
+import gilda
+scored_matches = gilda.ground('ER', context='Calcium is released from the ER.')
+```
+
+Gilda also implements a simple dictionary-based named entity recognition (NER)
+algorithm that can be used as follows:
+
+```python
+import gilda
+results = gilda.annotate('Calcium is released from the ER.')
+```
+
+### Use as a web service
+The REST service accepts POST requests with a JSON header on the /ground
+endpoint. There is a public REST service running at http://grounding.indra.bio
+but the service can also be run locally as
+
+```bash
+python -m gilda.app
+```
+which, by default, launches the server at `localhost:8001` (for local usage
+replace the URL in the examples below with this address).
+
+Below is an example request using `curl`:
+
+```bash
+curl -X POST -H "Content-Type: application/json" -d '{"text": "kras"}' http://grounding.indra.bio/ground
+```
+
+The same request using Python's request package would be as follows:
+
+```python
+import requests
+requests.post('http://grounding.indra.bio/ground', json={'text': 'kras'})
+```
+
+The web service also supports multiple inputs in a single request on the
+`ground_multi` endpoint, for instance
+
+```python
+import requests
+requests.post('http://grounding.indra.bio/ground_multi',
+              json=[
+                  {'text': 'braf'},
+                  {'text': 'ER', 'context': 'endoplasmic reticulum (ER) is a cellular component'}
+              ]
+          )
+```
+
+## Resource usage
+Gilda loads grounding terms into memory when first used. If memory usage
+is an issue, the following options are recommended.
+
+1. Run a single instance of Gilda as a local web service that one or more
+other processes send requests to.
+
+2. Create a custom Grounder instance that only loads a subset of terms
+approrpiate for a narrow use case.
+
+3. Gilda also offers an optional sqlite back-end which significantly decreases
+memory usage and results in minor drop in the number of strings grounder per
+unit time. The sqlite back-end database can be built as follows with an
+optional `[db_path]` argument, which if used, should use the .db extension. If
+not specified, the .db file is generated in Gilda's default resource folder.
+
+```bash
+python -m gilda.resources.sqlite_adapter [db_path]
+```
+
+A Grounder instance can then be instantiated as follows:
+
+```python
+from gilda.grounder import Grounder
+gr = Grounder(db_path)
+matches = gr.ground('kras')
+```
+
+## Run web service with Docker
+
+After cloning the repository locally, you can build and run a Docker image
+of Gilda using the following commands:
+
+```shell
+$ docker build -t gilda:latest .
+$ docker run -d -p 8001:8001 gilda:latest
+```
+
+Alternatively, you can use `docker-compose` to do both the initial build and
+run the container based on the `docker-compose.yml` configuration:
+
+```shell
+$ docker-compose up
+```
+
+## Citation
+
+```bibtex
+@article{gyori2022gilda,
+    author = {Gyori, Benjamin M and Hoyt, Charles Tapley and Steppi, Albert},
+    title = "{{Gilda: biomedical entity text normalization with machine-learned disambiguation as a service}}",
+    journal = {Bioinformatics Advances},
+    year = {2022},
+    month = {05},
+    issn = {2635-0041},
+    doi = {10.1093/bioadv/vbac034},
+    url = {https://doi.org/10.1093/bioadv/vbac034},
+    note = {vbac034}
+}
+```
+
+## Funding
+The development of Gilda was funded under the DARPA Communicating with Computers
+program (ARO grant W911NF-15-1-0544) and the DARPA Young Faculty Award
+(ARO grant W911NF-20-1-0255).
```

### Comparing `gilda-0.9.0/doc/Makefile` & `gilda-1.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gilda-0.9.0/doc/conf.py` & `gilda-1.0.0/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -167,10 +167,10 @@
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'https://docs.python.org/': None,
+    'python': ('https://docs.python.org/', None),
     'pyobo': ('https://pyobo.readthedocs.io/en/latest/', None),
 }
```

### Comparing `gilda-0.9.0/doc/make.bat` & `gilda-1.0.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gilda-0.9.0/gilda/__init__.py` & `gilda-1.0.0/gilda/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-__version__ = '0.9.0'
+__version__ = '1.0.0'
 
 import logging
 
-from .api import get_grounder, get_models, get_names, ground, make_grounder
+from .api import get_grounder, get_models, get_names, ground, make_grounder, annotate
+from .grounder import Grounder, ScoredMatch
+from .pandas_utils import ground_df, ground_df_map
 from .term import Term
 
 __all__ = [
     'ground',
+    'annotate',
     'get_models',
     'get_names',
     'get_grounder',
     'make_grounder',
     # Classes
     'Term',
+    'Grounder',
+    'ScoredMatch',
     # Meta
     '__version__',
+    # Pandas utilities
+    'ground_df',
+    'ground_df_map',
 ]
 
 logging.basicConfig(format=('%(levelname)s: [%(asctime)s] %(name)s'
                             ' - %(message)s'),
                     level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
 
 logger = logging.getLogger('gilda')
```

### Comparing `gilda-0.9.0/gilda/api.py` & `gilda-1.0.0/gilda/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-__all__ = ['ground', 'get_models', 'get_names', 'get_grounder', 'make_grounder']
+__all__ = [
+    'ground',
+    'get_models',
+    'get_names',
+    'get_grounder',
+    'make_grounder',
+    'annotate',
+]
 
 from typing import List, Mapping, Union, Optional
 
 from gilda.grounder import Grounder
 from gilda.term import Term
 
 
@@ -25,14 +32,18 @@
         return self.get_grounder().get_models()
 
     def get_names(self, db, id, status=None, source=None):
         return self.get_grounder().get_names(db, id,
                                              status=status,
                                              source=source)
 
+    @property
+    def prefix_index(self):
+        return self.get_grounder().prefix_index
+
 
 grounder = GrounderInstance()
 
 
 def ground(text, context=None, organisms=None, namespaces=None):
     """Return a list of scored matches for a text to ground.
 
@@ -92,14 +103,56 @@
     Only return results from a certain namespace, such as when a family and gene have the same name
 
     >>> scored_matches = gilda.ground('ESR', namespaces=["hgnc"])
     """
     return grounder.ground(text=text, context=context, organisms=organisms, namespaces=namespaces)
 
 
+def annotate(
+    text: str,
+    sent_split_fun=None,
+    organisms=None,
+    namespaces=None,
+):
+    """Annotate a given text with Gilda (i.e., do named entity recognition).
+
+    Parameters
+    ----------
+    text : str
+        The text to be annotated.
+    sent_split_fun : Callable, optional
+        A function that splits the text into sentences. The default is
+        :func:`nltk.tokenize.sent_tokenize`. The function should take a string
+        as input and return an iterable of strings corresponding to the sentences
+        in the input text.
+    organisms : list[str], optional
+        A list of organism names to pass to the grounder. If not provided,
+        human is used.
+    namespaces : list[str], optional
+        A list of namespaces to pass to the grounder to restrict the matches
+        to. By default, no restriction is applied.
+
+    Returns
+    -------
+    list[tuple[str, ScoredMatch, int, int]]
+        A list of tuples of start and end character offsets of the text
+        corresponding to the entity, the entity text, and the ScoredMatch
+        object corresponding to the entity.
+    """
+    from .ner import annotate as _annotate
+
+    return _annotate(
+        text,
+        grounder=grounder,
+        sent_split_fun=sent_split_fun,
+        organisms=organisms,
+        namespaces=namespaces
+    )
+
+
 def get_models():
     """Return a list of entity texts for which disambiguation models exist.
 
     Returns
     -------
     list[str]
         The list of entity texts for which a disambiguation model is
```

### Comparing `gilda-0.9.0/gilda/app/app.py` & `gilda-1.0.0/gilda/app/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 from textwrap import dedent
+from typing import Optional
 
-from flask import Flask, Response, abort, jsonify, render_template, request
+from flask import Blueprint, Flask, abort, jsonify, \
+    render_template, request, current_app
 from flask_bootstrap import Bootstrap
 from flask_restx import Api, Resource, fields
 from flask_wtf import FlaskForm
+from werkzeug.local import LocalProxy
 from wtforms import StringField, SubmitField, TextAreaField, \
     SelectMultipleField
 from wtforms.validators import DataRequired
 
-from gilda.api import *
 from gilda import __version__ as version
 from gilda.resources import popular_organisms, organism_labels
+from gilda.grounder import GrounderInput, Grounder
 
-app = Flask(__name__)
-app.config['RESTX_MASK_SWAGGER'] = False
-app.config['WTF_CSRF_ENABLED'] = False
-app.config['SWAGGER_UI_DOC_EXPANSION'] = 'list'
-Bootstrap(app)
+ui_blueprint = Blueprint("ui", __name__, url_prefix="/")
 
+# The way that local proxies work is that when the app gets
+# instantiated, you can stick objects into the `app.config`
+# dictionary, then the local proxy lets you access them through
+# a fake "current_app" object.
+grounder = LocalProxy(lambda: current_app.config["grounder"])
+
+ORGANISMS_FIELD = SelectMultipleField(
+    'Species priority (optional)',
+    choices=[(org, organism_labels[org]) for org in popular_organisms],
+    id='organism-select',
+    description=dedent("""\
+        Optionally select one or more taxonomy
+        species IDs to define a species priority list.  Click
+        <a type="button" href="#" data-toggle="modal" data-target="#species-modal">
+        here <i class="far fa-question-circle">
+        </i></a> for more details.
+    """),
+)
 
 class GroundForm(FlaskForm):
     text = StringField(
         'Text',
         validators=[DataRequired()],
         description=dedent("""\
             Input the entity text (e.g., <code>k-ras</code>) to ground."""
@@ -35,56 +52,85 @@
         description=dedent("""\
             Optionally provide additional text context to help disambiguation. Click
             <a type="button" href="#" data-toggle="modal" data-target="#context-modal">
             here <i class="far fa-question-circle">
             </i></a> for more details.
         """)
     )
-    organisms = SelectMultipleField(
-        'Species priority (optional)',
-        choices=[(org, organism_labels[org]) for org in popular_organisms],
-        id='organism-select',
+    organisms = ORGANISMS_FIELD
+    submit = SubmitField('Submit')
+
+    def get_matches(self):
+        return grounder.ground(self.text.data, context=self.context.data,
+                               organisms=self.organisms.data)
+
+
+class NERForm(FlaskForm):
+    text = TextAreaField(
+        'Text',
+        validators=[DataRequired()],
         description=dedent("""\
-            Optionally select one or more taxonomy
-            species IDs to define a species priority list.  Click
-            <a type="button" href="#" data-toggle="modal" data-target="#species-modal">
-            here <i class="far fa-question-circle">
-            </i></a> for more details.
-        """),
+            Text from which to identify and ground named entities.
+        """)
     )
+    organisms = ORGANISMS_FIELD
     submit = SubmitField('Submit')
 
-    def get_matches(self):
-        return ground(self.text.data, context=self.context.data,
-                      organisms=self.organisms.data)
+    def get_annotations(self):
+        from gilda.ner import annotate
+
+        return annotate(self.text.data, grounder=grounder,
+                        organisms=self.organisms.data)
 
 
-@app.route('/', methods=['GET', 'POST'])
+@ui_blueprint.route('/', methods=['GET', 'POST'])
 def home():
     text = request.args.get('text')
     if text is not None:
         context = request.args.get('context')
         organisms = request.args.getlist('organisms')
-        matches = ground(text, context=context, organisms=organisms)
+        matches = grounder.ground(text, context=context, organisms=organisms)
         return render_template('matches.html', matches=matches, version=version,
                                text=text, context=context)
 
     form = GroundForm()
     if form.validate_on_submit():
         matches = form.get_matches()
-        return render_template('matches.html', matches=matches, version=version,
-                               text=form.text.data, context=form.context.data)
+        return render_template(
+            'matches.html',
+            matches=matches,
+            version=version,
+            text=form.text.data,
+            context=form.context.data,
+            # Add a new form that doesn't auto-populate
+            form=GroundForm(formdata=None),
+        )
     return render_template('home.html', form=form, version=version)
 
 
+@ui_blueprint.route('/ner', methods=['GET', 'POST'])
+def view_ner():
+    form = NERForm()
+    if form.validate_on_submit():
+        annotations = form.get_annotations()
+        return render_template(
+            'ner_matches.html',
+            annotations=annotations,
+            version=version,
+            text=form.text.data,
+            # Add a new form that doesn't auto-populate
+            form=NERForm(formdata=None),
+        )
+    return render_template('ner_home.html', form=form, version=version)
+
+
 # NOTE: the Flask REST-X API has to be declared here, below the home endpoint
 # otherwise it reserves the / base path.
 
-api = Api(app,
-          title="Gilda",
+api = Api(title="Gilda",
           description="A service for grounding entity strings",
           version=version,
           license="Code available under the BSD 2-Clause License",
           contact="INDRA labs",
           contact_email="indra.sysbio@gmail.com",
           contact_url="https://indralab.github.io",
           doc='/apidocs',
@@ -224,69 +270,107 @@
 models_model = fields.List(
     fields.String,
     example=['A4', 'ABC1', 'p180'])
 
 
 @base_ns.route('/ground', methods=['POST'])
 class Ground(Resource):
-    # NOTE: formally this response should be a list
     @base_ns.response(200, "Grounding results", [scored_match_model])
     @base_ns.expect(grounding_input_model)
     def post(self):
         """Return a list of scored grounding matches for a given entity text.
 
         The returned value is a list with each entry being a scored match.
         Each scored match contains a term which was matched, and each term
         contains a db and id constituting a grounding. An empty list
         return value means that no grounding matches were found for the input.
         """
         if request.json is None:
-            abort(Response('Missing application/json header.', 415))
+            abort(415, 'Missing application/json header.')
         # Get input parameters
         text = request.json.get('text')
         context = request.json.get('context')
         organisms = request.json.get('organisms')
-        scored_matches = ground(text, context=context, organisms=organisms)
+        scored_matches = grounder.ground(text, context=context, organisms=organisms)
         res = [sm.to_json() for sm in scored_matches]
         return jsonify(res)
 
 
+@base_ns.route('/ground_multi', methods=['POST'])
+class GroundMulti(Resource):
+    @base_ns.response(200, "Grounding results", [[scored_match_model]])
+    @base_ns.expect([grounding_input_model])
+    def post(self):
+        """Return a list of grounding matches for a list of inputs.
+
+        This endpoint is useful for batch processing of inputs. The input
+        is a list with each entry containing a text key as well as optional
+        context and organism keys. The returned value is a list corresponding
+        to each input in order, each entry of the returned list being a list
+        of scored matches.
+        """
+        if request.json is None:
+            abort(415, 'Missing application/json header.')
+        # Get input parameters
+        all_matches = []
+        for input in request.json:
+            text = input.get('text')
+            context = input.get('context')
+            organisms = input.get('organisms')
+            scored_matches = grounder.ground(text, context=context, organisms=organisms)
+            all_matches.append([sm.to_json() for sm in scored_matches])
+        return jsonify(all_matches)
+
+
 @base_ns.route('/names', methods=['POST'])
 @base_ns.route('/get_names', methods=['POST'])
 class GetNames(Resource):
     @base_ns.response(200, "Get names result", names_model)
     @base_ns.expect(get_names_input_model)
     def post(self):
         """Return all known entity texts for a grounding.
 
         This endpoint can be used as a reverse lookup to find out what entity
         texts (names, synonyms, etc.) are known for a given grounded entity.
         """
         if request.json is None:
-            abort(Response('Missing application/json header.', 415))
+            abort(415, 'Missing application/json header.')
         # Get input parameters
         kwargs = {key: request.json.get(key) for key in {'db', 'id', 'status',
                                                          'source'}}
-        names = get_names(**kwargs)
+        names = grounder.get_names(**kwargs)
         return jsonify(names)
 
 
 @base_ns.route('/models', methods=['GET', 'POST'])
 class GetModels(Resource):
     @base_ns.response(200, "Get models result", models_model)
-    def post(selt):
+    def post(self):
         """Return a list of texts with Gilda disambiguation models.
 
         Gilda makes available more than one thousand disambiguation models
         between synonyms shared by multiple genes. This endpoint returns
         the list of entity texts for which such a model is available.
         """
-        return jsonify(get_models())
+        return jsonify(grounder.get_models())
 
     def get(self):
         """Return a list of texts with Gilda disambiguation models.
 
         Gilda makes available more than one thousand disambiguation models
         between synonyms shared by multiple genes. This endpoint returns
         the list of entity texts for which such a model is available.
         """
-        return jsonify(get_models())
+        return jsonify(grounder.get_models())
+
+
+def get_app(terms: Optional[GrounderInput] = None) -> Flask:
+    app = Flask(__name__)
+    app.config['RESTX_MASK_SWAGGER'] = False
+    app.config['WTF_CSRF_ENABLED'] = False
+    app.config['SWAGGER_UI_DOC_EXPANSION'] = 'list'
+    app.config["grounder"] = Grounder(terms=terms)
+    Bootstrap(app)
+    app.register_blueprint(ui_blueprint, url_prefix="/")
+    # has to be put after defining the UI blueprint otherwise it reserves "/"
+    api.init_app(app)
+    return app
```

### Comparing `gilda-0.9.0/gilda/generate_terms.py` & `gilda-1.0.0/gilda/generate_terms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """This is a script that can be run to generate a new grounding_terms.tsv file.
 It uses several resource files and database clients from INDRA and requires it
 to be available locally."""
 
 import re
 import os
 import csv
-import gzip
 import json
 import logging
 import requests
-import itertools
 import indra
 from indra.databases import hgnc_client, uniprot_client, chebi_client, \
     go_client, mesh_client, doid_client
 from indra.statements.resources import amino_acids
-from .term import Term
+from .term import Term, dump_terms, filter_out_duplicates
 from .process import normalize
 from .resources import resource_dir, popular_organisms
 
 
 indra_module_path = indra.__path__[0]
 indra_resources = os.path.join(indra_module_path, 'resources')
 
@@ -335,15 +333,15 @@
 
 def generate_uniprot_terms(download=False, organisms=None):
     if not organisms:
         organisms = popular_organisms
     path = os.path.join(resource_dir, 'up_synonyms.tsv')
     org_filter_str = ' OR '.join(organisms)
     if not os.path.exists(path) or download:
-        url = (f'https://www.uniprot.org/uniprot/?format=tab&columns=id,'
+        url = (f'https://legacy.uniprot.org/uniprot/?format=tab&columns=id,'
                f'genes(PREFERRED),genes(ALTERNATIVE),protein%20names,organism-id&sort=score&'
                f'query=reviewed:yes&fil=organism:{org_filter_str}')
         logger.info('Downloading UniProt resource file')
         res = requests.get(url)
         with open(path, 'w') as fh:
             fh.write(res.text)
     terms = []
@@ -502,20 +500,30 @@
 
 
 def generate_adeft_terms():
     from adeft import available_shortforms
     from adeft.disambiguate import load_disambiguator
     from indra.ontology.standardize import get_standard_name
     all_term_args = set()
+    add_prefix = ['BTO', 'HP', 'DOID']
+    remove_prefix = ['EFO', 'NCIT', 'OMIT']
     for shortform in available_shortforms:
         da = load_disambiguator(shortform)
         for grounding, name in da.names.items():
             if grounding == 'ungrounded' or ':' not in grounding:
                 continue
             db_ns, db_id = grounding.split(':', maxsplit=1)
+            if db_ns in remove_prefix:
+                if db_id.startswith(db_ns + ':'):
+                    db_id = db_id[len(db_ns) + 1:]
+            if db_ns in add_prefix:
+                if not db_id.startswith(db_ns + ':'):
+                    db_id = db_ns + ':' + db_id
+            if db_id == 'PF00112)':
+                db_id = 'PF00112'
             # Here we do a name standardization via INDRA just in case
             # there is a discrepancy
             indra_standard_name = get_standard_name({db_ns: db_id})
             if indra_standard_name:
                 name = indra_standard_name
             term_args = (normalize(shortform), shortform, db_ns, db_id,
                          name, 'synonym', 'adeft')
@@ -655,29 +663,14 @@
         mesh_mappings_reverse[(row[3], row[4])] = [row[1], row[2]]
     return mesh_mappings, mesh_mappings_reverse
 
 
 mesh_mappings, mesh_mappings_reverse = _make_mesh_mappings()
 
 
-def filter_out_duplicates(terms):
-    logger.info('Filtering %d terms for uniqueness...' % len(terms))
-    term_key = lambda term: (term.db, term.id, term.text)
-    statuses = {'curated': 1, 'name': 2, 'synonym': 3, 'former_name': 4}
-    new_terms = []
-    for _, terms in itertools.groupby(sorted(terms, key=lambda x: term_key(x)),
-                                      key=lambda x: term_key(x)):
-        terms = sorted(terms, key=lambda x: statuses[x.status])
-        new_terms.append(terms[0])
-    # Re-sort the terms
-    new_terms = sorted(new_terms, key=lambda x: (x.text, x.db, x.id))
-    logger.info('Got %d unique terms...' % len(new_terms))
-    return new_terms
-
-
 def terms_from_obo_url(url, prefix, ignore_mappings=False, map_to_ns=None):
     """Return terms extracted directly from an OBO given as a URL."""
     import obonet
     from indra.databases.obo_client import OboClient
     g = obonet.read_obo(url)
     entries = OboClient.entries_from_graph(g, prefix=prefix)
     terms = []
@@ -707,20 +700,14 @@
         terms += generated_terms
 
     terms = filter_out_duplicates(terms)
     return terms
 
 
 def main():
-    terms = get_all_terms()
     from .resources import GROUNDING_TERMS_PATH as fname
-    logger.info('Dumping into %s' % fname)
-    header = ['norm_text', 'text', 'db', 'id', 'entry_name', 'status',
-              'source', 'organism', 'source_db', 'source_id']
-    with gzip.open(fname, 'wt', encoding='utf-8') as fh:
-        writer = csv.writer(fh, delimiter='\t')
-        writer.writerow(header)
-        writer.writerows(t.to_list() for t in terms)
+    terms = get_all_terms()
+    dump_terms(terms, fname)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `gilda-0.9.0/gilda/greek_alphabet.py` & `gilda-1.0.0/gilda/greek_alphabet.py`

 * *Files identical despite different names*

### Comparing `gilda-0.9.0/gilda/grounder.py` & `gilda-1.0.0/gilda/grounder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,48 @@
+import os
 import csv
 import json
 import gzip
-import pickle
 import logging
 import itertools
 from pathlib import Path
 from collections import defaultdict, Counter
 from textwrap import dedent
-from typing import List, Mapping, Optional, Set, Tuple, Union
+from typing import Iterator, List, Mapping, Optional, Set, Tuple, Union
 from adeft.disambiguate import load_disambiguator
 from adeft.modeling.classify import load_model_info
 from adeft import available_shortforms as available_adeft_models
 from .term import Term, get_identifiers_curie, get_identifiers_url
 from .process import normalize, replace_dashes, replace_greek_uni, \
     replace_greek_latin, replace_greek_spelled_out, depluralize, \
     replace_roman_arabic
-from .scorer import Match, generate_match, score, score_namespace
+from .scorer import Match, generate_match, score
 from .resources import get_gilda_models, get_grounding_terms
 
 __all__ = [
     "Grounder",
     "GrounderInput",
     "ScoredMatch",
     "load_terms_file",
+    "load_entries_from_terms_file",
     "filter_for_organism",
     "load_adeft_models",
     "load_gilda_models",
 ]
 
 logger = logging.getLogger(__name__)
 
 
 GrounderInput = Union[str, Path, List[Term], Mapping[str, List[Term]]]
 
+#: The default namespace priority order
+DEFAULT_NAMESPACE_PRIORITY = [
+    'FPLX', 'HGNC', 'UP', 'CHEBI', 'GO', 'MESH', 'DOID', 'HP', 'EFO'
+]
+
 
 class Grounder(object):
     """Class to look up and ground query texts in a terms file.
 
     Parameters
     ----------
     terms :
@@ -48,37 +54,70 @@
           as a path to a grounding terms gzipped TSV file which is then
           loaded.
         - If :class:`list`, it is assumed to be a flat list of
           :class:`gilda.term.Term` instances.
         - If :class:`dict`, it is assumed to be a grounding terms dict with
           normalized entity strings as keys and :class:`gilda.term.Term`
           instances as values.
+    namespace_priority :
+        Specifies a term namespace priority order. For example, if multiple
+        terms are matched with the same score, will use this list to decide
+        which are given by which namespace appears further towards the front
+        of the list. By default, :data:`DEFAULT_NAMESPACE_PRIORITY` is used,
+        which, for example, prioritizes famplex entities over HGNC ones.
     """
 
     entries: Mapping[str, List[Term]]
+    namespace_priority: List[str]
 
-    def __init__(self, terms: Optional[GrounderInput] = None):
+    def __init__(
+        self,
+        terms: Optional[GrounderInput] = None,
+        *,
+        namespace_priority: Optional[List[str]] = None,
+    ):
         if terms is None:
             terms = get_grounding_terms()
 
         if isinstance(terms, (str, Path)):
-            self.entries = load_terms_file(terms)
+            extension = os.path.splitext(terms)[1]
+            if extension == '.db':
+                from .resources.sqlite_adapter import SqliteEntries
+                self.entries = SqliteEntries(terms)
+            else:
+                self.entries = load_terms_file(terms)
         elif isinstance(terms, list):
             self.entries = defaultdict(list)
             for term in terms:
                 self.entries[term.norm_text].append(term)
             self.entries = dict(self.entries)
         elif isinstance(terms, dict):
             self.entries = terms
         else:
             raise TypeError('terms is neither a path nor a list of terms,'
                             'nor a normalized entry name to term dictionary')
 
-        self.adeft_disambiguators = load_adeft_models()
-        self.gilda_disambiguators = load_gilda_models()
+        self.prefix_index = {}
+        self._build_prefix_index()
+
+        self.adeft_disambiguators = find_adeft_models()
+        self.gilda_disambiguators = None
+
+        self.namespace_priority = (
+            DEFAULT_NAMESPACE_PRIORITY
+            if namespace_priority is None else
+            namespace_priority
+        )
+
+    def _build_prefix_index(self):
+        prefix_index = defaultdict(set)
+        for norm_term in self.entries:
+            parts = norm_term.split()
+            prefix_index[parts[0]].add(len(parts))
+        self.prefix_index = dict(prefix_index)
 
     def lookup(self, raw_str: str) -> List[Term]:
         """Return matching Terms for a given raw string.
 
         Parameters
         ----------
         raw_str :
@@ -114,21 +153,34 @@
         lookups.add(greek_replaced)
         greek_replaced = normalize(replace_greek_spelled_out(raw_str))
         lookups.add(greek_replaced)
         # We try exchanging roman and arabic numerals
         roman_arabic = normalize(replace_roman_arabic(raw_str))
         lookups.add(roman_arabic)
         # Finally, we attempt to depluralize the word
-        depluralized = normalize(depluralize(raw_str)[0])
-        lookups.add(depluralized)
+        for singular, rule in depluralize(raw_str):
+            lookups.add(normalize(singular))
 
         logger.debug('Looking up the following strings: %s' %
                      ', '.join(lookups))
         return lookups
 
+    def _score_namespace(self, term) -> int:
+        """Apply a priority to the term based on its namespace.
+
+        .. note::
+
+            This is currently not included as an explicit score term.
+            It is just used to rank identically scored entries.
+        """
+        try:
+            return len(self.namespace_priority) - self.namespace_priority.index(term.db)
+        except ValueError:
+            return 0
+
     def ground(self, raw_str, context=None, organisms=None,
                namespaces=None):
         """Return scored groundings for a given raw string.
 
         Parameters
         ----------
         raw_str : str
@@ -154,14 +206,19 @@
         -------
         list[gilda.grounder.ScoredMatch]
             A list of ScoredMatch objects representing the groundings sorted
             by decreasing score.
         """
         if not organisms:
             organisms = ['9606']
+        # Stripping whitespaces is done up front directly on the raw string
+        # so that all lookups and comparisons are done with respect to the
+        # stripped string
+        raw_str = raw_str.strip()
+        # Initial lookup of all possible matches
         entries = self.lookup(raw_str)
         logger.debug('Filtering %d entries by organism' % len(entries))
         entries = filter_for_organism(entries, organisms)
         logger.debug('Comparing %s with %d entries' %
                      (raw_str, len(entries)))
         # For each entry to compare to, we generate a match data structure
         # describing the comparison of the raw (unnormalized) input string
@@ -184,28 +241,32 @@
         unique_scores = self._merge_equivalent_matches(scored_matches)
 
         # If there's context available, disambiguate based on that
         if context:
             unique_scores = self.disambiguate(raw_str, unique_scores, context)
 
         # Then sort by decreasing score
-        rank_fun = lambda x: (x.score, score_namespace(x.term))
+        rank_fun = lambda x: (x.score, self._score_namespace(x.term))
         unique_scores = sorted(unique_scores, key=rank_fun, reverse=True)
 
         # If we have a namespace constraint, we filter to the given
         # namespaces.
         if namespaces:
             unique_scores = [
                 scored_match for scored_match in unique_scores
                 if scored_match.get_namespaces() & set(namespaces)
             ]
 
         return unique_scores
 
     def disambiguate(self, raw_str, scored_matches, context):
+        # This is only called if context was passed in so we do lazy
+        # loading here
+        if self.gilda_disambiguators is None:
+            self.gilda_disambiguators = load_gilda_models()
         # If we don't have a disambiguator for this string, we return with
         # the original scores intact. Otherwise, we attempt to disambiguate.
         if raw_str in self.adeft_disambiguators:
             logger.info('Running Adeft disambiguation for %s' % raw_str)
             try:
                 scored_matches = \
                     self.disambiguate_adeft(raw_str, scored_matches, context)
@@ -220,14 +281,16 @@
                 logger.exception(e)
 
         return scored_matches
 
     def disambiguate_adeft(self, raw_str, scored_matches, context):
         # We find the disambiguator for the given string and pass in
         # context
+        if self.adeft_disambiguators[raw_str] is None:
+            self.adeft_disambiguators[raw_str] = load_disambiguator(raw_str)
         res = self.adeft_disambiguators[raw_str].disambiguate([context])
         # The actual grounding dict is at this index in the result
         grounding_dict = res[0][2]
         logger.debug('Result from Adeft: %s' % str(grounding_dict))
         # We attempt to get the score for the 'ungrounded' entry
         ungrounded_score = grounding_dict.get('ungrounded', 1.0)
         # Now we check if each scored match has a corresponding Adeft
@@ -296,14 +359,16 @@
 
         Returns
         -------
         list[str]
             The list of entity texts for which a disambiguation model is
             available.
         """
+        if self.gilda_disambiguators is None:
+            self.gilda_disambiguators = load_gilda_models()
         return sorted(list(self.gilda_disambiguators.keys()))
 
     def get_names(self, db, id, status=None, source=None):
         """Return a list of entity texts corresponding to a given database ID.
 
         Parameters
         ----------
@@ -520,42 +585,60 @@
         """Get the groundings as CURIEs and URLs."""
         return {
             get_identifiers_curie(db, db_id): get_identifiers_url(db, db_id)
             for db, db_id in self.get_groundings()
         }
 
 
-def load_terms_file(terms_file: Union[str, Path]) -> Mapping[str, List[Term]]:
-    """Load a TSV file containing terms into a lookup dictionary.
+def load_entries_from_terms_file(terms_file: Union[str, Path]) -> Iterator[Term]:
+    """Yield Terms from a compressed terms TSV file path.
 
     Parameters
     ----------
     terms_file :
-        Path to a TSV terms file with columns corresponding to the serialized
-        elements of a Term.
+        Path to a compressed TSV terms file with columns corresponding to the
+        serialized elements of a Term.
 
     Returns
     -------
     :
-        A lookup dictionary whose keys are normalized entity texts, and values
-        are lists of Terms with that normalized entity text.
+        Terms loaded from the file yielded by a generator.
     """
     with gzip.open(terms_file, 'rt', encoding='utf-8') as fh:
         entries = {}
         reader = csv.reader(fh, delimiter='\t')
         # Skip header
         next(reader)
         for row in reader:
             row_nones = [r if r else None for r in row]
-            entry = Term(*row_nones)
-            if row[0] in entries:
-                entries[row[0]].append(entry)
-            else:
-                entries[row[0]] = [entry]
-        return entries
+            yield Term(*row_nones)
+
+
+def load_terms_file(terms_file: Union[str, Path]) -> Mapping[str, List[Term]]:
+    """Load a TSV file containing terms into a lookup dictionary.
+
+    Parameters
+    ----------
+    terms_file :
+        Path to a compressed TSV terms file with columns corresponding to the
+        serialized elements of a Term.
+
+    Returns
+    -------
+    :
+        A lookup dictionary whose keys are normalized entity texts, and values
+        are lists of Terms with that normalized entity text.
+    """
+    entries = {}
+    for term in load_entries_from_terms_file(terms_file):
+        if term.norm_text in entries:
+            entries[term.norm_text].append(term)
+        else:
+            entries[term.norm_text] = [term]
+    return entries
 
 
 def filter_for_organism(terms, organisms):
     # First we organize terms by organism, including None
     terms_by_organism = defaultdict(list)
     for term in terms:
         # We filter out any organisms that aren't in the list provided
@@ -570,20 +653,25 @@
     if set(terms_by_organism) != {None}:
         top_organism = min(set(terms_by_organism) - {None},
                            key=lambda x: organisms.index(x))
         all_terms += terms_by_organism[top_organism]
     return all_terms
 
 
-def load_adeft_models():
+def find_adeft_models():
     adeft_disambiguators = {}
     for shortform in available_adeft_models:
-        adeft_disambiguators[shortform] = load_disambiguator(shortform)
+        adeft_disambiguators[shortform] = None
     return adeft_disambiguators
 
 
+def load_adeft_models():
+    return {shortform: load_disambiguator(shortform)
+            for shortform in find_adeft_models()}
+
+
 def load_gilda_models(cutoff=0.7):
-    with gzip.open(get_gilda_models(), 'rb') as fh:
-        models_raw = pickle.load(fh)
-    models = {k: load_model_info(v['cl']) for k, v in models_raw.items()}
-    models = {k: v for k, v in models.items() if v.stats['f1']['mean'] > cutoff}
+    with gzip.open(get_gilda_models(), 'rt') as fh:
+        models = {k: load_model_info(v)
+                  for k, v in json.loads(fh.read()).items()
+                  if v['stats']['f1']['mean'] > cutoff}
     return models
```

### Comparing `gilda-0.9.0/gilda/process.py` & `gilda-1.0.0/gilda/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Module containing various string processing functions used for grounding."""
+from typing import List, Tuple
+
 import regex as re
 import unidecode
 
 from .greek_alphabet import greek_alphabet, greek_to_latin
 
 
 #: A list of all kinds of dashes
@@ -164,61 +166,64 @@
         return 'all_lower'
     elif re.match(r'^\p{Lu}\p{Ll}+$', word):
         return 'initial_cap'
     else:
         return 'mixed'
 
 
-def depluralize(word):
-    """Return the depluralized version of the word, along with a status  flag.
+def depluralize(word: str) -> List[Tuple[str, str]]:
+    """Return the depluralized version of the word, along with a status flag.
 
     Parameters
     ----------
     word : str
         The word which is to be depluralized.
 
     Returns
     -------
-    str
+    list of str pairs:
         The original word, if it is detected to be non-plural, or the
-        depluralized version of the word.
-    str
-        A status flag represeting the detected pluralization status of the
+        depluralized version of the word, and a status flag representing the
+        detected pluralization status of the
         word, with non_plural (e.g., BRAF), plural_oes (e.g., mosquitoes),
         plural_ies (e.g., antibodies), plural_es (e.g., switches),
         plural_cap_s (e.g., MAPKs), and plural_s (e.g., receptors).
     """
     # If the word doesn't end in s, we assume it's not plural
     if not word.endswith('s'):
-        return word, 'non_plural'
+        return [(word, 'non_plural')]
     # Another case is words ending in -sis (e.g., apoptosis), these are almost
     # exclusively non plural so we return here too
     elif word.endswith('sis'):
-        return word, 'non_plural'
+        return [(word, 'non_plural')]
     # This is the case when the word ends with an o which is pluralized as oes
     # e.g., mosquitoes
     elif word.endswith('oes'):
-        return word[:-2], 'plural_oes'
+        return [(word[:-2], 'plural_oes'),
+                (word[:-1], 'plural_s')]
     # This is the case when the word ends with a y which is pluralized as ies,
     # e.g., antibodies
     elif word.endswith('ies'):
-        return word[:-3] + 'y', 'plural_ies'
+        return [(word[:-3] + 'y', 'plural_ies'),
+                (word[:-1], 'plural_s')]
     # These are the cases where words form plurals by adding -es so we
-    # return by stripping it off
+    # return by stripping it off. However, it's not possible to determine
+    # if the word doesn't end in e.g., -xe or -se in a singluar form, and
+    # so we also return a variant to account for this.
     elif word.endswith(('xes', 'ses', 'ches', 'shes')):
-        return word[:-2], 'plural_es'
+        return [(word[:-2], 'plural_es'), (word[:-1], 'plural_s')]
     # If the word is all caps and the last letter is an s, then it's a very
     # strong signal that it is pluralized so we have a custom return value
     # for that
     elif re.match(r'^\p{Lu}+$', word[:-1]):
-        return word[:-1], 'plural_caps_s'
+        return [(word[:-1], 'plural_caps_s')]
     # Otherwise, we just go with the assumption that the last s is the
     # plural marker
     else:
-        return word[:-1], 'plural_s'
+        return [(word[:-1], 'plural_s')]
     # Note: there don't seem to be any compelling examples of -f or -fe -> ves
     # so it is not implemented
 
 
 def replace_roman_arabic(s):
     match = roman_arabic_prefilter.match(s)
     if not match:
```

### Comparing `gilda-0.9.0/gilda/resources/__init__.py` & `gilda-1.0.0/gilda/resources/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,14 @@
         logger.info('Downloading grounding terms from S3.')
         out_file = _download_from_s3(resource_dir, base_name)
         logger.info('Saved grounding terms into: %s' % out_file)
     return full_path
 
 
 def get_gilda_models():
-    base_name = 'gilda_models.pkl.gz'
+    base_name = 'gilda_models.json.gz'
     full_path = os.path.join(resource_dir, base_name)
     if not os.path.exists(full_path):
         logger.info('Downloading disambiguation models from S3.')
         out_file = _download_from_s3(resource_dir, base_name)
         logger.info('Saved disambiguation models into: %s' % out_file)
     return full_path
```

### Comparing `gilda-0.9.0/gilda/resources/mesh_ambig_mappings.tsv` & `gilda-1.0.0/gilda/resources/mesh_ambig_mappings.tsv`

 * *Files identical despite different names*

### Comparing `gilda-0.9.0/gilda/resources/mesh_mappings.tsv` & `gilda-1.0.0/gilda/resources/mesh_mappings.tsv`

 * *Files identical despite different names*

### Comparing `gilda-0.9.0/gilda/scorer.py` & `gilda-1.0.0/gilda/scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
     get_capitalization_pattern
 
 __all__ = [
     "Match",
     "generate_match",
     "score_string_match",
     "score_status",
-    "score_namespace",
     "score",
 ]
 
 
 class Match(object):
     """Class representing a match between a query and a reference string"""
     def __init__(self, query, ref, exact=None, space_mismatch=None,
@@ -243,22 +242,12 @@
         'name': 3,
         'synonym': 2,
         'former_name': 1,
     }
     return scores[term.status]
 
 
-def score_namespace(term):
-    """Note: this is currently not included as an explicit score term.
-    It is just used to rank identically scored entries."""
-    order = ['FPLX', 'HGNC', 'UP', 'CHEBI', 'GO', 'MESH', 'DOID', 'HP', 'EFO']
-    try:
-        return len(order) - order.index(term.db)
-    except ValueError:
-        return 0
-
-
 def score(match, term):
     string_match_score = score_string_match(match)
     status_score = score_status(term)
     score = ((0 * 5 + status_score) * 2 + string_match_score) / 9
     return score
```

### Comparing `gilda-0.9.0/gilda/term.py` & `gilda-1.0.0/gilda/term.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-from typing import Optional, Set, Tuple
+import csv
+import gzip
+import itertools
+import logging
+from typing import Iterable, Optional, Set, Tuple
 
 __all__ = [
     "Term",
     "get_identifiers_curie",
     "get_identifiers_url",
+    "filter_out_duplicates",
+    "dump_terms",
 ]
 
+logger = logging.getLogger(__name__)
+
 
 class Term(object):
     """Represents a text entry corresponding to a grounded term.
 
     Attributes
     ----------
     norm_text : str
@@ -35,14 +43,15 @@
         from a given source, this attribute provides the original db value
         before mapping.
     source_id : Optional[str]
         If the term's db/id was mapped from a different, original db/id
         from a given source, this attribute provides the original ID value
         before mapping.
     """
+
     def __init__(self, norm_text, text, db, id, entry_name, status, source,
                  organism=None, source_db=None, source_id=None):
         if not text:
             raise ValueError('Text for Term cannot be empty')
         self.norm_text = norm_text
         self.text = text
         self.db = db
@@ -137,7 +146,52 @@
         return curie_pattern.format(db=id_parts[0].upper(), id=id_parts[-1])
 
 
 def get_identifiers_url(db, id):
     curie = get_identifiers_curie(db, id)
     if curie is not None:
         return f'https://identifiers.org/{curie}'
+
+
+def _term_key(term: Term) -> Tuple[str, str, str]:
+    return term.db, term.id, term.text
+
+
+statuses = {'curated': 1, 'name': 2, 'synonym': 3, 'former_name': 4}
+
+
+def _priority_key(term: Term) -> Tuple[int, int]:
+    """
+    Prioritize terms (that are pre-grouped by db/id/text) first
+    based on status, and if the status is the same, give priority
+    to the ones that are from primary resources
+    """
+    return (
+        statuses[term.status],
+        0 if term.db.casefold() == term.source.casefold() else 1
+    )
+
+
+def filter_out_duplicates(terms):
+    logger.info('Filtering %d terms for uniqueness...' % len(terms))
+    new_terms = []
+    for _, terms in itertools.groupby(sorted(terms, key=_term_key),
+                                      key=_term_key):
+        terms = sorted(terms, key=_priority_key)
+        new_terms.append(terms[0])
+    # Re-sort the terms
+    new_terms = sorted(new_terms, key=lambda x: (x.text, x.db, x.id))
+    logger.info('Got %d unique terms...' % len(new_terms))
+    return new_terms
+
+
+TERMS_HEADER = ['norm_text', 'text', 'db', 'id', 'entry_name', 'status',
+                'source', 'organism', 'source_db', 'source_id']
+
+
+def dump_terms(terms: Iterable[Term], fname) -> None:
+    """Dump a list of terms to a tsv.gz file."""
+    logger.info('Dumping into %s', fname)
+    with gzip.open(fname, 'wt', encoding='utf-8') as fh:
+        writer = csv.writer(fh, delimiter='\t')
+        writer.writerow(TERMS_HEADER)
+        writer.writerows(t.to_list() for t in terms)
```

### Comparing `gilda-0.9.0/gilda/tests/test_api.py` & `gilda-1.0.0/gilda/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gilda-0.9.0/gilda/tests/test_app.py` & `gilda-1.0.0/gilda/tests/test_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """Test the API in the Gilda app."""
 
 import unittest
 
-from gilda.app.app import app
+from gilda.app.app import get_app
 
 
 class TestApp(unittest.TestCase):
     """A test case for the Gilda Flask application."""
 
+    @classmethod
+    def setUpClass(cls) -> None:
+        cls.app = get_app()
+
     def test_get_home(self):
         """Test the GET response on the home page."""
-        with app.test_client() as client:
+        with self.app.test_client() as client:
             res = client.get("/?text=Raf1")
             self.assert_raf1_ui(res)
 
     def test_post_home(self):
         """Test the POST response on the home page."""
-        with app.test_client() as client:
+        with self.app.test_client() as client:
             res = client.post("/", json={"text": "Raf1"})
             self.assert_raf1_ui(res)
 
     def assert_raf1_ui(self, res) -> None:
         text = res.data.decode()
         self.assertEqual(200, res.status_code)
         self.assertIn('RAF1', text)
         self.assertIn('0.9998', text)
         self.assertIn('RNASE3', text)
         self.assertIn('0.5024', text)
 
     def test_post_grounding(self):
         """Test the POST response with text."""
-        with app.test_client() as client:
+        with self.app.test_client() as client:
             res = client.post("/ground")
             self.assertIn("message", res.json)
 
             res = client.post("/ground", json={"text": "Raf1"})
             self.assertIsInstance(res.json, list)
             self.assert_found(res.json, "HGNC", "9829")
 
@@ -43,21 +47,21 @@
             self.assert_found(res.json, "HGNC", "9829")
 
             res = client.post("/ground", json={"text": "Raf1", "organisms": ["10090", "9606"]})
             self.assertIsInstance(res.json, list)
             self.assert_found(res.json, "UP", "Q99N57")
 
     def test_get_names(self):
-        with app.test_client() as client:
+        with self.app.test_client() as client:
             res = client.post('/names', json={"db": "FPLX", "id": "ERK"})
             self.assertIsInstance(res.json, list)
             self.assertIn('ERK 1/2', res.json)
 
     def test_get_models(self):
-        with app.test_client() as client:
+        with self.app.test_client() as client:
             res = client.get('/models')
             self.assertIsInstance(res.json, list)
             self.assertIn('ABC1', res.json)
 
     def assert_found(self, matches, prefix: str, identifier: str) -> None:
         match_curies = {
             (match['term']['db'], match['term']['id'])
```

### Comparing `gilda-0.9.0/gilda/tests/test_generate_terms.py` & `gilda-1.0.0/gilda/tests/test_generate_terms.py`

 * *Files 11% similar despite different names*

```diff
@@ -71,14 +71,29 @@
                  'synonym', 'up', '9606')
     terms = filter_out_duplicates([term1, term2])
     assert len(terms) == 1
     term = terms[0]
     assert term.status == 'synonym'
 
 
+def test_filter_priority_by_source():
+    term1 = Term('mekk2', 'MEKK2', 'HGNC', '6854', 'MAP3K2',
+                 'synonym', 'hgnc', '9606')
+    term2 = Term('mekk2', 'MEKK2', 'HGNC', '6854', 'MAP3K2',
+                 'synonym', 'up', '9606')
+    terms = filter_out_duplicates([term1, term2])
+    assert len(terms) == 1
+    assert terms[0] == term1
+
+    # now test the other way, to make sure order doesn't matter
+    terms = filter_out_duplicates([term2, term1])
+    assert len(terms) == 1
+    assert terms[0] == term1
+
+
 def test_get_terms_simple():
     row = {'Entry': 'P15056',
            'Gene names  (primary )': 'BRAF',
            'Gene names  (synonym )': 'BRAF1 RAFB1',
            'Protein names':
                ('Serine/threonine-protein kinase B-raf '
                 '(EC 2.7.11.1) (Proto-oncogene B-Raf) (p94) '
```

### Comparing `gilda-0.9.0/gilda/tests/test_grounder.py` & `gilda-1.0.0/gilda/tests/test_grounder.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,14 +75,24 @@
         if match.term.db == 'HGNC' and match.term.id == '7679':
             assert match.disambiguation['score'] < 0.01
 
 
 def test_rank_namespace():
     matches = gr.ground('interferon-gamma')
     assert matches[0].term.db == 'HGNC'
+    assert matches[1].term.db == 'EFO'
+
+
+def test_rank_namespace_custom_order():
+    """Test when applying a custom order.
+    See also the above test ``test_rank_namespace``."""
+    custom_grounder = Grounder(namespace_priority=["EFO", "HGNC"])
+    matches = custom_grounder.ground('interferon-gamma')
+    assert matches[0].term.db == 'EFO'
+    assert matches[1].term.db == 'HGNC'
 
 
 def test_aa_synonym():
     matches = gr.ground('WN')
     assert '141447' not in {m.term.id for m in matches}
 
     matches = gr.ground('W-N')
@@ -204,8 +214,26 @@
     assert ('HGNC', '9600') in {(m.term.db, m.term.id) for m in matches}
 
 
 def test_namespaces():
     matches = gr.ground('KRAS', namespaces=['CHEBI'])
     assert not matches
     matches = gr.ground('KRAS', namespaces=['HGNC'])
-    assert matches
+    assert matches
+
+
+def test_sqlite():
+    from gilda.resources.sqlite_adapter import build
+    matches = gr.ground('braf')
+    entries = {'braf': gr.entries['braf']}
+    build(entries, 'test.db')
+
+    grsql = Grounder('test.db')
+    matchessql = grsql.ground('braf')
+    assert len(matches) == len(matchessql)
+
+    assert grsql.ground('kras') == []
+
+
+def test_strip_whitespace():
+    matches = gr.ground(' inflammatory response ')
+    assert matches
```

### Comparing `gilda-0.9.0/gilda/tests/test_scorer.py` & `gilda-1.0.0/gilda/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `gilda-0.9.0/gilda/tests/test_term.py` & `gilda-1.0.0/gilda/tests/test_term.py`

 * *Files identical despite different names*

### Comparing `gilda-0.9.0/gilda.egg-info/PKG-INFO` & `gilda-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,186 @@
 Metadata-Version: 2.1
 Name: gilda
-Version: 0.9.0
+Version: 1.0.0
 Summary: Grounding for biomedical entities with contextual disambiguation
 Home-page: https://github.com/indralab/gilda
 Author: Benjamin M. Gyori, Harvard Medical School
 Author-email: benjamin_gyori@hms.harvard.edu
-License: UNKNOWN
-Description: # Gilda: Grounding Integrating Learned Disambiguation
-        [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
-        [![Build](https://github.com/indralab/gilda/actions/workflows/tests.yml/badge.svg)](https://github.com/indralab/gilda/actions)
-        [![Documentation](https://readthedocs.org/projects/gilda/badge/?version=latest)](https://gilda.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/gilda.svg)](https://badge.fury.io/py/gilda)
-        
-        Gilda is a Python package and REST service that grounds (i.e., finds
-        appropriate identifiers in namespaces for) named entities in biomedical text.
-        
-        ## Installation
-        Gilda is deployed as a web service at http://grounding.indra.bio/ (see
-        Usage instructions below), however, it can also be used locally as a Python
-        package.
-        
-        The recommended method to install Gilda is through PyPI as
-        ```bash
-        pip install gilda
-        ```
-        Note that Gilda uses a single large resource file for grounding, which is
-        automatically downloaded into the `~/.data/gilda/<version>` folder during
-        runtime (see [pystow](https://github.com/cthoyt/pystow#%EF%B8%8F-configuration) for options to
-        configure the location of this folder).
-        
-        Given some additional dependencies, the grounding resource file can
-        also be regenerated locally by running `python -m gilda.generate_terms`.
-        
-        ## Documentation and notebooks
-        Documentation for Gilda is available [here](https://gilda.readthedocs.io).
-        We also provide several interactive Jupyter notebooks to help use and customize Gilda:
-        - [This notebook](https://github.com/indralab/gilda/blob/master/notebooks/gilda_introduction.ipynb) provides an interactive tutorial for using Gilda.
-        - [This notebook](https://github.com/indralab/gilda/blob/master/notebooks/custom_grounders.ipynb) shows several examples of how Gilda can be instantiated with custom
-        grounding resources.
-        - [This notebook](https://github.com/indralab/gilda/blob/master/models/model_training.ipynb) provides interactive sample code for training
-        new disambiguation models.
-        
-        ## Usage
-        Gilda can either be used as a REST web service or used programmatically
-        via its Python API. An introduction Jupyter notebook for using Gilda
-        is available at
-        https://github.com/indralab/gilda/blob/master/notebooks/gilda_introduction.ipynb
-        
-        ### Use as a Python package
-        For using Gilda as a Python package, the documentation at
-        http://gilda.readthedocs.org provides detailed descriptions of each module of
-        Gilda and their usage. A basic usage example is as follows
-        
-        ```python
-        import gilda
-        scored_matches = gilda.ground('ER', context='Calcium is released from the ER.')
-        ```
-        
-        ### Use as a web service
-        The REST service accepts POST requests with a JSON header on the /ground
-        endpoint. There is a public REST service running at http://grounding.indra.bio
-        but the service can also be run locally as
-        
-        ```bash
-        python -m gilda.app
-        ```
-        which, by default, launches the server at `localhost:8001` (for local usage
-        replace the URL in the examples below with this address).
-        
-        Below is an example request using `curl`:
-        
-        ```bash
-        curl -X POST -H "Content-Type: application/json" -d '{"text": "kras"}' http://grounding.indra.bio/ground
-        ```
-        
-        The same request using Python's request package would be as follows:
-        
-        ```python
-        import requests
-        requests.post('http://grounding.indra.bio/ground', json={'text': 'kras'})
-        ```
-        
-        ## Run web service with Docker
-        
-        After cloning the repository locally, you can build and run a Docker image
-        of Gilda using the following commands:
-        
-        ```shell
-        $ docker build -t gilda:latest .
-        $ docker run -d -p 8001:8001 gilda:latest
-        ```
-        
-        Alternatively, you can use `docker-compose` to do both the initial build and
-        run the container based on the `docker-compose.yml` configuration:
-        
-        ```shell
-        $ docker-compose up
-        ```
-        
-        ## Citation
-        
-        ```bibtex
-        @article{gyori2021gilda,
-          author = {Gyori, Benjamin M and Hoyt, Charles Tapley and Steppi, Albert},
-          doi = {10.1101/2021.09.10.459803},
-          journal = {bioRxiv},
-          publisher = {Cold Spring Harbor Laboratory},
-          title = {{Gilda: biomedical entity text normalization with machine-learned disambiguation as a service}},
-          url = {https://www.biorxiv.org/content/10.1101/2021.09.10.459803v1},
-          year = {2021}
-        }
-        ```
-        
-        ## Funding
-        The development of Gilda was funded under the DARPA Communicating with Computers
-        program (ARO grant W911NF-15-1-0544) and the DARPA Young Faculty Award
-        (ARO grant W911NF-20-1-0255).
-        
 Keywords: nlp,biology
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: terms
 Provides-Extra: benchmarks
 Provides-Extra: docs
+License-File: LICENSE
+
+# Gilda: Grounding Integrating Learned Disambiguation
+[![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
+[![Build](https://github.com/indralab/gilda/actions/workflows/tests.yml/badge.svg)](https://github.com/indralab/gilda/actions)
+[![Documentation](https://readthedocs.org/projects/gilda/badge/?version=latest)](https://gilda.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/gilda.svg)](https://badge.fury.io/py/gilda)
+[![DOI](https://img.shields.io/badge/DOI-10.1093/bioadv/vbac034-green.svg)](https://doi.org/10.1093/bioadv/vbac034)
+
+Gilda is a Python package and REST service that grounds (i.e., finds
+appropriate identifiers in namespaces for) named entities in biomedical text.
+
+Gyori BM, Hoyt CT, Steppi A (2022). Gilda: biomedical entity text normalization with machine-learned disambiguation as a service. Bioinformatics Advances, 2022; vbac034 [https://doi.org/10.1093/bioadv/vbac034](https://doi.org/10.1093/bioadv/vbac034).
+
+## Installation
+Gilda is deployed as a web service at http://grounding.indra.bio/ (see
+Usage instructions below), however, it can also be used locally as a Python
+package.
+
+The recommended method to install Gilda is through PyPI as
+```bash
+pip install gilda
+```
+Note that Gilda uses a single large resource file for grounding, which is
+automatically downloaded into the `~/.data/gilda/<version>` folder during
+runtime (see [pystow](https://github.com/cthoyt/pystow#%EF%B8%8F%EF%B8%8F-configuration) for options to
+configure the location of this folder).
+
+Given some additional dependencies, the grounding resource file can
+also be regenerated locally by running `python -m gilda.generate_terms`.
+
+## Documentation and notebooks
+Documentation for Gilda is available [here](https://gilda.readthedocs.io).
+We also provide several interactive Jupyter notebooks to help use and customize Gilda:
+- [Gilda Introduction](https://github.com/indralab/gilda/blob/master/notebooks/gilda_introduction.ipynb) provides an interactive tutorial for using Gilda.
+- [Custom Grounders](https://github.com/indralab/gilda/blob/master/notebooks/custom_grounders.ipynb) shows several examples of how Gilda can be instantiated with custom
+grounding resources.
+- [Model Training](https://github.com/indralab/gilda/blob/master/models/model_training.ipynb) provides interactive sample code for training
+new disambiguation models.
+
+## Usage
+Gilda can either be used as a REST web service or used programmatically
+via its Python API. An introduction Jupyter notebook for using Gilda
+is available at
+https://github.com/indralab/gilda/blob/master/notebooks/gilda_introduction.ipynb
+
+### Use as a Python package
+For using Gilda as a Python package, the documentation at
+http://gilda.readthedocs.org provides detailed descriptions of each module of
+Gilda and their usage. A basic usage example for named entity normalization (NEN),
+or _grounding_ is as follows:
+
+```python
+import gilda
+scored_matches = gilda.ground('ER', context='Calcium is released from the ER.')
+```
+
+Gilda also implements a simple dictionary-based named entity recognition (NER)
+algorithm that can be used as follows:
+
+```python
+import gilda
+results = gilda.annotate('Calcium is released from the ER.')
+```
+
+### Use as a web service
+The REST service accepts POST requests with a JSON header on the /ground
+endpoint. There is a public REST service running at http://grounding.indra.bio
+but the service can also be run locally as
+
+```bash
+python -m gilda.app
+```
+which, by default, launches the server at `localhost:8001` (for local usage
+replace the URL in the examples below with this address).
+
+Below is an example request using `curl`:
+
+```bash
+curl -X POST -H "Content-Type: application/json" -d '{"text": "kras"}' http://grounding.indra.bio/ground
+```
+
+The same request using Python's request package would be as follows:
+
+```python
+import requests
+requests.post('http://grounding.indra.bio/ground', json={'text': 'kras'})
+```
+
+The web service also supports multiple inputs in a single request on the
+`ground_multi` endpoint, for instance
+
+```python
+import requests
+requests.post('http://grounding.indra.bio/ground_multi',
+              json=[
+                  {'text': 'braf'},
+                  {'text': 'ER', 'context': 'endoplasmic reticulum (ER) is a cellular component'}
+              ]
+          )
+```
+
+## Resource usage
+Gilda loads grounding terms into memory when first used. If memory usage
+is an issue, the following options are recommended.
+
+1. Run a single instance of Gilda as a local web service that one or more
+other processes send requests to.
+
+2. Create a custom Grounder instance that only loads a subset of terms
+approrpiate for a narrow use case.
+
+3. Gilda also offers an optional sqlite back-end which significantly decreases
+memory usage and results in minor drop in the number of strings grounder per
+unit time. The sqlite back-end database can be built as follows with an
+optional `[db_path]` argument, which if used, should use the .db extension. If
+not specified, the .db file is generated in Gilda's default resource folder.
+
+```bash
+python -m gilda.resources.sqlite_adapter [db_path]
+```
+
+A Grounder instance can then be instantiated as follows:
+
+```python
+from gilda.grounder import Grounder
+gr = Grounder(db_path)
+matches = gr.ground('kras')
+```
+
+## Run web service with Docker
+
+After cloning the repository locally, you can build and run a Docker image
+of Gilda using the following commands:
+
+```shell
+$ docker build -t gilda:latest .
+$ docker run -d -p 8001:8001 gilda:latest
+```
+
+Alternatively, you can use `docker-compose` to do both the initial build and
+run the container based on the `docker-compose.yml` configuration:
+
+```shell
+$ docker-compose up
+```
+
+## Citation
+
+```bibtex
+@article{gyori2022gilda,
+    author = {Gyori, Benjamin M and Hoyt, Charles Tapley and Steppi, Albert},
+    title = "{{Gilda: biomedical entity text normalization with machine-learned disambiguation as a service}}",
+    journal = {Bioinformatics Advances},
+    year = {2022},
+    month = {05},
+    issn = {2635-0041},
+    doi = {10.1093/bioadv/vbac034},
+    url = {https://doi.org/10.1093/bioadv/vbac034},
+    note = {vbac034}
+}
+```
+
+## Funding
+The development of Gilda was funded under the DARPA Communicating with Computers
+program (ARO grant W911NF-15-1-0544) and the DARPA Young Faculty Award
+(ARO grant W911NF-20-1-0255).
```

### Comparing `gilda-0.9.0/gilda.egg-info/SOURCES.txt` & `gilda-1.0.0/gilda.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,31 +9,41 @@
 doc/requirements.txt
 doc/modules/index.rst
 gilda/__init__.py
 gilda/api.py
 gilda/generate_terms.py
 gilda/greek_alphabet.py
 gilda/grounder.py
+gilda/ner.py
+gilda/pandas_utils.py
 gilda/process.py
 gilda/scorer.py
 gilda/term.py
 gilda.egg-info/PKG-INFO
 gilda.egg-info/SOURCES.txt
 gilda.egg-info/dependency_links.txt
 gilda.egg-info/entry_points.txt
 gilda.egg-info/requires.txt
 gilda.egg-info/top_level.txt
 gilda/app/__init__.py
 gilda/app/__main__.py
 gilda/app/app.py
+gilda/app/templates/base.html
+gilda/app/templates/home.html
+gilda/app/templates/matches.html
+gilda/app/templates/ner_home.html
+gilda/app/templates/ner_matches.html
 gilda/resources/__init__.py
 gilda/resources/__main__.py
 gilda/resources/mesh_ambig_mappings.tsv
 gilda/resources/mesh_mappings.tsv
+gilda/resources/sqlite_adapter.py
 gilda/tests/__init__.py
 gilda/tests/test_api.py
 gilda/tests/test_app.py
 gilda/tests/test_generate_terms.py
 gilda/tests/test_grounder.py
+gilda/tests/test_ner.py
+gilda/tests/test_pandas_utils.py
 gilda/tests/test_process.py
 gilda/tests/test_scorer.py
 gilda/tests/test_term.py
```

### Comparing `gilda-0.9.0/setup.py` & `gilda-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,18 @@
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
       ],
       packages=find_packages(),
       install_requires=['regex', 'adeft>=0.11.0', 'boto3', 'flask',
                         'flask-wtf', 'flask-bootstrap', 'flask-restx',
-                        'obonet', 'pystow>=0.1.10', 'unidecode'],
-      extras_require={'test': ['pytest', 'pytest-cov'],
-                      'terms': ['indra'],
+                        'pystow>=0.1.10', 'unidecode',
+                        'werkzeug<2.2'],
+      extras_require={'test': ['pytest', 'pytest-cov', 'pandas'],
+                      'terms': ['indra', 'obonet'],
                       'benchmarks': ['pandas>=1.0', 'requests',
                                      'tabulate', 'tqdm', 'click'],
                       'docs': [
                           "sphinx",
                           "sphinx_autodoc_typehints",
                           "sphinx_rtd_theme",
                       ],
```

