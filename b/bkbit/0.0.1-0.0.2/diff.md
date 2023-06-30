# Comparing `tmp/bkbit-0.0.1.tar.gz` & `tmp/bkbit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkbit-0.0.1.tar", last modified: Fri Jun 23 21:46:44 2023, max compression
+gzip compressed data, was "bkbit-0.0.2.tar", last modified: Fri Jun 30 01:25:45 2023, max compression
```

## Comparing `bkbit-0.0.1.tar` & `bkbit-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxr-xr-x   0 dorota     (501) staff       (20)        0 2023-06-23 21:46:44.078962 bkbit-0.0.1/
--rw-r--r--   0 dorota     (501) staff       (20)    11357 2023-06-22 21:15:26.000000 bkbit-0.0.1/LICENSE
--rw-r--r--   0 dorota     (501) staff       (20)      466 2023-06-23 21:46:44.078778 bkbit-0.0.1/PKG-INFO
--rw-r--r--   0 dorota     (501) staff       (20)       48 2023-06-22 19:30:00.000000 bkbit-0.0.1/README.md
-drwxr-xr-x   0 dorota     (501) staff       (20)        0 2023-06-23 21:46:44.075423 bkbit-0.0.1/bkbit/
--rw-r--r--   0 dorota     (501) staff       (20)        0 2023-06-22 21:23:54.000000 bkbit-0.0.1/bkbit/__init__.py
-drwxr-xr-x   0 dorota     (501) staff       (20)        0 2023-06-23 21:46:44.076201 bkbit-0.0.1/bkbit/models/
--rw-r--r--   0 dorota     (501) staff       (20)        0 2023-06-22 19:32:03.000000 bkbit-0.0.1/bkbit/models/__init__.py
--rw-r--r--   0 dorota     (501) staff       (20)  1263600 2023-06-22 19:32:56.000000 bkbit-0.0.1/bkbit/models/kbmodel.py
-drwxr-xr-x   0 dorota     (501) staff       (20)        0 2023-06-23 21:46:44.078580 bkbit-0.0.1/bkbit/utils/
--rw-r--r--   0 dorota     (501) staff       (20)        0 2023-06-23 20:53:50.000000 bkbit-0.0.1/bkbit/utils/__init__.py
-drwxr-xr-x   0 dorota     (501) staff       (20)        0 2023-06-23 21:46:44.075989 bkbit-0.0.1/bkbit.egg-info/
--rw-r--r--   0 dorota     (501) staff       (20)      466 2023-06-23 21:46:44.000000 bkbit-0.0.1/bkbit.egg-info/PKG-INFO
--rw-r--r--   0 dorota     (501) staff       (20)      267 2023-06-23 21:46:44.000000 bkbit-0.0.1/bkbit.egg-info/SOURCES.txt
--rw-r--r--   0 dorota     (501) staff       (20)        1 2023-06-23 21:46:44.000000 bkbit-0.0.1/bkbit.egg-info/dependency_links.txt
--rw-r--r--   0 dorota     (501) staff       (20)       51 2023-06-23 21:46:44.000000 bkbit-0.0.1/bkbit.egg-info/requires.txt
--rw-r--r--   0 dorota     (501) staff       (20)        6 2023-06-23 21:46:44.000000 bkbit-0.0.1/bkbit.egg-info/top_level.txt
--rw-r--r--   0 dorota     (501) staff       (20)      707 2023-06-23 21:45:00.000000 bkbit-0.0.1/pyproject.toml
--rw-r--r--   0 dorota     (501) staff       (20)       38 2023-06-23 21:46:44.079010 bkbit-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:45.691128 bkbit-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 01:25:30.000000 bkbit-0.0.2/.autorc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:45.687128 bkbit-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:45.691128 bkbit-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-30 01:25:30.000000 bkbit-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-30 01:25:30.000000 bkbit-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 01:25:30.000000 bkbit-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-30 01:25:45.691128 bkbit-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 01:25:30.000000 bkbit-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:45.691128 bkbit-0.0.2/bkbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:30.000000 bkbit-0.0.2/bkbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 01:25:45.000000 bkbit-0.0.2/bkbit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:45.691128 bkbit-0.0.2/bkbit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:30.000000 bkbit-0.0.2/bkbit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1263623 2023-06-30 01:25:30.000000 bkbit-0.0.2/bkbit/models/kbmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:45.691128 bkbit-0.0.2/bkbit/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 01:25:30.000000 bkbit-0.0.2/bkbit/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 01:25:30.000000 bkbit-0.0.2/bkbit/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-30 01:25:30.000000 bkbit-0.0.2/bkbit/scripts/generateGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-30 01:25:30.000000 bkbit-0.0.2/bkbit/scripts/generateSmallGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-30 01:25:30.000000 bkbit-0.0.2/bkbit/scripts/gfftranslator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:45.691128 bkbit-0.0.2/bkbit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:30.000000 bkbit-0.0.2/bkbit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:25:45.691128 bkbit-0.0.2/bkbit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-30 01:25:45.000000 bkbit-0.0.2/bkbit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 01:25:45.000000 bkbit-0.0.2/bkbit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:25:45.000000 bkbit-0.0.2/bkbit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 01:25:45.000000 bkbit-0.0.2/bkbit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 01:25:45.000000 bkbit-0.0.2/bkbit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-30 01:25:30.000000 bkbit-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 01:25:45.691128 bkbit-0.0.2/setup.cfg
```

### Comparing `bkbit-0.0.1/LICENSE` & `bkbit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bkbit-0.0.1/bkbit/models/kbmodel.py` & `bkbit-0.0.2/bkbit/models/kbmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -3182,23 +3182,23 @@
     
 
 
 class GeneAnnotation(Gene):
     """
     An annotation describing the location, boundaries, and functions of  individual genes within a genome annotation.
     """
-    referenced_in: Optional[str] = Field(None)
+    referenced_in: Optional[GenomeAnnotation] = Field(None)
     molecular_type: Optional[BioType] = Field(None)
     source_id: Optional[str] = Field(None, description="""The authority specific identifier.""")
     symbol: Optional[str] = Field(None, description="""Symbol for a particular thing""")
     synonym: Optional[List[str]] = Field(default_factory=list, description="""Alternate human-readable names for a thing""")
     xref: Optional[List[str]] = Field(default_factory=list, description="""A database cross reference or alternative identifier for a NamedThing or edge between two  NamedThings.  This property should point to a database record or webpage that supports the existence of the edge, or  gives more detail about the edge. This property can be used on a node or edge to provide multiple URIs or CURIE cross references.""")
     has_biological_sequence: Optional[str] = Field(None, description="""connects a genomic feature to its sequence""")
     id: str = Field(..., description="""A unique identifier for an entity. Must be either a CURIE shorthand for a URI or a complete URI""")
-    in_taxon: Optional[List[str]] = Field(None, description="""connects an entity to its taxonomic classification. Only certain kinds of entities can be taxonomically classified; see 'thing with taxon'""")
+    in_taxon: Optional[List[OrganismTaxon]] = Field(None, description="""connects an entity to its taxonomic classification. Only certain kinds of entities can be taxonomically classified; see 'thing with taxon'""")
     in_taxon_label: Optional[str] = Field(None, description="""The human readable scientific name for the taxon of the entity.""")
     provided_by: Optional[List[str]] = Field(None, description="""The value in this node property represents the knowledge provider that created or assembled the node and all of its attributes.  Used internally to represent how a particular node made its way into a knowledge provider or graph.""")
     full_name: Optional[str] = Field(None, description="""a long-form human readable name for a thing""")
     iri: Optional[str] = Field(None, description="""An IRI for an entity. This is determined by the id using expansion rules.""")
     category: List[Literal["https://identifiers.org/brain-bican/vocab/GeneAnnotation","bican:GeneAnnotation"]] = Field(["bican:GeneAnnotation"], description="""Name of the high level ontology class in which this entity is categorized. Corresponds to the label for the biolink entity type class.
  * In a neo4j database this MAY correspond to the neo4j label tag.
  * In an RDF database it should be a biolink model class URI.
```

### Comparing `bkbit-0.0.1/pyproject.toml` & `bkbit-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 [build-system]
 # Setuptools version should match setup.py; wheel because pip will insert it noisily
 requires = ["setuptools >= 61.0", "setuptools-scm"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "bkbit"
-version = "0.0.1"
 authors = [
   { name="atlaskb developers"},
 ]
 description = "A library for atlaskb data models"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 license = {text = "Apache 2.0"}
 dependencies = [
     "linkml>=1.5",
+    "pandas"
 ]
+dynamic = ["version"]
+
 
 [project.optional-dependencies]
 test = [
     "pytest",
 ]
 docs = [
     "mkdocs-material"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/atlaskb/bkbit"
+
+[tool.setuptools_scm]
+write_to = "bkbit/_version.py"
```

