# Comparing `tmp/jupyterlab_pachyderm-2.7.0a2.tar.gz` & `tmp/jupyterlab_pachyderm-2.7.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.7.0a2.tar", last modified: Thu Jun  8 21:08:12 2023, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.7.0a4.tar", last modified: Fri Jun 23 16:36:19 2023, max compression
```

## Comparing `jupyterlab_pachyderm-2.7.0a2.tar` & `jupyterlab_pachyderm-2.7.0a4.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.026693 jupyterlab_pachyderm-2.7.0a2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-06-08 21:08:12.026693 jupyterlab_pachyderm-2.7.0a2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.002694 jupyterlab_pachyderm-2.7.0a2/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.006693 jupyterlab_pachyderm-2.7.0a2/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.006693 jupyterlab_pachyderm-2.7.0a2/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.010693 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/filemanager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13073 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.010693 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.002694 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.010693 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-06-08 21:07:59.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-06-08 21:07:59.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-08 21:07:59.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-06-08 21:07:59.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-08 21:07:59.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.014694 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   161100 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/829.e9784d0c17729cab49a8.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8300 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/remoteEntry.3717fd22eb9abc7f8046.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-06-08 21:07:59.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-06-08 21:08:09.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9229 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/mount_server_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/pachyderm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9590 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/pps_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.014694 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.014694 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/data/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19829 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/test_handlers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17560 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/test_integrations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.010693 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-06-08 21:08:11.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-06-08 21:08:11.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 21:08:11.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 21:07:44.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-06-08 21:08:11.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-08 21:08:11.000000 jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-06-08 21:05:54.000000 jupyterlab_pachyderm-2.7.0a2/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.014694 jupyterlab_pachyderm-2.7.0a2/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-06-08 21:08:12.026693 jupyterlab_pachyderm-2.7.0a2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.014694 jupyterlab_pachyderm-2.7.0a2/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.006693 jupyterlab_pachyderm-2.7.0a2/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/__tests__/mount.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.006693 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6365 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/Pipeline.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/Splash.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.018694 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/ListMount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/ListUnmount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3498 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/SortableList.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15391 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22029 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4382 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2763 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.006693 jupyterlab_pachyderm-2.7.0a2/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/src/utils/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/hooks/usePreviousValue.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/hooks/useSort.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:08:12.022693 jupyterlab_pachyderm-2.7.0a2/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-06-08 21:05:53.000000 jupyterlab_pachyderm-2.7.0a2/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.349360 jupyterlab_pachyderm-2.7.0a4/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.349360 jupyterlab_pachyderm-2.7.0a4/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.353360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/filemanager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13073 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.353360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.353360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   161100 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/829.e9784d0c17729cab49a8.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8300 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/remoteEntry.70a21b765fbc6385e2db.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11122 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/mount_server_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/pachyderm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9596 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/data/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19829 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/test_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17560 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/test_integrations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.353360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 16:35:49.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/__tests__/mount.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6365 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/Pipeline.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/Splash.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/ListMount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/ListUnmount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3498 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/SortableList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15391 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22029 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4382 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2763 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/src/utils/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/hooks/usePreviousValue.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/hooks/useSort.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/LICENSE` & `jupyterlab_pachyderm-2.7.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/MANIFEST.in` & `jupyterlab_pachyderm-2.7.0a4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/PKG-INFO` & `jupyterlab_pachyderm-2.7.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_pachyderm
-Version: 2.7.0a2
+Version: 2.7.0a4
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/README.md` & `jupyterlab_pachyderm-2.7.0a4/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/env.py` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/env.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 from distutils.util import strtobool
 
 PFS_MOUNT_DIR = os.environ.get("PFS_MOUNT_DIR", "/pfs")
 SIDECAR_MODE = strtobool(os.environ.get("SIDECAR_MODE", "False").lower())
 MOUNT_SERVER_LOG_DIR = os.environ.get("MOUNT_SERVER_LOG_DIR") # defaults to stdout/stderr
+NONPRIV_CONTAINER = os.environ.get("NONPRIV_CONTAINER") # Unset assume --privileged container
+
 
 PACHYDERM_EXT_DEBUG = strtobool(os.environ.get("PACHYDERM_EXT_DEBUG", "False").lower())
 if PACHYDERM_EXT_DEBUG:
     from jupyterlab_pachyderm.log import get_logger
 
     logger = get_logger()
     logger.setLevel("DEBUG")
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758597883597885%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.70a21b765fbc6385e2db.js'}}",*

 * * "'version'": "'2.7.0-alpha.4'"}*

```diff
@@ -68,15 +68,15 @@
                 "npm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3717fd22eb9abc7f8046.js",
+            "load": "static/remoteEntry.70a21b765fbc6385e2db.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
@@ -133,9 +133,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-alpha.2"
+    "version": "2.7.0-alpha.4"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.7.0-alpha.4'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-alpha.2"
+    "version": "2.7.0-alpha.4"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/829.e9784d0c17729cab49a8.js` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/829.e9784d0c17729cab49a8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/remoteEntry.3717fd22eb9abc7f8046.js` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/remoteEntry.70a21b765fbc6385e2db.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -116,15 +116,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : l > u.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (u("jupyterlab-pachyderm", "2.7.0-alpha.2", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab-pachyderm", "2.7.0-alpha.4", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/mount_server_client.py` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/mount_server_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 
 from tornado.httpclient import AsyncHTTPClient, HTTPClientError
 from tornado import locks
 
 from .pachyderm import MountInterface
 from .log import get_logger
-from .env import SIDECAR_MODE, MOUNT_SERVER_LOG_DIR
+from .env import SIDECAR_MODE, MOUNT_SERVER_LOG_DIR, NONPRIV_CONTAINER
 
 lock = locks.Lock()
 MOUNT_SERVER_PORT = 9002
 
 
 class MountServerClient(MountInterface):
     """Client interface for the mount-server backend."""
@@ -23,14 +23,17 @@
     def __init__(
         self,
         mount_dir: str,
     ):
         self.client = AsyncHTTPClient()
         self.mount_dir = mount_dir
         self.address = f"http://localhost:{MOUNT_SERVER_PORT}"
+        # non-prived container flag (set via -e NONPRIV_CONTAINER=1)
+        # TODO: Would be preferable to auto-detect this, but unclear how
+        self.nopriv = NONPRIV_CONTAINER
 
     async def _is_mount_server_running(self):
         get_logger().debug("Checking if mount server running...")
         try:
             await self.health()
         except Exception as e:
             get_logger().debug(f"Unable to hit server at {self.address}")
@@ -67,14 +70,20 @@
 
         get_logger().info("Starting mount server...")
         async with lock:
             if not await self._is_mount_server_running():
                 self._unmount()
 
                 mount_server_cmd = f"mount-server --mount-dir {self.mount_dir}"
+                if self.nopriv:
+                    # Cannot mount in non-privileged container, so use unshare for a private mount
+                    get_logger().info("Non-privileged container...")
+                    subprocess.run(['mkdir','-p', f'/mnt{self.mount_dir}'])
+                    mount_server_cmd = f"unshare -Ufirm mount-server --mount-dir /mnt{self.mount_dir} --allow-other=false"
+
                 if MOUNT_SERVER_LOG_DIR is not None and MOUNT_SERVER_LOG_DIR:
                   mount_server_cmd += f" >> {MOUNT_SERVER_LOG_DIR} 2>&1"
 
                 subprocess.Popen(
                     [
                         "bash",
                         "-c",
@@ -88,14 +97,32 @@
                 while not await self._is_mount_server_running():
                     time.sleep(1)
                     tries += 1
 
                     if tries == 10:
                         get_logger().debug("Unable to start mount server...")
                         return False
+                
+                if self.nopriv:
+                    # Using un-shared mount, replace /pfs with a softlink to the mount point
+                    mount_server_proc = subprocess.run(['pgrep','mount-server'], capture_output=True)
+                    mount_server_pid = mount_server_proc.stdout.decode("utf-8")
+                    if not mount_server_pid or not int(mount_server_pid) > 0:
+                        get_logger().debug(f"Unable to find mount-server process: {mount_server_pid}")
+                        return False
+                    mount_server_pid = int(mount_server_pid)
+                    get_logger().info(f"Link non-privileged /pfs to /proc/{mount_server_pid}/root/mnt{self.mount_dir}")
+                    if os.path.exists(self.mount_dir) or os.path.islink(self.mount_dir):
+                        if os.path.isdir(self.mount_dir): 
+                            get_logger().debug(f"Removing dir {self.mount_dir}")
+                            os.rmdir(self.mount_dir)
+                        else:
+                            get_logger().debug(f"Removing file {self.mount_dir}")
+                            os.remove(self.mount_dir) 
+                    os.symlink( f'/proc/{mount_server_pid}/root/mnt{self.mount_dir}', '/pfs', target_is_directory=True)
 
         return True
 
 
     async def list_repos(self):
         await self._ensure_mount_server()
         response = await self.client.fetch(f"{self.address}/repos")
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/pachyderm.py` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/pachyderm.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/pps_client.py` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/pps_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     pipeline = dict(name=config.pipeline.name)
     if config.pipeline.project and config.pipeline.project.name:
         pipeline['project'] = dict(name=config.pipeline.project.name)
     return dict(
         pipeline=pipeline,
         description="Auto-generated from notebook",
         transform=dict(
-            cmd=["python3", f"/pfs/{companion_repo}/entrypoint.py"],
+            cmd=["python3", "-u", f"/pfs/{companion_repo}/entrypoint.py"],
             image=config.image
         ),
         input=input_spec,
         update=True,
         reprocess=True,
     )
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/test_handlers.py` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-pachyderm
-Version: 2.7.0a2
+Version: 2.7.0a4
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
 jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
 jupyterlab_pachyderm/labextension/static/829.e9784d0c17729cab49a8.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.3717fd22eb9abc7f8046.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.70a21b765fbc6385e2db.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/test_handlers.py
 jupyterlab_pachyderm/tests/test_integrations.py
 jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
 jupyterlab_pachyderm/tests/data/requirements.txt
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/package.json` & `jupyterlab_pachyderm-2.7.0a4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.7.0-alpha.4'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-alpha.2"
+    "version": "2.7.0-alpha.4"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0a2/pyproject.toml` & `jupyterlab_pachyderm-2.7.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/setup.cfg` & `jupyterlab_pachyderm-2.7.0a4/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/setup.py` & `jupyterlab_pachyderm-2.7.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/handler.ts` & `jupyterlab_pachyderm-2.7.0a4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/Splash.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/Splash.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/ListMount.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/ListMount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/ListUnmount.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/ListUnmount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/SortableList.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/SortableList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/index.ts` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/pollMounts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.7.0a4/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/utils/hooks/useSort.ts` & `jupyterlab_pachyderm-2.7.0a4/src/utils/hooks/useSort.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/src/utils/icons.ts` & `jupyterlab_pachyderm-2.7.0a4/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/style/base.css` & `jupyterlab_pachyderm-2.7.0a4/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/style/components/button.css` & `jupyterlab_pachyderm-2.7.0a4/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/style/icons/file.svg` & `jupyterlab_pachyderm-2.7.0a4/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/style/icons/info.svg` & `jupyterlab_pachyderm-2.7.0a4/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.7.0a4/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a2/style/icons/repo.svg` & `jupyterlab_pachyderm-2.7.0a4/style/icons/repo.svg`

 * *Files identical despite different names*

