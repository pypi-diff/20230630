# Comparing `tmp/slabbe-0.7.tar.gz` & `tmp/slabbe-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slabbe-0.7.tar", last modified: Thu Dec  8 19:41:28 2022, max compression
+gzip compressed data, was "dist/slabbe-0.7.1.tar", last modified: Fri Jun 30 09:57:24 2023, max compression
```

## Comparing `slabbe-0.7.tar` & `slabbe-0.7.1.tar`

### file list

```diff
@@ -1,127 +1,130 @@
-drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2022-12-08 19:41:28.384348 slabbe-0.7/
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      315 2022-02-04 10:01:29.000000 slabbe-0.7/.gitignore
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2426 2022-11-10 10:25:43.000000 slabbe-0.7/.gitlab-ci.yml
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    18025 2017-10-12 11:54:33.000000 slabbe-0.7/LICENSE
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)       19 2018-10-19 21:34:23.000000 slabbe-0.7/MANIFEST.in
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10875 2022-12-08 19:41:28.384348 slabbe-0.7/PKG-INFO
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10252 2022-12-08 19:30:18.000000 slabbe-0.7/README.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     3968 2022-02-04 10:01:29.000000 slabbe-0.7/TODO.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)        4 2022-12-08 19:15:35.000000 slabbe-0.7/VERSION
-drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2022-12-08 19:41:28.372348 slabbe-0.7/demos/
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     5624 2022-02-04 10:01:29.000000 slabbe-0.7/demos/2018-03-22-ekekstar-minervino.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)   586631 2018-10-19 21:34:23.000000 slabbe-0.7/demos/Diophantine Approximation and MCF algorithms.ipynb
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     7844 2022-11-06 09:57:16.000000 slabbe-0.7/demos/arXiv_1802_03265.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     5286 2022-11-06 09:57:16.000000 slabbe-0.7/demos/arXiv_1808_07768_part1.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     7608 2022-02-04 10:01:29.000000 slabbe-0.7/demos/arXiv_1808_07768_part2.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    16445 2022-02-04 10:01:29.000000 slabbe-0.7/demos/arXiv_1906_01104.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     8537 2022-02-04 10:01:29.000000 slabbe-0.7/demos/chapter_three_characterizations.rst
-drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2022-12-08 19:41:28.372348 slabbe-0.7/docs/
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     6771 2018-10-19 21:34:23.000000 slabbe-0.7/docs/Makefile
-drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2022-12-08 19:41:28.376348 slabbe-0.7/docs/source/
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      174 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/EkEkstar.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      154 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/analyze_sage_build.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      208 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/arXiv_1808_07768.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      210 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/arXiv_1903_06137.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      207 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/arXiv_1906_01104.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      166 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/beta_numeration_system.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      136 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/billiard.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      169 2022-12-08 19:12:38.000000 slabbe-0.7/docs/source/billiard_nD.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      216 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/bispecial_extension_type.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      162 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/bond_percolation.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      151 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/christoffel_graph.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      218 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/coding_of_PETs.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      134 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/combinat.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10476 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/conf.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      201 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/ddim_sturmian_configuration.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      267 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/diophantine_approx.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      142 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/discrete_plane.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      145 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/discrete_subset.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      156 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/double_square_tile.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      137 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/dyck_3d.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      135 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/finite_word.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      115 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/fruit.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      117 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/graph.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      210 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/graph_directed_IFS.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     1790 2022-12-08 19:10:19.000000 slabbe-0.7/docs/source/index.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      141 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/infinite_word.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      145 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/joyal_bijection.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      241 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/kolakoski_word.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      126 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/language.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      170 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/lyapunov.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      153 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/magic_hexagon.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      165 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/markov_transformation.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      124 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/matrices.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      144 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/matrix_cocycle.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      301 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/mult_cont_frac.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      149 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/ostrowski.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      153 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/partial_injection.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      274 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/polyhedron_exchange_transformation.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      160 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/polyhedron_partition.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      181 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/ranking_scale.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      153 2022-11-06 09:57:16.000000 slabbe-0.7/docs/source/sturmian_subshift.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      147 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/substitution_2d.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      136 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/tikz_picture.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      168 2021-02-16 20:14:39.000000 slabbe-0.7/docs/source/wang_tiles.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      142 2018-10-19 21:34:23.000000 slabbe-0.7/docs/source/word_morphisms.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      144 2022-02-04 10:01:29.000000 slabbe-0.7/docs/source/write_to_file.rst
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     1043 2022-11-06 09:57:16.000000 slabbe-0.7/makefile
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)       38 2022-12-08 19:41:28.384348 slabbe-0.7/setup.cfg
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2168 2022-02-04 10:01:29.000000 slabbe-0.7/setup.py
-drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2022-12-08 19:41:28.384348 slabbe-0.7/slabbe/
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    44523 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/EkEkstar.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2761 2022-11-07 18:53:41.000000 slabbe-0.7/slabbe/__init__.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10432 2022-12-08 11:10:16.000000 slabbe-0.7/slabbe/analyze_sage_build.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    17589 2022-12-08 14:18:48.000000 slabbe-0.7/slabbe/arXiv_1808_07768.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    19030 2022-12-08 14:19:23.000000 slabbe-0.7/slabbe/arXiv_1903_06137.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     6064 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/arXiv_1906_01104.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     5669 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/beta_numeration_system.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     9514 2022-11-07 18:51:54.000000 slabbe-0.7/slabbe/billiard.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    24886 2022-11-10 09:41:40.000000 slabbe-0.7/slabbe/billiard_nD.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)   117730 2022-12-08 12:54:23.000000 slabbe-0.7/slabbe/bispecial_extension_type.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    28417 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/bond_percolation.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    11841 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/christoffel_graph.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    14900 2022-12-08 13:51:45.000000 slabbe-0.7/slabbe/coding_of_PETs.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10662 2022-12-08 14:24:42.000000 slabbe-0.7/slabbe/combinat.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    32914 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/ddim_sturmian_configuration.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    25826 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/diophantine_approx.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)   217191 2022-10-14 13:41:59.000000 slabbe-0.7/slabbe/diophantine_approx_pyx.c
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     5900 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/diophantine_approx_pyx.pyx
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     9251 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/discrete_plane.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    68311 2022-12-08 11:09:19.000000 slabbe-0.7/slabbe/discrete_subset.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    94198 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/double_square_tile.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2874 2018-10-19 21:34:23.000000 slabbe-0.7/slabbe/dyck_3d.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10889 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/finite_word.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     7133 2018-10-19 21:34:23.000000 slabbe-0.7/slabbe/fruit.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    19189 2022-12-08 10:14:51.000000 slabbe-0.7/slabbe/graph.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    32744 2022-12-08 14:20:21.000000 slabbe-0.7/slabbe/graph_directed_IFS.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     3037 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/infinite_word.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    20116 2018-10-19 21:34:23.000000 slabbe-0.7/slabbe/joyal_bijection.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     3052 2018-10-19 21:34:23.000000 slabbe-0.7/slabbe/kolakoski_word.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)   310913 2022-02-04 10:55:13.000000 slabbe-0.7/slabbe/kolakoski_word_pyx.c
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     7073 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/kolakoski_word_pyx.pyx
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    29470 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/language.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     9743 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/lyapunov.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2891 2022-12-08 14:20:57.000000 slabbe-0.7/slabbe/magic_hexagon.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    15521 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/markov_transformation.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    25685 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/matrices.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    45480 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/matrix_cocycle.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2980 2018-10-19 21:34:23.000000 slabbe-0.7/slabbe/modified_mcf.pyx.no
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    43503 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/mult_cont_frac.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)  2164367 2022-11-07 18:52:03.000000 slabbe-0.7/slabbe/mult_cont_frac_pyx.c
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    99327 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/mult_cont_frac_pyx.pyx
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     5388 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/ostrowski.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10421 2022-12-08 14:21:24.000000 slabbe-0.7/slabbe/partial_injection.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    43910 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/polyhedron_exchange_transformation.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    42584 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/polyhedron_partition.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    17569 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/ranking_scale.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     7202 2022-11-06 09:57:16.000000 slabbe-0.7/slabbe/sturmian_subshift.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    58599 2022-12-08 10:32:24.000000 slabbe-0.7/slabbe/substitution_2d.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    37991 2022-12-08 14:30:03.000000 slabbe-0.7/slabbe/tikz_picture.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)   177033 2022-12-08 10:38:05.000000 slabbe-0.7/slabbe/wang_tiles.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    15710 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/word_morphisms.py
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2174 2022-02-04 10:01:29.000000 slabbe-0.7/slabbe/write_to_file.py
-drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2022-12-08 19:41:28.384348 slabbe-0.7/slabbe.egg-info/
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10875 2022-12-08 19:41:28.000000 slabbe-0.7/slabbe.egg-info/PKG-INFO
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     3254 2022-12-08 19:41:28.000000 slabbe-0.7/slabbe.egg-info/SOURCES.txt
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)        1 2022-12-08 19:41:28.000000 slabbe-0.7/slabbe.egg-info/dependency_links.txt
--rw-rw-r--   0 slabbe    (1001) slabbe    (1001)        7 2022-12-08 19:41:28.000000 slabbe-0.7/slabbe.egg-info/top_level.txt
+drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2023-06-30 09:57:24.008878 slabbe-0.7.1/
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      315 2021-03-01 14:39:00.000000 slabbe-0.7.1/.gitignore
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2426 2022-11-28 16:57:50.000000 slabbe-0.7.1/.gitlab-ci.yml
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)    18025 2020-09-10 13:56:54.000000 slabbe-0.7.1/LICENSE
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)       19 2021-03-01 14:30:09.000000 slabbe-0.7.1/MANIFEST.in
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    11317 2023-06-30 09:57:24.008878 slabbe-0.7.1/PKG-INFO
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10692 2023-06-30 09:54:43.000000 slabbe-0.7.1/README.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     4149 2023-06-30 09:30:55.000000 slabbe-0.7.1/TODO.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)        6 2023-06-27 14:19:50.000000 slabbe-0.7.1/VERSION
+drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2023-06-30 09:57:23.992878 slabbe-0.7.1/demos/
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     5624 2021-03-01 14:39:00.000000 slabbe-0.7.1/demos/2018-03-22-ekekstar-minervino.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)   586631 2021-03-01 14:39:00.000000 slabbe-0.7.1/demos/Diophantine Approximation and MCF algorithms.ipynb
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     7826 2023-04-13 12:08:45.000000 slabbe-0.7.1/demos/arXiv_1802_03265.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     5286 2022-05-09 14:50:14.000000 slabbe-0.7.1/demos/arXiv_1808_07768_part1.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     7608 2021-03-01 14:39:00.000000 slabbe-0.7.1/demos/arXiv_1808_07768_part2.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)    16445 2021-03-01 14:39:00.000000 slabbe-0.7.1/demos/arXiv_1906_01104.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     8537 2021-03-01 14:39:00.000000 slabbe-0.7.1/demos/chapter_three_characterizations.rst
+drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2023-06-30 09:57:23.992878 slabbe-0.7.1/docs/
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     6771 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/Makefile
+drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2023-06-30 09:57:23.996878 slabbe-0.7.1/docs/source/
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      174 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/EkEkstar.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      154 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/analyze_sage_build.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      208 2021-12-10 09:26:10.000000 slabbe-0.7.1/docs/source/arXiv_1808_07768.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      210 2021-12-10 09:26:10.000000 slabbe-0.7.1/docs/source/arXiv_1903_06137.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      207 2021-12-10 09:26:10.000000 slabbe-0.7.1/docs/source/arXiv_1906_01104.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      166 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/beta_numeration_system.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      136 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/billiard.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      169 2023-03-02 13:32:54.000000 slabbe-0.7.1/docs/source/billiard_nD.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      216 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/bispecial_extension_type.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      162 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/bond_percolation.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      151 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/christoffel_graph.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      218 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/coding_of_PETs.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      134 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/combinat.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10476 2021-12-10 09:26:10.000000 slabbe-0.7.1/docs/source/conf.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      201 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/ddim_sturmian_configuration.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      267 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/diophantine_approx.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      142 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/discrete_plane.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      145 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/discrete_subset.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      156 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/double_square_tile.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      137 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/dyck_3d.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      135 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/finite_word.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      115 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/fruit.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      117 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/graph.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      210 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/graph_directed_IFS.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     1790 2023-03-02 13:32:54.000000 slabbe-0.7.1/docs/source/index.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      141 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/infinite_word.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      145 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/joyal_bijection.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      241 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/kolakoski_word.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      126 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/language.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      170 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/lyapunov.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      153 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/magic_hexagon.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      165 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/markov_transformation.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      124 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/matrices.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      144 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/matrix_cocycle.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      301 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/mult_cont_frac.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      149 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/ostrowski.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      153 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/partial_injection.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      274 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/polyhedron_exchange_transformation.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      160 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/polyhedron_partition.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      181 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/ranking_scale.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)      153 2022-01-28 16:24:57.000000 slabbe-0.7.1/docs/source/sturmian_subshift.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      147 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/substitution_2d.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      136 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/tikz_picture.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      168 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/wang_tiles.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      142 2021-03-01 14:30:09.000000 slabbe-0.7.1/docs/source/word_morphisms.rst
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)      144 2021-03-01 14:39:00.000000 slabbe-0.7.1/docs/source/write_to_file.rst
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     1044 2023-06-27 13:31:13.000000 slabbe-0.7.1/makefile
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)       38 2023-06-30 09:57:24.008878 slabbe-0.7.1/setup.cfg
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2168 2021-12-10 09:26:10.000000 slabbe-0.7.1/setup.py
+drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2023-06-30 09:57:24.008878 slabbe-0.7.1/slabbe/
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    44523 2022-03-24 15:34:17.000000 slabbe-0.7.1/slabbe/EkEkstar.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2979 2023-06-30 09:48:10.000000 slabbe-0.7.1/slabbe/__init__.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10432 2022-12-08 14:26:39.000000 slabbe-0.7.1/slabbe/analyze_sage_build.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    28967 2023-05-26 09:17:24.000000 slabbe-0.7.1/slabbe/aperiodic_monotile.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    17589 2022-12-08 14:26:39.000000 slabbe-0.7.1/slabbe/arXiv_1808_07768.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    19030 2022-12-08 14:26:39.000000 slabbe-0.7.1/slabbe/arXiv_1903_06137.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     6064 2021-12-10 09:26:10.000000 slabbe-0.7.1/slabbe/arXiv_1906_01104.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     5669 2021-07-12 12:00:43.000000 slabbe-0.7.1/slabbe/beta_numeration_system.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     9514 2022-11-07 14:45:42.000000 slabbe-0.7.1/slabbe/billiard.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    24886 2022-11-08 09:16:50.000000 slabbe-0.7.1/slabbe/billiard_nD.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)   117712 2023-04-13 12:08:45.000000 slabbe-0.7.1/slabbe/bispecial_extension_type.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)    28417 2021-03-01 14:39:00.000000 slabbe-0.7.1/slabbe/bond_percolation.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    11841 2022-05-09 15:44:02.000000 slabbe-0.7.1/slabbe/christoffel_graph.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    17673 2023-05-02 11:49:18.000000 slabbe-0.7.1/slabbe/coding_of_PETs.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10662 2022-12-08 14:26:39.000000 slabbe-0.7.1/slabbe/combinat.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    36259 2023-06-27 13:35:53.000000 slabbe-0.7.1/slabbe/cut_and_project_scheme.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    32914 2022-05-09 15:57:32.000000 slabbe-0.7.1/slabbe/ddim_sturmian_configuration.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    25826 2021-07-12 12:00:43.000000 slabbe-0.7.1/slabbe/diophantine_approx.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)   217191 2023-04-03 15:31:49.000000 slabbe-0.7.1/slabbe/diophantine_approx_pyx.c
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     5900 2021-07-12 12:00:43.000000 slabbe-0.7.1/slabbe/diophantine_approx_pyx.pyx
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     9251 2022-03-24 15:34:17.000000 slabbe-0.7.1/slabbe/discrete_plane.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    68311 2022-12-08 14:26:39.000000 slabbe-0.7.1/slabbe/discrete_subset.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    94198 2022-05-19 09:42:54.000000 slabbe-0.7.1/slabbe/double_square_tile.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     6202 2023-04-13 12:08:45.000000 slabbe-0.7.1/slabbe/dumont_thomas_on_Z.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     2874 2021-03-01 14:39:00.000000 slabbe-0.7.1/slabbe/dyck_3d.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)    10889 2021-03-01 14:39:00.000000 slabbe-0.7.1/slabbe/finite_word.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     7133 2021-03-01 14:39:00.000000 slabbe-0.7.1/slabbe/fruit.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    20486 2023-04-13 13:30:18.000000 slabbe-0.7.1/slabbe/graph.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    34091 2023-05-02 12:18:23.000000 slabbe-0.7.1/slabbe/graph_directed_IFS.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     3037 2021-07-12 12:00:43.000000 slabbe-0.7.1/slabbe/infinite_word.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)    20116 2021-03-01 14:39:00.000000 slabbe-0.7.1/slabbe/joyal_bijection.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     3052 2021-03-01 14:39:00.000000 slabbe-0.7.1/slabbe/kolakoski_word.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)   310913 2022-01-28 11:02:42.000000 slabbe-0.7.1/slabbe/kolakoski_word_pyx.c
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     7073 2021-12-10 09:26:10.000000 slabbe-0.7.1/slabbe/kolakoski_word_pyx.pyx
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    29470 2022-05-31 11:27:26.000000 slabbe-0.7.1/slabbe/language.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     9743 2022-05-19 09:47:34.000000 slabbe-0.7.1/slabbe/lyapunov.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     2891 2022-12-08 14:26:39.000000 slabbe-0.7.1/slabbe/magic_hexagon.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)    15521 2022-05-09 15:47:05.000000 slabbe-0.7.1/slabbe/markov_transformation.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    25685 2021-07-12 12:00:43.000000 slabbe-0.7.1/slabbe/matrices.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)    45480 2022-05-31 15:14:36.000000 slabbe-0.7.1/slabbe/matrix_cocycle.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     2980 2021-03-01 14:39:00.000000 slabbe-0.7.1/slabbe/modified_mcf.pyx.no
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    43503 2022-07-07 13:16:30.000000 slabbe-0.7.1/slabbe/mult_cont_frac.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)  2164367 2023-04-03 15:31:51.000000 slabbe-0.7.1/slabbe/mult_cont_frac_pyx.c
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    99327 2022-07-07 13:16:30.000000 slabbe-0.7.1/slabbe/mult_cont_frac_pyx.pyx
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     5388 2021-12-10 09:26:10.000000 slabbe-0.7.1/slabbe/ostrowski.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    10403 2023-04-13 12:08:45.000000 slabbe-0.7.1/slabbe/partial_injection.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    43910 2021-07-12 12:00:43.000000 slabbe-0.7.1/slabbe/polyhedron_exchange_transformation.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)    43193 2023-04-03 16:09:54.000000 slabbe-0.7.1/slabbe/polyhedron_partition.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)    17569 2021-03-01 14:39:00.000000 slabbe-0.7.1/slabbe/ranking_scale.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     7202 2022-01-28 16:24:57.000000 slabbe-0.7.1/slabbe/sturmian_subshift.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    72803 2023-05-02 11:49:41.000000 slabbe-0.7.1/slabbe/substitution_2d.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    37940 2023-06-30 09:48:37.000000 slabbe-0.7.1/slabbe/tikz_picture.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)   178341 2023-04-13 12:08:45.000000 slabbe-0.7.1/slabbe/wang_tiles.py
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    15710 2021-12-10 09:26:10.000000 slabbe-0.7.1/slabbe/word_morphisms.py
+-rw-r--r--   0 slabbe    (1001) slabbe    (1001)     2174 2021-03-01 14:39:00.000000 slabbe-0.7.1/slabbe/write_to_file.py
+drwxrwxr-x   0 slabbe    (1001) slabbe    (1001)        0 2023-06-30 09:57:24.008878 slabbe-0.7.1/slabbe.egg-info/
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)    11317 2023-06-30 09:57:23.000000 slabbe-0.7.1/slabbe.egg-info/PKG-INFO
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)     3345 2023-06-30 09:57:23.000000 slabbe-0.7.1/slabbe.egg-info/SOURCES.txt
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)        1 2023-06-30 09:57:23.000000 slabbe-0.7.1/slabbe.egg-info/dependency_links.txt
+-rw-rw-r--   0 slabbe    (1001) slabbe    (1001)        7 2023-06-30 09:57:23.000000 slabbe-0.7.1/slabbe.egg-info/top_level.txt
```

### Comparing `slabbe-0.7/.gitlab-ci.yml` & `slabbe-0.7.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/LICENSE` & `slabbe-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/PKG-INFO` & `slabbe-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slabbe
-Version: 0.7
+Version: 0.7.1
 Summary: Sebastien Labbe's Research code
 Home-page: http://gitlab.com/seblabbe/slabbe
 Author: Sebastien Labbe
 Author-email: slabbe@ulg.ac.be
 License: GPLv2+
 Keywords: sagemath combinatorics discrete geometry symbolic dynamics
 Classifier: Development Status :: 4 - Beta
@@ -24,20 +24,21 @@
 
 This is an optional package for SageMath containing code I wrote for research.
 It contains modules on the following topics.
 
 **Discrete dynamical systems**
   diophantine approximation, Markov transformations, Wang tilings, Lyapunov
   exponents, matrix cocycles, multidimensional continued fraction algorithms,
-  polyhedron exchange transformations, GIFS.
+  polyhedron exchange transformations (PETs), GIFS,
 
 **Combinatorics**
   2d substitutions, bispecial factors, bond percolation, Dyck word in 3D,
   words, Joyal bijection, languages, Oldenburger sequence, ostrowski
-  numeration, partial injections,
+  numeration, partial injections, d-dimensional Sturmian configurations,
+  hypercubic billiard words
 
 **Digital geometry**
   Christoffel graph, discrete subset, discrete plane, double square tiles,
   polyhedron partitions,
 
 **Vizualization**
   tikzpicture
@@ -181,19 +182,27 @@
 module(s) and I will create a ticket on trac__ for its inclusion into SageMath.
 
 __ https://trac.sagemath.org/
 
 Release history
 ---------------
 
+*Version 0.7.1 (June 30, 2023)*
+  New module on cut and project scheme (still preliminary).
+  New module to draw tilings with the Smith's aperiodic monotile (see this `blog post`__).
+  Few other improvements.
+  All tests passed on version 10.0 of SageMath.
+
+__ http://www.slabbe.org/blogue/2023/05/decoupe-laser-du-chapeau-tuile-aperiodique-decouverte-recemment/
+
 *Version 0.7 (December 8, 2022)*
   New module on d-dimensional Sturmian configurations, to draw figures from `arXiv:2204.06413`__.
   New module on Hypercubic billiard words (written with Mélodie Andrieu).
   The module ``TikzPicture`` got merged in SageMath 9.6 into
-  `sage.misc.latex_standalone` through ticket `#20343`__ during which many
+  ``sage.misc.latex_standalone`` through ticket `#20343`__ during which many
   improvements were made. The line ``from slabbe import TikzPicture`` now uses
   the one in SageMath by default. All tests passed on version 9.7 of SageMath.
   Up to recently, all tests passed on versions 9.0, 9.1, 9.2, 9.3 and 9.4 of SageMath;
   can't test those earlier versions of SageMath anymore because gitlab continuous
   integration tests is not free anymore.
 
 __ https://arxiv.org/abs/2204.06413
```

### Comparing `slabbe-0.7/README.rst` & `slabbe-0.7.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
 This is an optional package for SageMath containing code I wrote for research.
 It contains modules on the following topics.
 
 **Discrete dynamical systems**
   diophantine approximation, Markov transformations, Wang tilings, Lyapunov
   exponents, matrix cocycles, multidimensional continued fraction algorithms,
-  polyhedron exchange transformations, GIFS.
+  polyhedron exchange transformations (PETs), GIFS,
 
 **Combinatorics**
   2d substitutions, bispecial factors, bond percolation, Dyck word in 3D,
   words, Joyal bijection, languages, Oldenburger sequence, ostrowski
-  numeration, partial injections,
+  numeration, partial injections, d-dimensional Sturmian configurations,
+  hypercubic billiard words
 
 **Digital geometry**
   Christoffel graph, discrete subset, discrete plane, double square tiles,
   polyhedron partitions,
 
 **Vizualization**
   tikzpicture
@@ -164,19 +165,27 @@
 module(s) and I will create a ticket on trac__ for its inclusion into SageMath.
 
 __ https://trac.sagemath.org/
 
 Release history
 ---------------
 
+*Version 0.7.1 (June 30, 2023)*
+  New module on cut and project scheme (still preliminary).
+  New module to draw tilings with the Smith's aperiodic monotile (see this `blog post`__).
+  Few other improvements.
+  All tests passed on version 10.0 of SageMath.
+
+__ http://www.slabbe.org/blogue/2023/05/decoupe-laser-du-chapeau-tuile-aperiodique-decouverte-recemment/
+
 *Version 0.7 (December 8, 2022)*
   New module on d-dimensional Sturmian configurations, to draw figures from `arXiv:2204.06413`__.
   New module on Hypercubic billiard words (written with Mélodie Andrieu).
   The module ``TikzPicture`` got merged in SageMath 9.6 into
-  `sage.misc.latex_standalone` through ticket `#20343`__ during which many
+  ``sage.misc.latex_standalone`` through ticket `#20343`__ during which many
   improvements were made. The line ``from slabbe import TikzPicture`` now uses
   the one in SageMath by default. All tests passed on version 9.7 of SageMath.
   Up to recently, all tests passed on versions 9.0, 9.1, 9.2, 9.3 and 9.4 of SageMath;
   can't test those earlier versions of SageMath anymore because gitlab continuous
   integration tests is not free anymore.
 
 __ https://arxiv.org/abs/2204.06413
```

### Comparing `slabbe-0.7/TODO.rst` & `slabbe-0.7.1/TODO.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 
 ====
 TODO
 ====
 
+Update the package using setuptools and pyproject.toml
+------------------------------------------------------
+
+https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
+
 Use gitlab
 ----------
 
 https://about.gitlab.com/
 
 Transition à Python 3
 ---------------------
```

### Comparing `slabbe-0.7/demos/2018-03-22-ekekstar-minervino.rst` & `slabbe-0.7.1/demos/2018-03-22-ekekstar-minervino.rst`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/demos/Diophantine Approximation and MCF algorithms.ipynb` & `slabbe-0.7.1/demos/Diophantine Approximation and MCF algorithms.ipynb`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/demos/arXiv_1802_03265.rst` & `slabbe-0.7.1/demos/arXiv_1802_03265.rst`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ::
 
     sage: G = U.to_transducer_graph(); G
     Looped digraph on 10 vertices
     sage: t = TikzPicture.from_graph(G)
     doctest:...: FutureWarning: This class/method/function is marked as experimental.
     It, its functionality or its interface might change without a formal deprecation.
-    See http://trac.sagemath.org/20343 for details.
+    See http...20343 for details.
     sage: if not 'amsmath' in t._usepackage: t._usepackage.append('amsmath')
     sage: _ = t.pdf(view=False)
 
 *Proof of Lemma 13*. We compute the number of dominoes in the direction $e_2$
 allowing a surrounding of radius $1,2,3$ in $\Omega_U$. We obtain 35 dominoes
 in the direction $e_2$  allowing a surrounding of radius $2$ and $3$:
```

### Comparing `slabbe-0.7/demos/arXiv_1808_07768_part1.rst` & `slabbe-0.7.1/demos/arXiv_1808_07768_part1.rst`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/demos/arXiv_1808_07768_part2.rst` & `slabbe-0.7.1/demos/arXiv_1808_07768_part2.rst`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/demos/arXiv_1906_01104.rst` & `slabbe-0.7.1/demos/arXiv_1906_01104.rst`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/demos/chapter_three_characterizations.rst` & `slabbe-0.7.1/demos/chapter_three_characterizations.rst`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/docs/Makefile` & `slabbe-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/docs/source/conf.py` & `slabbe-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/docs/source/index.rst` & `slabbe-0.7.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/makefile` & `slabbe-0.7.1/makefile`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-all: install test
+all: install ptest
 
 install:
 	sage -pip install --upgrade --no-index -v .
 install-internet:
 	sage -pip install --upgrade -v .
 
 develop:
```

### Comparing `slabbe-0.7/setup.py` & `slabbe-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/EkEkstar.py` & `slabbe-0.7.1/slabbe/EkEkstar.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/__init__.py` & `slabbe-0.7.1/slabbe/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,20 +49,26 @@
 from .arXiv_1903_06137 import random_jeandel_rao_rectangular_pattern
 from .graph_directed_IFS import GraphDirectedIteratedFunctionSystem
 
 from .beta_numeration_system import BetaTransformation
 
 from .EkEkstar import kFace, kPatch, GeoSub
 
+from .cut_and_project_scheme import (CutAndProjectScheme,
+                                     ModelSet,
+                                     cut_and_project_schemes,
+                                     model_sets)
+
 # BUG (sometimes, cython code does not work properly)
 try:
     from .kolakoski_word import KolakoskiWord
 except ImportError:
     print("There was an error while importing KolakoskiWord cython module")
     print("Maybe that's because the pwd contains the slabbe folder?")
     print("We ignore the problem but this module won't work.")
 
 # for doctext to work, we import convex_boundary
 # from .discrete_subset import convex_boundary
 
 # do not import module names just the above stuff
 #__all__ = []
+
```

### Comparing `slabbe-0.7/slabbe/analyze_sage_build.py` & `slabbe-0.7.1/slabbe/analyze_sage_build.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/arXiv_1808_07768.py` & `slabbe-0.7.1/slabbe/arXiv_1808_07768.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/arXiv_1903_06137.py` & `slabbe-0.7.1/slabbe/arXiv_1903_06137.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/arXiv_1906_01104.py` & `slabbe-0.7.1/slabbe/arXiv_1906_01104.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/beta_numeration_system.py` & `slabbe-0.7.1/slabbe/beta_numeration_system.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/billiard.py` & `slabbe-0.7.1/slabbe/billiard.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/billiard_nD.py` & `slabbe-0.7.1/slabbe/billiard_nD.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/bispecial_extension_type.py` & `slabbe-0.7.1/slabbe/bispecial_extension_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1120,15 +1120,15 @@
         ::
 
             sage: G = E1.graph_under_sadic([132]*2+[123]*6, S)
             sage: from slabbe import TikzPicture
             sage: _ = TikzPicture.from_graph(G).pdf(view=False) # (9s)
             doctest:...: FutureWarning: This class/method/function is marked as experimental.
             It, its functionality or its interface might change without a formal deprecation.
-            See http://trac.sagemath.org/20343 for details.
+            See http...20343 for details.
         """
         R = self.rec_enum_set_under_sadic(substitutions,
                 substitutions_dict, keep_equal_length=keep_equal_length,
                 growth_limit=growth_limit)
         G = recursively_enumerated_set_to_digraph(R)
         if raw:
             return G
```

### Comparing `slabbe-0.7/slabbe/bond_percolation.py` & `slabbe-0.7.1/slabbe/bond_percolation.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/christoffel_graph.py` & `slabbe-0.7.1/slabbe/christoffel_graph.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/coding_of_PETs.py` & `slabbe-0.7.1/slabbe/coding_of_PETs.py`

 * *Files 15% similar despite different names*

```diff
@@ -148,21 +148,24 @@
             for j in range(sizes[1]-1):
                 p = Re2(p)
                 a = self._partition.code(Polyhedron([p]))
                 column.append(a)
             table.append(column)
         return table
 
-    def cylinder(self, pattern):
+    def cylinder(self, pattern, include_empty_interior_atom=False):
         r"""
         Return the coding region of the pattern.
 
         INPUT:
 
         - ``pattern`` -- list of lists or dict of positions to code
+        - ``include_empty_interior_atom`` -- boolean (default:``False``),
+          whether to include in the partition the atom that are not full
+          dimensional (that is, points, lines, etc.)
 
         OUTPUT:
 
             polyhedron partition (containing probably only one atom, or
             more to handle the case of union of polyhedrons)
 
         EXAMPLES::
@@ -213,32 +216,36 @@
         Re2_inv = Re2.inverse()
 
         region = self._partition
         for i,column in enumerate(pattern):
             for j,a in enumerate(column):
                 translated_back = Re1_inv(self._partition[a], niterations=i)
                 translated_back = Re2_inv(translated_back, niterations=j)
-                region = region.refinement(translated_back)
+                region = region.refinement(translated_back,
+                    include_empty_interior_atom=include_empty_interior_atom)
 
         return region
 
 
-    def partition_for_patterns(self, sizes):
+    def partition_for_patterns(self, sizes, include_empty_interior_atom=False):
         r"""
         Return the coding region of the pattern.
 
         INPUT:
 
-        - ``pattern`` -- list of lists or dict of the form
-          ``{positions:code}``
+        - ``sizes`` -- tuple of integers
+        - ``include_empty_interior_atom`` -- boolean (default:``False``),
+          whether to include in the partition the atom that are not full
+          dimensional (that is, points, lines, etc.)
 
         OUTPUT:
 
-            polyhedron partition (containing probably only one atom, or
-            more to handle the case of union of polyhedrons)
+            - polyhedron partition (containing probably only one atom, or
+              more to handle the case of union of polyhedrons)
+            - dictionnary, key to patterns (tuple of tuples)
 
         EXAMPLES::
 
             sage: from slabbe import PolyhedronPartition
             sage: h = 1/3
             sage: p = Polyhedron([(0,h),(0,1),(h,1)])
             sage: q = Polyhedron([(0,0), (0,h), (h,1), (h,0)])
@@ -249,87 +256,143 @@
             sage: base = identity_matrix(2)
             sage: Re1 = PET.toral_translation(base, vector((2/3, 0)))
             sage: Re2 = PET.toral_translation(base, vector((0, 1/4)))
             sage: from slabbe import PETsCoding
             sage: X_P_R = PETsCoding((Re1,Re2), P)
             sage: X_P_R.partition_for_patterns((2,2))
             (Polyhedron partition of 24 atoms with 24 letters,
-             {0: [[0, 0], [2, 2]],
-              1: [[0, 1], [2, 2]],
-              2: [[0, 1], [2, 3]],
-              3: [[1, 0], [2, 2]],
-              4: [[1, 0], [3, 2]],
-              5: [[1, 1], [2, 2]],
-              6: [[1, 1], [3, 2]],
-              7: [[1, 1], [3, 3]],
-              8: [[1, 1], [2, 3]],
-              9: [[2, 2], [0, 0]],
-              10: [[2, 2], [1, 0]],
-              11: [[2, 2], [1, 1]],
-              12: [[2, 2], [2, 2]],
-              13: [[2, 2], [0, 1]],
-              14: [[2, 2], [1, 1]],
-              15: [[2, 2], [2, 2]],
-              16: [[2, 3], [0, 1]],
-              17: [[2, 3], [1, 1]],
-              18: [[2, 3], [2, 2]],
-              19: [[2, 3], [2, 3]],
-              20: [[3, 2], [1, 1]],
-              21: [[3, 2], [2, 2]],
-              22: [[3, 2], [3, 2]],
-              23: [[3, 3], [3, 2]]})
+            {0: ((0, 0), (2, 2)),
+             1: ((0, 1), (2, 2)),
+             2: ((0, 1), (2, 3)),
+             3: ((1, 0), (2, 2)),
+             4: ((1, 0), (3, 2)),
+             5: ((1, 1), (2, 2)),
+             6: ((1, 1), (3, 2)),
+             7: ((1, 1), (3, 3)),
+             8: ((1, 1), (2, 3)),
+             9: ((2, 2), (0, 0)),
+             10: ((2, 2), (1, 0)),
+             11: ((2, 2), (1, 1)),
+             12: ((2, 2), (2, 2)),
+             13: ((2, 2), (0, 1)),
+             14: ((2, 2), (1, 1)),
+             15: ((2, 2), (2, 2)),
+             16: ((2, 3), (0, 1)),
+             17: ((2, 3), (1, 1)),
+             18: ((2, 3), (2, 2)),
+             19: ((2, 3), (2, 3)),
+             20: ((3, 2), (1, 1)),
+             21: ((3, 2), (2, 2)),
+             22: ((3, 2), (3, 2)),
+             23: ((3, 3), (3, 2))})
             sage: X_P_R.partition_for_patterns((1,3))
             (Polyhedron partition of 18 atoms with 18 letters,
-             {0: [[0, 0, 0]],
-              1: [[0, 0, 1]],
-              2: [[0, 1, 0]],
-              3: [[0, 1, 1]],
-              4: [[1, 0, 0]],
-              5: [[1, 0, 1]],
-              6: [[1, 1, 0]],
-              7: [[1, 1, 1]],
-              8: [[1, 1, 1]],
-              9: [[1, 1, 1]],
-              10: [[2, 2, 2]],
-              11: [[2, 2, 2]],
-              12: [[2, 2, 2]],
-              13: [[2, 2, 3]],
-              14: [[2, 3, 2]],
-              15: [[2, 3, 3]],
-              16: [[3, 2, 2]],
-              17: [[3, 3, 2]]})
+            {0: ((0, 0, 0),),
+             1: ((0, 0, 1),),
+             2: ((0, 1, 0),),
+             3: ((0, 1, 1),),
+             4: ((1, 0, 0),),
+             5: ((1, 0, 1),),
+             6: ((1, 1, 0),),
+             7: ((1, 1, 1),),
+             8: ((1, 1, 1),),
+             9: ((1, 1, 1),),
+             10: ((2, 2, 2),),
+             11: ((2, 2, 2),),
+             12: ((2, 2, 2),),
+             13: ((2, 2, 3),),
+             14: ((2, 3, 2),),
+             15: ((2, 3, 3),),
+             16: ((3, 2, 2),),
+             17: ((3, 3, 2),)})
 
         """
         if len(sizes) != 2:
             raise NotImplementedError("we assume len(sizes) is 2 for now")
 
         Re1 = self._PETs[0]
         Re2 = self._PETs[1]
 
         Re1_inv = Re1.inverse()
         Re2_inv = Re2.inverse()
 
         P = self._partition
-        key_to_column = {k:[k] for (k,atoms) in P}
+        key_to_column = {k:(k,) for (k,atoms) in P}
         #print("k",key_to_column)
 
         for j in range(sizes[1]-1):
-            P,d = self._partition.refinement(Re2_inv(P), certificate=True)
+            P,d = self._partition.refinement(Re2_inv(P), certificate=True,
+                    include_empty_interior_atom=include_empty_interior_atom)
             #print("d",d)
-            key_to_column = {k:[d[k][0]]+key_to_column[d[k][1]] for k in d}
+            key_to_column = {k:(d[k][0],)+key_to_column[d[k][1]] for k in d}
             #print("k",key_to_column)
 
         Q = P
-        key_to_word = {k:[col] for (k,col) in key_to_column.items()}
+        key_to_word = {k:(col,) for (k,col) in key_to_column.items()}
         for i in range(sizes[0]-1):
-            Q,d = P.refinement(Re1_inv(Q), certificate=True)
-            key_to_word = {k:[key_to_column[d[k][0]]]+key_to_word[d[k][1]] for k in d}
+            Q,d = P.refinement(Re1_inv(Q), certificate=True,
+                    include_empty_interior_atom=include_empty_interior_atom)
+            key_to_word = {k:(key_to_column[d[k][0]],)+key_to_word[d[k][1]] for k in d}
 
         return Q, key_to_word
 
+    def coincidence_patterns(self, sizes):
+        r"""
+        Return the coincidences for pattern of given shape.
+
+        INPUT:
+
+        - ``sizes`` -- tuple of integers
+
+        OUTPUT:
+
+            list of patterns
+
+        EXAMPLES::
+
+            sage: from slabbe import PolyhedronPartition
+            sage: h = 1/3
+            sage: p = Polyhedron([(0,h),(0,1),(h,1)])
+            sage: q = Polyhedron([(0,0), (0,h), (h,1), (h,0)])
+            sage: r = Polyhedron([(h,1), (1,1), (1,h), (h,0)])
+            sage: s = Polyhedron([(h,0), (1,0), (1,h)])
+            sage: P = PolyhedronPartition({0:p, 1:q, 2:r, 3:s})
+            sage: from slabbe import PolyhedronExchangeTransformation as PET
+            sage: base = identity_matrix(2)
+            sage: Re1 = PET.toral_translation(base, vector((2/3, 0)))
+            sage: Re2 = PET.toral_translation(base, vector((0, 1/4)))
+            sage: from slabbe import PETsCoding
+            sage: X_P_R = PETsCoding((Re1,Re2), P)
+            sage: L21 = X_P_R.coincidence_patterns((2,1))
+            sage: L21
+            [((0,), (0,)), ((1,), (0,)), ((1,), (1,)), ((2,), (3,))]
+            sage: L12 = X_P_R.coincidence_patterns((1,2))
+            sage: L12
+            [((0, 2),), ((1, 2),), ((1, 3),), ((2, 0),), ((2, 1),), ((3, 1),)]
+
+        TESTS:
+
+        This should be all zero::
+
+            sage: [X_P_R.cylinder(p).volume() for p in L21]
+            [0, 0, 0, 0]
+            sage: [X_P_R.cylinder(p).volume() for p in L12]
+            [0, 0, 0, 0, 0, 0]
+
+        """
+        Q, key_to_word = self.partition_for_patterns(sizes,
+                            include_empty_interior_atom=True)
+        # sometimes one key is mapped to a non-full dimensional polygon
+        # and the same key is mapped to a full dimensional polygon
+        # we want to ignore those keys!
+        candidate_patterns = set(key_to_word[a] for (a,p) in Q if not p.is_full_dimensional())
+        valid_patterns = set(key_to_word[a] for (a,p) in Q if p.is_full_dimensional())
+        return sorted(candidate_patterns-valid_patterns)
+
+
     def to_wang_tiles(self):
         r"""
         Recover the Wang tile sets associated to the atoms of the partition.
 
         EXAMPLES::
 
             sage: from slabbe import PolyhedronExchangeTransformation as PET
```

### Comparing `slabbe-0.7/slabbe/combinat.py` & `slabbe-0.7.1/slabbe/combinat.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/ddim_sturmian_configuration.py` & `slabbe-0.7.1/slabbe/ddim_sturmian_configuration.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/diophantine_approx.py` & `slabbe-0.7.1/slabbe/diophantine_approx.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/diophantine_approx_pyx.c` & `slabbe-0.7.1/slabbe/diophantine_approx_pyx.c`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/diophantine_approx_pyx.pyx` & `slabbe-0.7.1/slabbe/diophantine_approx_pyx.pyx`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/discrete_plane.py` & `slabbe-0.7.1/slabbe/discrete_plane.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/discrete_subset.py` & `slabbe-0.7.1/slabbe/discrete_subset.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/double_square_tile.py` & `slabbe-0.7.1/slabbe/double_square_tile.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/dyck_3d.py` & `slabbe-0.7.1/slabbe/dyck_3d.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/finite_word.py` & `slabbe-0.7.1/slabbe/finite_word.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/fruit.py` & `slabbe-0.7.1/slabbe/fruit.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/graph.py` & `slabbe-0.7.1/slabbe/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -633,7 +633,63 @@
             GG.add_edges((s, u_v) for s in GG.neighbors_in(u))
             if GG.out_degree(u) == 1:
                 GG.delete_vertex(u)
             GG.add_edges((u_v, t) for t in GG.neighbors_out(v) if filter(u_v,t))
         GG.delete_vertex(v)
     return GG
 
+def vertices_in_a_cycle(G, verbose=False):
+    r"""
+    Return the set of vertices belonging to a cycle.
+
+    INPUT:
+
+    - ``G`` -- digraph
+    - ``verbose`` -- bool (default:``False``)
+
+    OUTPUT:
+
+    list or set of vertices
+
+    EXAMPLES::
+
+        sage: from slabbe.graph import vertices_in_a_cycle
+        sage: G = DiGraph()
+        sage: G.add_vertex(0)
+        sage: vertices_in_a_cycle(G)
+        []
+        sage: vertices_in_a_cycle(G, verbose=True)
+        ignoring vertex 0 because it has no loop
+        []
+
+    ::
+
+        sage: G = DiGraph(loops=True)
+        sage: G.add_edge(0, 0)
+        sage: vertices_in_a_cycle(G)
+        [0]
+
+    ::
+
+        sage: D = DiGraph({0:[1, 3], 1:[2], 2:[0,3], 4:[5, 6], 5:[6]})
+        sage: D.strongly_connected_components()
+        [[3], [0, 1, 2], [6], [5], [4]]
+        sage: vertices_in_a_cycle(D)
+        [0, 1, 2]
+
+    """
+    V = []
+    for c in G.strongly_connected_components():
+        if len(c) > 1:
+            V.extend(c)
+        elif len(c) == 1:
+            v, = c
+            if G.has_edge(v,v):
+                V.append(v)
+            else:
+                if verbose:
+                    print("ignoring vertex {} because "
+                          "it has no loop".format(v))
+        else:
+            continue
+    return V
+
```

### Comparing `slabbe-0.7/slabbe/graph_directed_IFS.py` & `slabbe-0.7.1/slabbe/graph_directed_IFS.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,25 +211,31 @@
             for b in m_a:
                 j = alphabet.index(b)
                 d[(i,j)].append(pos)
                 pos += module([perron_left[j]])
         return cls.from_inflation_rule(module, root, d)
 
     @classmethod
-    def from_two_dimensional_substitution(cls, s):
+    def from_two_dimensional_substitution(cls, s, inflation=None,
+            stone_inflation_shapes=None):
         r"""
         Return the GIFS defined by a 2-dimensional primitive
         substitution
 
         The marker point associated to each rectangular tile is assumed to
         be in the lower left corner.
 
         INPUT:
 
         - ``s`` -- Substitution2d, primitive substitution
+        - ``inflation`` -- None or (Algebraic) number
+        - ``stone_inflation_shapes`` -- None or dict, from letters to tuple of
+          rectangular dimension of the tilebox associated to each letter.
+          If ``None``, it is computed automaticaly from left eigenvectors of
+          horizontal and vertical substitution.
 
         EXAMPLES::
 
             sage: from slabbe import GraphDirectedIteratedFunctionSystem as GIFS
             sage: from slabbe import Substitution2d
             sage: d = {0:[[3]], 1:[[3],[2]], 2:[[3,1]], 3:[[3,1],[2,0]]}
             sage: s = Substitution2d(d)
@@ -262,49 +268,67 @@
             edge (3,2):
                   [a 0]     [a]
             x |-> [0 a] x + [0]
             edge (3,0):
                   [a 0]     [a]
             x |-> [0 a] x + [a]
 
+        We can provide the rectangular shapes associated to each letter
+        (useful when they are not properly defined automatically)::
+
+            sage: z = polygen(QQ, 'z')
+            sage: K.<phi> = NumberField(z**2-z-1, 'phi', embedding=RR(1.6))
+            sage: shapes = {0:(1,1), 1:(phi,1), 2:(1,phi), 3:(phi,phi)}
+            sage: GIFS.from_two_dimensional_substitution(s, inflation=phi, stone_inflation_shapes=shapes)
+            GIFS defined by 9 maps on Vector space of dimension 2 over
+            Number Field in phi with defining polynomial z^2 - z - 1 with
+            phi = 1.618033988749895?
+
         """
         from sage.matrix.constructor import matrix
         from sage.groups.affine_gps.affine_group import AffineGroup
         from sage.rings.qqbar import number_field_elements_from_algebraics, AA
 
-        rootX, rootY, shapes = s.stone_inflation_shapes()
-        KX = rootX.parent()
-        KY = rootY.parent()
-        numbers = [AA(rootX), AA(rootY)]
-        KXY, (rootX_, rootY_), homo = number_field_elements_from_algebraics(numbers, minimal=True, embedded=True)
-        inflation_matrix = matrix.diagonal(KXY, [rootX, rootY])
-        F = AffineGroup(2, KXY)
-        vector_space = F.vector_space()
+        if inflation is None or stone_inflation_shapes is None:
+            rootX, rootY, stone_inflation_shapes = s.stone_inflation_shapes()
+            KX = rootX.parent()
+            KY = rootY.parent()
+            numbers = [AA(rootX), AA(rootY)]
+            K, (rootX_, rootY_), homo = number_field_elements_from_algebraics(numbers, 
+                                                       minimal=True, embedded=True)
+            inflationX = rootX
+            inflationY = rootY
+        else:
+            K = inflation.parent()
+            inflationX = inflation
+            inflationY = inflation
 
-        alphabet = s.domain_alphabet()
+        inflation_matrix = matrix.diagonal(K, [inflationX, inflationY])
+        F = AffineGroup(2, K)
+        vector_space = F.vector_space()
 
         edges = []
-        for a in alphabet:
+        for a in s.domain_alphabet():
             s_a = s([[a]])
 
             # compute the X positions of marker points
             lower_word = [col[0] for col in s_a]
             X_pos = []
-            pos = KXY.zero()
+            pos = K.zero()
             for b in lower_word:
                 X_pos.append(pos)
-                pos += shapes[b][0]
+                pos += stone_inflation_shapes[b][0]
 
             # compute the Y positions of marker points
             left_word = s_a[0]
             Y_pos = []
-            pos = KXY.zero()
+            pos = K.zero()
             for b in left_word:
                 Y_pos.append(pos)
-                pos += shapes[b][1]
+                pos += stone_inflation_shapes[b][1]
 
             # compute the translations
             for i,col in enumerate(s_a):
                 for j,b in enumerate(col):
                     translation = (X_pos[i], Y_pos[j])
                     f = F(inflation_matrix, translation)
                     edge = (a, b, f)
```

### Comparing `slabbe-0.7/slabbe/infinite_word.py` & `slabbe-0.7.1/slabbe/infinite_word.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/joyal_bijection.py` & `slabbe-0.7.1/slabbe/joyal_bijection.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/kolakoski_word.py` & `slabbe-0.7.1/slabbe/kolakoski_word.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/kolakoski_word_pyx.c` & `slabbe-0.7.1/slabbe/kolakoski_word_pyx.c`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/kolakoski_word_pyx.pyx` & `slabbe-0.7.1/slabbe/kolakoski_word_pyx.pyx`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/language.py` & `slabbe-0.7.1/slabbe/language.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/lyapunov.py` & `slabbe-0.7.1/slabbe/lyapunov.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/magic_hexagon.py` & `slabbe-0.7.1/slabbe/magic_hexagon.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/markov_transformation.py` & `slabbe-0.7.1/slabbe/markov_transformation.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/matrices.py` & `slabbe-0.7.1/slabbe/matrices.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/matrix_cocycle.py` & `slabbe-0.7.1/slabbe/matrix_cocycle.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/modified_mcf.pyx.no` & `slabbe-0.7.1/slabbe/modified_mcf.pyx.no`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/mult_cont_frac.py` & `slabbe-0.7.1/slabbe/mult_cont_frac.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/mult_cont_frac_pyx.c` & `slabbe-0.7.1/slabbe/mult_cont_frac_pyx.c`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/mult_cont_frac_pyx.pyx` & `slabbe-0.7.1/slabbe/mult_cont_frac_pyx.pyx`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/ostrowski.py` & `slabbe-0.7.1/slabbe/ostrowski.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/partial_injection.py` & `slabbe-0.7.1/slabbe/partial_injection.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 Visualisation of the graph::
 
     sage: from slabbe import TikzPicture
     sage: tikz = TikzPicture.from_graph(G)      # optional dot2tex
     doctest:...: FutureWarning: This class/method/function is marked as experimental.
     It, its functionality or its interface might change without a formal deprecation.
-    See http://trac.sagemath.org/20343 for details.
+    See http...20343 for details.
     sage: path_to_file = tikz.pdf()    # not tested
 
 REFERENCES:
 
 - Bassino, Frédérique; Nicaud, Cyril; Weil, Pascal Random generation of
   finitely generated subgroups of a free group.  Internat. J. Algebra
   Comput. 18 (2008), no. 2, 375–405.
```

### Comparing `slabbe-0.7/slabbe/polyhedron_exchange_transformation.py` & `slabbe-0.7.1/slabbe/polyhedron_exchange_transformation.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/polyhedron_partition.py` & `slabbe-0.7.1/slabbe/polyhedron_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             sage: P == R
             doctest:warning
             ...
             FutureWarning: The two partitions are not equal but are equal
             up to a permutation of the coding. The meaning of == for
             polyhedron partition is now more strict. Please update your
             code to use method `is_equal_up_to_relabeling` instead.
-            See https://trac.sagemath.org/99999 for details.
+            See ... for details.
             False
 
         """
         is_equivalent = self.is_equal_up_to_relabeling(other)
         if not is_equivalent:
             return False
         d = self.keys_permutation(other)
@@ -1179,24 +1179,27 @@
         half_partition = PolyhedronPartition([half])
         other_half = Polyhedron(ieqs=[[-a for a in ieq]])
         other_half_partition = PolyhedronPartition([other_half])
         A = self.refinement(half_partition)
         B = self.refinement(other_half_partition)
         return PolyhedronPartition(A.atoms()+B.atoms())
 
-    def refinement(self, other, certificate=False):
+    def refinement(self, other, include_empty_interior_atom=False, certificate=False):
         r"""
         Return the polyhedron partition obtained by the intersection of the
         atoms of self with the atoms of other.
 
         Only atoms of positive volume are kept.
 
         INPUT:
 
         - ``other`` -- a polyhedron partition
+        - ``include_empty_interior_atom`` -- boolean (default:``False``),
+          whether to include in the partition the atom that are non empty
+          but not full dimensional (that is, points, lines, etc.)
         - ``certificate`` -- boolean (default:``False``), return a
           dictionnary for i:(p,q) if atom number i was obtained as the
           intersection of atoms p in self and q in other
 
         OUTPUT:
 
             a polyhedron partition
@@ -1220,23 +1223,32 @@
             sage: P = PolyhedronPartition({0:p, 1:q, 2:r, 3:s})
             sage: g = 1/5
             sage: t1 = Polyhedron([(g,g), (g,1-g), (1-g,g) ])
             sage: t2 = Polyhedron([(g,1-g), (1-g,g), (1-g,1-g)])
             sage: Q = PolyhedronPartition([t1,t2])
             sage: P.refinement(Q)
             Polyhedron partition of 8 atoms with 8 letters
+
+        By default, atoms with empty interior are excluded, but we can
+        include them if necessary::
+
+            sage: P.refinement(P)
+            Polyhedron partition of 4 atoms with 4 letters
+            sage: P.refinement(P, include_empty_interior_atom=True)
+            Polyhedron partition of 14 atoms with 14 letters
+
         """
         if not isinstance(other, PolyhedronPartition):
             raise TypeError("other (of type={}) must a polyhedron"
                     " partition".format(type(other)))
         L = []
         d = {}
         for ((a,p),(b,q)) in itertools.product(self, other):
             p_q = p.intersection(q)
-            if p_q.is_full_dimensional():
+            if (include_empty_interior_atom and not p_q.is_empty()) or p_q.is_full_dimensional():
                 if certificate:
                     d[len(L)] = (a,b)
                 L.append(p_q)
 
         P = PolyhedronPartition(L)
         if certificate:
             return P, d
```

### Comparing `slabbe-0.7/slabbe/ranking_scale.py` & `slabbe-0.7.1/slabbe/ranking_scale.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/sturmian_subshift.py` & `slabbe-0.7.1/slabbe/sturmian_subshift.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/substitution_2d.py` & `slabbe-0.7.1/slabbe/substitution_2d.py`

 * *Files 12% similar despite different names*

```diff
@@ -156,70 +156,76 @@
             sage: hash(s) in ZZ
             True
         """
         sorted_items = tuple(sorted((key,tuple(tuple(column) for column in val))
                                     for (key,val) in self._d.items()))
         return hash(sorted_items)
 
-    def _latex_(self, ncolumns=8, align='l', variableA=None,
-            variableB=None):
+    def _latex_(self, ncolumns=5, align='l', variableA=None,
+            variableB=None, arraycolsep='1.4pt'):
         r"""
         INPUT:
 
-        - ``ncolumns`` -- integer
+        - ``ncolumns`` -- integer (default: ``5``)
         - ``align`` -- character (default:``'l'``), latex alignment symbol
           ``'l'``, ``'r'`` or ``'c'``.
         - ``variableA`` -- string or ``None``
         - ``variableB`` -- string or ``None``
+        - ``arraycolsep`` -- string (default: ``'1.4pt'``)
 
         EXAMPLES::
 
             sage: from slabbe import Substitution2d
             sage: A = [[0,1],[2,3]]
             sage: B = [[4,5]]
             sage: d = {0:A, 1:B}
             sage: s = Substitution2d(d)
             sage: latex(s)
-            \begin{array}{llllllll}
+            {\arraycolsep=1.4pt
+            \begin{array}{lllll}
             0\mapsto \left(\begin{array}{rr}
             1 & 3 \\
             0 & 2
             \end{array}\right)
             ,&
             1\mapsto \left(\begin{array}{r}
             5 \\
             4
             \end{array}\right)
             .
             \end{array}
+            }
 
         ::
 
             sage: s._latex_(2, 'c', variableA='x', variableB='y')
+            {\arraycolsep=1.4pt
             \begin{array}{cc}
             x_{0}\mapsto \left(\begin{array}{rr}
             y_{1} & y_{3} \\
             y_{0} & y_{2}
             \end{array}\right)
             ,&
             x_{1}\mapsto \left(\begin{array}{r}
             y_{5} \\
             y_{4}
             \end{array}\right)
             .
             \end{array}
+            }
 
         """
         from sage.matrix.constructor import matrix
         from sage.modules.free_module_element import vector
         from sage.misc.latex import latex
         from sage.misc.latex import LatexExpr
         from sage.calculus.var import var
         from slabbe.matrices import map_coefficients_to_variable_index
         lines = []
+        lines.append(r'{{\arraycolsep={}'.format(arraycolsep))
         lines.append(r'\begin{{array}}{{{}}}'.format(align*ncolumns))
         for i,(key,table) in enumerate(self._d.items()):
             M = matrix.column([col[::-1] for col in table])
             if M.nrows() == 1:
                 # do not latex array for horizontal vectors
                 M = vector(M)
             if variableA:
@@ -230,14 +236,15 @@
             if (i+1) == len(self._d):
                 lines.append(r'.')
             elif (i+1) % ncolumns == 0:
                 lines.append(r',\\')
             else:
                 lines.append(r',&')
         lines.append(r'\end{array}')
+        lines.append(r'}') # arraycolsep
         return LatexExpr('\n'.join(lines))
 
     @classmethod
     def from_1d_row_substitution(self, s):
         r"""
         INPUT:
 
@@ -1200,14 +1207,118 @@
             table = create_table(factor)
             image = self(table)
             return set_of_factors(image, shape)
         R = RecursivelyEnumeratedSet(seeds, children)
         #return [create_table(f) for f in R]
         return list(R)
 
+    def horizontal_structure_substitution(self):
+        r"""
+        Return the horizontal substitution obtained after quotient 
+        by the equivalence relation defined by letters appearing in the
+        same column.
+
+        INPUT:
+
+        - ``self`` -- expansive and primitive 2d substitution
+
+        OUTPUT:
+
+        - substitution `B\to B^*`
+        - dictionary `A\to B` 
+
+        EXAMPLES::
+
+            sage: from slabbe import Substitution2d
+            sage: A = [[3]]
+            sage: B = [[3],[2]]
+            sage: C = [[3,1]]
+            sage: D = [[3,1],[2,0]]
+            sage: d = {0:A, 1:B, 2:C, 3:D}
+            sage: s = Substitution2d(d)
+            sage: s.horizontal_structure_substitution()
+            (WordMorphism: 2->3, 3->32, {0: 2, 1: 3, 2: 2, 3: 3})
+
+        """
+        if not self.codomain_alphabet() <= self.domain_alphabet():
+            raise ValueError("codomain alphabet (='{}') is not a subset of the"
+                    " domain alphabet (={})".format(self.codomain_alphabet(),
+                                              self.domain_alphabet()))
+        alphabet = self.domain_alphabet()
+
+        from sage.sets.disjoint_set import DisjointSet
+        from sage.combinat.words.morphism import WordMorphism
+        from sage.combinat.words.words import Words
+
+        dominoesV = self.list_dominoes(direction='vertical')
+        partition = DisjointSet(alphabet)
+        for a,b in dominoesV:
+            partition.union(a,b)
+        pHd = partition.element_to_root_dict()
+        pH = Substitution2d.from_permutation(pHd)
+        repH = sorted(partition.root_to_elements_dict().keys())
+        qH = Substitution2d.from_permutation({r:r for r in repH})
+        sH = pH * self * qH
+        sH = {k:[col[0] for col in v] for k,v in sH._d.items()}
+        sH = WordMorphism(sH, codomain=Words(sorted(sH)))
+
+        return sH,pHd
+
+    def vertical_structure_substitution(self):
+        r"""
+        Return the vertical substitution obtained after quotient 
+        by the equivalence relation defined by letters appearing in the
+        same row.
+
+        INPUT:
+
+        - ``self`` -- expansive and primitive 2d substitution
+
+        OUTPUT:
+
+        - substitution `B\to B^*`
+        - dictionary `A\to B` 
+
+        EXAMPLES::
+
+            sage: from slabbe import Substitution2d
+            sage: A = [[3]]
+            sage: B = [[3],[2]]
+            sage: C = [[3,1]]
+            sage: D = [[3,1],[2,0]]
+            sage: d = {0:A, 1:B, 2:C, 3:D}
+            sage: s = Substitution2d(d)
+            sage: s.vertical_structure_substitution()
+            (WordMorphism: 1->3, 3->31, {0: 1, 1: 1, 2: 3, 3: 3})
+
+        """
+        if not self.codomain_alphabet() <= self.domain_alphabet():
+            raise ValueError("codomain alphabet (='{}') is not a subset of the"
+                    " domain alphabet (={})".format(self.codomain_alphabet(),
+                                              self.domain_alphabet()))
+        alphabet = self.domain_alphabet()
+
+        from sage.sets.disjoint_set import DisjointSet
+        from sage.combinat.words.morphism import WordMorphism
+        from sage.combinat.words.words import Words
+
+        dominoesH = self.list_dominoes(direction='horizontal')
+        partition = DisjointSet(alphabet)
+        for a,b in dominoesH:
+            partition.union(a,b)
+        pVd = partition.element_to_root_dict()
+        pV = Substitution2d.from_permutation(pVd)
+        repV = sorted(partition.root_to_elements_dict().keys())
+        qV = Substitution2d.from_permutation({r:r for r in repV})
+        sV = pV * self * qV
+        sV = {k:v[0] for k,v in sV._d.items()}
+        sV = WordMorphism(sV, codomain=Words(sorted(sV)))
+
+        return sV,pVd
+
     def stone_inflation_shapes(self):
         r"""
         Return a dictionary of letters of the domain alphabet associated to
         pairs ``(width, height)`` describing the rectangular shape
         associated to the given letter.
 
         Those rectangular shapes are such that the 2d substitution can be
@@ -1244,48 +1355,25 @@
         """
         if not self.codomain_alphabet() <= self.domain_alphabet():
             raise ValueError("codomain alphabet (='{}') is not a subset of the"
                     " domain alphabet (={})".format(self.codomain_alphabet(),
                                               self.domain_alphabet()))
         alphabet = self.domain_alphabet()
 
-        from sage.sets.disjoint_set import DisjointSet
-        from sage.combinat.words.morphism import WordMorphism
         from slabbe.matrices import perron_left_eigenvector_in_number_field
-        from sage.combinat.words.words import Words
 
-        dominoesH = self.list_dominoes(direction='horizontal')
-        partitionH = DisjointSet(alphabet)
-        for a,b in dominoesH:
-            partitionH.union(a,b)
-        pHd = partitionH.element_to_root_dict()
-        pH = Substitution2d.from_permutation(pHd)
-        repH = sorted(partitionH.root_to_elements_dict().keys())
-        qH = Substitution2d.from_permutation({r:r for r in repH})
-        sH = pH * self * qH
-        sH = {k:v[0] for k,v in sH._d.items()}
-        sH = WordMorphism(sH, codomain=Words(sorted(sH))).incidence_matrix()
-        rootY, heights = perron_left_eigenvector_in_number_field(sH, 'rootY')
-        heigths_dict = dict(zip(repH, heights))
-        heigths_dict = {k:heigths_dict[v] for k,v in pHd.items()}
-
-        dominoesV = self.list_dominoes(direction='vertical')
-        partitionV = DisjointSet(alphabet)
-        for a,b in dominoesV:
-            partitionV.union(a,b)
-        pVd = partitionV.element_to_root_dict()
-        pV = Substitution2d.from_permutation(pVd)
-        repV = sorted(partitionV.root_to_elements_dict().keys())
-        qV = Substitution2d.from_permutation({r:r for r in repV})
-        sV = pV * self * qV
-        sV = {k:[col[0] for col in v] for k,v in sV._d.items()}
-        sV = WordMorphism(sV, codomain=Words(sorted(sV))).incidence_matrix()
-        rootX, widths = perron_left_eigenvector_in_number_field(sV, 'rootX')
-        widths_dict = dict(zip(repV, widths))
-        widths_dict = {k:widths_dict[v] for k,v in pVd.items()}
+        sV,pVd = self.vertical_structure_substitution()
+        rootY, heights = perron_left_eigenvector_in_number_field(sV.incidence_matrix(), 'rootY')
+        heigths_dict = dict(zip(sV.codomain().alphabet(), heights))
+        heigths_dict = {k:heigths_dict[v] for k,v in pVd.items()}
+
+        sH,pHd = self.horizontal_structure_substitution()
+        rootX, widths = perron_left_eigenvector_in_number_field(sH.incidence_matrix(), 'rootX')
+        widths_dict = dict(zip(sH.codomain().alphabet(), widths))
+        widths_dict = {k:widths_dict[v] for k,v in pHd.items()}
 
         return rootX, rootY, {a:(widths_dict[a], heigths_dict[a]) for a in alphabet}
 
     def lines_alphabet(self, direction='horizontal'):
         r"""
         Return the possible alphabets on lines, i.e., the possible alphabet
         of letters that we see on a given line.
@@ -1322,22 +1410,26 @@
         result = []
         for s in G.strongly_connected_components_subgraphs():
             if s.num_edges() > 0:
                 for v in s.vertices(sort=True):
                     result.append(v)
         return result
 
-    def prolongable_seeds_graph(self):
+    def prolongable_seeds_graph(self, clean_sources=False):
         r"""
         Return the directed graph of 2x2 factors where (u,v) is an edge if
         v is the seed at the origin of the image of u under self.
 
+        INPUT:
+
+        - ``clean_sources`` -- bool (default:``False``)
+
         OUTPUT:
 
-            list of tuple (2x2 matrix, integer)
+            graph
 
         EXAMPLES::
 
             sage: d = {0: [[17]],
             ....:  1: [[16]],
             ....:  2: [[15], [11]],
             ....:  3: [[13], [9]],
@@ -1354,37 +1446,63 @@
             ....:  14: [[13, 7], [9, 1]],
             ....:  15: [[12, 6], [9, 1]],
             ....:  16: [[18, 5], [10, 1]],
             ....:  17: [[13, 4], [9, 1]],
             ....:  18: [[14, 2], [8, 0]]}
             sage: from slabbe import Substitution2d
             sage: omega = Substitution2d(d)
-            sage: G = omega.prolongable_seeds_graph()
-            sage: G
-            Looped digraph on 50 vertices
+            sage: omega.prolongable_seeds_graph()
+            Looped digraph on 1344 vertices
+            sage: omega.prolongable_seeds_graph(clean_sources=True)
+            Looped digraph on 256 vertices
 
         """
         from sage.matrix.constructor import matrix
         from sage.sets.recursively_enumerated_set import RecursivelyEnumeratedSet
-        seeds = self.list_2x2_factors(F=None)
-        seeds = [matrix.column(c[::-1] for c in columns) for columns in seeds]
-        for m in seeds: m.set_immutable()
+        # compute the letters appearing in the 4 corners
+        alphabet = self.domain_alphabet()
+        bottom_left  = sorted(set(self([[a]])[0][0] for a in alphabet))
+        bottom_right = sorted(set(self([[a]])[-1][0] for a in alphabet))
+        top_left     = sorted(set(self([[a]])[0][-1] for a in alphabet))
+        top_right    = sorted(set(self([[a]])[-1][-1] for a in alphabet))
+
+        # initialize the seeds with the cartesian product of these
+        seeds = []
+        for (a,b,c,d) in itertools.product(bottom_right, bottom_left,
+                                           top_right, top_left):
+            table = [(c,a), (d,b)]
+            try:
+                self(table)
+            except ValueError:
+                continue
+            else:
+                # consider only those for which the application of the
+                # substitution is defined
+                m = matrix(2,[a,b,c,d])
+                m.set_immutable()
+                seeds.append(m)
+
         def children(m):
             b,d,a,c = m.list()
-            A = self([[a]])[-1][-1] # bottom left
-            B = self([[b]])[-1][0] # top left
-            C = self([[c]])[0][-1] # bottom right
-            D = self([[d]])[0][0] # top right
+            A = self([[a]])[-1][-1] # bottom left  (in the seed)
+            B = self([[b]])[-1][0]  # top left     (in the seed)
+            C = self([[c]])[0][-1]  # bottom right (in the seed)
+            D = self([[d]])[0][0]   # top right    (in the seed)
             M = matrix.column(((B,A),(D,C)))
             M.set_immutable()
             return [M]
         R = RecursivelyEnumeratedSet(seeds, children)
-        return R.to_digraph(multiedges=False)
+        G = R.to_digraph(multiedges=False)
+        if clean_sources:
+            from slabbe.graph import clean_sources_and_sinks
+            return clean_sources_and_sinks(G)
+        else:
+            return G
+
 
-    prolongable_origins = deprecated_function_alias(123456, prolongable_seeds_graph)
     def prolongable_seeds_list(self):
         r"""
         Return the list of seed which are prolongable for some power of
         self.
 
         OUTPUT:
 
@@ -1409,36 +1527,306 @@
             ....:  14: [[13, 7], [9, 1]],
             ....:  15: [[12, 6], [9, 1]],
             ....:  16: [[18, 5], [10, 1]],
             ....:  17: [[13, 4], [9, 1]],
             ....:  18: [[14, 2], [8, 0]]}
             sage: from slabbe import Substitution2d
             sage: omega = Substitution2d(d)
-            sage: omega.prolongable_seeds_list()
-            [[
-             [ 9 14]  [17 13]
-             [ 1  6], [16 15]
-             ],
-             [
-             [ 9 14]  [17 13]
-             [ 8 16], [ 6  5]
-             ],
-             [
-             [10 12]  [16 15]
-             [ 9 14], [ 3  7]
-             ],
-             [
-             [10 14]  [16 13]
-             [11 17], [ 2  4]
-             ]]
+
+        Here there are many seeds::
+
+            sage: seeds = flatten(omega.prolongable_seeds_list())
+            sage: len(seeds)
+            256
+
+        If all seeds belong to the language of the substitution (computed
+        from the letters), then there exists a unique subshift which is
+        self-similar with respect to the substitution. In this example,
+        it is not true::
+
+            sage: seeds_as_table = [[list(col[::-1]) for col in m.columns()] for m in seeds]
+            sage: F = omega.list_2x2_factors()
+            sage: all(seed in F for seed in seeds_as_table)
+            False
+
+        Indeed, only 8 of the 256 seeds belong to the language of the
+        substitution::
+
+            sage: [seed for seed in seeds_as_table if seed in F]
+            [[[1, 9], [6, 14]],
+             [[16, 17], [15, 13]],
+             [[8, 9], [16, 14]],
+             [[6, 17], [5, 13]],
+             [[9, 10], [14, 12]],
+             [[3, 16], [7, 15]],
+             [[11, 10], [17, 14]],
+             [[2, 16], [4, 13]]]
+
+        This means that all the other 248 seeds give rise to configurations
+        which are fixed by the substitution but are not uniformly
+        recurrent. In particular, if a subshift is self-similar with
+        respect to that substitution, we can not conclude that it is
+        minimal.
 
         """
         G = self.prolongable_seeds_graph()
         return [cycle[:-1] for cycle in G.all_simple_cycles()]
 
+    def periodic_horizontal_domino_seeds_graph(self, clean_sources=False):
+        r"""
+        Return the directed graph of horizontal dominoes where (u,v) is an edge if
+        the domino v appears in the image of the domino u under self on the separation
+        between the image of the two letters of the domino.
+
+        INPUT:
+
+        - ``clean_sources`` -- bool (default:``False``)
+
+        OUTPUT:
+
+            graph
+
+        EXAMPLES::
+
+            sage: d = {0: [[17]],
+            ....:  1: [[16]],
+            ....:  2: [[15], [11]],
+            ....:  3: [[13], [9]],
+            ....:  4: [[17], [8]],
+            ....:  5: [[16], [8]],
+            ....:  6: [[15], [8]],
+            ....:  7: [[14], [8]],
+            ....:  8: [[14, 6]],
+            ....:  9: [[17, 3]],
+            ....:  10: [[16, 3]],
+            ....:  11: [[14, 2]],
+            ....:  12: [[15, 7], [11, 1]],
+            ....:  13: [[14, 6], [11, 1]],
+            ....:  14: [[13, 7], [9, 1]],
+            ....:  15: [[12, 6], [9, 1]],
+            ....:  16: [[18, 5], [10, 1]],
+            ....:  17: [[13, 4], [9, 1]],
+            ....:  18: [[14, 2], [8, 0]]}
+            sage: from slabbe import Substitution2d
+            sage: omega = Substitution2d(d)
+            sage: omega.periodic_horizontal_domino_seeds_graph()
+            Looped digraph on 79 vertices
+            sage: omega.periodic_horizontal_domino_seeds_graph(clean_sources=True)
+            Looped digraph on 51 vertices
+
+        """
+        # compute the letters appearing at the left/right of images
+        from collections import defaultdict
+        data_end = defaultdict(list)
+        data_start = defaultdict(list)
+        for a in self.domain_alphabet():
+            image = self([[a]])
+            right_column = image[-1]
+            length = len(right_column)
+            for j,b in enumerate(right_column):
+                data_end[(j,length)].append(b)
+
+            left_column = image[0]
+            for j,b in enumerate(left_column):
+                data_start[(j,length)].append(b)
+
+        possible_dominoes = set()
+        for j_length in data_end:
+            A = data_end[j_length]
+            B = data_start[j_length]
+            possible_dominoes.update(itertools.product(A,B))
+
+        def children(t):
+            a,b = t
+            A = self([[a]])
+            B = self([[b]])
+            A_right_col = A[-1]
+            B_first_col = B[0]
+            return list(zip(A_right_col, B_first_col))
+        from sage.sets.recursively_enumerated_set import RecursivelyEnumeratedSet
+        R = RecursivelyEnumeratedSet(possible_dominoes, children)
+        G = R.to_digraph(multiedges=False)
+
+        if clean_sources:
+            from slabbe.graph import clean_sources_and_sinks
+            return clean_sources_and_sinks(G)
+        else:
+            return G
+
+    def periodic_vertical_domino_seeds_graph(self, clean_sources=False):
+        r"""
+        Return the directed graph of vertical dominoes where (u,v) is an edge if
+        the domino v appears in the image of the domino u under self on the separation
+        between the image of the two letters of the domino.
+
+        INPUT:
+
+        - ``clean_sources`` -- bool (default:``False``)
+
+        OUTPUT:
+
+            graph
+
+        EXAMPLES::
+
+            sage: from slabbe import Substitution2d
+            sage: d = {0: [[17]],
+            ....:  1: [[16]],
+            ....:  2: [[15], [11]],
+            ....:  3: [[13], [9]],
+            ....:  4: [[17], [8]],
+            ....:  5: [[16], [8]],
+            ....:  6: [[15], [8]],
+            ....:  7: [[14], [8]],
+            ....:  8: [[14, 6]],
+            ....:  9: [[17, 3]],
+            ....:  10: [[16, 3]],
+            ....:  11: [[14, 2]],
+            ....:  12: [[15, 7], [11, 1]],
+            ....:  13: [[14, 6], [11, 1]],
+            ....:  14: [[13, 7], [9, 1]],
+            ....:  15: [[12, 6], [9, 1]],
+            ....:  16: [[18, 5], [10, 1]],
+            ....:  17: [[13, 4], [9, 1]],
+            ....:  18: [[14, 2], [8, 0]]}
+            sage: omega = Substitution2d(d)
+            sage: omega.periodic_vertical_domino_seeds_graph()
+            Looped digraph on 93 vertices
+            sage: omega.periodic_vertical_domino_seeds_graph(clean_sources=True)
+            Looped digraph on 56 vertices
+
+        """
+        # compute the letters appearing at the top/bottom of images
+        from collections import defaultdict
+        data_end = defaultdict(list)
+        data_start = defaultdict(list)
+        for a in self.domain_alphabet():
+            image = self([[a]])
+            top_row = [col[-1] for col in image]
+            length = len(top_row)
+            for j,b in enumerate(top_row):
+                data_end[(j,length)].append(b)
+
+            bottom_row = [col[0] for col in image]
+            for j,b in enumerate(bottom_row):
+                data_start[(j,length)].append(b)
+
+        possible_dominoes = set()
+        for j_length in data_end:
+            A = data_end[j_length]
+            B = data_start[j_length]
+            possible_dominoes.update(itertools.product(A,B))
+
+        def children(t):
+            a,b = t
+            A = self([[a]])
+            B = self([[b]])
+            A_top_row = [col[-1] for col in A]
+            B_bottom_row = [col[0] for col in B]
+            return list(zip(A_top_row, B_bottom_row))
+        from sage.sets.recursively_enumerated_set import RecursivelyEnumeratedSet
+        R = RecursivelyEnumeratedSet(possible_dominoes, children)
+        G = R.to_digraph(multiedges=False)
+
+        if clean_sources:
+            from slabbe.graph import clean_sources_and_sinks
+            return clean_sources_and_sinks(G)
+        else:
+            return G
+
+    def has_unique_self_similar_subshift(self, verbose=False):
+        r"""
+        Return whether there is a unique self-similar subshift associated
+        to this substitution.
+
+        INPUT:
+
+        - ``verbose`` -- bool (default:``False``), if ``True`` prints
+          information why there is no unique self-similar subshift
+
+        OUTPUT:
+
+            boolean
+
+        EXAMPLES::
+
+            sage: from slabbe import Substitution2d
+            sage: d = {0: [[17]],
+            ....:  1: [[16]],
+            ....:  2: [[15], [11]],
+            ....:  3: [[13], [9]],
+            ....:  4: [[17], [8]],
+            ....:  5: [[16], [8]],
+            ....:  6: [[15], [8]],
+            ....:  7: [[14], [8]],
+            ....:  8: [[14, 6]],
+            ....:  9: [[17, 3]],
+            ....:  10: [[16, 3]],
+            ....:  11: [[14, 2]],
+            ....:  12: [[15, 7], [11, 1]],
+            ....:  13: [[14, 6], [11, 1]],
+            ....:  14: [[13, 7], [9, 1]],
+            ....:  15: [[12, 6], [9, 1]],
+            ....:  16: [[18, 5], [10, 1]],
+            ....:  17: [[13, 4], [9, 1]],
+            ....:  18: [[14, 2], [8, 0]]}
+            sage: omega = Substitution2d(d)
+            sage: omega.has_unique_self_similar_subshift()
+            False
+
+        """
+        from slabbe.graph import vertices_in_a_cycle
+        result = True
+
+        # for unicity to hold, all prolongable seeds need to be
+        # in the language of the substitution
+        G = self.prolongable_seeds_graph()
+        seeds = vertices_in_a_cycle(G)
+        seeds_as_table = [[list(col[::-1]) for col in m.columns()] for m in seeds]
+        F = self.list_2x2_factors()
+        if not all(seed in F for seed in seeds_as_table):
+            if verbose:
+                print(("2x2 seeds preserved by the substitution, but which are not in the language "
+                    "of the substitution:"), [seed for seed in seeds_as_table if seed not in F])
+                result = False
+            else:
+                return False
+
+        # for unicity to hold, all horizontal dominos seeds need to be
+        # in the language of the substitution
+        G_h = self.periodic_horizontal_domino_seeds_graph(clean_sources=True)
+        seeds_h = set(vertices_in_a_cycle(G_h))
+        dominoes_h = set(self.list_dominoes(direction='horizontal'))
+        if not seeds_h <= dominoes_h:
+            if verbose:
+                print(("Horizontal domino seeds preserved by the substitution, but which are "
+                    "not in the language of the substitution:"), seeds_h - dominoes_h)
+                result = False
+            else:
+                return False
+
+        # for unicity to hold, all vertical dominos seeds need to be
+        # in the language of the substitution
+        G_v = self.periodic_vertical_domino_seeds_graph(clean_sources=True)
+        seeds_v = set(vertices_in_a_cycle(G_v))
+        dominoes_v = set(self.list_dominoes(direction='vertical'))
+        if not seeds_v <= dominoes_v:
+            if verbose:
+                print(("Vertical domino seeds preserved by the substitution, but which are "
+                    "not in the language of the substitution:"), seeds_v - dominoes_v)
+                result = False
+            else:
+                return False
+
+        if verbose and not result:
+            return result
+
+        raise NotImplementedError("if the above did not returned False,"
+                " then a Lemma is needed to show that the result is True")
+
     _matrix_ = incidence_matrix
     def relabel_domain(self, other):
         r"""
         Return a permutation p such that self*p == other, if it exists.
 
         INPUT:
```

### Comparing `slabbe-0.7/slabbe/tikz_picture.py` & `slabbe-0.7.1/slabbe/tikz_picture.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 If dot2tex Sage optional package and graphviz are installed, then the following
 one liner works::
 
     sage: t = TikzPicture.from_graph(g)  # optional: dot2tex (3s)
     doctest:...: FutureWarning: This class/method/function is marked as experimental.
     It, its functionality or its interface might change without a formal deprecation.
-    See http://trac.sagemath.org/20343 for details.
+    See http...20343 for details.
 
 ::
 
     sage: s = latex(transducers.GrayCode())
     sage: t = TikzPicture(s, usetikzlibrary=['automata'])
     sage: _ = t.pdf(view=False)  # long time (2s)
 
@@ -83,15 +83,15 @@
 except ImportError:
     from sage.misc.sage_ostools import have_program
 
 from sage.misc.temporary_file import tmp_filename
 from sage.structure.sage_object import SageObject
 
 from sage.misc.decorators import rename_keyword
-from sage.misc.superseded import experimental
+#from sage.misc.superseded import experimental
 
 class Standalone(SageObject):
     @rename_keyword(standalone_options="standalone_config")
     def __init__(self, content, standalone_config=None, usepackage=None,
             usetikzlibrary=None, macros=None, use_sage_preamble=False):
         r"""
         See the class documentation for full information.
@@ -684,15 +684,15 @@
                                crop=True,
                                figonly='True',
                                prog=prog).strip()
         return TikzPicture(tikz, standalone_config=["border=4mm"],
                            usetikzlibrary=['shapes'])
 
     @classmethod
-    @experimental(trac_number=20343)
+    #@experimental(trac_number=20343)
     def from_graph(cls, graph, merge_multiedges=True,
             merge_label_function=tuple, **kwds):
         r"""
         Convert a graph to a tikzpicture using graphviz and dot2tex.
 
         .. NOTE::
 
@@ -825,15 +825,15 @@
         graph.latex_options().set_options(**default)
         tikz = graph._latex_()
         usepackage = ['amsmath']
         return TikzPicture(tikz, standalone_config=["border=4mm"],
                 usepackage=usepackage)
 
     @classmethod
-    @experimental(trac_number=20343)
+    #@experimental(trac_number=20343)
     def from_graph_with_pos(cls, graph, scale=1, merge_multiedges=True,
             merge_label_function=tuple):
         r"""
         Convert a graph with positions defined for vertices to a tikzpicture.
 
         INPUT:
 
@@ -850,15 +850,15 @@
         EXAMPLES::
 
             sage: from slabbe import TikzPicture
             sage: g = graphs.PetersenGraph()
             sage: tikz = TikzPicture.from_graph_with_pos(g)
             doctest:...: FutureWarning: This class/method/function is marked as experimental.
             It, its functionality or its interface might change without a formal deprecation.
-            See http://trac.sagemath.org/20343 for details.
+            See http...20343 for details.
 
         ::
 
             sage: edges = [(0,0,'a'),(0,1,'b'),(0,1,'c')]
             sage: kwds = dict(format='list_of_edges', loops=True, multiedges=True)
             sage: G = DiGraph(edges, **kwds)
             sage: G.set_pos({0:(0,0), 1:(1,0)})
@@ -963,15 +963,15 @@
         EXAMPLES::
 
             sage: from slabbe import TikzPicture
             sage: P = posets.PentagonPoset()
             sage: tikz = TikzPicture.from_poset(P) # optional dot2tex # long time (3s)
             doctest:...: FutureWarning: This class/method/function is marked as experimental.
             It, its functionality or its interface might change without a formal deprecation.
-            See http://trac.sagemath.org/20343 for details.
+            See http...20343 for details.
             sage: tikz = TikzPicture.from_poset(P, prog='neato', color_by_label=True) # optional dot2tex # long time (3s)
 
         ::
 
             sage: P = posets.SymmetricGroupWeakOrderPoset(4)
             sage: tikz = TikzPicture.from_poset(P) # optional dot2tex # long time (4s)
             sage: tikz = TikzPicture.from_poset(P, prog='neato') # optional dot2tex # long time (4s)
```

### Comparing `slabbe-0.7/slabbe/wang_tiles.py` & `slabbe-0.7.1/slabbe/wang_tiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,17 +222,22 @@
             col0, col1, col2, col3 = color
             triangle = r'\fill[{}] {} -- {} -- {};'
             c = (x+.5*sx,y+.5*sy)
             lines.append(triangle.format(col0, (x+sx,y),c,(x+sx,y+sy)))
             lines.append(triangle.format(col1, (x,y+sy),c,(x+sx,y+sy)))
             lines.append(triangle.format(col2, (x,y),c,(x,y+sy)))
             lines.append(triangle.format(col3, (x,y),c,(x+sx,y)))
-        else:
+        elif draw_H is None and draw_V is None:
             square = r'\fill[{}] {} -- {} -- {} -- {} -- cycle;'
             lines.append(square.format(color, (x,y), (x+sx,y), (x+sx,y+sy), (x,y+sy)))
+        else:
+            # hacky way to fix issue with JR
+            half_square = r'\fill[{}] {} {} {};'
+            lines.append(half_square.format(color, (x,y), draw_H[tile[3]][14:-1], draw_V[tile[0]][14:-1]))
+            lines.append(half_square.format(color, (x,y), draw_V[tile[2]][14:-1], draw_H[tile[1]][14:-1]))
 
     if id is not None:
         c = (x+.5*sx,y+.5*sy)
         id = id_format.format(id)
         lines.append(r'\node[{}] at {} {{{}}};'.format(id_color, c, id))
 
     if draw_H is None:
@@ -3170,15 +3175,14 @@
               (0, 0, 3),
               (0, 0, 4),
               (0, 1, 0),
               (0, 1, 1),
               (0, 1, 2),
               (0, 1, 3),
               (0, 1, 4)])
-
         """
         from math import log, ceil
 
         # mapping the vertical colors to complementary binary strings
         vertical_alphabet = sorted(self.vertical_alphabet())
         padtoV = int(ceil(log(len(vertical_alphabet)+1, 2)))+1
         left_color_to_digits = {c:[k for (k,d) in 
@@ -3466,14 +3470,32 @@
 
         ::
 
             sage: tiles = [(0,0,0,0), (1,1,1,1), (2,2,2,2)]
             sage: W = WangTileSolver(tiles,2,2)
             sage: W.number_of_solutions()
             3
+
+        TESTS::
+
+            sage: tiles = [('E', 'F', 'G', 'H'), ('A', 'B', 'C', 'D')]
+            sage: preassigned_color = [{(0, 0): 'A'}, {(0, 0): 'B'}, {(0, 0): 'C'}, {(0, 0): 'D'}]
+            sage: W = WangTileSolver(tiles, 1, 1, preassigned_color=preassigned_color)
+            sage: W.number_of_solutions()     # known bug
+            1
+            sage: tiles = [('E', 'F', 'G', 'H'), ('A', 'B', 'C', 'D')]
+            sage: preassigned_color = [{(0, 0): 'A'}, {}, {}, {}]
+            sage: W = WangTileSolver(tiles, 1, 1, preassigned_color=preassigned_color)
+            sage: W.number_of_solutions()     # known bug
+            1
+            sage: preassigned_color = [{}, {}, {(0, 0): 'C'}, {}]
+            sage: W = WangTileSolver(tiles, 1, 1, preassigned_color=preassigned_color)
+            sage: W.number_of_solutions()     # known bug
+            1
+
         """
         return self.dlx_solver().number_of_solutions(ncpus=ncpus)
 
     def solutions_iterator(self):
         r"""
         Iterator over all solutions
 
@@ -4700,14 +4722,16 @@
                 this_id = i if id else None
                 position = (j,k)
                 tile = self._tiles[i]
                 right_edges = edges and (j == W - 1 or self._table[j+1][k] is None)
                 top_edges = edges and (k == H - 1 or self._table[j][k+1] is None)
                 if color_by_tile_id:
                     this_color = color_by_tile_id[i]
+                elif isinstance(color, str):
+                    this_color = color
                 elif color is not None:
                     this_color = tuple(color[a] for a in tile)
                 else:
                     this_color = None
                 more_lines = tile_to_tikz(tile, position, color=this_color,
                         id=this_id, id_color=id_color, id_format=id_format,
                         sizex=size, sizey=size, rotate=rotate, label=label,
```

### Comparing `slabbe-0.7/slabbe/word_morphisms.py` & `slabbe-0.7.1/slabbe/word_morphisms.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe/write_to_file.py` & `slabbe-0.7.1/slabbe/write_to_file.py`

 * *Files identical despite different names*

### Comparing `slabbe-0.7/slabbe.egg-info/PKG-INFO` & `slabbe-0.7.1/slabbe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slabbe
-Version: 0.7
+Version: 0.7.1
 Summary: Sebastien Labbe's Research code
 Home-page: http://gitlab.com/seblabbe/slabbe
 Author: Sebastien Labbe
 Author-email: slabbe@ulg.ac.be
 License: GPLv2+
 Keywords: sagemath combinatorics discrete geometry symbolic dynamics
 Classifier: Development Status :: 4 - Beta
@@ -24,20 +24,21 @@
 
 This is an optional package for SageMath containing code I wrote for research.
 It contains modules on the following topics.
 
 **Discrete dynamical systems**
   diophantine approximation, Markov transformations, Wang tilings, Lyapunov
   exponents, matrix cocycles, multidimensional continued fraction algorithms,
-  polyhedron exchange transformations, GIFS.
+  polyhedron exchange transformations (PETs), GIFS,
 
 **Combinatorics**
   2d substitutions, bispecial factors, bond percolation, Dyck word in 3D,
   words, Joyal bijection, languages, Oldenburger sequence, ostrowski
-  numeration, partial injections,
+  numeration, partial injections, d-dimensional Sturmian configurations,
+  hypercubic billiard words
 
 **Digital geometry**
   Christoffel graph, discrete subset, discrete plane, double square tiles,
   polyhedron partitions,
 
 **Vizualization**
   tikzpicture
@@ -181,19 +182,27 @@
 module(s) and I will create a ticket on trac__ for its inclusion into SageMath.
 
 __ https://trac.sagemath.org/
 
 Release history
 ---------------
 
+*Version 0.7.1 (June 30, 2023)*
+  New module on cut and project scheme (still preliminary).
+  New module to draw tilings with the Smith's aperiodic monotile (see this `blog post`__).
+  Few other improvements.
+  All tests passed on version 10.0 of SageMath.
+
+__ http://www.slabbe.org/blogue/2023/05/decoupe-laser-du-chapeau-tuile-aperiodique-decouverte-recemment/
+
 *Version 0.7 (December 8, 2022)*
   New module on d-dimensional Sturmian configurations, to draw figures from `arXiv:2204.06413`__.
   New module on Hypercubic billiard words (written with Mélodie Andrieu).
   The module ``TikzPicture`` got merged in SageMath 9.6 into
-  `sage.misc.latex_standalone` through ticket `#20343`__ during which many
+  ``sage.misc.latex_standalone`` through ticket `#20343`__ during which many
   improvements were made. The line ``from slabbe import TikzPicture`` now uses
   the one in SageMath by default. All tests passed on version 9.7 of SageMath.
   Up to recently, all tests passed on versions 9.0, 9.1, 9.2, 9.3 and 9.4 of SageMath;
   can't test those earlier versions of SageMath anymore because gitlab continuous
   integration tests is not free anymore.
 
 __ https://arxiv.org/abs/2204.06413
```

### Comparing `slabbe-0.7/slabbe.egg-info/SOURCES.txt` & `slabbe-0.7.1/slabbe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,32 +60,35 @@
 docs/source/tikz_picture.rst
 docs/source/wang_tiles.rst
 docs/source/word_morphisms.rst
 docs/source/write_to_file.rst
 slabbe/EkEkstar.py
 slabbe/__init__.py
 slabbe/analyze_sage_build.py
+slabbe/aperiodic_monotile.py
 slabbe/arXiv_1808_07768.py
 slabbe/arXiv_1903_06137.py
 slabbe/arXiv_1906_01104.py
 slabbe/beta_numeration_system.py
 slabbe/billiard.py
 slabbe/billiard_nD.py
 slabbe/bispecial_extension_type.py
 slabbe/bond_percolation.py
 slabbe/christoffel_graph.py
 slabbe/coding_of_PETs.py
 slabbe/combinat.py
+slabbe/cut_and_project_scheme.py
 slabbe/ddim_sturmian_configuration.py
 slabbe/diophantine_approx.py
 slabbe/diophantine_approx_pyx.c
 slabbe/diophantine_approx_pyx.pyx
 slabbe/discrete_plane.py
 slabbe/discrete_subset.py
 slabbe/double_square_tile.py
+slabbe/dumont_thomas_on_Z.py
 slabbe/dyck_3d.py
 slabbe/finite_word.py
 slabbe/fruit.py
 slabbe/graph.py
 slabbe/graph_directed_IFS.py
 slabbe/infinite_word.py
 slabbe/joyal_bijection.py
```

