# Comparing `tmp/nics-1.0.0rc9.tar.gz` & `tmp/nics-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-6dn_qnr6/nics-1.0.0rc9.tar", last modified: Thu Jun 29 21:12:50 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-zi7w0cc3/nics-2.0.0.tar", last modified: Fri Jun 30 15:28:43 2023, max compression
```

## Comparing `nics-1.0.0rc9.tar` & `nics-2.0.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 21:12:33.000000 nics-1.0.0rc9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 21:12:33.000000 nics-1.0.0rc9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 21:12:50.000000 nics-1.0.0rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 21:12:33.000000 nics-1.0.0rc9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/404.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/assets/nics-logo500.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/wizard/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/wizard/workflows_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-29 21:12:33.000000 nics-1.0.0rc9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 21:12:50.000000 nics-1.0.0rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 21:12:33.000000 nics-1.0.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-30 15:28:19.000000 nics-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 15:28:19.000000 nics-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 15:28:43.000000 nics-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 15:28:19.000000 nics-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 15:28:19.000000 nics-2.0.0/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/4 -- About -- about.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/wizard/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-30 15:28:19.000000 nics-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 15:28:43.000000 nics-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-30 15:28:19.000000 nics-2.0.0/setup.py
```

### Comparing `nics-1.0.0rc9/LICENSE` & `nics-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc9/nics/main/__init__.py` & `nics-2.0.0/nics/main/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import argparse
 
 from .constants import __version__, SOFTWARE_DIST_NAME
 from .wizard import run as run_init
+from .upgrade import run as run_upgrade
 from .compile import run as run_compile
 
 
 def main():
 
     psr = argparse.ArgumentParser(
         prog=SOFTWARE_DIST_NAME,
         usage=(
             '\n'
-            '└─ %(prog)s init'
+            '├─ Run `%(prog)s init`   : Set up NICS environment\n'
+            '└─ Run `%(prog)s upgrade`: Reconfigure NICS environment'
         ),
         formatter_class=argparse.RawTextHelpFormatter  # to use line breaks (\n) in the help message
     )
     psr.add_argument(
         '-v', '--version', action='version', version=f'%(prog)s-{__version__}',
         help='show software version'
     )
-    subpsr = psr.add_subparsers(dest='cmd')
+    subpsr = psr.add_subparsers(dest='cmd', help=argparse.SUPPRESS)  # `help=argparse.SUPPRESS` to hide the help message
 
     ## command 'init'
-    subpsr.add_parser(
-        'init',
-        help=argparse.SUPPRESS  # to hide the help message
-    )
+    subpsr.add_parser('init', help=argparse.SUPPRESS)
+
+    ## command 'upgrade'
+    subpsr.add_parser('upgrade', help=argparse.SUPPRESS)
 
     ## command '_compile' (that users shouldn't run)
     c = subpsr.add_parser('_compile', help=argparse.SUPPRESS)
     c.add_argument('container')
     c.add_argument('dock')
 
     args = psr.parse_args()
 
     if args.cmd == 'init':
         run_init()
+    elif args.cmd == 'upgrade':
+        run_upgrade()
     elif args.cmd == '_compile':
         run_compile(args.container, args.dock)
```

### Comparing `nics-1.0.0rc9/nics/main/_template/docs/assets/nics-logo500.jpg` & `nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc9/nics/main/_template/web/_sass/header.scss` & `nics-2.0.0/nics/main/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc9/nics/main/_template/web/_sass/main.scss` & `nics-2.0.0/nics/main/_template/web/_sass/main.scss`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc9/nics/main/_template/web/scripts/header.js` & `nics-2.0.0/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc9/nics/main/compile/__init__.py` & `nics-2.0.0/nics/main/compile/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,54 +5,51 @@
 
 from ..constants import __version__, SOFTWARE_DIST_NAME, SETTINGS_KEYS
 from .inspect import inspect_the_container
 from .update_header import update_header
 from .update_footer import update_footer
 from .update_jekyll_config import update_jekyll_config
 from .update_404_and_favicon import update_404_and_favicon
-from .update_assets import update_assets
 from .copying_template import copying_template
 from .update_sass_constants import update_sass_constants
 from .update_docs_tree import update_docs_tree
 
 
 def run(container, dock):
     ## `container`: the 'docs/' folder (in main branch)
     ## `dock`: the 'docs' branch
     printer(f"INFO: Running '_compile' command ({SOFTWARE_DIST_NAME}-v{__version__})")
 
-    C_ASSETS = os.path.join(container, 'assets')
     C_TREE = os.path.join(container, 'tree')
     C_404 = os.path.join(container, '404.md')
     C_ICON = os.path.join(container, 'favicon.png')
     C_SETTINGS = os.path.join(container, 'settings.txt')
 
     D__INCLUDES = os.path.join(dock, '_includes')
     D__PAGES = os.path.join(dock, '_pages')
     D_HEADER = os.path.join(dock, '_includes', 'header.html')
     D_FOOTER = os.path.join(dock, '_includes', 'footer.html')
     D_JEKYLL_CONFIG = os.path.join(dock, '_config.yml')
     D_404 = os.path.join(dock, '404.md')
     D_ICON = os.path.join(dock, 'favicon.png')
-    D_ASSETS = os.path.join(dock, 'assets')
     D_SASS_CONSTANTS = os.path.join(dock, '_sass', 'constants.scss')
 
     ## inspection
     inspect_the_container(container)
 
     ## parse the settings
     cfg = KeyCrate(C_SETTINGS, True, True, SETTINGS_KEYS, SETTINGS_KEYS)
 
 
     if not os.path.isdir(D__INCLUDES):  # handle init case: initially, '_includes' folder doesn't exist in docs branch
+        printer(f'DEBUG: Creating dir {repr(D__INCLUDES)}.')
         os.mkdir(D__INCLUDES)
     update_header(C_TREE, D_HEADER)
     update_footer(D_FOOTER, cfg.show_credit)
 
     update_jekyll_config(D_JEKYLL_CONFIG, cfg.author, cfg._gh_username, cfg._gh_repo)
     update_404_and_favicon(C_404, C_ICON, D_404, D_ICON)
-    update_assets(C_ASSETS, D_ASSETS)
 
     copying_template(dock)
     update_sass_constants(D_SASS_CONSTANTS, cfg.color_hue)
 
-    update_docs_tree(dock, C_TREE, D__PAGES)
+    update_docs_tree(C_TREE, D__PAGES, cfg.lowercase_the_url)
```

### Comparing `nics-1.0.0rc9/nics/main/compile/copying_template.py` & `nics-2.0.0/nics/main/compile/copying_template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
 import shutil
 
 from mykit.kit.utils import printer
 
-from ..constants import TEMPLATE_DIR_PTH
+from ..constants import TMPL_WEB_DIR_PTH
 
 
 def copying_template(dock):
 
     LAYOUTS = os.path.join(dock, '_layouts')
     SASS = os.path.join(dock, '_sass')
     SCRIPTS = os.path.join(dock, 'scripts')
 
     ## handle the case when the template already exists
     if os.path.isdir(LAYOUTS): shutil.rmtree(LAYOUTS)
     if os.path.isdir(SASS): shutil.rmtree(SASS)
     if os.path.isdir(SCRIPTS): shutil.rmtree(SCRIPTS)
 
     shutil.copytree(
-        os.path.join(TEMPLATE_DIR_PTH, 'web', '_layouts'),
+        os.path.join(TMPL_WEB_DIR_PTH, '_layouts'),
         LAYOUTS
     )
     shutil.copytree(
-        os.path.join(TEMPLATE_DIR_PTH, 'web', '_sass'),
+        os.path.join(TMPL_WEB_DIR_PTH, '_sass'),
         SASS
     )
     shutil.copytree(
-        os.path.join(TEMPLATE_DIR_PTH, 'web', 'scripts'),
+        os.path.join(TMPL_WEB_DIR_PTH, 'scripts'),
         SCRIPTS
     )
     printer(f'INFO: Template copied.')
```

### Comparing `nics-1.0.0rc9/nics/main/compile/update_404_and_favicon.py` & `nics-2.0.0/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc9/nics/main/compile/update_docs_tree.py` & `nics-2.0.0/nics/main/compile/update_docs_tree.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import os
 import re
 import shutil
 
 from mykit.kit.utils import printer
 
 
-def update_recursively(dock, D__PAGES, pth, base):
+def update_recursively(D__PAGES, lowercase_the_url, pth, base):
     printer(f'DEBUG: Updating docs-tree, pth: {repr(pth)}, base: {repr(base)}')
 
     for i in os.listdir(pth):
         pth2 = os.path.join(pth, i)
 
+        ## handle non-markdown files
+        if os.path.isfile(pth2) and (not i.endswith('.md')):
+            dst = os.path.join(D__PAGES, os.sep.join(filter(lambda s:s!='', base.split('/'))), i)
+            printer(f'DEBUG: Copying non-markdown files from {repr(pth2)} to {repr(dst)}.')
+            shutil.copy(pth2, dst)
+            continue
+
         ## <handling the index.md>
         if i == 'index.md':
             if base == '/':  # homepage
-                dst = os.path.join(dock, 'index.md')
+                dst = os.path.join(D__PAGES, 'index.md')
                 text = (
                     '---\n'
                     'permalink: /\n'
                     'layout: main\n'
                     'title: Home\n'
                     '---\n\n'
                 )
@@ -33,42 +40,47 @@
                 )
             with open(pth2, 'r') as f: text += f.read()
             with open(dst, 'w') as f: f.write(text)
             printer(f'DEBUG: Updated index.md from {repr(pth2)} to {repr(dst)}.')
             continue
         ## </handling the index.md>
 
-        res = re.match(r'(?:\d+ -- )?(?P<name>[\w -.]+) -- (?P<url>[\w -]+)(?:\.md)?', i)
+        res = re.match(r"^(?:\d+ - )?(?P<name>[\w \-'&\(\).]+)(?:\.md)?$", i)
+        if res is None: raise AssertionError(f'Invalid docs-tree format: {repr(i)}')
         name = res.group('name')
-        url = res.group('url')
+        url = name.replace(' ', '-').replace("'", '').replace('&', 'and').replace('(', '').replace(')', '').replace('.', '-')
+        if lowercase_the_url: url = url.lower()
+        printer(f'DEBUG: name: {repr(name)}; url: {repr(url)}')
 
         if os.path.isdir(pth2):
             ## if the folder doesn't exist, create a new one.
-            dir = os.path.join(D__PAGES, os.sep.join(filter(lambda s:s!='', base.split('/'))), name)
+            dir = os.path.join(D__PAGES, os.sep.join(filter(lambda s:s!='', base.split('/'))), url)
             if not os.path.isdir(dir):
                 os.mkdir(dir)
                 printer(f'DEBUG: Dir created: {repr(dir)}.')
             ## do it again
-            update_recursively(dock, D__PAGES, pth2, base+name+'/')
+            update_recursively(D__PAGES, lowercase_the_url, pth2, base+url+'/')
         else:
             dst = os.path.join(D__PAGES, os.sep.join(filter(lambda s:s!='', base.split('/'))), f'{name}.md')
             text = (
                 '---\n'
                 f'permalink: {base}{url}/\n'
                 'layout: main\n'
                 f'title: {name}\n'
                 '---\n\n'
             )
             with open(pth2, 'r') as f: text += f.read()
             with open(dst, 'w') as f: f.write(text)
             printer(f'DEBUG: Updated docs-tree file from {repr(pth2)} to {repr(dst)}.')
 
 
-def update_docs_tree(dock, C_TREE, D__PAGES):
+def update_docs_tree(C_TREE, D__PAGES, lowercase_the_url):
 
     ## delete the old '_pages' folder in docs branch
     if os.path.isdir(D__PAGES):  # reminder: initially, '_pages' doesn't exist
         printer(f'DEBUG: Deleting {repr(D__PAGES)} recursively.')
         shutil.rmtree(D__PAGES)
-        os.mkdir(D__PAGES)
 
-    update_recursively(dock, D__PAGES, C_TREE, '/')
+    printer(f'DEBUG: Creating dir {repr(D__PAGES)}.')
+    os.mkdir(D__PAGES)
+
+    update_recursively(D__PAGES, lowercase_the_url, C_TREE, '/')
```

### Comparing `nics-1.0.0rc9/nics/main/compile/update_header.py` & `nics-2.0.0/nics/main/compile/update_header.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 
 from mykit.kit.utils import printer
 
 
-def update_header(C_TREE, D_HEADER):
+def update_header(C_TREE, D_HEADER, lowercase_the_url):
     ## reminder: index.md will not be included in the header
 
     text = (
         '<header>'
             '<h1>{{ page.title }}</h1>'
             '<div class="wrap">'
                 '<button id="_root__nav">v Navigation</button>'
@@ -17,28 +17,34 @@
 
     ## reminder: `base` is the X in foo.com/baseurl/{X}page
     ##           (e.g. nvfp.github.io/mykit/docs/guide/foo, then X='docs/guide/')
     def build_the_nested_divs_recursively(pth, base):
         out = ''
 
         for fd in sorted(os.listdir(pth)):  # reminder: the file/dir `fd` order in `pth` matters.
-            if fd == 'index.md': continue  # index.md will not be shown in navigation bar
             fd_pth = os.path.join(pth, fd)
 
-            res = re.match(r'(?:\d+ -- )?(?P<name>[\w -.]+) -- (?P<url>[\w -]+)(?:\.md)?', fd)
+            if fd == 'index.md': continue  # index.md will not be shown in navigation bar
+            if os.path.isfile(fd_pth) and (not fd.endswith('.md')): continue  # ignore non-markdown files
+
+            res = re.match(r"^(?:\d+ - )?(?P<name>[\w \-'&\(\).]+)(?:\.md)?$", fd)
+            if res is None: raise AssertionError(f'Invalid docs-tree format: {repr(fd)}')
             name = res.group('name')
-            url = res.group('url')
+            url = name.replace(' ', '-').replace("'", '').replace('&', 'and').replace('(', '').replace(')', '').replace('.', '-')
+            if lowercase_the_url: url = url.lower()
+            printer(f'DEBUG: name: {repr(name)}; url: {repr(url)}')
 
             if os.path.isdir(fd_pth):
                 out += f'<button id="{base.replace("/", "-")}{url}">> {name}</button>'  # remember to replace all slashes to hyphens
                 out += f'<div class="child" id="{base.replace("/", "-")}{url}-div">'  # remember to replace all slashes to hyphens
                 out += build_the_nested_divs_recursively(fd_pth, base+url+'/')
                 out += '</div>'
             else:
                 out += '<a href="{{ site.baseurl }}/' + f'{base}{url}">{name}</a>'
+                printer(f'DEBUG: href {repr(name)} added.')
 
         return out
     text += build_the_nested_divs_recursively(C_TREE, '')
 
     text += (
                 '</div>'
             '</div>'
```

### Comparing `nics-1.0.0rc9/nics/main/compile/update_jekyll_config.py` & `nics-2.0.0/nics/main/compile/update_jekyll_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 include: [_pages, _sass, scripts]
 
 permalink: pretty
 
 sass:
   style: compact # possible values: nested expanded compact compressed
-  sass_dir: _sass    
+  sass_dir: _sass
 """
 
 
 def update_jekyll_config(D_JEKYLL_CONFIG, author, gh_username, gh_repo):
 
 	text = _writer(author, gh_username, gh_repo)
 	with open(D_JEKYLL_CONFIG, 'w') as f: f.write(text)
```

### Comparing `nics-1.0.0rc9/nics/main/constants.py` & `nics-2.0.0/nics/main/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,19 +10,26 @@
 
 SOFTWARE_REPO = 'https://github.com/nvfp/now-i-can-sleep'
 SOFTWARE_NAME = 'Now I Can Sleep'
 SOFTWARE_DIST_NAME = 'nics'  # distribution name
 
 ROOT_DIR_PTH = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 DIST_DIR_PTH = os.path.join(ROOT_DIR_PTH, SOFTWARE_DIST_NAME)
+MAIN_DIR_PTH = os.path.join(ROOT_DIR_PTH, SOFTWARE_DIST_NAME, 'main')
 
-TEMPLATE_DIR_PTH = os.path.join(DIST_DIR_PTH, '_template')
+TEMPLATE_DIR_PTH = os.path.join(MAIN_DIR_PTH, '_template')
 TMPL_DOCS_DIR_PTH = os.path.join(TEMPLATE_DIR_PTH, 'docs')
 TMPL_WEB_DIR_PTH = os.path.join(TEMPLATE_DIR_PTH, 'web')
 
 SETTINGS_KEYS = [
     'author',
     'color_hue',
+    'lowercase_the_url',
     'show_credit',
+    
+    '_email',
     '_gh_username',
     '_gh_repo',
+    '_main_branch_name',
+    
+    '_nics_version',
 ]
```

### Comparing `nics-1.0.0rc9/nics/main/wizard/__init__.py` & `nics-2.0.0/nics/main/wizard/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 
 from mykit.kit.utils import printer, print_screen
 
 from ..constants import TMPL_DOCS_DIR_PTH
 from .inspect import inspect
-from .workflows_writer import workflows_writer
+from .workflow_writer import workflow_writer
 from .settings_writer import settings_writer
 
 
 def run():
 
     CWD = os.getcwd()
 
@@ -41,21 +41,21 @@
             printer(f"INFO: Folder {repr(pth)} is created.")
         pth = os.path.join(CWD, '.github', 'workflows')
         if not os.path.isdir(pth):
             os.mkdir(pth)
             printer(f"INFO: Folder {repr(pth)} is created.")
     handle_workflow_dirs()
 
-    workflows_writer(WORKFLOW_FILE_PTH, author, email, gh_repo, main_branch_name)
-    
+    workflow_writer(WORKFLOW_FILE_PTH, author, email, gh_repo, main_branch_name)
+
     printer(f"INFO: Copying 'docs/' folder.")
     shutil.copytree(TMPL_DOCS_DIR_PTH, CONTAINER_DIR_PTH)
     printer(f'INFO: Done, {repr(CONTAINER_DIR_PTH)} is created.')
 
-    settings_writer(SETTINGS_FILE_PTH, author, gh_username, gh_repo)
+    settings_writer(SETTINGS_FILE_PTH, author, email, gh_username, gh_repo, main_branch_name)
 
     ## outro
     print_screen(f"""
 Almost done, now you need to do these final steps:
 1. Create docs branch
    - git commit -am "NICS init"
    - git checkout --orphan docs
```

### Comparing `nics-1.0.0rc9/nics/main/wizard/workflows_writer.py` & `nics-2.0.0/nics/main/wizard/workflow_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from ..constants import __version__, SOFTWARE_DIST_NAME, SOFTWARE_REPO
 
 
 def _writer(author, email, gh_repo, main_branch_name):
     return f"""
 
-# This file was generated by {SOFTWARE_DIST_NAME}-v{__version__}.
+# This file was generated by {SOFTWARE_DIST_NAME}-v{__version__} .
 # Please make sure to be careful when modifying the values below. For more information, visit: {SOFTWARE_REPO}
 
 name: Rebuild docs
 
 on:
   push:
     branches:
@@ -70,15 +70,15 @@
           git config user.email "{email}"
           git add .
           git commit -m "NICS rebuilds the docs"
           git push
 """
 
 
-def workflows_writer(pth, author, email, gh_repo, main_branch_name):
+def workflow_writer(pth, author, email, gh_repo, main_branch_name):
     printer(f'INFO: Writing GitHub workflow file.')
 
     text = _writer(author, email, gh_repo, main_branch_name)
     with open(pth, 'w') as f:
         f.write(text)
 
     printer(f'INFO: Done, {repr(pth)} is created.')
```

### Comparing `nics-1.0.0rc9/nics.egg-info/SOURCES.txt` & `nics-2.0.0/nics.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,37 +11,38 @@
 nics.egg-info/entry_points.txt
 nics.egg-info/requires.txt
 nics.egg-info/top_level.txt
 nics/main/__init__.py
 nics/main/constants.py
 nics/main/_template/docs/404.md
 nics/main/_template/docs/favicon.png
-nics/main/_template/docs/assets/nics-logo500.jpg
 nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
 nics/main/_template/docs/tree/4 -- About -- about.md
 nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
 nics/main/_template/docs/tree/index.md
+nics/main/_template/docs/tree/nics-logo500.jpg
 nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
 nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
 nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
+nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
 nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
 nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
 nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
 nics/main/_template/web/_layouts/main.html
 nics/main/_template/web/_sass/footer.scss
 nics/main/_template/web/_sass/header.scss
 nics/main/_template/web/_sass/main.scss
 nics/main/_template/web/scripts/header.js
 nics/main/compile/__init__.py
 nics/main/compile/copying_template.py
 nics/main/compile/inspect.py
 nics/main/compile/update_404_and_favicon.py
-nics/main/compile/update_assets.py
 nics/main/compile/update_docs_tree.py
 nics/main/compile/update_footer.py
 nics/main/compile/update_header.py
 nics/main/compile/update_jekyll_config.py
 nics/main/compile/update_sass_constants.py
+nics/main/upgrade/__init__.py
 nics/main/wizard/__init__.py
 nics/main/wizard/inspect.py
 nics/main/wizard/settings_writer.py
-nics/main/wizard/workflows_writer.py
+nics/main/wizard/workflow_writer.py
```

### Comparing `nics-1.0.0rc9/pyproject.toml` & `nics-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "1.0.0rc9"
+version = "2.0.0"
 description = "Automated docs repo generator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
@@ -30,14 +30,15 @@
     "mykit==4.1.0",
 ]
 
 
 [tool.setuptools.packages.find]
 exclude = [
     "archive*",
+    "assets*",
     "docs*",
     "tests*",
 ]
 
 
 [project.urls]
 documentation = "https://nvfp.github.io/now-i-can-sleep/docs"
```

