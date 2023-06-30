# Comparing `tmp/arraylib_solve-0.8.0.tar.gz` & `tmp/arraylib_solve-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraylib_solve-0.8.0.tar", max compression
+gzip compressed data, was "arraylib_solve-0.9.0.tar", max compression
```

## Comparing `arraylib_solve-0.8.0.tar` & `arraylib_solve-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4718 2023-02-24 13:40:05.579370 arraylib_solve-0.8.0/README.md
--rw-r--r--   0        0        0      753 2023-03-07 13:21:34.722316 arraylib_solve-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-13 10:54:08.516050 arraylib_solve-0.8.0/pysudoku_package/__init__.py
--rwxr-xr-x   0        0        0     3059 2023-03-07 10:18:27.850733 arraylib_solve-0.8.0/pysudoku_package/alignment.py
--rwxr-xr-x   0        0        0     2117 2023-02-22 14:15:09.317010 arraylib_solve-0.8.0/pysudoku_package/config.py
--rwxr-xr-x   0        0        0    10730 2023-03-07 12:11:32.047320 arraylib_solve-0.8.0/pysudoku_package/deconvolution.py
--rwxr-xr-x   0        0        0     7184 2023-03-07 10:36:20.757296 arraylib_solve-0.8.0/pysudoku_package/generate_count_matrix.py
--rwxr-xr-x   0        0        0      839 2023-02-23 08:36:28.360365 arraylib_solve-0.8.0/pysudoku_package/io.py
--rw-r--r--   0        0        0     8351 2023-03-07 10:36:28.641373 arraylib_solve-0.8.0/pysudoku_package/libraryexperiment.py
--rw-r--r--   0        0        0     5650 2023-02-09 09:00:09.902405 arraylib_solve-0.8.0/pysudoku_package/main.py
--rw-r--r--   0        0        0     3693 2023-03-07 12:09:14.942533 arraylib_solve-0.8.0/pysudoku_package/predict_locations.py
--rwxr-xr-x   0        0        0     3841 2022-10-13 10:54:08.520051 arraylib_solve-0.8.0/pysudoku_package/trimming.py
--rw-r--r--   0        0        0     5814 1970-01-01 00:00:00.000000 arraylib_solve-0.8.0/setup.py
--rw-r--r--   0        0        0     5515 1970-01-01 00:00:00.000000 arraylib_solve-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4719 2023-05-09 13:39:16.289426 arraylib_solve-0.9.0/README.md
+-rw-r--r--   0        0        0      753 2023-05-09 13:39:56.333981 arraylib_solve-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-13 10:54:08.516050 arraylib_solve-0.9.0/pysudoku_package/__init__.py
+-rwxr-xr-x   0        0        0     3059 2023-03-07 10:18:27.850733 arraylib_solve-0.9.0/pysudoku_package/alignment.py
+-rwxr-xr-x   0        0        0     2117 2023-02-22 14:15:09.317010 arraylib_solve-0.9.0/pysudoku_package/config.py
+-rwxr-xr-x   0        0        0    10730 2023-03-07 12:11:32.047320 arraylib_solve-0.9.0/pysudoku_package/deconvolution.py
+-rwxr-xr-x   0        0        0     7184 2023-03-07 10:36:20.757296 arraylib_solve-0.9.0/pysudoku_package/generate_count_matrix.py
+-rwxr-xr-x   0        0        0      839 2023-02-23 08:36:28.360365 arraylib_solve-0.9.0/pysudoku_package/io.py
+-rw-r--r--   0        0        0     8351 2023-03-07 10:36:28.641373 arraylib_solve-0.9.0/pysudoku_package/libraryexperiment.py
+-rw-r--r--   0        0        0     5650 2023-02-09 09:00:09.902405 arraylib_solve-0.9.0/pysudoku_package/main.py
+-rw-r--r--   0        0        0     3693 2023-03-07 12:09:14.942533 arraylib_solve-0.9.0/pysudoku_package/predict_locations.py
+-rwxr-xr-x   0        0        0     3841 2022-10-13 10:54:08.520051 arraylib_solve-0.9.0/pysudoku_package/trimming.py
+-rw-r--r--   0        0        0     5815 1970-01-01 00:00:00.000000 arraylib_solve-0.9.0/setup.py
+-rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 arraylib_solve-0.9.0/PKG-INFO
```

### Comparing `arraylib_solve-0.8.0/README.md` & `arraylib_solve-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 # How to run `arraylib-solve`
 
 To run `arraylib-solve` on a library deconvolution experiment with default parameters run:
 
 ```
-arraylib-run <input_directory> <experimental_design.csv> -c <number_of_cpu_cores_to_use> -b <path_to_genbank_reference> -br <path_to_bowtie2_indices> -t <transposon_sequence> -bu <upstream_sequence_of_barcodes> -bd <downstream_sequence_of_barcodes>
+arraylib-run <input_directory> <experimental_design.csv> -c <number_of_cpu_cores_to_use> -gb <path_to_genbank_reference> -br <path_to_bowtie2_indices> -t <transposon_sequence> -bu <upstream_sequence_of_barcodes> -bd <downstream_sequence_of_barcodes>
 ```
 
 ## Input parameters
 
 Required parameters:
 * input_dir: path to directory holding the input fastq files
 * exp_design: path to csv file indicating experimental design (values should be separated by a comma). The experimental design file
```

### Comparing `arraylib_solve-0.8.0/pyproject.toml` & `arraylib_solve-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arraylib-solve"
-version = "0.8.0"
+version = "0.9.0"
 description = "Tool to computationally deconvolve combinatorially pooled arrayed random mutagenesis libraries"
 authors = ["capraz <tuemayc@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "pysudoku_package"}]
 license = "MIT"
 
 [tool.pytest.ini_options]
```

### Comparing `arraylib_solve-0.8.0/pysudoku_package/alignment.py` & `arraylib_solve-0.9.0/pysudoku_package/alignment.py`

 * *Files identical despite different names*

### Comparing `arraylib_solve-0.8.0/pysudoku_package/config.py` & `arraylib_solve-0.9.0/pysudoku_package/config.py`

 * *Files identical despite different names*

### Comparing `arraylib_solve-0.8.0/pysudoku_package/deconvolution.py` & `arraylib_solve-0.9.0/pysudoku_package/deconvolution.py`

 * *Files identical despite different names*

### Comparing `arraylib_solve-0.8.0/pysudoku_package/generate_count_matrix.py` & `arraylib_solve-0.9.0/pysudoku_package/generate_count_matrix.py`

 * *Files identical despite different names*

### Comparing `arraylib_solve-0.8.0/pysudoku_package/io.py` & `arraylib_solve-0.9.0/pysudoku_package/io.py`

 * *Files identical despite different names*

### Comparing `arraylib_solve-0.8.0/pysudoku_package/libraryexperiment.py` & `arraylib_solve-0.9.0/pysudoku_package/libraryexperiment.py`

 * *Files identical despite different names*

### Comparing `arraylib_solve-0.8.0/pysudoku_package/main.py` & `arraylib_solve-0.9.0/pysudoku_package/main.py`

 * *Files identical despite different names*

### Comparing `arraylib_solve-0.8.0/pysudoku_package/predict_locations.py` & `arraylib_solve-0.9.0/pysudoku_package/predict_locations.py`

 * *Files identical despite different names*

### Comparing `arraylib_solve-0.8.0/pysudoku_package/trimming.py` & `arraylib_solve-0.9.0/pysudoku_package/trimming.py`

 * *Files identical despite different names*

### Comparing `arraylib_solve-0.8.0/setup.py` & `arraylib_solve-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 entry_points = \
 {'console_scripts': ['arraylib-deconvolve = pysudoku_package.main:deconvolve',
                      'arraylib-run = pysudoku_package.main:run']}
 
 setup_kwargs = {
     'name': 'arraylib-solve',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Tool to computationally deconvolve combinatorially pooled arrayed random mutagenesis libraries',
-    'long_description': '# arraylib-solve\n\n# Introduction\n\n`arraylib-solve` is a tool to deconvolve combinatorially pooled arrayed random mutagenesis libraries (e.g. by transposon mutagenesis). In a typical experiment generating arrayed mutagenesis libraries, first a pooled version of the library is created and arrayed on a grid of well plates. To infer the identities of each mutant on the well plate, wells are pooled in combinatorial manner such that each mutant appears in a unique combination of pools. The pools are then sequenced using NGS and sequenced reads are stored in individual fastq files per pool. `arraylib-solve` deconvolves the pools and returns summaries stating the identity and location of each mutant on the original well grid. The package is based on the approach described in [[1]](#1).\n\n# Installation\n\nTo install `arraylib-solve` first create `Python 3.8` environment e.g. by\n\n```\nconda create --name arraylib-env python=3.8\nconda activate arraylib-env\n```\n\nand install the package using \n\n```\npip install arraylib-solve\n```\n\n`arraylib-solve` uses bowtie2 [[2]](#2) to align reads to the reference genome. Please ensure that bowtie2 is installed in your environment by running:\n\n```\nconda install -c bioconda bowtie2\n```\n\n\n# How to run `arraylib-solve`\n\nTo run `arraylib-solve` on a library deconvolution experiment with default parameters run:\n\n```\narraylib-run <input_directory> <experimental_design.csv> -c <number_of_cpu_cores_to_use> -b <path_to_genbank_reference> -br <path_to_bowtie2_indices> -t <transposon_sequence> -bu <upstream_sequence_of_barcodes> -bd <downstream_sequence_of_barcodes>\n```\n\n## Input parameters\n\nRequired parameters:\n* input_dir: path to directory holding the input fastq files\n* exp_design: path to csv file indicating experimental design (values should be separated by a comma). The experimental design file \n       should have columns, Filename, Poolname and Pooldimension. (see example in tests/test_data/full_exp_design.csv)\n  * Filename should contain all the unqiue input fastq filenames.\n  * Poolname should indicate to which pool a given file belongs. Multiple files per poolname are allowed.\n  * Pooldimension indicates the pooling dimension a pool belongs to. All pools sharing the same pooling dimension should have the same string in the Pooldimension column.\n  \n\nAn example of how an exp_design file could look like:\n\n| Filename          | Poolname        | Pooldimension  |\n| :---------------: | :-------------: | :------------: |\n| column1.fastq     | column1         | columns        |\n| column2.fastq     | column2         | columns        |\n| row1.fastq        | row1            | rows           |\n| row2.fastq        | row2            | rows           |\n| platerow1.fastq   | platerow1       | platerows      |\n| platerow2.fastq   | platerow2       | platerows      |\n| platecol1.fastq   | platecol1       | platecols      |\n| platecol2.fastq   | platecol2       | platecols      |\n\n* -gb path to genbank reference file\n* -br path to bowtie index files, ending with the basename of your index (if the basename of your index is UTI89 and you store your bowtie2 references in bowtie_ref it should be bowtie_ref/UTI89). Please visit https://bowtie-bio.sourceforge.net/bowtie2/manual.shtml#the-bowtie2-build-indexer for a manual how to create bowtie2 indices.\n* -t transposon sequence (e.g. AGATGTGTATAAGAGACAG)\n* -bu upstream sequence of barcode (e.g. CGAGGTCTCT)\n* -bd downstream sequence of barcode (e.g. CGTACGCTGC)\n\nOptional parameters:\n* -mq minimum bowtie2 alignment quality score for each base to include read\n* -sq minimum phred score for each base to include read\n* -tm number of transposon mismatches allowed\n* -thr threshold for local filter (e.g. a threshold of 0.05 would filter out all reads < 0.05 of the maximum read count for a given mutant)\n\n## Output\n\n`arraylib-solve` outputs 4 files: \n* count_matrix.csv: Read counts per pool for each mutant.\n* filtered_matrix.csv: Read counts per pool for each mutant, but mutants with barcodes with low read counts for a given genomic location are filtered out.\n* mutant_location_summary.csv: A summary of mutants found in the well plate grid, where each row corresponds to a different mutant.\n* well_location_summary.csv: A summary of the deconvolved well plate grid, where each row corresponds to a different well.\n\n\n\n# References\n<a id="1">[1]</a> \nBaym, M., Shaket, L., Anzai, I.A., Adesina, O. and Barstow, B., 2016. Rapid construction of a whole-genome transposon insertion collection for Shewanella oneidensis by Knockout Sudoku. Nature communications, 7(1), p.13270.\\\n<a id="2">[2]</a> \nLangmead, B. and Salzberg, S.L., 2012. Fast gapped-read alignment with Bowtie 2. Nature methods, 9(4), pp.357-359.\n\n',
+    'long_description': '# arraylib-solve\n\n# Introduction\n\n`arraylib-solve` is a tool to deconvolve combinatorially pooled arrayed random mutagenesis libraries (e.g. by transposon mutagenesis). In a typical experiment generating arrayed mutagenesis libraries, first a pooled version of the library is created and arrayed on a grid of well plates. To infer the identities of each mutant on the well plate, wells are pooled in combinatorial manner such that each mutant appears in a unique combination of pools. The pools are then sequenced using NGS and sequenced reads are stored in individual fastq files per pool. `arraylib-solve` deconvolves the pools and returns summaries stating the identity and location of each mutant on the original well grid. The package is based on the approach described in [[1]](#1).\n\n# Installation\n\nTo install `arraylib-solve` first create `Python 3.8` environment e.g. by\n\n```\nconda create --name arraylib-env python=3.8\nconda activate arraylib-env\n```\n\nand install the package using \n\n```\npip install arraylib-solve\n```\n\n`arraylib-solve` uses bowtie2 [[2]](#2) to align reads to the reference genome. Please ensure that bowtie2 is installed in your environment by running:\n\n```\nconda install -c bioconda bowtie2\n```\n\n\n# How to run `arraylib-solve`\n\nTo run `arraylib-solve` on a library deconvolution experiment with default parameters run:\n\n```\narraylib-run <input_directory> <experimental_design.csv> -c <number_of_cpu_cores_to_use> -gb <path_to_genbank_reference> -br <path_to_bowtie2_indices> -t <transposon_sequence> -bu <upstream_sequence_of_barcodes> -bd <downstream_sequence_of_barcodes>\n```\n\n## Input parameters\n\nRequired parameters:\n* input_dir: path to directory holding the input fastq files\n* exp_design: path to csv file indicating experimental design (values should be separated by a comma). The experimental design file \n       should have columns, Filename, Poolname and Pooldimension. (see example in tests/test_data/full_exp_design.csv)\n  * Filename should contain all the unqiue input fastq filenames.\n  * Poolname should indicate to which pool a given file belongs. Multiple files per poolname are allowed.\n  * Pooldimension indicates the pooling dimension a pool belongs to. All pools sharing the same pooling dimension should have the same string in the Pooldimension column.\n  \n\nAn example of how an exp_design file could look like:\n\n| Filename          | Poolname        | Pooldimension  |\n| :---------------: | :-------------: | :------------: |\n| column1.fastq     | column1         | columns        |\n| column2.fastq     | column2         | columns        |\n| row1.fastq        | row1            | rows           |\n| row2.fastq        | row2            | rows           |\n| platerow1.fastq   | platerow1       | platerows      |\n| platerow2.fastq   | platerow2       | platerows      |\n| platecol1.fastq   | platecol1       | platecols      |\n| platecol2.fastq   | platecol2       | platecols      |\n\n* -gb path to genbank reference file\n* -br path to bowtie index files, ending with the basename of your index (if the basename of your index is UTI89 and you store your bowtie2 references in bowtie_ref it should be bowtie_ref/UTI89). Please visit https://bowtie-bio.sourceforge.net/bowtie2/manual.shtml#the-bowtie2-build-indexer for a manual how to create bowtie2 indices.\n* -t transposon sequence (e.g. AGATGTGTATAAGAGACAG)\n* -bu upstream sequence of barcode (e.g. CGAGGTCTCT)\n* -bd downstream sequence of barcode (e.g. CGTACGCTGC)\n\nOptional parameters:\n* -mq minimum bowtie2 alignment quality score for each base to include read\n* -sq minimum phred score for each base to include read\n* -tm number of transposon mismatches allowed\n* -thr threshold for local filter (e.g. a threshold of 0.05 would filter out all reads < 0.05 of the maximum read count for a given mutant)\n\n## Output\n\n`arraylib-solve` outputs 4 files: \n* count_matrix.csv: Read counts per pool for each mutant.\n* filtered_matrix.csv: Read counts per pool for each mutant, but mutants with barcodes with low read counts for a given genomic location are filtered out.\n* mutant_location_summary.csv: A summary of mutants found in the well plate grid, where each row corresponds to a different mutant.\n* well_location_summary.csv: A summary of the deconvolved well plate grid, where each row corresponds to a different well.\n\n\n\n# References\n<a id="1">[1]</a> \nBaym, M., Shaket, L., Anzai, I.A., Adesina, O. and Barstow, B., 2016. Rapid construction of a whole-genome transposon insertion collection for Shewanella oneidensis by Knockout Sudoku. Nature communications, 7(1), p.13270.\\\n<a id="2">[2]</a> \nLangmead, B. and Salzberg, S.L., 2012. Fast gapped-read alignment with Bowtie 2. Nature methods, 9(4), pp.357-359.\n\n',
     'author': 'capraz',
     'author_email': 'tuemayc@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `arraylib_solve-0.8.0/PKG-INFO` & `arraylib_solve-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraylib-solve
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tool to computationally deconvolve combinatorially pooled arrayed random mutagenesis libraries
 License: MIT
 Author: capraz
 Author-email: tuemayc@hotmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -50,15 +50,15 @@
 
 
 # How to run `arraylib-solve`
 
 To run `arraylib-solve` on a library deconvolution experiment with default parameters run:
 
 ```
-arraylib-run <input_directory> <experimental_design.csv> -c <number_of_cpu_cores_to_use> -b <path_to_genbank_reference> -br <path_to_bowtie2_indices> -t <transposon_sequence> -bu <upstream_sequence_of_barcodes> -bd <downstream_sequence_of_barcodes>
+arraylib-run <input_directory> <experimental_design.csv> -c <number_of_cpu_cores_to_use> -gb <path_to_genbank_reference> -br <path_to_bowtie2_indices> -t <transposon_sequence> -bu <upstream_sequence_of_barcodes> -bd <downstream_sequence_of_barcodes>
 ```
 
 ## Input parameters
 
 Required parameters:
 * input_dir: path to directory holding the input fastq files
 * exp_design: path to csv file indicating experimental design (values should be separated by a comma). The experimental design file
```

