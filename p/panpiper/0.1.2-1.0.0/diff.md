# Comparing `tmp/panpiper-0.1.2.tar.gz` & `tmp/panpiper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panpiper-0.1.2.tar", last modified: Fri Jun 30 16:38:04 2023, max compression
+gzip compressed data, was "panpiper-1.0.0.tar", last modified: Thu Mar 30 16:55:22 2023, max compression
```

## Comparing `panpiper-0.1.2.tar` & `panpiper-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-06-30 16:38:04.023155 panpiper-0.1.2/
--rw-r--r--   0 reneeoles   (501) staff       (20)     1509 2023-01-23 16:00:15.000000 panpiper-0.1.2/LICENSE
--rw-r--r--   0 reneeoles   (501) staff       (20)       37 2023-01-21 00:39:08.000000 panpiper-0.1.2/MANIFEST.in
--rw-r--r--   0 reneeoles   (501) staff       (20)     9324 2023-06-30 16:38:04.022924 panpiper-0.1.2/PKG-INFO
--rw-r--r--   0 reneeoles   (501) staff       (20)     8728 2023-03-30 16:43:34.000000 panpiper-0.1.2/README.md
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-06-30 16:38:04.018478 panpiper-0.1.2/panpiper/
--rw-r--r--   0 reneeoles   (501) staff       (20)      415 2023-01-23 16:01:59.000000 panpiper-0.1.2/panpiper/__init__.py
--rwxr-xr-x   0 reneeoles   (501) staff       (20)     6954 2023-06-30 16:32:19.000000 panpiper-0.1.2/panpiper/main.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     5638 2023-06-30 16:32:18.000000 panpiper-0.1.2/panpiper/test.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-06-30 16:38:04.022588 panpiper-0.1.2/panpiper/workflow/
--rw-r--r--   0 reneeoles   (501) staff       (20)     1706 2023-06-30 16:32:18.000000 panpiper-0.1.2/panpiper/workflow/assembly.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)    14718 2023-06-30 16:32:19.000000 panpiper-0.1.2/panpiper/workflow/pangenome.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)     7287 2023-06-30 16:32:18.000000 panpiper-0.1.2/panpiper/workflow/pyseer.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)     5999 2023-06-30 16:32:19.000000 panpiper-0.1.2/panpiper/workflow/quality.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)     3265 2023-06-30 16:32:19.000000 panpiper-0.1.2/panpiper/workflow.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-06-30 16:38:04.021170 panpiper-0.1.2/panpiper.egg-info/
--rw-r--r--   0 reneeoles   (501) staff       (20)     9324 2023-06-30 16:38:04.000000 panpiper-0.1.2/panpiper.egg-info/PKG-INFO
--rw-r--r--   0 reneeoles   (501) staff       (20)      461 2023-06-30 16:38:04.000000 panpiper-0.1.2/panpiper.egg-info/SOURCES.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)        1 2023-06-30 16:38:04.000000 panpiper-0.1.2/panpiper.egg-info/dependency_links.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)       47 2023-06-30 16:38:04.000000 panpiper-0.1.2/panpiper.egg-info/entry_points.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)        1 2023-06-30 16:38:03.000000 panpiper-0.1.2/panpiper.egg-info/not-zip-safe
--rw-r--r--   0 reneeoles   (501) staff       (20)       11 2023-06-30 16:38:04.000000 panpiper-0.1.2/panpiper.egg-info/requires.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)        9 2023-06-30 16:38:04.000000 panpiper-0.1.2/panpiper.egg-info/top_level.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)       38 2023-06-30 16:38:04.023201 panpiper-0.1.2/setup.cfg
--rw-r--r--   0 reneeoles   (501) staff       (20)     1419 2023-06-30 16:37:47.000000 panpiper-0.1.2/setup.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.691640 panpiper-1.0.0/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1509 2023-01-23 16:00:15.000000 panpiper-1.0.0/LICENSE
+-rw-r--r--   0 reneeoles   (501) staff       (20)       37 2023-01-21 00:39:08.000000 panpiper-1.0.0/MANIFEST.in
+-rw-r--r--   0 reneeoles   (501) staff       (20)     9324 2023-03-30 16:55:22.691265 panpiper-1.0.0/PKG-INFO
+-rw-r--r--   0 reneeoles   (501) staff       (20)     8728 2023-03-30 16:43:34.000000 panpiper-1.0.0/README.md
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.683112 panpiper-1.0.0/panpiper/
+-rw-r--r--   0 reneeoles   (501) staff       (20)      415 2023-01-23 16:01:59.000000 panpiper-1.0.0/panpiper/__init__.py
+-rwxr-xr-x   0 reneeoles   (501) staff       (20)     6888 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/main.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     5638 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/test.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.686933 panpiper-1.0.0/panpiper/tests/
+-rw-r--r--   0 reneeoles   (501) staff       (20)        0 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/__init__.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.687348 panpiper-1.0.0/panpiper/tests/test_data/
+-rw-r--r--   0 reneeoles   (501) staff       (20)        0 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/test_data/__init__.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     3918 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/tests/test_main.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.689027 panpiper-1.0.0/panpiper/tests/test_scripts/
+-rw-r--r--   0 reneeoles   (501) staff       (20)      361 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/test_scripts/__init__.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)    14686 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/test_scripts/filter_isolates.py
+-rwxr-xr-x   0 reneeoles   (501) staff       (20)     1493 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/test_scripts/test_concat_amrfinder.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.690783 panpiper-1.0.0/panpiper/workflow/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1706 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow/assembly.smk
+-rw-r--r--   0 reneeoles   (501) staff       (20)    14894 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow/pangenome.smk
+-rw-r--r--   0 reneeoles   (501) staff       (20)     7287 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow/pyseer.smk
+-rw-r--r--   0 reneeoles   (501) staff       (20)     5565 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow/quality.smk
+-rw-r--r--   0 reneeoles   (501) staff       (20)     3234 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.686066 panpiper-1.0.0/panpiper.egg-info/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     9324 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/PKG-INFO
+-rw-r--r--   0 reneeoles   (501) staff       (20)      693 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/SOURCES.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)        1 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/dependency_links.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)       47 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/entry_points.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)        1 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/not-zip-safe
+-rw-r--r--   0 reneeoles   (501) staff       (20)       11 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/requires.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)        9 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/top_level.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)       38 2023-03-30 16:55:22.691691 panpiper-1.0.0/setup.cfg
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1419 2023-03-30 16:54:51.000000 panpiper-1.0.0/setup.py
```

### Comparing `panpiper-0.1.2/LICENSE` & `panpiper-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panpiper-0.1.2/PKG-INFO` & `panpiper-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panpiper
-Version: 0.1.2
+Version: 1.0.0
 Summary: Panpiper: snakemake workflow for bacterial isolate analysis
 Home-page: https://github.com/rolesucsd/Panpiper
 Author: Renee Oles
 Author-email: roles@health.ucsd.edu
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panpiper-0.1.2/README.md` & `panpiper-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `panpiper-0.1.2/panpiper/main.py` & `panpiper-1.0.0/panpiper/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,19 +84,19 @@
     app = ap.add_argument_group('parameters')
     app.add_argument(
         '--ani_cutoff', help='Average percent identity to reference cutoff', default=95, type=float)
     app.add_argument('--contig_number',
                      help='Max number of contigs', default=1000, type=int)
     app.add_argument('--n50', help='N50 cutoff', default=5000, type=int)
     app.add_argument('--eggnog_dir', help='Path to the eggnog database directory',
-                     default="/panfs/roles/Panpiper/panpiper/databases/eggnog", type=str)
+                     default="panpiper/databases/eggnog", type=str)
     app.add_argument('--kraken_dir', help='Path to the kraken2 database directory',
-                     default="/panfs/roles/Panpiper/panpiper/databases/kraken", type=str)
+                     default="panpiper/databases/kraken", type=str)
     app.add_argument('--bakta_dir', help='Path to the bakta database directory',
-                     default="/panfs/roles/Panpiper/panpiper/databases/bakta", type=str)
+                     default="panpiper/databases/bakta", type=str)
     app.add_argument(
         '--pheno_column', help='The column in the phenotype file to use for the association study', type=str)
     app.add_argument(
         '--max_jobs', help='Maximum number of cluster jobs [%(default)s]', default=40, type=int)
 
     ########## Workflow ##########
     master = Test(ap)
```

### Comparing `panpiper-0.1.2/panpiper/test.py` & `panpiper-1.0.0/panpiper/test.py`

 * *Files identical despite different names*

### Comparing `panpiper-0.1.2/panpiper/workflow/assembly.smk` & `panpiper-1.0.0/panpiper/workflow/assembly.smk`

 * *Files identical despite different names*

### Comparing `panpiper-0.1.2/panpiper/workflow/pangenome.smk` & `panpiper-1.0.0/panpiper/workflow/pangenome.smk`

 * *Files 10% similar despite different names*

```diff
@@ -3,47 +3,46 @@
 Date Updated: 1/4/2022
 Purpose: Construct pangenome
 """
 import os
 import subprocess
 import math
 import distutils.util
-from scripts.wrangle_output import genes_long, gene_matrix_phylogroup, gene_matrix, process_data
-from scripts.phylogroup_cluster import cluster_samples
 
 
 OUT = config['out']
 FASTA = config['fasta']
 SAMPLE_LIST = config['list']
 PARAMS = config['params']
 
 with open(PARAMS, 'r') as fh:   
     fl = [x.strip().split() for x in fh.readlines()]
 param_dict = {x[0]: x[1] for x in fl}
 
 BAKTA = param_dict["bakta_dir"]
 REF = param_dict["ref"]
 EGGNOG = param_dict['eggnog_dir']
+KRAKEN = param_dict["kraken_dir"]
 
 def read_filtered_files():
     with open(SAMPLE_LIST) as f:
         raw_reads = [sample for sample in f.read().split('\n') if len(sample) > 0]
         return(raw_reads)
 filtered = read_filtered_files()
 
 # Output
 rule all:
     input:
         os.path.join(OUT,"Pangenome/Summary/amr.png"),
         os.path.join(OUT,"Pangenome/Panaroo/pan_genome_reference.bwt"),
+        os.path.join(OUT,"Pangenome/Summary/db_clusters.csv"),
         os.path.join(OUT,"Pangenome/Summary/core_gene_alignment.aln.iqtree"),
+        os.path.join(OUT,"Pangenome/Summary/Summary.emapper.annotations"),
+#        os.path.join(OUT,"Pangenome/Summary/kraken_ag.txt"),
         os.path.join(OUT,"Pangenome/Unitig/unitig.pyseer"),
-        os.path.join(OUT,"Pangenome/Summary/genes_phylogroup_matrix_perc.txt"),
-        os.path.join(OUT,"Pangenome/Summary/genes_anno.txt"),
-        os.path.join(OUT,"Pangenome/Summary/genes_matrix.txt"),
 
 # Download databases
 rule bakta:
     input:
         BAKTA,
     conda:
         "envs/bakta.yml",
@@ -66,14 +65,28 @@
     benchmark:
         os.path.join(OUT,"benchmark/eggnog_db.benchmark"),
     output:
         os.path.join(EGGNOG, "eggnog.db"),
     shell:
         "download_eggnog_data.py --data_dir {input}"
 
+rule kraken_db:
+    input:
+        KRAKEN,
+    conda:
+        "envs/kraken.yml",
+    log:
+        os.path.join(OUT,"report/kraken_db.log"),
+    benchmark:
+        os.path.join(OUT,"benchmark/kraken_db.benchmark"),
+    output:
+        os.path.join(KRAKEN, "taxo.k2d"),
+    shell:
+        "kraken2-build --standard -db {input}"
+
 # Set up files for downstream analysis
 rule setup:
     input:
         expand(os.path.join(FASTA, "{file}/{file}.fna"), file=filtered),
     params:
         os.path.join(OUT,"Pangenome")
     conda:
@@ -129,15 +142,14 @@
     log:
         os.path.join(OUT,"report/panaroo.log"),
     benchmark:
         os.path.join(OUT,"benchmark/panaroo.benchmark"),
     output:
         os.path.join(OUT,"Pangenome/Panaroo/pan_genome_reference.fa"),
         os.path.join(OUT,"Pangenome/Panaroo/core_gene_alignment.aln"),
-        os.path.join(OUT,"Pangenome/Panaroo/gene_presence_absence_roary.csv"),
     shell:
         "panaroo -i {input} -o {params} --remove-invalid-genes --clean-mode strict -a core --core_threshold 0.98 --len_dif_percent 0.98 -f 0.7 --merge_paralogs -t 20 &> {log}"
 
 # Translate DNA to AA
 rule translate:
     input:
         os.path.join(OUT,"Pangenome/Panaroo/pan_genome_reference.fa"),
@@ -186,16 +198,14 @@
     shell:
         """
         bwa index -a bwtsw {input} {params.one} &> {log}
         mv {params.inte} {output}
         """
 
 # Create a starting tree based off core genome alignment
-# gtr nt = a tree for a nucleotide alignment with GTR+CAT model 
-# gamma = 5% slower but rescales teh branch lengthsa nd computes a Gamma20-based likelihood which is more comparable across runs 
 rule fasttree:
     input:
         os.path.join(OUT,"Pangenome/Panaroo/core_gene_alignment.aln"),
     conda:
         "envs/fasttree.yml"
     log:
         os.path.join(OUT,"report/fasttree.log"),
@@ -204,15 +214,14 @@
     output:
         os.path.join(OUT,"Pangenome/Phylogeny/fasttree.nwk"),
     shell:
         "FastTree -gtr -nt -gamma -seed 12345 {input} > {output}"
 
 
 # Build more accurate tree using fasttree as a starting point
-# This step infers topology 
 rule raxml:
     input:
         tre=os.path.join(OUT,"Pangenome/Phylogeny/fasttree.nwk"),
         aln=os.path.join(OUT,"Pangenome/Panaroo/core_gene_alignment.aln"),
     params:
         outdir=os.path.join(OUT,"Pangenome/Phylogeny"),
     conda:
@@ -226,15 +235,14 @@
     shell:
         "raxmlHPC-AVX2 -m GTRCAT -F -f D -s {input.aln} -t {input.tre} -p 12345 -n tree2 -w {params.outdir} &> {log}"
 
 
 # Continue to build tree from RAXML with iqtree
 # all means combined tree search and bootstrapping analysis
 # GTR indicates the sequence is DNA data
-# This step optimizes branch lengths and computes likelihood score 
 rule iqtree:
     input:
         aln=os.path.join(OUT,"Pangenome/Panaroo/core_gene_alignment.aln"),
         tre=os.path.join(OUT,"Pangenome/Phylogeny/RAxML_result.tree2"),
     params:
         output=os.path.join(OUT,"Pangenome/Panaroo/core_gene_alignment.aln.iqtree"),
     conda:
@@ -305,119 +313,153 @@
         mem="1G"
     threads: 1
     output:
         os.path.join(OUT,"Pangenome/Summary/amr.png"),
     shell:
         "Rscript panpiper/workflow/scripts/AMR_heatmap.R {input} {params} &> {log}"
 
-rule eggnog_mapper:
+
+# Work on phylogroup division using Poppunk
+rule poppunk_sketch:
     input:
-        protein=os.path.join(OUT,"Pangenome/Panaroo/pan_genome_reference.faa"),
-        db=os.path.join(EGGNOG, "eggnog.db"),
-        fna=os.path.join(OUT,"Pangenome/Summary/pan_genome_reference.tsv"),
+        os.path.join(OUT,"Pangenome/Phylogroups/poppunk.list"),
     params:
-        outdir=os.path.join(OUT,"Pangenome/Summary/Summary"),
-        db=EGGNOG,
+        os.path.join(OUT,"Pangenome/Phylogroups/db"),
     conda:
-        "envs/eggnog.yml"
+        "envs/poppunk.yml"
     log:
-        os.path.join(OUT,"report/eggnog_mapper.log"),
+        os.path.join(OUT,"report/poppunk_sketch.log"),
     benchmark:
-        os.path.join(OUT,"benchmark/eggnog_mapper.benchmark"),
+        os.path.join(OUT,"benchmark/poppunk_sketch.benchmark"),
+    resources:
+        mem="5G"
     output:
-        os.path.join(OUT,"Pangenome/Summary/Summary.emapper.annotations"),
+        os.path.join(OUT,"Pangenome/Phylogroups/db/db.dists.pkl"),
     shell:
-        """
-        emapper.py -i {input.protein} --data_dir {params.db} -o {params.outdir} --override &> {log}
-        """
+        "poppunk --create-db --output {params} --r-files {input} --threads 20 &> {log}"
 
-# Unitig caller will create unitigs which is a kmer alternative (read about why using it in gwas is better or worse)
-# In future note that you can use fastq or fasta or both see commented out line of code for other use
-# Time: 25 minutes for 571 files 
-rule unitig:
+
+rule poppunk_qc:
     input:
-        os.path.join(OUT,"Pangenome/Unitig/unitig.list"),
+        os.path.join(OUT,"Pangenome/Phylogroups/db/db.dists.pkl"),
     params:
-        os.path.join(OUT,"Pangenome/Unitig/unitig"),
+        db=os.path.join(OUT,"Pangenome/Phylogroups/db"),
+        ref=REF,
     conda:
-        "envs/unitig.yml"
+        "envs/poppunk.yml"
     log:
-        os.path.join(OUT,"report/unitig.log"),
+        os.path.join(OUT,"report/poppunk_qc.log"),
     benchmark:
-        os.path.join(OUT,"benchmark/unitig.benchmark"),
+        os.path.join(OUT,"benchmark/poppunk_qc.benchmark"),
+    resources:
+        mem="5G"
     output:
-        os.path.join(OUT,"Pangenome/Unitig/unitig.pyseer"),
+        os.path.join(OUT,"Pangenome/Phylogroups/db/poppunk.txt"),
     shell:
-        "unitig-caller --call --reads {input} --out {params} &> {log}" 
+        "poppunk --qc-db --ref-db {params.db} --type-isolate {params.ref} &> {log}"
+
 
-rule mash_fasta:
+rule poppunk_fit:
     input:
-        expand(os.path.join(FASTA, "{file}/{file}.fna"), file=filtered),
+        os.path.join(OUT,"Pangenome/Phylogroups/db/db.dists.pkl"),
     params:
-        os.path.join(OUT,"Pangenome/Mash/fasta"),
+        db=os.path.join(OUT,"Pangenome/Phylogroups/db"),
+        out=os.path.join(OUT,"Pangenome/Phylogroups/db/db_clusters.csv"),
+        model="lineage",
     conda:
-        "envs/mash.yml"
+        "envs/poppunk.yml"
+    log:
+        os.path.join(OUT,"report/poppunk_fit.log"),
+    benchmark:
+        os.path.join(OUT,"benchmark/poppunk_fit.benchmark"),
     output:
-        os.path.join(OUT,"Pangenome/Mash/fasta.tsv"),
+        os.path.join(OUT,"Pangenome/Summary/db_clusters.csv"),
     shell:
         """
-        mash sketch -s 10000 -o {params} {input}
-        mash dist {params}.msh {params}.msh -t > {output}
+        poppunk --fit-model {params.model} --ref-db {params.db} --K 4 &> {log}
+        cp {params.out} {output}
         """
 
-# Add rule to interpret mash output
-rule phylogroups:
+rule eggnog_mapper:
     input:
-        os.path.join(OUT,"Pangenome/Mash/fasta.tsv"),
+        protein=os.path.join(OUT,"Pangenome/Panaroo/pan_genome_reference.faa"),
+        db=os.path.join(EGGNOG, "eggnog.db"),
+        fna=os.path.join(OUT,"Pangenome/Summary/pan_genome_reference.tsv"),
     params:
-        os.path.join(OUT,"Pangenome/Mash/"),
+        outdir=os.path.join(OUT,"Pangenome/Summary/Summary"),
+        db=EGGNOG,
+    conda:
+        "envs/eggnog.yml"
+    log:
+        os.path.join(OUT,"report/eggnog_mapper.log"),
+    benchmark:
+        os.path.join(OUT,"benchmark/eggnog_mapper.benchmark"),
     output:
-        os.path.join(OUT,"Pangenome/Mash/phylogroups.txt"),
-    run:
-        cluster_samples(mash_file=os.path.join(OUT,"Pangenome/Mash/fasta.tsv"), output_folder=os.path.join(OUT,"Pangenome/Mash/"))
-
+        os.path.join(OUT,"Pangenome/Summary/Summary.emapper.annotations"),
+    shell:
+        """
+        emapper.py -i {input.protein} --data_dir {params.db} -o {params.outdir} --override &> {log}
+        """
 
-# Add rule to wrangle panaroo output 
-rule process_data:
+rule kraken:
     input:
-        eggnog=os.path.join(OUT,"Pangenome/Summary/Summary.emapper.annotations"),
-        bakta=os.path.join(OUT,"Pangenome/Summary/pan_genome_reference.tsv"),
+        file=os.path.join(FASTA, "{file}/{file}.fna"),
+        db=os.path.join(KRAKEN, "taxo.k2d"),
     params:
-        output=os.path.join(OUT,"Pangenome/Summary/"),
-        genes=os.path.join(OUT,"Pangenome/Panaroo/gene_presence_absence_roary.csv"),
+        db=KRAKEN,
+    conda:
+        "envs/kraken.yml"
+    log:
+        os.path.join(OUT,"report/kraken_{file}.log"),
+    benchmark:
+        os.path.join(OUT,"benchmark/kraken_{file}.benchmark"),
     output:
-        os.path.join(OUT,"Pangenome/Summary/genes_anno.txt"),
-    run:
-        process_data(bakta=os.path.join(OUT,"Pangenome/Summary/pan_genome_reference.tsv"), genes=os.path.join(OUT,"Pangenome/Panaroo/gene_presence_absence_roary.csv"), eggnog=os.path.join(OUT,"Pangenome/Summary/Summary.emapper.annotations"), output=os.path.join(OUT,"Pangenome/Summary/"))
+        out=os.path.join(OUT,"Pangenome/Kraken/{file}.out"),
+        report=os.path.join(OUT,"Pangenome/Kraken/{file}.report")
+    shell:
+        """
+        kraken2 --db {params.db} --output {output.out} --threads 20 --use-names --report {output.report} --use-mpa-style {input.file} &> {log}
+        """
 
-rule genes_long:
+rule kraken_reformat:
     input:
-        clusters=os.path.join(OUT,"Pangenome/Mash/phylogroups.txt"),
+        out=os.path.join(OUT,"Pangenome/Kraken/{file}.out"),
     params:
-        genes=os.path.join(OUT,"Pangenome/Panaroo/gene_presence_absence_roary.csv"),
-        output=os.path.join(OUT,"Pangenome/Summary/"),
+        sample="{file}",
+        outpath=os.path.join(OUT,"Pangenome/Kraken"),
+    log:
+        os.path.join(OUT,"report/kraken_reformat_{file}.log"),
+    benchmark:
+        os.path.join(OUT,"benchmark/kraken_reformat_{file}.benchmark"),
     output:
-        os.path.join(OUT,"Pangenome/Summary/genes_long.txt"),
-    run:
-        genes_long(clusters=os.path.join(OUT,"Pangenome/Mash/phylogroups.txt"), genes=os.path.join(OUT,"Pangenome/Panaroo/gene_presence_absence_roary.csv"), output=os.path.join(OUT,"Pangenome/Summary/"))
-
+        report=os.path.join(OUT,"Pangenome/Kraken/{file}_reformat.txt"),
+    shell:
+        "python panpiper/workflow/scripts/kraken_reformat.py {params.sample} {params.outpath} &> {log}"
 
-rule gene_matrix_phylogroup:
+rule kraken_ag:
     input:
-        genes_long=os.path.join(OUT,"Pangenome/Summary/genes_long.txt"),
-    params:
-        output=os.path.join(OUT,"Pangenome/Summary/"),
+        report=expand(os.path.join(OUT,"Pangenome/Kraken/{file}_reformat.txt"), file=filtered),
     output:
-        os.path.join(OUT,"Pangenome/Summary/genes_phylogroup_matrix_perc.txt"),
-    run:
-        gene_matrix_phylogroup(genes_long=os.path.join(OUT,"Pangenome/Summary/genes_long.txt"), output=os.path.join(OUT,"Pangenome/Summary/"))
+        os.path.join(OUT,"Pangenome/Summary/kraken_ag.txt"),
+    shell:
+        "awk FNR!=1 {input} > {output}"
+
 
-rule gene_matrix:
+# Unitig caller will create unitigs which is a kmer alternative (read about why using it in gwas is better or worse)
+# In future note that you can use fastq or fasta or both see commented out line of code for other use
+# Time: 25 minutes for 571 files 
+rule unitig:
     input:
-        genes=os.path.join(OUT,"Pangenome/Panaroo/gene_presence_absence_roary.csv"),
+        os.path.join(OUT,"Pangenome/Unitig/unitig.list"),
     params:
-        output=os.path.join(OUT,"Pangenome/Summary/"),
+        os.path.join(OUT,"Pangenome/Unitig/unitig"),
+    conda:
+        "envs/unitig.yml"
+    log:
+        os.path.join(OUT,"report/unitig.log"),
+    benchmark:
+        os.path.join(OUT,"benchmark/unitig.benchmark"),
     output:
-        os.path.join(OUT,"Pangenome/Summary/genes_matrix.txt"),
-    run:
-        gene_matrix(genes=os.path.join(OUT,"Pangenome/Panaroo/gene_presence_absence_roary.csv"), output=os.path.join(OUT,"Pangenome/Summary/"))
+        os.path.join(OUT,"Pangenome/Unitig/unitig.pyseer"),
+    shell:
+        "unitig-caller --call --reads {input} --out {params} &> {log}"
```

### Comparing `panpiper-0.1.2/panpiper/workflow/pyseer.smk` & `panpiper-1.0.0/panpiper/workflow/pyseer.smk`

 * *Files identical despite different names*

### Comparing `panpiper-0.1.2/panpiper/workflow/quality.smk` & `panpiper-1.0.0/panpiper/workflow/quality.smk`

 * *Files 6% similar despite different names*

```diff
@@ -37,107 +37,91 @@
         SAMPLES_OUT,
 
 
 # Remove contigs smaller than 500 bp
 # 30 sec per file
 rule contig_filter:
     input:
-        assembly=os.path.join(OUT,"Assembly/{file}/contigs.fa"),
+        assembly=os.path.join(FASTA,"{file}/contigs.fa"),
     params:
         contig=500,
     conda:
         "envs/bbmap.yml"
     log:
         os.path.join(OUT,"report/prokka_filter_{file}.log"),
     resources:
         mem="1G"
     threads: 1
     benchmark:
         os.path.join(OUT,"benchmark/prokka_filter_{file}.benchmark"),    
     output:
-        fna=os.path.join(OUT,"Assembly/{file}/{file}.fna"),
+        fna=os.path.join(OUT,"Quality/Assembly_filter/{file}/{file}.fna"),
     shell:
         "reformat.sh in={input.assembly} out={output} minlength={params.contig} &> {log}"
 
 
 # 5 minutes per sample
 rule run_checkm:
     input:
-        file=os.path.join(OUT,"Assembly/{file}/{file}.fna"),
+        file=os.path.join(OUT,"Quality/Assembly_filter/{file}/{file}.fna"),
     params:
-        binset=os.path.join(OUT,"Assembly/{file}"),
+        binset=os.path.join(OUT,"Quality/Assembly_filter/{file}"),
     conda:
         "envs/checkm.yml"
     log:
-        log=os.path.join(OUT,"Assembly/{file}/lineage.log"),
+        log=os.path.join(OUT,"Quality/Assembly_filter/{file}/lineage.log"),
     benchmark:
         os.path.join(OUT,"benchmark/checkm_{file}.benchmark"),
     output:
-        stats=os.path.join(OUT,"Assembly/{file}/storage/bin_stats.analyze.tsv"),
+        stats=os.path.join(OUT,"Quality/Assembly_filter/{file}/storage/bin_stats.analyze.tsv"),
     shell:
         """
         checkm lineage_wf -t 20 -x fna {params.binset} {params.binset} &> {log}
         """
 
 
 rule checkm_to_graph:
     input:
-        stats=expand(os.path.join(OUT,"Assembly/{file}/storage/bin_stats.analyze.tsv"), file=READS),
+        stats=expand(os.path.join(OUT,"Quality/Assembly_filter/{file}/storage/bin_stats.analyze.tsv"), file=READS),
     params:
-        log=expand(os.path.join(OUT,"Assembly/{file}/lineage.log"), file=READS),
-        outpref=OUT,
+        log=expand(os.path.join(OUT,"Quality/Assembly_filter/{file}/lineage.log"), file=READS),
+    conda:
+        "envs/r.yml"
     log:
-        os.path.join(OUT,"report/checkm_stats.log"),
+        os.path.join(OUT,"report/checkm_graph.log"),
     benchmark:
         os.path.join(OUT,"benchmark/checkm_graph.benchmark"),
     resources:
         mem="1G"
     threads: 1        
     output:
+        png=os.path.join(OUT,"Quality/CheckM/checkm_log.txt"),
         stats=os.path.join(OUT,"Quality/CheckM/checkm_stats.txt"),
     shell:
         """
-        python /panfs/roles/Panpiper/panpiper/workflow/scripts/checkm_bin-stats.py {input.stats} {params.outpref} &> {log}
+        Rscript panpiper/workflow/scripts/checkm-log.R {params.log}  &> {log}
+        Rscript panpiper/workflow/scripts/checkm_bin-stats.R {input.stats}  &> {log}
         """
 
-rule checkm_to_graph2:
-    input:
-        stats=expand(os.path.join(OUT,"Assembly/{file}/storage/bin_stats.analyze.tsv"), file=READS),
-    params:
-        log=expand(os.path.join(OUT,"Assembly/{file}/lineage.log"), file=READS),
-        outpref=OUT,
-    log:
-        os.path.join(OUT,"report/checkm_log.log"),
-    benchmark:
-        os.path.join(OUT,"benchmark/checkm_graph.benchmark"),
-    resources:
-        mem="1G"
-    threads: 1        
-    output:
-        png=os.path.join(OUT,"Quality/CheckM/checkm_log.txt"),
-    shell:
-        """
-        python /panfs/roles/Panpiper/panpiper/workflow/scripts/checkm-log.py {params.log} {params.outpref} &> {log}
-        """
 
 rule fastani:
     input:
         ref=REFERENCE,
-        file=os.path.join(OUT,"Assembly/{file}/{file}.fna"),
+        file=os.path.join(OUT,"Quality/Assembly_filter/{file}/{file}.fna"),
     conda:
         "envs/fastani.yml"
     log:
         os.path.join(OUT,"report/fastani_{file}.log"),
     resources:
         mem="1G"
     threads: 1
     benchmark:
         os.path.join(OUT,"benchmark/fastani_{file}.benchmark"),    
     output:
-        os.path.join(OUT,"Quality/FastANI/{file}.txt"),
+        temp(os.path.join(OUT,"Quality/FastANI/{file}.txt")),
     shell:
         "fastANI -q {input.file} -r {input.ref} -o {output} &> {log}"
 
 
 rule fastani_concat:
     input:
         expand(os.path.join(OUT,"Quality/FastANI/{file}.txt"), file=READS),
```

### Comparing `panpiper-0.1.2/panpiper/workflow.py` & `panpiper-1.0.0/panpiper/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         """
         # Define core snakemake command
         # need to edit j
         cmd = ['snakemake',
                '--use-conda',
                '--latency-wait', '20',
                '--rerun-incomplete',
-               '--keep-going',
                '--jobs',str(self.max_jobs),
                '-s', snakefile,
                '--config',
                'out='+self.output,
                'fastq='+self.fastq,
                'fasta='+self.fasta,
                'list='+self.sample_list,
```

### Comparing `panpiper-0.1.2/panpiper.egg-info/PKG-INFO` & `panpiper-1.0.0/panpiper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panpiper
-Version: 0.1.2
+Version: 1.0.0
 Summary: Panpiper: snakemake workflow for bacterial isolate analysis
 Home-page: https://github.com/rolesucsd/Panpiper
 Author: Renee Oles
 Author-email: roles@health.ucsd.edu
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panpiper-0.1.2/setup.py` & `panpiper-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="panpiper", 
-    version="0.1.2",
+    version="1.0.0",
     license='BSD-3-Clause',
     author="Renee Oles",
     author_email="roles@health.ucsd.edu",
     description="Panpiper: snakemake workflow for bacterial isolate analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rolesucsd/Panpiper",
```

