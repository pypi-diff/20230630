# Comparing `tmp/splicekit-0.4.4.tar.gz` & `tmp/splicekit-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splicekit-0.4.4.tar", last modified: Mon Jun 12 17:57:04 2023, max compression
+gzip compressed data, was "splicekit-0.4.5.tar", last modified: Fri Jun 30 14:19:58 2023, max compression
```

## Comparing `splicekit-0.4.4.tar` & `splicekit-0.4.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.026227 splicekit-0.4.4/
--rw-rw-r--   0 rotg     (2023757) games       (20)    23142 2023-06-12 17:57:04.025850 splicekit-0.4.4/PKG-INFO
--rwxrwxr-x   0 rotg     (2023757) games       (20)    22744 2023-06-06 14:20:03.000000 splicekit-0.4.4/README.md
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-06-12 17:57:04.026327 splicekit-0.4.4/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)     1150 2023-06-12 17:55:56.000000 splicekit-0.4.4/setup.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.003757 splicekit-0.4.4/splicekit/
--rw-rw-r--   0 rotg     (2023757) games       (20)    13857 2023-06-08 07:08:02.000000 splicekit-0.4.4/splicekit/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.007341 splicekit-0.4.4/splicekit/clusterlogfc/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.4/splicekit/clusterlogfc/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.008686 splicekit-0.4.4/splicekit/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)      951 2023-06-07 13:26:10.000000 splicekit-0.4.4/splicekit/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.023391 splicekit-0.4.4/splicekit/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)      396 2023-01-31 12:27:24.000000 splicekit-0.4.4/splicekit/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.4/splicekit/core/anchors.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.4/splicekit/core/annotation.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.4/splicekit/core/delta_dar.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.4/splicekit/core/exons.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)    29902 2023-05-03 08:24:07.000000 splicekit-0.4.4/splicekit/core/features.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.4/splicekit/core/genes.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1059 2023-06-07 14:32:33.000000 splicekit-0.4.4/splicekit/core/jbrowse2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     9033 2023-06-08 11:52:41.000000 splicekit-0.4.4/splicekit/core/jbrowse2_create.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.4/splicekit/core/juan.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-05-02 17:27:43.000000 splicekit-0.4.4/splicekit/core/junctions.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.4/splicekit/core/motifs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.4/splicekit/core/patterns.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.4/splicekit/core/promisc.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.4/splicekit/core/report.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1527 2023-05-09 07:27:49.000000 splicekit-0.4.4/splicekit/folders.setup
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.024482 splicekit-0.4.4/splicekit/judge/
--rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-06-08 11:49:08.000000 splicekit-0.4.4/splicekit/judge/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.4/splicekit/splicecompare
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5165 2023-06-08 07:07:45.000000 splicekit-0.4.4/splicekit/splicekit
--rw-rw-r--   0 rotg     (2023757) games       (20)     1638 2023-06-06 07:56:19.000000 splicekit-0.4.4/splicekit/splicekit.config.template
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-12 17:56:05.000000 splicekit-0.4.4/splicekit/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.006803 splicekit-0.4.4/splicekit.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)    23142 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.4/splicekit.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/top_level.txt
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.838842 splicekit-0.4.5/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23915 2023-06-30 14:19:58.838444 splicekit-0.4.5/PKG-INFO
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    23517 2023-06-19 14:13:26.000000 splicekit-0.4.5/README.md
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-06-30 14:19:58.838946 splicekit-0.4.5/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1150 2023-06-12 17:55:56.000000 splicekit-0.4.5/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.828846 splicekit-0.4.5/splicekit/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    13857 2023-06-08 07:08:02.000000 splicekit-0.4.5/splicekit/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.831055 splicekit-0.4.5/splicekit/clusterlogfc/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.5/splicekit/clusterlogfc/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.831627 splicekit-0.4.5/splicekit/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      951 2023-06-07 13:26:10.000000 splicekit-0.4.5/splicekit/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.837498 splicekit-0.4.5/splicekit/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      119 2023-06-20 11:22:13.000000 splicekit-0.4.5/splicekit/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.5/splicekit/core/anchors.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.5/splicekit/core/annotation.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.5/splicekit/core/delta_dar.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.5/splicekit/core/exons.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    30130 2023-06-30 14:19:04.000000 splicekit-0.4.5/splicekit/core/features.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.5/splicekit/core/genes.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1059 2023-06-07 14:32:33.000000 splicekit-0.4.5/splicekit/core/jbrowse2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9033 2023-06-08 11:52:41.000000 splicekit-0.4.5/splicekit/core/jbrowse2_create.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.5/splicekit/core/juan.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-06-21 14:33:41.000000 splicekit-0.4.5/splicekit/core/junctions.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.5/splicekit/core/motifs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.5/splicekit/core/patterns.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.5/splicekit/core/promisc.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.5/splicekit/core/report.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1527 2023-05-09 07:27:49.000000 splicekit-0.4.5/splicekit/folders.setup
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.837940 splicekit-0.4.5/splicekit/judge/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-06-08 11:49:08.000000 splicekit-0.4.5/splicekit/judge/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.5/splicekit/splicecompare
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5117 2023-06-30 14:16:46.000000 splicekit-0.4.5/splicekit/splicekit
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1638 2023-06-06 07:56:19.000000 splicekit-0.4.5/splicekit/splicekit.config.template
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-30 14:19:54.000000 splicekit-0.4.5/splicekit/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.830692 splicekit-0.4.5/splicekit.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23915 2023-06-30 14:19:58.829232 splicekit-0.4.5/splicekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-06-30 14:19:58.829510 splicekit-0.4.5/splicekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-06-30 14:19:58.829771 splicekit-0.4.5/splicekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.5/splicekit.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-06-30 14:19:58.830357 splicekit-0.4.5/splicekit.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-06-30 14:19:58.830777 splicekit-0.4.5/splicekit.egg-info/top_level.txt
```

### Comparing `splicekit-0.4.4/PKG-INFO` & `splicekit-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.4
+Version: 0.4.5
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
 A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in BAM format (look at [datasets](datasets) for details on how to run examples).
 
 [What is splicekit?](#what_do)<br>
-[Installation and quick start](#initial_setup)<br>
+[Installation](#initial_setup)<br>
+[Quick start](#quick_start)<br>
+[Software dependencies](#software_dep)<br>
+[Example runs and datasets](#examples)<br>
 [Running splicekit](#running_splicekit)<br>
 &nbsp;&nbsp;[Annotation and comparisons](#annot_comp)<br>
 &nbsp;&nbsp;[Preparing feature (genes, exon, junction, anchor) data tables](#make_tables)<br>
 &nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#id_features)<br>
 [Motif analysis](#motif)<br>
 [Scanning for RNA-protein binding with scanRBP](#scanRBP)<br>
 [juDGE plots](#judgeplot)<br>
@@ -26,33 +29,37 @@
 [Changelog](#changelog)<br>
 
 <b>splicekit</b> is a modular platform for splicing analysis of RNA-seq datasets. The platform also integrates an JBrowse2 instance together with [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
 
 ## What is splicekit?<a name="what_do"></a>
 From an initial config file (`splicekit.config`), sample annotation (`samples.tab`) and aligned reads in BAM format, splicekit first defines comparisons (which test samples to compare to which controls). Next, feature count tables are generated (exons, anchors, junctions, genes) based on defined comparisons. Analysis incude edgeR alt-splice (differentially used features), motif analysis with DonJuAn (junction-anchor) and DREME, RNA-protein binding enrichment analysis with scanRBP and clustering analysis on expression of features. To facilitate result and data interpretation, splicekit also provides an instance of JBrowse2.
 
-## Installation and quick start<a name="initial_setup"></a>
+## Installation<a name="initial_setup"></a>
 
 The easiest way to install splicekit is to simply run:
 
 `$ pip install splicekit`
 
 Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ splicekit` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
 
 If you would like to install splicekit directly from this repository, clone the repository into a folder, for example `~/software/splicekit`. Add the `~/software/splicekit` folder to $PYTHONPATH (`export PYTHONPATH=$PYTHONPATH:~/software/splicekit`).
 
-### Software dependencies
+## Quick start<a name="quick_start"></a>
+
+If you already have aligned reads in BAM files, all you need is `samples.tab` and `splicekit.config` in one folder and the reference genome annotation downloaded and parsed (e.g. `$ pybio genome homo_sapiens`). Then run `$ splicekit process`. Check [datasets](datasets) examples to see how these files look like and also to check scripts if you need to map reads from FASTQ files with `pybio`.
+
+## Software dependencies<a name="software_dep"></a>
 
 splicekit uses several third-party open-source software. If you don't have the software installed on your system, we prepared a [singularity definition file](singularity), where you can also directly see all dependencies. Using the singularity image, you don't need to install the dependencies yourself, you just need to install singularity.
 
-### Example runs and datasets
+## Example runs and datasets<a name="examples"></a>
 
 Example runs can be found in the [datasets](datasets) folder.
 
-### Configuration file documentation
+## Configuration file documentation
 
 <details>
 <summary>Description of splicekit.config file parameters (click to show)</summary>
 
 Core parameters that need to be set for the analyses to be run:
 
 | Parameter | Description | Default / Example |
@@ -88,15 +95,15 @@
 | protein_label | short label for the used protein | "TDP43"
 
 Processing parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | platform | "desktop" or "cluster" (HPC with SLURM) | "desktop"
-| container | leave empty or for singularity use: "singularity"; this will download and run "singularity/splicekit_version.sif" | "desktop"
+| container | leave empty or "singularity run path_to/splicekit.sif"
 
 Visualization, labelling and other parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | short_names | List of triples for shortening names in results, if last string is "complete", only entire strings will be considered (no partial replacement) | [], example: [("cell_line_A", "A", "complete")], this would only replace cell_line_A with A if cell_line_A is the whole string, while if "partial" is provided, also strings like ...cell_line_A... would be replaced with ...A... | ("original name", "short name", "complete")
 
@@ -131,37 +138,38 @@
 Let's shortly describe and comment individual steps with the required inputs and resulting outputs.
 
 ### Annotation and comparisons <a name="annot_comp"></a>
 
 This first step of the analysis (`splicekit annotation`) loads samples from the file `samples.tab`. It also uses the `treatment_column` (where is the treatment stored), `control_name` (name of the controls in the treatment column), `group_column` (group experiments by this property, e.g. plate) and `separate_column` (generate comparisons inside groups, e.g. cell_type) to create comparisons. Each treatment (can have several replicates / samples / readouts) is compared to the controls.
 
 <details>
-<summary>An example `sample.tab` would look like this (click to show)</summary>
-
-An example `sample.tab` would look like this:
+<summary>An example sample.tab would look like this (click to show)</summary>
 
 | sample_id | treatment_id |
 |-|-|
-| 1 | control |
-| 2 | control |
-| 3 | control |
-| 4 | test1 |
-| 5 | test1 |
-| 6 | test1 |
-| 7 | test2 |
-| 8 | test2 |
-| 9 | test2 |
+| sample1 | control |
+| sample2 | control |
+| sample3 | control |
+| sample4 | test1 |
+| sample5 | test1 |
+| sample6 | test1 |
+| sample7 | test2 |
+| sample8 | test2 |
+| sample9 | test2 |
+
+splicekit would then expect BAM files with names `sample_id`.bam to be present (`sample1.bam`, `sample2.bam`, etc.) in the folder `bam_path` parameter specified in the `splicekit.config` file.
+
 </details>
 
-Once we have loaded and process the sample annotation, splicekit creates "comparisons", by default this will compare treated samples to control samples. The comparisons are also stored in a simple tab delimited file, `annotation/comparisons.tab`:
+Once we have loaded and process the sample annotation, splicekit creates **comparisons**, by default this will compare treated samples to control samples. The comparisons are also stored in a simple tab delimited file, `annotation/comparisons.tab`:
 
 | comparison | compound_samples | DMSO_samples |
 |-|-|-|
-| test1_control | 4_test1,5_test1,6_test1 | 1_control,2_control,3_control |
-| test2_control | 7_test2,8_test2,9_test2 | 1_control,2_control,3_control |
+| test1_control | sample4_test1,sample5_test1,sample6_test1 | sample1_control,sample2_control,sample3_control |
+| test2_control | sample7_test2,sample8_test2,sample9_test2 | sample1_control,sample2_control,sample3_control |
 
 In addition, this step will also create <b>processing shell scripts</b> and <b>cluster job files</b> (`jobs/*`). An example cluster job file:
 
 ```
 #!/bin/bash
 #BSUB -J edgeR_junctions_sample1                  # Job name
 #BSUB -n 4                                        # number of tasks
```

### Comparing `splicekit-0.4.4/README.md` & `splicekit-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # splicekit
 
 A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in BAM format (look at [datasets](datasets) for details on how to run examples).
 
 [What is splicekit?](#what_do)<br>
-[Installation and quick start](#initial_setup)<br>
+[Installation](#initial_setup)<br>
+[Quick start](#quick_start)<br>
+[Software dependencies](#software_dep)<br>
+[Example runs and datasets](#examples)<br>
 [Running splicekit](#running_splicekit)<br>
 &nbsp;&nbsp;[Annotation and comparisons](#annot_comp)<br>
 &nbsp;&nbsp;[Preparing feature (genes, exon, junction, anchor) data tables](#make_tables)<br>
 &nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#id_features)<br>
 [Motif analysis](#motif)<br>
 [Scanning for RNA-protein binding with scanRBP](#scanRBP)<br>
 [juDGE plots](#judgeplot)<br>
@@ -16,33 +19,37 @@
 [Changelog](#changelog)<br>
 
 <b>splicekit</b> is a modular platform for splicing analysis of RNA-seq datasets. The platform also integrates an JBrowse2 instance together with [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
 
 ## What is splicekit?<a name="what_do"></a>
 From an initial config file (`splicekit.config`), sample annotation (`samples.tab`) and aligned reads in BAM format, splicekit first defines comparisons (which test samples to compare to which controls). Next, feature count tables are generated (exons, anchors, junctions, genes) based on defined comparisons. Analysis incude edgeR alt-splice (differentially used features), motif analysis with DonJuAn (junction-anchor) and DREME, RNA-protein binding enrichment analysis with scanRBP and clustering analysis on expression of features. To facilitate result and data interpretation, splicekit also provides an instance of JBrowse2.
 
-## Installation and quick start<a name="initial_setup"></a>
+## Installation<a name="initial_setup"></a>
 
 The easiest way to install splicekit is to simply run:
 
 `$ pip install splicekit`
 
 Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ splicekit` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
 
 If you would like to install splicekit directly from this repository, clone the repository into a folder, for example `~/software/splicekit`. Add the `~/software/splicekit` folder to $PYTHONPATH (`export PYTHONPATH=$PYTHONPATH:~/software/splicekit`).
 
-### Software dependencies
+## Quick start<a name="quick_start"></a>
+
+If you already have aligned reads in BAM files, all you need is `samples.tab` and `splicekit.config` in one folder and the reference genome annotation downloaded and parsed (e.g. `$ pybio genome homo_sapiens`). Then run `$ splicekit process`. Check [datasets](datasets) examples to see how these files look like and also to check scripts if you need to map reads from FASTQ files with `pybio`.
+
+## Software dependencies<a name="software_dep"></a>
 
 splicekit uses several third-party open-source software. If you don't have the software installed on your system, we prepared a [singularity definition file](singularity), where you can also directly see all dependencies. Using the singularity image, you don't need to install the dependencies yourself, you just need to install singularity.
 
-### Example runs and datasets
+## Example runs and datasets<a name="examples"></a>
 
 Example runs can be found in the [datasets](datasets) folder.
 
-### Configuration file documentation
+## Configuration file documentation
 
 <details>
 <summary>Description of splicekit.config file parameters (click to show)</summary>
 
 Core parameters that need to be set for the analyses to be run:
 
 | Parameter | Description | Default / Example |
@@ -78,15 +85,15 @@
 | protein_label | short label for the used protein | "TDP43"
 
 Processing parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | platform | "desktop" or "cluster" (HPC with SLURM) | "desktop"
-| container | leave empty or for singularity use: "singularity"; this will download and run "singularity/splicekit_version.sif" | "desktop"
+| container | leave empty or "singularity run path_to/splicekit.sif"
 
 Visualization, labelling and other parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | short_names | List of triples for shortening names in results, if last string is "complete", only entire strings will be considered (no partial replacement) | [], example: [("cell_line_A", "A", "complete")], this would only replace cell_line_A with A if cell_line_A is the whole string, while if "partial" is provided, also strings like ...cell_line_A... would be replaced with ...A... | ("original name", "short name", "complete")
 
@@ -121,37 +128,38 @@
 Let's shortly describe and comment individual steps with the required inputs and resulting outputs.
 
 ### Annotation and comparisons <a name="annot_comp"></a>
 
 This first step of the analysis (`splicekit annotation`) loads samples from the file `samples.tab`. It also uses the `treatment_column` (where is the treatment stored), `control_name` (name of the controls in the treatment column), `group_column` (group experiments by this property, e.g. plate) and `separate_column` (generate comparisons inside groups, e.g. cell_type) to create comparisons. Each treatment (can have several replicates / samples / readouts) is compared to the controls.
 
 <details>
-<summary>An example `sample.tab` would look like this (click to show)</summary>
-
-An example `sample.tab` would look like this:
+<summary>An example sample.tab would look like this (click to show)</summary>
 
 | sample_id | treatment_id |
 |-|-|
-| 1 | control |
-| 2 | control |
-| 3 | control |
-| 4 | test1 |
-| 5 | test1 |
-| 6 | test1 |
-| 7 | test2 |
-| 8 | test2 |
-| 9 | test2 |
+| sample1 | control |
+| sample2 | control |
+| sample3 | control |
+| sample4 | test1 |
+| sample5 | test1 |
+| sample6 | test1 |
+| sample7 | test2 |
+| sample8 | test2 |
+| sample9 | test2 |
+
+splicekit would then expect BAM files with names `sample_id`.bam to be present (`sample1.bam`, `sample2.bam`, etc.) in the folder `bam_path` parameter specified in the `splicekit.config` file.
+
 </details>
 
-Once we have loaded and process the sample annotation, splicekit creates "comparisons", by default this will compare treated samples to control samples. The comparisons are also stored in a simple tab delimited file, `annotation/comparisons.tab`:
+Once we have loaded and process the sample annotation, splicekit creates **comparisons**, by default this will compare treated samples to control samples. The comparisons are also stored in a simple tab delimited file, `annotation/comparisons.tab`:
 
 | comparison | compound_samples | DMSO_samples |
 |-|-|-|
-| test1_control | 4_test1,5_test1,6_test1 | 1_control,2_control,3_control |
-| test2_control | 7_test2,8_test2,9_test2 | 1_control,2_control,3_control |
+| test1_control | sample4_test1,sample5_test1,sample6_test1 | sample1_control,sample2_control,sample3_control |
+| test2_control | sample7_test2,sample8_test2,sample9_test2 | sample1_control,sample2_control,sample3_control |
 
 In addition, this step will also create <b>processing shell scripts</b> and <b>cluster job files</b> (`jobs/*`). An example cluster job file:
 
 ```
 #!/bin/bash
 #BSUB -J edgeR_junctions_sample1                  # Job name
 #BSUB -n 4                                        # number of tasks
```

### Comparing `splicekit-0.4.4/setup.py` & `splicekit-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/__init__.py` & `splicekit-0.4.5/splicekit/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/clusterlogfc/__init__.py` & `splicekit-0.4.5/splicekit/clusterlogfc/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/config/__init__.py` & `splicekit-0.4.5/splicekit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/anchors.py` & `splicekit-0.4.5/splicekit/core/anchors.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/annotation.py` & `splicekit-0.4.5/splicekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/delta_dar.py` & `splicekit-0.4.5/splicekit/core/delta_dar.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/exons.py` & `splicekit-0.4.5/splicekit/core/exons.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/features.py` & `splicekit-0.4.5/splicekit/core/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,38 +62,41 @@
         exon_last_pos = pos_stop if strand=="+" else pos_start
         transcript_exons.setdefault((atts["transcript_id"], chr, strand, gene_id), []).append((exon_first_pos, exon_last_pos))
 
         annotation.genes[gene_id] = gene
         r = f.readline()
     f.close()
 
-    # save "promoters" (last nucleotide of first exon of each transcript)
-    print("[features] saving first_exons (last nucleotide of first exon of each transcript)")
+    def identify_exons(transcript_exons, annotation_data, exon_index):
+        for (transcript_id, chr, strand, gene_id), transcript_list in transcript_exons.items():
+            # sort exons by start position
+            transcript_list = sorted(transcript_list, key = lambda x: (x[0])) if strand=="+" else sorted(transcript_list, key = lambda x: (-x[0]))
+            # keep only first exons, even if there are >1 (same start position, but diff stop position)
+            transcript_list = [(x[0], x[1]) for x in transcript_list if x[0]==transcript_list[exon_index][0]]
+            for (exon_start, exon_stop) in transcript_list:
+                store_data = True
+                # store exon last pos, since we find this exon by first nucleotide of junction (last nucleotide of first exon)
+                current_data = annotation_data.get((chr, strand, exon_stop), None)
+                if current_data!=None: # already an exon stored at this "last" position
+                    current_transcript_id, current_gene_id, current_exon_start, current_exon_stop = current_data
+                    current_len = abs(current_exon_start - current_exon_stop + 1)
+                    new_len = abs(exon_start - exon_stop + 1)
+                    if new_len>current_len:
+                        store_data = False
+                if store_data:
+                    annotation_data[chr, strand, exon_stop] = (transcript_id, gene_id, exon_start, exon_stop)
+
+    # save last nucleotide of first/second exon of each transcript)
+    print("splicekit.features: saving last nucleotide of first/second exon of each transcript")
     annotation.first_exons = {}
-    for (transcript_id, chr, strand, gene_id), transcript_list in transcript_exons.items():
-        # sort exons by start position
-        transcript_list = sorted(transcript_list, key = lambda x: (x[0])) if strand=="+" else sorted(transcript_list, key = lambda x: (-x[0]))
-        # keep only first exons, even if there are >1 (same start position, but diff stop position)
-        transcript_list = [(x[0], x[1]) for x in transcript_list if x[0]==transcript_list[0][0]]
-        #if transcript_id=="NM_001330143.2":
-        #    print(transcript_list)
-        for (exon_start, exon_stop) in transcript_list:
-            store_data = True
-            # store exon last pos, since we find this exon by first nucleotide of junction (last nucleotide of first exon)
-            current_data = annotation.first_exons.get((chr, strand, exon_stop), None)
-            if current_data!=None: # already an exon stored at this "last" position
-                current_transcript_id, current_gene_id, current_exon_start, current_exon_stop = current_data
-                current_len = abs(current_exon_start - current_exon_stop + 1)
-                new_len = abs(exon_start - exon_stop + 1)
-                if new_len>current_len:
-                    store_data = False
-            if store_data:
-                annotation.first_exons[chr, strand, exon_stop] = (transcript_id, gene_id, exon_start, exon_stop)
+    identify_exons(transcript_exons, annotation.first_exons, 0)
+    #annotation.second_exons = {}
+    #identify_exons(transcript_exons, annotation.second_exons, 1)
     
-    print("[features] Reading junctions and anchors annotation: reference/junctions.tab")
+    print("splicekit.features: reading junctions and anchors annotation from: reference/junctions.tab")
     f = open("reference/junctions.tab", "rt")
     header = f.readline().replace("\r", "").replace("\n", "").split("\t")
     r = f.readline()
     while r:
         r = r.replace("\r", "").replace("\n", "").split("\t")
         data = dict(zip(header, r))
         gene_id = data["gene_id"]
```

### Comparing `splicekit-0.4.4/splicekit/core/genes.py` & `splicekit-0.4.5/splicekit/core/genes.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/jbrowse2.py` & `splicekit-0.4.5/splicekit/core/jbrowse2.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/jbrowse2_create.py` & `splicekit-0.4.5/splicekit/core/jbrowse2_create.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/juan.py` & `splicekit-0.4.5/splicekit/core/juan.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/junctions.py` & `splicekit-0.4.5/splicekit/core/junctions.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/motifs.py` & `splicekit-0.4.5/splicekit/core/motifs.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/patterns.py` & `splicekit-0.4.5/splicekit/core/patterns.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/promisc.py` & `splicekit-0.4.5/splicekit/core/promisc.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/core/report.py` & `splicekit-0.4.5/splicekit/core/report.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/folders.setup` & `splicekit-0.4.5/splicekit/folders.setup`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/judge/__init__.py` & `splicekit-0.4.5/splicekit/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/splicecompare` & `splicekit-0.4.5/splicekit/splicecompare`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit/splicekit` & `splicekit-0.4.5/splicekit/splicekit`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/apps/rocs/2020.08/cascadelake/software/Anaconda3/2021.05/bin/python
+#!/usr/bin/env python3
 
 import os
 import sys
 import argparse
 
 help_0 = """
 Usage: splicekit <command> [options]
```

### Comparing `splicekit-0.4.4/splicekit/splicekit.config.template` & `splicekit-0.4.5/splicekit/splicekit.config.template`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.4/splicekit.egg-info/PKG-INFO` & `splicekit-0.4.5/splicekit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.4
+Version: 0.4.5
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
 A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in BAM format (look at [datasets](datasets) for details on how to run examples).
 
 [What is splicekit?](#what_do)<br>
-[Installation and quick start](#initial_setup)<br>
+[Installation](#initial_setup)<br>
+[Quick start](#quick_start)<br>
+[Software dependencies](#software_dep)<br>
+[Example runs and datasets](#examples)<br>
 [Running splicekit](#running_splicekit)<br>
 &nbsp;&nbsp;[Annotation and comparisons](#annot_comp)<br>
 &nbsp;&nbsp;[Preparing feature (genes, exon, junction, anchor) data tables](#make_tables)<br>
 &nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#id_features)<br>
 [Motif analysis](#motif)<br>
 [Scanning for RNA-protein binding with scanRBP](#scanRBP)<br>
 [juDGE plots](#judgeplot)<br>
@@ -26,33 +29,37 @@
 [Changelog](#changelog)<br>
 
 <b>splicekit</b> is a modular platform for splicing analysis of RNA-seq datasets. The platform also integrates an JBrowse2 instance together with [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
 
 ## What is splicekit?<a name="what_do"></a>
 From an initial config file (`splicekit.config`), sample annotation (`samples.tab`) and aligned reads in BAM format, splicekit first defines comparisons (which test samples to compare to which controls). Next, feature count tables are generated (exons, anchors, junctions, genes) based on defined comparisons. Analysis incude edgeR alt-splice (differentially used features), motif analysis with DonJuAn (junction-anchor) and DREME, RNA-protein binding enrichment analysis with scanRBP and clustering analysis on expression of features. To facilitate result and data interpretation, splicekit also provides an instance of JBrowse2.
 
-## Installation and quick start<a name="initial_setup"></a>
+## Installation<a name="initial_setup"></a>
 
 The easiest way to install splicekit is to simply run:
 
 `$ pip install splicekit`
 
 Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ splicekit` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
 
 If you would like to install splicekit directly from this repository, clone the repository into a folder, for example `~/software/splicekit`. Add the `~/software/splicekit` folder to $PYTHONPATH (`export PYTHONPATH=$PYTHONPATH:~/software/splicekit`).
 
-### Software dependencies
+## Quick start<a name="quick_start"></a>
+
+If you already have aligned reads in BAM files, all you need is `samples.tab` and `splicekit.config` in one folder and the reference genome annotation downloaded and parsed (e.g. `$ pybio genome homo_sapiens`). Then run `$ splicekit process`. Check [datasets](datasets) examples to see how these files look like and also to check scripts if you need to map reads from FASTQ files with `pybio`.
+
+## Software dependencies<a name="software_dep"></a>
 
 splicekit uses several third-party open-source software. If you don't have the software installed on your system, we prepared a [singularity definition file](singularity), where you can also directly see all dependencies. Using the singularity image, you don't need to install the dependencies yourself, you just need to install singularity.
 
-### Example runs and datasets
+## Example runs and datasets<a name="examples"></a>
 
 Example runs can be found in the [datasets](datasets) folder.
 
-### Configuration file documentation
+## Configuration file documentation
 
 <details>
 <summary>Description of splicekit.config file parameters (click to show)</summary>
 
 Core parameters that need to be set for the analyses to be run:
 
 | Parameter | Description | Default / Example |
@@ -88,15 +95,15 @@
 | protein_label | short label for the used protein | "TDP43"
 
 Processing parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | platform | "desktop" or "cluster" (HPC with SLURM) | "desktop"
-| container | leave empty or for singularity use: "singularity"; this will download and run "singularity/splicekit_version.sif" | "desktop"
+| container | leave empty or "singularity run path_to/splicekit.sif"
 
 Visualization, labelling and other parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | short_names | List of triples for shortening names in results, if last string is "complete", only entire strings will be considered (no partial replacement) | [], example: [("cell_line_A", "A", "complete")], this would only replace cell_line_A with A if cell_line_A is the whole string, while if "partial" is provided, also strings like ...cell_line_A... would be replaced with ...A... | ("original name", "short name", "complete")
 
@@ -131,37 +138,38 @@
 Let's shortly describe and comment individual steps with the required inputs and resulting outputs.
 
 ### Annotation and comparisons <a name="annot_comp"></a>
 
 This first step of the analysis (`splicekit annotation`) loads samples from the file `samples.tab`. It also uses the `treatment_column` (where is the treatment stored), `control_name` (name of the controls in the treatment column), `group_column` (group experiments by this property, e.g. plate) and `separate_column` (generate comparisons inside groups, e.g. cell_type) to create comparisons. Each treatment (can have several replicates / samples / readouts) is compared to the controls.
 
 <details>
-<summary>An example `sample.tab` would look like this (click to show)</summary>
-
-An example `sample.tab` would look like this:
+<summary>An example sample.tab would look like this (click to show)</summary>
 
 | sample_id | treatment_id |
 |-|-|
-| 1 | control |
-| 2 | control |
-| 3 | control |
-| 4 | test1 |
-| 5 | test1 |
-| 6 | test1 |
-| 7 | test2 |
-| 8 | test2 |
-| 9 | test2 |
+| sample1 | control |
+| sample2 | control |
+| sample3 | control |
+| sample4 | test1 |
+| sample5 | test1 |
+| sample6 | test1 |
+| sample7 | test2 |
+| sample8 | test2 |
+| sample9 | test2 |
+
+splicekit would then expect BAM files with names `sample_id`.bam to be present (`sample1.bam`, `sample2.bam`, etc.) in the folder `bam_path` parameter specified in the `splicekit.config` file.
+
 </details>
 
-Once we have loaded and process the sample annotation, splicekit creates "comparisons", by default this will compare treated samples to control samples. The comparisons are also stored in a simple tab delimited file, `annotation/comparisons.tab`:
+Once we have loaded and process the sample annotation, splicekit creates **comparisons**, by default this will compare treated samples to control samples. The comparisons are also stored in a simple tab delimited file, `annotation/comparisons.tab`:
 
 | comparison | compound_samples | DMSO_samples |
 |-|-|-|
-| test1_control | 4_test1,5_test1,6_test1 | 1_control,2_control,3_control |
-| test2_control | 7_test2,8_test2,9_test2 | 1_control,2_control,3_control |
+| test1_control | sample4_test1,sample5_test1,sample6_test1 | sample1_control,sample2_control,sample3_control |
+| test2_control | sample7_test2,sample8_test2,sample9_test2 | sample1_control,sample2_control,sample3_control |
 
 In addition, this step will also create <b>processing shell scripts</b> and <b>cluster job files</b> (`jobs/*`). An example cluster job file:
 
 ```
 #!/bin/bash
 #BSUB -J edgeR_junctions_sample1                  # Job name
 #BSUB -n 4                                        # number of tasks
```

### Comparing `splicekit-0.4.4/splicekit.egg-info/SOURCES.txt` & `splicekit-0.4.5/splicekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

