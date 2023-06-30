# Comparing `tmp/receptor_digger-0.5.3.tar.gz` & `tmp/receptor_digger-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptor_digger-0.5.3.tar", last modified: Thu Jun 29 10:13:20 2023, max compression
+gzip compressed data, was "receptor_digger-0.5.4.tar", last modified: Fri Jun 30 12:40:30 2023, max compression
```

## Comparing `receptor_digger-0.5.3.tar` & `receptor_digger-0.5.4.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.085569 receptor_digger-0.5.3/
--rw-rw-rw-   0        0        0      582 2023-03-27 14:56:02.000000 receptor_digger-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1121 2023-06-29 10:13:20.086568 receptor_digger-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-06-29 10:12:31.000000 receptor_digger-0.5.3/README.md
--rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_digger-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0     1218 2023-06-29 10:13:20.087568 receptor_digger-0.5.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.850944 receptor_digger-0.5.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.986403 receptor_digger-0.5.3/src/digger/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:47:31.000000 receptor_digger-0.5.3/src/digger/__init__.py
--rw-rw-rw-   0        0        0     1364 2023-03-29 15:03:23.000000 receptor_digger-0.5.3/src/digger/blastresults_to_csv.py
--rw-rw-rw-   0        0        0     3812 2023-03-26 08:44:02.000000 receptor_digger-0.5.3/src/digger/calc_motifs.py
--rw-rw-rw-   0        0        0     2169 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/cirelli_contig_matches.py
--rw-rw-rw-   0        0        0      344 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/cirelli_to_fasta.py
--rw-rw-rw-   0        0        0    12754 2023-04-06 10:39:17.000000 receptor_digger-0.5.3/src/digger/compare_annotations.py
--rw-rw-rw-   0        0        0     9824 2023-06-27 10:55:29.000000 receptor_digger-0.5.3/src/digger/dig_sequence.py
--rw-rw-rw-   0        0        0    14103 2023-06-28 10:25:18.000000 receptor_digger-0.5.3/src/digger/dig_utils.py
--rw-rw-rw-   0        0        0     8440 2023-03-28 08:13:03.000000 receptor_digger-0.5.3/src/digger/digger.py
--rw-rw-rw-   0        0        0    18523 2023-06-29 09:28:28.000000 receptor_digger-0.5.3/src/digger/find_alignments.py
--rw-rw-rw-   0        0        0     3429 2023-03-26 08:44:02.000000 receptor_digger-0.5.3/src/digger/motif.py
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.848944 receptor_digger-0.5.3/src/digger/motifs/
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.848944 receptor_digger-0.5.3/src/digger/motifs/human/
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.001404 receptor_digger-0.5.3/src/digger/motifs/human/IGH/
--rw-rw-rw-   0        0        0      209 2023-03-20 09:36:55.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      267 2023-03-20 09:36:55.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      209 2023-03-20 09:36:54.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      269 2023-03-20 09:36:54.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      225 2023-03-20 09:36:53.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      280 2023-03-20 09:36:54.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1409 2023-03-20 09:36:57.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      334 2023-03-20 09:36:58.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      225 2023-03-20 09:36:58.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      281 2023-03-20 09:36:58.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-04-06 10:56:41.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.013403 receptor_digger-0.5.3/src/digger/motifs/human/IGK/
--rw-rw-rw-   0        0        0      225 2023-03-22 14:52:39.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-03-22 14:52:39.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1481 2023-03-22 14:52:40.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      341 2023-03-22 14:52:40.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/L-PART2_prob.csv
--rw-rw-rw-   0        0        0   152815 2023-03-22 14:52:37.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv
--rw-rw-rw-   0        0        0      194 2023-03-22 14:52:40.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      234 2023-03-22 14:52:40.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.023444 receptor_digger-0.5.3/src/digger/motifs/human/IGL/
--rw-rw-rw-   0        0        0      222 2023-03-23 17:10:50.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      280 2023-03-23 17:10:50.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1410 2023-03-23 10:57:55.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      339 2023-03-23 10:57:56.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      225 2023-03-23 10:57:56.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-03-23 10:57:56.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.850944 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.039562 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/
--rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1288 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      320 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      165 2023-04-04 14:13:25.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.057825 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/
--rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      890 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv
--rw-rw-rw-   0        0        0     1463 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      319 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      210 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      271 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0       90 2023-04-04 10:42:00.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/conserved_motifs.fasta
--rw-rw-rw-   0        0        0     8433 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/features.csv
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.074825 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/
--rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1397 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      339 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0       90 2023-04-04 11:10:35.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/conserved_motifs.fasta
--rw-rw-rw-   0        0        0     7674 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/features.csv
--rw-rw-rw-   0        0        0    40658 2023-06-28 10:49:28.000000 receptor_digger-0.5.3/src/digger/parse_genes.py
--rw-rw-rw-   0        0        0    14499 2023-04-01 08:42:36.000000 receptor_digger-0.5.3/src/digger/parse_imgt_annotations.py
--rw-rw-rw-   0        0        0    12271 2023-06-27 11:37:05.000000 receptor_digger-0.5.3/src/digger/search_motifs.py
--rw-rw-rw-   0        0        0      856 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/slugify.py
-drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.084569 receptor_digger-0.5.3/src/receptor_digger.egg-info/
--rw-rw-rw-   0        0        0     1121 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4011 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      338 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.766244 receptor_digger-0.5.4/
+-rw-rw-rw-   0        0        0      582 2023-03-27 14:56:02.000000 receptor_digger-0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1199 2023-06-30 12:40:30.766244 receptor_digger-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-06-30 12:39:43.000000 receptor_digger-0.5.4/README.md
+-rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_digger-0.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1218 2023-06-30 12:40:30.767245 receptor_digger-0.5.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.643095 receptor_digger-0.5.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.670096 receptor_digger-0.5.4/src/digger/
+-rw-rw-rw-   0        0        0        0 2023-03-13 09:47:31.000000 receptor_digger-0.5.4/src/digger/__init__.py
+-rw-rw-rw-   0        0        0     1364 2023-03-29 15:03:23.000000 receptor_digger-0.5.4/src/digger/blastresults_to_csv.py
+-rw-rw-rw-   0        0        0     3812 2023-03-26 08:44:02.000000 receptor_digger-0.5.4/src/digger/calc_motifs.py
+-rw-rw-rw-   0        0        0     2169 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/cirelli_contig_matches.py
+-rw-rw-rw-   0        0        0      344 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/cirelli_to_fasta.py
+-rw-rw-rw-   0        0        0    12754 2023-04-06 10:39:17.000000 receptor_digger-0.5.4/src/digger/compare_annotations.py
+-rw-rw-rw-   0        0        0     9824 2023-06-29 17:40:47.000000 receptor_digger-0.5.4/src/digger/dig_sequence.py
+-rw-rw-rw-   0        0        0    14074 2023-06-30 09:34:38.000000 receptor_digger-0.5.4/src/digger/dig_utils.py
+-rw-rw-rw-   0        0        0     8440 2023-03-28 08:13:03.000000 receptor_digger-0.5.4/src/digger/digger.py
+-rw-rw-rw-   0        0        0    18523 2023-06-29 17:40:47.000000 receptor_digger-0.5.4/src/digger/find_alignments.py
+-rw-rw-rw-   0        0        0     3429 2023-03-26 08:44:02.000000 receptor_digger-0.5.4/src/digger/motif.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.642218 receptor_digger-0.5.4/src/digger/motifs/
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.642094 receptor_digger-0.5.4/src/digger/motifs/human/
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.686095 receptor_digger-0.5.4/src/digger/motifs/human/IGH/
+-rw-rw-rw-   0        0        0      209 2023-03-20 09:36:55.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      267 2023-03-20 09:36:55.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      209 2023-03-20 09:36:54.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      269 2023-03-20 09:36:54.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      225 2023-03-20 09:36:53.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      280 2023-03-20 09:36:54.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1409 2023-03-20 09:36:57.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      334 2023-03-20 09:36:58.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      225 2023-03-20 09:36:58.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      281 2023-03-20 09:36:58.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-04-06 10:56:41.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGH/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.698094 receptor_digger-0.5.4/src/digger/motifs/human/IGK/
+-rw-rw-rw-   0        0        0      225 2023-03-22 14:52:39.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGK/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-03-22 14:52:39.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGK/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1481 2023-03-22 14:52:40.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGK/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      341 2023-03-22 14:52:40.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGK/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0   152815 2023-03-22 14:52:37.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv
+-rw-rw-rw-   0        0        0      194 2023-03-22 14:52:40.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGK/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      234 2023-03-22 14:52:40.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGK/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGK/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.708093 receptor_digger-0.5.4/src/digger/motifs/human/IGL/
+-rw-rw-rw-   0        0        0      222 2023-03-23 17:10:50.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGL/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      280 2023-03-23 17:10:50.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGL/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1410 2023-03-23 10:57:55.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGL/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      339 2023-03-23 10:57:56.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGL/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      225 2023-03-23 10:57:56.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGL/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-03-23 10:57:56.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGL/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.4/src/digger/motifs/human/IGL/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.643095 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.722869 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/
+-rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1288 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      320 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      165 2023-04-04 14:13:25.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.740244 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/
+-rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      890 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv
+-rw-rw-rw-   0        0        0     1463 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      319 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      210 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      271 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0       90 2023-04-04 10:42:00.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0     8433 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/features.csv
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.757244 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/
+-rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1397 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      339 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0       90 2023-04-04 11:10:35.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0     7674 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/features.csv
+-rw-rw-rw-   0        0        0    40654 2023-06-30 09:35:41.000000 receptor_digger-0.5.4/src/digger/parse_genes.py
+-rw-rw-rw-   0        0        0    14499 2023-04-01 08:42:36.000000 receptor_digger-0.5.4/src/digger/parse_imgt_annotations.py
+-rw-rw-rw-   0        0        0    12271 2023-06-29 17:40:47.000000 receptor_digger-0.5.4/src/digger/search_motifs.py
+-rw-rw-rw-   0        0        0      856 2023-02-06 16:38:59.000000 receptor_digger-0.5.4/src/digger/slugify.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:40:30.764245 receptor_digger-0.5.4/src/receptor_digger.egg-info/
+-rw-rw-rw-   0        0        0     1199 2023-06-30 12:40:30.000000 receptor_digger-0.5.4/src/receptor_digger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4011 2023-06-30 12:40:30.000000 receptor_digger-0.5.4/src/receptor_digger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 12:40:30.000000 receptor_digger-0.5.4/src/receptor_digger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      338 2023-06-30 12:40:30.000000 receptor_digger-0.5.4/src/receptor_digger.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-06-30 12:40:30.000000 receptor_digger-0.5.4/src/receptor_digger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 12:40:30.000000 receptor_digger-0.5.4/src/receptor_digger.egg-info/top_level.txt
```

### Comparing `receptor_digger-0.5.3/MANIFEST.in` & `receptor_digger-0.5.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/PKG-INFO` & `receptor_digger-0.5.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receptor_digger
-Version: 0.5.3
+Version: 0.5.4
 Summary: Tools for de novo discovery of genomic germline IG and TR receptor sequences
 Home-page: https://github.com/williamdlees/digger
 Author: William Lees
 Author-email: william@lees.org.uk
 Project-URL: Bug Tracker, https://github.com/williamdlees/digger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -13,13 +13,16 @@
 Description-Content-Type: text/markdown
 
 # Digger
 A toolkit for the automatic annotation of V,D and J genes and associated features in IG receptor genomic loci.
 
 For more details, please see the [documentation](https://williamdlees.github.io/digger/index.html).
 
+Changes in V 0.5.4:
+- Minor fixes to handling of non-functional sequences
+
 Changes in V 0.5.3:
 - Fixes to annotation in reverse-sense: false positives were not being filtered correctly
 - Introduction of dig_sequence: targeted annotation of an identified sequence
 
 Changes in V 0.5.1:
 - (internal only) - Refactored elements of the code to make it more modular and easier to maintain.
```

### Comparing `receptor_digger-0.5.3/README.md` & `receptor_digger-0.5.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Digger
 A toolkit for the automatic annotation of V,D and J genes and associated features in IG receptor genomic loci.
 
 For more details, please see the [documentation](https://williamdlees.github.io/digger/index.html).
 
+Changes in V 0.5.4:
+- Minor fixes to handling of non-functional sequences
+
 Changes in V 0.5.3:
 - Fixes to annotation in reverse-sense: false positives were not being filtered correctly
 - Introduction of dig_sequence: targeted annotation of an identified sequence
 
 Changes in V 0.5.1:
 - (internal only) - Refactored elements of the code to make it more modular and easier to maintain.
```

### Comparing `receptor_digger-0.5.3/setup.cfg` & `receptor_digger-0.5.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6563 6570 746f 725f 6469 6767   = receptor_digg
 00000020: 6572 0d0a 7665 7273 696f 6e20 3d20 302e  er..version = 0.
-00000030: 352e 330d 0a61 7574 686f 7220 3d20 5769  5.3..author = Wi
+00000030: 352e 340d 0a61 7574 686f 7220 3d20 5769  5.4..author = Wi
 00000040: 6c6c 6961 6d20 4c65 6573 0d0a 6175 7468  lliam Lees..auth
 00000050: 6f72 5f65 6d61 696c 203d 2077 696c 6c69  or_email = willi
 00000060: 616d 406c 6565 732e 6f72 672e 756b 0d0a  am@lees.org.uk..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 546f  description = To
 00000080: 6f6c 7320 666f 7220 6465 206e 6f76 6f20  ols for de novo 
 00000090: 6469 7363 6f76 6572 7920 6f66 2067 656e  discovery of gen
 000000a0: 6f6d 6963 2067 6572 6d6c 696e 6520 4947  omic germline IG
```

### Comparing `receptor_digger-0.5.3/src/digger/blastresults_to_csv.py` & `receptor_digger-0.5.4/src/digger/blastresults_to_csv.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/calc_motifs.py` & `receptor_digger-0.5.4/src/digger/calc_motifs.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/cirelli_contig_matches.py` & `receptor_digger-0.5.4/src/digger/cirelli_contig_matches.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/compare_annotations.py` & `receptor_digger-0.5.4/src/digger/compare_annotations.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/dig_sequence.py` & `receptor_digger-0.5.4/src/digger/dig_sequence.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/dig_utils.py` & `receptor_digger-0.5.4/src/digger/dig_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,20 +219,20 @@
                 'gene_start': start + 1,
                 'gene_end': end,
                 'gene_end_rev': rev_start,
                 'gene_start_rev': rev_end,
                 'notes': "Sequence to be annotated does not contain recognisable 3' or 5' regulatory regions",
                 'functional': row['functional']
             }
-        else:
-            nt_diff = min(diffs)
-            start, end, score = find_target_sequence(row['seq'], target_seq, 'local')
 
-            score = (100*score)/(2*len(target_seq))
-            score = round(score, 1)
+        nt_diff = min(diffs)
+        start, end, score = find_target_sequence(row['seq'], target_seq, 'local')
+
+        score = (100*score)/(2*len(target_seq))
+        score = round(score, 1)
 
     row['target_allele'] = target
     row['genbank_acc'] = genbank_acc
     row['patch'] = patch
     row['genbank_seq'] = assembly
     row['alignment_score'] = score
     row['sense'] = sense
```

### Comparing `receptor_digger-0.5.3/src/digger/digger.py` & `receptor_digger-0.5.4/src/digger/digger.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/find_alignments.py` & `receptor_digger-0.5.4/src/digger/find_alignments.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motif.py` & `receptor_digger-0.5.4/src/digger/motif.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/human/IGH/L-PART1_prob.csv` & `receptor_digger-0.5.4/src/digger/motifs/human/IGH/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/human/IGK/L-PART1_prob.csv` & `receptor_digger-0.5.4/src/digger/motifs/human/IGK/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv` & `receptor_digger-0.5.4/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/human/IGL/L-PART1_prob.csv` & `receptor_digger-0.5.4/src/digger/motifs/human/IGL/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv` & `receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv` & `receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv` & `receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/features.csv` & `receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGK/features.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv` & `receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/features.csv` & `receptor_digger-0.5.4/src/digger/motifs/rhesus_macaque/IGL/features.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/parse_genes.py` & `receptor_digger-0.5.4/src/digger/parse_genes.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,15 +703,15 @@
             v_annot.annotate()
             v_annot.likelihood = left.likelihood * right.likelihood
 
             if v_annot.functionality == 'Functional':
                 results.append((left, v_annot, right))
             if max_likelihood_rec is None or v_annot.likelihood > max_likelihood_rec[1].likelihood:
                 max_likelihood_rec = (left, v_annot, right)
-            if v_annot.start == start + 1 and (max_likelihood_rec_at_start is None or v_annot.likelihood > max_likelihood_rec[1].likelihood):
+            if v_annot.start == start and (max_likelihood_rec_at_start is None or v_annot.likelihood > max_likelihood_rec[1].likelihood):
                 max_likelihood_rec_at_start = (left, v_annot, right)
 
     # If we don't have any functional results, favour the one with the suggested start position.
     if len(results) == 0 and max_likelihood_rec_at_start is not None:
         results = [max_likelihood_rec_at_start]
 
     if len(results) == 0 and max_likelihood_rec is not None:
```

### Comparing `receptor_digger-0.5.3/src/digger/parse_imgt_annotations.py` & `receptor_digger-0.5.4/src/digger/parse_imgt_annotations.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/search_motifs.py` & `receptor_digger-0.5.4/src/digger/search_motifs.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/digger/slugify.py` & `receptor_digger-0.5.4/src/digger/slugify.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.3/src/receptor_digger.egg-info/PKG-INFO` & `receptor_digger-0.5.4/src/receptor_digger.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receptor-digger
-Version: 0.5.3
+Version: 0.5.4
 Summary: Tools for de novo discovery of genomic germline IG and TR receptor sequences
 Home-page: https://github.com/williamdlees/digger
 Author: William Lees
 Author-email: william@lees.org.uk
 Project-URL: Bug Tracker, https://github.com/williamdlees/digger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -13,13 +13,16 @@
 Description-Content-Type: text/markdown
 
 # Digger
 A toolkit for the automatic annotation of V,D and J genes and associated features in IG receptor genomic loci.
 
 For more details, please see the [documentation](https://williamdlees.github.io/digger/index.html).
 
+Changes in V 0.5.4:
+- Minor fixes to handling of non-functional sequences
+
 Changes in V 0.5.3:
 - Fixes to annotation in reverse-sense: false positives were not being filtered correctly
 - Introduction of dig_sequence: targeted annotation of an identified sequence
 
 Changes in V 0.5.1:
 - (internal only) - Refactored elements of the code to make it more modular and easier to maintain.
```

### Comparing `receptor_digger-0.5.3/src/receptor_digger.egg-info/SOURCES.txt` & `receptor_digger-0.5.4/src/receptor_digger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

