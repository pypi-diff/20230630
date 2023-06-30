# Comparing `tmp/hgitaly-0.8.1.tar.gz` & `tmp/hgitaly-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgitaly-0.8.1.tar", last modified: Sun Mar  7 20:39:57 2021, max compression
+gzip compressed data, was "hgitaly-0.9.0.tar", last modified: Thu Feb 25 23:28:35 2021, max compression
```

## Comparing `hgitaly-0.8.1.tar` & `hgitaly-0.9.0.tar`

### file list

```diff
@@ -1,77 +1,82 @@
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.987734 hgitaly-0.8.1/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2021-02-13 21:52:08.000000 hgitaly-0.8.1/MANIFEST.in
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8638 2021-03-07 20:39:57.987734 hgitaly-0.8.1/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6815 2021-02-13 21:52:08.000000 hgitaly-0.8.1/README.md
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.961733 hgitaly-0.8.1/hgext3rd/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgext3rd/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.961733 hgitaly-0.8.1/hgext3rd/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2931 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgext3rd/hgitaly/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.962734 hgitaly-0.8.1/hgext3rd/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgext3rd/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4334 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgext3rd/hgitaly/tests/test_serve.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.965734 hgitaly-0.8.1/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6802 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2703 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3645 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/message.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/path.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2042 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9238 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/server.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.968734 hgitaly-0.8.1/hgitaly/service/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26456 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1983 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18184 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5910 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/repository_service.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.969734 hgitaly-0.8.1/hgitaly/service/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24380 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/tests/test_commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1726 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/tests/test_default_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14846 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/tests/test_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/service/tests/test_repository_service.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2950 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1401 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stream.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.982734 hgitaly-0.8.1/hgitaly/stub/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32947 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/blob_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8719 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/blob_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   132023 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/commit_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    34185 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/commit_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    39307 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/diff_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8414 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/diff_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9188 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/lint_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/lint_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    93239 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/ref_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29037 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/ref_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   177974 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/repository_service_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    71159 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/repository_service_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29241 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/shared_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/stub/shared_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      449 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tag.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.985734 hgitaly-0.8.1/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3711 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tests/common.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4452 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tests/test_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      814 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tests/test_errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1530 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tests/test_messages.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1510 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tests/test_revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8672 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tests/test_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2847 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tests/test_servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      454 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/tests/test_stream.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1060 2021-02-13 21:52:08.000000 hgitaly-0.8.1/hgitaly/util.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.966734 hgitaly-0.8.1/hgitaly.egg-info/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8638 2021-03-07 20:39:57.000000 hgitaly-0.8.1/hgitaly.egg-info/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1760 2021-03-07 20:39:57.000000 hgitaly-0.8.1/hgitaly.egg-info/SOURCES.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2021-03-07 20:39:57.000000 hgitaly-0.8.1/hgitaly.egg-info/dependency_links.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       58 2021-03-07 20:39:57.000000 hgitaly-0.8.1/hgitaly.egg-info/requires.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2021-03-07 20:39:57.000000 hgitaly-0.8.1/hgitaly.egg-info/top_level.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       58 2021-02-13 21:52:08.000000 hgitaly-0.8.1/install-requirements.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2021-03-07 20:39:57.987734 hgitaly-0.8.1/setup.cfg
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      652 2021-03-07 20:39:48.000000 hgitaly-0.8.1/setup.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-03-07 20:39:57.987734 hgitaly-0.8.1/tests_with_gitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1655 2021-02-13 21:52:08.000000 hgitaly-0.8.1/tests_with_gitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2390 2021-02-13 21:52:08.000000 hgitaly-0.8.1/tests_with_gitaly/comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2024 2021-02-13 21:52:08.000000 hgitaly-0.8.1/tests_with_gitaly/conftest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2996 2021-02-13 21:52:08.000000 hgitaly-0.8.1/tests_with_gitaly/gitaly.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1385 2021-02-13 21:52:08.000000 hgitaly-0.8.1/tests_with_gitaly/test_gitaly_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5217 2021-02-13 21:52:08.000000 hgitaly-0.8.1/tests_with_gitaly/test_ref.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.907982 hgitaly-0.9.0/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2020-12-03 15:26:18.000000 hgitaly-0.9.0/MANIFEST.in
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8638 2021-02-25 23:28:35.907982 hgitaly-0.9.0/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6815 2021-01-10 11:37:54.000000 hgitaly-0.9.0/README.md
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.885982 hgitaly-0.9.0/hgext3rd/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2020-11-15 11:35:39.000000 hgitaly-0.9.0/hgext3rd/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.885982 hgitaly-0.9.0/hgext3rd/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2931 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgext3rd/hgitaly/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.887982 hgitaly-0.9.0/hgext3rd/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgext3rd/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4334 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgext3rd/hgitaly/tests/test_serve.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.889982 hgitaly-0.9.0/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2020-11-15 11:35:39.000000 hgitaly-0.9.0/hgitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6802 2021-02-13 20:13:56.000000 hgitaly-0.9.0/hgitaly/branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3042 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      838 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3645 2020-11-15 11:35:39.000000 hgitaly-0.9.0/hgitaly/message.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1083 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/path.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2042 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9238 2021-02-13 20:13:56.000000 hgitaly-0.9.0/hgitaly/server.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.891982 hgitaly-0.9.0/hgitaly/service/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2020-11-15 11:35:39.000000 hgitaly-0.9.0/hgitaly/service/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26456 2021-02-13 20:13:53.000000 hgitaly-0.9.0/hgitaly/service/commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6014 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/service/diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18184 2021-02-13 20:13:56.000000 hgitaly-0.9.0/hgitaly/service/ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5910 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/service/repository_service.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.893982 hgitaly-0.9.0/hgitaly/service/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2020-11-15 11:35:39.000000 hgitaly-0.9.0/hgitaly/service/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24380 2021-02-13 20:13:56.000000 hgitaly-0.9.0/hgitaly/service/tests/test_commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1726 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/service/tests/test_default_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3077 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/service/tests/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14846 2021-02-13 20:13:56.000000 hgitaly-0.9.0/hgitaly/service/tests/test_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/service/tests/test_repository_service.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2950 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1895 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/stream.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.900982 hgitaly-0.9.0/hgitaly/stub/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2020-11-15 11:35:39.000000 hgitaly-0.9.0/hgitaly/stub/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32947 2020-12-06 15:01:35.000000 hgitaly-0.9.0/hgitaly/stub/blob_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8719 2020-12-06 15:01:35.000000 hgitaly-0.9.0/hgitaly/stub/blob_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   132936 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/stub/commit_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    34185 2020-12-06 15:01:35.000000 hgitaly-0.9.0/hgitaly/stub/commit_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    46617 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/stub/diff_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10012 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/stub/diff_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9018 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/stub/lint_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2020-12-06 15:01:35.000000 hgitaly-0.9.0/hgitaly/stub/lint_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    93239 2020-12-06 15:01:36.000000 hgitaly-0.9.0/hgitaly/stub/ref_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29110 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/stub/ref_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   178930 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/stub/repository_service_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    71270 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/stub/repository_service_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    31453 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/stub/shared_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2020-12-06 15:01:35.000000 hgitaly-0.9.0/hgitaly/stub/shared_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      449 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/tag.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.905982 hgitaly-0.9.0/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2020-11-15 11:35:39.000000 hgitaly-0.9.0/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3711 2021-02-13 20:13:56.000000 hgitaly-0.9.0/hgitaly/tests/common.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4452 2021-02-13 20:13:56.000000 hgitaly-0.9.0/hgitaly/tests/test_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      814 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/tests/test_errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1530 2020-11-15 11:35:39.000000 hgitaly-0.9.0/hgitaly/tests/test_messages.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      689 2021-02-25 23:13:21.000000 hgitaly-0.9.0/hgitaly/tests/test_oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1510 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/tests/test_revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8672 2021-01-10 11:37:54.000000 hgitaly-0.9.0/hgitaly/tests/test_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2847 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/tests/test_servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      454 2020-12-03 15:26:18.000000 hgitaly-0.9.0/hgitaly/tests/test_stream.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1060 2020-11-15 11:35:39.000000 hgitaly-0.9.0/hgitaly/util.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.890982 hgitaly-0.9.0/hgitaly.egg-info/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8638 2021-02-25 23:28:35.000000 hgitaly-0.9.0/hgitaly.egg-info/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1882 2021-02-25 23:28:35.000000 hgitaly-0.9.0/hgitaly.egg-info/SOURCES.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2021-02-25 23:28:35.000000 hgitaly-0.9.0/hgitaly.egg-info/dependency_links.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       58 2021-02-25 23:28:35.000000 hgitaly-0.9.0/hgitaly.egg-info/requires.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2021-02-25 23:28:35.000000 hgitaly-0.9.0/hgitaly.egg-info/top_level.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       58 2021-02-13 20:13:56.000000 hgitaly-0.9.0/install-requirements.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2021-02-25 23:28:35.907982 hgitaly-0.9.0/setup.cfg
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      652 2021-02-25 23:13:31.000000 hgitaly-0.9.0/setup.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-02-25 23:28:35.906982 hgitaly-0.9.0/tests_with_gitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2153 2021-02-25 23:13:21.000000 hgitaly-0.9.0/tests_with_gitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2390 2021-01-10 11:37:54.000000 hgitaly-0.9.0/tests_with_gitaly/comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2024 2021-01-10 11:37:54.000000 hgitaly-0.9.0/tests_with_gitaly/conftest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3119 2021-02-25 23:13:21.000000 hgitaly-0.9.0/tests_with_gitaly/gitaly.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4771 2021-02-25 23:13:21.000000 hgitaly-0.9.0/tests_with_gitaly/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1385 2021-01-10 11:37:54.000000 hgitaly-0.9.0/tests_with_gitaly/test_gitaly_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4881 2021-02-25 23:13:21.000000 hgitaly-0.9.0/tests_with_gitaly/test_ref.py
```

### Comparing `hgitaly-0.8.1/PKG-INFO` & `hgitaly-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgitaly
-Version: 0.8.1
+Version: 0.9.0
 Summary: Server-side implementation of Gitaly protocol for Mercurial
 Home-page: https://foss.heptapod.net/heptapod/hgitaly
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Description: # HGitaly
```

### Comparing `hgitaly-0.8.1/README.md` & `hgitaly-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgext3rd/hgitaly/__init__.py` & `hgitaly-0.9.0/hgext3rd/hgitaly/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgext3rd/hgitaly/tests/test_serve.py` & `hgitaly-0.9.0/hgext3rd/hgitaly/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/branch.py` & `hgitaly-0.9.0/hgitaly/branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/errors.py` & `hgitaly-0.9.0/hgitaly/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,7 +62,18 @@
 
     Similar to :func:`not_found`, except for the default ``log_level``
     """
     context.set_code(StatusCode.INTERNAL)
     logger.log(log_level, message)
     context.set_details(message)
     return response_cls()
+
+
+def unknown_error(context, response_cls, message, log_level=logging.ERROR):
+    """Return grpc UNKNOWN code with message.
+
+    Similar to :func:`not_found`, except for the default ``log_level``
+    """
+    context.set_code(StatusCode.UNKNOWN)
+    logger.log(log_level, message)
+    context.set_details(message)
+    return response_cls()
```

### Comparing `hgitaly-0.8.1/hgitaly/message.py` & `hgitaly-0.9.0/hgitaly/message.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/path.py` & `hgitaly-0.9.0/hgitaly/path.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/revision.py` & `hgitaly-0.9.0/hgitaly/revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/server.py` & `hgitaly-0.9.0/hgitaly/server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/service/commit.py` & `hgitaly-0.9.0/hgitaly/service/commit.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/service/ref.py` & `hgitaly-0.9.0/hgitaly/service/ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/service/repository_service.py` & `hgitaly-0.9.0/hgitaly/service/repository_service.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/service/tests/test_commit.py` & `hgitaly-0.9.0/hgitaly/service/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/service/tests/test_default_branch.py` & `hgitaly-0.9.0/hgitaly/service/tests/test_default_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/service/tests/test_ref.py` & `hgitaly-0.9.0/hgitaly/service/tests/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/service/tests/test_repository_service.py` & `hgitaly-0.9.0/hgitaly/service/tests/test_repository_service.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/servicer.py` & `hgitaly-0.9.0/hgitaly/servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/stream.py` & `hgitaly-0.9.0/hgitaly/stream.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,14 +20,30 @@
 #     the string's prefix: 2 for "0b", 8 for "0" or "0o", 16 for "0x",
 #     and 10 otherwise. Also, for argument base 0 only,
 #     underscore characters are permitted as defined by the
 #     Go syntax for integer literals.
 import os
 
 
+def concat_resplit(in_chunks, out_chunks_size):
+    """Generator that aggregate incoming chunks of bytes and yield chunks with
+    the wished size.
+
+    in_chunks: an iterator of chunk of bytes of arbitrary sizes
+    out_chunks_size: size of chunks to be yield, except last one
+    """
+    data = b''
+    for chunk in in_chunks:
+        data += chunk
+        while len(data) > out_chunks_size:
+            yield data[:out_chunks_size]
+            data = data[out_chunks_size:]
+    yield data
+
+
 def parse_int(s):
     """Parse integer string representations, as Golangs `strconf.ParseInt`
 
     # TODO check at least octal and hex syntaxes
     >>> parse_int('10')
     10
     """
```

### Comparing `hgitaly-0.8.1/hgitaly/stub/blob_pb2.py` & `hgitaly-0.9.0/hgitaly/stub/blob_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/stub/blob_pb2_grpc.py` & `hgitaly-0.9.0/hgitaly/stub/blob_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/stub/commit_pb2.py` & `hgitaly-0.9.0/hgitaly/stub/commit_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='commit.proto',
   package='gitaly',
   syntax='proto3',
   serialized_options=b'Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypb',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0c\x63ommit.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"T\n\x12\x43ommitStatsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"H\n\x13\x43ommitStatsResponse\x12\x0b\n\x03oid\x18\x01 \x01(\t\x12\x11\n\tadditions\x18\x02 \x01(\x05\x12\x11\n\tdeletions\x18\x03 \x01(\x05\"n\n\x17\x43ommitIsAncestorRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x61ncestor_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hild_id\x18\x03 \x01(\t\")\n\x18\x43ommitIsAncestorResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x81\x01\n\x10TreeEntryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12\r\n\x05limit\x18\x04 \x01(\x03\x12\x10\n\x08max_size\x18\x05 \x01(\x03\"\xb5\x01\n\x11TreeEntryResponse\x12\x32\n\x04type\x18\x01 \x01(\x0e\x32$.gitaly.TreeEntryResponse.ObjectType\x12\x0b\n\x03oid\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\x03\x12\x0c\n\x04mode\x18\x04 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"5\n\nObjectType\x12\n\n\x06\x43OMMIT\x10\x00\x12\x08\n\x04\x42LOB\x10\x01\x12\x08\n\x04TREE\x10\x02\x12\x07\n\x03TAG\x10\x03\"_\n\x15\x43ommitsBetweenRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x66rom\x18\x02 \x01(\x0c\x12\n\n\x02to\x18\x03 \x01(\x0c\"<\n\x16\x43ommitsBetweenResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"\x9f\x02\n\x13\x43ountCommitsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12)\n\x05\x61\x66ter\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x62\x65\x66ore\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04path\x18\x05 \x01(\x0c\x12\x11\n\tmax_count\x18\x06 \x01(\x05\x12\x0b\n\x03\x61ll\x18\x07 \x01(\x08\x12\x14\n\x0c\x66irst_parent\x18\x08 \x01(\x08\x12-\n\x0eglobal_options\x18\t \x01(\x0b\x32\x15.gitaly.GlobalOptions\"%\n\x14\x43ountCommitsResponse\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\"\x8b\x01\n\x1c\x43ountDivergingCommitsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x66rom\x18\x02 \x01(\x0c\x12\n\n\x02to\x18\x03 \x01(\x0c\x12\x11\n\tmax_count\x18\x07 \x01(\x05J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"H\n\x1d\x43ountDivergingCommitsResponse\x12\x12\n\nleft_count\x18\x01 \x01(\x05\x12\x13\n\x0bright_count\x18\x02 \x01(\x05\"\xc5\x01\n\tTreeEntry\x12\x0b\n\x03oid\x18\x01 \x01(\t\x12\x10\n\x08root_oid\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12)\n\x04type\x18\x04 \x01(\x0e\x32\x1b.gitaly.TreeEntry.EntryType\x12\x0c\n\x04mode\x18\x05 \x01(\x05\x12\x12\n\ncommit_oid\x18\x06 \x01(\t\x12\x11\n\tflat_path\x18\x07 \x01(\x0c\"+\n\tEntryType\x12\x08\n\x04\x42LOB\x10\x00\x12\x08\n\x04TREE\x10\x01\x12\n\n\x06\x43OMMIT\x10\x03\"x\n\x15GetTreeEntriesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12\x11\n\trecursive\x18\x04 \x01(\x08\"<\n\x16GetTreeEntriesResponse\x12\"\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x11.gitaly.TreeEntry\"R\n\x10ListFilesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"\"\n\x11ListFilesResponse\x12\r\n\x05paths\x18\x01 \x03(\x0c\"S\n\x11\x46indCommitRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"7\n\x12\x46indCommitResponse\x12!\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x11.gitaly.GitCommit\"T\n\x17ListCommitsByOidRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03oid\x18\x02 \x03(\t\">\n\x18ListCommitsByOidResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"^\n\x1bListCommitsByRefNameRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tref_names\x18\x02 \x03(\x0c\"\xb1\x01\n\x1cListCommitsByRefNameResponse\x12\x46\n\x0b\x63ommit_refs\x18\x02 \x03(\x0b\x32\x31.gitaly.ListCommitsByRefNameResponse.CommitForRef\x1a\x43\n\x0c\x43ommitForRef\x12!\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x10\n\x08ref_name\x18\x02 \x01(\x0cJ\x04\x08\x01\x10\x02\"\xd3\x01\n\x15\x46indAllCommitsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x11\n\tmax_count\x18\x03 \x01(\x05\x12\x0c\n\x04skip\x18\x04 \x01(\x05\x12\x32\n\x05order\x18\x05 \x01(\x0e\x32#.gitaly.FindAllCommitsRequest.Order\"%\n\x05Order\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04TOPO\x10\x01\x12\x08\n\x04\x44\x41TE\x10\x02\"<\n\x16\x46indAllCommitsResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"\xc4\x03\n\x12\x46indCommitsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\r\n\x05limit\x18\x03 \x01(\x05\x12\x0e\n\x06offset\x18\x04 \x01(\x05\x12\r\n\x05paths\x18\x05 \x03(\x0c\x12\x0e\n\x06\x66ollow\x18\x06 \x01(\x08\x12\x13\n\x0bskip_merges\x18\x07 \x01(\x08\x12\x14\n\x0c\x64isable_walk\x18\x08 \x01(\x08\x12)\n\x05\x61\x66ter\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x62\x65\x66ore\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03\x61ll\x18\x0b \x01(\x08\x12\x14\n\x0c\x66irst_parent\x18\x0c \x01(\x08\x12\x0e\n\x06\x61uthor\x18\r \x01(\x0c\x12/\n\x05order\x18\x0e \x01(\x0e\x32 .gitaly.FindCommitsRequest.Order\x12-\n\x0eglobal_options\x18\x0f \x01(\x0b\x32\x15.gitaly.GlobalOptions\"\x1b\n\x05Order\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04TOPO\x10\x01\"9\n\x13\x46indCommitsResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"X\n\x16\x43ommitLanguagesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"\xb1\x01\n\x17\x43ommitLanguagesResponse\x12;\n\tlanguages\x18\x01 \x03(\x0b\x32(.gitaly.CommitLanguagesResponse.Language\x1aY\n\x08Language\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05share\x18\x02 \x01(\x02\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x12\n\nfile_count\x18\x04 \x01(\r\x12\r\n\x05\x62ytes\x18\x05 \x01(\x04\"_\n\x0fRawBlameRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0c\n\x04path\x18\x03 \x01(\x0c\" \n\x10RawBlameResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\xb1\x01\n\x18LastCommitForPathRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12\x18\n\x10literal_pathspec\x18\x04 \x01(\x08\x12-\n\x0eglobal_options\x18\x05 \x01(\x0b\x32\x15.gitaly.GlobalOptions\">\n\x19LastCommitForPathResponse\x12!\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x11.gitaly.GitCommit\"\xd9\x01\n\x1dListLastCommitsForTreeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12\r\n\x05limit\x18\x04 \x01(\x05\x12\x0e\n\x06offset\x18\x05 \x01(\x05\x12\x1c\n\x10literal_pathspec\x18\x06 \x01(\x08\x42\x02\x18\x01\x12-\n\x0eglobal_options\x18\x07 \x01(\x0b\x32\x15.gitaly.GlobalOptions\"\xbb\x01\n\x1eListLastCommitsForTreeResponse\x12\x45\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x34.gitaly.ListLastCommitsForTreeResponse.CommitForTree\x1aR\n\rCommitForTree\x12!\n\x06\x63ommit\x18\x02 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x12\n\npath_bytes\x18\x04 \x01(\x0cJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04\"\xc4\x01\n\x17\x43ommitsByMessageRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0e\n\x06offset\x18\x03 \x01(\x05\x12\r\n\x05limit\x18\x04 \x01(\x05\x12\x0c\n\x04path\x18\x05 \x01(\x0c\x12\r\n\x05query\x18\x06 \x01(\t\x12-\n\x0eglobal_options\x18\x07 \x01(\x0b\x32\x15.gitaly.GlobalOptions\">\n\x18\x43ommitsByMessageResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"]\n\x1f\x46ilterShasWithSignaturesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04shas\x18\x02 \x03(\x0c\"0\n FilterShasWithSignaturesResponse\x12\x0c\n\x04shas\x18\x01 \x03(\x0c\"`\n\x1d\x45xtractCommitSignatureRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tcommit_id\x18\x02 \x01(\t\"H\n\x1e\x45xtractCommitSignatureResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\x13\n\x0bsigned_text\x18\x02 \x01(\x0c\"^\n\x1aGetCommitSignaturesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x12\n\ncommit_ids\x18\x02 \x03(\t\"X\n\x1bGetCommitSignaturesResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x11\n\tsignature\x18\x02 \x01(\x0c\x12\x13\n\x0bsigned_text\x18\x03 \x01(\x0c\"\\\n\x18GetCommitMessagesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x12\n\ncommit_ids\x18\x02 \x03(\t\"?\n\x19GetCommitMessagesResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\x0c\x32\xb9\x0f\n\rCommitService\x12]\n\x10\x43ommitIsAncestor\x12\x1f.gitaly.CommitIsAncestorRequest\x1a .gitaly.CommitIsAncestorResponse\"\x06\xfa\x97(\x02\x08\x02\x12J\n\tTreeEntry\x12\x18.gitaly.TreeEntryRequest\x1a\x19.gitaly.TreeEntryResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12Y\n\x0e\x43ommitsBetween\x12\x1d.gitaly.CommitsBetweenRequest\x1a\x1e.gitaly.CommitsBetweenResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12Q\n\x0c\x43ountCommits\x12\x1b.gitaly.CountCommitsRequest\x1a\x1c.gitaly.CountCommitsResponse\"\x06\xfa\x97(\x02\x08\x02\x12l\n\x15\x43ountDivergingCommits\x12$.gitaly.CountDivergingCommitsRequest\x1a%.gitaly.CountDivergingCommitsResponse\"\x06\xfa\x97(\x02\x08\x02\x12Y\n\x0eGetTreeEntries\x12\x1d.gitaly.GetTreeEntriesRequest\x1a\x1e.gitaly.GetTreeEntriesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tListFiles\x12\x18.gitaly.ListFilesRequest\x1a\x19.gitaly.ListFilesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12K\n\nFindCommit\x12\x19.gitaly.FindCommitRequest\x1a\x1a.gitaly.FindCommitResponse\"\x06\xfa\x97(\x02\x08\x02\x12N\n\x0b\x43ommitStats\x12\x1a.gitaly.CommitStatsRequest\x1a\x1b.gitaly.CommitStatsResponse\"\x06\xfa\x97(\x02\x08\x02\x12Y\n\x0e\x46indAllCommits\x12\x1d.gitaly.FindAllCommitsRequest\x1a\x1e.gitaly.FindAllCommitsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12P\n\x0b\x46indCommits\x12\x1a.gitaly.FindCommitsRequest\x1a\x1b.gitaly.FindCommitsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12Z\n\x0f\x43ommitLanguages\x12\x1e.gitaly.CommitLanguagesRequest\x1a\x1f.gitaly.CommitLanguagesResponse\"\x06\xfa\x97(\x02\x08\x02\x12G\n\x08RawBlame\x12\x17.gitaly.RawBlameRequest\x1a\x18.gitaly.RawBlameResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12`\n\x11LastCommitForPath\x12 .gitaly.LastCommitForPathRequest\x1a!.gitaly.LastCommitForPathResponse\"\x06\xfa\x97(\x02\x08\x02\x12q\n\x16ListLastCommitsForTree\x12%.gitaly.ListLastCommitsForTreeRequest\x1a&.gitaly.ListLastCommitsForTreeResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12_\n\x10\x43ommitsByMessage\x12\x1f.gitaly.CommitsByMessageRequest\x1a .gitaly.CommitsByMessageResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12_\n\x10ListCommitsByOid\x12\x1f.gitaly.ListCommitsByOidRequest\x1a .gitaly.ListCommitsByOidResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12k\n\x14ListCommitsByRefName\x12#.gitaly.ListCommitsByRefNameRequest\x1a$.gitaly.ListCommitsByRefNameResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12y\n\x18\x46ilterShasWithSignatures\x12\'.gitaly.FilterShasWithSignaturesRequest\x1a(.gitaly.FilterShasWithSignaturesResponse\"\x06\xfa\x97(\x02\x08\x02(\x01\x30\x01\x12h\n\x13GetCommitSignatures\x12\".gitaly.GetCommitSignaturesRequest\x1a#.gitaly.GetCommitSignaturesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x62\n\x11GetCommitMessages\x12 .gitaly.GetCommitMessagesRequest\x1a!.gitaly.GetCommitMessagesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
+  serialized_pb=b'\n\x0c\x63ommit.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"T\n\x12\x43ommitStatsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"H\n\x13\x43ommitStatsResponse\x12\x0b\n\x03oid\x18\x01 \x01(\t\x12\x11\n\tadditions\x18\x02 \x01(\x05\x12\x11\n\tdeletions\x18\x03 \x01(\x05\"n\n\x17\x43ommitIsAncestorRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x61ncestor_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hild_id\x18\x03 \x01(\t\")\n\x18\x43ommitIsAncestorResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x81\x01\n\x10TreeEntryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12\r\n\x05limit\x18\x04 \x01(\x03\x12\x10\n\x08max_size\x18\x05 \x01(\x03\"\xb5\x01\n\x11TreeEntryResponse\x12\x32\n\x04type\x18\x01 \x01(\x0e\x32$.gitaly.TreeEntryResponse.ObjectType\x12\x0b\n\x03oid\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\x03\x12\x0c\n\x04mode\x18\x04 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"5\n\nObjectType\x12\n\n\x06\x43OMMIT\x10\x00\x12\x08\n\x04\x42LOB\x10\x01\x12\x08\n\x04TREE\x10\x02\x12\x07\n\x03TAG\x10\x03\"_\n\x15\x43ommitsBetweenRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x66rom\x18\x02 \x01(\x0c\x12\n\n\x02to\x18\x03 \x01(\x0c\"<\n\x16\x43ommitsBetweenResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"\x9f\x02\n\x13\x43ountCommitsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12)\n\x05\x61\x66ter\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x62\x65\x66ore\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04path\x18\x05 \x01(\x0c\x12\x11\n\tmax_count\x18\x06 \x01(\x05\x12\x0b\n\x03\x61ll\x18\x07 \x01(\x08\x12\x14\n\x0c\x66irst_parent\x18\x08 \x01(\x08\x12-\n\x0eglobal_options\x18\t \x01(\x0b\x32\x15.gitaly.GlobalOptions\"%\n\x14\x43ountCommitsResponse\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\"\x8b\x01\n\x1c\x43ountDivergingCommitsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x66rom\x18\x02 \x01(\x0c\x12\n\n\x02to\x18\x03 \x01(\x0c\x12\x11\n\tmax_count\x18\x07 \x01(\x05J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"H\n\x1d\x43ountDivergingCommitsResponse\x12\x12\n\nleft_count\x18\x01 \x01(\x05\x12\x13\n\x0bright_count\x18\x02 \x01(\x05\"\xc5\x01\n\tTreeEntry\x12\x0b\n\x03oid\x18\x01 \x01(\t\x12\x10\n\x08root_oid\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12)\n\x04type\x18\x04 \x01(\x0e\x32\x1b.gitaly.TreeEntry.EntryType\x12\x0c\n\x04mode\x18\x05 \x01(\x05\x12\x12\n\ncommit_oid\x18\x06 \x01(\t\x12\x11\n\tflat_path\x18\x07 \x01(\x0c\"+\n\tEntryType\x12\x08\n\x04\x42LOB\x10\x00\x12\x08\n\x04TREE\x10\x01\x12\n\n\x06\x43OMMIT\x10\x03\"x\n\x15GetTreeEntriesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12\x11\n\trecursive\x18\x04 \x01(\x08\"<\n\x16GetTreeEntriesResponse\x12\"\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x11.gitaly.TreeEntry\"R\n\x10ListFilesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"\"\n\x11ListFilesResponse\x12\r\n\x05paths\x18\x01 \x03(\x0c\"e\n\x11\x46indCommitRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x10\n\x08trailers\x18\x03 \x01(\x08\"7\n\x12\x46indCommitResponse\x12!\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x11.gitaly.GitCommit\"T\n\x17ListCommitsByOidRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03oid\x18\x02 \x03(\t\">\n\x18ListCommitsByOidResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"^\n\x1bListCommitsByRefNameRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tref_names\x18\x02 \x03(\x0c\"\xb1\x01\n\x1cListCommitsByRefNameResponse\x12\x46\n\x0b\x63ommit_refs\x18\x02 \x03(\x0b\x32\x31.gitaly.ListCommitsByRefNameResponse.CommitForRef\x1a\x43\n\x0c\x43ommitForRef\x12!\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x10\n\x08ref_name\x18\x02 \x01(\x0cJ\x04\x08\x01\x10\x02\"\xd3\x01\n\x15\x46indAllCommitsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x11\n\tmax_count\x18\x03 \x01(\x05\x12\x0c\n\x04skip\x18\x04 \x01(\x05\x12\x32\n\x05order\x18\x05 \x01(\x0e\x32#.gitaly.FindAllCommitsRequest.Order\"%\n\x05Order\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04TOPO\x10\x01\x12\x08\n\x04\x44\x41TE\x10\x02\"<\n\x16\x46indAllCommitsResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"\xd6\x03\n\x12\x46indCommitsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\r\n\x05limit\x18\x03 \x01(\x05\x12\x0e\n\x06offset\x18\x04 \x01(\x05\x12\r\n\x05paths\x18\x05 \x03(\x0c\x12\x0e\n\x06\x66ollow\x18\x06 \x01(\x08\x12\x13\n\x0bskip_merges\x18\x07 \x01(\x08\x12\x14\n\x0c\x64isable_walk\x18\x08 \x01(\x08\x12)\n\x05\x61\x66ter\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x62\x65\x66ore\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03\x61ll\x18\x0b \x01(\x08\x12\x14\n\x0c\x66irst_parent\x18\x0c \x01(\x08\x12\x0e\n\x06\x61uthor\x18\r \x01(\x0c\x12/\n\x05order\x18\x0e \x01(\x0e\x32 .gitaly.FindCommitsRequest.Order\x12-\n\x0eglobal_options\x18\x0f \x01(\x0b\x32\x15.gitaly.GlobalOptions\x12\x10\n\x08trailers\x18\x10 \x01(\x08\"\x1b\n\x05Order\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04TOPO\x10\x01\"9\n\x13\x46indCommitsResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"X\n\x16\x43ommitLanguagesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"\xb1\x01\n\x17\x43ommitLanguagesResponse\x12;\n\tlanguages\x18\x01 \x03(\x0b\x32(.gitaly.CommitLanguagesResponse.Language\x1aY\n\x08Language\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05share\x18\x02 \x01(\x02\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x12\n\nfile_count\x18\x04 \x01(\r\x12\r\n\x05\x62ytes\x18\x05 \x01(\x04\"_\n\x0fRawBlameRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0c\n\x04path\x18\x03 \x01(\x0c\" \n\x10RawBlameResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\xb1\x01\n\x18LastCommitForPathRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12\x18\n\x10literal_pathspec\x18\x04 \x01(\x08\x12-\n\x0eglobal_options\x18\x05 \x01(\x0b\x32\x15.gitaly.GlobalOptions\">\n\x19LastCommitForPathResponse\x12!\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x11.gitaly.GitCommit\"\xd9\x01\n\x1dListLastCommitsForTreeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\x0c\x12\r\n\x05limit\x18\x04 \x01(\x05\x12\x0e\n\x06offset\x18\x05 \x01(\x05\x12\x1c\n\x10literal_pathspec\x18\x06 \x01(\x08\x42\x02\x18\x01\x12-\n\x0eglobal_options\x18\x07 \x01(\x0b\x32\x15.gitaly.GlobalOptions\"\xbb\x01\n\x1eListLastCommitsForTreeResponse\x12\x45\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x34.gitaly.ListLastCommitsForTreeResponse.CommitForTree\x1aR\n\rCommitForTree\x12!\n\x06\x63ommit\x18\x02 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x12\n\npath_bytes\x18\x04 \x01(\x0cJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04\"\xc4\x01\n\x17\x43ommitsByMessageRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x0e\n\x06offset\x18\x03 \x01(\x05\x12\r\n\x05limit\x18\x04 \x01(\x05\x12\x0c\n\x04path\x18\x05 \x01(\x0c\x12\r\n\x05query\x18\x06 \x01(\t\x12-\n\x0eglobal_options\x18\x07 \x01(\x0b\x32\x15.gitaly.GlobalOptions\">\n\x18\x43ommitsByMessageResponse\x12\"\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x11.gitaly.GitCommit\"]\n\x1f\x46ilterShasWithSignaturesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04shas\x18\x02 \x03(\x0c\"0\n FilterShasWithSignaturesResponse\x12\x0c\n\x04shas\x18\x01 \x03(\x0c\"`\n\x1d\x45xtractCommitSignatureRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tcommit_id\x18\x02 \x01(\t\"H\n\x1e\x45xtractCommitSignatureResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\x13\n\x0bsigned_text\x18\x02 \x01(\x0c\"^\n\x1aGetCommitSignaturesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x12\n\ncommit_ids\x18\x02 \x03(\t\"X\n\x1bGetCommitSignaturesResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x11\n\tsignature\x18\x02 \x01(\x0c\x12\x13\n\x0bsigned_text\x18\x03 \x01(\x0c\"\\\n\x18GetCommitMessagesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x12\n\ncommit_ids\x18\x02 \x03(\t\"?\n\x19GetCommitMessagesResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\x0c\x32\xb9\x0f\n\rCommitService\x12]\n\x10\x43ommitIsAncestor\x12\x1f.gitaly.CommitIsAncestorRequest\x1a .gitaly.CommitIsAncestorResponse\"\x06\xfa\x97(\x02\x08\x02\x12J\n\tTreeEntry\x12\x18.gitaly.TreeEntryRequest\x1a\x19.gitaly.TreeEntryResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12Y\n\x0e\x43ommitsBetween\x12\x1d.gitaly.CommitsBetweenRequest\x1a\x1e.gitaly.CommitsBetweenResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12Q\n\x0c\x43ountCommits\x12\x1b.gitaly.CountCommitsRequest\x1a\x1c.gitaly.CountCommitsResponse\"\x06\xfa\x97(\x02\x08\x02\x12l\n\x15\x43ountDivergingCommits\x12$.gitaly.CountDivergingCommitsRequest\x1a%.gitaly.CountDivergingCommitsResponse\"\x06\xfa\x97(\x02\x08\x02\x12Y\n\x0eGetTreeEntries\x12\x1d.gitaly.GetTreeEntriesRequest\x1a\x1e.gitaly.GetTreeEntriesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tListFiles\x12\x18.gitaly.ListFilesRequest\x1a\x19.gitaly.ListFilesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12K\n\nFindCommit\x12\x19.gitaly.FindCommitRequest\x1a\x1a.gitaly.FindCommitResponse\"\x06\xfa\x97(\x02\x08\x02\x12N\n\x0b\x43ommitStats\x12\x1a.gitaly.CommitStatsRequest\x1a\x1b.gitaly.CommitStatsResponse\"\x06\xfa\x97(\x02\x08\x02\x12Y\n\x0e\x46indAllCommits\x12\x1d.gitaly.FindAllCommitsRequest\x1a\x1e.gitaly.FindAllCommitsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12P\n\x0b\x46indCommits\x12\x1a.gitaly.FindCommitsRequest\x1a\x1b.gitaly.FindCommitsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12Z\n\x0f\x43ommitLanguages\x12\x1e.gitaly.CommitLanguagesRequest\x1a\x1f.gitaly.CommitLanguagesResponse\"\x06\xfa\x97(\x02\x08\x02\x12G\n\x08RawBlame\x12\x17.gitaly.RawBlameRequest\x1a\x18.gitaly.RawBlameResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12`\n\x11LastCommitForPath\x12 .gitaly.LastCommitForPathRequest\x1a!.gitaly.LastCommitForPathResponse\"\x06\xfa\x97(\x02\x08\x02\x12q\n\x16ListLastCommitsForTree\x12%.gitaly.ListLastCommitsForTreeRequest\x1a&.gitaly.ListLastCommitsForTreeResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12_\n\x10\x43ommitsByMessage\x12\x1f.gitaly.CommitsByMessageRequest\x1a .gitaly.CommitsByMessageResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12_\n\x10ListCommitsByOid\x12\x1f.gitaly.ListCommitsByOidRequest\x1a .gitaly.ListCommitsByOidResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12k\n\x14ListCommitsByRefName\x12#.gitaly.ListCommitsByRefNameRequest\x1a$.gitaly.ListCommitsByRefNameResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12y\n\x18\x46ilterShasWithSignatures\x12\'.gitaly.FilterShasWithSignaturesRequest\x1a(.gitaly.FilterShasWithSignaturesResponse\"\x06\xfa\x97(\x02\x08\x02(\x01\x30\x01\x12h\n\x13GetCommitSignatures\x12\".gitaly.GetCommitSignaturesRequest\x1a#.gitaly.GetCommitSignaturesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x62\n\x11GetCommitMessages\x12 .gitaly.GetCommitMessagesRequest\x1a!.gitaly.GetCommitMessagesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
   ,
   dependencies=[lint__pb2.DESCRIPTOR,shared__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 
 
 _TREEENTRYRESPONSE_OBJECTTYPE = _descriptor.EnumDescriptor(
   name='ObjectType',
@@ -114,16 +114,16 @@
       name='DATE', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2665,
-  serialized_end=2702,
+  serialized_start=2683,
+  serialized_end=2720,
 )
 _sym_db.RegisterEnumDescriptor(_FINDALLCOMMITSREQUEST_ORDER)
 
 _FINDCOMMITSREQUEST_ORDER = _descriptor.EnumDescriptor(
   name='Order',
   full_name='gitaly.FindCommitsRequest.Order',
   filename=None,
@@ -139,16 +139,16 @@
       name='TOPO', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2665,
-  serialized_end=2692,
+  serialized_start=2683,
+  serialized_end=2710,
 )
 _sym_db.RegisterEnumDescriptor(_FINDCOMMITSREQUEST_ORDER)
 
 
 _COMMITSTATSREQUEST = _descriptor.Descriptor(
   name='CommitStatsRequest',
   full_name='gitaly.CommitStatsRequest',
@@ -972,28 +972,35 @@
     _descriptor.FieldDescriptor(
       name='revision', full_name='gitaly.FindCommitRequest.revision', index=1,
       number=2, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=b"",
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='trailers', full_name='gitaly.FindCommitRequest.trailers', index=2,
+      number=3, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1922,
-  serialized_end=2005,
+  serialized_end=2023,
 )
 
 
 _FINDCOMMITRESPONSE = _descriptor.Descriptor(
   name='FindCommitResponse',
   full_name='gitaly.FindCommitResponse',
   filename=None,
@@ -1016,16 +1023,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2007,
-  serialized_end=2062,
+  serialized_start=2025,
+  serialized_end=2080,
 )
 
 
 _LISTCOMMITSBYOIDREQUEST = _descriptor.Descriptor(
   name='ListCommitsByOidRequest',
   full_name='gitaly.ListCommitsByOidRequest',
   filename=None,
@@ -1055,16 +1062,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2064,
-  serialized_end=2148,
+  serialized_start=2082,
+  serialized_end=2166,
 )
 
 
 _LISTCOMMITSBYOIDRESPONSE = _descriptor.Descriptor(
   name='ListCommitsByOidResponse',
   full_name='gitaly.ListCommitsByOidResponse',
   filename=None,
@@ -1087,16 +1094,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2150,
-  serialized_end=2212,
+  serialized_start=2168,
+  serialized_end=2230,
 )
 
 
 _LISTCOMMITSBYREFNAMEREQUEST = _descriptor.Descriptor(
   name='ListCommitsByRefNameRequest',
   full_name='gitaly.ListCommitsByRefNameRequest',
   filename=None,
@@ -1126,16 +1133,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2214,
-  serialized_end=2308,
+  serialized_start=2232,
+  serialized_end=2326,
 )
 
 
 _LISTCOMMITSBYREFNAMERESPONSE_COMMITFORREF = _descriptor.Descriptor(
   name='CommitForRef',
   full_name='gitaly.ListCommitsByRefNameResponse.CommitForRef',
   filename=None,
@@ -1165,16 +1172,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2415,
-  serialized_end=2482,
+  serialized_start=2433,
+  serialized_end=2500,
 )
 
 _LISTCOMMITSBYREFNAMERESPONSE = _descriptor.Descriptor(
   name='ListCommitsByRefNameResponse',
   full_name='gitaly.ListCommitsByRefNameResponse',
   filename=None,
   file=DESCRIPTOR,
@@ -1196,16 +1203,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2311,
-  serialized_end=2488,
+  serialized_start=2329,
+  serialized_end=2506,
 )
 
 
 _FINDALLCOMMITSREQUEST = _descriptor.Descriptor(
   name='FindAllCommitsRequest',
   full_name='gitaly.FindAllCommitsRequest',
   filename=None,
@@ -1257,16 +1264,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2491,
-  serialized_end=2702,
+  serialized_start=2509,
+  serialized_end=2720,
 )
 
 
 _FINDALLCOMMITSRESPONSE = _descriptor.Descriptor(
   name='FindAllCommitsResponse',
   full_name='gitaly.FindAllCommitsResponse',
   filename=None,
@@ -1289,16 +1296,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2704,
-  serialized_end=2764,
+  serialized_start=2722,
+  serialized_end=2782,
 )
 
 
 _FINDCOMMITSREQUEST = _descriptor.Descriptor(
   name='FindCommitsRequest',
   full_name='gitaly.FindCommitsRequest',
   filename=None,
@@ -1407,29 +1414,36 @@
     _descriptor.FieldDescriptor(
       name='global_options', full_name='gitaly.FindCommitsRequest.global_options', index=14,
       number=15, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='trailers', full_name='gitaly.FindCommitsRequest.trailers', index=15,
+      number=16, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
     _FINDCOMMITSREQUEST_ORDER,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2767,
-  serialized_end=3219,
+  serialized_start=2785,
+  serialized_end=3255,
 )
 
 
 _FINDCOMMITSRESPONSE = _descriptor.Descriptor(
   name='FindCommitsResponse',
   full_name='gitaly.FindCommitsResponse',
   filename=None,
@@ -1452,16 +1466,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3221,
-  serialized_end=3278,
+  serialized_start=3257,
+  serialized_end=3314,
 )
 
 
 _COMMITLANGUAGESREQUEST = _descriptor.Descriptor(
   name='CommitLanguagesRequest',
   full_name='gitaly.CommitLanguagesRequest',
   filename=None,
@@ -1491,16 +1505,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3280,
-  serialized_end=3368,
+  serialized_start=3316,
+  serialized_end=3404,
 )
 
 
 _COMMITLANGUAGESRESPONSE_LANGUAGE = _descriptor.Descriptor(
   name='Language',
   full_name='gitaly.CommitLanguagesResponse.Language',
   filename=None,
@@ -1551,16 +1565,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3459,
-  serialized_end=3548,
+  serialized_start=3495,
+  serialized_end=3584,
 )
 
 _COMMITLANGUAGESRESPONSE = _descriptor.Descriptor(
   name='CommitLanguagesResponse',
   full_name='gitaly.CommitLanguagesResponse',
   filename=None,
   file=DESCRIPTOR,
@@ -1582,16 +1596,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3371,
-  serialized_end=3548,
+  serialized_start=3407,
+  serialized_end=3584,
 )
 
 
 _RAWBLAMEREQUEST = _descriptor.Descriptor(
   name='RawBlameRequest',
   full_name='gitaly.RawBlameRequest',
   filename=None,
@@ -1628,16 +1642,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3550,
-  serialized_end=3645,
+  serialized_start=3586,
+  serialized_end=3681,
 )
 
 
 _RAWBLAMERESPONSE = _descriptor.Descriptor(
   name='RawBlameResponse',
   full_name='gitaly.RawBlameResponse',
   filename=None,
@@ -1660,16 +1674,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3647,
-  serialized_end=3679,
+  serialized_start=3683,
+  serialized_end=3715,
 )
 
 
 _LASTCOMMITFORPATHREQUEST = _descriptor.Descriptor(
   name='LastCommitForPathRequest',
   full_name='gitaly.LastCommitForPathRequest',
   filename=None,
@@ -1720,16 +1734,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3682,
-  serialized_end=3859,
+  serialized_start=3718,
+  serialized_end=3895,
 )
 
 
 _LASTCOMMITFORPATHRESPONSE = _descriptor.Descriptor(
   name='LastCommitForPathResponse',
   full_name='gitaly.LastCommitForPathResponse',
   filename=None,
@@ -1752,16 +1766,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3861,
-  serialized_end=3923,
+  serialized_start=3897,
+  serialized_end=3959,
 )
 
 
 _LISTLASTCOMMITSFORTREEREQUEST = _descriptor.Descriptor(
   name='ListLastCommitsForTreeRequest',
   full_name='gitaly.ListLastCommitsForTreeRequest',
   filename=None,
@@ -1826,16 +1840,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3926,
-  serialized_end=4143,
+  serialized_start=3962,
+  serialized_end=4179,
 )
 
 
 _LISTLASTCOMMITSFORTREERESPONSE_COMMITFORTREE = _descriptor.Descriptor(
   name='CommitForTree',
   full_name='gitaly.ListLastCommitsForTreeResponse.CommitForTree',
   filename=None,
@@ -1865,16 +1879,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4251,
-  serialized_end=4333,
+  serialized_start=4287,
+  serialized_end=4369,
 )
 
 _LISTLASTCOMMITSFORTREERESPONSE = _descriptor.Descriptor(
   name='ListLastCommitsForTreeResponse',
   full_name='gitaly.ListLastCommitsForTreeResponse',
   filename=None,
   file=DESCRIPTOR,
@@ -1896,16 +1910,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4146,
-  serialized_end=4333,
+  serialized_start=4182,
+  serialized_end=4369,
 )
 
 
 _COMMITSBYMESSAGEREQUEST = _descriptor.Descriptor(
   name='CommitsByMessageRequest',
   full_name='gitaly.CommitsByMessageRequest',
   filename=None,
@@ -1970,16 +1984,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4336,
-  serialized_end=4532,
+  serialized_start=4372,
+  serialized_end=4568,
 )
 
 
 _COMMITSBYMESSAGERESPONSE = _descriptor.Descriptor(
   name='CommitsByMessageResponse',
   full_name='gitaly.CommitsByMessageResponse',
   filename=None,
@@ -2002,16 +2016,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4534,
-  serialized_end=4596,
+  serialized_start=4570,
+  serialized_end=4632,
 )
 
 
 _FILTERSHASWITHSIGNATURESREQUEST = _descriptor.Descriptor(
   name='FilterShasWithSignaturesRequest',
   full_name='gitaly.FilterShasWithSignaturesRequest',
   filename=None,
@@ -2041,16 +2055,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4598,
-  serialized_end=4691,
+  serialized_start=4634,
+  serialized_end=4727,
 )
 
 
 _FILTERSHASWITHSIGNATURESRESPONSE = _descriptor.Descriptor(
   name='FilterShasWithSignaturesResponse',
   full_name='gitaly.FilterShasWithSignaturesResponse',
   filename=None,
@@ -2073,16 +2087,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4693,
-  serialized_end=4741,
+  serialized_start=4729,
+  serialized_end=4777,
 )
 
 
 _EXTRACTCOMMITSIGNATUREREQUEST = _descriptor.Descriptor(
   name='ExtractCommitSignatureRequest',
   full_name='gitaly.ExtractCommitSignatureRequest',
   filename=None,
@@ -2112,16 +2126,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4743,
-  serialized_end=4839,
+  serialized_start=4779,
+  serialized_end=4875,
 )
 
 
 _EXTRACTCOMMITSIGNATURERESPONSE = _descriptor.Descriptor(
   name='ExtractCommitSignatureResponse',
   full_name='gitaly.ExtractCommitSignatureResponse',
   filename=None,
@@ -2151,16 +2165,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4841,
-  serialized_end=4913,
+  serialized_start=4877,
+  serialized_end=4949,
 )
 
 
 _GETCOMMITSIGNATURESREQUEST = _descriptor.Descriptor(
   name='GetCommitSignaturesRequest',
   full_name='gitaly.GetCommitSignaturesRequest',
   filename=None,
@@ -2190,16 +2204,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4915,
-  serialized_end=5009,
+  serialized_start=4951,
+  serialized_end=5045,
 )
 
 
 _GETCOMMITSIGNATURESRESPONSE = _descriptor.Descriptor(
   name='GetCommitSignaturesResponse',
   full_name='gitaly.GetCommitSignaturesResponse',
   filename=None,
@@ -2236,16 +2250,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5011,
-  serialized_end=5099,
+  serialized_start=5047,
+  serialized_end=5135,
 )
 
 
 _GETCOMMITMESSAGESREQUEST = _descriptor.Descriptor(
   name='GetCommitMessagesRequest',
   full_name='gitaly.GetCommitMessagesRequest',
   filename=None,
@@ -2275,16 +2289,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5101,
-  serialized_end=5193,
+  serialized_start=5137,
+  serialized_end=5229,
 )
 
 
 _GETCOMMITMESSAGESRESPONSE = _descriptor.Descriptor(
   name='GetCommitMessagesResponse',
   full_name='gitaly.GetCommitMessagesResponse',
   filename=None,
@@ -2314,16 +2328,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5195,
-  serialized_end=5258,
+  serialized_start=5231,
+  serialized_end=5294,
 )
 
 _COMMITSTATSREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _COMMITISANCESTORREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _TREEENTRYREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _TREEENTRYRESPONSE.fields_by_name['type'].enum_type = _TREEENTRYRESPONSE_OBJECTTYPE
 _TREEENTRYRESPONSE_OBJECTTYPE.containing_type = _TREEENTRYRESPONSE
@@ -2792,16 +2806,16 @@
 _COMMITSERVICE = _descriptor.ServiceDescriptor(
   name='CommitService',
   full_name='gitaly.CommitService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=5261,
-  serialized_end=7238,
+  serialized_start=5297,
+  serialized_end=7274,
   methods=[
   _descriptor.MethodDescriptor(
     name='CommitIsAncestor',
     full_name='gitaly.CommitService.CommitIsAncestor',
     index=0,
     containing_service=None,
     input_type=_COMMITISANCESTORREQUEST,
```

### Comparing `hgitaly-0.8.1/hgitaly/stub/commit_pb2_grpc.py` & `hgitaly-0.9.0/hgitaly/stub/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/stub/diff_pb2.py` & `hgitaly-0.9.0/hgitaly/stub/diff_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,60 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='diff.proto',
   package='gitaly',
   syntax='proto3',
   serialized_options=b'Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypb',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\ndiff.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"\xed\x02\n\x11\x43ommitDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\x12 \n\x18ignore_whitespace_change\x18\x04 \x01(\x08\x12\r\n\x05paths\x18\x05 \x03(\x0c\x12\x16\n\x0e\x63ollapse_diffs\x18\x06 \x01(\x08\x12\x16\n\x0e\x65nforce_limits\x18\x07 \x01(\x08\x12\x11\n\tmax_files\x18\x08 \x01(\x05\x12\x11\n\tmax_lines\x18\t \x01(\x05\x12\x11\n\tmax_bytes\x18\n \x01(\x05\x12\x17\n\x0fmax_patch_bytes\x18\x0e \x01(\x05\x12\x16\n\x0esafe_max_files\x18\x0b \x01(\x05\x12\x16\n\x0esafe_max_lines\x18\x0c \x01(\x05\x12\x16\n\x0esafe_max_bytes\x18\r \x01(\x05\"\xff\x01\n\x12\x43ommitDiffResponse\x12\x11\n\tfrom_path\x18\x01 \x01(\x0c\x12\x0f\n\x07to_path\x18\x02 \x01(\x0c\x12\x0f\n\x07\x66rom_id\x18\x03 \x01(\t\x12\r\n\x05to_id\x18\x04 \x01(\t\x12\x10\n\x08old_mode\x18\x05 \x01(\x05\x12\x10\n\x08new_mode\x18\x06 \x01(\x05\x12\x0e\n\x06\x62inary\x18\x07 \x01(\x08\x12\x16\n\x0eraw_patch_data\x18\t \x01(\x0c\x12\x14\n\x0c\x65nd_of_patch\x18\n \x01(\x08\x12\x17\n\x0foverflow_marker\x18\x0b \x01(\x08\x12\x11\n\tcollapsed\x18\x0c \x01(\x08\x12\x11\n\ttoo_large\x18\r \x01(\x08J\x04\x08\x08\x10\t\"\x82\x01\n\x12\x43ommitDeltaRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\x12\r\n\x05paths\x18\x04 \x03(\x0c\"u\n\x0b\x43ommitDelta\x12\x11\n\tfrom_path\x18\x01 \x01(\x0c\x12\x0f\n\x07to_path\x18\x02 \x01(\x0c\x12\x0f\n\x07\x66rom_id\x18\x03 \x01(\t\x12\r\n\x05to_id\x18\x04 \x01(\t\x12\x10\n\x08old_mode\x18\x05 \x01(\x05\x12\x10\n\x08new_mode\x18\x06 \x01(\x05\":\n\x13\x43ommitDeltaResponse\x12#\n\x06\x64\x65ltas\x18\x01 \x03(\x0b\x32\x13.gitaly.CommitDelta\"o\n\x0eRawDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\"\x1f\n\x0fRawDiffResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"p\n\x0fRawPatchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\" \n\x10RawPatchResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"q\n\x10\x44iffStatsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\"Q\n\tDiffStats\x12\x0c\n\x04path\x18\x01 \x01(\x0c\x12\x11\n\tadditions\x18\x02 \x01(\x05\x12\x11\n\tdeletions\x18\x03 \x01(\x05\x12\x10\n\x08old_path\x18\x04 \x01(\x0c\"5\n\x11\x44iffStatsResponse\x12 \n\x05stats\x18\x01 \x03(\x0b\x32\x11.gitaly.DiffStats2\x89\x03\n\x0b\x44iffService\x12M\n\nCommitDiff\x12\x19.gitaly.CommitDiffRequest\x1a\x1a.gitaly.CommitDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12P\n\x0b\x43ommitDelta\x12\x1a.gitaly.CommitDeltaRequest\x1a\x1b.gitaly.CommitDeltaResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x44\n\x07RawDiff\x12\x16.gitaly.RawDiffRequest\x1a\x17.gitaly.RawDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12G\n\x08RawPatch\x12\x17.gitaly.RawPatchRequest\x1a\x18.gitaly.RawPatchResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tDiffStats\x12\x18.gitaly.DiffStatsRequest\x1a\x19.gitaly.DiffStatsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
+  serialized_pb=b'\n\ndiff.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"\xed\x02\n\x11\x43ommitDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\x12 \n\x18ignore_whitespace_change\x18\x04 \x01(\x08\x12\r\n\x05paths\x18\x05 \x03(\x0c\x12\x16\n\x0e\x63ollapse_diffs\x18\x06 \x01(\x08\x12\x16\n\x0e\x65nforce_limits\x18\x07 \x01(\x08\x12\x11\n\tmax_files\x18\x08 \x01(\x05\x12\x11\n\tmax_lines\x18\t \x01(\x05\x12\x11\n\tmax_bytes\x18\n \x01(\x05\x12\x17\n\x0fmax_patch_bytes\x18\x0e \x01(\x05\x12\x16\n\x0esafe_max_files\x18\x0b \x01(\x05\x12\x16\n\x0esafe_max_lines\x18\x0c \x01(\x05\x12\x16\n\x0esafe_max_bytes\x18\r \x01(\x05\"\xff\x01\n\x12\x43ommitDiffResponse\x12\x11\n\tfrom_path\x18\x01 \x01(\x0c\x12\x0f\n\x07to_path\x18\x02 \x01(\x0c\x12\x0f\n\x07\x66rom_id\x18\x03 \x01(\t\x12\r\n\x05to_id\x18\x04 \x01(\t\x12\x10\n\x08old_mode\x18\x05 \x01(\x05\x12\x10\n\x08new_mode\x18\x06 \x01(\x05\x12\x0e\n\x06\x62inary\x18\x07 \x01(\x08\x12\x16\n\x0eraw_patch_data\x18\t \x01(\x0c\x12\x14\n\x0c\x65nd_of_patch\x18\n \x01(\x08\x12\x17\n\x0foverflow_marker\x18\x0b \x01(\x08\x12\x11\n\tcollapsed\x18\x0c \x01(\x08\x12\x11\n\ttoo_large\x18\r \x01(\x08J\x04\x08\x08\x10\t\"\x82\x01\n\x12\x43ommitDeltaRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\x12\r\n\x05paths\x18\x04 \x03(\x0c\"u\n\x0b\x43ommitDelta\x12\x11\n\tfrom_path\x18\x01 \x01(\x0c\x12\x0f\n\x07to_path\x18\x02 \x01(\x0c\x12\x0f\n\x07\x66rom_id\x18\x03 \x01(\t\x12\r\n\x05to_id\x18\x04 \x01(\t\x12\x10\n\x08old_mode\x18\x05 \x01(\x05\x12\x10\n\x08new_mode\x18\x06 \x01(\x05\":\n\x13\x43ommitDeltaResponse\x12#\n\x06\x64\x65ltas\x18\x01 \x03(\x0b\x32\x13.gitaly.CommitDelta\"o\n\x0eRawDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\"\x1f\n\x0fRawDiffResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"p\n\x0fRawPatchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\" \n\x10RawPatchResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"q\n\x10\x44iffStatsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\"Q\n\tDiffStats\x12\x0c\n\x04path\x18\x01 \x01(\x0c\x12\x11\n\tadditions\x18\x02 \x01(\x05\x12\x11\n\tdeletions\x18\x03 \x01(\x05\x12\x10\n\x08old_path\x18\x04 \x01(\x0c\"5\n\x11\x44iffStatsResponse\x12 \n\x05stats\x18\x01 \x03(\x0b\x32\x11.gitaly.DiffStats\"X\n\x17\x46indChangedPathsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0f\n\x07\x63ommits\x18\x02 \x03(\t\"?\n\x18\x46indChangedPathsResponse\x12#\n\x05paths\x18\x01 \x03(\x0b\x32\x14.gitaly.ChangedPaths\"\x96\x01\n\x0c\x43hangedPaths\x12\x0c\n\x04path\x18\x01 \x01(\x0c\x12+\n\x06status\x18\x02 \x01(\x0e\x32\x1b.gitaly.ChangedPaths.Status\"K\n\x06Status\x12\t\n\x05\x41\x44\x44\x45\x44\x10\x00\x12\x0c\n\x08MODIFIED\x10\x01\x12\x0b\n\x07\x44\x45LETED\x10\x02\x12\x0f\n\x0bTYPE_CHANGE\x10\x03\x12\n\n\x06\x43OPIED\x10\x04\x32\xea\x03\n\x0b\x44iffService\x12M\n\nCommitDiff\x12\x19.gitaly.CommitDiffRequest\x1a\x1a.gitaly.CommitDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12P\n\x0b\x43ommitDelta\x12\x1a.gitaly.CommitDeltaRequest\x1a\x1b.gitaly.CommitDeltaResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x44\n\x07RawDiff\x12\x16.gitaly.RawDiffRequest\x1a\x17.gitaly.RawDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12G\n\x08RawPatch\x12\x17.gitaly.RawPatchRequest\x1a\x18.gitaly.RawPatchResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tDiffStats\x12\x18.gitaly.DiffStatsRequest\x1a\x19.gitaly.DiffStatsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12_\n\x10\x46indChangedPaths\x12\x1f.gitaly.FindChangedPathsRequest\x1a .gitaly.FindChangedPathsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
   ,
   dependencies=[lint__pb2.DESCRIPTOR,shared__pb2.DESCRIPTOR,])
 
 
 
+_CHANGEDPATHS_STATUS = _descriptor.EnumDescriptor(
+  name='Status',
+  full_name='gitaly.ChangedPaths.Status',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='ADDED', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='MODIFIED', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DELETED', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='TYPE_CHANGE', index=3, number=3,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='COPIED', index=4, number=4,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=1764,
+  serialized_end=1839,
+)
+_sym_db.RegisterEnumDescriptor(_CHANGEDPATHS_STATUS)
+
 
 _COMMITDIFFREQUEST = _descriptor.Descriptor(
   name='CommitDiffRequest',
   full_name='gitaly.CommitDiffRequest',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
@@ -694,33 +734,151 @@
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1478,
   serialized_end=1531,
 )
 
+
+_FINDCHANGEDPATHSREQUEST = _descriptor.Descriptor(
+  name='FindChangedPathsRequest',
+  full_name='gitaly.FindChangedPathsRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='repository', full_name='gitaly.FindChangedPathsRequest.repository', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=b'\230\306,\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='commits', full_name='gitaly.FindChangedPathsRequest.commits', index=1,
+      number=2, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1533,
+  serialized_end=1621,
+)
+
+
+_FINDCHANGEDPATHSRESPONSE = _descriptor.Descriptor(
+  name='FindChangedPathsResponse',
+  full_name='gitaly.FindChangedPathsResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='paths', full_name='gitaly.FindChangedPathsResponse.paths', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1623,
+  serialized_end=1686,
+)
+
+
+_CHANGEDPATHS = _descriptor.Descriptor(
+  name='ChangedPaths',
+  full_name='gitaly.ChangedPaths',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='path', full_name='gitaly.ChangedPaths.path', index=0,
+      number=1, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='status', full_name='gitaly.ChangedPaths.status', index=1,
+      number=2, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+    _CHANGEDPATHS_STATUS,
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1689,
+  serialized_end=1839,
+)
+
 _COMMITDIFFREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _COMMITDELTAREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _COMMITDELTARESPONSE.fields_by_name['deltas'].message_type = _COMMITDELTA
 _RAWDIFFREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _RAWPATCHREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _DIFFSTATSREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _DIFFSTATSRESPONSE.fields_by_name['stats'].message_type = _DIFFSTATS
+_FINDCHANGEDPATHSREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
+_FINDCHANGEDPATHSRESPONSE.fields_by_name['paths'].message_type = _CHANGEDPATHS
+_CHANGEDPATHS.fields_by_name['status'].enum_type = _CHANGEDPATHS_STATUS
+_CHANGEDPATHS_STATUS.containing_type = _CHANGEDPATHS
 DESCRIPTOR.message_types_by_name['CommitDiffRequest'] = _COMMITDIFFREQUEST
 DESCRIPTOR.message_types_by_name['CommitDiffResponse'] = _COMMITDIFFRESPONSE
 DESCRIPTOR.message_types_by_name['CommitDeltaRequest'] = _COMMITDELTAREQUEST
 DESCRIPTOR.message_types_by_name['CommitDelta'] = _COMMITDELTA
 DESCRIPTOR.message_types_by_name['CommitDeltaResponse'] = _COMMITDELTARESPONSE
 DESCRIPTOR.message_types_by_name['RawDiffRequest'] = _RAWDIFFREQUEST
 DESCRIPTOR.message_types_by_name['RawDiffResponse'] = _RAWDIFFRESPONSE
 DESCRIPTOR.message_types_by_name['RawPatchRequest'] = _RAWPATCHREQUEST
 DESCRIPTOR.message_types_by_name['RawPatchResponse'] = _RAWPATCHRESPONSE
 DESCRIPTOR.message_types_by_name['DiffStatsRequest'] = _DIFFSTATSREQUEST
 DESCRIPTOR.message_types_by_name['DiffStats'] = _DIFFSTATS
 DESCRIPTOR.message_types_by_name['DiffStatsResponse'] = _DIFFSTATSRESPONSE
+DESCRIPTOR.message_types_by_name['FindChangedPathsRequest'] = _FINDCHANGEDPATHSREQUEST
+DESCRIPTOR.message_types_by_name['FindChangedPathsResponse'] = _FINDCHANGEDPATHSRESPONSE
+DESCRIPTOR.message_types_by_name['ChangedPaths'] = _CHANGEDPATHS
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 CommitDiffRequest = _reflection.GeneratedProtocolMessageType('CommitDiffRequest', (_message.Message,), {
   'DESCRIPTOR' : _COMMITDIFFREQUEST,
   '__module__' : 'diff_pb2'
   # @@protoc_insertion_point(class_scope:gitaly.CommitDiffRequest)
   })
@@ -799,31 +957,53 @@
 DiffStatsResponse = _reflection.GeneratedProtocolMessageType('DiffStatsResponse', (_message.Message,), {
   'DESCRIPTOR' : _DIFFSTATSRESPONSE,
   '__module__' : 'diff_pb2'
   # @@protoc_insertion_point(class_scope:gitaly.DiffStatsResponse)
   })
 _sym_db.RegisterMessage(DiffStatsResponse)
 
+FindChangedPathsRequest = _reflection.GeneratedProtocolMessageType('FindChangedPathsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _FINDCHANGEDPATHSREQUEST,
+  '__module__' : 'diff_pb2'
+  # @@protoc_insertion_point(class_scope:gitaly.FindChangedPathsRequest)
+  })
+_sym_db.RegisterMessage(FindChangedPathsRequest)
+
+FindChangedPathsResponse = _reflection.GeneratedProtocolMessageType('FindChangedPathsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _FINDCHANGEDPATHSRESPONSE,
+  '__module__' : 'diff_pb2'
+  # @@protoc_insertion_point(class_scope:gitaly.FindChangedPathsResponse)
+  })
+_sym_db.RegisterMessage(FindChangedPathsResponse)
+
+ChangedPaths = _reflection.GeneratedProtocolMessageType('ChangedPaths', (_message.Message,), {
+  'DESCRIPTOR' : _CHANGEDPATHS,
+  '__module__' : 'diff_pb2'
+  # @@protoc_insertion_point(class_scope:gitaly.ChangedPaths)
+  })
+_sym_db.RegisterMessage(ChangedPaths)
+
 
 DESCRIPTOR._options = None
 _COMMITDIFFREQUEST.fields_by_name['repository']._options = None
 _COMMITDELTAREQUEST.fields_by_name['repository']._options = None
 _RAWDIFFREQUEST.fields_by_name['repository']._options = None
 _RAWPATCHREQUEST.fields_by_name['repository']._options = None
 _DIFFSTATSREQUEST.fields_by_name['repository']._options = None
+_FINDCHANGEDPATHSREQUEST.fields_by_name['repository']._options = None
 
 _DIFFSERVICE = _descriptor.ServiceDescriptor(
   name='DiffService',
   full_name='gitaly.DiffService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=1534,
-  serialized_end=1927,
+  serialized_start=1842,
+  serialized_end=2332,
   methods=[
   _descriptor.MethodDescriptor(
     name='CommitDiff',
     full_name='gitaly.DiffService.CommitDiff',
     index=0,
     containing_service=None,
     input_type=_COMMITDIFFREQUEST,
@@ -867,13 +1047,23 @@
     index=4,
     containing_service=None,
     input_type=_DIFFSTATSREQUEST,
     output_type=_DIFFSTATSRESPONSE,
     serialized_options=b'\372\227(\002\010\002',
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='FindChangedPaths',
+    full_name='gitaly.DiffService.FindChangedPaths',
+    index=5,
+    containing_service=None,
+    input_type=_FINDCHANGEDPATHSREQUEST,
+    output_type=_FINDCHANGEDPATHSRESPONSE,
+    serialized_options=b'\372\227(\002\010\002',
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_DIFFSERVICE)
 
 DESCRIPTOR.services_by_name['DiffService'] = _DIFFSERVICE
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hgitaly-0.8.1/hgitaly/stub/diff_pb2_grpc.py` & `hgitaly-0.9.0/hgitaly/stub/diff_pb2_grpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,19 @@
                 response_deserializer=diff__pb2.RawPatchResponse.FromString,
                 )
         self.DiffStats = channel.unary_stream(
                 '/gitaly.DiffService/DiffStats',
                 request_serializer=diff__pb2.DiffStatsRequest.SerializeToString,
                 response_deserializer=diff__pb2.DiffStatsResponse.FromString,
                 )
+        self.FindChangedPaths = channel.unary_stream(
+                '/gitaly.DiffService/FindChangedPaths',
+                request_serializer=diff__pb2.FindChangedPathsRequest.SerializeToString,
+                response_deserializer=diff__pb2.FindChangedPathsResponse.FromString,
+                )
 
 
 class DiffServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def CommitDiff(self, request, context):
         """Returns stream of CommitDiffResponse with patches chunked over messages
@@ -72,14 +77,21 @@
 
     def DiffStats(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def FindChangedPaths(self, request, context):
+        """Return a list of files changed along with the status of each file
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DiffServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CommitDiff': grpc.unary_stream_rpc_method_handler(
                     servicer.CommitDiff,
                     request_deserializer=diff__pb2.CommitDiffRequest.FromString,
                     response_serializer=diff__pb2.CommitDiffResponse.SerializeToString,
@@ -100,14 +112,19 @@
                     response_serializer=diff__pb2.RawPatchResponse.SerializeToString,
             ),
             'DiffStats': grpc.unary_stream_rpc_method_handler(
                     servicer.DiffStats,
                     request_deserializer=diff__pb2.DiffStatsRequest.FromString,
                     response_serializer=diff__pb2.DiffStatsResponse.SerializeToString,
             ),
+            'FindChangedPaths': grpc.unary_stream_rpc_method_handler(
+                    servicer.FindChangedPaths,
+                    request_deserializer=diff__pb2.FindChangedPathsRequest.FromString,
+                    response_serializer=diff__pb2.FindChangedPathsResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'gitaly.DiffService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -194,7 +211,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/gitaly.DiffService/DiffStats',
             diff__pb2.DiffStatsRequest.SerializeToString,
             diff__pb2.DiffStatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def FindChangedPaths(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/gitaly.DiffService/FindChangedPaths',
+            diff__pb2.FindChangedPathsRequest.SerializeToString,
+            diff__pb2.FindChangedPathsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `hgitaly-0.8.1/hgitaly/stub/lint_pb2.py` & `hgitaly-0.9.0/hgitaly/stub/lint_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='lint.proto',
   package='gitaly',
   syntax='proto3',
   serialized_options=b'Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypb',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\nlint.proto\x12\x06gitaly\x1a google/protobuf/descriptor.proto\"\xd2\x01\n\x0cOperationMsg\x12*\n\x02op\x18\x01 \x01(\x0e\x32\x1e.gitaly.OperationMsg.Operation\x12/\n\x0bscope_level\x18\x02 \x01(\x0e\x32\x1a.gitaly.OperationMsg.Scope\"3\n\tOperation\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MUTATOR\x10\x01\x12\x0c\n\x08\x41\x43\x43\x45SSOR\x10\x02\"0\n\x05Scope\x12\x0e\n\nREPOSITORY\x10\x00\x12\n\n\x06SERVER\x10\x01\x12\x0b\n\x07STORAGE\x10\x02:6\n\x0bintercepted\x12\x1f.google.protobuf.ServiceOptions\x18\xfe\x82\x05 \x01(\x08:G\n\x07op_type\x12\x1e.google.protobuf.MethodOptions\x18\xff\x82\x05 \x01(\x0b\x32\x14.gitaly.OperationMsg:0\n\x07storage\x12\x1d.google.protobuf.FieldOptions\x18\xe1\xc8\x05 \x01(\x08:3\n\nrepository\x12\x1d.google.protobuf.FieldOptions\x18\xe2\xc8\x05 \x01(\x08::\n\x11target_repository\x12\x1d.google.protobuf.FieldOptions\x18\xe3\xc8\x05 \x01(\x08:>\n\x15\x61\x64\x64itional_repository\x12\x1d.google.protobuf.FieldOptions\x18\xe4\xc8\x05 \x01(\x08\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
+  serialized_pb=b'\n\nlint.proto\x12\x06gitaly\x1a google/protobuf/descriptor.proto\"\xd4\x01\n\x0cOperationMsg\x12*\n\x02op\x18\x01 \x01(\x0e\x32\x1e.gitaly.OperationMsg.Operation\x12/\n\x0bscope_level\x18\x02 \x01(\x0e\x32\x1a.gitaly.OperationMsg.Scope\"3\n\tOperation\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MUTATOR\x10\x01\x12\x0c\n\x08\x41\x43\x43\x45SSOR\x10\x02\"2\n\x05Scope\x12\x0e\n\nREPOSITORY\x10\x00\x12\x0b\n\x07STORAGE\x10\x02\"\x04\x08\x01\x10\x01*\x06SERVER:6\n\x0bintercepted\x12\x1f.google.protobuf.ServiceOptions\x18\xfe\x82\x05 \x01(\x08:G\n\x07op_type\x12\x1e.google.protobuf.MethodOptions\x18\xff\x82\x05 \x01(\x0b\x32\x14.gitaly.OperationMsg:0\n\x07storage\x12\x1d.google.protobuf.FieldOptions\x18\xe1\xc8\x05 \x01(\x08:3\n\nrepository\x12\x1d.google.protobuf.FieldOptions\x18\xe2\xc8\x05 \x01(\x08::\n\x11target_repository\x12\x1d.google.protobuf.FieldOptions\x18\xe3\xc8\x05 \x01(\x08:>\n\x15\x61\x64\x64itional_repository\x12\x1d.google.protobuf.FieldOptions\x18\xe4\xc8\x05 \x01(\x08\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_descriptor__pb2.DESCRIPTOR,])
 
 
 INTERCEPTED_FIELD_NUMBER = 82302
 intercepted = _descriptor.FieldDescriptor(
   name='intercepted', full_name='gitaly.intercepted', index=0,
@@ -113,28 +113,23 @@
   values=[
     _descriptor.EnumValueDescriptor(
       name='REPOSITORY', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='SERVER', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='STORAGE', index=2, number=2,
+      name='STORAGE', index=1, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
   serialized_start=219,
-  serialized_end=267,
+  serialized_end=269,
 )
 _sym_db.RegisterEnumDescriptor(_OPERATIONMSG_SCOPE)
 
 
 _OPERATIONMSG = _descriptor.Descriptor(
   name='OperationMsg',
   full_name='gitaly.OperationMsg',
@@ -168,15 +163,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=57,
-  serialized_end=267,
+  serialized_end=269,
 )
 
 _OPERATIONMSG.fields_by_name['op'].enum_type = _OPERATIONMSG_OPERATION
 _OPERATIONMSG.fields_by_name['scope_level'].enum_type = _OPERATIONMSG_SCOPE
 _OPERATIONMSG_OPERATION.containing_type = _OPERATIONMSG
 _OPERATIONMSG_SCOPE.containing_type = _OPERATIONMSG
 DESCRIPTOR.message_types_by_name['OperationMsg'] = _OPERATIONMSG
```

### Comparing `hgitaly-0.8.1/hgitaly/stub/ref_pb2.py` & `hgitaly-0.9.0/hgitaly/stub/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/stub/ref_pb2_grpc.py` & `hgitaly-0.9.0/hgitaly/stub/ref_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,17 @@
     def RefExists(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def FindBranch(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """FindBranch finds a branch by its unqualified name (like "master") and
+        returns the commit it currently points to.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteRefs(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
```

### Comparing `hgitaly-0.8.1/hgitaly/stub/repository_service_pb2.py` & `hgitaly-0.9.0/hgitaly/stub/repository_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='repository-service.proto',
   package='gitaly',
   syntax='proto3',
   serialized_options=b'Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypb',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x18repository-service.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"G\n\x17RepositoryExistsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"*\n\x18RepositoryExistsResponse\x12\x0e\n\x06\x65xists\x18\x01 \x01(\x08\"H\n\x18RepackIncrementalRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1b\n\x19RepackIncrementalResponse\"X\n\x11RepackFullRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rcreate_bitmap\x18\x02 \x01(\x08\"\x14\n\x12RepackFullResponse\"A\n\x11MidxRepackRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x14\n\x12MidxRepackResponse\"k\n\x15GarbageCollectRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rcreate_bitmap\x18\x02 \x01(\x08\x12\r\n\x05prune\x18\x03 \x01(\x08\"\x18\n\x16GarbageCollectResponse\"G\n\x17WriteCommitGraphRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1a\n\x18WriteCommitGraphResponse\">\n\x0e\x43leanupRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x11\n\x0f\x43leanupResponse\"E\n\x15RepositorySizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"&\n\x16RepositorySizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\"[\n\x19\x41pplyGitattributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"\x1c\n\x1a\x41pplyGitattributesResponse\"\xe8\x01\n\x12\x46\x65tchRemoteRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0e\n\x06remote\x18\x02 \x01(\t\x12\r\n\x05\x66orce\x18\x03 \x01(\x08\x12\x0f\n\x07no_tags\x18\x04 \x01(\x08\x12\x0f\n\x07timeout\x18\x05 \x01(\x05\x12\x0f\n\x07ssh_key\x18\x06 \x01(\t\x12\x13\n\x0bknown_hosts\x18\x07 \x01(\t\x12\x10\n\x08no_prune\x18\t \x01(\x08\x12%\n\rremote_params\x18\n \x01(\x0b\x32\x0e.gitaly.RemoteJ\x04\x08\x08\x10\t\"\x15\n\x13\x46\x65tchRemoteResponse\"G\n\x17\x43reateRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1a\n\x18\x43reateRepositoryResponse\"\x99\x02\n\x11GetArchiveRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tcommit_id\x18\x02 \x01(\t\x12\x0e\n\x06prefix\x18\x03 \x01(\t\x12\x30\n\x06\x66ormat\x18\x04 \x01(\x0e\x32 .gitaly.GetArchiveRequest.Format\x12\x0c\n\x04path\x18\x05 \x01(\x0c\x12\x0f\n\x07\x65xclude\x18\x06 \x03(\x0c\x12\x12\n\nelide_path\x18\x07 \x01(\x08\x12\x19\n\x11include_lfs_blobs\x18\x08 \x01(\x08\"3\n\x06\x46ormat\x12\x07\n\x03ZIP\x10\x00\x12\x07\n\x03TAR\x10\x01\x12\n\n\x06TAR_GZ\x10\x02\x12\x0b\n\x07TAR_BZ2\x10\x03\"\"\n\x12GetArchiveResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"G\n\x17HasLocalBranchesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\")\n\x18HasLocalBranchesResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\xa2\x01\n\x18\x46\x65tchSourceBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11source_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x15\n\rsource_branch\x18\x03 \x01(\x0c\x12\x12\n\ntarget_ref\x18\x04 \x01(\x0c\"+\n\x19\x46\x65tchSourceBranchResponse\x12\x0e\n\x06result\x18\x01 \x01(\x08\";\n\x0b\x46sckRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1d\n\x0c\x46sckResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\x0c\"\x89\x01\n\x0fWriteRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03ref\x18\x02 \x01(\x0c\x12\x10\n\x08revision\x18\x03 \x01(\x0c\x12\x14\n\x0cold_revision\x18\x04 \x01(\x0c\x12\r\n\x05\x66orce\x18\x05 \x01(\x08J\x04\x08\x06\x10\x07\"\x18\n\x10WriteRefResponseJ\x04\x08\x01\x10\x02\"W\n\x14\x46indMergeBaseRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\x0c\"%\n\x15\x46indMergeBaseResponse\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"p\n\x11\x43reateForkRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11source_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\"\x14\n\x12\x43reateForkResponse\"\\\n\x19IsRebaseInProgressRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trebase_id\x18\x02 \x01(\t\"1\n\x1aIsRebaseInProgressResponse\x12\x13\n\x0bin_progress\x18\x01 \x01(\x08\"\\\n\x19IsSquashInProgressRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tsquash_id\x18\x02 \x01(\t\"1\n\x1aIsSquashInProgressResponse\x12\x13\n\x0bin_progress\x18\x01 \x01(\x08\"[\n\x1e\x43reateRepositoryFromURLRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03url\x18\x02 \x01(\t\"!\n\x1f\x43reateRepositoryFromURLResponse\"C\n\x13\x43reateBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"$\n\x14\x43reateBundleResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\xd2\x01\n\x10SetConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12/\n\x07\x65ntries\x18\x02 \x03(\x0b\x32\x1e.gitaly.SetConfigRequest.Entry\x1a_\n\x05\x45ntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x13\n\tvalue_str\x18\x02 \x01(\tH\x00\x12\x15\n\x0bvalue_int32\x18\x03 \x01(\x05H\x00\x12\x14\n\nvalue_bool\x18\x04 \x01(\x08H\x00\x42\x07\n\x05value\"\x13\n\x11SetConfigResponse\"Q\n\x13\x44\x65leteConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04keys\x18\x02 \x03(\t\"\x16\n\x14\x44\x65leteConfigResponse\"W\n\x19RestoreCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x1c\n\x1aRestoreCustomHooksResponse\"H\n\x18\x42\x61\x63kupCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\")\n\x19\x42\x61\x63kupCustomHooksResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"_\n!CreateRepositoryFromBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"$\n\"CreateRepositoryFromBundleResponse\"B\n\x12\x46indLicenseRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"1\n\x13\x46indLicenseResponse\x12\x1a\n\x12license_short_name\x18\x01 \x01(\t\"H\n\x18GetInfoAttributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"/\n\x19GetInfoAttributesResponse\x12\x12\n\nattributes\x18\x01 \x01(\x0c\"H\n\x18\x43\x61lculateChecksumRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"-\n\x19\x43\x61lculateChecksumResponse\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\"B\n\x12GetSnapshotRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"#\n\x13GetSnapshotResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"x\n#CreateRepositoryFromSnapshotRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08http_url\x18\x02 \x01(\t\x12\x11\n\thttp_auth\x18\x03 \x01(\t\"&\n$CreateRepositoryFromSnapshotResponse\"p\n\x14GetRawChangesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rfrom_revision\x18\x02 \x01(\t\x12\x13\n\x0bto_revision\x18\x03 \x01(\t\"\xca\x03\n\x15GetRawChangesResponse\x12<\n\x0braw_changes\x18\x01 \x03(\x0b\x32\'.gitaly.GetRawChangesResponse.RawChange\x1a\xf2\x02\n\tRawChange\x12\x0f\n\x07\x62lob_id\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x03\x12\x14\n\x08new_path\x18\x03 \x01(\tB\x02\x18\x01\x12\x14\n\x08old_path\x18\x04 \x01(\tB\x02\x18\x01\x12\x44\n\toperation\x18\x05 \x01(\x0e\x32\x31.gitaly.GetRawChangesResponse.RawChange.Operation\x12\x15\n\rraw_operation\x18\x06 \x01(\t\x12\x10\n\x08old_mode\x18\x07 \x01(\x05\x12\x10\n\x08new_mode\x18\x08 \x01(\x05\x12\x16\n\x0enew_path_bytes\x18\t \x01(\x0c\x12\x16\n\x0eold_path_bytes\x18\n \x01(\x0c\"i\n\tOperation\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x41\x44\x44\x45\x44\x10\x01\x12\n\n\x06\x43OPIED\x10\x02\x12\x0b\n\x07\x44\x45LETED\x10\x03\x12\x0c\n\x08MODIFIED\x10\x04\x12\x0b\n\x07RENAMED\x10\x05\x12\x10\n\x0cTYPE_CHANGED\x10\x06\"t\n\x18SearchFilesByNameRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x03 \x01(\x0c\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t\"*\n\x19SearchFilesByNameResponse\x12\r\n\x05\x66iles\x18\x01 \x03(\x0c\"\x81\x01\n\x1bSearchFilesByContentRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x03 \x01(\x0c\x12\x18\n\x10\x63hunked_response\x18\x04 \x01(\x08\"Y\n\x1cSearchFilesByContentResponse\x12\x0f\n\x07matches\x18\x01 \x03(\x0c\x12\x12\n\nmatch_data\x18\x02 \x01(\x0c\x12\x14\n\x0c\x65nd_of_match\x18\x03 \x01(\x08\"^\n\x06Remote\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12!\n\x19http_authorization_header\x18\x03 \x01(\t\x12\x16\n\x0emirror_refmaps\x18\x04 \x03(\t\"M\n\x1dGetObjectDirectorySizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\".\n\x1eGetObjectDirectorySizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\"\x86\x01\n\x14\x43loneFromPoolRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12 \n\x04pool\x18\x02 \x01(\x0b\x32\x12.gitaly.ObjectPool\x12\x1e\n\x06remote\x18\x03 \x01(\x0b\x32\x0e.gitaly.Remote\"\x17\n\x15\x43loneFromPoolResponse\"\x9d\x01\n\x1c\x43loneFromPoolInternalRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12 \n\x04pool\x18\x02 \x01(\x0b\x32\x12.gitaly.ObjectPool\x12-\n\x11source_repository\x18\x03 \x01(\x0b\x32\x12.gitaly.Repository\"\x1f\n\x1d\x43loneFromPoolInternalResponse\"G\n\x17RemoveRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1a\n\x18RemoveRepositoryResponse\"^\n\x17RenameRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rrelative_path\x18\x02 \x01(\t\"\x1a\n\x18RenameRepositoryResponse\"n\n\x1aReplicateRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\"\n\x06source\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\"\x1d\n\x1bReplicateRepositoryResponse\"I\n\x19OptimizeRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1c\n\x1aOptimizeRepositoryResponse2\xdb\x1e\n\x11RepositoryService\x12]\n\x10RepositoryExists\x12\x1f.gitaly.RepositoryExistsRequest\x1a .gitaly.RepositoryExistsResponse\"\x06\xfa\x97(\x02\x08\x02\x12`\n\x11RepackIncremental\x12 .gitaly.RepackIncrementalRequest\x1a!.gitaly.RepackIncrementalResponse\"\x06\xfa\x97(\x02\x08\x01\x12K\n\nRepackFull\x12\x19.gitaly.RepackFullRequest\x1a\x1a.gitaly.RepackFullResponse\"\x06\xfa\x97(\x02\x08\x01\x12K\n\nMidxRepack\x12\x19.gitaly.MidxRepackRequest\x1a\x1a.gitaly.MidxRepackResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eGarbageCollect\x12\x1d.gitaly.GarbageCollectRequest\x1a\x1e.gitaly.GarbageCollectResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10WriteCommitGraph\x12\x1f.gitaly.WriteCommitGraphRequest\x1a .gitaly.WriteCommitGraphResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eRepositorySize\x12\x1d.gitaly.RepositorySizeRequest\x1a\x1e.gitaly.RepositorySizeResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x63\n\x12\x41pplyGitattributes\x12!.gitaly.ApplyGitattributesRequest\x1a\".gitaly.ApplyGitattributesResponse\"\x06\xfa\x97(\x02\x08\x01\x12N\n\x0b\x46\x65tchRemote\x12\x1a.gitaly.FetchRemoteRequest\x1a\x1b.gitaly.FetchRemoteResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10\x43reateRepository\x12\x1f.gitaly.CreateRepositoryRequest\x1a .gitaly.CreateRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12M\n\nGetArchive\x12\x19.gitaly.GetArchiveRequest\x1a\x1a.gitaly.GetArchiveResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12]\n\x10HasLocalBranches\x12\x1f.gitaly.HasLocalBranchesRequest\x1a .gitaly.HasLocalBranchesResponse\"\x06\xfa\x97(\x02\x08\x02\x12`\n\x11\x46\x65tchSourceBranch\x12 .gitaly.FetchSourceBranchRequest\x1a!.gitaly.FetchSourceBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x39\n\x04\x46sck\x12\x13.gitaly.FsckRequest\x1a\x14.gitaly.FsckResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x45\n\x08WriteRef\x12\x17.gitaly.WriteRefRequest\x1a\x18.gitaly.WriteRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rFindMergeBase\x12\x1c.gitaly.FindMergeBaseRequest\x1a\x1d.gitaly.FindMergeBaseResponse\"\x06\xfa\x97(\x02\x08\x02\x12K\n\nCreateFork\x12\x19.gitaly.CreateForkRequest\x1a\x1a.gitaly.CreateForkResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x63\n\x12IsRebaseInProgress\x12!.gitaly.IsRebaseInProgressRequest\x1a\".gitaly.IsRebaseInProgressResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x63\n\x12IsSquashInProgress\x12!.gitaly.IsSquashInProgressRequest\x1a\".gitaly.IsSquashInProgressResponse\"\x06\xfa\x97(\x02\x08\x02\x12r\n\x17\x43reateRepositoryFromURL\x12&.gitaly.CreateRepositoryFromURLRequest\x1a\'.gitaly.CreateRepositoryFromURLResponse\"\x06\xfa\x97(\x02\x08\x01\x12S\n\x0c\x43reateBundle\x12\x1b.gitaly.CreateBundleRequest\x1a\x1c.gitaly.CreateBundleResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12}\n\x1a\x43reateRepositoryFromBundle\x12).gitaly.CreateRepositoryFromBundleRequest\x1a*.gitaly.CreateRepositoryFromBundleResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12H\n\tSetConfig\x12\x18.gitaly.SetConfigRequest\x1a\x19.gitaly.SetConfigResponse\"\x06\xfa\x97(\x02\x08\x01\x12Q\n\x0c\x44\x65leteConfig\x12\x1b.gitaly.DeleteConfigRequest\x1a\x1c.gitaly.DeleteConfigResponse\"\x06\xfa\x97(\x02\x08\x01\x12N\n\x0b\x46indLicense\x12\x1a.gitaly.FindLicenseRequest\x1a\x1b.gitaly.FindLicenseResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x62\n\x11GetInfoAttributes\x12 .gitaly.GetInfoAttributesRequest\x1a!.gitaly.GetInfoAttributesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12`\n\x11\x43\x61lculateChecksum\x12 .gitaly.CalculateChecksumRequest\x1a!.gitaly.CalculateChecksumResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x42\n\x07\x43leanup\x12\x16.gitaly.CleanupRequest\x1a\x17.gitaly.CleanupResponse\"\x06\xfa\x97(\x02\x08\x01\x12P\n\x0bGetSnapshot\x12\x1a.gitaly.GetSnapshotRequest\x1a\x1b.gitaly.GetSnapshotResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x81\x01\n\x1c\x43reateRepositoryFromSnapshot\x12+.gitaly.CreateRepositoryFromSnapshotRequest\x1a,.gitaly.CreateRepositoryFromSnapshotResponse\"\x06\xfa\x97(\x02\x08\x01\x12V\n\rGetRawChanges\x12\x1c.gitaly.GetRawChangesRequest\x1a\x1d.gitaly.GetRawChangesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12k\n\x14SearchFilesByContent\x12#.gitaly.SearchFilesByContentRequest\x1a$.gitaly.SearchFilesByContentResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x62\n\x11SearchFilesByName\x12 .gitaly.SearchFilesByNameRequest\x1a!.gitaly.SearchFilesByNameResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x65\n\x12RestoreCustomHooks\x12!.gitaly.RestoreCustomHooksRequest\x1a\".gitaly.RestoreCustomHooksResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12\x62\n\x11\x42\x61\x63kupCustomHooks\x12 .gitaly.BackupCustomHooksRequest\x1a!.gitaly.BackupCustomHooksResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12o\n\x16GetObjectDirectorySize\x12%.gitaly.GetObjectDirectorySizeRequest\x1a&.gitaly.GetObjectDirectorySizeResponse\"\x06\xfa\x97(\x02\x08\x02\x12T\n\rCloneFromPool\x12\x1c.gitaly.CloneFromPoolRequest\x1a\x1d.gitaly.CloneFromPoolResponse\"\x06\xfa\x97(\x02\x08\x01\x12l\n\x15\x43loneFromPoolInternal\x12$.gitaly.CloneFromPoolInternalRequest\x1a%.gitaly.CloneFromPoolInternalResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10RemoveRepository\x12\x1f.gitaly.RemoveRepositoryRequest\x1a .gitaly.RemoveRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10RenameRepository\x12\x1f.gitaly.RenameRepositoryRequest\x1a .gitaly.RenameRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x66\n\x13ReplicateRepository\x12\".gitaly.ReplicateRepositoryRequest\x1a#.gitaly.ReplicateRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x63\n\x12OptimizeRepository\x12!.gitaly.OptimizeRepositoryRequest\x1a\".gitaly.OptimizeRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
+  serialized_pb=b'\n\x18repository-service.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"G\n\x17RepositoryExistsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"*\n\x18RepositoryExistsResponse\x12\x0e\n\x06\x65xists\x18\x01 \x01(\x08\"H\n\x18RepackIncrementalRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1b\n\x19RepackIncrementalResponse\"X\n\x11RepackFullRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rcreate_bitmap\x18\x02 \x01(\x08\"\x14\n\x12RepackFullResponse\"A\n\x11MidxRepackRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x14\n\x12MidxRepackResponse\"k\n\x15GarbageCollectRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rcreate_bitmap\x18\x02 \x01(\x08\x12\r\n\x05prune\x18\x03 \x01(\x08\"\x18\n\x16GarbageCollectResponse\"G\n\x17WriteCommitGraphRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1a\n\x18WriteCommitGraphResponse\">\n\x0e\x43leanupRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x11\n\x0f\x43leanupResponse\"E\n\x15RepositorySizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"&\n\x16RepositorySizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\"[\n\x19\x41pplyGitattributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"\x1c\n\x1a\x41pplyGitattributesResponse\"\x84\x02\n\x12\x46\x65tchRemoteRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0e\n\x06remote\x18\x02 \x01(\t\x12\r\n\x05\x66orce\x18\x03 \x01(\x08\x12\x0f\n\x07no_tags\x18\x04 \x01(\x08\x12\x0f\n\x07timeout\x18\x05 \x01(\x05\x12\x0f\n\x07ssh_key\x18\x06 \x01(\t\x12\x13\n\x0bknown_hosts\x18\x07 \x01(\t\x12\x10\n\x08no_prune\x18\t \x01(\x08\x12%\n\rremote_params\x18\n \x01(\x0b\x32\x0e.gitaly.Remote\x12\x1a\n\x12\x63heck_tags_changed\x18\x0b \x01(\x08J\x04\x08\x08\x10\t\"+\n\x13\x46\x65tchRemoteResponse\x12\x14\n\x0ctags_changed\x18\x01 \x01(\x08\"G\n\x17\x43reateRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1a\n\x18\x43reateRepositoryResponse\"\x99\x02\n\x11GetArchiveRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tcommit_id\x18\x02 \x01(\t\x12\x0e\n\x06prefix\x18\x03 \x01(\t\x12\x30\n\x06\x66ormat\x18\x04 \x01(\x0e\x32 .gitaly.GetArchiveRequest.Format\x12\x0c\n\x04path\x18\x05 \x01(\x0c\x12\x0f\n\x07\x65xclude\x18\x06 \x03(\x0c\x12\x12\n\nelide_path\x18\x07 \x01(\x08\x12\x19\n\x11include_lfs_blobs\x18\x08 \x01(\x08\"3\n\x06\x46ormat\x12\x07\n\x03ZIP\x10\x00\x12\x07\n\x03TAR\x10\x01\x12\n\n\x06TAR_GZ\x10\x02\x12\x0b\n\x07TAR_BZ2\x10\x03\"\"\n\x12GetArchiveResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"G\n\x17HasLocalBranchesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\")\n\x18HasLocalBranchesResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\xa2\x01\n\x18\x46\x65tchSourceBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11source_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x15\n\rsource_branch\x18\x03 \x01(\x0c\x12\x12\n\ntarget_ref\x18\x04 \x01(\x0c\"+\n\x19\x46\x65tchSourceBranchResponse\x12\x0e\n\x06result\x18\x01 \x01(\x08\";\n\x0b\x46sckRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1d\n\x0c\x46sckResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\x0c\"\x89\x01\n\x0fWriteRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03ref\x18\x02 \x01(\x0c\x12\x10\n\x08revision\x18\x03 \x01(\x0c\x12\x14\n\x0cold_revision\x18\x04 \x01(\x0c\x12\r\n\x05\x66orce\x18\x05 \x01(\x08J\x04\x08\x06\x10\x07\"\x18\n\x10WriteRefResponseJ\x04\x08\x01\x10\x02\"W\n\x14\x46indMergeBaseRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\x0c\"%\n\x15\x46indMergeBaseResponse\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"p\n\x11\x43reateForkRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11source_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\"\x14\n\x12\x43reateForkResponse\"\\\n\x19IsRebaseInProgressRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trebase_id\x18\x02 \x01(\t\"1\n\x1aIsRebaseInProgressResponse\x12\x13\n\x0bin_progress\x18\x01 \x01(\x08\"\\\n\x19IsSquashInProgressRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tsquash_id\x18\x02 \x01(\t\"1\n\x1aIsSquashInProgressResponse\x12\x13\n\x0bin_progress\x18\x01 \x01(\x08\"[\n\x1e\x43reateRepositoryFromURLRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03url\x18\x02 \x01(\t\"!\n\x1f\x43reateRepositoryFromURLResponse\"C\n\x13\x43reateBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"$\n\x14\x43reateBundleResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\xd2\x01\n\x10SetConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12/\n\x07\x65ntries\x18\x02 \x03(\x0b\x32\x1e.gitaly.SetConfigRequest.Entry\x1a_\n\x05\x45ntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x13\n\tvalue_str\x18\x02 \x01(\tH\x00\x12\x15\n\x0bvalue_int32\x18\x03 \x01(\x05H\x00\x12\x14\n\nvalue_bool\x18\x04 \x01(\x08H\x00\x42\x07\n\x05value\"\x13\n\x11SetConfigResponse\"Q\n\x13\x44\x65leteConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04keys\x18\x02 \x03(\t\"\x16\n\x14\x44\x65leteConfigResponse\"W\n\x19RestoreCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x1c\n\x1aRestoreCustomHooksResponse\"H\n\x18\x42\x61\x63kupCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\")\n\x19\x42\x61\x63kupCustomHooksResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"_\n!CreateRepositoryFromBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"$\n\"CreateRepositoryFromBundleResponse\"B\n\x12\x46indLicenseRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"1\n\x13\x46indLicenseResponse\x12\x1a\n\x12license_short_name\x18\x01 \x01(\t\"H\n\x18GetInfoAttributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"/\n\x19GetInfoAttributesResponse\x12\x12\n\nattributes\x18\x01 \x01(\x0c\"H\n\x18\x43\x61lculateChecksumRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"-\n\x19\x43\x61lculateChecksumResponse\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\"B\n\x12GetSnapshotRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"#\n\x13GetSnapshotResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"x\n#CreateRepositoryFromSnapshotRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08http_url\x18\x02 \x01(\t\x12\x11\n\thttp_auth\x18\x03 \x01(\t\"&\n$CreateRepositoryFromSnapshotResponse\"p\n\x14GetRawChangesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rfrom_revision\x18\x02 \x01(\t\x12\x13\n\x0bto_revision\x18\x03 \x01(\t\"\xca\x03\n\x15GetRawChangesResponse\x12<\n\x0braw_changes\x18\x01 \x03(\x0b\x32\'.gitaly.GetRawChangesResponse.RawChange\x1a\xf2\x02\n\tRawChange\x12\x0f\n\x07\x62lob_id\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x03\x12\x14\n\x08new_path\x18\x03 \x01(\tB\x02\x18\x01\x12\x14\n\x08old_path\x18\x04 \x01(\tB\x02\x18\x01\x12\x44\n\toperation\x18\x05 \x01(\x0e\x32\x31.gitaly.GetRawChangesResponse.RawChange.Operation\x12\x15\n\rraw_operation\x18\x06 \x01(\t\x12\x10\n\x08old_mode\x18\x07 \x01(\x05\x12\x10\n\x08new_mode\x18\x08 \x01(\x05\x12\x16\n\x0enew_path_bytes\x18\t \x01(\x0c\x12\x16\n\x0eold_path_bytes\x18\n \x01(\x0c\"i\n\tOperation\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x41\x44\x44\x45\x44\x10\x01\x12\n\n\x06\x43OPIED\x10\x02\x12\x0b\n\x07\x44\x45LETED\x10\x03\x12\x0c\n\x08MODIFIED\x10\x04\x12\x0b\n\x07RENAMED\x10\x05\x12\x10\n\x0cTYPE_CHANGED\x10\x06\"t\n\x18SearchFilesByNameRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x03 \x01(\x0c\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t\"*\n\x19SearchFilesByNameResponse\x12\r\n\x05\x66iles\x18\x01 \x03(\x0c\"\x81\x01\n\x1bSearchFilesByContentRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x03 \x01(\x0c\x12\x18\n\x10\x63hunked_response\x18\x04 \x01(\x08\"Y\n\x1cSearchFilesByContentResponse\x12\x0f\n\x07matches\x18\x01 \x03(\x0c\x12\x12\n\nmatch_data\x18\x02 \x01(\x0c\x12\x14\n\x0c\x65nd_of_match\x18\x03 \x01(\x08\"^\n\x06Remote\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12!\n\x19http_authorization_header\x18\x03 \x01(\t\x12\x16\n\x0emirror_refmaps\x18\x04 \x03(\t\"M\n\x1dGetObjectDirectorySizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\".\n\x1eGetObjectDirectorySizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\"\x86\x01\n\x14\x43loneFromPoolRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12 \n\x04pool\x18\x02 \x01(\x0b\x32\x12.gitaly.ObjectPool\x12\x1e\n\x06remote\x18\x03 \x01(\x0b\x32\x0e.gitaly.Remote\"\x17\n\x15\x43loneFromPoolResponse\"\x9d\x01\n\x1c\x43loneFromPoolInternalRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12 \n\x04pool\x18\x02 \x01(\x0b\x32\x12.gitaly.ObjectPool\x12-\n\x11source_repository\x18\x03 \x01(\x0b\x32\x12.gitaly.Repository\"\x1f\n\x1d\x43loneFromPoolInternalResponse\"G\n\x17RemoveRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1a\n\x18RemoveRepositoryResponse\"^\n\x17RenameRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rrelative_path\x18\x02 \x01(\t\"\x1a\n\x18RenameRepositoryResponse\"n\n\x1aReplicateRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\"\n\x06source\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\"\x1d\n\x1bReplicateRepositoryResponse\"I\n\x19OptimizeRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1c\n\x1aOptimizeRepositoryResponse2\xdb\x1e\n\x11RepositoryService\x12]\n\x10RepositoryExists\x12\x1f.gitaly.RepositoryExistsRequest\x1a .gitaly.RepositoryExistsResponse\"\x06\xfa\x97(\x02\x08\x02\x12`\n\x11RepackIncremental\x12 .gitaly.RepackIncrementalRequest\x1a!.gitaly.RepackIncrementalResponse\"\x06\xfa\x97(\x02\x08\x01\x12K\n\nRepackFull\x12\x19.gitaly.RepackFullRequest\x1a\x1a.gitaly.RepackFullResponse\"\x06\xfa\x97(\x02\x08\x01\x12K\n\nMidxRepack\x12\x19.gitaly.MidxRepackRequest\x1a\x1a.gitaly.MidxRepackResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eGarbageCollect\x12\x1d.gitaly.GarbageCollectRequest\x1a\x1e.gitaly.GarbageCollectResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10WriteCommitGraph\x12\x1f.gitaly.WriteCommitGraphRequest\x1a .gitaly.WriteCommitGraphResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eRepositorySize\x12\x1d.gitaly.RepositorySizeRequest\x1a\x1e.gitaly.RepositorySizeResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x63\n\x12\x41pplyGitattributes\x12!.gitaly.ApplyGitattributesRequest\x1a\".gitaly.ApplyGitattributesResponse\"\x06\xfa\x97(\x02\x08\x01\x12N\n\x0b\x46\x65tchRemote\x12\x1a.gitaly.FetchRemoteRequest\x1a\x1b.gitaly.FetchRemoteResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10\x43reateRepository\x12\x1f.gitaly.CreateRepositoryRequest\x1a .gitaly.CreateRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12M\n\nGetArchive\x12\x19.gitaly.GetArchiveRequest\x1a\x1a.gitaly.GetArchiveResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12]\n\x10HasLocalBranches\x12\x1f.gitaly.HasLocalBranchesRequest\x1a .gitaly.HasLocalBranchesResponse\"\x06\xfa\x97(\x02\x08\x02\x12`\n\x11\x46\x65tchSourceBranch\x12 .gitaly.FetchSourceBranchRequest\x1a!.gitaly.FetchSourceBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x39\n\x04\x46sck\x12\x13.gitaly.FsckRequest\x1a\x14.gitaly.FsckResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x45\n\x08WriteRef\x12\x17.gitaly.WriteRefRequest\x1a\x18.gitaly.WriteRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rFindMergeBase\x12\x1c.gitaly.FindMergeBaseRequest\x1a\x1d.gitaly.FindMergeBaseResponse\"\x06\xfa\x97(\x02\x08\x02\x12K\n\nCreateFork\x12\x19.gitaly.CreateForkRequest\x1a\x1a.gitaly.CreateForkResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x63\n\x12IsRebaseInProgress\x12!.gitaly.IsRebaseInProgressRequest\x1a\".gitaly.IsRebaseInProgressResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x63\n\x12IsSquashInProgress\x12!.gitaly.IsSquashInProgressRequest\x1a\".gitaly.IsSquashInProgressResponse\"\x06\xfa\x97(\x02\x08\x02\x12r\n\x17\x43reateRepositoryFromURL\x12&.gitaly.CreateRepositoryFromURLRequest\x1a\'.gitaly.CreateRepositoryFromURLResponse\"\x06\xfa\x97(\x02\x08\x01\x12S\n\x0c\x43reateBundle\x12\x1b.gitaly.CreateBundleRequest\x1a\x1c.gitaly.CreateBundleResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12}\n\x1a\x43reateRepositoryFromBundle\x12).gitaly.CreateRepositoryFromBundleRequest\x1a*.gitaly.CreateRepositoryFromBundleResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12H\n\tSetConfig\x12\x18.gitaly.SetConfigRequest\x1a\x19.gitaly.SetConfigResponse\"\x06\xfa\x97(\x02\x08\x01\x12Q\n\x0c\x44\x65leteConfig\x12\x1b.gitaly.DeleteConfigRequest\x1a\x1c.gitaly.DeleteConfigResponse\"\x06\xfa\x97(\x02\x08\x01\x12N\n\x0b\x46indLicense\x12\x1a.gitaly.FindLicenseRequest\x1a\x1b.gitaly.FindLicenseResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x62\n\x11GetInfoAttributes\x12 .gitaly.GetInfoAttributesRequest\x1a!.gitaly.GetInfoAttributesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12`\n\x11\x43\x61lculateChecksum\x12 .gitaly.CalculateChecksumRequest\x1a!.gitaly.CalculateChecksumResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x42\n\x07\x43leanup\x12\x16.gitaly.CleanupRequest\x1a\x17.gitaly.CleanupResponse\"\x06\xfa\x97(\x02\x08\x01\x12P\n\x0bGetSnapshot\x12\x1a.gitaly.GetSnapshotRequest\x1a\x1b.gitaly.GetSnapshotResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x81\x01\n\x1c\x43reateRepositoryFromSnapshot\x12+.gitaly.CreateRepositoryFromSnapshotRequest\x1a,.gitaly.CreateRepositoryFromSnapshotResponse\"\x06\xfa\x97(\x02\x08\x01\x12V\n\rGetRawChanges\x12\x1c.gitaly.GetRawChangesRequest\x1a\x1d.gitaly.GetRawChangesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12k\n\x14SearchFilesByContent\x12#.gitaly.SearchFilesByContentRequest\x1a$.gitaly.SearchFilesByContentResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x62\n\x11SearchFilesByName\x12 .gitaly.SearchFilesByNameRequest\x1a!.gitaly.SearchFilesByNameResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x65\n\x12RestoreCustomHooks\x12!.gitaly.RestoreCustomHooksRequest\x1a\".gitaly.RestoreCustomHooksResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12\x62\n\x11\x42\x61\x63kupCustomHooks\x12 .gitaly.BackupCustomHooksRequest\x1a!.gitaly.BackupCustomHooksResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12o\n\x16GetObjectDirectorySize\x12%.gitaly.GetObjectDirectorySizeRequest\x1a&.gitaly.GetObjectDirectorySizeResponse\"\x06\xfa\x97(\x02\x08\x02\x12T\n\rCloneFromPool\x12\x1c.gitaly.CloneFromPoolRequest\x1a\x1d.gitaly.CloneFromPoolResponse\"\x06\xfa\x97(\x02\x08\x01\x12l\n\x15\x43loneFromPoolInternal\x12$.gitaly.CloneFromPoolInternalRequest\x1a%.gitaly.CloneFromPoolInternalResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10RemoveRepository\x12\x1f.gitaly.RemoveRepositoryRequest\x1a .gitaly.RemoveRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10RenameRepository\x12\x1f.gitaly.RenameRepositoryRequest\x1a .gitaly.RenameRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x66\n\x13ReplicateRepository\x12\".gitaly.ReplicateRepositoryRequest\x1a#.gitaly.ReplicateRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x63\n\x12OptimizeRepository\x12!.gitaly.OptimizeRepositoryRequest\x1a\".gitaly.OptimizeRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
   ,
   dependencies=[lint__pb2.DESCRIPTOR,shared__pb2.DESCRIPTOR,])
 
 
 
 _GETARCHIVEREQUEST_FORMAT = _descriptor.EnumDescriptor(
   name='Format',
@@ -53,16 +53,16 @@
       name='TAR_BZ2', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1626,
-  serialized_end=1677,
+  serialized_start=1676,
+  serialized_end=1727,
 )
 _sym_db.RegisterEnumDescriptor(_GETARCHIVEREQUEST_FORMAT)
 
 _GETRAWCHANGESRESPONSE_RAWCHANGE_OPERATION = _descriptor.EnumDescriptor(
   name='Operation',
   full_name='gitaly.GetRawChangesResponse.RawChange.Operation',
   filename=None,
@@ -103,16 +103,16 @@
       name='TYPE_CHANGED', index=6, number=6,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=4898,
-  serialized_end=5003,
+  serialized_start=4948,
+  serialized_end=5053,
 )
 _sym_db.RegisterEnumDescriptor(_GETRAWCHANGESRESPONSE_RAWCHANGE_OPERATION)
 
 
 _REPOSITORYEXISTSREQUEST = _descriptor.Descriptor(
   name='RepositoryExistsRequest',
   full_name='gitaly.RepositoryExistsRequest',
@@ -735,53 +735,67 @@
     _descriptor.FieldDescriptor(
       name='remote_params', full_name='gitaly.FetchRemoteRequest.remote_params', index=8,
       number=10, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='check_tags_changed', full_name='gitaly.FetchRemoteRequest.check_tags_changed', index=9,
+      number=11, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1037,
-  serialized_end=1269,
+  serialized_end=1297,
 )
 
 
 _FETCHREMOTERESPONSE = _descriptor.Descriptor(
   name='FetchRemoteResponse',
   full_name='gitaly.FetchRemoteResponse',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
+    _descriptor.FieldDescriptor(
+      name='tags_changed', full_name='gitaly.FetchRemoteResponse.tags_changed', index=0,
+      number=1, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1271,
-  serialized_end=1292,
+  serialized_start=1299,
+  serialized_end=1342,
 )
 
 
 _CREATEREPOSITORYREQUEST = _descriptor.Descriptor(
   name='CreateRepositoryRequest',
   full_name='gitaly.CreateRepositoryRequest',
   filename=None,
@@ -804,16 +818,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1294,
-  serialized_end=1365,
+  serialized_start=1344,
+  serialized_end=1415,
 )
 
 
 _CREATEREPOSITORYRESPONSE = _descriptor.Descriptor(
   name='CreateRepositoryResponse',
   full_name='gitaly.CreateRepositoryResponse',
   filename=None,
@@ -829,16 +843,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1367,
-  serialized_end=1393,
+  serialized_start=1417,
+  serialized_end=1443,
 )
 
 
 _GETARCHIVEREQUEST = _descriptor.Descriptor(
   name='GetArchiveRequest',
   full_name='gitaly.GetArchiveRequest',
   filename=None,
@@ -911,16 +925,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1396,
-  serialized_end=1677,
+  serialized_start=1446,
+  serialized_end=1727,
 )
 
 
 _GETARCHIVERESPONSE = _descriptor.Descriptor(
   name='GetArchiveResponse',
   full_name='gitaly.GetArchiveResponse',
   filename=None,
@@ -943,16 +957,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1679,
-  serialized_end=1713,
+  serialized_start=1729,
+  serialized_end=1763,
 )
 
 
 _HASLOCALBRANCHESREQUEST = _descriptor.Descriptor(
   name='HasLocalBranchesRequest',
   full_name='gitaly.HasLocalBranchesRequest',
   filename=None,
@@ -975,16 +989,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1715,
-  serialized_end=1786,
+  serialized_start=1765,
+  serialized_end=1836,
 )
 
 
 _HASLOCALBRANCHESRESPONSE = _descriptor.Descriptor(
   name='HasLocalBranchesResponse',
   full_name='gitaly.HasLocalBranchesResponse',
   filename=None,
@@ -1007,16 +1021,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1788,
-  serialized_end=1829,
+  serialized_start=1838,
+  serialized_end=1879,
 )
 
 
 _FETCHSOURCEBRANCHREQUEST = _descriptor.Descriptor(
   name='FetchSourceBranchRequest',
   full_name='gitaly.FetchSourceBranchRequest',
   filename=None,
@@ -1060,16 +1074,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1832,
-  serialized_end=1994,
+  serialized_start=1882,
+  serialized_end=2044,
 )
 
 
 _FETCHSOURCEBRANCHRESPONSE = _descriptor.Descriptor(
   name='FetchSourceBranchResponse',
   full_name='gitaly.FetchSourceBranchResponse',
   filename=None,
@@ -1092,16 +1106,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1996,
-  serialized_end=2039,
+  serialized_start=2046,
+  serialized_end=2089,
 )
 
 
 _FSCKREQUEST = _descriptor.Descriptor(
   name='FsckRequest',
   full_name='gitaly.FsckRequest',
   filename=None,
@@ -1124,16 +1138,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2041,
-  serialized_end=2100,
+  serialized_start=2091,
+  serialized_end=2150,
 )
 
 
 _FSCKRESPONSE = _descriptor.Descriptor(
   name='FsckResponse',
   full_name='gitaly.FsckResponse',
   filename=None,
@@ -1156,16 +1170,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2102,
-  serialized_end=2131,
+  serialized_start=2152,
+  serialized_end=2181,
 )
 
 
 _WRITEREFREQUEST = _descriptor.Descriptor(
   name='WriteRefRequest',
   full_name='gitaly.WriteRefRequest',
   filename=None,
@@ -1216,16 +1230,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2134,
-  serialized_end=2271,
+  serialized_start=2184,
+  serialized_end=2321,
 )
 
 
 _WRITEREFRESPONSE = _descriptor.Descriptor(
   name='WriteRefResponse',
   full_name='gitaly.WriteRefResponse',
   filename=None,
@@ -1241,16 +1255,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2273,
-  serialized_end=2297,
+  serialized_start=2323,
+  serialized_end=2347,
 )
 
 
 _FINDMERGEBASEREQUEST = _descriptor.Descriptor(
   name='FindMergeBaseRequest',
   full_name='gitaly.FindMergeBaseRequest',
   filename=None,
@@ -1280,16 +1294,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2299,
-  serialized_end=2386,
+  serialized_start=2349,
+  serialized_end=2436,
 )
 
 
 _FINDMERGEBASERESPONSE = _descriptor.Descriptor(
   name='FindMergeBaseResponse',
   full_name='gitaly.FindMergeBaseResponse',
   filename=None,
@@ -1312,16 +1326,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2388,
-  serialized_end=2425,
+  serialized_start=2438,
+  serialized_end=2475,
 )
 
 
 _CREATEFORKREQUEST = _descriptor.Descriptor(
   name='CreateForkRequest',
   full_name='gitaly.CreateForkRequest',
   filename=None,
@@ -1351,16 +1365,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2427,
-  serialized_end=2539,
+  serialized_start=2477,
+  serialized_end=2589,
 )
 
 
 _CREATEFORKRESPONSE = _descriptor.Descriptor(
   name='CreateForkResponse',
   full_name='gitaly.CreateForkResponse',
   filename=None,
@@ -1376,16 +1390,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2541,
-  serialized_end=2561,
+  serialized_start=2591,
+  serialized_end=2611,
 )
 
 
 _ISREBASEINPROGRESSREQUEST = _descriptor.Descriptor(
   name='IsRebaseInProgressRequest',
   full_name='gitaly.IsRebaseInProgressRequest',
   filename=None,
@@ -1415,16 +1429,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2563,
-  serialized_end=2655,
+  serialized_start=2613,
+  serialized_end=2705,
 )
 
 
 _ISREBASEINPROGRESSRESPONSE = _descriptor.Descriptor(
   name='IsRebaseInProgressResponse',
   full_name='gitaly.IsRebaseInProgressResponse',
   filename=None,
@@ -1447,16 +1461,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2657,
-  serialized_end=2706,
+  serialized_start=2707,
+  serialized_end=2756,
 )
 
 
 _ISSQUASHINPROGRESSREQUEST = _descriptor.Descriptor(
   name='IsSquashInProgressRequest',
   full_name='gitaly.IsSquashInProgressRequest',
   filename=None,
@@ -1486,16 +1500,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2708,
-  serialized_end=2800,
+  serialized_start=2758,
+  serialized_end=2850,
 )
 
 
 _ISSQUASHINPROGRESSRESPONSE = _descriptor.Descriptor(
   name='IsSquashInProgressResponse',
   full_name='gitaly.IsSquashInProgressResponse',
   filename=None,
@@ -1518,16 +1532,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2802,
-  serialized_end=2851,
+  serialized_start=2852,
+  serialized_end=2901,
 )
 
 
 _CREATEREPOSITORYFROMURLREQUEST = _descriptor.Descriptor(
   name='CreateRepositoryFromURLRequest',
   full_name='gitaly.CreateRepositoryFromURLRequest',
   filename=None,
@@ -1557,16 +1571,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2853,
-  serialized_end=2944,
+  serialized_start=2903,
+  serialized_end=2994,
 )
 
 
 _CREATEREPOSITORYFROMURLRESPONSE = _descriptor.Descriptor(
   name='CreateRepositoryFromURLResponse',
   full_name='gitaly.CreateRepositoryFromURLResponse',
   filename=None,
@@ -1582,16 +1596,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2946,
-  serialized_end=2979,
+  serialized_start=2996,
+  serialized_end=3029,
 )
 
 
 _CREATEBUNDLEREQUEST = _descriptor.Descriptor(
   name='CreateBundleRequest',
   full_name='gitaly.CreateBundleRequest',
   filename=None,
@@ -1614,16 +1628,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2981,
-  serialized_end=3048,
+  serialized_start=3031,
+  serialized_end=3098,
 )
 
 
 _CREATEBUNDLERESPONSE = _descriptor.Descriptor(
   name='CreateBundleResponse',
   full_name='gitaly.CreateBundleResponse',
   filename=None,
@@ -1646,16 +1660,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3050,
-  serialized_end=3086,
+  serialized_start=3100,
+  serialized_end=3136,
 )
 
 
 _SETCONFIGREQUEST_ENTRY = _descriptor.Descriptor(
   name='Entry',
   full_name='gitaly.SetConfigRequest.Entry',
   filename=None,
@@ -1704,16 +1718,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='value', full_name='gitaly.SetConfigRequest.Entry.value',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3204,
-  serialized_end=3299,
+  serialized_start=3254,
+  serialized_end=3349,
 )
 
 _SETCONFIGREQUEST = _descriptor.Descriptor(
   name='SetConfigRequest',
   full_name='gitaly.SetConfigRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -1742,16 +1756,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3089,
-  serialized_end=3299,
+  serialized_start=3139,
+  serialized_end=3349,
 )
 
 
 _SETCONFIGRESPONSE = _descriptor.Descriptor(
   name='SetConfigResponse',
   full_name='gitaly.SetConfigResponse',
   filename=None,
@@ -1767,16 +1781,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3301,
-  serialized_end=3320,
+  serialized_start=3351,
+  serialized_end=3370,
 )
 
 
 _DELETECONFIGREQUEST = _descriptor.Descriptor(
   name='DeleteConfigRequest',
   full_name='gitaly.DeleteConfigRequest',
   filename=None,
@@ -1806,16 +1820,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3322,
-  serialized_end=3403,
+  serialized_start=3372,
+  serialized_end=3453,
 )
 
 
 _DELETECONFIGRESPONSE = _descriptor.Descriptor(
   name='DeleteConfigResponse',
   full_name='gitaly.DeleteConfigResponse',
   filename=None,
@@ -1831,16 +1845,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3405,
-  serialized_end=3427,
+  serialized_start=3455,
+  serialized_end=3477,
 )
 
 
 _RESTORECUSTOMHOOKSREQUEST = _descriptor.Descriptor(
   name='RestoreCustomHooksRequest',
   full_name='gitaly.RestoreCustomHooksRequest',
   filename=None,
@@ -1870,16 +1884,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3429,
-  serialized_end=3516,
+  serialized_start=3479,
+  serialized_end=3566,
 )
 
 
 _RESTORECUSTOMHOOKSRESPONSE = _descriptor.Descriptor(
   name='RestoreCustomHooksResponse',
   full_name='gitaly.RestoreCustomHooksResponse',
   filename=None,
@@ -1895,16 +1909,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3518,
-  serialized_end=3546,
+  serialized_start=3568,
+  serialized_end=3596,
 )
 
 
 _BACKUPCUSTOMHOOKSREQUEST = _descriptor.Descriptor(
   name='BackupCustomHooksRequest',
   full_name='gitaly.BackupCustomHooksRequest',
   filename=None,
@@ -1927,16 +1941,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3548,
-  serialized_end=3620,
+  serialized_start=3598,
+  serialized_end=3670,
 )
 
 
 _BACKUPCUSTOMHOOKSRESPONSE = _descriptor.Descriptor(
   name='BackupCustomHooksResponse',
   full_name='gitaly.BackupCustomHooksResponse',
   filename=None,
@@ -1959,16 +1973,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3622,
-  serialized_end=3663,
+  serialized_start=3672,
+  serialized_end=3713,
 )
 
 
 _CREATEREPOSITORYFROMBUNDLEREQUEST = _descriptor.Descriptor(
   name='CreateRepositoryFromBundleRequest',
   full_name='gitaly.CreateRepositoryFromBundleRequest',
   filename=None,
@@ -1998,16 +2012,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3665,
-  serialized_end=3760,
+  serialized_start=3715,
+  serialized_end=3810,
 )
 
 
 _CREATEREPOSITORYFROMBUNDLERESPONSE = _descriptor.Descriptor(
   name='CreateRepositoryFromBundleResponse',
   full_name='gitaly.CreateRepositoryFromBundleResponse',
   filename=None,
@@ -2023,16 +2037,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3762,
-  serialized_end=3798,
+  serialized_start=3812,
+  serialized_end=3848,
 )
 
 
 _FINDLICENSEREQUEST = _descriptor.Descriptor(
   name='FindLicenseRequest',
   full_name='gitaly.FindLicenseRequest',
   filename=None,
@@ -2055,16 +2069,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3800,
-  serialized_end=3866,
+  serialized_start=3850,
+  serialized_end=3916,
 )
 
 
 _FINDLICENSERESPONSE = _descriptor.Descriptor(
   name='FindLicenseResponse',
   full_name='gitaly.FindLicenseResponse',
   filename=None,
@@ -2087,16 +2101,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3868,
-  serialized_end=3917,
+  serialized_start=3918,
+  serialized_end=3967,
 )
 
 
 _GETINFOATTRIBUTESREQUEST = _descriptor.Descriptor(
   name='GetInfoAttributesRequest',
   full_name='gitaly.GetInfoAttributesRequest',
   filename=None,
@@ -2119,16 +2133,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3919,
-  serialized_end=3991,
+  serialized_start=3969,
+  serialized_end=4041,
 )
 
 
 _GETINFOATTRIBUTESRESPONSE = _descriptor.Descriptor(
   name='GetInfoAttributesResponse',
   full_name='gitaly.GetInfoAttributesResponse',
   filename=None,
@@ -2151,16 +2165,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3993,
-  serialized_end=4040,
+  serialized_start=4043,
+  serialized_end=4090,
 )
 
 
 _CALCULATECHECKSUMREQUEST = _descriptor.Descriptor(
   name='CalculateChecksumRequest',
   full_name='gitaly.CalculateChecksumRequest',
   filename=None,
@@ -2183,16 +2197,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4042,
-  serialized_end=4114,
+  serialized_start=4092,
+  serialized_end=4164,
 )
 
 
 _CALCULATECHECKSUMRESPONSE = _descriptor.Descriptor(
   name='CalculateChecksumResponse',
   full_name='gitaly.CalculateChecksumResponse',
   filename=None,
@@ -2215,16 +2229,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4116,
-  serialized_end=4161,
+  serialized_start=4166,
+  serialized_end=4211,
 )
 
 
 _GETSNAPSHOTREQUEST = _descriptor.Descriptor(
   name='GetSnapshotRequest',
   full_name='gitaly.GetSnapshotRequest',
   filename=None,
@@ -2247,16 +2261,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4163,
-  serialized_end=4229,
+  serialized_start=4213,
+  serialized_end=4279,
 )
 
 
 _GETSNAPSHOTRESPONSE = _descriptor.Descriptor(
   name='GetSnapshotResponse',
   full_name='gitaly.GetSnapshotResponse',
   filename=None,
@@ -2279,16 +2293,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4231,
-  serialized_end=4266,
+  serialized_start=4281,
+  serialized_end=4316,
 )
 
 
 _CREATEREPOSITORYFROMSNAPSHOTREQUEST = _descriptor.Descriptor(
   name='CreateRepositoryFromSnapshotRequest',
   full_name='gitaly.CreateRepositoryFromSnapshotRequest',
   filename=None,
@@ -2325,16 +2339,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4268,
-  serialized_end=4388,
+  serialized_start=4318,
+  serialized_end=4438,
 )
 
 
 _CREATEREPOSITORYFROMSNAPSHOTRESPONSE = _descriptor.Descriptor(
   name='CreateRepositoryFromSnapshotResponse',
   full_name='gitaly.CreateRepositoryFromSnapshotResponse',
   filename=None,
@@ -2350,16 +2364,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4390,
-  serialized_end=4428,
+  serialized_start=4440,
+  serialized_end=4478,
 )
 
 
 _GETRAWCHANGESREQUEST = _descriptor.Descriptor(
   name='GetRawChangesRequest',
   full_name='gitaly.GetRawChangesRequest',
   filename=None,
@@ -2396,16 +2410,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4430,
-  serialized_end=4542,
+  serialized_start=4480,
+  serialized_end=4592,
 )
 
 
 _GETRAWCHANGESRESPONSE_RAWCHANGE = _descriptor.Descriptor(
   name='RawChange',
   full_name='gitaly.GetRawChangesResponse.RawChange',
   filename=None,
@@ -2492,16 +2506,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4633,
-  serialized_end=5003,
+  serialized_start=4683,
+  serialized_end=5053,
 )
 
 _GETRAWCHANGESRESPONSE = _descriptor.Descriptor(
   name='GetRawChangesResponse',
   full_name='gitaly.GetRawChangesResponse',
   filename=None,
   file=DESCRIPTOR,
@@ -2523,16 +2537,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4545,
-  serialized_end=5003,
+  serialized_start=4595,
+  serialized_end=5053,
 )
 
 
 _SEARCHFILESBYNAMEREQUEST = _descriptor.Descriptor(
   name='SearchFilesByNameRequest',
   full_name='gitaly.SearchFilesByNameRequest',
   filename=None,
@@ -2576,16 +2590,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5005,
-  serialized_end=5121,
+  serialized_start=5055,
+  serialized_end=5171,
 )
 
 
 _SEARCHFILESBYNAMERESPONSE = _descriptor.Descriptor(
   name='SearchFilesByNameResponse',
   full_name='gitaly.SearchFilesByNameResponse',
   filename=None,
@@ -2608,16 +2622,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5123,
-  serialized_end=5165,
+  serialized_start=5173,
+  serialized_end=5215,
 )
 
 
 _SEARCHFILESBYCONTENTREQUEST = _descriptor.Descriptor(
   name='SearchFilesByContentRequest',
   full_name='gitaly.SearchFilesByContentRequest',
   filename=None,
@@ -2661,16 +2675,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5168,
-  serialized_end=5297,
+  serialized_start=5218,
+  serialized_end=5347,
 )
 
 
 _SEARCHFILESBYCONTENTRESPONSE = _descriptor.Descriptor(
   name='SearchFilesByContentResponse',
   full_name='gitaly.SearchFilesByContentResponse',
   filename=None,
@@ -2707,16 +2721,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5299,
-  serialized_end=5388,
+  serialized_start=5349,
+  serialized_end=5438,
 )
 
 
 _REMOTE = _descriptor.Descriptor(
   name='Remote',
   full_name='gitaly.Remote',
   filename=None,
@@ -2760,16 +2774,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5390,
-  serialized_end=5484,
+  serialized_start=5440,
+  serialized_end=5534,
 )
 
 
 _GETOBJECTDIRECTORYSIZEREQUEST = _descriptor.Descriptor(
   name='GetObjectDirectorySizeRequest',
   full_name='gitaly.GetObjectDirectorySizeRequest',
   filename=None,
@@ -2792,16 +2806,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5486,
-  serialized_end=5563,
+  serialized_start=5536,
+  serialized_end=5613,
 )
 
 
 _GETOBJECTDIRECTORYSIZERESPONSE = _descriptor.Descriptor(
   name='GetObjectDirectorySizeResponse',
   full_name='gitaly.GetObjectDirectorySizeResponse',
   filename=None,
@@ -2824,16 +2838,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5565,
-  serialized_end=5611,
+  serialized_start=5615,
+  serialized_end=5661,
 )
 
 
 _CLONEFROMPOOLREQUEST = _descriptor.Descriptor(
   name='CloneFromPoolRequest',
   full_name='gitaly.CloneFromPoolRequest',
   filename=None,
@@ -2870,16 +2884,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5614,
-  serialized_end=5748,
+  serialized_start=5664,
+  serialized_end=5798,
 )
 
 
 _CLONEFROMPOOLRESPONSE = _descriptor.Descriptor(
   name='CloneFromPoolResponse',
   full_name='gitaly.CloneFromPoolResponse',
   filename=None,
@@ -2895,16 +2909,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5750,
-  serialized_end=5773,
+  serialized_start=5800,
+  serialized_end=5823,
 )
 
 
 _CLONEFROMPOOLINTERNALREQUEST = _descriptor.Descriptor(
   name='CloneFromPoolInternalRequest',
   full_name='gitaly.CloneFromPoolInternalRequest',
   filename=None,
@@ -2941,16 +2955,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5776,
-  serialized_end=5933,
+  serialized_start=5826,
+  serialized_end=5983,
 )
 
 
 _CLONEFROMPOOLINTERNALRESPONSE = _descriptor.Descriptor(
   name='CloneFromPoolInternalResponse',
   full_name='gitaly.CloneFromPoolInternalResponse',
   filename=None,
@@ -2966,16 +2980,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5935,
-  serialized_end=5966,
+  serialized_start=5985,
+  serialized_end=6016,
 )
 
 
 _REMOVEREPOSITORYREQUEST = _descriptor.Descriptor(
   name='RemoveRepositoryRequest',
   full_name='gitaly.RemoveRepositoryRequest',
   filename=None,
@@ -2998,16 +3012,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5968,
-  serialized_end=6039,
+  serialized_start=6018,
+  serialized_end=6089,
 )
 
 
 _REMOVEREPOSITORYRESPONSE = _descriptor.Descriptor(
   name='RemoveRepositoryResponse',
   full_name='gitaly.RemoveRepositoryResponse',
   filename=None,
@@ -3023,16 +3037,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6041,
-  serialized_end=6067,
+  serialized_start=6091,
+  serialized_end=6117,
 )
 
 
 _RENAMEREPOSITORYREQUEST = _descriptor.Descriptor(
   name='RenameRepositoryRequest',
   full_name='gitaly.RenameRepositoryRequest',
   filename=None,
@@ -3062,16 +3076,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6069,
-  serialized_end=6163,
+  serialized_start=6119,
+  serialized_end=6213,
 )
 
 
 _RENAMEREPOSITORYRESPONSE = _descriptor.Descriptor(
   name='RenameRepositoryResponse',
   full_name='gitaly.RenameRepositoryResponse',
   filename=None,
@@ -3087,16 +3101,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6165,
-  serialized_end=6191,
+  serialized_start=6215,
+  serialized_end=6241,
 )
 
 
 _REPLICATEREPOSITORYREQUEST = _descriptor.Descriptor(
   name='ReplicateRepositoryRequest',
   full_name='gitaly.ReplicateRepositoryRequest',
   filename=None,
@@ -3126,16 +3140,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6193,
-  serialized_end=6303,
+  serialized_start=6243,
+  serialized_end=6353,
 )
 
 
 _REPLICATEREPOSITORYRESPONSE = _descriptor.Descriptor(
   name='ReplicateRepositoryResponse',
   full_name='gitaly.ReplicateRepositoryResponse',
   filename=None,
@@ -3151,16 +3165,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6305,
-  serialized_end=6334,
+  serialized_start=6355,
+  serialized_end=6384,
 )
 
 
 _OPTIMIZEREPOSITORYREQUEST = _descriptor.Descriptor(
   name='OptimizeRepositoryRequest',
   full_name='gitaly.OptimizeRepositoryRequest',
   filename=None,
@@ -3183,16 +3197,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6336,
-  serialized_end=6409,
+  serialized_start=6386,
+  serialized_end=6459,
 )
 
 
 _OPTIMIZEREPOSITORYRESPONSE = _descriptor.Descriptor(
   name='OptimizeRepositoryResponse',
   full_name='gitaly.OptimizeRepositoryResponse',
   filename=None,
@@ -3208,16 +3222,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6411,
-  serialized_end=6439,
+  serialized_start=6461,
+  serialized_end=6489,
 )
 
 _REPOSITORYEXISTSREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _REPACKINCREMENTALREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _REPACKFULLREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _MIDXREPACKREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
 _GARBAGECOLLECTREQUEST.fields_by_name['repository'].message_type = shared__pb2._REPOSITORY
@@ -4031,16 +4045,16 @@
 _REPOSITORYSERVICE = _descriptor.ServiceDescriptor(
   name='RepositoryService',
   full_name='gitaly.RepositoryService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=6442,
-  serialized_end=10373,
+  serialized_start=6492,
+  serialized_end=10423,
   methods=[
   _descriptor.MethodDescriptor(
     name='RepositoryExists',
     full_name='gitaly.RepositoryService.RepositoryExists',
     index=0,
     containing_service=None,
     input_type=_REPOSITORYEXISTSREQUEST,
```

### Comparing `hgitaly-0.8.1/hgitaly/stub/repository_service_pb2_grpc.py` & `hgitaly-0.9.0/hgitaly/stub/repository_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,17 @@
     def ApplyGitattributes(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def FetchRemote(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """FetchRemote fetches references from a remote repository into the local
+        repository.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateRepository(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -298,15 +300,17 @@
     def HasLocalBranches(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def FetchSourceBranch(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """FetchSourceBranch fetches a branch from a second (potentially remote)
+        repository into the given repository.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Fsck(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
```

### Comparing `hgitaly-0.8.1/hgitaly/stub/shared_pb2.py` & `hgitaly-0.9.0/hgitaly/stub/shared_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='shared.proto',
   package='gitaly',
   syntax='proto3',
   serialized_options=b'Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypb',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0cshared.proto\x12\x06gitaly\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\nlint.proto\"\xc3\x01\n\nRepository\x12\x14\n\x0cstorage_name\x18\x02 \x01(\t\x12\x15\n\rrelative_path\x18\x03 \x01(\t\x12\x1c\n\x14git_object_directory\x18\x04 \x01(\t\x12(\n git_alternate_object_directories\x18\x05 \x03(\t\x12\x15\n\rgl_repository\x18\x06 \x01(\t\x12\x17\n\x0fgl_project_path\x18\x08 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x07\x10\x08R\x04path\"\xec\x01\n\tGitCommit\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\x0c\x12\x0c\n\x04\x62ody\x18\x03 \x01(\x0c\x12$\n\x06\x61uthor\x18\x04 \x01(\x0b\x32\x14.gitaly.CommitAuthor\x12\'\n\tcommitter\x18\x05 \x01(\x0b\x32\x14.gitaly.CommitAuthor\x12\x12\n\nparent_ids\x18\x06 \x03(\t\x12\x11\n\tbody_size\x18\x07 \x01(\x03\x12-\n\x0esignature_type\x18\x08 \x01(\x0e\x32\x15.gitaly.SignatureType\x12\x0f\n\x07tree_id\x18\t \x01(\t\"g\n\x0c\x43ommitAuthor\x12\x0c\n\x04name\x18\x01 \x01(\x0c\x12\r\n\x05\x65mail\x18\x02 \x01(\x0c\x12(\n\x04\x64\x61te\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x04 \x01(\x0c\"\x1b\n\nExitStatus\x12\r\n\x05value\x18\x01 \x01(\x05\"@\n\x06\x42ranch\x12\x0c\n\x04name\x18\x01 \x01(\x0c\x12(\n\rtarget_commit\x18\x02 \x01(\x0b\x32\x11.gitaly.GitCommit\"\xc5\x01\n\x03Tag\x12\x0c\n\x04name\x18\x01 \x01(\x0c\x12\n\n\x02id\x18\x02 \x01(\t\x12(\n\rtarget_commit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x0f\n\x07message\x18\x04 \x01(\x0c\x12\x14\n\x0cmessage_size\x18\x05 \x01(\x03\x12$\n\x06tagger\x18\x06 \x01(\x0b\x32\x14.gitaly.CommitAuthor\x12-\n\x0esignature_type\x18\x07 \x01(\x0e\x32\x15.gitaly.SignatureType\"G\n\x04User\x12\r\n\x05gl_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\x0c\x12\r\n\x05\x65mail\x18\x03 \x01(\x0c\x12\x13\n\x0bgl_username\x18\x04 \x01(\t\":\n\nObjectPool\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x90\xc6,\x01\"8\n\x13PaginationParameter\x12\x12\n\npage_token\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\x05\"*\n\rGlobalOptions\x12\x19\n\x11literal_pathspecs\x18\x01 \x01(\x08*B\n\nObjectType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x43OMMIT\x10\x01\x12\x08\n\x04\x42LOB\x10\x02\x12\x08\n\x04TREE\x10\x03\x12\x07\n\x03TAG\x10\x04*,\n\rSignatureType\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03PGP\x10\x01\x12\x08\n\x04X509\x10\x02\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
+  serialized_pb=b'\n\x0cshared.proto\x12\x06gitaly\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\nlint.proto\"\xc3\x01\n\nRepository\x12\x14\n\x0cstorage_name\x18\x02 \x01(\t\x12\x15\n\rrelative_path\x18\x03 \x01(\t\x12\x1c\n\x14git_object_directory\x18\x04 \x01(\t\x12(\n git_alternate_object_directories\x18\x05 \x03(\t\x12\x15\n\rgl_repository\x18\x06 \x01(\t\x12\x17\n\x0fgl_project_path\x18\x08 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x07\x10\x08R\x04path\"+\n\rCommitTrailer\x12\x0b\n\x03key\x18\x01 \x01(\x0c\x12\r\n\x05value\x18\x02 \x01(\x0c\"\x95\x02\n\tGitCommit\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\x0c\x12\x0c\n\x04\x62ody\x18\x03 \x01(\x0c\x12$\n\x06\x61uthor\x18\x04 \x01(\x0b\x32\x14.gitaly.CommitAuthor\x12\'\n\tcommitter\x18\x05 \x01(\x0b\x32\x14.gitaly.CommitAuthor\x12\x12\n\nparent_ids\x18\x06 \x03(\t\x12\x11\n\tbody_size\x18\x07 \x01(\x03\x12-\n\x0esignature_type\x18\x08 \x01(\x0e\x32\x15.gitaly.SignatureType\x12\x0f\n\x07tree_id\x18\t \x01(\t\x12\'\n\x08trailers\x18\n \x03(\x0b\x32\x15.gitaly.CommitTrailer\"g\n\x0c\x43ommitAuthor\x12\x0c\n\x04name\x18\x01 \x01(\x0c\x12\r\n\x05\x65mail\x18\x02 \x01(\x0c\x12(\n\x04\x64\x61te\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x04 \x01(\x0c\"\x1b\n\nExitStatus\x12\r\n\x05value\x18\x01 \x01(\x05\"@\n\x06\x42ranch\x12\x0c\n\x04name\x18\x01 \x01(\x0c\x12(\n\rtarget_commit\x18\x02 \x01(\x0b\x32\x11.gitaly.GitCommit\"\xc5\x01\n\x03Tag\x12\x0c\n\x04name\x18\x01 \x01(\x0c\x12\n\n\x02id\x18\x02 \x01(\t\x12(\n\rtarget_commit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x0f\n\x07message\x18\x04 \x01(\x0c\x12\x14\n\x0cmessage_size\x18\x05 \x01(\x03\x12$\n\x06tagger\x18\x06 \x01(\x0b\x32\x14.gitaly.CommitAuthor\x12-\n\x0esignature_type\x18\x07 \x01(\x0e\x32\x15.gitaly.SignatureType\"G\n\x04User\x12\r\n\x05gl_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\x0c\x12\r\n\x05\x65mail\x18\x03 \x01(\x0c\x12\x13\n\x0bgl_username\x18\x04 \x01(\t\":\n\nObjectPool\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x90\xc6,\x01\"8\n\x13PaginationParameter\x12\x12\n\npage_token\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\x05\"*\n\rGlobalOptions\x12\x19\n\x11literal_pathspecs\x18\x01 \x01(\x08*B\n\nObjectType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x43OMMIT\x10\x01\x12\x08\n\x04\x42LOB\x10\x02\x12\x08\n\x04TREE\x10\x03\x12\x07\n\x03TAG\x10\x04*,\n\rSignatureType\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03PGP\x10\x01\x12\x08\n\x04X509\x10\x02\x42\x30Z.gitlab.com/gitlab-org/gitaly/proto/go/gitalypbb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,lint__pb2.DESCRIPTOR,])
 
 _OBJECTTYPE = _descriptor.EnumDescriptor(
   name='ObjectType',
   full_name='gitaly.ObjectType',
   filename=None,
@@ -57,16 +57,16 @@
       name='TAG', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1141,
-  serialized_end=1207,
+  serialized_start=1227,
+  serialized_end=1293,
 )
 _sym_db.RegisterEnumDescriptor(_OBJECTTYPE)
 
 ObjectType = enum_type_wrapper.EnumTypeWrapper(_OBJECTTYPE)
 _SIGNATURETYPE = _descriptor.EnumDescriptor(
   name='SignatureType',
   full_name='gitaly.SignatureType',
@@ -88,16 +88,16 @@
       name='X509', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1209,
-  serialized_end=1253,
+  serialized_start=1295,
+  serialized_end=1339,
 )
 _sym_db.RegisterEnumDescriptor(_SIGNATURETYPE)
 
 SignatureType = enum_type_wrapper.EnumTypeWrapper(_SIGNATURETYPE)
 UNKNOWN = 0
 COMMIT = 1
 BLOB = 2
@@ -172,14 +172,53 @@
   oneofs=[
   ],
   serialized_start=70,
   serialized_end=265,
 )
 
 
+_COMMITTRAILER = _descriptor.Descriptor(
+  name='CommitTrailer',
+  full_name='gitaly.CommitTrailer',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='gitaly.CommitTrailer.key', index=0,
+      number=1, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='gitaly.CommitTrailer.value', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=267,
+  serialized_end=310,
+)
+
+
 _GITCOMMIT = _descriptor.Descriptor(
   name='GitCommit',
   full_name='gitaly.GitCommit',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -243,28 +282,35 @@
     _descriptor.FieldDescriptor(
       name='tree_id', full_name='gitaly.GitCommit.tree_id', index=8,
       number=9, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='trailers', full_name='gitaly.GitCommit.trailers', index=9,
+      number=10, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=268,
-  serialized_end=504,
+  serialized_start=313,
+  serialized_end=590,
 )
 
 
 _COMMITAUTHOR = _descriptor.Descriptor(
   name='CommitAuthor',
   full_name='gitaly.CommitAuthor',
   filename=None,
@@ -308,16 +354,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=506,
-  serialized_end=609,
+  serialized_start=592,
+  serialized_end=695,
 )
 
 
 _EXITSTATUS = _descriptor.Descriptor(
   name='ExitStatus',
   full_name='gitaly.ExitStatus',
   filename=None,
@@ -340,16 +386,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=611,
-  serialized_end=638,
+  serialized_start=697,
+  serialized_end=724,
 )
 
 
 _BRANCH = _descriptor.Descriptor(
   name='Branch',
   full_name='gitaly.Branch',
   filename=None,
@@ -379,16 +425,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=640,
-  serialized_end=704,
+  serialized_start=726,
+  serialized_end=790,
 )
 
 
 _TAG = _descriptor.Descriptor(
   name='Tag',
   full_name='gitaly.Tag',
   filename=None,
@@ -453,16 +499,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=707,
-  serialized_end=904,
+  serialized_start=793,
+  serialized_end=990,
 )
 
 
 _USER = _descriptor.Descriptor(
   name='User',
   full_name='gitaly.User',
   filename=None,
@@ -506,16 +552,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=906,
-  serialized_end=977,
+  serialized_start=992,
+  serialized_end=1063,
 )
 
 
 _OBJECTPOOL = _descriptor.Descriptor(
   name='ObjectPool',
   full_name='gitaly.ObjectPool',
   filename=None,
@@ -538,16 +584,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=979,
-  serialized_end=1037,
+  serialized_start=1065,
+  serialized_end=1123,
 )
 
 
 _PAGINATIONPARAMETER = _descriptor.Descriptor(
   name='PaginationParameter',
   full_name='gitaly.PaginationParameter',
   filename=None,
@@ -577,16 +623,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1039,
-  serialized_end=1095,
+  serialized_start=1125,
+  serialized_end=1181,
 )
 
 
 _GLOBALOPTIONS = _descriptor.Descriptor(
   name='GlobalOptions',
   full_name='gitaly.GlobalOptions',
   filename=None,
@@ -609,28 +655,30 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1097,
-  serialized_end=1139,
+  serialized_start=1183,
+  serialized_end=1225,
 )
 
 _GITCOMMIT.fields_by_name['author'].message_type = _COMMITAUTHOR
 _GITCOMMIT.fields_by_name['committer'].message_type = _COMMITAUTHOR
 _GITCOMMIT.fields_by_name['signature_type'].enum_type = _SIGNATURETYPE
+_GITCOMMIT.fields_by_name['trailers'].message_type = _COMMITTRAILER
 _COMMITAUTHOR.fields_by_name['date'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _BRANCH.fields_by_name['target_commit'].message_type = _GITCOMMIT
 _TAG.fields_by_name['target_commit'].message_type = _GITCOMMIT
 _TAG.fields_by_name['tagger'].message_type = _COMMITAUTHOR
 _TAG.fields_by_name['signature_type'].enum_type = _SIGNATURETYPE
 _OBJECTPOOL.fields_by_name['repository'].message_type = _REPOSITORY
 DESCRIPTOR.message_types_by_name['Repository'] = _REPOSITORY
+DESCRIPTOR.message_types_by_name['CommitTrailer'] = _COMMITTRAILER
 DESCRIPTOR.message_types_by_name['GitCommit'] = _GITCOMMIT
 DESCRIPTOR.message_types_by_name['CommitAuthor'] = _COMMITAUTHOR
 DESCRIPTOR.message_types_by_name['ExitStatus'] = _EXITSTATUS
 DESCRIPTOR.message_types_by_name['Branch'] = _BRANCH
 DESCRIPTOR.message_types_by_name['Tag'] = _TAG
 DESCRIPTOR.message_types_by_name['User'] = _USER
 DESCRIPTOR.message_types_by_name['ObjectPool'] = _OBJECTPOOL
@@ -643,14 +691,21 @@
 Repository = _reflection.GeneratedProtocolMessageType('Repository', (_message.Message,), {
   'DESCRIPTOR' : _REPOSITORY,
   '__module__' : 'shared_pb2'
   # @@protoc_insertion_point(class_scope:gitaly.Repository)
   })
 _sym_db.RegisterMessage(Repository)
 
+CommitTrailer = _reflection.GeneratedProtocolMessageType('CommitTrailer', (_message.Message,), {
+  'DESCRIPTOR' : _COMMITTRAILER,
+  '__module__' : 'shared_pb2'
+  # @@protoc_insertion_point(class_scope:gitaly.CommitTrailer)
+  })
+_sym_db.RegisterMessage(CommitTrailer)
+
 GitCommit = _reflection.GeneratedProtocolMessageType('GitCommit', (_message.Message,), {
   'DESCRIPTOR' : _GITCOMMIT,
   '__module__' : 'shared_pb2'
   # @@protoc_insertion_point(class_scope:gitaly.GitCommit)
   })
 _sym_db.RegisterMessage(GitCommit)
```

### Comparing `hgitaly-0.8.1/hgitaly/tests/common.py` & `hgitaly-0.9.0/hgitaly/tests/common.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/tests/test_branch.py` & `hgitaly-0.9.0/hgitaly/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/tests/test_errors.py` & `hgitaly-0.9.0/hgitaly/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/tests/test_messages.py` & `hgitaly-0.9.0/hgitaly/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/tests/test_revision.py` & `hgitaly-0.9.0/hgitaly/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/tests/test_server.py` & `hgitaly-0.9.0/hgitaly/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/tests/test_servicer.py` & `hgitaly-0.9.0/hgitaly/tests/test_servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly/util.py` & `hgitaly-0.9.0/hgitaly/util.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/hgitaly.egg-info/PKG-INFO` & `hgitaly-0.9.0/hgitaly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgitaly
-Version: 0.8.1
+Version: 0.9.0
 Summary: Server-side implementation of Gitaly protocol for Mercurial
 Home-page: https://foss.heptapod.net/heptapod/hgitaly
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Description: # HGitaly
```

### Comparing `hgitaly-0.8.1/hgitaly.egg-info/SOURCES.txt` & `hgitaly-0.9.0/hgitaly.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 hgext3rd/__init__.py
 hgext3rd/hgitaly/__init__.py
 hgext3rd/hgitaly/tests/__init__.py
 hgext3rd/hgitaly/tests/test_serve.py
 hgitaly/__init__.py
 hgitaly/branch.py
 hgitaly/errors.py
+hgitaly/git.py
 hgitaly/message.py
+hgitaly/oid.py
 hgitaly/path.py
 hgitaly/revision.py
 hgitaly/server.py
 hgitaly/servicer.py
 hgitaly/stream.py
 hgitaly/tag.py
 hgitaly/util.py
@@ -26,14 +28,15 @@
 hgitaly/service/commit.py
 hgitaly/service/diff.py
 hgitaly/service/ref.py
 hgitaly/service/repository_service.py
 hgitaly/service/tests/__init__.py
 hgitaly/service/tests/test_commit.py
 hgitaly/service/tests/test_default_branch.py
+hgitaly/service/tests/test_diff.py
 hgitaly/service/tests/test_ref.py
 hgitaly/service/tests/test_repository_service.py
 hgitaly/stub/__init__.py
 hgitaly/stub/blob_pb2.py
 hgitaly/stub/blob_pb2_grpc.py
 hgitaly/stub/commit_pb2.py
 hgitaly/stub/commit_pb2_grpc.py
@@ -48,17 +51,19 @@
 hgitaly/stub/shared_pb2.py
 hgitaly/stub/shared_pb2_grpc.py
 hgitaly/tests/__init__.py
 hgitaly/tests/common.py
 hgitaly/tests/test_branch.py
 hgitaly/tests/test_errors.py
 hgitaly/tests/test_messages.py
+hgitaly/tests/test_oid.py
 hgitaly/tests/test_revision.py
 hgitaly/tests/test_server.py
 hgitaly/tests/test_servicer.py
 hgitaly/tests/test_stream.py
 tests_with_gitaly/__init__.py
 tests_with_gitaly/comparison.py
 tests_with_gitaly/conftest.py
 tests_with_gitaly/gitaly.py
+tests_with_gitaly/test_diff.py
 tests_with_gitaly/test_gitaly_server.py
 tests_with_gitaly/test_ref.py
```

### Comparing `hgitaly-0.8.1/setup.py` & `hgitaly-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('install-requirements.txt', 'r') as install_reqf:
     install_req = [req.strip() for req in install_reqf]
 
 setup(
     name='hgitaly',
-    version='0.8.1',
+    version='0.9.0',
     author='Georges Racinet',
     author_email='georges.racinet@octobus.net',
     url='https://foss.heptapod.net/heptapod/hgitaly',
     description="Server-side implementation of Gitaly protocol for Mercurial",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     keywords='hg mercurial heptapod gitlab',
```

### Comparing `hgitaly-0.8.1/tests_with_gitaly/comparison.py` & `hgitaly-0.9.0/tests_with_gitaly/comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/tests_with_gitaly/conftest.py` & `hgitaly-0.9.0/tests_with_gitaly/conftest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/tests_with_gitaly/gitaly.py` & `hgitaly-0.9.0/tests_with_gitaly/gitaly.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 from hgitaly.stub.repository_service_pb2 import RepositoryExistsRequest
 from hgitaly.stub.shared_pb2 import Repository
 from hgitaly.stub.repository_service_pb2_grpc import RepositoryServiceStub
 
 from . import GITALY_INSTALL_DIR
 
 
-def wait_gitaly_accepts_connection(gitaly_channel):
+def wait_gitaly_accepts_connection(gitaly_channel, timeout=5):
     """Wait for the Gitaly server to accept connections.
 
     wait for server to start enough that the address in bound
     Then the `wait_for_ready` optionis there to ensure full readiness, but
     the client must at least receive something, e.g., the `CONNECTING` status
     for that to work.
     """
     repo_stub = RepositoryServiceStub(gitaly_channel)
     repo_stub.RepositoryExists(
         RepositoryExistsRequest(
             repository=Repository(
                 relative_path="we/dont/care/waiting/for/any/connection",
                 storage_name="default")
         ),
+        timeout=timeout,
         wait_for_ready=True
     )
 
 
 @attr.s
 class GitalyServer:
     home_dir = attr.ib()
@@ -69,21 +70,22 @@
 
     @contextmanager
     def start(self):
         self.configure()
 
         env = dict(os.environ)
         env['GITALY_TESTING_NO_GIT_HOOKS'] = "1"
+        timeout = int(env.pop('GITALY_STARTUP_TIMEOUT', '5').strip())
 
         # Note: Python 3.8 does not need the conversions to str, but it's
         # handy to support Python 3.7 (Debian buster in CI)
         gitaly = subprocess.Popen([str(GITALY_INSTALL_DIR / 'gitaly'),
                                    str(self.gitaly_conf)],
                                   env=env)
 
         with grpc.insecure_channel('unix:' + str(self.gitaly_socket),
                                    ) as gitaly_channel:
-            wait_gitaly_accepts_connection(gitaly_channel)
+            wait_gitaly_accepts_connection(gitaly_channel, timeout=timeout)
             yield gitaly_channel
 
         gitaly.terminate()
         gitaly.wait()
```

### Comparing `hgitaly-0.8.1/tests_with_gitaly/test_gitaly_server.py` & `hgitaly-0.9.0/tests_with_gitaly/test_gitaly_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-0.8.1/tests_with_gitaly/test_ref.py` & `hgitaly-0.9.0/tests_with_gitaly/test_ref.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,14 @@
 
 from . import gitaly_not_installed
 if gitaly_not_installed():  # pragma no cover
     pytestmark = pytest.mark.skip
 
 
 def test_compare_find_branch(gitaly_comparison):
-    """In this test we use Heptapod's GitLab mirror to write the Git repo.
-
-    Lots of duplication from py-heptapod tests and setup reuse from
-    other HGitaly tests feels weird because asymetrical, but it makes the
-    point.
-
-    We don't need to pre-create the Git repo, because GitLab mirror will
-    do it automatically.
-    """
     fixture = gitaly_comparison
     hgitaly_repo = fixture.hgitaly_repo
     gitaly_repo = fixture.gitaly_repo
     git_repo = fixture.git_repo
 
     fixture.hg_repo_wrapper.write_commit('foo', message="Some foo")
```

