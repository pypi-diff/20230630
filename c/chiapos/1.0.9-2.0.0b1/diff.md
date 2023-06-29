# Comparing `tmp/chiapos-1.0.9.tar.gz` & `tmp/chiapos-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiapos-1.0.9.tar", last modified: Tue Feb  1 05:09:02 2022, max compression
+gzip compressed data, was "chiapos-2.0.0b1.tar", last modified: Thu Jun 29 23:31:37 2023, max compression
```

## Comparing `chiapos-1.0.9.tar` & `chiapos-2.0.0b1.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.065206 chiapos-1.0.9/
--rw-r--r--   0 runner     (501) staff       (20)      428 2022-02-01 05:08:30.000000 chiapos-1.0.9/.clang-format
--rw-r--r--   0 runner     (501) staff       (20)       97 2022-02-01 05:08:30.000000 chiapos-1.0.9/.dockerignore
--rw-r--r--   0 runner     (501) staff       (20)       56 2022-02-01 05:08:30.000000 chiapos-1.0.9/.flake8
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.977973 chiapos-1.0.9/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.992634 chiapos-1.0.9/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     3009 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/build-aarch64.yml
--rw-r--r--   0 runner     (501) staff       (20)     3124 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/build-m1-wheel.yml
--rw-r--r--   0 runner     (501) staff       (20)     2719 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/build-test-cplusplus.yml
--rw-r--r--   0 runner     (501) staff       (20)     4684 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner     (501) staff       (20)     1382 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/doc-html-pdf.yml
--rw-r--r--   0 runner     (501) staff       (20)     1883 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/manual-plot.yml
--rw-r--r--   0 runner     (501) staff       (20)     1252 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/plot-k27-no-bitfield.yaml
--rw-r--r--   0 runner     (501) staff       (20)     1232 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/plot-k27.yaml
--rwxr-xr-x   0 runner     (501) staff       (20)     1330 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner     (501) staff       (20)      316 2022-02-01 05:08:30.000000 chiapos-1.0.9/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     5765 2022-02-01 05:08:30.000000 chiapos-1.0.9/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      583 2022-02-01 05:08:30.000000 chiapos-1.0.9/Dockerfile
--rw-r--r--   0 runner     (501) staff       (20)    11357 2022-02-01 05:08:30.000000 chiapos-1.0.9/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     4195 2022-02-01 05:09:02.064738 chiapos-1.0.9/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3833 2022-02-01 05:08:30.000000 chiapos-1.0.9/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.994817 chiapos-1.0.9/chiapos.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     4195 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4740 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)        8 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/top_level.txt
--rwxr-xr-x   0 runner     (501) staff       (20)       41 2022-02-01 05:08:30.000000 chiapos-1.0.9/docker-build.sh
--rwxr-xr-x   0 runner     (501) staff       (20)       57 2022-02-01 05:08:30.000000 chiapos-1.0.9/docker-test.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.001801 chiapos-1.0.9/documents/
--rw-r--r--   0 runner     (501) staff       (20)      398 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/README.txt
--rw-r--r--   0 runner     (501) staff       (20)   224153 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/bucket_graph.pdf
--rw-r--r--   0 runner     (501) staff       (20)   116670 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/code_documentation.pdf
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.005189 chiapos-1.0.9/documents/images/
--rw-r--r--   0 runner     (501) staff       (20)    13861 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/aesctr.png
--rw-r--r--   0 runner     (501) staff       (20)    62757 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/beyondhellman.png
--rw-r--r--   0 runner     (501) staff       (20)    67446 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/beyondhellman2.png
--rw-r--r--   0 runner     (501) staff       (20)   146667 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/pointerformat.png
--rw-r--r--   0 runner     (501) staff       (20)    40389 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/proofofspace.png
--rw-r--r--   0 runner     (501) staff       (20)  1368315 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/proof_of_space.html
--rw-r--r--   0 runner     (501) staff       (20)    75263 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/proof_of_space.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.013658 chiapos-1.0.9/hellman_example/
--rw-r--r--   0 runner     (501) staff       (20)    85217 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/Hellman attacks.pdf
--rw-r--r--   0 runner     (501) staff       (20)      353 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/Makefile
--rw-r--r--   0 runner     (501) staff       (20)    10179 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/aes.hpp
--rw-r--r--   0 runner     (501) staff       (20)    22632 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/bits.hpp
--rw-r--r--   0 runner     (501) staff       (20)    15920 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/calculate_bucket.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8358 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/cli.cpp
--rw-r--r--   0 runner     (501) staff       (20)    41970 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/cxxopts.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6187 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/encoding.hpp
--rw-r--r--   0 runner     (501) staff       (20)    13236 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/hellman.hpp
--rw-r--r--   0 runner     (501) staff       (20)    13016 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/picosha2.hpp
--rw-r--r--   0 runner     (501) staff       (20)    78714 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/plotter_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2766 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/pos_constants.hpp
--rw-r--r--   0 runner     (501) staff       (20)    28580 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/prover_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)      433 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/readme.md
--rw-r--r--   0 runner     (501) staff       (20)    34630 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/sort_on_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6605 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/util.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5474 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/verifier.hpp
--rw-r--r--   0 runner     (501) staff       (20)      343 2022-02-01 05:08:30.000000 chiapos-1.0.9/lgtm.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.981036 chiapos-1.0.9/lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.014940 chiapos-1.0.9/lib/FiniteStateEntropy/
--rw-r--r--   0 runner     (501) staff       (20)     1293 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     3636 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.979475 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.015366 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.016303 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/
--rw-r--r--   0 runner     (501) staff       (20)    10066 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
--rw-r--r--   0 runner     (501) staff       (20)     1414 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
--rw-r--r--   0 runner     (501) staff       (20)     2821 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.016728 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
--rw-r--r--   0 runner     (501) staff       (20)     8930 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.017677 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/
--rw-r--r--   0 runner     (501) staff       (20)     1414 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
--rw-r--r--   0 runner     (501) staff       (20)    10601 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
--rw-r--r--   0 runner     (501) staff       (20)     5026 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.026654 chiapos-1.0.9/lib/FiniteStateEntropy/lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.027611 chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/
--rw-r--r--   0 runner     (501) staff       (20)     2928 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/hufx6.h
--rw-r--r--   0 runner     (501) staff       (20)    18735 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
--rw-r--r--   0 runner     (501) staff       (20)     1579 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/README.md
--rw-r--r--   0 runner     (501) staff       (20)    18204 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/bitstream.h
--rw-r--r--   0 runner     (501) staff       (20)     3919 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/compiler.h
--rw-r--r--   0 runner     (501) staff       (20)     1912 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/debug.c
--rw-r--r--   0 runner     (501) staff       (20)     4605 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/debug.h
--rw-r--r--   0 runner     (501) staff       (20)     9599 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/entropy_common.c
--rw-r--r--   0 runner     (501) staff       (20)     4375 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/error_private.h
--rw-r--r--   0 runner     (501) staff       (20)     2434 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/error_public.h
--rw-r--r--   0 runner     (501) staff       (20)    32982 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse.h
--rw-r--r--   0 runner     (501) staff       (20)    11446 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fseU16.c
--rw-r--r--   0 runner     (501) staff       (20)     3570 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fseU16.h
--rw-r--r--   0 runner     (501) staff       (20)    27523 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse_compress.c
--rw-r--r--   0 runner     (501) staff       (20)    11179 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse_decompress.c
--rw-r--r--   0 runner     (501) staff       (20)     7926 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/hist.c
--rw-r--r--   0 runner     (501) staff       (20)     4327 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/hist.h
--rw-r--r--   0 runner     (501) staff       (20)    19479 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf.h
--rw-r--r--   0 runner     (501) staff       (20)    32593 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf_compress.c
--rw-r--r--   0 runner     (501) staff       (20)    45802 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf_decompress.c
--rw-r--r--   0 runner     (501) staff       (20)    11394 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/mem.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.036744 chiapos-1.0.9/lib/FiniteStateEntropy/programs/
--rw-r--r--   0 runner     (501) staff       (20)    18092 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/COPYING
--rw-r--r--   0 runner     (501) staff       (20)      287 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/README.md
--rw-r--r--   0 runner     (501) staff       (20)    29002 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/bench.c
--rw-r--r--   0 runner     (501) staff       (20)     1455 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/bench.h
--rw-r--r--   0 runner     (501) staff       (20)    12301 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/commandline.c
--rw-r--r--   0 runner     (501) staff       (20)     4444 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/cpu.h
--rw-r--r--   0 runner     (501) staff       (20)    22894 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fileio.c
--rw-r--r--   0 runner     (501) staff       (20)     2073 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fileio.h
--rw-r--r--   0 runner     (501) staff       (20)    19607 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fseDist.c
--rw-r--r--   0 runner     (501) staff       (20)     1608 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fseDist.h
--rw-r--r--   0 runner     (501) staff       (20)    44827 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fullbench.c
--rw-r--r--   0 runner     (501) staff       (20)    20262 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzer.c
--rw-r--r--   0 runner     (501) staff       (20)    14122 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
--rw-r--r--   0 runner     (501) staff       (20)    13406 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzerU16.c
--rw-r--r--   0 runner     (501) staff       (20)     4406 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/probaGenerator.c
--rw-r--r--   0 runner     (501) staff       (20)    28510 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/xxhash.c
--rw-r--r--   0 runner     (501) staff       (20)    12352 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/xxhash.h
--rw-r--r--   0 runner     (501) staff       (20)    68887 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/zlibh.c
--rw-r--r--   0 runner     (501) staff       (20)     4817 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/zlibh.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.037165 chiapos-1.0.9/lib/include/
--rw-r--r--   0 runner     (501) staff       (20)    13016 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/include/picosha2.hpp
--rw-r--r--   0 runner     (501) staff       (20)       37 2022-02-01 05:08:30.000000 chiapos-1.0.9/mypi.ini
--rw-r--r--   0 runner     (501) staff       (20)      194 2022-02-01 05:08:30.000000 chiapos-1.0.9/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.037596 chiapos-1.0.9/python-bindings/
--rw-r--r--   0 runner     (501) staff       (20)     6452 2022-02-01 05:08:30.000000 chiapos-1.0.9/python-bindings/chiapos.cpp
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-02-01 05:09:02.065398 chiapos-1.0.9/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     7006 2022-02-01 05:08:30.000000 chiapos-1.0.9/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.051625 chiapos-1.0.9/src/
--rw-r--r--   0 runner     (501) staff       (20)    21159 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b17phase2.hpp
--rw-r--r--   0 runner     (501) staff       (20)    21395 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b17phase3.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8685 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b17phase4.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11996 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b17sort_manager.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.056936 chiapos-1.0.9/src/b3/
--rw-r--r--   0 runner     (501) staff       (20)    26722 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3.c
--rw-r--r--   0 runner     (501) staff       (20)     1759 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3.h
--rw-r--r--   0 runner     (501) staff       (20)    12411 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_avx2.c
--rw-r--r--   0 runner     (501) staff       (20)    65803 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_avx2_x86-64_unix.S
--rw-r--r--   0 runner     (501) staff       (20)    47960 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_avx512.c
--rw-r--r--   0 runner     (501) staff       (20)    89081 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_avx512_x86-64_unix.S
--rw-r--r--   0 runner     (501) staff       (20)     6764 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_dispatch.c
--rw-r--r--   0 runner     (501) staff       (20)     8423 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_impl.h
--rw-r--r--   0 runner     (501) staff       (20)     6078 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_portable.c
--rw-r--r--   0 runner     (501) staff       (20)    20772 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_sse41.c
--rw-r--r--   0 runner     (501) staff       (20)    60859 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_sse41_x86-64_unix.S
--rw-r--r--   0 runner     (501) staff       (20)     2144 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/bitfield.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2223 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/bitfield_index.hpp
--rw-r--r--   0 runner     (501) staff       (20)    19655 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/bits.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11224 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/calculate_bucket.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4292 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/chacha8.c
--rw-r--r--   0 runner     (501) staff       (20)      431 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/chacha8.h
--rw-r--r--   0 runner     (501) staff       (20)     1104 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/chia_filesystem.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11257 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/cli.cpp
--rw-r--r--   0 runner     (501) staff       (20)    16417 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     7635 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/encoding.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4427 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/entry_sizes.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1449 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/exceptions.hpp
--rw-r--r--   0 runner     (501) staff       (20)    32661 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phase1.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11324 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phase2.hpp
--rw-r--r--   0 runner     (501) staff       (20)    23014 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phase3.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8587 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phase4.hpp
--rw-r--r--   0 runner     (501) staff       (20)      799 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phases.hpp
--rw-r--r--   0 runner     (501) staff       (20)    19237 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/plotter_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3819 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/pos_constants.hpp
--rw-r--r--   0 runner     (501) staff       (20)      284 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/progress.hpp
--rw-r--r--   0 runner     (501) staff       (20)    28981 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/prover_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3272 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/quicksort.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11844 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/sort_manager.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1853 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/threading.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4253 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/uniformsort.hpp
--rw-r--r--   0 runner     (501) staff       (20)    10882 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/util.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6193 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/verifier.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.059710 chiapos-1.0.9/tests/
--rw-r--r--   0 runner     (501) staff       (20)       31 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/.flake8
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6367 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/plot-resources.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/test-main.cpp
--rw-r--r--   0 runner     (501) staff       (20)    36230 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/test.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5403 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/test_python_bindings.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.060519 chiapos-1.0.9/tools/
--rwxr-xr-x   0 runner     (501) staff       (20)      879 2022-02-01 05:08:30.000000 chiapos-1.0.9/tools/disk.gnuplot
--rw-r--r--   0 runner     (501) staff       (20)      864 2022-02-01 05:08:30.000000 chiapos-1.0.9/tools/parse_disk.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.064131 chiapos-1.0.9/uint128_t/
--rw-r--r--   0 runner     (501) staff       (20)     1108 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     1385 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1124 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/endianness.h
--rw-r--r--   0 runner     (501) staff       (20)      203 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t.build
--rw-r--r--   0 runner     (501) staff       (20)    13671 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t.cpp
--rw-r--r--   0 runner     (501) staff       (20)      180 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t.h
--rw-r--r--   0 runner     (501) staff       (20)    19685 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t.include
--rw-r--r--   0 runner     (501) staff       (20)      653 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t_config.include
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.598599 chiapos-2.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.570598 chiapos-2.0.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.574598 chiapos-2.0.0b1/.github/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1855 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.github/actions/fetch_bladebit_harvester.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.574598 chiapos-2.0.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.github/workflows/build-test-cplusplus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.github/workflows/doc-html-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.github/workflows/manual-plot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.github/workflows/plot-k27-no-bitfield.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.github/workflows/plot-k27.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-29 23:31:37.598599 chiapos-2.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.574598 chiapos-2.0.0b1/chiapos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-29 23:31:37.000000 chiapos-2.0.0b1/chiapos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-29 23:31:37.000000 chiapos-2.0.0b1/chiapos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:31:37.000000 chiapos-2.0.0b1/chiapos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:31:37.000000 chiapos-2.0.0b1/chiapos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 23:31:37.000000 chiapos-2.0.0b1/chiapos.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/docker-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/docker-test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.578598 chiapos-2.0.0b1/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   224153 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/bucket_graph.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   116670 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/code_documentation.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.578598 chiapos-2.0.0b1/documents/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/images/aesctr.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/images/beyondhellman.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67446 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/images/beyondhellman2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/images/pointerformat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/images/proofofspace.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1368315 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/proof_of_space.html
+-rw-r--r--   0 runner    (1001) docker     (123)    75267 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/documents/proof_of_space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.582599 chiapos-2.0.0b1/hellman_example/
+-rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/Hellman attacks.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/aes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/cxxopts.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/hellman.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    78714 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34630 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/sort_on_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/hellman_example/verifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lgtm.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.570598 chiapos-2.0.0b1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.582599 chiapos-2.0.0b1/lib/FiniteStateEntropy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.570598 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.582599 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.582599 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/FSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.582599 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.582599 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/libfse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.586598 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.586598 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/Archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/Archives/hufx6.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/debug.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/error_public.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fseU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fseU16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/hist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/hist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/huf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/mem.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.590599 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29002 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/bench.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/bench.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/commandline.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fileio.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fileio.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fseDist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fseDist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fullbench.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fuzzerU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/probaGenerator.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28510 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (123)    68887 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/zlibh.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/zlibh.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.590599 chiapos-2.0.0b1/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/lib/include/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.590599 chiapos-2.0.0b1/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/python-bindings/chiapos.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 23:31:37.598599 chiapos-2.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.594599 chiapos-2.0.0b1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b17phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b17phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b17phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b17sort_manager.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.594599 chiapos-2.0.0b1/src/b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3_avx2_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3_avx512.c
+-rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3_avx512_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3_dispatch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3_portable.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3_sse41.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60859 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/b3/blake3_sse41_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/bitfield.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/bitfield_index.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/chacha8.c
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/chacha8.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/chia_filesystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/entry_sizes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/exceptions.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/phase1.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/phases.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/progress.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/quicksort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/serialize.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/sort_manager.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/threading.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/uniformsort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/src/verifier.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.598599 chiapos-2.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/tests/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/tests/plot-resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/tests/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/tests/test_python_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.598599 chiapos-2.0.0b1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/tools/disk.gnuplot
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/tools/parse_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:31:37.598599 chiapos-2.0.0b1/uint128_t/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/uint128_t/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/uint128_t/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/uint128_t/endianness.h
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/uint128_t/uint128_t.build
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/uint128_t/uint128_t.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/uint128_t/uint128_t.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/uint128_t/uint128_t.include
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-29 23:31:27.000000 chiapos-2.0.0b1/uint128_t/uint128_t_config.include
```

### Comparing `chiapos-1.0.9/.github/workflows/build-test-cplusplus.yml` & `chiapos-2.0.0b1/.github/workflows/build-test-cplusplus.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 name: Build and Test C++
 
 on: [push, pull_request]
 
+concurrency:
+  group: ${{ github.ref }}-${{ github.workflow }}-${{ github.event_name }}--${{ (github.ref == 'refs/heads/main' || startsWith(github.ref, 'refs/heads/release/') || startsWith(github.ref, 'refs/heads/long_lived/')) && github.sha || '' }}
+  cancel-in-progress: true
+
 jobs:
   valgrind:
     name: valgrind ubuntu
     runs-on: ubuntu-20.04
     steps:
-
-      - name: Cancel previous runs on the same branch
-        if: ${{ github.ref != 'refs/heads/main' }}
-        uses: styfle/cancel-workflow-action@0.9.1
-        with:
-          access_token: ${{ github.token }}
-
       - name: Checkout code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: cmake, RunTests, and valgrind on ubuntu-20.04
         run: |
           sudo apt update
           sudo apt-get install valgrind -y
           mkdir build
           cd build
@@ -28,23 +25,16 @@
           ctest -j 6 --output-on-failure
           valgrind --leak-check=full --show-leak-kinds=all --errors-for-leak-kinds=all ctest -j 6 --output-on-failure
 
   asan:
     name: ASAN ubuntu
     runs-on: ubuntu-20.04
     steps:
-
-      - name: Cancel previous runs on the same branch
-        if: ${{ github.ref != 'refs/heads/main' }}
-        uses: styfle/cancel-workflow-action@0.9.1
-        with:
-          access_token: ${{ github.token }}
-
       - name: Checkout code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: cmake, RunTests with address- and undefined sanitizer on Ubuntu
         run: |
           sudo fallocate -l 16G /swapfile
           sudo chmod 600 /swapfile
           sudo mkswap /swapfile
           sudo swapon /swapfile
@@ -56,44 +46,31 @@
           swapon -s
           ./RunTests
 
   tsan:
     name: TSAN ubuntu
     runs-on: ubuntu-20.04
     steps:
-      - name: Cancel previous runs on the same branch
-        if: ${{ github.ref != 'refs/heads/main' }}
-        uses: styfle/cancel-workflow-action@0.9.1
-        with:
-          access_token: ${{ github.token }}
-
       - name: Checkout code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: cmake, RunTests with thread sanitizer on Ubuntu
         run: |
           mkdir build-tsan
           cd build-tsan
           cmake -DCMAKE_BUILD_TYPE=TSAN ../
           cmake --build . -- -j 6
           TSAN_OPTIONS="memory_limit_mb=6000" ./RunTests
 
   windows:
     name: Windows Latest
     runs-on: windows-latest
     steps:
-
-    - name: Cancel previous runs on the same branch
-      if: ${{ github.ref != 'refs/heads/main' }}
-      uses: styfle/cancel-workflow-action@0.9.1
-      with:
-        access_token: ${{ github.token }}
-
     - name: Checkout code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
 
     - name: cmake, RunTests with Windows
       run: |
         mkdir build-win
         cd build-win
         cmake ..
         cmake --build . --config Release -j 6
```

### Comparing `chiapos-1.0.9/.github/workflows/doc-html-pdf.yml` & `chiapos-2.0.0b1/.github/workflows/doc-html-pdf.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 name: Build PoSpace Doc
 
 on: [workflow_dispatch]
 
+concurrency:
+  group: ${{ github.ref }}-${{ github.workflow }}-${{ github.event_name }}--${{ (github.ref == 'refs/heads/main' || startsWith(github.ref, 'refs/heads/release/') || startsWith(github.ref, 'refs/heads/long_lived/')) && github.sha || '' }}
+  cancel-in-progress: true
+
 jobs:
   html_to_pdf:
     name: Generate PDF of PoSpace Doc
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
 
     steps:
-    - name: Cancel previous runs on the same branch
-      if: ${{ github.ref != 'refs/heads/main' }}
-      uses: styfle/cancel-workflow-action@0.9.1
-      with:
-        access_token: ${{ github.token }}
-
     - name: Checkout code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
 
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v4
       name: Install Python
       with:
         python-version: '3.8'
 
     - name: Install python markdown
       shell: bash
       run: |
@@ -33,18 +31,18 @@
          source venv/bin/activate
          python -m pip install --upgrade pip
          pip install markdown
          pip install python-markdown-math
 #         python -m markdown -x mdx_math --verbose -f proof_of_space.html proof_of_space.md
 
     - name: html to pdf
-      uses: fifsky/html-to-pdf-action@master
+      uses: fifsky/html-to-pdf-action@v0.1
       with:
         htmlFile: ./documents/proof_of_space.html
         outputFile: ./documents/proof_of_space.pdf
         pdfOptions: '{"margin": {"top": "1cm", "left": "1cm", "right": "1cm", "bottom": "1cm"}}'
 
     - name: Upload artifacts
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: Proof-of-Space-Document
         path: ./documents/proof_of_space.pdf
```

### Comparing `chiapos-1.0.9/.github/workflows/manual-plot.yml` & `chiapos-2.0.0b1/.github/workflows/manual-plot.yml`

 * *Files 16% similar despite different names*

```diff
@@ -19,36 +19,35 @@
         required: true
         default: '1'
       k_size:
         description: 'The K size to plot'
         required: true
         default: '27'
 
+concurrency:
+  group: ${{ github.ref }}-${{ github.workflow }}-${{ github.event_name }}--${{ (github.ref == 'refs/heads/main' || startsWith(github.ref, 'refs/heads/release/') || startsWith(github.ref, 'refs/heads/long_lived/')) && github.sha || '' }}
+  cancel-in-progress: true
+
 jobs:
   Plot:
     name: Call Plotter
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
 
     steps:
-    - name: Cancel previous runs on the same branch
-      uses: styfle/cancel-workflow-action@0.9.1
-      with:
-        access_token: ${{ github.token }}
-
     - name: Test for secrets access
       id: check_secrets
       shell: bash
       run: |
         unset HAS_SECRET
         if [ -n "$SECRET" ]; then HAS_SECRET='true' ; fi
-        echo ::set-output name=HAS_SECRET::${HAS_SECRET}
+        echo "HAS_SECRET=${HAS_SECRET}" >>$GITHUB_OUTPUT
       env:
         SECRET: "${{ secrets.TEST_WEBHOOK_SECRET }}"
 
     #${{ secrets.REPO_ADMIN }}
     - name: Plot
       run: |
         curl -XPOST -H "Authorization: token ${{ secrets.WEBHOOK_CREDENTIAL }}" -H "Accept: application/vnd.github.v3+json" -H "Content-Type: application/json" https://api.github.com/repos/Chia-Network/chia-plotter/actions/workflows/chia-plotter.yml/dispatches --data '{"ref": "main", "inputs": {  "upstream_branch": "${{ github.event.inputs.upstream_branch }}", "instance_name_tag": "${{ github.event.inputs.instance_name_tag }}", "commit_sha": "${{ github.event.inputs.commit_sha}}", "ksize": "${{ github.event.inputs.k_size }}", "count": "${{ github.event.inputs.count }}"  } }'
```

### Comparing `chiapos-1.0.9/.github/workflows/plot-k27-no-bitfield.yaml` & `chiapos-2.0.0b1/.github/workflows/plot-k27.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-name: Plot k=27 without bitfield
+name: Plot k=27
 
 on: [push, pull_request]
 
+concurrency:
+  group: ${{ github.ref }}-${{ github.workflow }}-${{ github.event_name }}--${{ (github.ref == 'refs/heads/main' || startsWith(github.ref, 'refs/heads/release/') || startsWith(github.ref, 'refs/heads/long_lived/')) && github.sha || '' }}
+  cancel-in-progress: true
+
 jobs:
   build_wheels:
     name: Plot k=27 on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
 
     steps:
-    - name: Cancel previous runs on the same branch
-      if: ${{ github.ref != 'refs/heads/main' }}
-      uses: styfle/cancel-workflow-action@0.9.1
-      with:
-        access_token: ${{ github.token }}
-
     - name: Checkout code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
 
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v4
       name: Install Python
       with:
         python-version: '3.8'
 
     - name: cmake, Plot k=27
       run: |
         mkdir build
@@ -33,12 +31,12 @@
         cmake ../
         cmake --build . -- -j 6
         mkdir plots
         mkdir plots/temp
         mkdir plots/final
         pip install wheel
         pip install psutil
-        python ../tests/plot-resources.py -k 27 -r 2 -e
+        python ../tests/plot-resources.py -k 27 -r 2
         EXPECTED_SHA="1f144aa10df010a557009c0c032926cfff58fd5e6b4a5317caca5c405b08163a  plots/final/plot.dat"
         SHACHECK=$(sha256sum plots/final/plot.dat)
         echo "$SHACHECK"
         if [ "$SHACHECK" != "$EXPECTED_SHA" ]; then echo "Sha256sum does not match"; exit 1; else echo "Sha256sum matches 0x1f144aa1...163a"; fi
```

### Comparing `chiapos-1.0.9/.github/workflows/plot-k27.yaml` & `chiapos-2.0.0b1/.github/workflows/plot-k27-no-bitfield.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-name: Plot k=27
+name: Plot k=27 without bitfield
 
 on: [push, pull_request]
 
+concurrency:
+  group: ${{ github.ref }}-${{ github.workflow }}-${{ github.event_name }}--${{ (github.ref == 'refs/heads/main' || startsWith(github.ref, 'refs/heads/release/') || startsWith(github.ref, 'refs/heads/long_lived/')) && github.sha || '' }}
+  cancel-in-progress: true
+
 jobs:
   build_wheels:
     name: Plot k=27 on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
 
     steps:
-    - name: Cancel previous runs on the same branch
-      if: ${{ github.ref != 'refs/heads/main' }}
-      uses: styfle/cancel-workflow-action@0.9.1
-      with:
-        access_token: ${{ github.token }}
-
     - name: Checkout code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
 
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v4
       name: Install Python
       with:
         python-version: '3.8'
 
     - name: cmake, Plot k=27
       run: |
         mkdir build
@@ -33,12 +31,12 @@
         cmake ../
         cmake --build . -- -j 6
         mkdir plots
         mkdir plots/temp
         mkdir plots/final
         pip install wheel
         pip install psutil
-        python ../tests/plot-resources.py -k 27 -r 2
+        python ../tests/plot-resources.py -k 27 -r 2 -e
         EXPECTED_SHA="1f144aa10df010a557009c0c032926cfff58fd5e6b4a5317caca5c405b08163a  plots/final/plot.dat"
         SHACHECK=$(sha256sum plots/final/plot.dat)
         echo "$SHACHECK"
         if [ "$SHACHECK" != "$EXPECTED_SHA" ]; then echo "Sha256sum does not match"; exit 1; else echo "Sha256sum matches 0x1f144aa1...163a"; fi
```

### Comparing `chiapos-1.0.9/.github/workflows/stale-issue.yml` & `chiapos-2.0.0b1/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/CMakeLists.txt` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,53 +12,40 @@
 endif()
 
 project(chiapos C CXX ASM)
 
 # CMake 3.14+
 include(FetchContent)
 
-if (${CMAKE_SYSTEM_NAME} MATCHES "FreeBSD")
-include(${CMAKE_INSTALL_PREFIX}/share/cmake/pybind11/pybind11Config.cmake)
-else()
 FetchContent_Declare(
   pybind11-src
   GIT_REPOSITORY https://github.com/pybind/pybind11.git
-  GIT_TAG        v2.7.1
+  GIT_TAG        v2.6.2
 )
 FetchContent_MakeAvailable(pybind11-src)
-endif()
-
-FetchContent_Declare(
-  cxxopts
-  GIT_REPOSITORY https://github.com/jarro2783/cxxopts.git
-  GIT_TAG        v2.2.1
-)
-FetchContent_MakeAvailable(cxxopts)
 
 FetchContent_Declare(
-  gulrak
-  GIT_REPOSITORY https://github.com/gulrak/filesystem.git
-  GIT_TAG        v1.5.6
+  fse
+  GIT_REPOSITORY https://github.com/Cyan4973/FiniteStateEntropy.git
+  GIT_TAG        510d22b221c8c02f281c35f9edeb606baacef27b
 )
-FetchContent_MakeAvailable(gulrak)
+FetchContent_MakeAvailable(fse)
 
-set(FSE_LIB ${CMAKE_CURRENT_SOURCE_DIR}/lib/FiniteStateEntropy/lib)
+set(FSE_LIB ${fse_SOURCE_DIR}/lib)
 set(FSE_FILES
     ${FSE_LIB}/fse_compress.c
     ${FSE_LIB}/fse_decompress.c
     ${FSE_LIB}/entropy_common.c
     ${FSE_LIB}/hist.c
 )
 
 include_directories(
   ${INCLUDE_DIRECTORIES}
   ${CMAKE_CURRENT_SOURCE_DIR}/../lib/include
-  ${cxxopts_SOURCE_DIR}/include
-  ${gulrak_SOURCE_DIR}/include/ghc
-  ${CMAKE_CURRENT_SOURCE_DIR}/../lib/FiniteStateEntropy/lib
+  ${FSE_LIB}
   ${CMAKE_CURRENT_SOURCE_DIR}/src
   ${CMAKE_CURRENT_SOURCE_DIR}/test
   )
 
 add_library(fse ${FSE_FILES})
 
 IF (MSVC)
@@ -84,22 +71,22 @@
 
 set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -g")
 set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -g")
 
 ENDIF()
 
 IF (CMAKE_BUILD_TYPE STREQUAL "ASAN")
-set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O1 -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
-set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -O1 -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
+set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
+set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
 set (CMAKE_LINKER_FLAGS "${CMAKE_LINKER_FLAGS} -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
 ENDIF()
 
 IF (CMAKE_BUILD_TYPE STREQUAL "TSAN")
-set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O2 -fno-omit-frame-pointer -fsanitize=thread")
-set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -O2 -fno-omit-frame-pointer -fsanitize=thread")
+set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fno-omit-frame-pointer -fsanitize=thread")
+set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fno-omit-frame-pointer -fsanitize=thread")
 set (CMAKE_LINKER_FLAGS "${CMAKE_LINKER_FLAGS} -fno-omit-frame-pointer -fsanitize=thread")
 ENDIF()
 
 IF (APPLE)
 # on macOS "uname -m" returns the architecture (x86_64 or arm64)
 execute_process(
     COMMAND uname -m
@@ -138,64 +125,47 @@
 
 add_executable(ProofOfSpace
     src/cli.cpp
     src/chacha8.c
     ${BLAKE3_SRC}
 )
 
-option(BUILD_PROOF_OF_SPACE_STATICALLY "Build ProofOfSpace target statically" OFF)
-IF (BUILD_PROOF_OF_SPACE_STATICALLY)
-  message("Statically build ProofOfSpace")
-  target_link_libraries(ProofOfSpace -static -Wl,--whole-archive -lrt -lpthread -Wl,--no-whole-archive)
-ENDIF()
-
-FetchContent_Declare(
-  Catch2
-  GIT_REPOSITORY https://github.com/catchorg/Catch2.git
-  GIT_TAG        v2.13.7
-)
-FetchContent_MakeAvailable(Catch2)
-
 add_executable(RunTests
     tests/test-main.cpp
     tests/test.cpp
     src/chacha8.c
     ${BLAKE3_SRC}
 )
 
-target_link_libraries(RunTests
-  PRIVATE
-    fse
-    Threads::Threads
-    Catch2::Catch2
-)
-
 find_package(Threads REQUIRED)
 
 add_library(uint128 STATIC uint128_t/uint128_t.cpp)
 target_include_directories(uint128 PUBLIC uint128_t)
 
 target_compile_features(fse PUBLIC cxx_std_17)
 target_compile_features(chiapos PUBLIC cxx_std_17)
 target_compile_features(RunTests PUBLIC cxx_std_17)
 
 if (${CMAKE_SYSTEM_NAME} MATCHES "Darwin")
   target_link_libraries(chiapos PRIVATE fse Threads::Threads)
   target_link_libraries(ProofOfSpace fse Threads::Threads)
+  target_link_libraries(RunTests fse Threads::Threads)
 elseif (${CMAKE_SYSTEM_NAME} MATCHES "OpenBSD")
   target_link_libraries(chiapos PRIVATE fse Threads::Threads)
   target_link_libraries(ProofOfSpace fse Threads::Threads)
+  target_link_libraries(RunTests fse Threads::Threads)
 elseif (${CMAKE_SYSTEM_NAME} MATCHES "FreeBSD")
   target_link_libraries(chiapos PRIVATE fse Threads::Threads)
   target_link_libraries(ProofOfSpace fse Threads::Threads)
+  target_link_libraries(RunTests fse Threads::Threads)
 elseif (MSVC)
   target_link_libraries(chiapos PRIVATE fse Threads::Threads uint128)
   target_link_libraries(ProofOfSpace fse Threads::Threads uint128)
-  target_link_libraries(RunTests PRIVATE uint128)
+  target_link_libraries(RunTests fse Threads::Threads uint128)
 else()
   target_link_libraries(chiapos PRIVATE fse stdc++fs Threads::Threads)
   target_link_libraries(ProofOfSpace fse stdc++fs Threads::Threads)
-  target_link_libraries(RunTests PRIVATE stdc++fs)
+  target_link_libraries(RunTests fse stdc++fs Threads::Threads)
 endif()
 
 enable_testing()
 add_test(NAME RunTests COMMAND RunTests)
```

### Comparing `chiapos-1.0.9/Dockerfile` & `chiapos-2.0.0b1/Dockerfile`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/LICENSE` & `chiapos-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/PKG-INFO` & `chiapos-2.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 1.0.9
+Version: 2.0.0b1
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chia Proof of Space
 ![Build](https://github.com/Chia-Network/chiapos/workflows/Build/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/chiapos?logo=pypi)
@@ -118,9 +117,7 @@
 chia-blockchain requires in it's main/release version in preparation for a
 new chia-blockchain release. Please branch or fork main and then create a
 pull request to the main branch. Linear merging is enforced on main and
 merging requires a completed review. PRs will kick off a GitHub actions ci build
 and analysis of chiapos at
 [lgtm.com](https://lgtm.com/projects/g/Chia-Network/chiapos/?mode=list). Please
 make sure your build is passing and that it does not increase alerts at lgtm.
-
-
```

### Comparing `chiapos-1.0.9/README.md` & `chiapos-2.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/chiapos.egg-info/PKG-INFO` & `chiapos-2.0.0b1/chiapos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 1.0.9
+Version: 2.0.0b1
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chia Proof of Space
 ![Build](https://github.com/Chia-Network/chiapos/workflows/Build/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/chiapos?logo=pypi)
@@ -118,9 +117,7 @@
 chia-blockchain requires in it's main/release version in preparation for a
 new chia-blockchain release. Please branch or fork main and then create a
 pull request to the main branch. Linear merging is enforced on main and
 merging requires a completed review. PRs will kick off a GitHub actions ci build
 and analysis of chiapos at
 [lgtm.com](https://lgtm.com/projects/g/Chia-Network/chiapos/?mode=list). Please
 make sure your build is passing and that it does not increase alerts at lgtm.
-
-
```

### Comparing `chiapos-1.0.9/chiapos.egg-info/SOURCES.txt` & `chiapos-2.0.0b1/chiapos.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 docker-build.sh
 docker-test.sh
 lgtm.yml
 mypi.ini
 pyproject.toml
 setup.py
 ./
-.github/workflows/build-aarch64.yml
-.github/workflows/build-m1-wheel.yml
+.github/actions/fetch_bladebit_harvester.sh
 .github/workflows/build-test-cplusplus.yml
 .github/workflows/build-wheels.yml
 .github/workflows/doc-html-pdf.yml
 .github/workflows/manual-plot.yml
 .github/workflows/plot-k27-no-bitfield.yaml
 .github/workflows/plot-k27.yaml
 .github/workflows/stale-issue.yml
@@ -127,14 +126,15 @@
 src/phase4.hpp
 src/phases.hpp
 src/plotter_disk.hpp
 src/pos_constants.hpp
 src/progress.hpp
 src/prover_disk.hpp
 src/quicksort.hpp
+src/serialize.hpp
 src/sort_manager.hpp
 src/threading.hpp
 src/uniformsort.hpp
 src/util.hpp
 src/verifier.hpp
 src/b3/blake3.c
 src/b3/blake3.h
@@ -146,15 +146,14 @@
 src/b3/blake3_impl.h
 src/b3/blake3_portable.c
 src/b3/blake3_sse41.c
 src/b3/blake3_sse41_x86-64_unix.S
 tests/.flake8
 tests/__init__.py
 tests/plot-resources.py
-tests/test-main.cpp
 tests/test.cpp
 tests/test_python_bindings.py
 tools/disk.gnuplot
 tools/parse_disk.py
 uint128_t/LICENSE
 uint128_t/README.md
 uint128_t/endianness.h
```

### Comparing `chiapos-1.0.9/documents/bucket_graph.pdf` & `chiapos-2.0.0b1/documents/bucket_graph.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/documents/code_documentation.pdf` & `chiapos-2.0.0b1/documents/code_documentation.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/documents/images/aesctr.png` & `chiapos-2.0.0b1/documents/images/aesctr.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/documents/images/beyondhellman.png` & `chiapos-2.0.0b1/documents/images/beyondhellman.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/documents/images/beyondhellman2.png` & `chiapos-2.0.0b1/documents/images/beyondhellman2.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/documents/images/pointerformat.png` & `chiapos-2.0.0b1/documents/images/pointerformat.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/documents/images/proofofspace.png` & `chiapos-2.0.0b1/documents/images/proofofspace.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/documents/proof_of_space.html` & `chiapos-2.0.0b1/documents/proof_of_space.html`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/documents/proof_of_space.md` & `chiapos-2.0.0b1/documents/proof_of_space.md`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,15 @@
 | $Table_{3}$ | $E_{\{3, i\}}=pos_{2;L}, pos_{2;R}$ | Mapped to line point, deltafied, encoded, and parked | $0.807*2^k$                         |
 | $Table_{4}$ | $E_{\{4, i\}}=pos_{3;L}, pos_{3;R}$ | Mapped to line point, deltafied, encoded, and parked | $0.823*2^k$                         |
 | $Table_{5}$ | $E_{\{5, i\}}=pos_{4;L}, pos_{4;R}$ | Mapped to line point, deltafied, encoded, and parked | $0.865*2^k$                         |
 | $Table_{6}$ | $E_{\{6, i\}}=pos_{5;L}, pos_{5;R}$ | Mapped to line point, deltafied, encoded, and parked | $2^k$                         |
 | $Table_{7}$ | $E_{\{7, i\}}=pos_{6;L}$            | Parked                                               | $2^k$                               |
 | $C_{1}$     | $f_7$                               | Byte aligned storage                                 | $\frac{2^k}{param\_c_1}$            |
 | $C_{2}$     | $f_7$                               | Byte aligned storage                                 | $\frac{2^k}{param\_c_1*param\_c_2}$ |
-| $C_{3}$     | $f_7$                               | Deltafied, encoded, and parked                       | $\frac{2^k}{param\_c_1}$            |
+| $C_{3}$     | $f_7$                               | Deltafied, encoded, and parked                       | $2^k-\frac{2^k}{param\_c_1}$            |
 
 ##### Full algorithm
 
 The plotting algorithm $\text{PlotAlgo1}$ takes as input a unique $\text{plot\_seed} \in [2^{256}]$, a space parameter $30 \leq k \leq 50$, a param object $param$, and deterministically outputs a final file $F$.
 
 $Sort$, or sort on disk, takes in a table on disk, and performs a full ascending sort, starting at a specified bit position.
```

### Comparing `chiapos-1.0.9/hellman_example/Hellman attacks.pdf` & `chiapos-2.0.0b1/hellman_example/Hellman attacks.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/aes.hpp` & `chiapos-2.0.0b1/hellman_example/aes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/bits.hpp` & `chiapos-2.0.0b1/hellman_example/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/calculate_bucket.hpp` & `chiapos-2.0.0b1/hellman_example/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/cli.cpp` & `chiapos-2.0.0b1/hellman_example/cli.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/cxxopts.hpp` & `chiapos-2.0.0b1/hellman_example/cxxopts.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/encoding.hpp` & `chiapos-2.0.0b1/hellman_example/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/hellman.hpp` & `chiapos-2.0.0b1/hellman_example/hellman.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/picosha2.hpp` & `chiapos-2.0.0b1/hellman_example/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/plotter_disk.hpp` & `chiapos-2.0.0b1/hellman_example/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/pos_constants.hpp` & `chiapos-2.0.0b1/hellman_example/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/prover_disk.hpp` & `chiapos-2.0.0b1/hellman_example/prover_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/sort_on_disk.hpp` & `chiapos-2.0.0b1/hellman_example/sort_on_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/util.hpp` & `chiapos-2.0.0b1/hellman_example/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/hellman_example/verifier.hpp` & `chiapos-2.0.0b1/hellman_example/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/LICENSE` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/README.md` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/hufx6.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/Archives/hufx6.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/README.md` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/bitstream.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/bitstream.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/compiler.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/compiler.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/debug.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/debug.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/debug.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/debug.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/entropy_common.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/entropy_common.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/error_private.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/error_private.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/error_public.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/error_public.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fse.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fseU16.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fseU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fseU16.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fseU16.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse_compress.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fse_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse_decompress.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/hist.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/hist.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/hist.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/hist.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/huf.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf_compress.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/huf_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf_decompress.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/lib/mem.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/lib/mem.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/COPYING` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/COPYING`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/bench.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/bench.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/bench.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/bench.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/commandline.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/commandline.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/cpu.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/cpu.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fileio.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fileio.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fileio.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fileio.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fseDist.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fseDist.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fseDist.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fseDist.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fullbench.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fullbench.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzer.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fuzzer.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzerHuff0.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fuzzerHuff0.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzerU16.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/fuzzerU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/probaGenerator.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/probaGenerator.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/xxhash.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/xxhash.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/xxhash.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/xxhash.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/zlibh.c` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/zlibh.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/FiniteStateEntropy/programs/zlibh.h` & `chiapos-2.0.0b1/lib/FiniteStateEntropy/programs/zlibh.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/lib/include/picosha2.hpp` & `chiapos-2.0.0b1/lib/include/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/python-bindings/chiapos.cpp` & `chiapos-2.0.0b1/python-bindings/chiapos.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -72,57 +72,77 @@
                 } catch (const std::exception &e) {
                     std::cout << "Caught plotting error: " << e.what() << std::endl;
                     throw e;
                 }
             });
 
     py::class_<DiskProver>(m, "DiskProver")
-        .def(py::init<const std::string &>())
+        .def(py::init<const std::string &>(), py::call_guard<py::gil_scoped_release>())
+        .def_static("from_bytes", [](const py::bytes &bytes) -> DiskProver {
+            py::buffer_info info(py::buffer(bytes).request());
+            auto data = reinterpret_cast<const uint8_t*>(info.ptr);
+            auto vecBytes = std::vector<uint8_t>(data, data + info.size);
+            py::gil_scoped_release release;
+            return DiskProver(vecBytes);
+        })
+        .def("__bytes__", [](DiskProver &dp) {
+            std::vector<uint8_t> vecBytes;
+            {
+                py::gil_scoped_release release;
+                vecBytes = dp.ToBytes();
+            }
+            return py::bytes(reinterpret_cast<const char*>(vecBytes.data()), vecBytes.size());
+        })
         .def(
             "get_memo",
             [](DiskProver &dp) {
                 const std::vector<uint8_t>& memo = dp.GetMemo();
                 return py::bytes(reinterpret_cast<const char*>(memo.data()), memo.size());
             })
         .def(
             "get_id",
             [](DiskProver &dp) {
                 const std::vector<uint8_t>& id = dp.GetId();
                 return py::bytes(reinterpret_cast<const char*>(id.data()), id.size());
             })
         .def("get_size", [](DiskProver &dp) { return dp.GetSize(); })
+        .def("get_compresion_level", [](DiskProver &dp) { return dp.GetCompressionLevel(); })
         .def("get_filename", [](DiskProver &dp) { return dp.GetFilename(); })
         .def(
             "get_qualities_for_challenge",
             [](DiskProver &dp, const py::bytes &challenge) {
                 if (len(challenge) != 32) {
                     throw std::invalid_argument("Challenge must be exactly 32 bytes");
                 }
                 std::string challenge_str(challenge);
                 const uint8_t *challenge_ptr =
                     reinterpret_cast<const uint8_t *>(challenge_str.data());
-                py::gil_scoped_release release;
-                std::vector<LargeBits> qualities = dp.GetQualitiesForChallenge(challenge_ptr);
-                py::gil_scoped_acquire acquire;
+                std::vector<LargeBits> qualities;
+                {
+                    py::gil_scoped_release release;
+                    qualities = dp.GetQualitiesForChallenge(challenge_ptr);
+                }
                 std::vector<py::bytes> ret;
                 uint8_t *quality_buf = new uint8_t[32];
                 for (LargeBits quality : qualities) {
                     quality.ToBytes(quality_buf);
                     py::bytes quality_py = py::bytes(reinterpret_cast<char *>(quality_buf), 32);
                     ret.push_back(quality_py);
                 }
                 delete[] quality_buf;
                 return ret;
             })
         .def("get_full_proof", [](DiskProver &dp, const py::bytes &challenge, uint32_t index, bool parallel_read) {
             std::string challenge_str(challenge);
             const uint8_t *challenge_ptr = reinterpret_cast<const uint8_t *>(challenge_str.data());
-            py::gil_scoped_release release;
-            LargeBits proof = dp.GetFullProof(challenge_ptr, index, parallel_read);
-            py::gil_scoped_acquire acquire;
+            LargeBits proof;
+            {
+                py::gil_scoped_release release;
+                proof = dp.GetFullProof(challenge_ptr, index, parallel_read);
+            }
             uint8_t *proof_buf = new uint8_t[Util::ByteAlign(64 * dp.GetSize()) / 8];
             proof.ToBytes(proof_buf);
             py::bytes ret = py::bytes(
                 reinterpret_cast<char *>(proof_buf), Util::ByteAlign(64 * dp.GetSize()) / 8);
             delete[] proof_buf;
             return ret;
         },py::arg("challenge"), py::arg("index"), py::arg("parallel_read") = true);
@@ -142,21 +162,28 @@
                 std::string challenge_str(challenge);
                 const uint8_t *challenge_ptr =
                     reinterpret_cast<const uint8_t *>(challenge_str.data());
 
                 std::string proof_str(proof);
                 const uint8_t *proof_ptr = reinterpret_cast<const uint8_t *>(proof_str.data());
 
-                LargeBits quality =
-                    v.ValidateProof(seed_ptr, k, challenge_ptr, proof_ptr, len(proof));
+                LargeBits quality;
+                {
+                    py::gil_scoped_release release;
+                    quality = v.ValidateProof(seed_ptr, k, challenge_ptr, proof_ptr, len(proof));
+                }
                 if (quality.GetSize() == 0) {
                     return stdx::optional<py::bytes>();
                 }
                 uint8_t *quality_buf = new uint8_t[32];
                 quality.ToBytes(quality_buf);
                 py::bytes quality_py = py::bytes(reinterpret_cast<char *>(quality_buf), 32);
                 delete[] quality_buf;
                 return stdx::optional<py::bytes>(quality_py);
             });
+
+    py::class_<ContextQueue>(m, "ContextQueue")
+        .def("init", &ContextQueue::init);
+    m.attr("decompresser_context_queue") = &decompresser_context_queue;
 }
 
 #endif  // PYTHON_BINDINGS_PYTHON_BINDINGS_HPP_
```

### Comparing `chiapos-1.0.9/setup.py` & `chiapos-2.0.0b1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python3
 import os
 import re
+import shutil
 import sys
 import platform
 import subprocess
 
 from setuptools import setup, setuptools, Extension
 from setuptools.command.build_ext import build_ext
 from distutils.version import LooseVersion
@@ -40,14 +41,17 @@
     def build_extension(self, ext):
         extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
         cmake_args = [
             "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=" + str(extdir),
             "-DPYTHON_EXECUTABLE=" + sys.executable,
         ]
 
+        if os.getenv("CP_USE_GREEN_REAPER") == "1":
+            cmake_args.append("-DCP_LINK_BLADEBIT_HARVESTER=ON")
+
         cfg = "Debug" if self.debug else "Release"
         build_args = ["--config", cfg]
 
         if platform.system() == "Windows":
             cmake_args += [
                 "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{}={}".format(cfg.upper(), extdir)
             ]
@@ -173,32 +177,45 @@
         if ct == "unix":
             opts.append('-DVERSION_INFO="%s"' % self.distribution.get_version())
             opts.append(cpp_flag(self.compiler))
             if has_flag(self.compiler, "-fvisibility=hidden"):
                 opts.append("-fvisibility=hidden")
         elif ct == "msvc":
             opts.append('/DVERSION_INFO=\\"%s\\"' % self.distribution.get_version())
+
+            # Link bladebit_harvester
+            if os.getenv("CP_USE_GREEN_REAPER") == "1":
+                opts.append("/DUSE_GREEN_REAPER=1")
+                opts.append("/DBLADEBIT_HARVESTER_LINKED=1")
+                opts.append("/Ilibs/green_reaper/include")
+                link_opts.append("libs/green_reaper/lib/bladebit_harvester.lib")
+
         for ext in self.extensions:
             ext.extra_compile_args = opts
             ext.extra_link_args = link_opts
         build_ext.build_extensions(self)
 
+        # Copy bladebit_harvester.dll on windows to the target build directory
+        # in order to package it into the root directory of the wheel
+        if os.getenv("CP_USE_GREEN_REAPER") == "1" and sys.platform == "win32":
+            shutil.copy2("libs/green_reaper/lib/bladebit_harvester.dll", self.build_lib + "/bladebit_harvester.dll")
+
 
 if platform.system() == "Windows":
     setup(
         name="chiapos",
         author="Mariano Sorgente",
         author_email="mariano@chia.net",
         description="Chia proof of space plotting, proving, and verifying (wraps C++)",
         license="Apache License",
         python_requires=">=3.7",
         long_description=open("README.md").read(),
         long_description_content_type="text/markdown",
         url="https://github.com/Chia-Network/chiapos",
-        setup_requires=["pybind11"],
+        setup_requires=["pybind11>=2.10.0"],
         tests_require=["pytest"],
         ext_modules=ext_modules,
         cmdclass={"build_ext": BuildExt},
         zip_safe=False,
     )
 else:
     setup(
```

### Comparing `chiapos-1.0.9/src/b17phase2.hpp` & `chiapos-2.0.0b1/src/b17phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b17phase3.hpp` & `chiapos-2.0.0b1/src/b17phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b17phase4.hpp` & `chiapos-2.0.0b1/src/b17phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b17sort_manager.hpp` & `chiapos-2.0.0b1/src/b17sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3.c` & `chiapos-2.0.0b1/src/b3/blake3.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3.h` & `chiapos-2.0.0b1/src/b3/blake3.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3_avx2.c` & `chiapos-2.0.0b1/src/b3/blake3_avx2.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3_avx2_x86-64_unix.S` & `chiapos-2.0.0b1/src/b3/blake3_avx2_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3_avx512.c` & `chiapos-2.0.0b1/src/b3/blake3_avx512.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3_avx512_x86-64_unix.S` & `chiapos-2.0.0b1/src/b3/blake3_avx512_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3_dispatch.c` & `chiapos-2.0.0b1/src/b3/blake3_dispatch.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3_impl.h` & `chiapos-2.0.0b1/src/b3/blake3_impl.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3_portable.c` & `chiapos-2.0.0b1/src/b3/blake3_portable.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3_sse41.c` & `chiapos-2.0.0b1/src/b3/blake3_sse41.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/b3/blake3_sse41_x86-64_unix.S` & `chiapos-2.0.0b1/src/b3/blake3_sse41_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/bitfield.hpp` & `chiapos-2.0.0b1/src/bitfield.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/bitfield_index.hpp` & `chiapos-2.0.0b1/src/bitfield_index.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/bits.hpp` & `chiapos-2.0.0b1/src/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/calculate_bucket.hpp` & `chiapos-2.0.0b1/src/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/chacha8.c` & `chiapos-2.0.0b1/src/chacha8.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/chia_filesystem.hpp` & `chiapos-2.0.0b1/src/chia_filesystem.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/cli.cpp` & `chiapos-2.0.0b1/src/cli.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,25 @@
     cout << "./ProofOfSpace create" << endl;
     cout << "./ProofOfSpace prove <challenge>" << endl;
     cout << "./ProofOfSpace verify <proof> <challenge>" << endl;
     cout << "./ProofOfSpace check" << endl;
     exit(0);
 }
 
+// Not thread safe
+inline void InitDecompresserQueueDefault(bool no_cuda = false)
+{
+    static bool initialized = false;
+    if (initialized) {
+        return;
+    }
+    decompresser_context_queue.init(1, (uint32_t)std::thread::hardware_concurrency(), false, 9, !no_cuda, 0, false);
+    initialized = true;
+}
+
 int main(int argc, char *argv[]) try {
     cxxopts::Options options(
         "ProofOfSpace", "Utility for plotting, generating and verifying proofs of space.");
     options.positional_help("(create/prove/verify/check) param1 param2 ")
         .show_positional_help();
 
     // Default values
@@ -157,14 +168,16 @@
                 id_bytes.size(),
                 buffmegabytes,
                 num_buckets,
                 num_stripes,
                 num_threads,
                 phases_flags);
     } else if (operation == "prove") {
+        InitDecompresserQueueDefault();
+
         if (argc < 3) {
             HelpAndQuit(options);
         }
         cout << "Proving using filename=" << filename << " challenge=" << argv[2] << endl
              << endl;
         string challenge = Strip0x(argv[2]);
         if (challenge.size() != 64) {
@@ -234,64 +247,71 @@
             cout << "Proof verification suceeded. Quality: " << quality << endl;
         } else {
             cout << "Proof verification failed." << endl;
             exit(1);
         }
         delete[] proof_bytes;
     } else if (operation == "check") {
+        InitDecompresserQueueDefault();
+
         uint32_t iterations = 1000;
         if (argc == 3) {
             iterations = std::stoi(argv[2]);
         }
 
         DiskProver prover(filename);
         Verifier verifier = Verifier();
 
         uint32_t success = 0;
+        uint32_t failures = 0;
+        uint32_t exceptions = 0;
         std::vector<uint8_t> id_bytes = prover.GetId();
         k = prover.GetSize();
 
         for (uint32_t num = 0; num < iterations; num++) {
             vector<unsigned char> hash_input = intToBytes(num, 4);
             hash_input.insert(hash_input.end(), id_bytes.begin(), id_bytes.end());
 
             vector<unsigned char> hash(picosha2::k_digest_size);
             picosha2::hash256(hash_input.begin(), hash_input.end(), hash.begin(), hash.end());
 
-            try {
-                vector<LargeBits> qualities = prover.GetQualitiesForChallenge(hash.data());
+            vector<LargeBits> qualities = prover.GetQualitiesForChallenge(hash.data());
 
-                for (uint32_t i = 0; i < qualities.size(); i++) {
+            for (uint32_t i = 0; i < qualities.size(); i++) {
+                try {
                     LargeBits proof = prover.GetFullProof(hash.data(), i, parallel_read);
                     uint8_t *proof_data = new uint8_t[proof.GetSize() / 8];
                     proof.ToBytes(proof_data);
                     cout << "i: " << num << std::endl;
                     cout << "challenge: 0x" << Util::HexStr(hash.data(), 256 / 8) << endl;
                     cout << "proof: 0x" << Util::HexStr(proof_data, k * 8) << endl;
                     LargeBits quality =
                         verifier.ValidateProof(id_bytes.data(), k, hash.data(), proof_data, k * 8);
                     if (quality.GetSize() == 256 && quality == qualities[i]) {
                         cout << "quality: " << quality << endl;
                         cout << "Proof verification succeeded. k = " << static_cast<int>(k) << endl;
                         success++;
                     } else {
                         cout << "Proof verification failed." << endl;
+                        failures += 1;
                     }
                     delete[] proof_data;
+                } catch (const std::exception& error) {
+                    cout << "Threw: " << error.what() << endl;
+                    exceptions += 1;
                 }
-            } catch (const std::exception& error) {
-                cout << "Threw: " << error.what() << endl;
-                continue;
             }
         }
         std::cout << "Total success: " << success << "/" << iterations << ", "
                   << (success * 100 / static_cast<double>(iterations)) << "%." << std::endl;
+        std::cout << "Total failures: " << failures << std::endl;
+        std::cout << "Exceptions: " << exceptions << std::endl;
         if (show_progress) { progress(4, 1, 1); }
     } else {
-        cout << "Invalid operation. Use create/prove/verify/check" << endl;
+        cout << "Invalid operation '" << operation << "'. Use create/prove/verify/check" << endl;
     }
     return 0;
 } catch (const cxxopts::OptionException &e) {
     cout << "error parsing options: " << e.what() << endl;
     return 1;
 } catch (const std::exception &e) {
     std::cerr << "Caught exception: " << e.what() << endl;
```

### Comparing `chiapos-1.0.9/src/disk.hpp` & `chiapos-2.0.0b1/src/disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/encoding.hpp` & `chiapos-2.0.0b1/src/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/entry_sizes.hpp` & `chiapos-2.0.0b1/src/entry_sizes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/exceptions.hpp` & `chiapos-2.0.0b1/src/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/phase1.hpp` & `chiapos-2.0.0b1/src/phase1.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/phase2.hpp` & `chiapos-2.0.0b1/src/phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/phase3.hpp` & `chiapos-2.0.0b1/src/phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/phase4.hpp` & `chiapos-2.0.0b1/src/phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/phases.hpp` & `chiapos-2.0.0b1/src/phases.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/plotter_disk.hpp` & `chiapos-2.0.0b1/src/plotter_disk.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -196,17 +196,14 @@
         }
         for (fs::path& p : tmp_1_filenames) {
             fs::remove(p);
         }
         fs::remove(tmp_2_filename);
         fs::remove(final_filename);
 
-        std::ios_base::sync_with_stdio(false);
-        std::ostream* prevstr = std::cin.tie(NULL);
-
         {
             // Scope for FileDisk
             std::vector<FileDisk> tmp_1_disks;
             for (auto const& fname : tmp_1_filenames)
                 tmp_1_disks.emplace_back(fname);
 
             FileDisk tmp2_disk(tmp_2_filename);
@@ -355,17 +352,14 @@
             std::cout << "Final File size: "
                       << static_cast<double>(finalsize) /
                              (1024 * 1024 * 1024)
                       << " GiB" << std::endl;
             all_phases.PrintElapsed("Total time =");
         }
 
-        std::cin.tie(prevstr);
-        std::ios_base::sync_with_stdio(true);
-
         for (fs::path p : tmp_1_filenames) {
             fs::remove(p);
         }
 
         bool bCopied = false;
         bool bRenamed = false;
         Timer copy;
```

### Comparing `chiapos-1.0.9/src/pos_constants.hpp` & `chiapos-2.0.0b1/src/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/quicksort.hpp` & `chiapos-2.0.0b1/src/quicksort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/sort_manager.hpp` & `chiapos-2.0.0b1/src/sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/threading.hpp` & `chiapos-2.0.0b1/src/threading.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/uniformsort.hpp` & `chiapos-2.0.0b1/src/uniformsort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/util.hpp` & `chiapos-2.0.0b1/src/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/src/verifier.hpp` & `chiapos-2.0.0b1/src/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/tests/plot-resources.py` & `chiapos-2.0.0b1/tests/plot-resources.py`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/tests/test.cpp` & `chiapos-2.0.0b1/tests/test.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include <stdio.h>
 
 #include <set>
 
-#include <catch2/catch.hpp>
+#include <catch2/catch_test_macros.hpp>
+#include <catch2/catch_session.hpp>
+#include <catch2/matchers/catch_matchers.hpp>
 
 #include "../lib/include/picosha2.hpp"
 #include "calculate_bucket.hpp"
 #include "disk.hpp"
 #include "plotter_disk.hpp"
 #include "prover_disk.hpp"
+#include "serialize.hpp"
 #include "sort_manager.hpp"
 #include "verifier.hpp"
 
 using namespace std;
 
 uint8_t plot_id_1[] = {35,  2,   52,  4,  51, 55,  23,  84, 91, 10, 111, 12,  13,  222, 151, 16,
                        228, 211, 254, 45, 92, 198, 204, 10, 9,  10, 11,  129, 139, 171, 15,  23};
@@ -140,15 +143,14 @@
     CHECK(Util::SliceInt64FromBytesFull(bytes, 3, 64) == 0x0102030405060708ull << 3);
     CHECK(Util::SliceInt64FromBytesFull(bytes, 4, 64) == 0x1020304050607080ull);
     CHECK(Util::SliceInt64FromBytesFull(bytes, 5, 64) == ((0x1020304050607080ull << 1) | 0b1));
     CHECK(Util::SliceInt64FromBytesFull(bytes, 6, 64) == ((0x1020304050607080ull << 2) | 0b10));
     CHECK(Util::SliceInt64FromBytesFull(bytes, 7, 64) == ((0x1020304050607080ull << 3) | 0b100));
     CHECK(Util::SliceInt64FromBytesFull(bytes, 8, 64) == 0x0203040506070809ull);
 }
-
 TEST_CASE("Util")
 {
     SECTION("Increment and decrement")
     {
         uint8_t bytes[3 + 7] = {45, 172, 225};
         REQUIRE(Util::SliceInt64FromBytes(bytes, 2, 19) == 374172);
         uint8_t bytes2[1 + 7] = {213};
@@ -476,14 +478,123 @@
         VerifyFC(6, 16, 0xc965815a47c5, 0xf5e008d6af57, 0x1f121a, 0x1cabbe, 0xc8cc6947);
         VerifyFC(6, 16, 0xd420677f6cbd, 0x5894aa2ca1af, 0x2efde9, 0xc2121, 0x421bb8ec);
         VerifyFC(7, 16, 0x5fec898f, 0x82283d15, 0x14f410, 0x24c3c2, 0x0);
         VerifyFC(7, 16, 0x64ac5db9, 0x7923986, 0x590fd, 0x1c74a2, 0x0);
     }
 }
 
+TEST_CASE("(De)Serialization")
+{
+    Serializer serializer;
+    Deserializer deserializer(serializer.Data());
+    SECTION("Basics")
+    {
+        serializer.Reset();
+        for (uint8_t i = 0; i < 0xFF; ++i) {
+            serializer << i;
+        }
+        uint8_t n{0}, n_deserialized;
+        do{
+            deserializer >> n_deserialized;
+            REQUIRE(n_deserialized == n++);
+        } while (!deserializer.End());
+        serializer.Reset();
+        deserializer.Reset();
+        std::vector<float> vecFloat;
+        REQUIRE_THROWS(deserializer >> vecFloat); // Unexpected vector, leads to read out of bounds
+        float f = 0.123, f_deserialized = 0;
+        double d = 1.23, d_deserialized = 0;
+        int64_t i = -123, i_deserialized = 0;
+        uint64_t u = 123, u_deserialized = 0;
+        serializer << f;
+        deserializer >> f_deserialized;
+        REQUIRE(f_deserialized == f);
+        serializer << d;
+        deserializer >> d_deserialized;
+        REQUIRE(d_deserialized == d);
+        serializer << i;
+        deserializer >> i_deserialized;
+        REQUIRE(i_deserialized == i);
+        serializer << u;
+        deserializer >> u_deserialized;
+        REQUIRE(u_deserialized == u);
+        REQUIRE(deserializer.End());
+        deserializer.Reset();
+        deserializer >> f_deserialized;
+        deserializer >> d_deserialized;
+        deserializer >> i_deserialized;
+        deserializer >> u_deserialized;
+        REQUIRE(f_deserialized == f);
+        REQUIRE(d_deserialized == d);
+        REQUIRE(i_deserialized == i);
+        REQUIRE(u_deserialized == u);
+        REQUIRE(deserializer.End());
+        REQUIRE_THROWS(deserializer >> f_deserialized); // Read out of bounds
+    }
+    SECTION("vector")
+    {
+        std::vector<uint64_t> vec1{1,2,3}, vec2;
+        std::vector<std::vector<uint64_t>> vec3{{1}, {2,3}, {4,5,6}}, vec4;
+        serializer << vec1;
+        serializer << vec2;
+        serializer << vec3;
+        serializer << vec4;
+        std::vector<uint64_t> vec1_deserialized, vec2_deserialized;
+        std::vector<std::vector<uint64_t>> vec3_deserialized, vec4_deserialized;
+        deserializer >> vec1_deserialized;
+        deserializer >> vec2_deserialized;
+        deserializer >> vec3_deserialized;
+        deserializer >> vec4_deserialized;
+        REQUIRE(vec1_deserialized == vec1);
+        REQUIRE(vec2_deserialized == vec2);
+        REQUIRE(vec3_deserialized == vec3);
+        REQUIRE(vec4_deserialized == vec4);
+        REQUIRE(deserializer.End());
+    }
+    SECTION("string")
+    {
+        std::string str1 = "123", str2;
+        serializer << str1;
+        serializer << str2;
+        std::string str1_deserialized, str2_deserialized;
+        deserializer >> str1_deserialized;
+        deserializer >> str2_deserialized;
+        REQUIRE(str1_deserialized == str1);
+        REQUIRE(str2_deserialized == str2);
+        REQUIRE(deserializer.End());
+    }
+    SECTION("DiskProver")
+    {
+        std::string filename = "prover_test.plot";
+        DiskPlotter plotter = DiskPlotter();
+        uint8_t memo[5] = {1, 2, 3, 4, 5};
+        plotter.CreatePlotDisk(
+            ".", ".", ".", filename, 18, memo, 5, plot_id_1, 32, 11, 0, 4000, 2);
+        DiskProver prover1(filename);
+        std::vector<uint8_t> vecBytes = prover1.ToBytes();
+        DiskProver prover2(vecBytes);
+        REQUIRE(prover1.GetFilename() == prover2.GetFilename());
+        REQUIRE(prover1.GetSize() == prover2.GetSize());
+        REQUIRE(prover1.GetId() == prover2.GetId());
+        REQUIRE(prover1.GetMemo() == prover2.GetMemo());
+        vector<unsigned char> hash_input = intToBytes(0, 4);
+        vector<unsigned char> hash(picosha2::k_digest_size);
+        picosha2::hash256(hash_input.begin(), hash_input.end(), hash.begin(), hash.end());
+        vector<LargeBits> qualities1 = prover1.GetQualitiesForChallenge(hash.data());
+        LargeBits proof1 = prover1.GetFullProof(hash.data(), 0);
+        vector<LargeBits> qualities2 = prover2.GetQualitiesForChallenge(hash.data());
+        LargeBits proof2 = prover2.GetFullProof(hash.data(), 0);
+        REQUIRE(qualities1 == qualities2);
+        REQUIRE(proof1 == proof2);
+        vecBytes[0] = 0x02; // Change version
+        REQUIRE_THROWS(DiskProver(vecBytes)); // Invalid version
+        REQUIRE(remove(filename.c_str()) == 0);
+    }
+}
+
 void HexToBytes(const string& hex, uint8_t* result)
 {
     for (unsigned int i = 0; i < hex.length(); i += 2) {
         string byteString = hex.substr(i, 2);
         uint8_t byte = (uint8_t)strtol(byteString.c_str(), NULL, 16);
         result[i / 2] = byte;
     }
@@ -963,14 +1074,46 @@
         auto const val = *reinterpret_cast<std::uint32_t const*>(bd.Read(i * 4, 4));
         CHECK(i == val);
     }
 
     remove("test_file.bin");
 }
 
+TEST_CASE("DiskProver")
+{
+    SECTION("Move constructor")
+    {
+        std::string filename = "prover_test.plot";
+        DiskPlotter plotter = DiskPlotter();
+        std::vector<uint8_t> memo{1, 2, 3};
+        plotter.CreatePlotDisk(
+            ".", ".", ".", filename, 18, memo.data(),
+            memo.size(), plot_id_1, 32, 11, 0,
+            4000, 2);
+        DiskProver prover1(filename);
+        auto* p1_filename_ptr = prover1.GetFilename().data();
+        auto* p1_memo_ptr = prover1.GetMemo().data();
+        auto* p1_id_ptr = prover1.GetId().data();
+        auto* p1_table_begin_pointers_ptr = prover1.GetTableBeginPointers().data();
+        auto* p1_C2_ptr = prover1.GetC2().data();
+        DiskProver prover2(std::move(prover1));
+        REQUIRE(prover2.GetFilename().data() == p1_filename_ptr);
+        REQUIRE(prover2.GetMemo().data() == p1_memo_ptr);
+        REQUIRE(prover2.GetId().data() == p1_id_ptr);
+        REQUIRE(prover2.GetTableBeginPointers().data() == p1_table_begin_pointers_ptr);
+        REQUIRE(prover2.GetC2().data() == p1_C2_ptr);
+        REQUIRE(prover1.GetFilename().empty());
+        REQUIRE(prover1.GetMemo().empty());
+        REQUIRE(prover1.GetId().empty());
+        REQUIRE(prover1.GetSize() == prover1.GetSize());
+        REQUIRE(prover1.GetTableBeginPointers().empty());
+        REQUIRE(prover1.GetC2().empty());
+    }
+}
+
 TEST_CASE("FilteredDisk")
 {
     FileDisk d = FileDisk("test_file.bin");
     write_disk_file(d);
 
     SECTION("filter even")
     {
@@ -1023,7 +1166,13 @@
         BufferedDisk bd(&d, num_test_entries * 4);
         bitfield filter(num_test_entries);
         FilteredDisk fd(std::move(bd), std::move(filter), 4);
     }
 */
     remove("test_file.bin");
 }
+
+int main(int argc, char* argv[])
+{
+    int result = Catch::Session().run(argc, argv);
+    return result;
+}
```

### Comparing `chiapos-1.0.9/tests/test_python_bindings.py` & `chiapos-2.0.0b1/tests/test_python_bindings.py`

 * *Files 22% similar despite different names*

```diff
@@ -172,10 +172,34 @@
                         failures += 1
             except Exception as e:
                 print(f"Exception: {e}")
                 failures += 1
         print(f"Successes: {successes}")
         print(f"Failures: {failures}")
 
+    def test_disk_prover_byte_conversions(self):
+        plot_path = Path("byte_conversion_plot.dat")
+        if plot_path.exists():
+            plot_path.unlink()
+        challenge = sha256(b"\x00").digest()
+        pl = DiskPlotter()
+        pl.create_plot_disk(
+            ".", ".", ".", str(plot_path), 21, bytes([1, 2, 3, 4, 5]), bytes(b'\0' * 32), 300, 32, 8192, 8, False
+        )
+        pr = DiskProver(str(plot_path))
+        serialized = bytes(pr)
+        pr_recovered = DiskProver.from_bytes(serialized)
+        assert bytes(pr_recovered) == serialized
+        assert pr.get_memo() == pr_recovered.get_memo()
+        assert pr.get_id() == pr_recovered.get_id()
+        assert pr.get_size() == pr_recovered.get_size()
+        assert pr.get_filename() == pr_recovered.get_filename()
+        assert pr.get_size() == pr_recovered.get_size()
+        assert pr.get_qualities_for_challenge(challenge) == pr_recovered.get_qualities_for_challenge(challenge)
+        with self.assertRaises(ValueError):
+            DiskProver.from_bytes(bytes())
+        with self.assertRaises(ValueError):
+            DiskProver.from_bytes(serialized[0:int(len(serialized)/2)])
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `chiapos-1.0.9/tools/disk.gnuplot` & `chiapos-2.0.0b1/tools/disk.gnuplot`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/tools/parse_disk.py` & `chiapos-2.0.0b1/tools/parse_disk.py`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/uint128_t/LICENSE` & `chiapos-2.0.0b1/uint128_t/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/uint128_t/README.md` & `chiapos-2.0.0b1/uint128_t/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/uint128_t/endianness.h` & `chiapos-2.0.0b1/uint128_t/endianness.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/uint128_t/uint128_t.cpp` & `chiapos-2.0.0b1/uint128_t/uint128_t.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/uint128_t/uint128_t.include` & `chiapos-2.0.0b1/uint128_t/uint128_t.include`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.9/uint128_t/uint128_t_config.include` & `chiapos-2.0.0b1/uint128_t/uint128_t_config.include`

 * *Files identical despite different names*

