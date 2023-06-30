# Comparing `tmp/estival-0.3.0.tar.gz` & `tmp/estival-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estival-0.3.0.tar", max compression
+gzip compressed data, was "estival-0.3.1.tar", max compression
```

## Comparing `estival-0.3.0.tar` & `estival-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     4837 2023-06-22 22:51:47.913836 estival-0.3.0/estival/model.py
--rw-r--r--   0        0        0     4396 2023-06-26 23:39:41.366366 estival-0.3.0/estival/priors.py
--rw-r--r--   0        0        0       69 2023-06-26 23:53:46.119711 estival-0.3.0/estival/sampling/__init__.py
--rw-r--r--   0        0        0      220 2023-06-27 02:39:58.936134 estival-0.3.0/estival/sampling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2987 2023-06-28 02:53:51.550147 estival-0.3.0/estival/sampling/__pycache__/tools.cpython-310.pyc
--rw-r--r--   0        0        0     3617 2023-06-28 02:36:09.560248 estival-0.3.0/estival/sampling/tools.py
--rw-r--r--   0        0        0    11486 2023-05-19 02:24:52.265480 estival-0.3.0/estival/targets.py
--rw-r--r--   0        0        0     1696 2023-06-28 02:36:46.808894 estival-0.3.0/estival/utils/__pycache__/parallel.cpython-310.pyc
--rw-r--r--   0        0        0     1636 2023-06-28 02:36:36.802184 estival-0.3.0/estival/utils/parallel.py
--rw-r--r--   0        0        0     3030 2023-06-28 01:48:29.525182 estival-0.3.0/estival/wrappers/__pycache__/nevergrad.cpython-310.pyc
--rw-r--r--   0        0        0     3465 2023-06-28 01:50:17.395604 estival-0.3.0/estival/wrappers/__pycache__/pymc.cpython-310.pyc
--rw-r--r--   0        0        0     2906 2023-06-28 02:05:42.685331 estival-0.3.0/estival/wrappers/nevergrad.py
--rw-r--r--   0        0        0     3091 2023-06-25 23:10:26.123729 estival-0.3.0/estival/wrappers/pymc.py
--rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.3.0/LICENSE
--rw-r--r--   0        0        0     1034 2023-06-28 01:49:42.426551 estival-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      834 2023-06-28 02:57:17.837902 estival-0.3.0/README.md
--rw-r--r--   0        0        0     1964 1970-01-01 00:00:00.000000 estival-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       79 2023-06-30 01:05:55.108051 estival-0.3.1/estival/__init__.py
+-rw-r--r--   0        0        0     4837 2023-06-30 01:03:28.991433 estival-0.3.1/estival/model.py
+-rw-r--r--   0        0        0     4396 2023-06-30 01:03:28.992428 estival-0.3.1/estival/priors.py
+-rw-r--r--   0        0        0       69 2023-06-26 23:53:46.119711 estival-0.3.1/estival/sampling/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-27 02:39:58.936134 estival-0.3.1/estival/sampling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2987 2023-06-30 01:06:23.734552 estival-0.3.1/estival/sampling/__pycache__/tools.cpython-310.pyc
+-rw-r--r--   0        0        0     3617 2023-06-30 01:03:28.992928 estival-0.3.1/estival/sampling/tools.py
+-rw-r--r--   0        0        0    11486 2023-05-19 02:24:52.265480 estival-0.3.1/estival/targets.py
+-rw-r--r--   0        0        0       24 2023-06-30 01:01:37.182961 estival-0.3.1/estival/utils/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-30 01:06:23.736049 estival-0.3.1/estival/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1696 2023-06-30 01:06:23.739049 estival-0.3.1/estival/utils/__pycache__/parallel.cpython-310.pyc
+-rw-r--r--   0        0        0     1636 2023-06-30 01:03:28.993428 estival-0.3.1/estival/utils/parallel.py
+-rw-r--r--   0        0        0       31 2023-06-30 01:01:24.074862 estival-0.3.1/estival/wrappers/__init__.py
+-rw-r--r--   0        0        0      189 2023-06-30 01:06:23.741049 estival-0.3.1/estival/wrappers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3048 2023-06-30 01:06:23.747549 estival-0.3.1/estival/wrappers/__pycache__/nevergrad.cpython-310.pyc
+-rw-r--r--   0        0        0     3465 2023-06-30 01:06:23.744049 estival-0.3.1/estival/wrappers/__pycache__/pymc.cpython-310.pyc
+-rw-r--r--   0        0        0     2906 2023-06-30 01:03:28.994438 estival-0.3.1/estival/wrappers/nevergrad.py
+-rw-r--r--   0        0        0     3091 2023-06-30 01:03:28.994927 estival-0.3.1/estival/wrappers/pymc.py
+-rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1034 2023-06-30 01:07:19.748623 estival-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      883 2023-06-30 01:07:12.285115 estival-0.3.1/README.md
+-rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 estival-0.3.1/PKG-INFO
```

### Comparing `estival-0.3.0/estival/model.py` & `estival-0.3.1/estival/model.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.0/estival/priors.py` & `estival-0.3.1/estival/priors.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.0/estival/sampling/__pycache__/tools.cpython-310.pyc` & `estival-0.3.1/estival/sampling/__pycache__/tools.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun 28 02:36:09 2023 UTC, .py size: 3617 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 999c 9b64 210e 0000  o..........d!...
+00000000: 6f0d 0d0a 0000 0000 e029 9e64 210e 0000  o........).d!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c06 5a06 6400 6403 6c07 5a08 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -170,15 +170,15 @@
 00000a90: 0208 011a 0114 0110 011a 0102 fe0a 0412  ................
 00000aa0: 0514 0208 0204 0308 0116 0104 0272 3700  .............r7.
 00000ab0: 0000 2901 4e29 16da 0674 7970 696e 6772  ..).N)...typingr
 00000ac0: 0200 0000 7203 0000 00da 0f6d 756c 7469  ....r......multi
 00000ad0: 7072 6f63 6573 7369 6e67 7204 0000 0072  processingr....r
 00000ae0: 0500 0000 da0b 636c 6f75 6470 6963 6b6c  ......cloudpickl
 00000af0: 65da 0670 616e 6461 7372 3000 0000 da05  e..pandasr0.....
-00000b00: 6172 7669 7a72 0600 0000 da0d 6573 7469  arvizr......esti
+00000b00: 6172 7669 7a72 0600 0000 5a0d 6573 7469  arvizr....Z.esti
 00000b10: 7661 6c2e 6d6f 6465 6c72 0700 0000 5a16  val.modelr....Z.
 00000b20: 6573 7469 7661 6c2e 7574 696c 732e 7061  estival.utils.pa
 00000b30: 7261 6c6c 656c 7208 0000 0072 2400 0000  rallelr....r$...
 00000b40: 722a 0000 00da 0373 7472 722d 0000 0072  r*.....strr-...r
 00000b50: 2b00 0000 7231 0000 0072 3700 0000 720f  +...r1...r7...r.
 00000b60: 0000 0072 0f00 0000 720f 0000 0072 1300  ...r....r....r..
 00000b70: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
```

### Comparing `estival-0.3.0/estival/sampling/tools.py` & `estival-0.3.1/estival/sampling/tools.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.0/estival/targets.py` & `estival-0.3.1/estival/targets.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.0/estival/utils/__pycache__/parallel.cpython-310.pyc` & `estival-0.3.1/estival/utils/__pycache__/parallel.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun 28 02:36:36 2023 UTC, .py size: 1636 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b49c 9b64 6406 0000  o..........dd...
+00000000: 6f0d 0d0a 0000 0000 e029 9e64 6406 0000  o........).dd...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c06 5a06 6404 6405 8400 5a07 6406  d.l.Z.d.d...Z.d.
 00000060: 6407 8400 5a08 640d 6408 6501 6409 6502  d...Z.d.d.e.d.e.
 00000070: 640a 6509 6606 640b 640c 8405 5a0a 6403  d.e.f.d.d...Z.d.
@@ -87,20 +87,20 @@
 00000560: 756e 630a 2020 2020 4ee9 0200 0000 2902  unc.    N.....).
 00000570: da0b 696e 6974 6961 6c69 7a65 72da 0869  ..initializer..i
 00000580: 6e69 7461 7267 7329 0ada 0369 6e74 7205  nitargs)...intr.
 00000590: 0000 0072 0400 0000 720b 0000 0072 0600  ...r....r....r..
 000005a0: 0000 da05 6475 6d70 73da 036d 6170 720e  ....dumps..mapr.
 000005b0: 0000 00da 0563 6c6f 7365 da04 6a6f 696e  .....close..join
 000005c0: 2905 720d 0000 0072 0f00 0000 7210 0000  ).r....r....r...
-000005d0: 00da 0470 6f6f 6c5a 0470 7265 7372 0900  ...poolZ.presr..
+000005d0: 00da 0470 6f6f 6cda 0470 7265 7372 0900  ...pool..presr..
 000005e0: 0000 7209 0000 0072 0a00 0000 da0c 6d61  ..r....r......ma
 000005f0: 705f 7061 7261 6c6c 656c 2300 0000 731a  p_parallel#...s.
 00000600: 0000 0008 0c0e 0102 020e 0106 ff02 020c  ................
-00000610: 0108 010a 010a fb04 0610 fa04 0672 1a00  .............r..
+00000610: 0108 010a 010a fb04 0610 fa04 0672 1b00  .............r..
 00000620: 0000 2901 4e29 0bda 0674 7970 696e 6772  ..).N)...typingr
 00000630: 0200 0000 7203 0000 00da 0f6d 756c 7469  ....r......multi
 00000640: 7072 6f63 6573 7369 6e67 7204 0000 0072  processingr....r
 00000650: 0500 0000 7206 0000 0072 0b00 0000 720e  ....r....r....r.
-00000660: 0000 0072 1400 0000 721a 0000 0072 0900  ...r....r....r..
+00000660: 0000 0072 1400 0000 721b 0000 0072 0900  ...r....r....r..
 00000670: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
 00000680: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
 00000690: 0c00 0000 1000 1002 0802 0804 080c 1c0e  ................
```

### Comparing `estival-0.3.0/estival/utils/parallel.py` & `estival-0.3.1/estival/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.0/estival/wrappers/__pycache__/nevergrad.cpython-310.pyc` & `estival-0.3.1/estival/wrappers/__pycache__/nevergrad.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun 28 01:46:54 2023 UTC, .py size: 2897 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0e91 9b64 510b 0000  o..........dQ...
+00000000: 6f0d 0d0a 0000 0000 e029 9e64 5a0b 0000  o........).dZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 5a07 6400 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 7a06 6400 6404 6c0a 5a0b  m.Z...z.d.d.l.Z.
 00000070: 5700 6e04 0100 0100 0100 5900 6417 6407  W.n.......Y.d.d.
@@ -101,90 +101,91 @@
 00000640: 0d00 0000 720d 0000 0072 0d00 0000 721f  ....r....r....r.
 00000650: 0000 0072 2100 0000 2e00 0000 7306 0000  ...r!.......s...
 00000660: 0008 0008 010c 0572 2100 0000 69e8 0300  .......r!...i...
 00000670: 0054 da03 6263 6d72 2900 0000 7224 0000  .T..bcmr)...r$..
 00000680: 0072 1b00 0000 721c 0000 00da 0c6f 626a  .r....r......obj
 00000690: 5f66 756e 6374 696f 6e63 0800 0000 0000  _functionc......
 000006a0: 0000 0000 0000 0c00 0000 0500 0000 4300  ..............C.
-000006b0: 0000 7362 0000 007c 0373 0574 0083 007d  ..sb...|.s.t...}
-000006c0: 0374 017c 006a 027c 047c 0583 037d 0864  .t.|.j.|.|...}.d
-000006d0: 0164 0284 007d 097c 0664 0075 0072 177c  .d...}.|.d.u.r.|
-000006e0: 006a 037d 067c 0772 1e74 047c 0683 017d  .j.}.|.r.t.|...}
-000006f0: 066e 047c 097c 0683 017d 067c 067d 0a7c  .n.|.|...}.|.}.|
-00000700: 027c 087c 017c 0364 038d 037d 0b74 057c  .|.|.|.d...}.t.|
-00000710: 0b7c 0a7c 0383 0353 0029 044e 6301 0000  .|.|...S.).Nc...
-00000720: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000730: 0013 0000 0073 1000 0000 8700 6601 6401  .....s......f.d.
-00000740: 6402 8408 7d01 7c01 5300 2903 4e63 0000  d...}.|.S.).Nc..
-00000750: 0000 0000 0000 0000 0000 0100 0000 0500  ................
-00000760: 0000 1b00 0000 7312 0000 0074 0088 0064  ......s....t...d
-00000770: 0169 007c 00a4 018e 0183 0153 0029 024e  .i.|.......S.).N
-00000780: 720d 0000 00a9 01da 0566 6c6f 6174 2901  r........float).
-00000790: da0a 7061 7261 6d65 7465 7273 a901 da07  ..parameters....
-000007a0: 7772 6170 7065 6472 0d00 0000 721f 0000  wrappedr....r...
-000007b0: 00da 0d66 6c6f 6174 5f77 7261 7070 6572  ...float_wrapper
-000007c0: 4c00 0000 7302 0000 0012 017a 376f 7074  L...s......z7opt
-000007d0: 696d 697a 655f 6d6f 6465 6c2e 3c6c 6f63  imize_model.<loc
-000007e0: 616c 733e 2e61 735f 666c 6f61 742e 3c6c  als>.as_float.<l
-000007f0: 6f63 616c 733e 2e66 6c6f 6174 5f77 7261  ocals>.float_wra
-00000800: 7070 6572 720d 0000 0029 0272 3600 0000  pperr....).r6...
-00000810: 7237 0000 0072 0d00 0000 7235 0000 0072  r7...r....r5...r
-00000820: 1f00 0000 da08 6173 5f66 6c6f 6174 4b00  ......as_floatK.
-00000830: 0000 7304 0000 000c 0104 037a 206f 7074  ..s........z opt
-00000840: 696d 697a 655f 6d6f 6465 6c2e 3c6c 6f63  imize_model.<loc
-00000850: 616c 733e 2e61 735f 666c 6f61 7429 035a  als>.as_float).Z
-00000860: 0f70 6172 616d 6574 7269 7a61 7469 6f6e  .parametrization
-00000870: 7229 0000 0072 2400 0000 2906 7204 0000  r)...r$...).r...
-00000880: 0072 2000 0000 721a 0000 00da 0d6c 6f67  .r ...r......log
-00000890: 6c69 6b65 6c69 686f 6f64 da08 6e65 6761  likelihood..nega
-000008a0: 7469 7665 7221 0000 0029 0c72 3000 0000  tiver!...).r0...
-000008b0: 7229 0000 005a 096f 7074 5f63 6c61 7373  r)...Z.opt_class
-000008c0: 7224 0000 0072 1b00 0000 721c 0000 0072  r$...r....r....r
-000008d0: 3100 0000 5a0f 696e 7665 7274 5f66 756e  1...Z.invert_fun
-000008e0: 6374 696f 6e5a 0769 6e73 7472 756d 7238  ctionZ.instrumr8
-000008f0: 0000 0072 2300 0000 7222 0000 0072 0d00  ...r#...r"...r..
-00000900: 0000 720d 0000 0072 1f00 0000 da0e 6f70  ..r....r......op
-00000910: 7469 6d69 7a65 5f6d 6f64 656c 3c00 0000  timize_model<...
-00000920: 7318 0000 0004 0a06 010e 0208 0208 0606  s...............
-00000930: 0104 010a 0108 0204 020e 010c 0172 3b00  .............r;.
-00000940: 0000 6301 0000 0000 0000 0000 0000 0004  ..c.............
-00000950: 0000 0003 0000 000f 0000 0073 1000 0000  ...........s....
-00000960: 8700 6601 6401 6402 8408 7d03 7c03 5300  ..f.d.d...}.|.S.
-00000970: 2903 7a7c 5772 6170 2061 2070 6f73 6974  ).z|Wrap a posit
-00000980: 6976 6520 6675 6e63 7469 6f6e 2073 7563  ive function suc
-00000990: 6820 7468 6174 2061 206d 696e 696d 697a  h that a minimiz
-000009a0: 6162 6c65 2076 6572 7369 6f6e 2069 7320  able version is 
-000009b0: 7265 7475 726e 6564 2069 6e73 7465 6164  returned instead
-000009c0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-000009d0: 2020 2020 663a 2054 6865 2063 616c 6c61      f: The calla
-000009e0: 626c 6520 746f 2077 7261 700a 2020 2020  ble to wrap.    
-000009f0: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
-00000a00: 0006 0000 001f 0000 0073 1600 0000 7400  .........s....t.
-00000a10: 6401 8800 7c00 6900 7c01 a401 8e01 1800  d...|.i.|.......
-00000a20: 8301 5300 2902 4e67 0000 0000 0000 0000  ..S.).Ng........
-00000a30: 7232 0000 0029 02da 0461 7267 73da 066b  r2...)...args..k
-00000a40: 7761 7267 73a9 01da 0166 720d 0000 0072  wargs....fr....r
-00000a50: 1f00 0000 da0a 5f72 6566 6c65 6374 6564  ......_reflected
-00000a60: 6400 0000 7302 0000 0016 017a 1c6e 6567  d...s......z.neg
-00000a70: 6174 6976 652e 3c6c 6f63 616c 733e 2e5f  ative.<locals>._
-00000a80: 7265 666c 6563 7465 6472 0d00 0000 2904  reflectedr....).
-00000a90: 723f 0000 0072 3c00 0000 723d 0000 0072  r?...r<...r=...r
-00000aa0: 4000 0000 720d 0000 0072 3e00 0000 721f  @...r....r>...r.
-00000ab0: 0000 0072 3a00 0000 5d00 0000 7304 0000  ...r:...]...s...
-00000ac0: 000c 0704 0372 3a00 0000 2902 4e72 0600  .....r:...).Nr..
-00000ad0: 0000 2915 da06 7479 7069 6e67 7202 0000  ..)...typingr...
-00000ae0: 00da 0a63 6f6e 6375 7272 656e 7472 0300  ...concurrentr..
-00000af0: 0000 da0f 6d75 6c74 6970 726f 6365 7373  ....multiprocess
-00000b00: 696e 6772 0400 0000 da05 6e75 6d70 7972  ingr......numpyr
-00000b10: 1000 0000 da0d 6573 7469 7661 6c2e 6d6f  ......estival.mo
-00000b20: 6465 6c72 0500 0000 5a09 6e65 7665 7267  delr....Z.neverg
-00000b30: 7261 6472 1600 0000 7220 0000 0072 2100  radr....r ...r!.
-00000b40: 0000 5a0a 6f70 7469 6d69 7a65 7273 5a05  ..Z.optimizersZ.
-00000b50: 4e47 4f70 74da 0369 6e74 da04 6469 6374  NGOpt..int..dict
-00000b60: da03 7374 7272 3b00 0000 723a 0000 0072  ..strr;...r:...r
-00000b70: 0d00 0000 720d 0000 0072 0d00 0000 721f  ....r....r....r.
-00000b80: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000b90: 0073 4000 0000 0c00 0c02 0c01 0802 0c02  .s@.............
-00000ba0: 0203 0c01 0601 0201 0a03 0e1d 0210 0601  ................
-00000bb0: 0201 0201 0201 0201 0201 04f8 0201 02ff  ................
-00000bc0: 0202 02fe 0204 02fc 0205 02fb 0206 02fa  ................
-00000bd0: 0207 0af9 0c21                           .....!
+000006b0: 0000 736a 0000 007c 0373 0974 0074 0183  ..sj...|.s.t.t..
+000006c0: 0064 011b 0083 017d 0374 027c 006a 037c  .d.....}.t.|.j.|
+000006d0: 047c 0583 037d 0864 0264 0384 007d 097c  .|...}.d.d...}.|
+000006e0: 0664 0075 0072 1b7c 006a 047d 067c 0772  .d.u.r.|.j.}.|.r
+000006f0: 2274 057c 0683 017d 066e 047c 097c 0683  "t.|...}.n.|.|..
+00000700: 017d 067c 067d 0a7c 027c 087c 017c 0364  .}.|.}.|.|.|.|.d
+00000710: 048d 037d 0b74 067c 0b7c 0a7c 0383 0353  ...}.t.|.|.|...S
+00000720: 0029 054e e902 0000 0063 0100 0000 0000  .).N.....c......
+00000730: 0000 0000 0000 0200 0000 0300 0000 1300  ................
+00000740: 0000 7310 0000 0087 0066 0164 0164 0284  ..s......f.d.d..
+00000750: 087d 017c 0153 0029 034e 6300 0000 0000  .}.|.S.).Nc.....
+00000760: 0000 0000 0000 0001 0000 0005 0000 001b  ................
+00000770: 0000 0073 1200 0000 7400 8800 6401 6900  ...s....t...d.i.
+00000780: 7c00 a401 8e01 8301 5300 2902 4e72 0d00  |.......S.).Nr..
+00000790: 0000 a901 da05 666c 6f61 7429 01da 0a70  ......float)...p
+000007a0: 6172 616d 6574 6572 73a9 01da 0777 7261  arameters....wra
+000007b0: 7070 6564 720d 0000 0072 1f00 0000 da0d  ppedr....r......
+000007c0: 666c 6f61 745f 7772 6170 7065 724c 0000  float_wrapperL..
+000007d0: 0073 0200 0000 1201 7a37 6f70 7469 6d69  .s......z7optimi
+000007e0: 7a65 5f6d 6f64 656c 2e3c 6c6f 6361 6c73  ze_model.<locals
+000007f0: 3e2e 6173 5f66 6c6f 6174 2e3c 6c6f 6361  >.as_float.<loca
+00000800: 6c73 3e2e 666c 6f61 745f 7772 6170 7065  ls>.float_wrappe
+00000810: 7272 0d00 0000 2902 7237 0000 0072 3800  rr....).r7...r8.
+00000820: 0000 720d 0000 0072 3600 0000 721f 0000  ..r....r6...r...
+00000830: 00da 0861 735f 666c 6f61 744b 0000 0073  ...as_floatK...s
+00000840: 0400 0000 0c01 0403 7a20 6f70 7469 6d69  ........z optimi
+00000850: 7a65 5f6d 6f64 656c 2e3c 6c6f 6361 6c73  ze_model.<locals
+00000860: 3e2e 6173 5f66 6c6f 6174 2903 5a0f 7061  >.as_float).Z.pa
+00000870: 7261 6d65 7472 697a 6174 696f 6e72 2900  rametrizationr).
+00000880: 0000 7224 0000 0029 07da 0369 6e74 7204  ..r$...)...intr.
+00000890: 0000 0072 2000 0000 721a 0000 00da 0d6c  ...r ...r......l
+000008a0: 6f67 6c69 6b65 6c69 686f 6f64 da08 6e65  oglikelihood..ne
+000008b0: 6761 7469 7665 7221 0000 0029 0c72 3000  gativer!...).r0.
+000008c0: 0000 7229 0000 005a 096f 7074 5f63 6c61  ..r)...Z.opt_cla
+000008d0: 7373 7224 0000 0072 1b00 0000 721c 0000  ssr$...r....r...
+000008e0: 0072 3100 0000 5a0f 696e 7665 7274 5f66  .r1...Z.invert_f
+000008f0: 756e 6374 696f 6e5a 0769 6e73 7472 756d  unctionZ.instrum
+00000900: 7239 0000 0072 2300 0000 7222 0000 0072  r9...r#...r"...r
+00000910: 0d00 0000 720d 0000 0072 1f00 0000 da0e  ....r....r......
+00000920: 6f70 7469 6d69 7a65 5f6d 6f64 656c 3c00  optimize_model<.
+00000930: 0000 7318 0000 0004 0a0e 010e 0208 0208  ..s.............
+00000940: 0606 0104 010a 0108 0204 020e 010c 0172  ...............r
+00000950: 3d00 0000 6301 0000 0000 0000 0000 0000  =...c...........
+00000960: 0004 0000 0003 0000 000f 0000 0073 1000  .............s..
+00000970: 0000 8700 6601 6401 6402 8408 7d03 7c03  ....f.d.d...}.|.
+00000980: 5300 2903 7a7c 5772 6170 2061 2070 6f73  S.).z|Wrap a pos
+00000990: 6974 6976 6520 6675 6e63 7469 6f6e 2073  itive function s
+000009a0: 7563 6820 7468 6174 2061 206d 696e 696d  uch that a minim
+000009b0: 697a 6162 6c65 2076 6572 7369 6f6e 2069  izable version i
+000009c0: 7320 7265 7475 726e 6564 2069 6e73 7465  s returned inste
+000009d0: 6164 0a0a 2020 2020 4172 6773 3a0a 2020  ad..    Args:.  
+000009e0: 2020 2020 2020 663a 2054 6865 2063 616c        f: The cal
+000009f0: 6c61 626c 6520 746f 2077 7261 700a 2020  lable to wrap.  
+00000a00: 2020 6300 0000 0000 0000 0000 0000 0002    c.............
+00000a10: 0000 0006 0000 001f 0000 0073 1600 0000  ...........s....
+00000a20: 7400 6401 8800 7c00 6900 7c01 a401 8e01  t.d...|.i.|.....
+00000a30: 1800 8301 5300 2902 4e67 0000 0000 0000  ....S.).Ng......
+00000a40: 0000 7233 0000 0029 02da 0461 7267 73da  ..r3...)...args.
+00000a50: 066b 7761 7267 73a9 01da 0166 720d 0000  .kwargs....fr...
+00000a60: 0072 1f00 0000 da0a 5f72 6566 6c65 6374  .r......_reflect
+00000a70: 6564 6400 0000 7302 0000 0016 017a 1c6e  edd...s......z.n
+00000a80: 6567 6174 6976 652e 3c6c 6f63 616c 733e  egative.<locals>
+00000a90: 2e5f 7265 666c 6563 7465 6472 0d00 0000  ._reflectedr....
+00000aa0: 2904 7241 0000 0072 3e00 0000 723f 0000  ).rA...r>...r?..
+00000ab0: 0072 4200 0000 720d 0000 0072 4000 0000  .rB...r....r@...
+00000ac0: 721f 0000 0072 3c00 0000 5d00 0000 7304  r....r<...]...s.
+00000ad0: 0000 000c 0704 0372 3c00 0000 2902 4e72  .......r<...).Nr
+00000ae0: 0600 0000 2915 da06 7479 7069 6e67 7202  ....)...typingr.
+00000af0: 0000 00da 0a63 6f6e 6375 7272 656e 7472  .....concurrentr
+00000b00: 0300 0000 da0f 6d75 6c74 6970 726f 6365  ......multiproce
+00000b10: 7373 696e 6772 0400 0000 da05 6e75 6d70  ssingr......nump
+00000b20: 7972 1000 0000 5a0d 6573 7469 7661 6c2e  yr....Z.estival.
+00000b30: 6d6f 6465 6c72 0500 0000 da09 6e65 7665  modelr......neve
+00000b40: 7267 7261 6472 1600 0000 7220 0000 0072  rgradr....r ...r
+00000b50: 2100 0000 5a0a 6f70 7469 6d69 7a65 7273  !...Z.optimizers
+00000b60: 5a05 4e47 4f70 7472 3a00 0000 da04 6469  Z.NGOptr:.....di
+00000b70: 6374 da03 7374 7272 3d00 0000 723c 0000  ct..strr=...r<..
+00000b80: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000b90: 721f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000ba0: 0000 0073 4000 0000 0c00 0c02 0c01 0802  ...s@...........
+00000bb0: 0c02 0203 0c01 0601 0201 0a03 0e1d 0210  ................
+00000bc0: 0601 0201 0201 0201 0201 0201 04f8 0201  ................
+00000bd0: 02ff 0202 02fe 0204 02fc 0205 02fb 0206  ................
+00000be0: 02fa 0207 0af9 0c21                      .......!
```

### Comparing `estival-0.3.0/estival/wrappers/__pycache__/pymc.cpython-310.pyc` & `estival-0.3.1/estival/wrappers/__pycache__/pymc.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 25 23:10:26 2023 UTC, .py size: 3091 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 62c9 9864 130c 0000  o.......b..d....
+00000000: 6f0d 0d0a 0000 0000 e029 9e64 130c 0000  o........).d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 6d05 5a06 0100 6400 6402 6c07  d.l.m.Z...d.d.l.
 00000050: 6d08 5a08 0100 6400 6401 6c09 5a09 6403  m.Z...d.d.l.Z.d.
 00000060: 6508 6602 6404 6405 8404 5a0a 640c 6403  e.f.d.d...Z.d.d.
 00000070: 6508 6407 650b 6604 6408 6409 8405 5a0c  e.d.e.f.d.d...Z.
@@ -204,14 +204,14 @@
 00000cb0: 5f65 7374 7207 0000 0072 0700 0000 7208  _estr....r....r.
 00000cc0: 0000 00da 0772 756e 5f6d 6170 6700 0000  .....run_mapg...
 00000cd0: 7310 0000 000a 010a 010c 0112 010a fe04  s...............
 00000ce0: 0310 fd04 0372 4300 0000 2901 4629 0eda  .....rC...).F)..
 00000cf0: 056e 756d 7079 7213 0000 00da 0470 796d  .numpyr......pym
 00000d00: 6372 3200 0000 da0f 7079 7465 6e73 6f72  cr2.....pytensor
 00000d10: 2e74 656e 736f 72da 0674 656e 736f 7272  .tensor..tensorr
-00000d20: 2000 0000 da0d 6573 7469 7661 6c2e 6d6f   .....estival.mo
+00000d20: 2000 0000 5a0d 6573 7469 7661 6c2e 6d6f   ...Z.estival.mo
 00000d30: 6465 6c72 0200 0000 723c 0000 0072 2b00  delr....r<...r+.
 00000d40: 0000 da04 6c69 7374 7239 0000 0072 4300  ....listr9...rC.
 00000d50: 0000 7207 0000 0072 0700 0000 7207 0000  ..r....r....r...
 00000d60: 0072 0800 0000 da08 3c6d 6f64 756c 653e  .r......<module>
 00000d70: 0100 0000 7310 0000 0008 0008 010c 010c  ....s...........
 00000d80: 0208 020e 0314 3b0c 22                   ......;."
```

### Comparing `estival-0.3.0/estival/wrappers/nevergrad.py` & `estival-0.3.1/estival/wrappers/nevergrad.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.0/estival/wrappers/pymc.py` & `estival-0.3.1/estival/wrappers/pymc.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.0/LICENSE` & `estival-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `estival-0.3.0/pyproject.toml` & `estival-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "estival"
-version = "0.3.0"
+version = "0.3.1"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "https://github.com/monash-emu/estival"
 repository = "https://github.com/monash-emu/estival"
 documentation = "https://github.com/monash-emu/estival"
 keywords = [
     "calibration",
```

### Comparing `estival-0.3.0/README.md` & `estival-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,7 +21,9 @@
 Bugfix (reference index for models without date returned incorrect type)
 - 0.3.0
 Note - breaking changes!
 Remove old AuTuMN MCMC implementation
 Move nevergrad/pymc -> wrappers
 Expand likelihood output tools
 Include parallelism framework
+- 0.3.1
+Bugfix (submodules not properly exported)
```

### Comparing `estival-0.3.0/PKG-INFO` & `estival-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estival
-Version: 0.3.0
+Version: 0.3.1
 Summary: A set of calibration and probabilistic programming tools for use with summerepi2
 Home-page: https://github.com/monash-emu/estival
 License: BSD-2-Clause
 Keywords: calibration,optimization,bayesian,compartmental modelling,summerepi
 Author: David Shipman
 Author-email: dshipman@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -49,8 +49,9 @@
 Bugfix (reference index for models without date returned incorrect type)
 - 0.3.0
 Note - breaking changes!
 Remove old AuTuMN MCMC implementation
 Move nevergrad/pymc -> wrappers
 Expand likelihood output tools
 Include parallelism framework
-
+- 0.3.1
+Bugfix (submodules not properly exported)
```

