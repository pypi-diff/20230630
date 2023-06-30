# Comparing `tmp/pathogen-embed-0.1.1.tar.gz` & `tmp/pathogen-embed-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathogen-embed-0.1.1.tar", last modified: Thu Jun 22 23:30:59 2023, max compression
+gzip compressed data, was "pathogen-embed-1.0.0.tar", last modified: Fri Jun 30 20:26:59 2023, max compression
```

## Comparing `pathogen-embed-0.1.1.tar` & `pathogen-embed-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-22 23:30:59.665323 pathogen-embed-0.1.1/
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     1068 2023-06-21 05:19:15.000000 pathogen-embed-0.1.1/LICENSE
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     4810 2023-06-22 23:30:59.658745 pathogen-embed-0.1.1/PKG-INFO
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     3879 2023-06-22 23:23:27.000000 pathogen-embed-0.1.1/README.md
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      103 2022-01-21 05:41:32.000000 pathogen-embed-0.1.1/pyproject.toml
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)       38 2023-06-22 23:30:59.667792 pathogen-embed-0.1.1/setup.cfg
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     1764 2023-06-22 23:26:13.000000 pathogen-embed-0.1.1/setup.py
-drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-22 23:30:58.639024 pathogen-embed-0.1.1/src/
-drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-22 23:30:59.136146 pathogen-embed-0.1.1/src/embed/
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     5341 2023-06-21 15:35:01.000000 pathogen-embed-0.1.1/src/embed/__init__.py
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      337 2022-01-21 05:41:32.000000 pathogen-embed-0.1.1/src/embed/__main__.py
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)    13721 2023-01-12 19:45:51.000000 pathogen-embed-0.1.1/src/embed/embed.py
-drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-22 23:30:59.591062 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     4810 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/PKG-INFO
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      358 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/SOURCES.txt
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        1 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/dependency_links.txt
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)       46 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/entry_points.txt
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)       74 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/requires.txt
--rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        6 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/top_level.txt
+drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-30 20:26:59.082073 pathogen-embed-1.0.0/
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     1068 2023-06-21 05:19:15.000000 pathogen-embed-1.0.0/LICENSE
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     4808 2023-06-30 20:26:59.073358 pathogen-embed-1.0.0/PKG-INFO
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     3879 2023-06-22 23:23:27.000000 pathogen-embed-1.0.0/README.md
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      103 2022-01-21 05:41:32.000000 pathogen-embed-1.0.0/pyproject.toml
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)       38 2023-06-30 20:26:59.082073 pathogen-embed-1.0.0/setup.cfg
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     2176 2023-06-30 20:23:00.000000 pathogen-embed-1.0.0/setup.py
+drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-30 20:26:58.153805 pathogen-embed-1.0.0/src/
+drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-30 20:26:58.560521 pathogen-embed-1.0.0/src/pathogen_embed/
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      275 2023-06-30 20:23:00.000000 pathogen-embed-1.0.0/src/pathogen_embed/__init__.py
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     6771 2023-06-30 20:23:01.000000 pathogen-embed-1.0.0/src/pathogen_embed/__main__.py
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)    14462 2023-06-30 20:23:01.000000 pathogen-embed-1.0.0/src/pathogen_embed/pathogen_embed.py
+drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-30 20:26:58.990175 pathogen-embed-1.0.0/src/pathogen_embed.egg-info/
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     4808 2023-06-30 20:26:57.000000 pathogen-embed-1.0.0/src/pathogen_embed.egg-info/PKG-INFO
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      394 2023-06-30 20:26:58.000000 pathogen-embed-1.0.0/src/pathogen_embed.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        1 2023-06-30 20:26:57.000000 pathogen-embed-1.0.0/src/pathogen_embed.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      181 2023-06-30 20:26:57.000000 pathogen-embed-1.0.0/src/pathogen_embed.egg-info/entry_points.txt
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)       94 2023-06-30 20:26:57.000000 pathogen-embed-1.0.0/src/pathogen_embed.egg-info/requires.txt
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)       15 2023-06-30 20:26:57.000000 pathogen-embed-1.0.0/src/pathogen_embed.egg-info/top_level.txt
```

### Comparing `pathogen-embed-0.1.1/LICENSE` & `pathogen-embed-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathogen-embed-0.1.1/PKG-INFO` & `pathogen-embed-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pathogen-embed
-Version: 0.1.1
+Version: 1.0.0
 Summary: Reduced dimension embeddings for pathogen sequences
 Home-page: https://github.com/blab/pathogen-embed/
 Author: Sravani Nanduri <nandsra@cs.washington.edu> , John Huddleston <huddlej@gmail.com>
 Author-email: nandsra@cs.washington.edu
 License: MIT License
 Project-URL: Documentation, https://blab.github.io/pathogen-embed/
 Project-URL: Bug Reports, https://github.com/blab/pathogen-embed/issues
 Project-URL: Source Code, https://github.com/blab/pathogen-embed/tree/main
-Project-URL: Change Log, https://github.com/blab/pathogen-embed/tree/master/CHANGES.md
+Project-URL: Change Log, https://github.com/blab/pathogen-embed/tree/main/CHANGES.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pathogen-embed-0.1.1/README.md` & `pathogen-embed-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pathogen-embed-0.1.1/setup.py` & `pathogen-embed-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,46 +3,51 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pathogen-embed',
-    version='0.1.1',
+    version='1.0.0',
     description='Reduced dimension embeddings for pathogen sequences',
     url='https://github.com/blab/pathogen-embed/',
     author='Sravani Nanduri <nandsra@cs.washington.edu> , John Huddleston <huddlej@gmail.com>',
     author_email='nandsra@cs.washington.edu',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT License',
     project_urls = {
         "Documentation": "https://blab.github.io/pathogen-embed/",
         "Bug Reports": "https://github.com/blab/pathogen-embed/issues",
         "Source Code": "https://github.com/blab/pathogen-embed/tree/main",
-	"Change Log": "https://github.com/blab/pathogen-embed/tree/master/CHANGES.md",
+        "Change Log": "https://github.com/blab/pathogen-embed/tree/main/CHANGES.md",
     },
     package_dir={"": "src"},
-	packages = find_packages(where="src", exclude=['test']),
-    #packages=['seaborn', 'scikit-learn', 'umap-learn', 'matplotlib', 'pandas', 'numpy', 'hdbscan'],
+    packages=find_packages(where="src", exclude=['test']),
     install_requires=['numpy',
                       'pandas',
                       "biopython",
                       'seaborn',
                       'scikit-learn',
-                      'umap-learn',
+                      'umap-learn ==0.5.*',
+                      # Pin Numba at maximum supported version for the pinned umap-learn version.
+                      # For more details see:
+                      # https://numba.readthedocs.io/en/stable/reference/deprecation.html#deprecation-of-object-mode-fall-back-behaviour-when-using-jit
+                      'numba <0.59.0',
                       'matplotlib',
                       'hdbscan'
                       ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
     ],
     entry_points = {
         "console_scripts": [
-            "embed = embed.__main__:main",
+            "pathogen-embed = pathogen_embed.__main__:run_embed",
+            "pathogen-distance = pathogen_embed.__main__:run_distance",
+            "pathogen-cluster = pathogen_embed.__main__:run_cluster"
         ]
     }
 )
```

### Comparing `pathogen-embed-0.1.1/src/embed/__init__.py` & `pathogen-embed-1.0.0/src/pathogen_embed/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-"""
-pathogen-embed.
-
-Reduced dimension embeddings for pathogen sequences.
-"""
-
-__version__ = "0.1.0"
-__author__ = 'Sravani Nanduri, John Huddleston'
-__credits__ = 'Bedford Lab, Vaccine and Infectious Disease Division, Fred Hutchinson Cancer Research Center, Seattle, WA, USA'
-
 import argparse
 import sys
-from .embed import embed, get_hamming_distances
+from sys import argv
+from .pathogen_embed import embed, distance, cluster
 
-def make_parser():
+def make_parser_embed():
     parser = argparse.ArgumentParser(description = "Reduced dimension embeddings for pathogen sequences", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
+    parser.add_argument("--alignment", required = True, help="an aligned FASTA file to create a distance matrix with. Make sure the strain order in this file matches the order in the distance matrix.")
     parser.add_argument("--distance-matrix", help="a distance matrix that can be read in by pandas, index column as row 0")
     parser.add_argument("--separator", default=",", help="separator between columns in the given distance matrix")
-    parser.add_argument("--alignment", help="an aligned FASTA file to create a distance matrix with. Make sure the strain order in this file matches the order in the distance matrix.")
-    parser.add_argument("--cluster-data", help="The file (same separator as distance-matrix) that contains the distance threshold by which to cluster data in the embedding and assign labels given via HDBSCAN (https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html). If no value is given in cluster-data or cluster-threshold, the default distance threshold of 0.0 will be used. If any additional columns in this file match embedding-specific parameters (e.g., 'n_components' or 'learning_rate'), the values from the first record of this file will override default values or values provided by the command line arguments.")
-    parser.add_argument("--cluster-min-size", type=int, default=5, help="minimum cluster size for HDBSCAN")
-    parser.add_argument("--cluster-min-samples", type=int, default=5, help="minimum number of sample to seed a cluster for HDBSCAN. Lowering this value reduces number of samples that do not get clustered.")
-    parser.add_argument("--cluster-threshold", type=float, help="The float value for the distance threshold by which to cluster data in the embedding and assign labels via HDBSCAN. If no value is given in cluster-data or cluster-threshold, the default distance threshold of 0.0 will be used.")
-    parser.add_argument("--random-seed", default = 314159, type=int, help="an integer used for reproducible results.")
     parser.add_argument("--indel-distance", action="store_true", help="include insertions/deletions in genetic distance calculations")
+    parser.add_argument("--random-seed", default = 314159, type=int, help="an integer used for reproducible results.")
     parser.add_argument("--output-dataframe", help="a csv file outputting the embedding with the strain name and its components.")
     parser.add_argument("--output-figure", help="outputs a PNG plot of the embedding")
+    parser.add_argument("--embedding-parameters", help="The file containing the parameters by which to tune the embedding. The values from the first record of this file will override default values or values provided by the command line arguments.")
 
     subparsers = parser.add_subparsers(
         dest="command",
         required=True
     )
 
     pca = subparsers.add_parser("pca", description="Principal Component Analysis")
@@ -47,15 +35,53 @@
     umap.add_argument("--min-dist", default=.5, type=float, help="Minimum Distance controls how tightly packed the UMAP embedding is. While it does not change the structure of the data, it does change the embedding's shape. The default value is the value consistently the best for pathogen analyses, results from an exhaustive grid search.")
 
     mds = subparsers.add_parser("mds", description="Multidimensional Scaling")
     mds.add_argument("--components", default=10, type=int, help="the number of components for MDS")
 
     return parser
 
+def make_parser_distance():
+    parser = argparse.ArgumentParser(description = "Hamming distance (optionally indel sensitive) similarity matrix for pathogen sequences", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+
+    parser.add_argument("--alignment", required = True,  help="an aligned FASTA file to create a distance matrix with. Make sure the strain order in this file matches the order in the distance matrix.")
+    parser.add_argument("--indel-distance", action="store_true", help="include insertions/deletions in genetic distance calculations")
+    parser.add_argument("--output", required = True, help="a csv file outputting the distance matrix annotated with strain names as the columns")
+   
+    return parser
+
+def make_parser_cluster():
+    parser = argparse.ArgumentParser(description = "HDBSCAN clustering for reduced dimension embeddings", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+
+    parser.add_argument("--embedding", required = True, help="The embedding to assign clustering labels to via HDBSCAN (https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)")
+    parser.add_argument("--label-attribute", help="the name of the cluster used to label the column in the resulting dataframe")
+    parser.add_argument("--random-seed", default = 314159, type=int, help="an integer used for reproducible results.")
+    parser.add_argument("--min-size", type=int, default=5, help="minimum cluster size for HDBSCAN")
+    parser.add_argument("--min-samples", type=int, default=5, help="minimum number of sample to seed a cluster for HDBSCAN. Lowering this value reduces number of samples that do not get clustered.")
+    parser.add_argument("--distance-threshold", type=float, help="The float value for the distance threshold by which to cluster data in the embedding and assign labels via HDBSCAN. If no value is given in distance-threshold, the default distance threshold of 0.0 will be used.")
+    parser.add_argument("--output-dataframe", required = True, help="a csv file outputting the embedding with the strain name and its components.")
+    parser.add_argument("--output-figure", help="outputs a PDF with a plot of the embedding colored by cluster")
 
-def run(argv):
-    args = make_parser().parse_args(argv)
+    return parser
+
+def run_embed():
     try:
+        args = make_parser_embed().parse_args(argv[1:])
         return embed(args)
     except Exception as error:
         print(error, file=sys.stderr)
         sys.exit(1)
+   
+def run_distance():
+    try:
+        args = make_parser_distance().parse_args(argv[1:])
+        return distance(args)
+    except Exception as error:
+        print(error, file=sys.stderr)
+        sys.exit(1)
+
+def run_cluster():
+    try:
+        args = make_parser_cluster().parse_args(argv[1:])
+        return cluster(args)
+    except Exception as error:
+        print(error, file=sys.stderr)
+        sys.exit(1)
```

### Comparing `pathogen-embed-0.1.1/src/embed/embed.py` & `pathogen-embed-1.0.0/src/pathogen_embed/pathogen_embed.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,16 @@
-import argparse
+# Ignore warnings from Numba deprecation:
+# https://numba.readthedocs.io/en/stable/reference/deprecation.html#deprecation-of-object-mode-fall-back-behaviour-when-using-jit
+# Numba is required by UMAP.
+from numba.core.errors import NumbaDeprecationWarning
+import warnings
+
+warnings.simplefilter('ignore', category=NumbaDeprecationWarning)
 
+import argparse
 import Bio.SeqIO
 from collections import OrderedDict
 import hdbscan
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import re
@@ -171,16 +178,14 @@
 
             hamming_distances.append(distance)
 
     return hamming_distances
 
 
 def embed(args):
-    # TODO: Create a default cluster distance threshold if none given.
-
     # Setting Random seed for numpy
     np.random.seed(seed=args.random_seed)
 
     if args.output_dataframe is None and args.output_figure is None:
         print("You must specify one of the outputs", file=sys.stderr)
         sys.exit(1)
 
@@ -199,53 +204,32 @@
         for sequence in Bio.SeqIO.parse(args.alignment, "fasta"):
             sequences_by_name[sequence.id] = str(sequence.seq)
 
         sequence_names = list(sequences_by_name.keys())
         if args.command != "pca" and distance_matrix is None:
             # Calculate Distance Matrix
             hamming_distances = get_hamming_distances(
-                sequences_by_name.values(),
+                list(sequences_by_name.values()),
                 args.indel_distance,
             )
             distance_matrix = pd.DataFrame(squareform(hamming_distances))
             distance_matrix.index = sequence_names
 
-    # Calculate Embedding
-    clusterer = None
-
-    if args.cluster_threshold is not None:
-        cluster_threshold = float(args.cluster_threshold)
-        clusterer = hdbscan.HDBSCAN(
-            min_cluster_size=args.cluster_min_size,
-            min_samples=args.cluster_min_samples,
-            cluster_selection_epsilon=cluster_threshold,
-        )
-
-    # Load embedding and cluster parameters from an external CSV file, if
-    # possible.
-    cluster_data = None
-    if args.cluster_data is not None:
-        max_df = pd.read_csv(args.cluster_data)
-
-        # Look for cluster distance threshold in the cluster data, if the user
-        # has not provided a value from the command line.
-        if args.cluster_threshold is None:
-            clusterer = hdbscan.HDBSCAN(
-                min_cluster_size=args.cluster_min_size,
-                min_samples=args.cluster_min_samples,
-                cluster_selection_epsilon=float(max_df.where(max_df["method"] == args.command).dropna(subset = ['distance_threshold'])[["distance_threshold"]].values.tolist()[0][0])
-            )
-
-        # Get a dictionary of additional parameters provided by the cluster data
-        # to override defaults for the current method.
-        cluster_data = max_df.to_dict("records")[0]
-
-    if cluster_data is not None and "components" in cluster_data:
-        n_components = int(cluster_data["components"])
-        cluster_data["n_components"] = n_components
+    # Load embedding parameters from an external CSV file, if possible.
+    external_embedding_parameters = None
+    if args.embedding_parameters is not None:
+        external_embedding_parameters_df = pd.read_csv(args.embedding_parameters)
+
+        # Get a dictionary of additional parameters provided by the external
+        # file to override defaults for the current method.
+        external_embedding_parameters = external_embedding_parameters_df.to_dict("records")[0]
+
+    if external_embedding_parameters is not None and "components" in external_embedding_parameters:
+        n_components = int(external_embedding_parameters["components"])
+        external_embedding_parameters["n_components"] = n_components
     else:
         n_components = args.components
 
     # Use PCA as its own embedding or as an initialization for t-SNE.
     if args.command == "pca" or args.command == "t-sne":
         sequence_names = list(sequences_by_name.keys())
 
@@ -254,70 +238,71 @@
             numbers[i] = re.sub(r'[^AGCT]', '5', numbers[i])
             numbers[i] = list(numbers[i].replace('A','1').replace('G','2').replace('C', '3').replace('T','4'))
             numbers[i] = [int(j) for j in numbers[i]]
 
         genomes_df = pd.DataFrame(numbers)
         genomes_df.columns = ["Site " + str(k) for k in range(0,len(numbers[i]))]
 
+
         #performing PCA on my pandas dataframe
-        pca = PCA(n_components=n_components, svd_solver='full') #can specify n, since with no prior knowledge, I use None
+        pca = PCA(n_components=n_components, svd_solver='full')
         principalComponents = pca.fit_transform(genomes_df)
 
         # Create a data frame from the PCA embedding.
         embedding = principalComponents
         embedding_df = pd.DataFrame(principalComponents)
         embedding_df.index = sequence_names
 
     if args.command == "t-sne":
         embedding_class = TSNE
         embedding_parameters = {
-            "n_components": args.components,
+            "n_components": n_components,
             "metric": "precomputed",
-            "init": principalComponents[:, :args.components],
+            "init": principalComponents[:, :n_components],
             "perplexity": args.perplexity,
             "learning_rate": args.learning_rate,
             "random_state" : args.random_seed,
             "square_distances": True,
         }
     elif args.command == "umap":
         embedding_class = UMAP
         embedding_parameters = {
             "n_neighbors": args.nearest_neighbors,
             "min_dist": args.min_dist,
-            "n_components": args.components,
+            "n_components": n_components,
             "init": "spectral",
             "random_state" : args.random_seed
         }
     elif args.command == "mds":
         embedding_class = MDS
         embedding_parameters = {
             "dissimilarity": "precomputed",
-            "n_components": args.components,
+            "n_components": n_components,
             "n_jobs": 1,
             "n_init": 2
         }
 
-    # Override defaults with parameter values passed through cluster data, if
+    # Override defaults with parameter values passed through embedding parameters, if
     # possible.
-    if cluster_data is not None and args.command != "pca":
-        for key, value in cluster_data.items():
+    if external_embedding_parameters is not None and args.command != "pca":
+        for key, value in external_embedding_parameters.items():
             if key in embedding_parameters:
                 value_type = type(embedding_parameters[key])
                 print(
-                    f"INFO: Replacing embedding parameter {key} value of '{embedding_parameters[key]}' with '{value_type(value)}' provided by '{args.cluster_data}'.",
+                    f"INFO: Replacing embedding parameter {key} value of '{embedding_parameters[key]}' with '{value_type(value)}' provided by '{args.embedding_parameters}'.",
                     file=sys.stderr
                 )
                 embedding_parameters[key] = value_type(value)
 
     if args.command != "pca":
         embedder = embedding_class(**embedding_parameters)
         embedding = embedder.fit_transform(distance_matrix)
 
         # Output Embedding
-            # create dictionary to be "wrapped" by write_json
+        # create dictionary to be "wrapped" by write_json
 
         embedding_df = pd.DataFrame(embedding)
         embedding_df.index = list(distance_matrix.index)
 
     if args.command == "mds" or args.command == "pca":
         embedding_df.columns=[args.command + str(i) for i in range(1, n_components + 1)]
     else:
@@ -326,38 +311,81 @@
     if args.command == "pca":
 
         #add explained variance as the first row of the dataframe
         explained_variance = pd.DataFrame([round(pca.explained_variance_ratio_[i],4) for i in range(0,len(pca.explained_variance_ratio_))], columns=["explained variance"])
         explained_variance["principal components"] = [i for i in range(1, n_components + 1)]
         explained_variance.to_csv(args.explained_variance, index=False)
 
-    if clusterer is not None:
-        clusterer_default = hdbscan.HDBSCAN()
-        clusterer.fit(embedding_df)
-        clusterer_default.fit(embedding_df)
-        embedding_df[f"{args.command}_label"] = clusterer.labels_.astype(str)
-        embedding_df[f"{args.command}_label_default"] = clusterer_default.labels_.astype(str)
-
     if args.output_dataframe is not None:
         embedding_df.to_csv(args.output_dataframe, index_label="strain")
 
     if args.output_figure:
         plot_data = {
             "x": embedding[:, 0],
             "y": embedding[:, 1],
         }
 
-        if clusterer is not None:
-            plot_data["cluster"] = clusterer.labels_.astype(str)
-        else:
-            plot_data["cluster"] = "0"
+        plot_df = pd.DataFrame(plot_data)
+        ax = sns.scatterplot(
+            data=plot_df,
+            x="x",
+            y="y",
+            alpha=0.5,
+        )
+        plt.savefig(args.output_figure)
+        plt.close()
+
+def cluster(args):
+
+    embedding_df = pd.read_csv(args.embedding, index_col=0)
+
+    clustering_parameters = {
+        **({"min_cluster_size": args.min_size} if args.min_size is not None else {}),
+        **({"min_samples": args.min_samples} if args.min_samples is not None else {}),
+        **({"cluster_selection_epsilon": args.distance_threshold} if args.distance_threshold is not None else {})
+    }
+
+    clusterer = hdbscan.HDBSCAN(**clustering_parameters)
+
+    clusterer.fit(embedding_df)
+    embedding_df[args.label_attribute] = clusterer.labels_.astype(str)
+
+    if args.output_figure is not None:
+
+        plot_data = {
+            "x": embedding_df.to_numpy()[:, 0],
+            "y": embedding_df.to_numpy()[:, 1],
+        }
+
+        plot_data["cluster"] = clusterer.labels_.astype(str)
 
         plot_df = pd.DataFrame(plot_data)
         ax = sns.scatterplot(
             data=plot_df,
             x="x",
             y="y",
             hue="cluster",
             alpha=0.5,
         )
         plt.savefig(args.output_figure)
         plt.close()
+
+    if args.output_dataframe is not None:
+        embedding_df.to_csv(args.output_dataframe, index_label="strain")
+
+def distance(args):
+    sequences_by_name = OrderedDict()
+
+    for sequence in Bio.SeqIO.parse(args.alignment, "fasta"):
+        sequences_by_name[sequence.id] = str(sequence.seq)
+
+    sequence_names = list(sequences_by_name.keys())
+
+    hamming_distances = get_hamming_distances(
+        list(sequences_by_name.values()),
+        args.indel_distance,
+    )
+    distance_matrix = pd.DataFrame(squareform(hamming_distances))
+    distance_matrix.index = sequence_names
+    distance_matrix.columns = distance_matrix.index
+
+    distance_matrix.to_csv(args.output)
```

### Comparing `pathogen-embed-0.1.1/src/pathogen_embed.egg-info/PKG-INFO` & `pathogen-embed-1.0.0/src/pathogen_embed.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pathogen-embed
-Version: 0.1.1
+Version: 1.0.0
 Summary: Reduced dimension embeddings for pathogen sequences
 Home-page: https://github.com/blab/pathogen-embed/
 Author: Sravani Nanduri <nandsra@cs.washington.edu> , John Huddleston <huddlej@gmail.com>
 Author-email: nandsra@cs.washington.edu
 License: MIT License
 Project-URL: Documentation, https://blab.github.io/pathogen-embed/
 Project-URL: Bug Reports, https://github.com/blab/pathogen-embed/issues
 Project-URL: Source Code, https://github.com/blab/pathogen-embed/tree/main
-Project-URL: Change Log, https://github.com/blab/pathogen-embed/tree/master/CHANGES.md
+Project-URL: Change Log, https://github.com/blab/pathogen-embed/tree/main/CHANGES.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

