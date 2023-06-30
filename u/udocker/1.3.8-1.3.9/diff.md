# Comparing `tmp/udocker-1.3.8.tar.gz` & `tmp/udocker-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udocker-1.3.8.tar", last modified: Thu Mar 23 17:19:08 2023, max compression
+gzip compressed data, was "udocker-1.3.9.tar", last modified: Wed Jun  7 15:20:41 2023, max compression
```

## Comparing `udocker-1.3.8.tar` & `udocker-1.3.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.662225 udocker-1.3.8/
--rw-rw-r--   0 david     (1000) david     (1000)      893 2023-01-13 09:37:04.000000 udocker-1.3.8/AUTHORS.md
--rw-rw-r--   0 david     (1000) david     (1000)    13068 2023-03-23 17:15:28.000000 udocker-1.3.8/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)      418 2023-03-23 16:32:23.000000 udocker-1.3.8/CITING.md
--rw-rw-r--   0 david     (1000) david     (1000)     5489 2023-01-13 09:37:04.000000 udocker-1.3.8/CODE_OF_CONDUCT.md
--rw-rw-r--   0 david     (1000) david     (1000)     1821 2023-03-23 16:32:23.000000 udocker-1.3.8/CONTRIBUTING.md
--rw-r--r--   0 david     (1000) david     (1000)    11357 2019-06-11 07:52:40.000000 udocker-1.3.8/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       77 2021-06-24 09:56:32.000000 udocker-1.3.8/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)    31810 2023-03-23 17:19:08.662225 udocker-1.3.8/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)    17454 2023-03-23 16:32:30.000000 udocker-1.3.8/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      548 2023-03-23 16:32:23.000000 udocker-1.3.8/SECURITY.md
--rw-rw-r--   0 david     (1000) david     (1000)      207 2021-06-24 09:56:32.000000 udocker-1.3.8/SUMMARY.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.654225 udocker-1.3.8/docs/
--rw-rw-r--   0 david     (1000) david     (1000)       26 2021-06-17 16:15:57.000000 udocker-1.3.8/docs/_config.yml
--rw-rw-r--   0 david     (1000) david     (1000)      144 2023-03-23 16:32:23.000000 udocker-1.3.8/docs/index.md
--rw-rw-r--   0 david     (1000) david     (1000)    26343 2023-03-23 17:13:41.000000 udocker-1.3.8/docs/installation_manual.md
--rw-rw-r--   0 david     (1000) david     (1000)    15260 2021-06-17 13:25:20.000000 udocker-1.3.8/docs/logo-small.png
--rw-rw-r--   0 david     (1000) david     (1000)      813 2023-03-23 17:10:32.000000 udocker-1.3.8/docs/make_release.md
--rw-rw-r--   0 david     (1000) david     (1000)     3355 2023-03-23 16:32:23.000000 udocker-1.3.8/docs/reference_card.md
--rw-rw-r--   0 david     (1000) david     (1000)    16365 2023-03-23 16:32:23.000000 udocker-1.3.8/docs/udocker.1
--rw-rw-r--   0 david     (1000) david     (1000)     1684 2023-01-13 09:37:04.000000 udocker-1.3.8/docs/udocker_organ.md
--rw-rw-r--   0 david     (1000) david     (1000)    51316 2023-01-13 09:37:04.000000 udocker-1.3.8/docs/user_manual.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.654225 udocker-1.3.8/etc/
--rw-rw-r--   0 david     (1000) david     (1000)      411 2023-03-23 16:32:23.000000 udocker-1.3.8/etc/udocker.conf
--rw-rw-r--   0 david     (1000) david     (1000)      162 2023-03-23 17:19:08.662225 udocker-1.3.8/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     2863 2023-03-23 16:32:23.000000 udocker-1.3.8/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.654225 udocker-1.3.8/tests/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.658225 udocker-1.3.8/tests/unit/
--rwxrwxr-x   0 david     (1000) david     (1000)     3201 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_chksum.py
--rwxrwxr-x   0 david     (1000) david     (1000)    57341 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_cli.py
--rwxrwxr-x   0 david     (1000) david     (1000)     3544 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_cmdparser.py
--rwxrwxr-x   0 david     (1000) david     (1000)    15823 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_commonlocalfile.py
--rwxrwxr-x   0 david     (1000) david     (1000)     3609 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_config.py
--rwxrwxr-x   0 david     (1000) david     (1000)    18268 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_containerstructure.py
--rwxrwxr-x   0 david     (1000) david     (1000)    12181 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_curl.py
--rwxrwxr-x   0 david     (1000) david     (1000)     2386 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_curlheader.py
--rwxrwxr-x   0 david     (1000) david     (1000)    32765 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_dockerioapi.py
--rwxrwxr-x   0 david     (1000) david     (1000)    15470 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_dockerlocalfileapi.py
--rwxrwxr-x   0 david     (1000) david     (1000)    16813 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_elfpatcher.py
--rwxrwxr-x   0 david     (1000) david     (1000)    38618 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_execenginecommon.py
--rwxrwxr-x   0 david     (1000) david     (1000)     7522 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_executionmode.py
--rwxrwxr-x   0 david     (1000) david     (1000)    14325 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_fakechroot.py
--rwxrwxr-x   0 david     (1000) david     (1000)     8069 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_filebind.py
--rwxrwxr-x   0 david     (1000) david     (1000)    45120 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_fileutil.py
--rwxrwxr-x   0 david     (1000) david     (1000)     5172 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_geturl.py
--rwxrwxr-x   0 david     (1000) david     (1000)     4699 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_geturlexecurl.py
--rwxrwxr-x   0 david     (1000) david     (1000)     4729 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_geturlpycurl.py
--rwxrwxr-x   0 david     (1000) david     (1000)     3423 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_hostinfo.py
--rwxrwxr-x   0 david     (1000) david     (1000)     5848 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_keystore.py
--rwxrwxr-x   0 david     (1000) david     (1000)     3864 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_localfile.py
--rwxrwxr-x   0 david     (1000) david     (1000)    62554 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_localrepository.py
--rwxrwxr-x   0 david     (1000) david     (1000)    11004 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_mountpoint.py
--rwxrwxr-x   0 david     (1000) david     (1000)     2036 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_msg.py
--rwxrwxr-x   0 david     (1000) david     (1000)    10562 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_nixauthentication.py
--rwxrwxr-x   0 david     (1000) david     (1000)    10913 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_nvidia.py
--rwxrwxr-x   0 david     (1000) david     (1000)     5019 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_oci.py
--rwxrwxr-x   0 david     (1000) david     (1000)     4151 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_osinfo.py
--rwxrwxr-x   0 david     (1000) david     (1000)     8650 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_proot.py
--rwxrwxr-x   0 david     (1000) david     (1000)    29166 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_runc.py
--rwxrwxr-x   0 david     (1000) david     (1000)     9693 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_singularity.py
--rwxrwxr-x   0 david     (1000) david     (1000)    14396 2023-03-23 16:59:38.000000 udocker-1.3.8/tests/unit/test_tools.py
--rwxrwxr-x   0 david     (1000) david     (1000)     5160 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_uenv.py
--rwxrwxr-x   0 david     (1000) david     (1000)     3465 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_umain.py
--rwxrwxr-x   0 david     (1000) david     (1000)     1879 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_unique.py
--rwxrwxr-x   0 david     (1000) david     (1000)     3647 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_unshare.py
--rwxrwxr-x   0 david     (1000) david     (1000)     2660 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_uprocess.py
--rwxrwxr-x   0 david     (1000) david     (1000)     1220 2023-03-23 16:32:23.000000 udocker-1.3.8/tests/unit/test_uvolume.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.658225 udocker-1.3.8/udocker/
--rw-rw-r--   0 david     (1000) david     (1000)     1195 2023-03-23 17:11:28.000000 udocker-1.3.8/udocker/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    53650 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)     7228 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/cmdparser.py
--rw-rw-r--   0 david     (1000) david     (1000)    10252 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/commonlocalfile.py
--rw-rw-r--   0 david     (1000) david     (1000)    11794 2023-03-23 17:06:10.000000 udocker-1.3.8/udocker/config.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.658225 udocker-1.3.8/udocker/container/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-17 13:25:20.000000 udocker-1.3.8/udocker/container/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    32330 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/container/localrepo.py
--rw-rw-r--   0 david     (1000) david     (1000)    13498 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/container/structure.py
--rw-rw-r--   0 david     (1000) david     (1000)    35506 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/docker.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.662225 udocker-1.3.8/udocker/engine/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-17 13:25:20.000000 udocker-1.3.8/udocker/engine/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    28554 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/engine/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     5237 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/engine/execmode.py
--rw-rw-r--   0 david     (1000) david     (1000)    12774 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/engine/fakechroot.py
--rw-rw-r--   0 david     (1000) david     (1000)     8523 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/engine/nvidia.py
--rw-rw-r--   0 david     (1000) david     (1000)     7605 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/engine/proot.py
--rw-rw-r--   0 david     (1000) david     (1000)    17818 2023-03-23 17:04:59.000000 udocker-1.3.8/udocker/engine/runc.py
--rw-rw-r--   0 david     (1000) david     (1000)     7679 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/engine/singularity.py
--rw-rw-r--   0 david     (1000) david     (1000)      511 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/genstr.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.662225 udocker-1.3.8/udocker/helper/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-17 13:25:20.000000 udocker-1.3.8/udocker/helper/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    11501 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/helper/elfpatcher.py
--rw-rw-r--   0 david     (1000) david     (1000)     3074 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/helper/hostinfo.py
--rw-rw-r--   0 david     (1000) david     (1000)     3419 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/helper/keystore.py
--rw-rw-r--   0 david     (1000) david     (1000)     6878 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/helper/nixauth.py
--rw-rw-r--   0 david     (1000) david     (1000)     3893 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/helper/osinfo.py
--rw-rw-r--   0 david     (1000) david     (1000)     1707 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/helper/unique.py
--rw-rw-r--   0 david     (1000) david     (1000)     2457 2023-03-23 16:32:23.000000 udocker-1.3.8/udocker/helper/unshare.py
--rw-rw-r--   0 david     (1000) david     (1000)     1811 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/localfile.py
--rwxrwxr-x   0 david     (1000) david     (1000)     1698 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/maincmd.py
--rw-rw-r--   0 david     (1000) david     (1000)     2136 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/msg.py
--rw-rw-r--   0 david     (1000) david     (1000)     5168 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/oci.py
--rw-rw-r--   0 david     (1000) david     (1000)    12024 2023-03-23 17:03:30.000000 udocker-1.3.8/udocker/tools.py
--rw-rw-r--   0 david     (1000) david     (1000)     4479 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/umain.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.662225 udocker-1.3.8/udocker/utils/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-17 13:25:20.000000 udocker-1.3.8/udocker/utils/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2485 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/utils/chksum.py
--rw-rw-r--   0 david     (1000) david     (1000)    15599 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/utils/curl.py
--rw-rw-r--   0 david     (1000) david     (1000)     4436 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/utils/filebind.py
--rw-rw-r--   0 david     (1000) david     (1000)    22449 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/utils/fileutil.py
--rw-rw-r--   0 david     (1000) david     (1000)     4851 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/utils/mountpoint.py
--rw-rw-r--   0 david     (1000) david     (1000)     4104 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/utils/uenv.py
--rw-rw-r--   0 david     (1000) david     (1000)     3959 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/utils/uprocess.py
--rw-rw-r--   0 david     (1000) david     (1000)     1038 2023-03-23 16:32:24.000000 udocker-1.3.8/udocker/utils/uvolume.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-23 17:19:08.658225 udocker-1.3.8/udocker.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    31810 2023-03-23 17:19:08.000000 udocker-1.3.8/udocker.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     2626 2023-03-23 17:19:08.000000 udocker-1.3.8/udocker.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-23 17:19:08.000000 udocker-1.3.8/udocker.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       50 2023-03-23 17:19:08.000000 udocker-1.3.8/udocker.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-23 17:18:52.000000 udocker-1.3.8/udocker.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-03-23 17:19:08.000000 udocker-1.3.8/udocker.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.967068 udocker-1.3.9/
+-rw-rw-r--   0 david     (1000) david     (1000)      893 2023-01-13 09:37:04.000000 udocker-1.3.9/AUTHORS.md
+-rw-rw-r--   0 david     (1000) david     (1000)    13090 2023-06-07 15:15:23.000000 udocker-1.3.9/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)      418 2023-06-07 14:59:13.000000 udocker-1.3.9/CITING.md
+-rw-rw-r--   0 david     (1000) david     (1000)     5488 2023-06-07 14:59:13.000000 udocker-1.3.9/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 david     (1000) david     (1000)     1821 2023-06-07 14:59:13.000000 udocker-1.3.9/CONTRIBUTING.md
+-rw-r--r--   0 david     (1000) david     (1000)    11357 2019-06-11 07:52:40.000000 udocker-1.3.9/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)       77 2021-06-24 09:56:32.000000 udocker-1.3.9/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)    31806 2023-06-07 15:20:41.971068 udocker-1.3.9/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)    17448 2023-06-07 14:59:13.000000 udocker-1.3.9/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      548 2023-06-07 14:59:13.000000 udocker-1.3.9/SECURITY.md
+-rw-rw-r--   0 david     (1000) david     (1000)      207 2021-06-24 09:56:32.000000 udocker-1.3.9/SUMMARY.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.959068 udocker-1.3.9/docs/
+-rw-rw-r--   0 david     (1000) david     (1000)       26 2021-06-17 16:15:57.000000 udocker-1.3.9/docs/_config.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      144 2023-06-07 14:59:13.000000 udocker-1.3.9/docs/index.md
+-rw-rw-r--   0 david     (1000) david     (1000)    26343 2023-06-07 14:59:13.000000 udocker-1.3.9/docs/installation_manual.md
+-rw-rw-r--   0 david     (1000) david     (1000)    15260 2021-06-17 13:25:20.000000 udocker-1.3.9/docs/logo-small.png
+-rw-rw-r--   0 david     (1000) david     (1000)      814 2023-03-24 14:40:52.000000 udocker-1.3.9/docs/make_release.md
+-rw-rw-r--   0 david     (1000) david     (1000)     3355 2023-06-07 14:59:13.000000 udocker-1.3.9/docs/reference_card.md
+-rw-rw-r--   0 david     (1000) david     (1000)    16365 2023-06-07 14:59:13.000000 udocker-1.3.9/docs/udocker.1
+-rw-rw-r--   0 david     (1000) david     (1000)     1668 2023-06-07 14:59:13.000000 udocker-1.3.9/docs/udocker_organ.md
+-rw-rw-r--   0 david     (1000) david     (1000)    51316 2023-01-13 09:37:04.000000 udocker-1.3.9/docs/user_manual.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.959068 udocker-1.3.9/etc/
+-rw-rw-r--   0 david     (1000) david     (1000)      411 2023-06-07 14:59:13.000000 udocker-1.3.9/etc/udocker.conf
+-rw-rw-r--   0 david     (1000) david     (1000)      162 2023-06-07 15:20:41.971068 udocker-1.3.9/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     2863 2023-06-07 14:59:13.000000 udocker-1.3.9/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.955067 udocker-1.3.9/tests/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.963068 udocker-1.3.9/tests/unit/
+-rwxrwxr-x   0 david     (1000) david     (1000)     3201 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_chksum.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    57341 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_cli.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     3544 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_cmdparser.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    15823 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_commonlocalfile.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     3609 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_config.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    18268 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_containerstructure.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    12181 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_curl.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     2386 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_curlheader.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    32765 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_dockerioapi.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    15470 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_dockerlocalfileapi.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    16813 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_elfpatcher.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    38618 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_execenginecommon.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     7522 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_executionmode.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    14325 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_fakechroot.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     8069 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_filebind.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    45120 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_fileutil.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     5172 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_geturl.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     4699 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_geturlexecurl.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     4729 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_geturlpycurl.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     3423 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_hostinfo.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     5848 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_keystore.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     3864 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_localfile.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    62554 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_localrepository.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    11004 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_mountpoint.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     2036 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_msg.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    10562 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_nixauthentication.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    10913 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_nvidia.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     5019 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_oci.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     4151 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_osinfo.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     8650 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_proot.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    29166 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_runc.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     9693 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_singularity.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    14396 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_tools.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     5160 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_uenv.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     3465 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_umain.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     1879 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_unique.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     3647 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_unshare.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     2660 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_uprocess.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     1220 2023-06-07 14:59:13.000000 udocker-1.3.9/tests/unit/test_uvolume.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.963068 udocker-1.3.9/udocker/
+-rw-rw-r--   0 david     (1000) david     (1000)     1195 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    53914 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7228 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/cmdparser.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10252 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/commonlocalfile.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11794 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/config.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.967068 udocker-1.3.9/udocker/container/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-17 13:25:20.000000 udocker-1.3.9/udocker/container/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    32330 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/container/localrepo.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13281 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/container/structure.py
+-rw-rw-r--   0 david     (1000) david     (1000)    38719 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/docker.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.967068 udocker-1.3.9/udocker/engine/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-17 13:25:20.000000 udocker-1.3.9/udocker/engine/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    28554 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/engine/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5237 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/engine/execmode.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12774 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/engine/fakechroot.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8523 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/engine/nvidia.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7605 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/engine/proot.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17818 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/engine/runc.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7679 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/engine/singularity.py
+-rw-rw-r--   0 david     (1000) david     (1000)      511 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/genstr.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.967068 udocker-1.3.9/udocker/helper/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-17 13:25:20.000000 udocker-1.3.9/udocker/helper/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11501 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/helper/elfpatcher.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5235 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/helper/hostinfo.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3419 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/helper/keystore.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6878 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/helper/nixauth.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3893 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/helper/osinfo.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1707 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/helper/unique.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2457 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/helper/unshare.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1811 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/localfile.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     1698 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/maincmd.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2136 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/msg.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5168 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/oci.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12025 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/tools.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4479 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/umain.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.967068 udocker-1.3.9/udocker/utils/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-17 13:25:20.000000 udocker-1.3.9/udocker/utils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2485 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/utils/chksum.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15599 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/utils/curl.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4436 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/utils/filebind.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22449 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/utils/fileutil.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4851 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/utils/mountpoint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4104 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/utils/uenv.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3959 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/utils/uprocess.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1038 2023-06-07 14:59:13.000000 udocker-1.3.9/udocker/utils/uvolume.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 15:20:41.967068 udocker-1.3.9/udocker.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)    31806 2023-06-07 15:20:41.000000 udocker-1.3.9/udocker.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     2626 2023-06-07 15:20:41.000000 udocker-1.3.9/udocker.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-07 15:20:41.000000 udocker-1.3.9/udocker.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       49 2023-06-07 15:20:41.000000 udocker-1.3.9/udocker.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-07 15:20:05.000000 udocker-1.3.9/udocker.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-06-07 15:20:41.000000 udocker-1.3.9/udocker.egg-info/top_level.txt
```

### Comparing `udocker-1.3.8/AUTHORS.md` & `udocker-1.3.9/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/CHANGELOG.md` & `udocker-1.3.9/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## udocker (1.3.9)
+
+* add support to access non-config metadata from containers
+* added support for multiplatform manifests and indices solves #392
+
 ## udocker (1.3.8)
 
 * build udockertools 1.2.9 and set it as default
 * add Fn support for Ubuntu:22
 * remove files to be installed
 * set Fn preference to use runc
 
@@ -15,28 +20,26 @@
 
 * re-implement udocker namespace solves #380
 * login fails all the time solves #379
 * Ignore image loading if already exists solves #378
 
 ## udocker (1.3.5)
 
-* fix python backwards compatibility issues
-  * closes: #374
+* fix python backwards compatibility issues - closes: #374
 * fix incorrectly reported errors by image verification
 * fix image search returning empty results
 * fix issue with logical links in the udocker executable path
 * add check to verify if container name exists before creation
   or cloning
 * add --force option to create and clone to allow creation
   of container even if the intended name given by --name exists
 * prevent closing of file descriptors upon engine invocation
   improves PMI process management interface interoperability
 * fix issues in import and export while using pipes.
-* fix image name parsing where "library" component is missing
-  * closes: #359
+* fix image name parsing where "library" component is missing - closes: #359
 
 ## udocker (1.3.4)
 
 * fix 2 unit tests
 
 ## udocker (1.3.3)
 
@@ -78,26 +81,22 @@
 * Fix support for `newfstatat()` in Pn execution modes
 * Add Fn libraries for Fedora 34 and Ubuntu 21.04
 * Remove broken links in FileUtil.remove()
 * update minimum udocker tools tarball to 1.2.8
 * Cmd and entrypoint metadata and arguments processing changed to mimic docker
 * Improve removal of files and links in install and filebind restore
 * Add follow location option to GetURL()
-* Implement use of `--entrypoint=<cmd>` to force execution of command
-  * closes: #306
-* Implement use of `--entrypoint=""` to bypass entrypoint in metadata
-  * closes: #306
+* Implement use of `--entrypoint=<cmd>` to force execution of command - closes: #306
+* Implement use of `--entrypoint=""` to bypass entrypoint in metadata - closes: #306
 
 ## udocker (1.2.9)
 
-* method Unshare.unshare os.strerror() takes one argument,
-  * closes: #254
+* method Unshare.unshare os.strerror() takes one argument - closes: #254
 * Add unit test for #254
-* Method chown udocker.utils.fileutil FileUtil
-  * closes: #276
+* Method chown udocker.utils.fileutil FileUtil - closes: #276
 * Several fixes of unit tests and pylint
 * Fix confusion between exit code 0 and inferred False
 * Dereference on `safe_prefixes`
 * untar exclude dev
 * Fix rmi for referenced layers
 * Set default for `PROOT_TMP_DIR`
 * sysdir mountpoint not found and set tmpdir
@@ -111,51 +110,41 @@
 ## udocker (1.2.8b2)
 
 * Fix Rn modes to enable containers execution from readonly dirs
 * Documentation centralized installation and readonly setups
 * Fix handling of dockerhub repository names in /v2
 * Improve documentation and algn with 1.1.8b2
 * Add credits
-* Fix delete of paths with symlinks
-  * closes: #267, #265
-* Fix issues with login credentials
-  * closes: #310
-* Fix pull images from docker hub in Termux
-  * closes: #307
-* Fix issues on running udocker in googlecolab
-  * closes: #286
-* Fix execution with Pn modes in alternate /tmp
-  * closes: #284
+* Fix delete of paths with symlinks - closes: #267, #265
+* Fix issues with login credentials - closes: #310
+* Fix pull images from docker hub in Termux - closes: #307
+* Fix issues on running udocker in googlecolab - closes: #286
+* Fix execution with Pn modes in alternate /tmp - closes: #284
 * Add conditional delay-directory-restore to untar layers
 * Add exclude of whiteouts on layer untar
 * Add --nobanner to udocker run
 
 ## udocker (1.2.7)
 
 * Major restructuring of the code
 * Major restructuring of the unit tests
 * Porting to Python 3, still supports python 2.7
 * all fixes up to previous 1.1.7 version have been applied
 * added scripts tests udocker: `utils/udocker_test.sh utils/udocker_test-run.sh`
 
 ## udocker (1.1.7)
 
-* Fix P1 when Linux 4.8.0 SECCOMP is backported, affects newer CentOS 7
-  * closes: #282
-* Check for file ownership on remove wrongly follows symlinks
-  * closes: #266, #267
-* udocker unexpectedly uses P1 exec mode instead of P2
-  * closes: #274
-* Allow passing of `PROOT_TMP_DIR` environment variable
-  * closes: #284
+* Fix P1 when Linux 4.8.0 SECCOMP is backported, affects newer CentOS 7 - closes: #282
+* Check for file ownership on remove wrongly follows symlinks - closes: #266, #267
+* udocker unexpectedly uses P1 exec mode instead of P2 - closes: #274
+* Allow passing of `PROOT_TMP_DIR` environment variable - closes: #284
 
 ## udocker (1.1.6)
 
-* Complete fix for of ELF paths in modes Fn for $ORIGIN:$ORIGIN
-  * closes: #255
+* Complete fix for of ELF paths in modes Fn for $ORIGIN:$ORIGIN - closes: #255
 
 ## udocker (1.1.5)
 
 * Preliminary fix for of ELF paths in modes Fn for $ORIGIN:$ORIGIN
 * Add Fn libraries for Ubuntu20, Fedora32, Fedora33
 * Add Fn libraries for Alpine 3.12, 3.13
 
@@ -201,185 +190,138 @@
 * Add command rename for renaming of containers
 * Create processes without shell context
 * Safer parsing of config files and removal of directories
 * Improve installation
 * Improved fix of SECCOMP accelerated mode for P1 mode
 * Added loading and handling of container images in OCI format
 * Fixes for udocker in ARM aarch64
-* Fix processing of --dri in Sn mode
-  * closes: #241
-* Improve handling of container and host authentication
-  * partially addresses: #239
-* Fixes to address authentication and redirects in pull
-  * closes: #225, #230
-* Added minimal support to load OCI images
-  * closes: #111
-* Added Pn support for newer distributions
-  * closes: #192
-* Improve the installation of udockertools
-  * closes: #220, #228
-* Read environment variables from file with --env-file=
-  * closes: #212
-* Prepare for pypy
-  * closes: #211
-* Fixes for verification of container images
-  * closes: #209
-* Fix command line processing for "-" in argument
-  * closes: #202
-* Fix file protections on extraction making files u+r
-  * closes: #202, #206
-* Fix comparison of kernel versions having non-integers
-  * closes: #183
-* Support for both manifest V2 schema 1 and schema 2
-  * closes: #218, #225
-* Further improved pathname translation in Fn modes
-  * closes: #160
-* Implement save images in docker format
-  * closes: #74
-* useradd and groupadd not working in containers
-  * closes: #141
-* fix return code when exporting to stdin
-  * closes: #202
+* Fix processing of --dri in Sn mode - closes: #241
+* Improve handling of container and host authentication - partially addresses: #239
+* Fixes to address authentication and redirects in pull - closes: #225, #230
+* Added minimal support to load OCI images - closes: #111
+* Added Pn support for newer distributions - closes: #192
+* Improve the installation of udockertools - closes: #220, #228
+* Read environment variables from file with --env-file= - closes: #212
+* Prepare for pypy - closes: #211
+* Fixes for verification of container images - closes: #209
+* Fix command line processing for "-" in argument - closes: #202
+* Fix file protections on extraction making files u+r - closes: #202, #206
+* Fix comparison of kernel versions having non-integers - closes: #183
+* Support for both manifest V2 schema 1 and schema 2 - closes: #218, #225
+* Further improved pathname translation in Fn modes - closes: #160
+* Implement save images in docker format - closes: #74
+* useradd and groupadd not working in containers - closes: #141
+* fix return code when exporting to stdin - closes: #202
 
 ## udocker (1.1.3)
 
-* Support for nvidia drivers on ubuntu
-  * closes: #162
-* Installation improvements
-  * closes: #166
-* Fix issue on Fn mode symlink convertion
-  * partially addresses: #160
+* Support for nvidia drivers on ubuntu - closes: #162
+* Installation improvements - closes: #166
+* Fix issue on Fn mode symlink conversion - partially addresses: #160
 
 ## udocker (1.1.2)
 
-* Improve parsing of quotes in the command line
-  * closes: #98
-* Fix version command to exit with 0
-  * closes: #107
+* Improve parsing of quotes in the command line - closes: #98
+* Fix version command to exit with 0 - closes: #107
 * Add kill-on-exit to proot on Pn modes
 * Improve download of udocker utils
-* Handle authentication headers when pulling
-  * closes: #110
+* Handle authentication headers when pulling - closes: #110
 * Handle of redirects when pulling
 * Fix registries table
 * Support search quay.io
 * Fix auth header when no standard Docker registry is used
 * Add registry detection on image name
 * Add --version option
-* Force python2 as interpreter
-  * closes: #131
+* Force python2 as interpreter - closes: #131
 * Fix handling of volumes in metadata
 * Handle empty metadata
-* Fix http proxy functionality
-  * closes: #115
-* Ignore --no-trunc and --all in the images command
-  * closes: #108
+* Fix http proxy functionality - closes: #115
+* Ignore --no-trunc and --all in the images command - closes: #108
 * Implement verification of layers in manifest
 * Add --nvidia to support GPUs and related drivers
 * Send download messages to stderr
 * Enable override of curl executable
-* Fix building on CentOS 6
-  * closes: #157
-* Mitigation for upstream limitation in runC without tty
-  * closes: #132
-* Fix detection of executable with symlinks in container
-  * closes: #118
+* Fix building on CentOS 6 - closes: #157
+* Mitigation for upstream limitation in runC without tty - closes: #132
+* Fix detection of executable with symlinks in container - closes: #118
 * Updated runC to v1.0.0-rc5
 * Experimental support for Alpine in Fn modes
-* Improve pathname translation in Fn modes for mounted dirs
-  * partially addresses: #160
+* Improve pathname translation in Fn modes for mounted dirs - partially addresses: #160
 
 ## udocker (1.1.1)
 
 * New execution engine using singularity
 * Updated documentation with OpenMPI information and examples
 * Additional unit tests
 * Redirect messages to stderr
-* Improved parsing of quotes in the command line
-  * closes: #87
+* Improved parsing of quotes in the command line - closes: #87
 * Allow override of the HOME environment variable
 * Allow override of libfakechroot.so at the container level
 * Automatic selection of libfakechroot.so from container info
 * Improve automatic install
 * Enable resetting prefix paths in Fn modes in remote hosts
 * Do not set `AF_UNIX_PATH` in Fn modes when the host /tmp is a volume
 * Export containers in both docker and udocker format
 * Import containers docker and udocker format
 * Load, import and export to/from stdin/stdout
 * Clone existing containers
 * Support for TCP/IP port remap in execution modes Pn
-* Fix run with basenames failing
-  * closes: #89
-* Allow run as root flag
-  * closes: #91
+* Fix run with basenames failing - closes: #89
+* Allow run as root flag - closes: #91
 
 ## udocker (1.1.0)
 
 * Support image names prefixed by registry similarly to docker
 * Add execution engine selection logic
 * Add fr execution engine based on shared library interception
 * Add rc execution engine based on rootless namespaces
 * Improve proot tmp files cleanup on non ext filesystems
 * Improve search returning empty on Docker repositories
 * Improve runC execution portability
-* Add environment variable `UDOCKER_KEYSTORE`
-  * closes: #75
-* Prevent creation of .udocker when `UDOCKER_KEYSTORE` is used
-  * closes: #75
+* Add environment variable `UDOCKER_KEYSTORE` - closes: #75
+* Prevent creation of .udocker when `UDOCKER_KEYSTORE` is used - closes: #75
 
 ## udocker (1.0.4)
 
 * Documentation fixes
 
 ## udocker (1.0.3)
 
 * Support for import Docker containers in newer metadata structure
 * Improve the command line parsing
 * Improve temporary file handling and removal
 * Support for additional execution engines to be provided in the future
-* Improved parsing of entrypoint and cmd metadata
-  * closes: #53
-* Increase name alias length
-  * closes: #52
-* Add support for change dir into volume directories
-  * closes: #51
-* Fix deletion of files upon container import
-  * closes: #50
-* Fix exporting of host environment variables to the containers
-  * closes: #48
-* Change misleading behavior of import tarball from move to copy
-  * closes: #44
-* Fix validation of volumes specification
-  * closes: #43
+* Improved parsing of entrypoint and cmd metadata - closes: #53
+* Increase name alias length - closes: #52
+* Add support for change dir into volume directories - closes: #51
+* Fix deletion of files upon container import - closes: #50
+* Fix exporting of host environment variables to the containers - closes: #48
+* Change misleading behavior of import tarball from move to copy - closes: #44
+* Fix validation of volumes specification - closes: #43
 
 ## udocker (1.0.2)
 
 * Improve download on repositories that fail authentication on /v2
 * Improve run verification of binaries with recursive symbolic links
-* Improve accelerated seccomp on kernels >= 4.8.0
-  * closes: #40
+* Improve accelerated seccomp on kernels >= 4.8.0 - closes: #40
 
 ## udocker (1.0.1)
 
 * Minor bugfixes
 * Executable name changed from udocker.py to udocker
 * Added support for login into docker repositories
 * Added support for private repositories
 * Added support for listing of v2 repositories catalog
 * Added checksum verification for sha256 layers
 * Improved download handling for v1 and v2 repositories
 * Improved installation tarball structure
 * Insecure flag fixed
 * Address seccomp change introduced on kernels >= 4.8.0
 * Utilities for packaging
-* Improved verbose levels, messaging and output
-  * closes: #24, #23
-* Fully implement support for registry selection --registry parameter
-  * closes: #29
-* Provide support for private repositories e.g. gitlab registries
-  * closes: #30
-* Provide --insecure command line parameter for SSL requests
-  * closes: #31
+* Improved verbose levels, messaging and output - closes: #24, #23
+* Fully implement support for registry selection --registry parameter - closes: #29
+* Provide support for private repositories e.g. gitlab registries - closes: #30
+* Provide --insecure command line parameter for SSL requests - closes: #31
 
 ## udocker (1.0.0)
 
 * Initial version
```

### Comparing `udocker-1.3.8/CODE_OF_CONDUCT.md` & `udocker-1.3.9/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -126,8 +126,7 @@
 [https://www.contributor-covenant.org/translations][translations].
 
 [homepage]: https://www.contributor-covenant.org
 [v2.1]: https://www.contributor-covenant.org/version/2/1/code_of_conduct.html
 [Mozilla CoC]: https://github.com/mozilla/diversity
 [FAQ]: https://www.contributor-covenant.org/faq
 [translations]: https://www.contributor-covenant.org/translations
-
```

### Comparing `udocker-1.3.8/CONTRIBUTING.md` & `udocker-1.3.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/LICENSE` & `udocker-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/PKG-INFO` & `udocker-1.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: udocker
-Version: 1.3.8
+Version: 1.3.9
 Summary: A basic user tool to execute simple docker         containers in batch or interactive systems without root privileges
 Home-page: https://github.com/indigo-dc/udocker
 Author: Jorge Gomes
 Author-email: udocker@lip.pt
 License: Apache Software License 2.0
 Keywords: Linux containers,HPC on cloud,Virtualization
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
@@ -56,17 +55,17 @@
 containers with minimal functionality.
 
 ## Documentation
 
 The full documentation is available at:
 
 * [udocker documentation](https://indigo-dc.github.io/udocker/)
-  * [Installation manual](https://indigo-dc.github.io/udocker/installation_manual.html)
-  * [User manual](https://indigo-dc.github.io/udocker/user_manual.html)
-  * [Reference card](https://indigo-dc.github.io/udocker/reference_card.html)
+* [Installation manual](https://indigo-dc.github.io/udocker/installation_manual.html)
+* [User manual](https://indigo-dc.github.io/udocker/user_manual.html)
+* [Reference card](https://indigo-dc.github.io/udocker/reference_card.html)
 
 ## How does it work
 
 udocker is written in Python, it has a minimal set of dependencies so
 that can be executed in a wide range of Linux systems.
 
 udocker does not make use of docker nor requires its presence.
@@ -470,14 +469,19 @@
 The authors wish to acknowleadge the support of INCD-Infraestrutura Nacional de
 Computação Distribuída (funded by FCT, P2020, Lisboa2020, COMPETE and FEDER
 under the project number 22153-01/SAICT/2016).
 
 
 # Changelog
 
+## udocker (1.3.9)
+
+* add support to access non-config metadata from containers
+* added support for multiplatform manifests and indices solves #392
+
 ## udocker (1.3.8)
 
 * build udockertools 1.2.9 and set it as default
 * add Fn support for Ubuntu:22
 * remove files to be installed
 * set Fn preference to use runc
 
@@ -489,28 +493,26 @@
 
 * re-implement udocker namespace solves #380
 * login fails all the time solves #379
 * Ignore image loading if already exists solves #378
 
 ## udocker (1.3.5)
 
-* fix python backwards compatibility issues
-  * closes: #374
+* fix python backwards compatibility issues - closes: #374
 * fix incorrectly reported errors by image verification
 * fix image search returning empty results
 * fix issue with logical links in the udocker executable path
 * add check to verify if container name exists before creation
   or cloning
 * add --force option to create and clone to allow creation
   of container even if the intended name given by --name exists
 * prevent closing of file descriptors upon engine invocation
   improves PMI process management interface interoperability
 * fix issues in import and export while using pipes.
-* fix image name parsing where "library" component is missing
-  * closes: #359
+* fix image name parsing where "library" component is missing - closes: #359
 
 ## udocker (1.3.4)
 
 * fix 2 unit tests
 
 ## udocker (1.3.3)
 
@@ -552,26 +554,22 @@
 * Fix support for `newfstatat()` in Pn execution modes
 * Add Fn libraries for Fedora 34 and Ubuntu 21.04
 * Remove broken links in FileUtil.remove()
 * update minimum udocker tools tarball to 1.2.8
 * Cmd and entrypoint metadata and arguments processing changed to mimic docker
 * Improve removal of files and links in install and filebind restore
 * Add follow location option to GetURL()
-* Implement use of `--entrypoint=<cmd>` to force execution of command
-  * closes: #306
-* Implement use of `--entrypoint=""` to bypass entrypoint in metadata
-  * closes: #306
+* Implement use of `--entrypoint=<cmd>` to force execution of command - closes: #306
+* Implement use of `--entrypoint=""` to bypass entrypoint in metadata - closes: #306
 
 ## udocker (1.2.9)
 
-* method Unshare.unshare os.strerror() takes one argument,
-  * closes: #254
+* method Unshare.unshare os.strerror() takes one argument - closes: #254
 * Add unit test for #254
-* Method chown udocker.utils.fileutil FileUtil
-  * closes: #276
+* Method chown udocker.utils.fileutil FileUtil - closes: #276
 * Several fixes of unit tests and pylint
 * Fix confusion between exit code 0 and inferred False
 * Dereference on `safe_prefixes`
 * untar exclude dev
 * Fix rmi for referenced layers
 * Set default for `PROOT_TMP_DIR`
 * sysdir mountpoint not found and set tmpdir
@@ -585,51 +583,41 @@
 ## udocker (1.2.8b2)
 
 * Fix Rn modes to enable containers execution from readonly dirs
 * Documentation centralized installation and readonly setups
 * Fix handling of dockerhub repository names in /v2
 * Improve documentation and algn with 1.1.8b2
 * Add credits
-* Fix delete of paths with symlinks
-  * closes: #267, #265
-* Fix issues with login credentials
-  * closes: #310
-* Fix pull images from docker hub in Termux
-  * closes: #307
-* Fix issues on running udocker in googlecolab
-  * closes: #286
-* Fix execution with Pn modes in alternate /tmp
-  * closes: #284
+* Fix delete of paths with symlinks - closes: #267, #265
+* Fix issues with login credentials - closes: #310
+* Fix pull images from docker hub in Termux - closes: #307
+* Fix issues on running udocker in googlecolab - closes: #286
+* Fix execution with Pn modes in alternate /tmp - closes: #284
 * Add conditional delay-directory-restore to untar layers
 * Add exclude of whiteouts on layer untar
 * Add --nobanner to udocker run
 
 ## udocker (1.2.7)
 
 * Major restructuring of the code
 * Major restructuring of the unit tests
 * Porting to Python 3, still supports python 2.7
 * all fixes up to previous 1.1.7 version have been applied
 * added scripts tests udocker: `utils/udocker_test.sh utils/udocker_test-run.sh`
 
 ## udocker (1.1.7)
 
-* Fix P1 when Linux 4.8.0 SECCOMP is backported, affects newer CentOS 7
-  * closes: #282
-* Check for file ownership on remove wrongly follows symlinks
-  * closes: #266, #267
-* udocker unexpectedly uses P1 exec mode instead of P2
-  * closes: #274
-* Allow passing of `PROOT_TMP_DIR` environment variable
-  * closes: #284
+* Fix P1 when Linux 4.8.0 SECCOMP is backported, affects newer CentOS 7 - closes: #282
+* Check for file ownership on remove wrongly follows symlinks - closes: #266, #267
+* udocker unexpectedly uses P1 exec mode instead of P2 - closes: #274
+* Allow passing of `PROOT_TMP_DIR` environment variable - closes: #284
 
 ## udocker (1.1.6)
 
-* Complete fix for of ELF paths in modes Fn for $ORIGIN:$ORIGIN
-  * closes: #255
+* Complete fix for of ELF paths in modes Fn for $ORIGIN:$ORIGIN - closes: #255
 
 ## udocker (1.1.5)
 
 * Preliminary fix for of ELF paths in modes Fn for $ORIGIN:$ORIGIN
 * Add Fn libraries for Ubuntu20, Fedora32, Fedora33
 * Add Fn libraries for Alpine 3.12, 3.13
 
@@ -675,187 +663,138 @@
 * Add command rename for renaming of containers
 * Create processes without shell context
 * Safer parsing of config files and removal of directories
 * Improve installation
 * Improved fix of SECCOMP accelerated mode for P1 mode
 * Added loading and handling of container images in OCI format
 * Fixes for udocker in ARM aarch64
-* Fix processing of --dri in Sn mode
-  * closes: #241
-* Improve handling of container and host authentication
-  * partially addresses: #239
-* Fixes to address authentication and redirects in pull
-  * closes: #225, #230
-* Added minimal support to load OCI images
-  * closes: #111
-* Added Pn support for newer distributions
-  * closes: #192
-* Improve the installation of udockertools
-  * closes: #220, #228
-* Read environment variables from file with --env-file=
-  * closes: #212
-* Prepare for pypy
-  * closes: #211
-* Fixes for verification of container images
-  * closes: #209
-* Fix command line processing for "-" in argument
-  * closes: #202
-* Fix file protections on extraction making files u+r
-  * closes: #202, #206
-* Fix comparison of kernel versions having non-integers
-  * closes: #183
-* Support for both manifest V2 schema 1 and schema 2
-  * closes: #218, #225
-* Further improved pathname translation in Fn modes
-  * closes: #160
-* Implement save images in docker format
-  * closes: #74
-* useradd and groupadd not working in containers
-  * closes: #141
-* fix return code when exporting to stdin
-  * closes: #202
+* Fix processing of --dri in Sn mode - closes: #241
+* Improve handling of container and host authentication - partially addresses: #239
+* Fixes to address authentication and redirects in pull - closes: #225, #230
+* Added minimal support to load OCI images - closes: #111
+* Added Pn support for newer distributions - closes: #192
+* Improve the installation of udockertools - closes: #220, #228
+* Read environment variables from file with --env-file= - closes: #212
+* Prepare for pypy - closes: #211
+* Fixes for verification of container images - closes: #209
+* Fix command line processing for "-" in argument - closes: #202
+* Fix file protections on extraction making files u+r - closes: #202, #206
+* Fix comparison of kernel versions having non-integers - closes: #183
+* Support for both manifest V2 schema 1 and schema 2 - closes: #218, #225
+* Further improved pathname translation in Fn modes - closes: #160
+* Implement save images in docker format - closes: #74
+* useradd and groupadd not working in containers - closes: #141
+* fix return code when exporting to stdin - closes: #202
 
 ## udocker (1.1.3)
 
-* Support for nvidia drivers on ubuntu
-  * closes: #162
-* Installation improvements
-  * closes: #166
-* Fix issue on Fn mode symlink convertion
-  * partially addresses: #160
+* Support for nvidia drivers on ubuntu - closes: #162
+* Installation improvements - closes: #166
+* Fix issue on Fn mode symlink conversion - partially addresses: #160
 
 ## udocker (1.1.2)
 
-* Improve parsing of quotes in the command line
-  * closes: #98
-* Fix version command to exit with 0
-  * closes: #107
+* Improve parsing of quotes in the command line - closes: #98
+* Fix version command to exit with 0 - closes: #107
 * Add kill-on-exit to proot on Pn modes
 * Improve download of udocker utils
-* Handle authentication headers when pulling
-  * closes: #110
+* Handle authentication headers when pulling - closes: #110
 * Handle of redirects when pulling
 * Fix registries table
 * Support search quay.io
 * Fix auth header when no standard Docker registry is used
 * Add registry detection on image name
 * Add --version option
-* Force python2 as interpreter
-  * closes: #131
+* Force python2 as interpreter - closes: #131
 * Fix handling of volumes in metadata
 * Handle empty metadata
-* Fix http proxy functionality
-  * closes: #115
-* Ignore --no-trunc and --all in the images command
-  * closes: #108
+* Fix http proxy functionality - closes: #115
+* Ignore --no-trunc and --all in the images command - closes: #108
 * Implement verification of layers in manifest
 * Add --nvidia to support GPUs and related drivers
 * Send download messages to stderr
 * Enable override of curl executable
-* Fix building on CentOS 6
-  * closes: #157
-* Mitigation for upstream limitation in runC without tty
-  * closes: #132
-* Fix detection of executable with symlinks in container
-  * closes: #118
+* Fix building on CentOS 6 - closes: #157
+* Mitigation for upstream limitation in runC without tty - closes: #132
+* Fix detection of executable with symlinks in container - closes: #118
 * Updated runC to v1.0.0-rc5
 * Experimental support for Alpine in Fn modes
-* Improve pathname translation in Fn modes for mounted dirs
-  * partially addresses: #160
+* Improve pathname translation in Fn modes for mounted dirs - partially addresses: #160
 
 ## udocker (1.1.1)
 
 * New execution engine using singularity
 * Updated documentation with OpenMPI information and examples
 * Additional unit tests
 * Redirect messages to stderr
-* Improved parsing of quotes in the command line
-  * closes: #87
+* Improved parsing of quotes in the command line - closes: #87
 * Allow override of the HOME environment variable
 * Allow override of libfakechroot.so at the container level
 * Automatic selection of libfakechroot.so from container info
 * Improve automatic install
 * Enable resetting prefix paths in Fn modes in remote hosts
 * Do not set `AF_UNIX_PATH` in Fn modes when the host /tmp is a volume
 * Export containers in both docker and udocker format
 * Import containers docker and udocker format
 * Load, import and export to/from stdin/stdout
 * Clone existing containers
 * Support for TCP/IP port remap in execution modes Pn
-* Fix run with basenames failing
-  * closes: #89
-* Allow run as root flag
-  * closes: #91
+* Fix run with basenames failing - closes: #89
+* Allow run as root flag - closes: #91
 
 ## udocker (1.1.0)
 
 * Support image names prefixed by registry similarly to docker
 * Add execution engine selection logic
 * Add fr execution engine based on shared library interception
 * Add rc execution engine based on rootless namespaces
 * Improve proot tmp files cleanup on non ext filesystems
 * Improve search returning empty on Docker repositories
 * Improve runC execution portability
-* Add environment variable `UDOCKER_KEYSTORE`
-  * closes: #75
-* Prevent creation of .udocker when `UDOCKER_KEYSTORE` is used
-  * closes: #75
+* Add environment variable `UDOCKER_KEYSTORE` - closes: #75
+* Prevent creation of .udocker when `UDOCKER_KEYSTORE` is used - closes: #75
 
 ## udocker (1.0.4)
 
 * Documentation fixes
 
 ## udocker (1.0.3)
 
 * Support for import Docker containers in newer metadata structure
 * Improve the command line parsing
 * Improve temporary file handling and removal
 * Support for additional execution engines to be provided in the future
-* Improved parsing of entrypoint and cmd metadata
-  * closes: #53
-* Increase name alias length
-  * closes: #52
-* Add support for change dir into volume directories
-  * closes: #51
-* Fix deletion of files upon container import
-  * closes: #50
-* Fix exporting of host environment variables to the containers
-  * closes: #48
-* Change misleading behavior of import tarball from move to copy
-  * closes: #44
-* Fix validation of volumes specification
-  * closes: #43
+* Improved parsing of entrypoint and cmd metadata - closes: #53
+* Increase name alias length - closes: #52
+* Add support for change dir into volume directories - closes: #51
+* Fix deletion of files upon container import - closes: #50
+* Fix exporting of host environment variables to the containers - closes: #48
+* Change misleading behavior of import tarball from move to copy - closes: #44
+* Fix validation of volumes specification - closes: #43
 
 ## udocker (1.0.2)
 
 * Improve download on repositories that fail authentication on /v2
 * Improve run verification of binaries with recursive symbolic links
-* Improve accelerated seccomp on kernels >= 4.8.0
-  * closes: #40
+* Improve accelerated seccomp on kernels >= 4.8.0 - closes: #40
 
 ## udocker (1.0.1)
 
 * Minor bugfixes
 * Executable name changed from udocker.py to udocker
 * Added support for login into docker repositories
 * Added support for private repositories
 * Added support for listing of v2 repositories catalog
 * Added checksum verification for sha256 layers
 * Improved download handling for v1 and v2 repositories
 * Improved installation tarball structure
 * Insecure flag fixed
 * Address seccomp change introduced on kernels >= 4.8.0
 * Utilities for packaging
-* Improved verbose levels, messaging and output
-  * closes: #24, #23
-* Fully implement support for registry selection --registry parameter
-  * closes: #29
-* Provide support for private repositories e.g. gitlab registries
-  * closes: #30
-* Provide --insecure command line parameter for SSL requests
-  * closes: #31
+* Improved verbose levels, messaging and output - closes: #24, #23
+* Fully implement support for registry selection --registry parameter - closes: #29
+* Provide support for private repositories e.g. gitlab registries - closes: #30
+* Provide --insecure command line parameter for SSL requests - closes: #31
 
 ## udocker (1.0.0)
 
 * Initial version
-
-
```

### Comparing `udocker-1.3.8/README.md` & `udocker-1.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 containers with minimal functionality.
 
 ## Documentation
 
 The full documentation is available at:
 
 * [udocker documentation](https://indigo-dc.github.io/udocker/)
-  * [Installation manual](https://indigo-dc.github.io/udocker/installation_manual.html)
-  * [User manual](https://indigo-dc.github.io/udocker/user_manual.html)
-  * [Reference card](https://indigo-dc.github.io/udocker/reference_card.html)
+* [Installation manual](https://indigo-dc.github.io/udocker/installation_manual.html)
+* [User manual](https://indigo-dc.github.io/udocker/user_manual.html)
+* [Reference card](https://indigo-dc.github.io/udocker/reference_card.html)
 
 ## How does it work
 
 udocker is written in Python, it has a minimal set of dependencies so
 that can be executed in a wide range of Linux systems.
 
 udocker does not make use of docker nor requires its presence.
```

### Comparing `udocker-1.3.8/SECURITY.md` & `udocker-1.3.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/docs/installation_manual.md` & `udocker-1.3.9/docs/installation_manual.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,26 +28,26 @@
 ## 2. Installation
 
 ### 2.1. Install from a released version
 
 Download a release tarball from <https://github.com/indigo-dc/udocker/releases>:
 
 ```bash
-wget https://github.com/indigo-dc/udocker/releases/download/1.3.8/udocker-1.3.8.tar.gz
-tar zxvf udocker-1.3.8.tar.gz
-export PATH=`pwd`/udocker-1.3.8/udocker:$PATH
+wget https://github.com/indigo-dc/udocker/releases/download/1.3.9/udocker-1.3.9.tar.gz
+tar zxvf udocker-1.3.9.tar.gz
+export PATH=`pwd`/udocker-1.3.9/udocker:$PATH
 ```
 
 Alternatively use `curl` instead of `wget` as follows:
 
 ```bash
-curl -L https://github.com/indigo-dc/udocker/releases/download/1.3.8/udocker-1.3.8.tar.gz \
-  > udocker-1.3.8.tar.gz
-tar zxvf udocker-1.3.8.tar.gz
-export PATH=`pwd`/udocker-1.3.8/udocker:$PATH
+curl -L https://github.com/indigo-dc/udocker/releases/download/1.3.9/udocker-1.3.9.tar.gz \
+  > udocker-1.3.9.tar.gz
+tar zxvf udocker-1.3.9.tar.gz
+export PATH=`pwd`/udocker-1.3.9/udocker:$PATH
 ```
 
 udocker executes containers using external tools and libraries that
 are enhanced and packaged for use with udocker. For more information see
 [section 6 External tools and libraries](#6-external-tools-and-libraries).
 Therefore to complete the installation invoke `udocker install` to download
 and install the required tools and libraries.
@@ -341,16 +341,16 @@
 subdirectories: `bin`,  `containers`,  `layers`,  `lib`,  `repos`. For the
 binaries and libraries the only directories required are `bin` and `lib`.
 
 The udocker tool should be installed as shown in section 2.1:
 
 ```bash
 cd /sw
-wget https://github.com/indigo-dc/udocker/releases/download/1.3.8/udocker-1.3.8.tar.gz
-tar zxvf udocker-1.3.8.tar.gz
+wget https://github.com/indigo-dc/udocker/releases/download/1.3.9/udocker-1.3.9.tar.gz
+tar zxvf udocker-1.3.9.tar.gz
 ```
 
 Directing users to the central udocker installation can be done using the
 environment variables described in section 5, or through the configuration files
 described in section 6. The recommended approach is to set environment
 variables at the user level as in the example where the assumed central location
 will be under `/sw/udocker`:
```

### Comparing `udocker-1.3.8/docs/logo-small.png` & `udocker-1.3.9/docs/logo-small.png`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/docs/make_release.md` & `udocker-1.3.9/docs/make_release.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 cd utils
 ./make_udockertar.sh
 cd ..
 ```
 
 * It produces udocker-x.y.z.tar.gz
 * On github make a **new release** and upload this tarball, copy/paste text
-  from other release.
+  from other release.
```

### Comparing `udocker-1.3.8/docs/reference_card.md` & `udocker-1.3.9/docs/reference_card.md`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/docs/udocker.1` & `udocker-1.3.9/docs/udocker.1`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/docs/udocker_organ.md` & `udocker-1.3.9/docs/udocker_organ.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,37 +6,36 @@
 
 ## Base directory
 
 dir = .
 
 * udocker.py - class Main(object):
 * cmdparser.py - class CmdParser(object):
-* cli.py -     class UdockerCLI(object):
-  * This is the command line implementation
+* cli.py -     class UdockerCLI(object): This is the command line implementation
 * config.py -  class Config(object):
 * tools.py -   class UdockerTools(object):
 * msg.py - class Msg(object):
 * docker.py:
-  * class DockerIoAPI(object):
-  * class DockerLocalFileAPI(object):
+* class DockerIoAPI(object):
+* class DockerLocalFileAPI(object):
 
 ## Directory utils
 
 dir = utils/
 
 * uprocess.py - class Uprocess(object):
 * filebind.py - class FileBind(object):
 * fileutil.py - class FileUtil(object):
 * chkcsum.py -  class ChkSUM(object):
 
 * curl.py:
-  * class CurlHeader(object):
-  * class GetURL(object):
-  * class GetURLpyCurl(GetURL):
-  * class GetURLexeCurl(GetURL):
+* class CurlHeader(object):
+* class GetURL(object):
+* class GetURLpyCurl(GetURL):
+* class GetURLexeCurl(GetURL):
 
 ## Directory helper
 
 dir = helper
 
 * guestinfo.py -  class GuestInfo(object):
 * keystore.py -   class KeyStore(object):
```

### Comparing `udocker-1.3.8/docs/user_manual.md` & `udocker-1.3.9/docs/user_manual.md`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/setup.py` & `udocker-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_chksum.py` & `udocker-1.3.9/tests/unit/test_chksum.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_cli.py` & `udocker-1.3.9/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_cmdparser.py` & `udocker-1.3.9/tests/unit/test_cmdparser.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_commonlocalfile.py` & `udocker-1.3.9/tests/unit/test_commonlocalfile.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_config.py` & `udocker-1.3.9/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_containerstructure.py` & `udocker-1.3.9/tests/unit/test_containerstructure.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_curl.py` & `udocker-1.3.9/tests/unit/test_curl.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_curlheader.py` & `udocker-1.3.9/tests/unit/test_curlheader.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_dockerioapi.py` & `udocker-1.3.9/tests/unit/test_dockerioapi.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_dockerlocalfileapi.py` & `udocker-1.3.9/tests/unit/test_dockerlocalfileapi.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_elfpatcher.py` & `udocker-1.3.9/tests/unit/test_elfpatcher.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_execenginecommon.py` & `udocker-1.3.9/tests/unit/test_execenginecommon.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_executionmode.py` & `udocker-1.3.9/tests/unit/test_executionmode.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_fakechroot.py` & `udocker-1.3.9/tests/unit/test_fakechroot.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_filebind.py` & `udocker-1.3.9/tests/unit/test_filebind.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_fileutil.py` & `udocker-1.3.9/tests/unit/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_geturl.py` & `udocker-1.3.9/tests/unit/test_geturl.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_geturlexecurl.py` & `udocker-1.3.9/tests/unit/test_geturlexecurl.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_geturlpycurl.py` & `udocker-1.3.9/tests/unit/test_geturlpycurl.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_hostinfo.py` & `udocker-1.3.9/tests/unit/test_hostinfo.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_keystore.py` & `udocker-1.3.9/tests/unit/test_keystore.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_localfile.py` & `udocker-1.3.9/tests/unit/test_localfile.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_localrepository.py` & `udocker-1.3.9/tests/unit/test_localrepository.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_mountpoint.py` & `udocker-1.3.9/tests/unit/test_mountpoint.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_msg.py` & `udocker-1.3.9/tests/unit/test_msg.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_nixauthentication.py` & `udocker-1.3.9/tests/unit/test_nixauthentication.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_nvidia.py` & `udocker-1.3.9/tests/unit/test_nvidia.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_oci.py` & `udocker-1.3.9/tests/unit/test_oci.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_osinfo.py` & `udocker-1.3.9/tests/unit/test_osinfo.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_proot.py` & `udocker-1.3.9/tests/unit/test_proot.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_runc.py` & `udocker-1.3.9/tests/unit/test_runc.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_singularity.py` & `udocker-1.3.9/tests/unit/test_singularity.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_tools.py` & `udocker-1.3.9/tests/unit/test_tools.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_uenv.py` & `udocker-1.3.9/tests/unit/test_uenv.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_umain.py` & `udocker-1.3.9/tests/unit/test_umain.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_unique.py` & `udocker-1.3.9/tests/unit/test_unique.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_unshare.py` & `udocker-1.3.9/tests/unit/test_unshare.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_uprocess.py` & `udocker-1.3.9/tests/unit/test_uprocess.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/tests/unit/test_uvolume.py` & `udocker-1.3.9/tests/unit/test_uvolume.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/__init__.py` & `udocker-1.3.9/udocker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,9 @@
     "PRoot http://proot.me",
     "runC https://runc.io",
     "crun https://github.com/containers/crun",
     "Fakechroot https://github.com/dex4er/fakechroot",
     "Singularity http://singularity.lbl.gov"
     ]
 __license__ = "Licensed under the Apache License, Version 2.0"
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __date__ = "2023"
```

### Comparing `udocker-1.3.8/udocker/cli.py` & `udocker-1.3.9/udocker/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,30 +528,32 @@
         --httpproxy=socks5://host:port                  :use http proxy
         --httpproxy=socks4a://user:pass@host:port       :use http proxy
         --httpproxy=socks5h://user:pass@host:port       :use http proxy
         --httpproxy=socks4a://host:port                 :use http proxy
         --httpproxy=socks5h://host:port                 :use http proxy
         --index=https://index.docker.io/v1              :docker index
         --registry=https://registry-1.docker.io         :docker registry
+        --platform=os/arch                              :docker platform
 
         Examples:
           pull fedora:latest
           pull quay.io/something/somewhere:latest
         """
         index_url = cmdp.get("--index=")
         registry_url = cmdp.get("--registry=")
         http_proxy = cmdp.get("--httpproxy=")
+        platform = cmdp.get("--platform=")
         (imagerepo, tag) = self._check_imagespec(cmdp.get("P1"))
         if (not imagerepo) or cmdp.missing_options():    # syntax error
             return self.STATUS_ERROR
 
         self._set_repository(registry_url, index_url, imagerepo, http_proxy)
         v2_auth_token = self.keystore.get(self.dockerioapi.registry_url)
         self.dockerioapi.set_v2_login_token(v2_auth_token)
-        if self.dockerioapi.get(imagerepo, tag):
+        if self.dockerioapi.get(imagerepo, tag, platform):
             return self.STATUS_OK
 
         Msg().err("Error: no files downloaded")
         return self.STATUS_ERROR
 
     def _create(self, imagespec):
         """Auxiliary to create(), performs the creation"""
@@ -686,14 +688,18 @@
             "devices": {
                 "fl": ("--device=",), "act": "E",
                 "p2": "CMD_OPT", "p3": True
             },
             "nobanner": {
                 "fl": ("--nobanner",), "act": 'R',
                 "p2": "CMD_OPT", "p3": False
+            },
+            "platform": {
+                "fl": ("--platform=",), "act": 'R',
+                "p2": "CMD_OPT", "p3": False
             }
         }
         for option, cmdp_args in list(cmd_options.items()):
             last_value = None
             for cmdp_fl in cmdp_args["fl"]:
                 option_value = cmdp.get(cmdp_fl, cmdp_args["p2"],
                                         cmdp_args["p3"])
```

### Comparing `udocker-1.3.8/udocker/cmdparser.py` & `udocker-1.3.9/udocker/cmdparser.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/commonlocalfile.py` & `udocker-1.3.9/udocker/commonlocalfile.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/config.py` & `udocker-1.3.9/udocker/config.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/container/localrepo.py` & `udocker-1.3.9/udocker/container/localrepo.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/container/structure.py` & `udocker-1.3.9/udocker/container/structure.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 """Tools to manage the container structure"""
 
 import os
 import subprocess
 
-from udocker.genstr import is_genstr
 from udocker.config import Config
 from udocker.msg import Msg
 from udocker.helper.unique import Unique
 from udocker.helper.hostinfo import HostInfo
 from udocker.utils.fileutil import FileUtil
 from udocker.utils.uprocess import Uprocess
 
@@ -41,41 +40,47 @@
             container_json = self.localrepo.load_json(fjson)
             if not container_json:
                 Msg().err("Error: invalid container json metadata")
                 return (False, False)
 
         return (container_dir, container_json)
 
-    def get_container_meta(self, param, default, container_json):
-        """Get the container metadata from the container"""
-        confidx = ""
-        if "config" in container_json:
-            confidx = "config"
-        elif "container_config" in container_json:
-            confidx = "container_config"
-        if container_json[confidx] and param in container_json[confidx]:
-            if container_json[confidx][param] is None:
-                pass
-            elif (is_genstr(container_json[confidx][param]) and
-                  (isinstance(default, (list, tuple)))):
-                return container_json[confidx][param].strip().split()
-            elif (is_genstr(default) and (
-                    isinstance(container_json[confidx][param], (list, tuple)))):
-                return " ".join(container_json[confidx][param])
-            elif (is_genstr(default) and (
-                    isinstance(container_json[confidx][param], dict))):
-                return self._dict_to_str(container_json[confidx][param])
-            elif (isinstance(default, list) and (
-                    isinstance(container_json[confidx][param], dict))):
-                return self._dict_to_list(container_json[confidx][param])
-            else:
-                return container_json[confidx][param]
+    def get_container_meta(self, param, default, cntjson):
+        """Get the metadata configuration from the container"""
+        cidx = ""
+        if "config" in cntjson:
+            cidx = "config"
+        elif "container_config" in cntjson:
+            cidx = "container_config"
+
+        meta_item = None
+        if cntjson[cidx] and param in cntjson[cidx]:
+            meta_item = cntjson[cidx][param]
+        elif param in cntjson:
+            meta_item = cntjson[param]
+
+        if meta_item is None:
+            pass
+        elif (isinstance(meta_item, str) and
+              (isinstance(default, (list, tuple)))):
+            return meta_item.strip().split()
+        elif (isinstance(default, str) and
+              (isinstance(meta_item, (list, tuple)))):
+            return " ".join(meta_item)
+        elif (isinstance(default, str) and
+              (isinstance(meta_item, dict))):
+            return self._dict_to_str(meta_item)
+        elif (isinstance(default, list) and
+              (isinstance(meta_item, dict))):
+            return self._dict_to_list(meta_item)
+        else:
+            return meta_item
+
         return default
 
-    # DEBUG
     def _dict_to_str(self, in_dict):
         """Convert dict to str"""
         out_str = ""
         for (key, val) in in_dict.items():
             out_str += "%s:%s " % (str(key), str(val))
         return out_str
```

### Comparing `udocker-1.3.8/udocker/docker.py` & `udocker-1.3.9/udocker/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from udocker.config import Config
 from udocker.msg import Msg
 from udocker.commonlocalfile import CommonLocalFileApi
 from udocker.helper.unique import Unique
 from udocker.utils.fileutil import FileUtil
 from udocker.utils.curl import GetURL
 from udocker.utils.chksum import ChkSUM
+from udocker.helper.hostinfo import HostInfo
 
 
 class DockerIoAPI(object):
     """Class to encapsulate the access to the Docker Hub service
     Allows to search and download images from Docker Hub
     """
 
@@ -92,15 +93,19 @@
                     return (hdr, buf)
                 auth_header = ""
                 if "/v2/" in url:
                     auth_header = self._get_v2_auth(www_authenticate,
                                                     kwargs["RETRY"])
                 if "/v1/" in url:
                     auth_header = self._get_v1_auth(www_authenticate)
-                auth_kwargs.update({"header": [auth_header]})
+                # OCI and multiplatform, prevent removal of header attributes
+                try:
+                    auth_kwargs["header"].append(auth_header)
+                except KeyError:
+                    auth_kwargs.update({"header": [auth_header]})
         (hdr, buf) = self._get_url(*args, **auth_kwargs)
         return (hdr, buf)
 
     def _get_file(self, url, filename, cache_mode):
         """Get a file and check its size. Optionally enable other
         capabilities such as caching to check if the
         file already exists locally and whether its size is the
@@ -352,26 +357,79 @@
                     tags.append(tag)
                 return tags
 
             return json.loads(buf.getvalue().decode())
         except (IOError, OSError, AttributeError, ValueError, TypeError):
             return []
 
-    def get_v2_image_manifest(self, imagerepo, tag):
-        """Get the image manifest which contains JSON metadata
+    def _get_v2_digest_from_image_index(self, image_index, platform):
+        """Get OCI or docker manifest from an image index"""
+        if isinstance(image_index, dict):
+            index_list = image_index
+        else:
+            try:
+                index_list = json.loads(image_index.decode())
+            except (OSError, AttributeError, ValueError, TypeError):
+                return ""
+        (p_os, p_architecture, p_variant) = HostInfo().parse_platform(platform)
+        try:
+            for manifest in index_list["manifests"]:
+                manifest_p = manifest["platform"]
+                if (p_os and
+                    (manifest_p["os"]).lower() != p_os):
+                    continue
+                if (p_architecture and
+                    (manifest_p["architecture"]).lower() != p_architecture):
+                    continue
+                if (p_variant and
+                    (manifest_p["variant"]).lower() != p_variant):
+                    continue
+                return manifest["digest"]
+        except (KeyError, AttributeError, ValueError, TypeError):
+            pass
+        return ""
+
+    def get_v2_image_manifest(self, imagerepo, tag, platform=""):
+        """API v2 Get the image manifest which contains JSON metadata
         that is common to all layers in this image tag
         """
-        url = self.registry_url + "/v2/" + imagerepo + \
-            "/manifests/" + tag
+        reqhdr = [
+            'Accept: application/vnd.docker.distribution.manifest.v2+json',
+            'Accept: application/vnd.docker.distribution.manifest.v1+prettyjws',
+            'Accept: application/json',
+            'Accept: application/vnd.docker.distribution.manifest.list.v2+json',
+            'Accept: application/vnd.oci.image.manifest.v1+json',
+            'Accept: application/vnd.oci.image.index.v1+json',
+        ]
+        url = self.registry_url + "/v2/" + imagerepo + "/manifests/" + tag
         Msg().out("Debug: manifest url", url, l=Msg.DBG)
-        (hdr, buf) = self._get_url(url)
+        (hdr, buf) = self._get_url(url, header=reqhdr)
+
         try:
-            return (hdr.data, json.loads(buf.getvalue().decode()))
-        except (IOError, OSError, AttributeError, ValueError, TypeError):
-            return (hdr.data, [])
+            content_type = hdr.data['content-type']
+            if "docker.distribution.manifest.v1" in content_type:
+                return (hdr.data, json.loads(buf.getvalue().decode()))
+            if "docker.distribution.manifest.v2" in content_type:
+                return (hdr.data, json.loads(buf.getvalue().decode()))
+            if "oci.image.manifest.v1+json" in content_type:
+                return (hdr.data, json.loads(buf.getvalue().decode()))
+            if ("docker.distribution.manifest.list.v2" in content_type
+                or "oci.image.index.v1+json" in content_type):
+                image_index = json.loads(buf.getvalue().decode())
+                digest = self._get_v2_digest_from_image_index(image_index,
+                                                              platform)
+                if not digest:
+                    Msg().err("no image found in manifest for platform (%s)" %
+                              HostInfo().platform_to_str(platform))
+                else:
+                    return self.get_v2_image_manifest(imagerepo,
+                                                      digest, platform)
+        except (OSError, KeyError, AttributeError, ValueError, TypeError):
+            pass
+        return (hdr.data, [])
 
     def get_v2_image_layer(self, imagerepo, layer_id):
         """Get one image layer data file (tarball)"""
         url = self.registry_url + "/v2/" + imagerepo + \
             "/blobs/" + layer_id
         Msg().out("Debug: layer url", url, l=Msg.DBG)
         filename = self.localrepo.layersdir + '/' + layer_id
@@ -392,25 +450,29 @@
                     blob = layer["digest"]
                 Msg().out("Info: downloading layer", blob, l=Msg.INF)
                 if not self.get_v2_image_layer(imagerepo, blob):
                     return []
                 files.append(blob)
         return files
 
-    def get_v2(self, imagerepo, tag):
+    def get_v2(self, imagerepo, tag, platform=""):
         """Pull container with v2 API"""
         files = []
-        (hdr_data, manifest) = self.get_v2_image_manifest(imagerepo, tag)
+        (hdr_data, manifest) = self.get_v2_image_manifest(imagerepo, tag,
+                                                          platform)
         status = self.curl.get_status_code(hdr_data["X-ND-HTTPSTATUS"])
         if status == 401:
             Msg().err("Error: manifest not found or not authorized")
             return []
         if status != 200:
             Msg().err("Error: pulling manifest:")
             return []
+        if not manifest:
+            Msg().err("no manifest for given image and platform")
+            return []
         try:
             if not (self.localrepo.setup_tag(tag) and
                     self.localrepo.set_version("v2")):
                 Msg().err("Error: setting localrepo v2 tag and version")
                 return []
             self.localrepo.save_json("manifest", manifest)
             Msg().out("Debug: v2 layers: %s" % (imagerepo), l=Msg.DBG)
@@ -514,25 +576,27 @@
                 index_url = registry_url
             if registry_url:
                 self.registry_url = registry_url
             if index_url:
                 self.index_url = index_url
         return (imagerepo, remoterepo)
 
-    def get(self, imagerepo, tag):
+    def get(self, imagerepo, tag, platform=""):
         """Pull a docker image from a v2 registry or v1 index"""
         Msg().out("Debug: get imagerepo: %s tag: %s" % (imagerepo, tag), l=Msg.DBG)
         (imagerepo, remoterepo) = self._parse_imagerepo(imagerepo)
         if self.localrepo.cd_imagerepo(imagerepo, tag):
             new_repo = False
         else:
             self.localrepo.setup_imagerepo(imagerepo)
             new_repo = True
         if self.is_v2():
-            files = self.get_v2(remoterepo, tag)  # try v2
+            if not platform:
+                platform = HostInfo().platform()
+            files = self.get_v2(remoterepo, tag, platform)  # try v2
         else:
             files = self.get_v1(remoterepo, tag)  # try v1
         if new_repo and not files:
             self.localrepo.del_imagerepo(imagerepo, tag, False)
         return files
 
     def get_tags(self, imagerepo):
```

### Comparing `udocker-1.3.8/udocker/engine/base.py` & `udocker-1.3.9/udocker/engine/base.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/engine/execmode.py` & `udocker-1.3.9/udocker/engine/execmode.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/engine/fakechroot.py` & `udocker-1.3.9/udocker/engine/fakechroot.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/engine/nvidia.py` & `udocker-1.3.9/udocker/engine/nvidia.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/engine/proot.py` & `udocker-1.3.9/udocker/engine/proot.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/engine/runc.py` & `udocker-1.3.9/udocker/engine/runc.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/engine/singularity.py` & `udocker-1.3.9/udocker/engine/singularity.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/helper/elfpatcher.py` & `udocker-1.3.9/udocker/helper/elfpatcher.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/helper/keystore.py` & `udocker-1.3.9/udocker/helper/keystore.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/helper/nixauth.py` & `udocker-1.3.9/udocker/helper/nixauth.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/helper/osinfo.py` & `udocker-1.3.9/udocker/helper/osinfo.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/helper/unique.py` & `udocker-1.3.9/udocker/helper/unique.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/helper/unshare.py` & `udocker-1.3.9/udocker/helper/unshare.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/localfile.py` & `udocker-1.3.9/udocker/localfile.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/maincmd.py` & `udocker-1.3.9/udocker/maincmd.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/msg.py` & `udocker-1.3.9/udocker/msg.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/oci.py` & `udocker-1.3.9/udocker/oci.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/tools.py` & `udocker-1.3.9/udocker/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
             if status:
                 return True
         return False
 
     def install(self, force=False):
         """Get the udocker tools tarball and install the binaries"""
         if self.is_available() and not force:
-            Msg().out("Info: already installed, installation skipped", l=Msg.INF)
+            Msg().out("Debug: already installed, installation skipped", l=Msg.DBG)
             return True
 
         if not self._autoinstall and not force:
             Msg().out("Warning: installation missing and autoinstall disabled",
                       l=Msg.WAR)
             return None
```

### Comparing `udocker-1.3.8/udocker/umain.py` & `udocker-1.3.9/udocker/umain.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/utils/chksum.py` & `udocker-1.3.9/udocker/utils/chksum.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/utils/curl.py` & `udocker-1.3.9/udocker/utils/curl.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/utils/filebind.py` & `udocker-1.3.9/udocker/utils/filebind.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/utils/fileutil.py` & `udocker-1.3.9/udocker/utils/fileutil.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/utils/mountpoint.py` & `udocker-1.3.9/udocker/utils/mountpoint.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/utils/uenv.py` & `udocker-1.3.9/udocker/utils/uenv.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/utils/uprocess.py` & `udocker-1.3.9/udocker/utils/uprocess.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker/utils/uvolume.py` & `udocker-1.3.9/udocker/utils/uvolume.py`

 * *Files identical despite different names*

### Comparing `udocker-1.3.8/udocker.egg-info/PKG-INFO` & `udocker-1.3.9/udocker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: udocker
-Version: 1.3.8
+Version: 1.3.9
 Summary: A basic user tool to execute simple docker         containers in batch or interactive systems without root privileges
 Home-page: https://github.com/indigo-dc/udocker
 Author: Jorge Gomes
 Author-email: udocker@lip.pt
 License: Apache Software License 2.0
 Keywords: Linux containers,HPC on cloud,Virtualization
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
@@ -56,17 +55,17 @@
 containers with minimal functionality.
 
 ## Documentation
 
 The full documentation is available at:
 
 * [udocker documentation](https://indigo-dc.github.io/udocker/)
-  * [Installation manual](https://indigo-dc.github.io/udocker/installation_manual.html)
-  * [User manual](https://indigo-dc.github.io/udocker/user_manual.html)
-  * [Reference card](https://indigo-dc.github.io/udocker/reference_card.html)
+* [Installation manual](https://indigo-dc.github.io/udocker/installation_manual.html)
+* [User manual](https://indigo-dc.github.io/udocker/user_manual.html)
+* [Reference card](https://indigo-dc.github.io/udocker/reference_card.html)
 
 ## How does it work
 
 udocker is written in Python, it has a minimal set of dependencies so
 that can be executed in a wide range of Linux systems.
 
 udocker does not make use of docker nor requires its presence.
@@ -470,14 +469,19 @@
 The authors wish to acknowleadge the support of INCD-Infraestrutura Nacional de
 Computação Distribuída (funded by FCT, P2020, Lisboa2020, COMPETE and FEDER
 under the project number 22153-01/SAICT/2016).
 
 
 # Changelog
 
+## udocker (1.3.9)
+
+* add support to access non-config metadata from containers
+* added support for multiplatform manifests and indices solves #392
+
 ## udocker (1.3.8)
 
 * build udockertools 1.2.9 and set it as default
 * add Fn support for Ubuntu:22
 * remove files to be installed
 * set Fn preference to use runc
 
@@ -489,28 +493,26 @@
 
 * re-implement udocker namespace solves #380
 * login fails all the time solves #379
 * Ignore image loading if already exists solves #378
 
 ## udocker (1.3.5)
 
-* fix python backwards compatibility issues
-  * closes: #374
+* fix python backwards compatibility issues - closes: #374
 * fix incorrectly reported errors by image verification
 * fix image search returning empty results
 * fix issue with logical links in the udocker executable path
 * add check to verify if container name exists before creation
   or cloning
 * add --force option to create and clone to allow creation
   of container even if the intended name given by --name exists
 * prevent closing of file descriptors upon engine invocation
   improves PMI process management interface interoperability
 * fix issues in import and export while using pipes.
-* fix image name parsing where "library" component is missing
-  * closes: #359
+* fix image name parsing where "library" component is missing - closes: #359
 
 ## udocker (1.3.4)
 
 * fix 2 unit tests
 
 ## udocker (1.3.3)
 
@@ -552,26 +554,22 @@
 * Fix support for `newfstatat()` in Pn execution modes
 * Add Fn libraries for Fedora 34 and Ubuntu 21.04
 * Remove broken links in FileUtil.remove()
 * update minimum udocker tools tarball to 1.2.8
 * Cmd and entrypoint metadata and arguments processing changed to mimic docker
 * Improve removal of files and links in install and filebind restore
 * Add follow location option to GetURL()
-* Implement use of `--entrypoint=<cmd>` to force execution of command
-  * closes: #306
-* Implement use of `--entrypoint=""` to bypass entrypoint in metadata
-  * closes: #306
+* Implement use of `--entrypoint=<cmd>` to force execution of command - closes: #306
+* Implement use of `--entrypoint=""` to bypass entrypoint in metadata - closes: #306
 
 ## udocker (1.2.9)
 
-* method Unshare.unshare os.strerror() takes one argument,
-  * closes: #254
+* method Unshare.unshare os.strerror() takes one argument - closes: #254
 * Add unit test for #254
-* Method chown udocker.utils.fileutil FileUtil
-  * closes: #276
+* Method chown udocker.utils.fileutil FileUtil - closes: #276
 * Several fixes of unit tests and pylint
 * Fix confusion between exit code 0 and inferred False
 * Dereference on `safe_prefixes`
 * untar exclude dev
 * Fix rmi for referenced layers
 * Set default for `PROOT_TMP_DIR`
 * sysdir mountpoint not found and set tmpdir
@@ -585,51 +583,41 @@
 ## udocker (1.2.8b2)
 
 * Fix Rn modes to enable containers execution from readonly dirs
 * Documentation centralized installation and readonly setups
 * Fix handling of dockerhub repository names in /v2
 * Improve documentation and algn with 1.1.8b2
 * Add credits
-* Fix delete of paths with symlinks
-  * closes: #267, #265
-* Fix issues with login credentials
-  * closes: #310
-* Fix pull images from docker hub in Termux
-  * closes: #307
-* Fix issues on running udocker in googlecolab
-  * closes: #286
-* Fix execution with Pn modes in alternate /tmp
-  * closes: #284
+* Fix delete of paths with symlinks - closes: #267, #265
+* Fix issues with login credentials - closes: #310
+* Fix pull images from docker hub in Termux - closes: #307
+* Fix issues on running udocker in googlecolab - closes: #286
+* Fix execution with Pn modes in alternate /tmp - closes: #284
 * Add conditional delay-directory-restore to untar layers
 * Add exclude of whiteouts on layer untar
 * Add --nobanner to udocker run
 
 ## udocker (1.2.7)
 
 * Major restructuring of the code
 * Major restructuring of the unit tests
 * Porting to Python 3, still supports python 2.7
 * all fixes up to previous 1.1.7 version have been applied
 * added scripts tests udocker: `utils/udocker_test.sh utils/udocker_test-run.sh`
 
 ## udocker (1.1.7)
 
-* Fix P1 when Linux 4.8.0 SECCOMP is backported, affects newer CentOS 7
-  * closes: #282
-* Check for file ownership on remove wrongly follows symlinks
-  * closes: #266, #267
-* udocker unexpectedly uses P1 exec mode instead of P2
-  * closes: #274
-* Allow passing of `PROOT_TMP_DIR` environment variable
-  * closes: #284
+* Fix P1 when Linux 4.8.0 SECCOMP is backported, affects newer CentOS 7 - closes: #282
+* Check for file ownership on remove wrongly follows symlinks - closes: #266, #267
+* udocker unexpectedly uses P1 exec mode instead of P2 - closes: #274
+* Allow passing of `PROOT_TMP_DIR` environment variable - closes: #284
 
 ## udocker (1.1.6)
 
-* Complete fix for of ELF paths in modes Fn for $ORIGIN:$ORIGIN
-  * closes: #255
+* Complete fix for of ELF paths in modes Fn for $ORIGIN:$ORIGIN - closes: #255
 
 ## udocker (1.1.5)
 
 * Preliminary fix for of ELF paths in modes Fn for $ORIGIN:$ORIGIN
 * Add Fn libraries for Ubuntu20, Fedora32, Fedora33
 * Add Fn libraries for Alpine 3.12, 3.13
 
@@ -675,187 +663,138 @@
 * Add command rename for renaming of containers
 * Create processes without shell context
 * Safer parsing of config files and removal of directories
 * Improve installation
 * Improved fix of SECCOMP accelerated mode for P1 mode
 * Added loading and handling of container images in OCI format
 * Fixes for udocker in ARM aarch64
-* Fix processing of --dri in Sn mode
-  * closes: #241
-* Improve handling of container and host authentication
-  * partially addresses: #239
-* Fixes to address authentication and redirects in pull
-  * closes: #225, #230
-* Added minimal support to load OCI images
-  * closes: #111
-* Added Pn support for newer distributions
-  * closes: #192
-* Improve the installation of udockertools
-  * closes: #220, #228
-* Read environment variables from file with --env-file=
-  * closes: #212
-* Prepare for pypy
-  * closes: #211
-* Fixes for verification of container images
-  * closes: #209
-* Fix command line processing for "-" in argument
-  * closes: #202
-* Fix file protections on extraction making files u+r
-  * closes: #202, #206
-* Fix comparison of kernel versions having non-integers
-  * closes: #183
-* Support for both manifest V2 schema 1 and schema 2
-  * closes: #218, #225
-* Further improved pathname translation in Fn modes
-  * closes: #160
-* Implement save images in docker format
-  * closes: #74
-* useradd and groupadd not working in containers
-  * closes: #141
-* fix return code when exporting to stdin
-  * closes: #202
+* Fix processing of --dri in Sn mode - closes: #241
+* Improve handling of container and host authentication - partially addresses: #239
+* Fixes to address authentication and redirects in pull - closes: #225, #230
+* Added minimal support to load OCI images - closes: #111
+* Added Pn support for newer distributions - closes: #192
+* Improve the installation of udockertools - closes: #220, #228
+* Read environment variables from file with --env-file= - closes: #212
+* Prepare for pypy - closes: #211
+* Fixes for verification of container images - closes: #209
+* Fix command line processing for "-" in argument - closes: #202
+* Fix file protections on extraction making files u+r - closes: #202, #206
+* Fix comparison of kernel versions having non-integers - closes: #183
+* Support for both manifest V2 schema 1 and schema 2 - closes: #218, #225
+* Further improved pathname translation in Fn modes - closes: #160
+* Implement save images in docker format - closes: #74
+* useradd and groupadd not working in containers - closes: #141
+* fix return code when exporting to stdin - closes: #202
 
 ## udocker (1.1.3)
 
-* Support for nvidia drivers on ubuntu
-  * closes: #162
-* Installation improvements
-  * closes: #166
-* Fix issue on Fn mode symlink convertion
-  * partially addresses: #160
+* Support for nvidia drivers on ubuntu - closes: #162
+* Installation improvements - closes: #166
+* Fix issue on Fn mode symlink conversion - partially addresses: #160
 
 ## udocker (1.1.2)
 
-* Improve parsing of quotes in the command line
-  * closes: #98
-* Fix version command to exit with 0
-  * closes: #107
+* Improve parsing of quotes in the command line - closes: #98
+* Fix version command to exit with 0 - closes: #107
 * Add kill-on-exit to proot on Pn modes
 * Improve download of udocker utils
-* Handle authentication headers when pulling
-  * closes: #110
+* Handle authentication headers when pulling - closes: #110
 * Handle of redirects when pulling
 * Fix registries table
 * Support search quay.io
 * Fix auth header when no standard Docker registry is used
 * Add registry detection on image name
 * Add --version option
-* Force python2 as interpreter
-  * closes: #131
+* Force python2 as interpreter - closes: #131
 * Fix handling of volumes in metadata
 * Handle empty metadata
-* Fix http proxy functionality
-  * closes: #115
-* Ignore --no-trunc and --all in the images command
-  * closes: #108
+* Fix http proxy functionality - closes: #115
+* Ignore --no-trunc and --all in the images command - closes: #108
 * Implement verification of layers in manifest
 * Add --nvidia to support GPUs and related drivers
 * Send download messages to stderr
 * Enable override of curl executable
-* Fix building on CentOS 6
-  * closes: #157
-* Mitigation for upstream limitation in runC without tty
-  * closes: #132
-* Fix detection of executable with symlinks in container
-  * closes: #118
+* Fix building on CentOS 6 - closes: #157
+* Mitigation for upstream limitation in runC without tty - closes: #132
+* Fix detection of executable with symlinks in container - closes: #118
 * Updated runC to v1.0.0-rc5
 * Experimental support for Alpine in Fn modes
-* Improve pathname translation in Fn modes for mounted dirs
-  * partially addresses: #160
+* Improve pathname translation in Fn modes for mounted dirs - partially addresses: #160
 
 ## udocker (1.1.1)
 
 * New execution engine using singularity
 * Updated documentation with OpenMPI information and examples
 * Additional unit tests
 * Redirect messages to stderr
-* Improved parsing of quotes in the command line
-  * closes: #87
+* Improved parsing of quotes in the command line - closes: #87
 * Allow override of the HOME environment variable
 * Allow override of libfakechroot.so at the container level
 * Automatic selection of libfakechroot.so from container info
 * Improve automatic install
 * Enable resetting prefix paths in Fn modes in remote hosts
 * Do not set `AF_UNIX_PATH` in Fn modes when the host /tmp is a volume
 * Export containers in both docker and udocker format
 * Import containers docker and udocker format
 * Load, import and export to/from stdin/stdout
 * Clone existing containers
 * Support for TCP/IP port remap in execution modes Pn
-* Fix run with basenames failing
-  * closes: #89
-* Allow run as root flag
-  * closes: #91
+* Fix run with basenames failing - closes: #89
+* Allow run as root flag - closes: #91
 
 ## udocker (1.1.0)
 
 * Support image names prefixed by registry similarly to docker
 * Add execution engine selection logic
 * Add fr execution engine based on shared library interception
 * Add rc execution engine based on rootless namespaces
 * Improve proot tmp files cleanup on non ext filesystems
 * Improve search returning empty on Docker repositories
 * Improve runC execution portability
-* Add environment variable `UDOCKER_KEYSTORE`
-  * closes: #75
-* Prevent creation of .udocker when `UDOCKER_KEYSTORE` is used
-  * closes: #75
+* Add environment variable `UDOCKER_KEYSTORE` - closes: #75
+* Prevent creation of .udocker when `UDOCKER_KEYSTORE` is used - closes: #75
 
 ## udocker (1.0.4)
 
 * Documentation fixes
 
 ## udocker (1.0.3)
 
 * Support for import Docker containers in newer metadata structure
 * Improve the command line parsing
 * Improve temporary file handling and removal
 * Support for additional execution engines to be provided in the future
-* Improved parsing of entrypoint and cmd metadata
-  * closes: #53
-* Increase name alias length
-  * closes: #52
-* Add support for change dir into volume directories
-  * closes: #51
-* Fix deletion of files upon container import
-  * closes: #50
-* Fix exporting of host environment variables to the containers
-  * closes: #48
-* Change misleading behavior of import tarball from move to copy
-  * closes: #44
-* Fix validation of volumes specification
-  * closes: #43
+* Improved parsing of entrypoint and cmd metadata - closes: #53
+* Increase name alias length - closes: #52
+* Add support for change dir into volume directories - closes: #51
+* Fix deletion of files upon container import - closes: #50
+* Fix exporting of host environment variables to the containers - closes: #48
+* Change misleading behavior of import tarball from move to copy - closes: #44
+* Fix validation of volumes specification - closes: #43
 
 ## udocker (1.0.2)
 
 * Improve download on repositories that fail authentication on /v2
 * Improve run verification of binaries with recursive symbolic links
-* Improve accelerated seccomp on kernels >= 4.8.0
-  * closes: #40
+* Improve accelerated seccomp on kernels >= 4.8.0 - closes: #40
 
 ## udocker (1.0.1)
 
 * Minor bugfixes
 * Executable name changed from udocker.py to udocker
 * Added support for login into docker repositories
 * Added support for private repositories
 * Added support for listing of v2 repositories catalog
 * Added checksum verification for sha256 layers
 * Improved download handling for v1 and v2 repositories
 * Improved installation tarball structure
 * Insecure flag fixed
 * Address seccomp change introduced on kernels >= 4.8.0
 * Utilities for packaging
-* Improved verbose levels, messaging and output
-  * closes: #24, #23
-* Fully implement support for registry selection --registry parameter
-  * closes: #29
-* Provide support for private repositories e.g. gitlab registries
-  * closes: #30
-* Provide --insecure command line parameter for SSL requests
-  * closes: #31
+* Improved verbose levels, messaging and output - closes: #24, #23
+* Fully implement support for registry selection --registry parameter - closes: #29
+* Provide support for private repositories e.g. gitlab registries - closes: #30
+* Provide --insecure command line parameter for SSL requests - closes: #31
 
 ## udocker (1.0.0)
 
 * Initial version
-
-
```

### Comparing `udocker-1.3.8/udocker.egg-info/SOURCES.txt` & `udocker-1.3.9/udocker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

