# Comparing `tmp/trimnami-0.0.1.tar.gz` & `tmp/trimnami-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimnami-0.0.1.tar", last modified: Thu Jun 29 06:36:58 2023, max compression
+gzip compressed data, was "trimnami-0.0.2.tar", last modified: Fri Jun 30 07:19:55 2023, max compression
```

## Comparing `trimnami-0.0.1.tar` & `trimnami-0.0.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.725986 trimnami-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-29 06:36:42.000000 trimnami-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-29 06:36:58.725986 trimnami-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-29 06:36:42.000000 trimnami-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 06:36:58.725986 trimnami-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-29 06:36:42.000000 trimnami-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.701985 trimnami-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-29 06:36:42.000000 trimnami-0.0.1/tests/test_skipHostRm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-29 06:36:42.000000 trimnami-0.0.1/tests/test_trimnami.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.705985 trimnami-0.0.1/trimnami/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.705985 trimnami-0.0.1/trimnami/config/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/config/system_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.705985 trimnami-0.0.1/trimnami/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/scripts/skipHostRm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.713986 trimnami-0.0.1/trimnami/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.717985 trimnami-0.0.1/trimnami/test_data/nanopore/
--rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/test_data/nanopore/SRR7947171.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/test_data/nanopore/SRR7947176.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/test_data/ref.fna
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/trimnami.CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/trimnami.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/trimnami.VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.717985 trimnami-0.0.1/trimnami/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.721985 trimnami-0.0.1/trimnami/workflow/databases/
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/databases/nebnext_adapters.fa
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/databases/primerB.fa
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/databases/rc_primerB_ad6.fa
--rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/databases/vector_contaminants.fa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.721985 trimnami-0.0.1/trimnami/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/envs/bbmap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/envs/fastp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/envs/filtlong.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/envs/minimap2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/envs/pigz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/envs/prinseq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/envs/rasusa.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.725986 trimnami-0.0.1/trimnami/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/rules/fastp.smk
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/rules/hostRemoval.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/rules/nanopore.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/rules/preflight.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/rules/prinseq.smk
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/rules/reports.smk
--rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-06-29 06:36:42.000000 trimnami-0.0.1/trimnami/workflow/rules/roundAB.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:58.705985 trimnami-0.0.1/trimnami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-29 06:36:58.000000 trimnami-0.0.1/trimnami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-29 06:36:58.000000 trimnami-0.0.1/trimnami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:36:58.000000 trimnami-0.0.1/trimnami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 06:36:58.000000 trimnami-0.0.1/trimnami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 06:36:58.000000 trimnami-0.0.1/trimnami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 06:36:58.000000 trimnami-0.0.1/trimnami.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.602539 trimnami-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-30 07:19:46.000000 trimnami-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-30 07:19:55.602539 trimnami-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-30 07:19:46.000000 trimnami-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 07:19:55.602539 trimnami-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-30 07:19:46.000000 trimnami-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.586539 trimnami-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 07:19:46.000000 trimnami-0.0.2/tests/test_skipHostRm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-30 07:19:46.000000 trimnami-0.0.2/tests/test_trimnami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.586539 trimnami-0.0.2/trimnami/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.590539 trimnami-0.0.2/trimnami/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/config/system_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.590539 trimnami-0.0.2/trimnami/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/scripts/skipHostRm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.594539 trimnami-0.0.2/trimnami/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.598539 trimnami-0.0.2/trimnami/test_data/nanopore/
+-rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/nanopore/SRR7947171.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/nanopore/SRR7947176.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/ref.fna
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/trimnami.CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/trimnami.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/trimnami.VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.598539 trimnami-0.0.2/trimnami/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.598539 trimnami-0.0.2/trimnami/workflow/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/databases/nebnext_adapters.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/databases/primerB.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/databases/rc_primerB_ad6.fa
+-rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/databases/vector_contaminants.fa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.598539 trimnami-0.0.2/trimnami/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/bbmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/fastp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/filtlong.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/minimap2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/pigz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/prinseq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/rasusa.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.602539 trimnami-0.0.2/trimnami/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/fastp.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/hostRemoval.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/nanopore.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/notrim.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/preflight.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/prinseq.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/reports.smk
+-rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/roundAB.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.590539 trimnami-0.0.2/trimnami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/top_level.txt
```

### Comparing `trimnami-0.0.1/PKG-INFO` & `trimnami-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimnami
-Version: 0.0.1
+Version: 0.0.2
 Summary: Trim lots of metagenomics samples all at once.
 Home-page: https://github.com/beardymcjohnface/Trimnami
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -34,16 +34,23 @@
 - Prinseq++
 - BBtools for Round A/B viral metagenomics
 - Filtlong + Rasusa for longreads
 
 ## Install
 
 Trimnami is still in development but can be easily installed with pip:
+ 
+__Easy install__
 
 ```shell
+pip install trimnami
+```
+
+__Developer install__
+```shell
 git clone https://github.com/beardymcjohnface/Trimnami.git
 cd Trimnami/
 pip install -e .
 ```
 
 ## Test
```

### Comparing `trimnami-0.0.1/README.md` & `trimnami-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,23 @@
 - Prinseq++
 - BBtools for Round A/B viral metagenomics
 - Filtlong + Rasusa for longreads
 
 ## Install
 
 Trimnami is still in development but can be easily installed with pip:
+ 
+__Easy install__
 
 ```shell
+pip install trimnami
+```
+
+__Developer install__
+```shell
 git clone https://github.com/beardymcjohnface/Trimnami.git
 cd Trimnami/
 pip install -e .
 ```
 
 ## Test
```

### Comparing `trimnami-0.0.1/setup.py` & `trimnami-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,18 +49,18 @@
     version=get_version(),
     author="Michael Roach",
     author_email="beardymcjohnface@gmail.com",
     data_files=get_data_files(),
     py_modules=["trimnami"],
     install_requires=[
         "snaketool-utils>=0.0.3",
-        "snakemake>=7.14.0,<=7.26.0",
+        "snakemake>=7.14.0",
         "pyyaml>=6.0",
         "Click>=8.1.3",
-        "metasnek>=0.0.3",
+        "metasnek>=0.0.4",
         "attrmap>=0.0.7",
     ],
     entry_points={
         "console_scripts": [
             "trimnami=trimnami.__main__:main"
         ]
     },
```

### Comparing `trimnami-0.0.1/tests/test_skipHostRm.py` & `trimnami-0.0.2/tests/test_skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/tests/test_trimnami.py` & `trimnami-0.0.2/tests/test_trimnami.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     exec_command("trimnami -v")
     exec_command("trimnami -h")
     exec_command("trimnami run -h")
     exec_command("trimnami config -h")
 
 
 def test_trimnami_commands(tmp_dir):
-    exec_command("trimnami test --threads 1 -n prinseq fastp roundAB nanopore")
+    exec_command("trimnami test --threads 1 -n prinseq fastp roundAB nanopore notrim")
     exec_command("trimnami config")
     exec_command("trimnami citation")
```

### Comparing `trimnami-0.0.1/trimnami/__main__.py` & `trimnami-0.0.2/trimnami/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,21 +255,22 @@
             "host": snake_base(os.path.join("test_data", "ref.fna")),
             "output": kwargs["output"],
             "minimap": "map-ont",
             "log": kwargs["log"]
         }
     }
 
+    kwargs["snake_args"] = ["nanopore"]
+
     # run!
     run_snakemake(
         # Full path to Snakefile
         snakefile_path=snake_base(os.path.join("workflow", "Snakefile")),
         system_config=snake_base(os.path.join("config", "config.yaml")),
         merge_config=merge_config,
-        snake_args=["nanopore"],
         **kwargs
     )
 
 
 @click.command()
 @common_options
 def config(configfile, **kwargs):
```

### Comparing `trimnami-0.0.1/trimnami/config/system_config.yaml` & `trimnami-0.0.2/trimnami/config/system_config.yaml`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/scripts/skipHostRm.py` & `trimnami-0.0.2/trimnami/scripts/skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz` & `trimnami-0.0.2/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz` & `trimnami-0.0.2/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz` & `trimnami-0.0.2/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz` & `trimnami-0.0.2/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/test_data/A13-135-177-06_AGTTCC.fastq` & `trimnami-0.0.2/trimnami/test_data/A13-135-177-06_AGTTCC.fastq`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/test_data/nanopore/SRR7947171.fastq.gz` & `trimnami-0.0.2/trimnami/test_data/nanopore/SRR7947171.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/test_data/nanopore/SRR7947176.fastq.gz` & `trimnami-0.0.2/trimnami/test_data/nanopore/SRR7947176.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/test_data/ref.fna` & `trimnami-0.0.2/trimnami/test_data/ref.fna`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/trimnami.LICENSE` & `trimnami-0.0.2/trimnami/trimnami.LICENSE`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/workflow/Snakefile` & `trimnami-0.0.2/trimnami/workflow/Snakefile`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # Import rules
 include: os.path.join("rules", "preflight.smk")
 include: os.path.join("rules", "hostRemoval.smk")
 include: os.path.join("rules", "fastp.smk")
 include: os.path.join("rules", "prinseq.smk")
 include: os.path.join("rules", "roundAB.smk")
 include: os.path.join("rules", "nanopore.smk")
+include: os.path.join("rules", "notrim.smk")
 include: os.path.join("rules", "reports.smk")
 
 
 # Mark target rules
 target_rules = []
 def targetRule(fn):
     assert fn.__name__.startswith('__')
@@ -65,11 +66,18 @@
 rule nanopore:
     input:
         targets.nanopore,
         targets.reports
 
 
 @targetRule
+rule notrim:
+    input:
+        targets.notrim,
+        targets.reports
+
+
+@targetRule
 rule print_targets:
     run:
         print("\nTop level rules are: \n", file=sys.stderr)
         print("* " + "\n* ".join(target_rules) + "\n\n", file=sys.stderr)
```

### Comparing `trimnami-0.0.1/trimnami/workflow/databases/nebnext_adapters.fa` & `trimnami-0.0.2/trimnami/workflow/databases/nebnext_adapters.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/workflow/databases/primerB.fa` & `trimnami-0.0.2/trimnami/workflow/databases/primerB.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/workflow/databases/rc_primerB_ad6.fa` & `trimnami-0.0.2/trimnami/workflow/databases/rc_primerB_ad6.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/workflow/databases/vector_contaminants.fa` & `trimnami-0.0.2/trimnami/workflow/databases/vector_contaminants.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/workflow/rules/fastp.smk` & `trimnami-0.0.2/trimnami/workflow/rules/fastp.smk`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,26 @@
             -O {output.r2} \
             --unpaired1 {output.s1} \
             --unpaired2 {output.s2} \
             -z {params.compression} \
             -j {output.stats} \
             -h {output.html} \
             --thread {threads} \
-            --detect_adapter_for_pe {params.fastp} \
+            {params.fastp} \
             2> {log}
         if [[ -s {input.s} ]]
         then
             fastp \
             -i {input.s} \
             -o {output.s} \
             -z {params.compression} \
             -j {output.stats} \
             -h {output.html} \
             --thread {threads} \
-            --detect_adapter_for_pe {params.fastp} \
+            {params.fastp} \
             2> {log}
         else
             touch {output.s}
         fi
         cat {output.s1} {output.s2} >> {output.s}
         """
 
@@ -86,10 +86,10 @@
         fastp \
             -i {input.r1} \
             -o {output.r1} \
             -z {params.compression} \
             -j {output.stats} \
             -h {output.html} \
             --thread {threads} \
-            --detect_adapter_for_pe {params.fastp} \
+            {params.fastp} \
             2> {log}
         """
```

### Comparing `trimnami-0.0.1/trimnami/workflow/rules/hostRemoval.smk` & `trimnami-0.0.2/trimnami/workflow/rules/hostRemoval.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/workflow/rules/nanopore.smk` & `trimnami-0.0.2/trimnami/workflow/rules/nanopore.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/workflow/rules/preflight.smk` & `trimnami-0.0.2/trimnami/workflow/rules/preflight.smk`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 dir.temp = os.path.join(dir.out, "temp")
 dir.log = os.path.join(dir.out, "logs")
 dir.fastp = os.path.join(dir.out, "fastp")
 dir.prinseq = os.path.join(dir.out, "prinseq")
 dir.roundAB = os.path.join(dir.out, "roundAB")
 dir.nanopore = os.path.join(dir.out, "nanopore")
+dir.notrim = os.path.join(dir.out, "notrim")
 dir.bench = os.path.join(dir.out, "benchmarks")
 
 
 """
 Define file intermediates
 """
 # Check if host removal
@@ -74,17 +75,19 @@
 
 
 # target lists
 targets.fastp = []
 targets.prinseq = []
 targets.roundAB = []
 targets.nanopore = []
+targets.notrim = []
 targets.reports = [
     os.path.join(dir.out,"samples.tsv"),
 ]
 
 # populate target lists
 for sample_name in samples.names:
     targets.fastp.append(expand(os.path.join(dir.fastp, "{file}"), file=samples.reads[sample_name]["targetNames"]))
     targets.prinseq.append(expand(os.path.join(dir.prinseq, "{file}"), file=samples.reads[sample_name]["targetNames"]))
     targets.roundAB.append(expand(os.path.join(dir.roundAB, "{file}"), file=samples.reads[sample_name]["targetNames"]))
     targets.nanopore.append(expand(os.path.join(dir.nanopore, "{file}"), file=samples.reads[sample_name]["targetNames"]))
+    targets.notrim.append(expand(os.path.join(dir.notrim, "{file}"), file=samples.reads[sample_name]["targetNames"]))
```

### Comparing `trimnami-0.0.1/trimnami/workflow/rules/prinseq.smk` & `trimnami-0.0.2/trimnami/workflow/rules/prinseq.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami/workflow/rules/roundAB.smk` & `trimnami-0.0.2/trimnami/workflow/rules/roundAB.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.1/trimnami.egg-info/PKG-INFO` & `trimnami-0.0.2/trimnami.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimnami
-Version: 0.0.1
+Version: 0.0.2
 Summary: Trim lots of metagenomics samples all at once.
 Home-page: https://github.com/beardymcjohnface/Trimnami
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -34,16 +34,23 @@
 - Prinseq++
 - BBtools for Round A/B viral metagenomics
 - Filtlong + Rasusa for longreads
 
 ## Install
 
 Trimnami is still in development but can be easily installed with pip:
+ 
+__Easy install__
 
 ```shell
+pip install trimnami
+```
+
+__Developer install__
+```shell
 git clone https://github.com/beardymcjohnface/Trimnami.git
 cd Trimnami/
 pip install -e .
 ```
 
 ## Test
```

### Comparing `trimnami-0.0.1/trimnami.egg-info/SOURCES.txt` & `trimnami-0.0.2/trimnami.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,11 +37,12 @@
 trimnami/workflow/envs/minimap2.yaml
 trimnami/workflow/envs/pigz.yaml
 trimnami/workflow/envs/prinseq.yaml
 trimnami/workflow/envs/rasusa.yaml
 trimnami/workflow/rules/fastp.smk
 trimnami/workflow/rules/hostRemoval.smk
 trimnami/workflow/rules/nanopore.smk
+trimnami/workflow/rules/notrim.smk
 trimnami/workflow/rules/preflight.smk
 trimnami/workflow/rules/prinseq.smk
 trimnami/workflow/rules/reports.smk
 trimnami/workflow/rules/roundAB.smk
```

