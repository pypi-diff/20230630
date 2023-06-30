# Comparing `tmp/pyrdfsubset-0.1.0.tar.gz` & `tmp/pyrdfsubset-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrdfsubset-0.1.0.tar", last modified: Fri Jun 30 05:20:24 2023, max compression
+gzip compressed data, was "pyrdfsubset-0.1.2.tar", last modified: Fri Jun 30 08:18:29 2023, max compression
```

## Comparing `pyrdfsubset-0.1.0.tar` & `pyrdfsubset-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:20:24.578833 pyrdfsubset-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-30 05:20:14.000000 pyrdfsubset-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-30 05:20:24.578833 pyrdfsubset-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 05:20:14.000000 pyrdfsubset-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-30 05:20:14.000000 pyrdfsubset-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 05:20:24.578833 pyrdfsubset-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:20:24.578833 pyrdfsubset-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:20:24.578833 pyrdfsubset-0.1.0/src/pyrdfsubset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 05:20:14.000000 pyrdfsubset-0.1.0/src/pyrdfsubset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-30 05:20:14.000000 pyrdfsubset-0.1.0/src/pyrdfsubset/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-30 05:20:14.000000 pyrdfsubset-0.1.0/src/pyrdfsubset/rdfsubset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-30 05:20:14.000000 pyrdfsubset-0.1.0/src/pyrdfsubset/sparqlsubset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:20:24.578833 pyrdfsubset-0.1.0/src/pyrdfsubset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-30 05:20:24.000000 pyrdfsubset-0.1.0/src/pyrdfsubset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 05:20:24.000000 pyrdfsubset-0.1.0/src/pyrdfsubset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 05:20:24.000000 pyrdfsubset-0.1.0/src/pyrdfsubset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 05:20:24.000000 pyrdfsubset-0.1.0/src/pyrdfsubset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 05:20:24.000000 pyrdfsubset-0.1.0/src/pyrdfsubset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 05:20:24.000000 pyrdfsubset-0.1.0/src/pyrdfsubset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:18:29.941557 pyrdfsubset-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-30 08:18:18.000000 pyrdfsubset-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-30 08:18:29.941557 pyrdfsubset-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 08:18:18.000000 pyrdfsubset-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-30 08:18:18.000000 pyrdfsubset-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 08:18:29.941557 pyrdfsubset-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:18:29.937557 pyrdfsubset-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:18:29.941557 pyrdfsubset-0.1.2/src/pyrdfsubset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:18:18.000000 pyrdfsubset-0.1.2/src/pyrdfsubset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-30 08:18:18.000000 pyrdfsubset-0.1.2/src/pyrdfsubset/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-30 08:18:18.000000 pyrdfsubset-0.1.2/src/pyrdfsubset/rdfsubset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-30 08:18:18.000000 pyrdfsubset-0.1.2/src/pyrdfsubset/sparqlsubset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:18:29.941557 pyrdfsubset-0.1.2/src/pyrdfsubset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-30 08:18:29.000000 pyrdfsubset-0.1.2/src/pyrdfsubset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 08:18:29.000000 pyrdfsubset-0.1.2/src/pyrdfsubset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:18:29.000000 pyrdfsubset-0.1.2/src/pyrdfsubset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 08:18:29.000000 pyrdfsubset-0.1.2/src/pyrdfsubset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 08:18:29.000000 pyrdfsubset-0.1.2/src/pyrdfsubset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 08:18:29.000000 pyrdfsubset-0.1.2/src/pyrdfsubset.egg-info/top_level.txt
```

### Comparing `pyrdfsubset-0.1.0/LICENSE` & `pyrdfsubset-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrdfsubset-0.1.0/PKG-INFO` & `pyrdfsubset-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyrdfsubset
-Version: 0.1.0
-Summary: Create RDF subsets based on ShEx constraints and optionally SPARQL query results
+Version: 0.1.2
+Summary: Create RDF subsets based on ShEx constraints and optionally SPARQL query results. The development of this library started at the Biohackathon Japan in 2023 in Shodoshima
 Author-email: Andra Waagmeester <andra@micelio.be>
 License: MIT License
         
         Copyright (c) 2023 Micelio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pyrdfsubset-0.1.0/pyproject.toml` & `pyrdfsubset-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrdfsubset"
-version = "0.1.0"
-description = "Create RDF subsets based on ShEx constraints and optionally SPARQL query results"
+version = "0.1.2"
+description = "Create RDF subsets based on ShEx constraints and optionally SPARQL query results. The development of this library started at the Biohackathon Japan in 2023 in Shodoshima"
 readme = "README.md"
 authors = [{ name = "Andra Waagmeester", email = "andra@micelio.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `pyrdfsubset-0.1.0/src/pyrdfsubset/rdfsubset.py` & `pyrdfsubset-0.1.2/src/pyrdfsubset/rdfsubset.py`

 * *Files identical despite different names*

### Comparing `pyrdfsubset-0.1.0/src/pyrdfsubset/sparqlsubset.py` & `pyrdfsubset-0.1.2/src/pyrdfsubset/sparqlsubset.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 
 SELECT * WHERE {
    ?item wdt:P699 ?doid .
 }
 """
 shex = "https://raw.githubusercontent.com/kg-subsetting/biohackathon2020/main/use_cases/genewiki/genewiki.shex"
 get_sparql_subset(shex, sparql_query, "https://query.wikidata.org/sparql", "http://www.wikidata.org/entity/Q12136", subsettype="open")
-# shexeval(['-h'])
+
```

### Comparing `pyrdfsubset-0.1.0/src/pyrdfsubset.egg-info/PKG-INFO` & `pyrdfsubset-0.1.2/src/pyrdfsubset.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyrdfsubset
-Version: 0.1.0
-Summary: Create RDF subsets based on ShEx constraints and optionally SPARQL query results
+Version: 0.1.2
+Summary: Create RDF subsets based on ShEx constraints and optionally SPARQL query results. The development of this library started at the Biohackathon Japan in 2023 in Shodoshima
 Author-email: Andra Waagmeester <andra@micelio.be>
 License: MIT License
         
         Copyright (c) 2023 Micelio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

