# Comparing `tmp/dark-matter-4.0.8.tar.gz` & `tmp/dark-matter-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dark-matter-4.0.8.tar", last modified: Fri Oct  1 15:33:40 2021, max compression
+gzip compressed data, was "dark-matter-4.0.9.tar", last modified: Sun Oct  3 19:42:47 2021, max compression
```

## Comparing `dark-matter-4.0.8.tar` & `dark-matter-4.0.9.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-01 15:33:40.262521 dark-matter-4.0.8/
--rw-rw-r--   0 terry      (501) staff       (20)      763 2021-10-01 15:33:40.262246 dark-matter-4.0.8/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)     2244 2021-08-17 14:54:46.000000 dark-matter-4.0.8/README.md
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-01 15:33:40.233217 dark-matter-4.0.8/bin/
--rwxrwxr-x   0 terry      (501) staff       (20)     1170 2021-08-17 14:54:46.000000 dark-matter-4.0.8/bin/aa-info.py
--rwxrwxr-x   0 terry      (501) staff       (20)     1370 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/aa-to-dna.py
--rwxr-xr-x   0 terry      (501) staff       (20)      528 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/aa-to-properties.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1204 2016-09-07 14:55:30.000000 dark-matter-4.0.8/bin/adaptor-distances.py
--rwxrwxr-x   0 terry      (501) staff       (20)    16440 2021-08-17 14:54:53.000000 dark-matter-4.0.8/bin/alignment-panel-civ.py
--rwxr-xr-x   0 terry      (501) staff       (20)      753 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/alignments-per-read.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1273 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/bit-score-to-e-value.py
--rwxrwxr-x   0 terry      (501) staff       (20)      377 2021-08-17 14:54:46.000000 dark-matter-4.0.8/bin/cat-json-blast-records.py
--rwxr-xr-x   0 terry      (501) staff       (20)     2968 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/check-fasta-json-blast-consistency.py
--rwxrwxr-x   0 terry      (501) staff       (20)     1388 2021-08-17 14:54:53.000000 dark-matter-4.0.8/bin/codon-distance.py
--rwxrwxr-x   0 terry      (501) staff       (20)     7658 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/compare-consensuses.py
--rwxrwxr-x   0 terry      (501) staff       (20)     7064 2021-08-17 14:54:50.000000 dark-matter-4.0.8/bin/compare-sequences.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1179 2016-10-24 23:36:53.000000 dark-matter-4.0.8/bin/convert-blast-xml-to-json.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1584 2016-10-31 17:37:21.000000 dark-matter-4.0.8/bin/convert-diamond-to-json.py
--rwxrwxr-x   0 terry      (501) staff       (20)     4841 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/convert-diamond-to-sam.py
--rwxr-xr-x   0 terry      (501) staff       (20)      528 2015-05-01 08:27:43.000000 dark-matter-4.0.8/bin/convert-sam-to-fastq.sh
--rwxrwxr-x   0 terry      (501) staff       (20)     1342 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/create-newick-relabeling-output.py
--rwxr-xr-x   0 terry      (501) staff       (20)      111 2017-05-08 11:22:57.000000 dark-matter-4.0.8/bin/dark-matter-version.py
--rwxrwxr-x   0 terry      (501) staff       (20)      520 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/describe-protein-database.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1728 2017-02-13 16:20:08.000000 dark-matter-4.0.8/bin/dna-to-aa.py
--rwxrwxr-x   0 terry      (501) staff       (20)     5393 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/download-genbank.sh
--rwxr-xr-x   0 terry      (501) staff       (20)     1259 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/e-value-to-bit-score.py
--rwxrwxr-x   0 terry      (501) staff       (20)     5545 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/extract-ORFs.py
--rwxr-xr-x   0 terry      (501) staff       (20)     2968 2017-03-03 10:05:48.000000 dark-matter-4.0.8/bin/fasta-base-indices.py
--rwxr-xr-x   0 terry      (501) staff       (20)      588 2017-09-22 10:12:42.000000 dark-matter-4.0.8/bin/fasta-count.py
--rwxrwxr-x   0 terry      (501) staff       (20)     3765 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/fasta-diff.sh
--rwxrwxr-x   0 terry      (501) staff       (20)    20538 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/fasta-identity-table.py
--rwxr-xr-x   0 terry      (501) staff       (20)      512 2017-03-03 10:05:48.000000 dark-matter-4.0.8/bin/fasta-ids.py
--rwxrwxr-x   0 terry      (501) staff       (20)     1407 2021-08-24 13:14:53.000000 dark-matter-4.0.8/bin/fasta-join.py
--rwxr-xr-x   0 terry      (501) staff       (20)      535 2017-02-13 16:20:08.000000 dark-matter-4.0.8/bin/fasta-lengths.py
--rwxrwxr-x   0 terry      (501) staff       (20)      492 2021-08-17 14:54:46.000000 dark-matter-4.0.8/bin/fasta-sequences.py
--rwxr-xr-x   0 terry      (501) staff       (20)      506 2017-12-06 09:59:11.000000 dark-matter-4.0.8/bin/fasta-sort.py
--rwxr-xr-x   0 terry      (501) staff       (20)     3784 2018-01-29 11:44:38.000000 dark-matter-4.0.8/bin/fasta-split-by-id.py
--rwxrwxr-x   0 terry      (501) staff       (20)     3575 2021-08-17 15:14:32.000000 dark-matter-4.0.8/bin/fasta-split.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1673 2016-09-07 14:55:30.000000 dark-matter-4.0.8/bin/fasta-subset.py
--rwxr-xr-x   0 terry      (501) staff       (20)      419 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/fasta-subtraction.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1791 2018-03-01 09:56:23.000000 dark-matter-4.0.8/bin/fasta-to-phylip.py
--rwxrwxr-x   0 terry      (501) staff       (20)     4891 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/fasta-variable-sites.py
--rwxr-xr-x   0 terry      (501) staff       (20)     3065 2018-04-16 23:38:28.000000 dark-matter-4.0.8/bin/filter-fasta-by-complexity.py
--rwxrwxr-x   0 terry      (501) staff       (20)     4113 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/filter-fasta-by-taxonomy.py
--rwxrwxr-x   0 terry      (501) staff       (20)     3527 2021-08-17 15:16:18.000000 dark-matter-4.0.8/bin/filter-fasta.py
--rwxrwxr-x   0 terry      (501) staff       (20)     6147 2021-08-17 14:54:53.000000 dark-matter-4.0.8/bin/filter-hits-to-fasta.py
--rwxr-xr-x   0 terry      (501) staff       (20)     8530 2017-05-24 20:29:37.000000 dark-matter-4.0.8/bin/filter-reads-alignments.py
--rwxrwxr-x   0 terry      (501) staff       (20)     4544 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/filter-sam.py
--rwxr-xr-x   0 terry      (501) staff       (20)      572 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/find-hits.py
--rwxrwxr-x   0 terry      (501) staff       (20)     3055 2021-08-17 14:54:46.000000 dark-matter-4.0.8/bin/format-fasta.py
--rwxrwxr-x   0 terry      (501) staff       (20)     8720 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/genome-protein-summary.py
--rwxr-xr-x   0 terry      (501) staff       (20)     2136 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/get-features.py
--rwxrwxr-x   0 terry      (501) staff       (20)     2172 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/get-hosts.py
--rwxrwxr-x   0 terry      (501) staff       (20)     4263 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/get-reads.py
--rwxrwxr-x   0 terry      (501) staff       (20)     2893 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/get-taxonomy.py
--rwxr-xr-x   0 terry      (501) staff       (20)      642 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/graph-evalues.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1588 2018-01-09 15:17:05.000000 dark-matter-4.0.8/bin/local-align.py
--rwxrwxr-x   0 terry      (501) staff       (20)    10130 2021-08-17 14:54:58.000000 dark-matter-4.0.8/bin/make-consensus.py
--rwxrwxr-x   0 terry      (501) staff       (20)     2377 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/make-fasta-database.py
--rwxrwxr-x   0 terry      (501) staff       (20)     9031 2021-08-17 14:54:50.000000 dark-matter-4.0.8/bin/make-protein-database.py
--rwxrwxr-x   0 terry      (501) staff       (20)      845 2021-08-17 14:54:46.000000 dark-matter-4.0.8/bin/ncbi-fetch-id.py
--rwxrwxr-x   0 terry      (501) staff       (20)     1564 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/newick-to-ascii.py
--rwxrwxr-x   0 terry      (501) staff       (20)    19208 2021-08-17 14:54:53.000000 dark-matter-4.0.8/bin/noninteractive-alignment-panel.py
--rwxrwxr-x   0 terry      (501) staff       (20)     1397 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/parse-genbank-flat-file.py
--rwxrwxr-x   0 terry      (501) staff       (20)    10764 2021-10-01 15:32:44.000000 dark-matter-4.0.8/bin/plot-references-by-inter-read-distance.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1006 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/position-summary.py
--rwxrwxr-x   0 terry      (501) staff       (20)      862 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/pre-commit.sh
--rwxr-xr-x   0 terry      (501) staff       (20)      519 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/print-blast-xml-for-derek.py
--rwxr-xr-x   0 terry      (501) staff       (20)      517 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/print-blast-xml.py
--rwxr-xr-x   0 terry      (501) staff       (20)      906 2016-09-07 14:55:30.000000 dark-matter-4.0.8/bin/print-read-lengths.py
--rwxrwxr-x   0 terry      (501) staff       (20)    11947 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/proteins-to-pathogens-civ.py
--rwxrwxr-x   0 terry      (501) staff       (20)    11659 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/proteins-to-pathogens.py
--rwxr-xr-x   0 terry      (501) staff       (20)      615 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/randomize-fasta.py
--rwxr-xr-x   0 terry      (501) staff       (20)      729 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/read-blast-json.py
--rwxr-xr-x   0 terry      (501) staff       (20)      667 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/read-blast-xml.py
--rwxrwxr-x   0 terry      (501) staff       (20)     2564 2021-10-01 15:32:44.000000 dark-matter-4.0.8/bin/reference-read-scores-to-JSON.py
--rwxrwxr-x   0 terry      (501) staff       (20)     2581 2021-08-17 14:54:38.000000 dark-matter-4.0.8/bin/relabel-newick-tree.py
--rwxrwxr-x   0 terry      (501) staff       (20)    14642 2021-08-17 14:54:58.000000 dark-matter-4.0.8/bin/run-bowtie2.py
--rwxr-xr-x   0 terry      (501) staff       (20)     3482 2018-04-16 23:38:28.000000 dark-matter-4.0.8/bin/run-bwa.py
--rwxrwxr-x   0 terry      (501) staff       (20)     4827 2021-08-17 14:54:46.000000 dark-matter-4.0.8/bin/sam-coverage-depth.py
--rwxrwxr-x   0 terry      (501) staff       (20)     2601 2021-08-17 14:54:46.000000 dark-matter-4.0.8/bin/sam-coverage.py
--rwxrwxr-x   0 terry      (501) staff       (20)     5885 2021-08-17 15:13:05.000000 dark-matter-4.0.8/bin/sam-reference-read-counts.py
--rwxrwxr-x   0 terry      (501) staff       (20)      444 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/sam-references.py
--rwxrwxr-x   0 terry      (501) staff       (20)     3449 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/sam-to-fasta-alignment.py
--rwxr-xr-x   0 terry      (501) staff       (20)      275 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/sff-to-fastq.py
--rwxr-xr-x   0 terry      (501) staff       (20)     5973 2016-09-07 14:55:30.000000 dark-matter-4.0.8/bin/split-fasta-by-adaptors.py
--rwxrwxr-x   0 terry      (501) staff       (20)     2385 2021-08-17 14:54:05.000000 dark-matter-4.0.8/bin/subset-protein-database.py
--rwxr-xr-x   0 terry      (501) staff       (20)     2795 2017-02-13 16:20:08.000000 dark-matter-4.0.8/bin/summarize-fasta-bases.py
--rwxr-xr-x   0 terry      (501) staff       (20)     1023 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/summarize-reads.py
--rwxrwxr-x   0 terry      (501) staff       (20)      221 2021-08-17 14:54:50.000000 dark-matter-4.0.8/bin/translate.py
--rwxrwxr-x   0 terry      (501) staff       (20)     1709 2021-08-17 14:54:50.000000 dark-matter-4.0.8/bin/trim-primers.py
--rwxr-xr-x   0 terry      (501) staff       (20)      557 2015-12-07 18:00:12.000000 dark-matter-4.0.8/bin/trim-reads.py
--rwxr-xr-x   0 terry      (501) staff       (20)     9382 2016-09-07 14:55:30.000000 dark-matter-4.0.8/bin/write-htcondor-job-spec.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-01 15:33:40.245019 dark-matter-4.0.8/dark/
--rw-rw-r--   0 terry      (501) staff       (20)      351 2021-10-01 15:32:44.000000 dark-matter-4.0.8/dark/__init__.py
--rw-rw-r--   0 terry      (501) staff       (20)    37165 2021-08-17 14:54:46.000000 dark-matter-4.0.8/dark/aa.py
--rw-rw-r--   0 terry      (501) staff       (20)     2824 2021-08-17 14:54:46.000000 dark-matter-4.0.8/dark/aligners.py
--rw-rw-r--   0 terry      (501) staff       (20)    19331 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/alignments.py
--rw-r--r--   0 terry      (501) staff       (20)     1411 2015-05-01 08:27:43.000000 dark-matter-4.0.8/dark/analyze_reads.py
--rw-r--r--   0 terry      (501) staff       (20)      819 2015-05-01 08:27:43.000000 dark-matter-4.0.8/dark/baseimage.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-01 15:33:40.246818 dark-matter-4.0.8/dark/blast/
--rw-r--r--   0 terry      (501) staff       (20)        0 2015-05-01 08:27:43.000000 dark-matter-4.0.8/dark/blast/__init__.py
--rw-rw-r--   0 terry      (501) staff       (20)    11202 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/blast/alignments.py
--rw-rw-r--   0 terry      (501) staff       (20)    12742 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/blast/conversion.py
--rw-r--r--   0 terry      (501) staff       (20)     1061 2015-12-07 18:00:12.000000 dark-matter-4.0.8/dark/blast/hacks.py
--rw-rw-r--   0 terry      (501) staff       (20)     7637 2021-08-17 14:54:53.000000 dark-matter-4.0.8/dark/blast/hsp.py
--rw-rw-r--   0 terry      (501) staff       (20)     1761 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/blast/params.py
--rw-rw-r--   0 terry      (501) staff       (20)     1057 2021-08-17 14:54:53.000000 dark-matter-4.0.8/dark/blast/records.py
--rw-r--r--   0 terry      (501) staff       (20)     2257 2015-05-01 08:27:43.000000 dark-matter-4.0.8/dark/blast/score.py
--rw-rw-r--   0 terry      (501) staff       (20)    12559 2021-08-17 14:54:50.000000 dark-matter-4.0.8/dark/bowtie2.py
--rw-rw-r--   0 terry      (501) staff       (20)     5555 2021-08-17 14:54:58.000000 dark-matter-4.0.8/dark/btop.py
--rw-rw-r--   0 terry      (501) staff       (20)     1835 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/cigar.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-01 15:33:40.247820 dark-matter-4.0.8/dark/civ/
--rw-rw-r--   0 terry      (501) staff       (20)        0 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/civ/__init__.py
--rw-rw-r--   0 terry      (501) staff       (20)    22462 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/civ/graphics.py
--rw-rw-r--   0 terry      (501) staff       (20)     6677 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/civ/html.py
--rw-rw-r--   0 terry      (501) staff       (20)   101450 2021-08-24 13:14:53.000000 dark-matter-4.0.8/dark/civ/proteins.py
--rw-r--r--   0 terry      (501) staff       (20)      866 2015-05-01 08:27:43.000000 dark-matter-4.0.8/dark/codonDistance.py
--rw-rw-r--   0 terry      (501) staff       (20)     3758 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/colors.py
--rw-r--r--   0 terry      (501) staff       (20)     4382 2016-10-31 11:28:25.000000 dark-matter-4.0.8/dark/consensus.py
--rw-r--r--   0 terry      (501) staff       (20)      277 2016-03-18 20:57:48.000000 dark-matter-4.0.8/dark/database.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-01 15:33:40.249524 dark-matter-4.0.8/dark/diamond/
--rw-r--r--   0 terry      (501) staff       (20)        0 2016-10-24 09:27:12.000000 dark-matter-4.0.8/dark/diamond/__init__.py
--rw-rw-r--   0 terry      (501) staff       (20)     8932 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/diamond/alignments.py
--rw-rw-r--   0 terry      (501) staff       (20)    18385 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/diamond/conversion.py
--rw-r--r--   0 terry      (501) staff       (20)     8972 2018-12-11 11:06:01.000000 dark-matter-4.0.8/dark/diamond/hsp.py
--rw-rw-r--   0 terry      (501) staff       (20)     3506 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/diamond/run.py
--rw-rw-r--   0 terry      (501) staff       (20)    15748 2021-08-17 14:54:58.000000 dark-matter-4.0.8/dark/diamond/sam.py
--rw-rw-r--   0 terry      (501) staff       (20)     1373 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/dimension.py
--rw-r--r--   0 terry      (501) staff       (20)     1525 2014-10-27 10:38:50.000000 dark-matter-4.0.8/dark/distance.py
--rw-rw-r--   0 terry      (501) staff       (20)    16883 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/dna.py
--rw-r--r--   0 terry      (501) staff       (20)      994 2015-12-07 18:00:12.000000 dark-matter-4.0.8/dark/entrez.py
--rw-rw-r--   0 terry      (501) staff       (20)      397 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/errors.py
--rw-rw-r--   0 terry      (501) staff       (20)    16081 2021-08-17 14:54:50.000000 dark-matter-4.0.8/dark/fasta.py
--rw-rw-r--   0 terry      (501) staff       (20)     3741 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/fasta_ss.py
--rw-r--r--   0 terry      (501) staff       (20)     1456 2016-12-14 13:37:44.000000 dark-matter-4.0.8/dark/fastq.py
--rw-rw-r--   0 terry      (501) staff       (20)    12233 2021-08-17 14:54:53.000000 dark-matter-4.0.8/dark/features.py
--rw-rw-r--   0 terry      (501) staff       (20)    18835 2021-08-17 14:54:50.000000 dark-matter-4.0.8/dark/filter.py
--rw-rw-r--   0 terry      (501) staff       (20)     2127 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/fpcache.py
--rw-rw-r--   0 terry      (501) staff       (20)     9316 2021-08-17 15:14:32.000000 dark-matter-4.0.8/dark/genbank.py
--rw-rw-r--   0 terry      (501) staff       (20)     9689 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/genomes.py
--rw-rw-r--   0 terry      (501) staff       (20)    37967 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/graphics.py
--rw-rw-r--   0 terry      (501) staff       (20)     7156 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/hsp.py
--rw-rw-r--   0 terry      (501) staff       (20)    11911 2021-08-24 13:14:53.000000 dark-matter-4.0.8/dark/html.py
--rw-r--r--   0 terry      (501) staff       (20)     6072 2017-04-21 09:11:56.000000 dark-matter-4.0.8/dark/intervals.py
--rw-r--r--   0 terry      (501) staff       (20)     1108 2015-05-01 08:27:43.000000 dark-matter-4.0.8/dark/ipynb.py
--rw-rw-r--   0 terry      (501) staff       (20)    14817 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/local_align.py
--rw-rw-r--   0 terry      (501) staff       (20)    16447 2021-08-17 14:54:53.000000 dark-matter-4.0.8/dark/mutations.py
--rw-r--r--   0 terry      (501) staff       (20)      535 2016-03-16 00:16:11.000000 dark-matter-4.0.8/dark/ncbidb.py
--rw-r--r--   0 terry      (501) staff       (20)     2745 2016-12-07 11:27:46.000000 dark-matter-4.0.8/dark/orfs.py
--rw-rw-r--   0 terry      (501) staff       (20)     4451 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/process.py
--rw-rw-r--   0 terry      (501) staff       (20)    44260 2021-08-17 14:54:38.000000 dark-matter-4.0.8/dark/proteins.py
--rw-rw-r--   0 terry      (501) staff       (20)    64784 2021-08-17 14:54:50.000000 dark-matter-4.0.8/dark/reads.py
--rw-rw-r--   0 terry      (501) staff       (20)    41610 2021-10-01 15:32:44.000000 dark-matter-4.0.8/dark/sam.py
--rw-r--r--   0 terry      (501) staff       (20)     1367 2015-05-01 08:27:43.000000 dark-matter-4.0.8/dark/score.py
--rw-rw-r--   0 terry      (501) staff       (20)     2939 2021-08-17 14:54:05.000000 dark-matter-4.0.8/dark/sequence.py
--rw-r--r--   0 terry      (501) staff       (20)     1142 2014-08-02 08:59:00.000000 dark-matter-4.0.8/dark/simplify.py
--rw-r--r--   0 terry      (501) staff       (20)     4059 2017-02-09 14:45:59.000000 dark-matter-4.0.8/dark/summarize.py
--rw-rw-r--   0 terry      (501) staff       (20)    23555 2021-08-17 14:54:46.000000 dark-matter-4.0.8/dark/taxonomy.py
--rw-rw-r--   0 terry      (501) staff       (20)    20236 2021-08-17 14:54:53.000000 dark-matter-4.0.8/dark/titles.py
--rw-rw-r--   0 terry      (501) staff       (20)    11499 2021-10-01 15:32:44.000000 dark-matter-4.0.8/dark/utils.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-01 15:33:40.250926 dark-matter-4.0.8/dark_matter.egg-info/
--rw-rw-r--   0 terry      (501) staff       (20)      763 2021-10-01 15:33:40.000000 dark-matter-4.0.8/dark_matter.egg-info/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)     4298 2021-10-01 15:33:40.000000 dark-matter-4.0.8/dark_matter.egg-info/SOURCES.txt
--rw-rw-r--   0 terry      (501) staff       (20)        1 2021-10-01 15:33:40.000000 dark-matter-4.0.8/dark_matter.egg-info/dependency_links.txt
--rw-rw-r--   0 terry      (501) staff       (20)      217 2021-10-01 15:33:40.000000 dark-matter-4.0.8/dark_matter.egg-info/requires.txt
--rw-rw-r--   0 terry      (501) staff       (20)        5 2021-10-01 15:33:40.000000 dark-matter-4.0.8/dark_matter.egg-info/top_level.txt
--rw-rw-r--   0 terry      (501) staff       (20)       38 2021-10-01 15:33:40.262669 dark-matter-4.0.8/setup.cfg
--rw-rw-r--   0 terry      (501) staff       (20)     4906 2021-10-01 15:32:44.000000 dark-matter-4.0.8/setup.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-01 15:33:40.261746 dark-matter-4.0.8/test/
--rw-rw-r--   0 terry      (501) staff       (20)    38223 2021-08-17 14:54:53.000000 dark-matter-4.0.8/test/test_aa.py
--rw-rw-r--   0 terry      (501) staff       (20)     7224 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_alignments.py
--rw-rw-r--   0 terry      (501) staff       (20)     4539 2021-08-17 14:54:05.000000 dark-matter-4.0.8/test/test_analyze_reads.py
--rw-rw-r--   0 terry      (501) staff       (20)    18487 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_bowtie2.py
--rw-rw-r--   0 terry      (501) staff       (20)    10223 2021-08-17 14:54:58.000000 dark-matter-4.0.8/test/test_btop.py
--rw-rw-r--   0 terry      (501) staff       (20)     5197 2021-08-17 14:54:05.000000 dark-matter-4.0.8/test/test_cigar.py
--rw-r--r--   0 terry      (501) staff       (20)     1059 2015-05-01 08:27:43.000000 dark-matter-4.0.8/test/test_codonDistance.py
--rw-rw-r--   0 terry      (501) staff       (20)     6080 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_colors.py
--rw-rw-r--   0 terry      (501) staff       (20)     3798 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_dimension.py
--rw-r--r--   0 terry      (501) staff       (20)      831 2014-10-27 10:38:50.000000 dark-matter-4.0.8/test/test_distance.py
--rw-rw-r--   0 terry      (501) staff       (20)    41767 2021-08-17 14:54:50.000000 dark-matter-4.0.8/test/test_dna.py
--rw-rw-r--   0 terry      (501) staff       (20)    40962 2021-08-17 14:54:50.000000 dark-matter-4.0.8/test/test_fasta.py
--rw-rw-r--   0 terry      (501) staff       (20)     6412 2021-08-17 14:54:50.000000 dark-matter-4.0.8/test/test_fasta_ss.py
--rw-rw-r--   0 terry      (501) staff       (20)     4526 2021-08-17 14:54:50.000000 dark-matter-4.0.8/test/test_fastq.py
--rw-rw-r--   0 terry      (501) staff       (20)    24040 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_features.py
--rw-rw-r--   0 terry      (501) staff       (20)    14079 2021-08-17 14:54:50.000000 dark-matter-4.0.8/test/test_filter.py
--rw-rw-r--   0 terry      (501) staff       (20)    18296 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_genbank.py
--rw-rw-r--   0 terry      (501) staff       (20)     8753 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_genomes.py
--rw-r--r--   0 terry      (501) staff       (20)     1342 2016-02-21 22:27:36.000000 dark-matter-4.0.8/test/test_graphics.py
--rw-rw-r--   0 terry      (501) staff       (20)     5801 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_hsp.py
--rw-rw-r--   0 terry      (501) staff       (20)     2891 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_html.py
--rw-r--r--   0 terry      (501) staff       (20)    21091 2017-04-21 09:11:56.000000 dark-matter-4.0.8/test/test_intervals.py
--rw-rw-r--   0 terry      (501) staff       (20)    11532 2021-08-17 14:54:50.000000 dark-matter-4.0.8/test/test_local_align.py
--rw-r--r--   0 terry      (501) staff       (20)     4451 2015-12-07 20:56:44.000000 dark-matter-4.0.8/test/test_mutations.py
--rw-r--r--   0 terry      (501) staff       (20)     1293 2014-08-02 08:58:59.000000 dark-matter-4.0.8/test/test_orfs.py
--rw-rw-r--   0 terry      (501) staff       (20)     2718 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_process.py
--rw-rw-r--   0 terry      (501) staff       (20)    50108 2021-08-17 14:54:50.000000 dark-matter-4.0.8/test/test_proteins.py
--rw-rw-r--   0 terry      (501) staff       (20)   143353 2021-08-17 14:54:50.000000 dark-matter-4.0.8/test/test_reads.py
--rw-rw-r--   0 terry      (501) staff       (20)    68403 2021-10-01 15:32:44.000000 dark-matter-4.0.8/test/test_sam.py
--rw-r--r--   0 terry      (501) staff       (20)     1685 2015-05-01 08:27:43.000000 dark-matter-4.0.8/test/test_score.py
--rw-rw-r--   0 terry      (501) staff       (20)     5244 2021-08-17 14:54:50.000000 dark-matter-4.0.8/test/test_sequence.py
--rw-r--r--   0 terry      (501) staff       (20)     1892 2014-08-02 08:58:59.000000 dark-matter-4.0.8/test/test_simplify.py
--rw-rw-r--   0 terry      (501) staff       (20)     9767 2021-08-17 14:54:05.000000 dark-matter-4.0.8/test/test_summarize.py
--rw-rw-r--   0 terry      (501) staff       (20)    15477 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_taxonomy.py
--rw-rw-r--   0 terry      (501) staff       (20)    42821 2021-08-17 14:54:38.000000 dark-matter-4.0.8/test/test_titles.py
--rw-rw-r--   0 terry      (501) staff       (20)    16458 2021-08-17 15:14:32.000000 dark-matter-4.0.8/test/test_utils.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-03 19:42:47.614698 dark-matter-4.0.9/
+-rw-rw-r--   0 terry      (501) staff       (20)      763 2021-10-03 19:42:47.614442 dark-matter-4.0.9/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)     2244 2021-08-17 14:54:46.000000 dark-matter-4.0.9/README.md
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-03 19:42:47.586204 dark-matter-4.0.9/bin/
+-rwxrwxr-x   0 terry      (501) staff       (20)     1170 2021-08-17 14:54:46.000000 dark-matter-4.0.9/bin/aa-info.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     1370 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/aa-to-dna.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      528 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/aa-to-properties.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1204 2016-09-07 14:55:30.000000 dark-matter-4.0.9/bin/adaptor-distances.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    16440 2021-08-17 14:54:53.000000 dark-matter-4.0.9/bin/alignment-panel-civ.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      753 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/alignments-per-read.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1273 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/bit-score-to-e-value.py
+-rwxrwxr-x   0 terry      (501) staff       (20)      377 2021-08-17 14:54:46.000000 dark-matter-4.0.9/bin/cat-json-blast-records.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     2968 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/check-fasta-json-blast-consistency.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     1388 2021-08-17 14:54:53.000000 dark-matter-4.0.9/bin/codon-distance.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     7658 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/compare-consensuses.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     7064 2021-08-17 14:54:50.000000 dark-matter-4.0.9/bin/compare-sequences.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1179 2016-10-24 23:36:53.000000 dark-matter-4.0.9/bin/convert-blast-xml-to-json.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1584 2016-10-31 17:37:21.000000 dark-matter-4.0.9/bin/convert-diamond-to-json.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     4841 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/convert-diamond-to-sam.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      528 2015-05-01 08:27:43.000000 dark-matter-4.0.9/bin/convert-sam-to-fastq.sh
+-rwxrwxr-x   0 terry      (501) staff       (20)     1342 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/create-newick-relabeling-output.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      111 2017-05-08 11:22:57.000000 dark-matter-4.0.9/bin/dark-matter-version.py
+-rwxrwxr-x   0 terry      (501) staff       (20)      520 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/describe-protein-database.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1728 2017-02-13 16:20:08.000000 dark-matter-4.0.9/bin/dna-to-aa.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     5393 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/download-genbank.sh
+-rwxr-xr-x   0 terry      (501) staff       (20)     1259 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/e-value-to-bit-score.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     5545 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/extract-ORFs.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     2968 2017-03-03 10:05:48.000000 dark-matter-4.0.9/bin/fasta-base-indices.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      588 2017-09-22 10:12:42.000000 dark-matter-4.0.9/bin/fasta-count.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     3765 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/fasta-diff.sh
+-rwxrwxr-x   0 terry      (501) staff       (20)    20538 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/fasta-identity-table.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      512 2017-03-03 10:05:48.000000 dark-matter-4.0.9/bin/fasta-ids.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     1407 2021-08-24 13:14:53.000000 dark-matter-4.0.9/bin/fasta-join.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      535 2017-02-13 16:20:08.000000 dark-matter-4.0.9/bin/fasta-lengths.py
+-rwxrwxr-x   0 terry      (501) staff       (20)      492 2021-08-17 14:54:46.000000 dark-matter-4.0.9/bin/fasta-sequences.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      506 2017-12-06 09:59:11.000000 dark-matter-4.0.9/bin/fasta-sort.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     3784 2018-01-29 11:44:38.000000 dark-matter-4.0.9/bin/fasta-split-by-id.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     3575 2021-08-17 15:14:32.000000 dark-matter-4.0.9/bin/fasta-split.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1673 2016-09-07 14:55:30.000000 dark-matter-4.0.9/bin/fasta-subset.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      419 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/fasta-subtraction.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1791 2018-03-01 09:56:23.000000 dark-matter-4.0.9/bin/fasta-to-phylip.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     4891 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/fasta-variable-sites.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     3065 2018-04-16 23:38:28.000000 dark-matter-4.0.9/bin/filter-fasta-by-complexity.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     4113 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/filter-fasta-by-taxonomy.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     3527 2021-08-17 15:16:18.000000 dark-matter-4.0.9/bin/filter-fasta.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     6147 2021-08-17 14:54:53.000000 dark-matter-4.0.9/bin/filter-hits-to-fasta.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     8530 2017-05-24 20:29:37.000000 dark-matter-4.0.9/bin/filter-reads-alignments.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     4544 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/filter-sam.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      572 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/find-hits.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     3055 2021-08-17 14:54:46.000000 dark-matter-4.0.9/bin/format-fasta.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     8720 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/genome-protein-summary.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     2136 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/get-features.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     2172 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/get-hosts.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     4263 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/get-reads.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     2893 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/get-taxonomy.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      642 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/graph-evalues.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1588 2018-01-09 15:17:05.000000 dark-matter-4.0.9/bin/local-align.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    10130 2021-08-17 14:54:58.000000 dark-matter-4.0.9/bin/make-consensus.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     2377 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/make-fasta-database.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     9031 2021-08-17 14:54:50.000000 dark-matter-4.0.9/bin/make-protein-database.py
+-rwxrwxr-x   0 terry      (501) staff       (20)      845 2021-08-17 14:54:46.000000 dark-matter-4.0.9/bin/ncbi-fetch-id.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     1564 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/newick-to-ascii.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    19208 2021-08-17 14:54:53.000000 dark-matter-4.0.9/bin/noninteractive-alignment-panel.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     1397 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/parse-genbank-flat-file.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    10764 2021-10-01 15:32:44.000000 dark-matter-4.0.9/bin/plot-references-by-inter-read-distance.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1006 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/position-summary.py
+-rwxrwxr-x   0 terry      (501) staff       (20)      862 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/pre-commit.sh
+-rwxr-xr-x   0 terry      (501) staff       (20)      519 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/print-blast-xml-for-derek.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      517 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/print-blast-xml.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      906 2016-09-07 14:55:30.000000 dark-matter-4.0.9/bin/print-read-lengths.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    11947 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/proteins-to-pathogens-civ.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    11659 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/proteins-to-pathogens.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      615 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/randomize-fasta.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      729 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/read-blast-json.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      667 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/read-blast-xml.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     2564 2021-10-01 15:32:44.000000 dark-matter-4.0.9/bin/reference-read-scores-to-JSON.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     2581 2021-08-17 14:54:38.000000 dark-matter-4.0.9/bin/relabel-newick-tree.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    14642 2021-08-17 14:54:58.000000 dark-matter-4.0.9/bin/run-bowtie2.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     3482 2018-04-16 23:38:28.000000 dark-matter-4.0.9/bin/run-bwa.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     4827 2021-08-17 14:54:46.000000 dark-matter-4.0.9/bin/sam-coverage-depth.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     2601 2021-08-17 14:54:46.000000 dark-matter-4.0.9/bin/sam-coverage.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     5885 2021-08-17 15:13:05.000000 dark-matter-4.0.9/bin/sam-reference-read-counts.py
+-rwxrwxr-x   0 terry      (501) staff       (20)      444 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/sam-references.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     3449 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/sam-to-fasta-alignment.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      275 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/sff-to-fastq.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     5973 2016-09-07 14:55:30.000000 dark-matter-4.0.9/bin/split-fasta-by-adaptors.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     2385 2021-08-17 14:54:05.000000 dark-matter-4.0.9/bin/subset-protein-database.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     2795 2017-02-13 16:20:08.000000 dark-matter-4.0.9/bin/summarize-fasta-bases.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     1023 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/summarize-reads.py
+-rwxrwxr-x   0 terry      (501) staff       (20)      221 2021-08-17 14:54:50.000000 dark-matter-4.0.9/bin/translate.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     1709 2021-08-17 14:54:50.000000 dark-matter-4.0.9/bin/trim-primers.py
+-rwxr-xr-x   0 terry      (501) staff       (20)      557 2015-12-07 18:00:12.000000 dark-matter-4.0.9/bin/trim-reads.py
+-rwxr-xr-x   0 terry      (501) staff       (20)     9382 2016-09-07 14:55:30.000000 dark-matter-4.0.9/bin/write-htcondor-job-spec.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-03 19:42:47.598690 dark-matter-4.0.9/dark/
+-rw-rw-r--   0 terry      (501) staff       (20)      351 2021-10-03 19:42:37.000000 dark-matter-4.0.9/dark/__init__.py
+-rw-rw-r--   0 terry      (501) staff       (20)    37165 2021-08-17 14:54:46.000000 dark-matter-4.0.9/dark/aa.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2824 2021-08-17 14:54:46.000000 dark-matter-4.0.9/dark/aligners.py
+-rw-rw-r--   0 terry      (501) staff       (20)    19331 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/alignments.py
+-rw-r--r--   0 terry      (501) staff       (20)     1411 2015-05-01 08:27:43.000000 dark-matter-4.0.9/dark/analyze_reads.py
+-rw-r--r--   0 terry      (501) staff       (20)      819 2015-05-01 08:27:43.000000 dark-matter-4.0.9/dark/baseimage.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-03 19:42:47.600603 dark-matter-4.0.9/dark/blast/
+-rw-r--r--   0 terry      (501) staff       (20)        0 2015-05-01 08:27:43.000000 dark-matter-4.0.9/dark/blast/__init__.py
+-rw-rw-r--   0 terry      (501) staff       (20)    11202 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/blast/alignments.py
+-rw-rw-r--   0 terry      (501) staff       (20)    12742 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/blast/conversion.py
+-rw-r--r--   0 terry      (501) staff       (20)     1061 2015-12-07 18:00:12.000000 dark-matter-4.0.9/dark/blast/hacks.py
+-rw-rw-r--   0 terry      (501) staff       (20)     7637 2021-08-17 14:54:53.000000 dark-matter-4.0.9/dark/blast/hsp.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1761 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/blast/params.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1057 2021-08-17 14:54:53.000000 dark-matter-4.0.9/dark/blast/records.py
+-rw-r--r--   0 terry      (501) staff       (20)     2257 2015-05-01 08:27:43.000000 dark-matter-4.0.9/dark/blast/score.py
+-rw-rw-r--   0 terry      (501) staff       (20)    12559 2021-08-17 14:54:50.000000 dark-matter-4.0.9/dark/bowtie2.py
+-rw-rw-r--   0 terry      (501) staff       (20)     5555 2021-08-17 14:54:58.000000 dark-matter-4.0.9/dark/btop.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1835 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/cigar.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-03 19:42:47.601565 dark-matter-4.0.9/dark/civ/
+-rw-rw-r--   0 terry      (501) staff       (20)        0 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/civ/__init__.py
+-rw-rw-r--   0 terry      (501) staff       (20)    22462 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/civ/graphics.py
+-rw-rw-r--   0 terry      (501) staff       (20)     6677 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/civ/html.py
+-rw-rw-r--   0 terry      (501) staff       (20)    94038 2021-10-03 19:42:37.000000 dark-matter-4.0.9/dark/civ/proteins.py
+-rw-r--r--   0 terry      (501) staff       (20)      866 2015-05-01 08:27:43.000000 dark-matter-4.0.9/dark/codonDistance.py
+-rw-rw-r--   0 terry      (501) staff       (20)     3758 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/colors.py
+-rw-r--r--   0 terry      (501) staff       (20)     4382 2016-10-31 11:28:25.000000 dark-matter-4.0.9/dark/consensus.py
+-rw-r--r--   0 terry      (501) staff       (20)      277 2016-03-18 20:57:48.000000 dark-matter-4.0.9/dark/database.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-03 19:42:47.603137 dark-matter-4.0.9/dark/diamond/
+-rw-r--r--   0 terry      (501) staff       (20)        0 2016-10-24 09:27:12.000000 dark-matter-4.0.9/dark/diamond/__init__.py
+-rw-rw-r--   0 terry      (501) staff       (20)     8932 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/diamond/alignments.py
+-rw-rw-r--   0 terry      (501) staff       (20)    18385 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/diamond/conversion.py
+-rw-r--r--   0 terry      (501) staff       (20)     8972 2018-12-11 11:06:01.000000 dark-matter-4.0.9/dark/diamond/hsp.py
+-rw-rw-r--   0 terry      (501) staff       (20)     3506 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/diamond/run.py
+-rw-rw-r--   0 terry      (501) staff       (20)    15748 2021-08-17 14:54:58.000000 dark-matter-4.0.9/dark/diamond/sam.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1373 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/dimension.py
+-rw-r--r--   0 terry      (501) staff       (20)     1525 2014-10-27 10:38:50.000000 dark-matter-4.0.9/dark/distance.py
+-rw-rw-r--   0 terry      (501) staff       (20)    16883 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/dna.py
+-rw-r--r--   0 terry      (501) staff       (20)      994 2015-12-07 18:00:12.000000 dark-matter-4.0.9/dark/entrez.py
+-rw-rw-r--   0 terry      (501) staff       (20)      397 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/errors.py
+-rw-rw-r--   0 terry      (501) staff       (20)    16081 2021-08-17 14:54:50.000000 dark-matter-4.0.9/dark/fasta.py
+-rw-rw-r--   0 terry      (501) staff       (20)     3741 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/fasta_ss.py
+-rw-r--r--   0 terry      (501) staff       (20)     1456 2016-12-14 13:37:44.000000 dark-matter-4.0.9/dark/fastq.py
+-rw-rw-r--   0 terry      (501) staff       (20)    12233 2021-08-17 14:54:53.000000 dark-matter-4.0.9/dark/features.py
+-rw-rw-r--   0 terry      (501) staff       (20)    18835 2021-08-17 14:54:50.000000 dark-matter-4.0.9/dark/filter.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2127 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/fpcache.py
+-rw-rw-r--   0 terry      (501) staff       (20)    16422 2021-10-03 19:42:37.000000 dark-matter-4.0.9/dark/genbank.py
+-rw-rw-r--   0 terry      (501) staff       (20)     9689 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/genomes.py
+-rw-rw-r--   0 terry      (501) staff       (20)    37967 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/graphics.py
+-rw-rw-r--   0 terry      (501) staff       (20)     7156 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/hsp.py
+-rw-rw-r--   0 terry      (501) staff       (20)    11911 2021-08-24 13:14:53.000000 dark-matter-4.0.9/dark/html.py
+-rw-r--r--   0 terry      (501) staff       (20)     6072 2017-04-21 09:11:56.000000 dark-matter-4.0.9/dark/intervals.py
+-rw-r--r--   0 terry      (501) staff       (20)     1108 2015-05-01 08:27:43.000000 dark-matter-4.0.9/dark/ipynb.py
+-rw-rw-r--   0 terry      (501) staff       (20)    14817 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/local_align.py
+-rw-rw-r--   0 terry      (501) staff       (20)    16447 2021-08-17 14:54:53.000000 dark-matter-4.0.9/dark/mutations.py
+-rw-r--r--   0 terry      (501) staff       (20)      535 2016-03-16 00:16:11.000000 dark-matter-4.0.9/dark/ncbidb.py
+-rw-r--r--   0 terry      (501) staff       (20)     2745 2016-12-07 11:27:46.000000 dark-matter-4.0.9/dark/orfs.py
+-rw-rw-r--   0 terry      (501) staff       (20)     4451 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/process.py
+-rw-rw-r--   0 terry      (501) staff       (20)    44260 2021-08-17 14:54:38.000000 dark-matter-4.0.9/dark/proteins.py
+-rw-rw-r--   0 terry      (501) staff       (20)    64784 2021-08-17 14:54:50.000000 dark-matter-4.0.9/dark/reads.py
+-rw-rw-r--   0 terry      (501) staff       (20)    41610 2021-10-01 15:32:44.000000 dark-matter-4.0.9/dark/sam.py
+-rw-r--r--   0 terry      (501) staff       (20)     1367 2015-05-01 08:27:43.000000 dark-matter-4.0.9/dark/score.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2939 2021-08-17 14:54:05.000000 dark-matter-4.0.9/dark/sequence.py
+-rw-r--r--   0 terry      (501) staff       (20)     1142 2014-08-02 08:59:00.000000 dark-matter-4.0.9/dark/simplify.py
+-rw-r--r--   0 terry      (501) staff       (20)     4059 2017-02-09 14:45:59.000000 dark-matter-4.0.9/dark/summarize.py
+-rw-rw-r--   0 terry      (501) staff       (20)    23555 2021-08-17 14:54:46.000000 dark-matter-4.0.9/dark/taxonomy.py
+-rw-rw-r--   0 terry      (501) staff       (20)    20236 2021-08-17 14:54:53.000000 dark-matter-4.0.9/dark/titles.py
+-rw-rw-r--   0 terry      (501) staff       (20)    11499 2021-10-01 15:32:44.000000 dark-matter-4.0.9/dark/utils.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-03 19:42:47.604357 dark-matter-4.0.9/dark_matter.egg-info/
+-rw-rw-r--   0 terry      (501) staff       (20)      763 2021-10-03 19:42:47.000000 dark-matter-4.0.9/dark_matter.egg-info/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)     4298 2021-10-03 19:42:47.000000 dark-matter-4.0.9/dark_matter.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        1 2021-10-03 19:42:47.000000 dark-matter-4.0.9/dark_matter.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry      (501) staff       (20)      217 2021-10-03 19:42:47.000000 dark-matter-4.0.9/dark_matter.egg-info/requires.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        5 2021-10-03 19:42:47.000000 dark-matter-4.0.9/dark_matter.egg-info/top_level.txt
+-rw-rw-r--   0 terry      (501) staff       (20)       38 2021-10-03 19:42:47.614776 dark-matter-4.0.9/setup.cfg
+-rw-rw-r--   0 terry      (501) staff       (20)     4906 2021-10-01 15:32:44.000000 dark-matter-4.0.9/setup.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2021-10-03 19:42:47.614053 dark-matter-4.0.9/test/
+-rw-rw-r--   0 terry      (501) staff       (20)    38223 2021-08-17 14:54:53.000000 dark-matter-4.0.9/test/test_aa.py
+-rw-rw-r--   0 terry      (501) staff       (20)     7224 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_alignments.py
+-rw-rw-r--   0 terry      (501) staff       (20)     4539 2021-08-17 14:54:05.000000 dark-matter-4.0.9/test/test_analyze_reads.py
+-rw-rw-r--   0 terry      (501) staff       (20)    18487 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_bowtie2.py
+-rw-rw-r--   0 terry      (501) staff       (20)    10223 2021-08-17 14:54:58.000000 dark-matter-4.0.9/test/test_btop.py
+-rw-rw-r--   0 terry      (501) staff       (20)     5197 2021-08-17 14:54:05.000000 dark-matter-4.0.9/test/test_cigar.py
+-rw-r--r--   0 terry      (501) staff       (20)     1059 2015-05-01 08:27:43.000000 dark-matter-4.0.9/test/test_codonDistance.py
+-rw-rw-r--   0 terry      (501) staff       (20)     6080 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_colors.py
+-rw-rw-r--   0 terry      (501) staff       (20)     3798 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_dimension.py
+-rw-r--r--   0 terry      (501) staff       (20)      831 2014-10-27 10:38:50.000000 dark-matter-4.0.9/test/test_distance.py
+-rw-rw-r--   0 terry      (501) staff       (20)    41767 2021-08-17 14:54:50.000000 dark-matter-4.0.9/test/test_dna.py
+-rw-rw-r--   0 terry      (501) staff       (20)    40962 2021-08-17 14:54:50.000000 dark-matter-4.0.9/test/test_fasta.py
+-rw-rw-r--   0 terry      (501) staff       (20)     6412 2021-08-17 14:54:50.000000 dark-matter-4.0.9/test/test_fasta_ss.py
+-rw-rw-r--   0 terry      (501) staff       (20)     4526 2021-08-17 14:54:50.000000 dark-matter-4.0.9/test/test_fastq.py
+-rw-rw-r--   0 terry      (501) staff       (20)    24040 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_features.py
+-rw-rw-r--   0 terry      (501) staff       (20)    14079 2021-08-17 14:54:50.000000 dark-matter-4.0.9/test/test_filter.py
+-rw-rw-r--   0 terry      (501) staff       (20)    18296 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_genbank.py
+-rw-rw-r--   0 terry      (501) staff       (20)     8753 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_genomes.py
+-rw-r--r--   0 terry      (501) staff       (20)     1342 2016-02-21 22:27:36.000000 dark-matter-4.0.9/test/test_graphics.py
+-rw-rw-r--   0 terry      (501) staff       (20)     5801 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_hsp.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2891 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_html.py
+-rw-r--r--   0 terry      (501) staff       (20)    21091 2017-04-21 09:11:56.000000 dark-matter-4.0.9/test/test_intervals.py
+-rw-rw-r--   0 terry      (501) staff       (20)    11532 2021-08-17 14:54:50.000000 dark-matter-4.0.9/test/test_local_align.py
+-rw-r--r--   0 terry      (501) staff       (20)     4451 2015-12-07 20:56:44.000000 dark-matter-4.0.9/test/test_mutations.py
+-rw-r--r--   0 terry      (501) staff       (20)     1293 2014-08-02 08:58:59.000000 dark-matter-4.0.9/test/test_orfs.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2718 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_process.py
+-rw-rw-r--   0 terry      (501) staff       (20)    50108 2021-08-17 14:54:50.000000 dark-matter-4.0.9/test/test_proteins.py
+-rw-rw-r--   0 terry      (501) staff       (20)   143353 2021-08-17 14:54:50.000000 dark-matter-4.0.9/test/test_reads.py
+-rw-rw-r--   0 terry      (501) staff       (20)    68403 2021-10-01 15:32:44.000000 dark-matter-4.0.9/test/test_sam.py
+-rw-r--r--   0 terry      (501) staff       (20)     1685 2015-05-01 08:27:43.000000 dark-matter-4.0.9/test/test_score.py
+-rw-rw-r--   0 terry      (501) staff       (20)     5244 2021-08-17 14:54:50.000000 dark-matter-4.0.9/test/test_sequence.py
+-rw-r--r--   0 terry      (501) staff       (20)     1892 2014-08-02 08:58:59.000000 dark-matter-4.0.9/test/test_simplify.py
+-rw-rw-r--   0 terry      (501) staff       (20)     9767 2021-08-17 14:54:05.000000 dark-matter-4.0.9/test/test_summarize.py
+-rw-rw-r--   0 terry      (501) staff       (20)    15477 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_taxonomy.py
+-rw-rw-r--   0 terry      (501) staff       (20)    42821 2021-08-17 14:54:38.000000 dark-matter-4.0.9/test/test_titles.py
+-rw-rw-r--   0 terry      (501) staff       (20)    16458 2021-08-17 15:14:32.000000 dark-matter-4.0.9/test/test_utils.py
```

### Comparing `dark-matter-4.0.8/PKG-INFO` & `dark-matter-4.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dark-matter
-Version: 4.0.8
+Version: 4.0.9
 Summary: Python classes for working with genetic sequence data
 Home-page: https://github.com/acorg/dark-matter
 Author: Terry Jones, Barbara Mühlemann, Tali Veith, Sophie Mathias, Udo Gieraths
 Author-email: tcj25@cam.ac.uk
 License: MIT
 Download-URL: https://github.com/acorg/dark-matter
 Description: UNKNOWN
```

### Comparing `dark-matter-4.0.8/README.md` & `dark-matter-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/aa-info.py` & `dark-matter-4.0.9/bin/aa-info.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/aa-to-dna.py` & `dark-matter-4.0.9/bin/aa-to-dna.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/aa-to-properties.py` & `dark-matter-4.0.9/bin/aa-to-properties.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/adaptor-distances.py` & `dark-matter-4.0.9/bin/adaptor-distances.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/alignment-panel-civ.py` & `dark-matter-4.0.9/bin/alignment-panel-civ.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/alignments-per-read.py` & `dark-matter-4.0.9/bin/alignments-per-read.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/bit-score-to-e-value.py` & `dark-matter-4.0.9/bin/bit-score-to-e-value.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/check-fasta-json-blast-consistency.py` & `dark-matter-4.0.9/bin/check-fasta-json-blast-consistency.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/codon-distance.py` & `dark-matter-4.0.9/bin/codon-distance.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/compare-consensuses.py` & `dark-matter-4.0.9/bin/compare-consensuses.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/compare-sequences.py` & `dark-matter-4.0.9/bin/compare-sequences.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/convert-blast-xml-to-json.py` & `dark-matter-4.0.9/bin/convert-blast-xml-to-json.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/convert-diamond-to-json.py` & `dark-matter-4.0.9/bin/convert-diamond-to-json.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/convert-diamond-to-sam.py` & `dark-matter-4.0.9/bin/convert-diamond-to-sam.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/convert-sam-to-fastq.sh` & `dark-matter-4.0.9/bin/convert-sam-to-fastq.sh`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/create-newick-relabeling-output.py` & `dark-matter-4.0.9/bin/create-newick-relabeling-output.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/describe-protein-database.py` & `dark-matter-4.0.9/bin/describe-protein-database.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/dna-to-aa.py` & `dark-matter-4.0.9/bin/dna-to-aa.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/download-genbank.sh` & `dark-matter-4.0.9/bin/download-genbank.sh`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/e-value-to-bit-score.py` & `dark-matter-4.0.9/bin/e-value-to-bit-score.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/extract-ORFs.py` & `dark-matter-4.0.9/bin/extract-ORFs.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-base-indices.py` & `dark-matter-4.0.9/bin/fasta-base-indices.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-count.py` & `dark-matter-4.0.9/bin/fasta-count.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-diff.sh` & `dark-matter-4.0.9/bin/fasta-diff.sh`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-identity-table.py` & `dark-matter-4.0.9/bin/fasta-identity-table.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-ids.py` & `dark-matter-4.0.9/bin/fasta-ids.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-join.py` & `dark-matter-4.0.9/bin/fasta-join.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-lengths.py` & `dark-matter-4.0.9/bin/fasta-lengths.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-split-by-id.py` & `dark-matter-4.0.9/bin/fasta-split-by-id.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-split.py` & `dark-matter-4.0.9/bin/fasta-split.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-subset.py` & `dark-matter-4.0.9/bin/fasta-subset.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-to-phylip.py` & `dark-matter-4.0.9/bin/fasta-to-phylip.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/fasta-variable-sites.py` & `dark-matter-4.0.9/bin/fasta-variable-sites.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/filter-fasta-by-complexity.py` & `dark-matter-4.0.9/bin/filter-fasta-by-complexity.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/filter-fasta-by-taxonomy.py` & `dark-matter-4.0.9/bin/filter-fasta-by-taxonomy.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/filter-fasta.py` & `dark-matter-4.0.9/bin/filter-fasta.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/filter-hits-to-fasta.py` & `dark-matter-4.0.9/bin/filter-hits-to-fasta.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/filter-reads-alignments.py` & `dark-matter-4.0.9/bin/filter-reads-alignments.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/filter-sam.py` & `dark-matter-4.0.9/bin/filter-sam.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/find-hits.py` & `dark-matter-4.0.9/bin/find-hits.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/format-fasta.py` & `dark-matter-4.0.9/bin/format-fasta.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/genome-protein-summary.py` & `dark-matter-4.0.9/bin/genome-protein-summary.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/get-features.py` & `dark-matter-4.0.9/bin/get-features.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/get-hosts.py` & `dark-matter-4.0.9/bin/get-hosts.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/get-reads.py` & `dark-matter-4.0.9/bin/get-reads.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/get-taxonomy.py` & `dark-matter-4.0.9/bin/get-taxonomy.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/graph-evalues.py` & `dark-matter-4.0.9/bin/graph-evalues.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/local-align.py` & `dark-matter-4.0.9/bin/local-align.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/make-consensus.py` & `dark-matter-4.0.9/bin/make-consensus.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/make-fasta-database.py` & `dark-matter-4.0.9/bin/make-fasta-database.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/make-protein-database.py` & `dark-matter-4.0.9/bin/make-protein-database.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/ncbi-fetch-id.py` & `dark-matter-4.0.9/bin/ncbi-fetch-id.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/newick-to-ascii.py` & `dark-matter-4.0.9/bin/newick-to-ascii.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/noninteractive-alignment-panel.py` & `dark-matter-4.0.9/bin/noninteractive-alignment-panel.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/parse-genbank-flat-file.py` & `dark-matter-4.0.9/bin/parse-genbank-flat-file.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/plot-references-by-inter-read-distance.py` & `dark-matter-4.0.9/bin/plot-references-by-inter-read-distance.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/position-summary.py` & `dark-matter-4.0.9/bin/position-summary.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/pre-commit.sh` & `dark-matter-4.0.9/bin/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/print-blast-xml-for-derek.py` & `dark-matter-4.0.9/bin/print-blast-xml-for-derek.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/print-blast-xml.py` & `dark-matter-4.0.9/bin/print-blast-xml.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/print-read-lengths.py` & `dark-matter-4.0.9/bin/print-read-lengths.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/proteins-to-pathogens-civ.py` & `dark-matter-4.0.9/bin/proteins-to-pathogens-civ.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/proteins-to-pathogens.py` & `dark-matter-4.0.9/bin/proteins-to-pathogens.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/randomize-fasta.py` & `dark-matter-4.0.9/bin/randomize-fasta.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/read-blast-json.py` & `dark-matter-4.0.9/bin/read-blast-json.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/read-blast-xml.py` & `dark-matter-4.0.9/bin/read-blast-xml.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/reference-read-scores-to-JSON.py` & `dark-matter-4.0.9/bin/reference-read-scores-to-JSON.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/relabel-newick-tree.py` & `dark-matter-4.0.9/bin/relabel-newick-tree.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/run-bowtie2.py` & `dark-matter-4.0.9/bin/run-bowtie2.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/run-bwa.py` & `dark-matter-4.0.9/bin/run-bwa.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/sam-coverage-depth.py` & `dark-matter-4.0.9/bin/sam-coverage-depth.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/sam-coverage.py` & `dark-matter-4.0.9/bin/sam-coverage.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/sam-reference-read-counts.py` & `dark-matter-4.0.9/bin/sam-reference-read-counts.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/sam-to-fasta-alignment.py` & `dark-matter-4.0.9/bin/sam-to-fasta-alignment.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/split-fasta-by-adaptors.py` & `dark-matter-4.0.9/bin/split-fasta-by-adaptors.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/subset-protein-database.py` & `dark-matter-4.0.9/bin/subset-protein-database.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/summarize-fasta-bases.py` & `dark-matter-4.0.9/bin/summarize-fasta-bases.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/summarize-reads.py` & `dark-matter-4.0.9/bin/summarize-reads.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/trim-primers.py` & `dark-matter-4.0.9/bin/trim-primers.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/trim-reads.py` & `dark-matter-4.0.9/bin/trim-reads.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/bin/write-htcondor-job-spec.py` & `dark-matter-4.0.9/bin/write-htcondor-job-spec.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/aa.py` & `dark-matter-4.0.9/dark/aa.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/aligners.py` & `dark-matter-4.0.9/dark/aligners.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/alignments.py` & `dark-matter-4.0.9/dark/alignments.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/analyze_reads.py` & `dark-matter-4.0.9/dark/analyze_reads.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/baseimage.py` & `dark-matter-4.0.9/dark/baseimage.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/blast/alignments.py` & `dark-matter-4.0.9/dark/blast/alignments.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/blast/conversion.py` & `dark-matter-4.0.9/dark/blast/conversion.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/blast/hacks.py` & `dark-matter-4.0.9/dark/blast/hacks.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/blast/hsp.py` & `dark-matter-4.0.9/dark/blast/hsp.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/blast/params.py` & `dark-matter-4.0.9/dark/blast/params.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/blast/records.py` & `dark-matter-4.0.9/dark/blast/records.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/blast/score.py` & `dark-matter-4.0.9/dark/blast/score.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/bowtie2.py` & `dark-matter-4.0.9/dark/bowtie2.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/btop.py` & `dark-matter-4.0.9/dark/btop.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/cigar.py` & `dark-matter-4.0.9/dark/cigar.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/civ/graphics.py` & `dark-matter-4.0.9/dark/civ/graphics.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/civ/html.py` & `dark-matter-4.0.9/dark/civ/html.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/civ/proteins.py` & `dark-matter-4.0.9/dark/civ/proteins.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 from functools import partial
 from json import load
 from operator import attrgetter, itemgetter
 from os.path import dirname, exists, join
 from six import string_types
 from six.moves.urllib.parse import quote
 from textwrap import fill
-from warnings import warn
 
 from dark.dimension import dimensionalIterator
 from dark.errors import DatabaseDuplicationError
 from dark.fasta import FastaReads
 from dark.fastq import FastqReads
 from dark.filter import TitleFilter
-from dark.genbank import GenomeRanges
+from dark.genbank import getCDSInfo, getSourceInfo
 from dark.html import NCBISequenceLinkURL, NCBISequenceLink, readCountText
 from dark.reads import Reads
 from dark.taxonomy import (
     # isDNAVirus, isRNAVirus, formatLineage,
     lineageTaxonomyLinks, Hierarchy,
     LineageElement)
 
@@ -1585,18 +1584,18 @@
         assert not (dnaOnly and rnaOnly), (
             'dnaOnly and rnaOnly cannot both be True.')
 
         examinedGenomeCount = addedGenomeCount = addedProteinCount = 0
 
         for genome in genomes:
             examinedGenomeCount += 1
-            source = self._sourceInfo(genome, logfp=logfp)
+            source = getSourceInfo(genome, logfp=logfp)
 
             if source is None:
-                # The lack of a source is logged by self._sourceInfo.
+                # The lack of a source is logged by getSourceInfo.
                 continue
 
             genomeLength = len(str(genome.seq))
 
             if logfp:
                 print('\n%s: %s' % (genome.id, genome.description), file=logfp)
                 print('  length = %d' % genomeLength, file=logfp)
@@ -1761,15 +1760,15 @@
     def addGenome(self, genome, source, taxonomyId, proteinCount, databaseName,
                   duplicationPolicy='error', logfp=None):
         """
         Add information about a genome to the genomes table.
 
         @param genome: A GenBank genome record, as parsed by SeqIO.parse
         @param source: A C{dict} containing genome source information, as
-            returned by C{self._sourceInfo}.
+            returned by C{getSourceInfo}.
         @param taxonomyId: Either an C{int} taxonomy id or C{None} if the
             genome taxonomy could not be looked up.
         @param proteinCount: The C{int} number of proteins in the genome.
         @param databaseName: A C{str} indicating the database the records
             in C{filename} came from (e.g., 'refseq' or 'RVDB').
         @param duplicationPolicy: A C{str} indicating what to do if a
             to-be-inserted accession number is already present in the database.
@@ -1823,15 +1822,15 @@
         write out their sequences to the proteins FASTA file (in
         C{self._fastaFp}).
 
         @param genome: Either a GenBank genome record, as parsed by
             C{SeqIO.parse} or a C{_Genome} instance (which behaves like the
             former).
         @param source: A C{dict} containing genome source information, as
-            returned by C{self._sourceInfo}.
+            returned by C{getSourceInfo}.
         @param proteinSource: A C{str} giving the source of the protein
             accession number. This becomes part of the sequence id printed
             in the protein FASTA output.
         @param genomeSource: A C{str} giving the source of the genome
             accession number. This becomes part of the sequence id printed
             in the protein FASTA output.
         @param duplicationPolicy: A C{str} indicating what to do if a
@@ -1929,193 +1928,28 @@
             else:
                 raise
         else:
             if logfp:
                 print('    Protein %s: genome=%s product=%s' % (
                     accession, genomeAccession, product), file=logfp)
 
-    def _sourceInfo(self, genome, logfp):
-        """
-        Extract summary information from a genome source feature.
-
-        @param genome: A GenBank genome record, as parsed by SeqIO.parse
-        @param logfp: If not C{None}, a file pointer to write verbose
-            progress output to.
-        @return: A C{dict} with keys for the various pieces of information
-            (if any) found in the source feature (see the return value below
-            for detail). Or C{None} if no source feature is found or a source
-            feature does not have length 1.
-        """
-        result = {}
-
-        for feature in genome.features:
-            if feature.type == 'source':
-                for key in 'host', 'note', 'organism', 'mol_type':
-                    try:
-                        values = feature.qualifiers[key]
-                    except KeyError:
-                        value = None
-                        if key != 'note':
-                            print('Genome %r (accession %s) source info has '
-                                  'no %r feature.' %
-                                  (genome.description, genome.id, key),
-                                  file=logfp)
-                    else:
-                        if len(values) == 1:
-                            value = values[0]
-
-                            if key == 'mol_type':
-                                assert value[-3:] in ('DNA', 'RNA')
-
-                        elif len(values) > 1 and key == 'host':
-                            value = ', '.join(values)
-                        else:
-                            print('Genome %r (accession %s) has source '
-                                  'feature %r with length != 1: %r' % (
-                                      genome.description, genome.id, key,
-                                      values), file=logfp)
-                            return
-
-                    result[key] = value
-                break
-        else:
-            print('Genome %r (accession %s) had no source feature! '
-                  'Skipping.' % (genome.description, genome.id), file=logfp)
-            return
-
-        return result
-
-    def _cdsInfo(self, genome, feature, logfp=None):
-        """
-        Extract summary information from a genome CDS feature.
-
-        @param genome: A GenBank genome record, as parsed by SeqIO.parse
-        @param feature: A feature from a genome, as produced by BioPython's
-            GenBank parser.
-        @param logfp: If not C{None}, a file pointer to write verbose
-            progress output to.
-        @return: A C{dict} with keys for the various pieces of information
-            found in the feature (see the return value below for detail).
-            Or C{None} if the feature is not of interest or otherwise invalid.
-        """
-        qualifiers = feature.qualifiers
-
-        # Check in advance that all feature qualifiers we're interested in
-        # have the right lengths, if they're present.
-        for key in 'gene', 'note', 'product', 'protein_id', 'translation':
-            if key in qualifiers:
-                assert len(qualifiers[key]) == 1, (
-                    'GenBank qualifier key %s is not length one %r' %
-                    (key, qualifiers[key]))
-
-        # A protein id is mandatory.
-        if 'protein_id' in qualifiers:
-            proteinId = qualifiers['protein_id'][0]
-        else:
-            if 'translation' in qualifiers:
-                warn('Genome %r (accession %s) has CDS feature with no '
-                     'protein_id feature but has a translation! '
-                     'Skipping.\nFeature: %s' %
-                     (genome.description, genome.id, feature))
-            return
-
-        # A translated (i.e., amino acid) sequence is mandatory.
-        if 'translation' in qualifiers:
-            translation = qualifiers['translation'][0]
-        else:
-            warn('Genome %r (accession %s) has CDS feature with protein '
-                 '%r with no translated sequence. Skipping.' %
-                 (genome.description, genome.id, proteinId))
-            return
-
-        featureLocation = str(feature.location)
-
-        # Make sure the feature's location string can be parsed.
-        try:
-            ranges = GenomeRanges(featureLocation)
-        except ValueError as e:
-            warn('Genome %r  (accession %s) contains unparseable CDS '
-                 'location for protein %r. Skipping. Error: %s' %
-                 (genome.description, genome.id, proteinId, e))
-            return
-        else:
-            # Does the protein span the end of the genome? This indicates a
-            # circular genome.
-            circular = int(ranges.circular(len(genome.seq)))
-
-        if feature.location.start >= feature.location.end:
-            warn('Genome %r (accession %s) contains feature with start '
-                 '(%d) >= stop (%d). Skipping.\nFeature: %s' %
-                 (genome.description, genome.id, feature.location.start,
-                  feature.location.end, feature))
-            return
-
-        strand = feature.strand
-        if strand is None:
-            # The strands of the protein in the genome are not all the same
-            # (see Bio.SeqFeature.CompoundLocation._get_strand).  The
-            # protein is formed by the combination of reading one strand in
-            # one direction and the other in the other direction.
-            #
-            # This occurs just once in all 1.17M proteins found in all 700K
-            # RVDB (C-RVDBv15.1) genomes, for protein YP_656697.1 on the
-            # Ranid herpesvirus 1 strain McKinnell genome (NC_008211.1).
-            #
-            # This situation makes turning DIAMOND protein output into
-            # SAM very complicated because a match on such a protein
-            # cannot be stored as a SAM linear alignment. It instead
-            # requires a multi-line 'supplementary' alignment. The code
-            # and tests for that are more complex than I want to deal
-            # with at the moment, just for the sake of one protein in a
-            # frog herpesvirus.
-            warn('Genome %s (accession %s) has protein %r with mixed '
-                 'orientation!' % (genome.description, genome.id,
-                                   proteinId))
-            return
-        elif strand == 0:
-            # This never occurs for proteins corresponding to genomes in
-            # the RVDB database C-RVDBv15.1.
-            warn('Genome %r (accession %s) has protein %r with feature '
-                 'with strand of zero!' %
-                 (genome.description, genome.id, proteinId))
-            return
-        else:
-            assert strand in (1, -1)
-            forward = strand == 1
-            # Make sure the strand agrees with the orientations in the
-            # string BioPython makes out of the locations.
-            assert ranges.orientations() == {forward}
-
-        return {
-            'circular': circular,
-            'featureLocation': featureLocation,
-            'forward': forward,
-            'gene': qualifiers.get('gene', [''])[0],
-            'note': qualifiers.get('note', [''])[0],
-            'product': qualifiers.get('product', ['UNKNOWN'])[0],
-            'proteinId': proteinId,
-            'ranges': ranges,
-            'strand': strand,
-            'translation': translation,
-        }
-
     def _genomeProteins(self, genome, logfp=None):
         """
         Get proteins (CDS features) that we can process from a genome, along
         with information extracted from each.
 
         @param genome: A GenBank genome record, as parsed by SeqIO.parse
         @param logfp: If not C{None}, a file pointer to write verbose
             progress output to.
         @return: A generator yielding feature info C{dict}s as returned by
-            C{self._cdsInfo}.
+            C{getCDSInfo}.
         """
         for feature in genome.features:
             if feature.type == 'CDS':
-                featureInfo = self._cdsInfo(genome, feature, logfp=None)
+                featureInfo = getCDSInfo(genome, feature)
                 if featureInfo:
                     yield featureInfo
 
     def close(self):
         """
         Create indices on the accesssion ids and close the connection.
         """
```

### Comparing `dark-matter-4.0.8/dark/codonDistance.py` & `dark-matter-4.0.9/dark/codonDistance.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/colors.py` & `dark-matter-4.0.9/dark/colors.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/consensus.py` & `dark-matter-4.0.9/dark/consensus.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/diamond/alignments.py` & `dark-matter-4.0.9/dark/diamond/alignments.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/diamond/conversion.py` & `dark-matter-4.0.9/dark/diamond/conversion.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/diamond/hsp.py` & `dark-matter-4.0.9/dark/diamond/hsp.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/diamond/run.py` & `dark-matter-4.0.9/dark/diamond/run.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/diamond/sam.py` & `dark-matter-4.0.9/dark/diamond/sam.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/dimension.py` & `dark-matter-4.0.9/dark/dimension.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/distance.py` & `dark-matter-4.0.9/dark/distance.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/dna.py` & `dark-matter-4.0.9/dark/dna.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/entrez.py` & `dark-matter-4.0.9/dark/entrez.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/fasta.py` & `dark-matter-4.0.9/dark/fasta.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/fasta_ss.py` & `dark-matter-4.0.9/dark/fasta_ss.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/fastq.py` & `dark-matter-4.0.9/dark/fastq.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/features.py` & `dark-matter-4.0.9/dark/features.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/filter.py` & `dark-matter-4.0.9/dark/filter.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/fpcache.py` & `dark-matter-4.0.9/dark/fpcache.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/genomes.py` & `dark-matter-4.0.9/dark/genomes.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/graphics.py` & `dark-matter-4.0.9/dark/graphics.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/hsp.py` & `dark-matter-4.0.9/dark/hsp.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/html.py` & `dark-matter-4.0.9/dark/html.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/intervals.py` & `dark-matter-4.0.9/dark/intervals.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/ipynb.py` & `dark-matter-4.0.9/dark/ipynb.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/local_align.py` & `dark-matter-4.0.9/dark/local_align.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/mutations.py` & `dark-matter-4.0.9/dark/mutations.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/ncbidb.py` & `dark-matter-4.0.9/dark/ncbidb.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/orfs.py` & `dark-matter-4.0.9/dark/orfs.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/process.py` & `dark-matter-4.0.9/dark/process.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/proteins.py` & `dark-matter-4.0.9/dark/proteins.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/reads.py` & `dark-matter-4.0.9/dark/reads.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/sam.py` & `dark-matter-4.0.9/dark/sam.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/score.py` & `dark-matter-4.0.9/dark/score.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/sequence.py` & `dark-matter-4.0.9/dark/sequence.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/simplify.py` & `dark-matter-4.0.9/dark/simplify.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/summarize.py` & `dark-matter-4.0.9/dark/summarize.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/taxonomy.py` & `dark-matter-4.0.9/dark/taxonomy.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/titles.py` & `dark-matter-4.0.9/dark/titles.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark/utils.py` & `dark-matter-4.0.9/dark/utils.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/dark_matter.egg-info/PKG-INFO` & `dark-matter-4.0.9/dark_matter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dark-matter
-Version: 4.0.8
+Version: 4.0.9
 Summary: Python classes for working with genetic sequence data
 Home-page: https://github.com/acorg/dark-matter
 Author: Terry Jones, Barbara Mühlemann, Tali Veith, Sophie Mathias, Udo Gieraths
 Author-email: tcj25@cam.ac.uk
 License: MIT
 Download-URL: https://github.com/acorg/dark-matter
 Description: UNKNOWN
```

### Comparing `dark-matter-4.0.8/dark_matter.egg-info/SOURCES.txt` & `dark-matter-4.0.9/dark_matter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/setup.py` & `dark-matter-4.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_aa.py` & `dark-matter-4.0.9/test/test_aa.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_alignments.py` & `dark-matter-4.0.9/test/test_alignments.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_analyze_reads.py` & `dark-matter-4.0.9/test/test_analyze_reads.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_bowtie2.py` & `dark-matter-4.0.9/test/test_bowtie2.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_btop.py` & `dark-matter-4.0.9/test/test_btop.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_cigar.py` & `dark-matter-4.0.9/test/test_cigar.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_codonDistance.py` & `dark-matter-4.0.9/test/test_codonDistance.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_colors.py` & `dark-matter-4.0.9/test/test_colors.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_dimension.py` & `dark-matter-4.0.9/test/test_dimension.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_distance.py` & `dark-matter-4.0.9/test/test_distance.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_dna.py` & `dark-matter-4.0.9/test/test_dna.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_fasta.py` & `dark-matter-4.0.9/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_fasta_ss.py` & `dark-matter-4.0.9/test/test_fasta_ss.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_fastq.py` & `dark-matter-4.0.9/test/test_fastq.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_features.py` & `dark-matter-4.0.9/test/test_features.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_filter.py` & `dark-matter-4.0.9/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_genbank.py` & `dark-matter-4.0.9/test/test_genbank.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_genomes.py` & `dark-matter-4.0.9/test/test_genomes.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_graphics.py` & `dark-matter-4.0.9/test/test_graphics.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_hsp.py` & `dark-matter-4.0.9/test/test_hsp.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_html.py` & `dark-matter-4.0.9/test/test_html.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_intervals.py` & `dark-matter-4.0.9/test/test_intervals.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_local_align.py` & `dark-matter-4.0.9/test/test_local_align.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_mutations.py` & `dark-matter-4.0.9/test/test_mutations.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_orfs.py` & `dark-matter-4.0.9/test/test_orfs.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_process.py` & `dark-matter-4.0.9/test/test_process.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_proteins.py` & `dark-matter-4.0.9/test/test_proteins.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_reads.py` & `dark-matter-4.0.9/test/test_reads.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_sam.py` & `dark-matter-4.0.9/test/test_sam.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_score.py` & `dark-matter-4.0.9/test/test_score.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_sequence.py` & `dark-matter-4.0.9/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_simplify.py` & `dark-matter-4.0.9/test/test_simplify.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_summarize.py` & `dark-matter-4.0.9/test/test_summarize.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_taxonomy.py` & `dark-matter-4.0.9/test/test_taxonomy.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_titles.py` & `dark-matter-4.0.9/test/test_titles.py`

 * *Files identical despite different names*

### Comparing `dark-matter-4.0.8/test/test_utils.py` & `dark-matter-4.0.9/test/test_utils.py`

 * *Files identical despite different names*

