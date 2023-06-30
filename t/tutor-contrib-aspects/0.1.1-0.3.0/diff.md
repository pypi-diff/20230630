# Comparing `tmp/tutor-contrib-aspects-0.1.1.tar.gz` & `tmp/tutor-contrib-aspects-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.1.1.tar", last modified: Tue Jun 27 16:39:26 2023, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.3.0.tar", last modified: Fri Jun 30 16:51:53 2023, max compression
```

## Comparing `tutor-contrib-aspects-0.1.1.tar` & `tutor-contrib-aspects-0.3.0.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.861550 tutor-contrib-aspects-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10264 2023-06-27 16:39:26.861550 tutor-contrib-aspects-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9381 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-27 16:39:26.861550 tutor-contrib-aspects-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.849550 tutor-contrib-aspects-0.1.1/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10264 2023-06-27 16:39:26.000000 tutor-contrib-aspects-0.1.1/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-06-27 16:39:26.000000 tutor-contrib-aspects-0.1.1/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 16:39:26.000000 tutor-contrib-aspects-0.1.1/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-27 16:39:26.000000 tutor-contrib-aspects-0.1.1/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-27 16:39:26.000000 tutor-contrib-aspects-0.1.1/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-27 16:39:26.000000 tutor-contrib-aspects-0.1.1/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.849550 tutor-contrib-aspects-0.1.1/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.853550 tutor-contrib-aspects-0.1.1/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (122)    16601 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (122)     9045 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (122)     2795 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/openedx-cms-common-settings
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (122)    19670 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.853550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.845550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.853550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.845550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.853550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.845550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.853550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (122)     1346 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/ralph/config/env
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.853550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (122)      283 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.845550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.853550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/scripts/aspects/
--rwxr-xr-x   0 runner    (1001) docker     (122)      714 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/scripts/aspects/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/scripts/aspects/dbt.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/scripts/aspects/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/scripts/aspects/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.853550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.853550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2113 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.857550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (122)    14695 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     5094 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     5469 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3223 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.857550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/security/
--rw-r--r--   0 runner    (1001) docker     (122)    95955 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.857550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.857550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.857550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.857550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/build/aspects/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.857550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.845550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.857550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.857550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (122)    14814 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.861550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/dbt/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/dbt/init-dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 16:39:26.861550 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/superset/
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     2931 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1334 2023-06-27 16:39:21.000000 tutor-contrib-aspects-0.1.1/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 16:51:53.941579 tutor-contrib-aspects-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.929579 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.929579 tutor-contrib-aspects-0.3.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/openedx-cms-common-settings
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.929579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.925579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.925579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.925579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (123)    23753 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/security/
+-rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.929579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/dbt/init-dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2931 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/base-docker-compose-services
```

### Comparing `tutor-contrib-aspects-0.1.1/PKG-INFO` & `tutor-contrib-aspects-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.1.1
+Version: 0.3.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,15 @@
 
 - `ClickHouse <https://clickhouse.com>`__, a fast, scalable analytics database that can be run anywhere
 - `Apache Superset <https://superset.apache.org>`__, a data visualization platform and data API
 - `OpenFUN Ralph <https://https://openfun.github.io/ralph/>`__, a Learning Record store (and more) that can validate and store xAPI statements in ClickHouse
 - `Vector <https://vector.dev/>`__, a log forwarding tool that can be used to forward tracking log and xAPI data to ClickHouse
 - `event-routing-backends <https://https://event-routing-backends.readthedocs.io/en/latest/>`__, an Open edX plugin that transforms tracking logs into xAPI and optionally forwards them to one or more Learning Record Stores in near real time
 - `event-sink-clickhouse <https://github.com/openedx/openedx-event-sink-clickhouse>`__, an Open edX plugin that exports course structure and high level data to ClickHouse at publish time
+- `dbt <https://www.getdbt.com/>`__, a tool to build data pipelines from SQL queries. The dbt project used by this plugin is `aspects-dbt <https://github.com/openedx/aspects-dbt>`__.
 
 See https://github.com/openedx/openedx-oars for more details about the Aspects architecture and high level documentation.
 
 Aspects is a community developed effort combining the Cairn project by Overhang.io and the OARS project by EduNEXT, OpenCraft, and Axim Collaborative.
 
 Note: Aspects is in heavy development and not yet production ready! Please feel
 free to experiment with the system and offer feedback about what you'd like to see
@@ -171,15 +172,15 @@
 #. Expand the ``.zip`` file.
 #. Update any database connection strings to use Tutor configuration template variables
    instead of hard-coded strings, e.g. replace ``clickhouse`` with ``{{CLICKHOUSE_HOST}}``.
    Passwords can be left as ``{{CLICKHOUSE_PASSWORD}}``, though be aware that if you are adding new
    databases, you'll need to update ``SUPERSET_DB_PASSWORDS`` in the init scripts.
    Here is the default connection string for reference::
 
-    ``clickhousedb+connect://{{ASPECTS_CLICKHOUSE_REPORT_USER}}:{{ASPECTS_CLICKHOUSE_REPORT_PASSWORD}}@{{CLICKHOUSE_HOST}}:{% if CLICKHOUSE_SECURE_CONNECTION%}{{CLICKHOUSE_HTTPS_PORT}}{% else %}{{CLICKHOUSE_HTTP_PORT}}{% endif %}/{{ASPECTS_XAPI_DATABASE}}``
+    ``clickhousedb+connect://{{CLICKHOUSE_REPORT_URL}}``
 #. Remove any ``metadata.yaml`` files from the export. We generate these as needed during import.
 #. Merge your exported files into the directories and files in the `assets.yaml`_.
 #. Submit a PR with screenshots of your new chart or dashboards, along with an explanation
    of what data question they answer.
 
 
 Changing Superset Language Settings
```

### Comparing `tutor-contrib-aspects-0.1.1/README.rst` & `tutor-contrib-aspects-0.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 - `ClickHouse <https://clickhouse.com>`__, a fast, scalable analytics database that can be run anywhere
 - `Apache Superset <https://superset.apache.org>`__, a data visualization platform and data API
 - `OpenFUN Ralph <https://https://openfun.github.io/ralph/>`__, a Learning Record store (and more) that can validate and store xAPI statements in ClickHouse
 - `Vector <https://vector.dev/>`__, a log forwarding tool that can be used to forward tracking log and xAPI data to ClickHouse
 - `event-routing-backends <https://https://event-routing-backends.readthedocs.io/en/latest/>`__, an Open edX plugin that transforms tracking logs into xAPI and optionally forwards them to one or more Learning Record Stores in near real time
 - `event-sink-clickhouse <https://github.com/openedx/openedx-event-sink-clickhouse>`__, an Open edX plugin that exports course structure and high level data to ClickHouse at publish time
+- `dbt <https://www.getdbt.com/>`__, a tool to build data pipelines from SQL queries. The dbt project used by this plugin is `aspects-dbt <https://github.com/openedx/aspects-dbt>`__.
 
 See https://github.com/openedx/openedx-oars for more details about the Aspects architecture and high level documentation.
 
 Aspects is a community developed effort combining the Cairn project by Overhang.io and the OARS project by EduNEXT, OpenCraft, and Axim Collaborative.
 
 Note: Aspects is in heavy development and not yet production ready! Please feel
 free to experiment with the system and offer feedback about what you'd like to see
@@ -150,15 +151,15 @@
 #. Expand the ``.zip`` file.
 #. Update any database connection strings to use Tutor configuration template variables
    instead of hard-coded strings, e.g. replace ``clickhouse`` with ``{{CLICKHOUSE_HOST}}``.
    Passwords can be left as ``{{CLICKHOUSE_PASSWORD}}``, though be aware that if you are adding new
    databases, you'll need to update ``SUPERSET_DB_PASSWORDS`` in the init scripts.
    Here is the default connection string for reference::
 
-    ``clickhousedb+connect://{{ASPECTS_CLICKHOUSE_REPORT_USER}}:{{ASPECTS_CLICKHOUSE_REPORT_PASSWORD}}@{{CLICKHOUSE_HOST}}:{% if CLICKHOUSE_SECURE_CONNECTION%}{{CLICKHOUSE_HTTPS_PORT}}{% else %}{{CLICKHOUSE_HTTP_PORT}}{% endif %}/{{ASPECTS_XAPI_DATABASE}}``
+    ``clickhousedb+connect://{{CLICKHOUSE_REPORT_URL}}``
 #. Remove any ``metadata.yaml`` files from the export. We generate these as needed during import.
 #. Merge your exported files into the directories and files in the `assets.yaml`_.
 #. Submit a PR with screenshots of your new chart or dashboards, along with an explanation
    of what data question they answer.
 
 
 Changing Superset Language Settings
```

### Comparing `tutor-contrib-aspects-0.1.1/setup.py` & `tutor-contrib-aspects-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.1.1
+Version: 0.3.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,15 @@
 
 - `ClickHouse <https://clickhouse.com>`__, a fast, scalable analytics database that can be run anywhere
 - `Apache Superset <https://superset.apache.org>`__, a data visualization platform and data API
 - `OpenFUN Ralph <https://https://openfun.github.io/ralph/>`__, a Learning Record store (and more) that can validate and store xAPI statements in ClickHouse
 - `Vector <https://vector.dev/>`__, a log forwarding tool that can be used to forward tracking log and xAPI data to ClickHouse
 - `event-routing-backends <https://https://event-routing-backends.readthedocs.io/en/latest/>`__, an Open edX plugin that transforms tracking logs into xAPI and optionally forwards them to one or more Learning Record Stores in near real time
 - `event-sink-clickhouse <https://github.com/openedx/openedx-event-sink-clickhouse>`__, an Open edX plugin that exports course structure and high level data to ClickHouse at publish time
+- `dbt <https://www.getdbt.com/>`__, a tool to build data pipelines from SQL queries. The dbt project used by this plugin is `aspects-dbt <https://github.com/openedx/aspects-dbt>`__.
 
 See https://github.com/openedx/openedx-oars for more details about the Aspects architecture and high level documentation.
 
 Aspects is a community developed effort combining the Cairn project by Overhang.io and the OARS project by EduNEXT, OpenCraft, and Axim Collaborative.
 
 Note: Aspects is in heavy development and not yet production ready! Please feel
 free to experiment with the system and offer feedback about what you'd like to see
@@ -171,15 +172,15 @@
 #. Expand the ``.zip`` file.
 #. Update any database connection strings to use Tutor configuration template variables
    instead of hard-coded strings, e.g. replace ``clickhouse`` with ``{{CLICKHOUSE_HOST}}``.
    Passwords can be left as ``{{CLICKHOUSE_PASSWORD}}``, though be aware that if you are adding new
    databases, you'll need to update ``SUPERSET_DB_PASSWORDS`` in the init scripts.
    Here is the default connection string for reference::
 
-    ``clickhousedb+connect://{{ASPECTS_CLICKHOUSE_REPORT_USER}}:{{ASPECTS_CLICKHOUSE_REPORT_PASSWORD}}@{{CLICKHOUSE_HOST}}:{% if CLICKHOUSE_SECURE_CONNECTION%}{{CLICKHOUSE_HTTPS_PORT}}{% else %}{{CLICKHOUSE_HTTP_PORT}}{% endif %}/{{ASPECTS_XAPI_DATABASE}}``
+    ``clickhousedb+connect://{{CLICKHOUSE_REPORT_URL}}``
 #. Remove any ``metadata.yaml`` files from the export. We generate these as needed during import.
 #. Merge your exported files into the directories and files in the `assets.yaml`_.
 #. Submit a PR with screenshots of your new chart or dashboards, along with an explanation
    of what data question they answer.
 
 
 Changing Superset Language Settings
```

### Comparing `tutor-contrib-aspects-0.1.1/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,24 @@
 tutoraspects/patches/k8s-volumes
 tutoraspects/patches/kustomization-configmapgenerator
 tutoraspects/patches/local-docker-compose-dev-services
 tutoraspects/patches/local-docker-compose-jobs-services
 tutoraspects/patches/local-docker-compose-services
 tutoraspects/patches/openedx-cms-common-settings
 tutoraspects/patches/superset-extra-assets
+tutoraspects/patches/superset-jinja-filters
 tutoraspects/templates/base-docker-compose-services
 tutoraspects/templates/aspects/apps/.gitignore
+tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
 tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
 tutoraspects/templates/aspects/apps/ralph/config/env
 tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-tutoraspects/templates/aspects/apps/scripts/aspects/clickhouse-demo-xapi-data.sh
-tutoraspects/templates/aspects/apps/scripts/aspects/dbt.sh
-tutoraspects/templates/aspects/apps/scripts/aspects/profiles.yml
-tutoraspects/templates/aspects/apps/scripts/aspects/requirements.txt
 tutoraspects/templates/aspects/apps/superset/.gitignore
 tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
 tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
 tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
 tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-deployments`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__EVENT_TABLE_NAME
               value: "{{ASPECTS_RAW_XAPI_TABLE}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__HOST
               value: "{{CLICKHOUSE_HOST}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__PASSWORD
               value: "{{CLICKHOUSE_ADMIN_PASSWORD}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__PORT
-              value: "{% if CLICKHOUSE_SECURE_CONNECTION%}{{CLICKHOUSE_HTTPS_PORT}}{% else %}{{CLICKHOUSE_HTTP_PORT}}{% endif %}"
+              value: "{{CLICKHOUSE_PORT}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__TEST_HOST
               value: "clickhouse"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__USERNAME
               value: "{{CLICKHOUSE_ADMIN_USER}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__XAPI_DATABASE
               value: "{{ASPECTS_XAPI_DATABASE}}"
             - name: RALPH_RUNSERVER_BACKEND
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-jobs`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,34 @@
     spec:
       restartPolicy: Never
       containers:
       - name: aspects
         env:
           - name: VENV_DIR
             value: /opt/venv
+          - name: XAPI_SCHEMA
+            value: {{ ASPECTS_XAPI_DATABASE }}
+          - name: ASPECTS_ENROLLMENT_EVENTS_TABLE
+            value: {{ ASPECTS_ENROLLMENT_EVENTS_TABLE }}
         image: {{ DOCKER_IMAGE_ASPECTS }}
         securityContext:
           allowPrivilegeEscalation: false
           runAsUser: 0
         volumeMounts:
-            - mountPath: /app/aspects/scripts
-              name: scripts
+          - mountPath: /app/aspects/dbt
+            name: dbt
+          - mountPath: /app/aspects/scripts
+            name: scripts
       volumes:
         - name: scripts
           configMap:
             name: aspects-scripts
+        - name: dbt
+          configMap:
+            name: aspects-dbt
 ---
 apiVersion: batch/v1
 kind: Job
 metadata:
   name: clickhouse-job
   labels:
     app.kubernetes.io/component: job
@@ -79,15 +88,15 @@
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__EVENT_TABLE_NAME
               value: "{{ASPECTS_RAW_XAPI_TABLE}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__HOST
               value: "{{CLICKHOUSE_HOST}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__PASSWORD
               value: "{{CLICKHOUSE_ADMIN_PASSWORD}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__PORT
-              value: "{% if CLICKHOUSE_SECURE_CONNECTION%}{{CLICKHOUSE_HTTPS_PORT}}{% else %}{{CLICKHOUSE_HTTP_PORT}}{% endif %}"
+              value: "{{CLICKHOUSE_PORT}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__TEST_HOST
               value: "clickhouse"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__USERNAME
               value: "{{CLICKHOUSE_ADMIN_USER}}"
             - name: RALPH_BACKENDS__DATABASE__CLICKHOUSE__XAPI_DATABASE
               value: "{{ASPECTS_XAPI_DATABASE}}"
             - name: RALPH_RUNSERVER_BACKEND
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.3.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 - name: aspects-scripts
-  files:{% for file in "aspects/apps/scripts"|walk_templates %}
+  files:{% for file in "aspects/apps/aspects/scripts"|walk_templates %}
   - plugins/{{ file }}{% endfor %}
   options:
     labels:
         app.kubernetes.io/name: aspects
+- name: aspects-dbt
+  files:{% for file in "aspects/apps/aspects/dbt"|walk_templates %}
+  - plugins/{{ file }}{% endfor %}
+  options:
+    labels:
+        app.kubernetes.io/name: aspects
+
 {% if RUN_CLICKHOUSE %}
 - name: clickhouse-settings
   files:
     - plugins/aspects/apps/clickhouse/config/docker_config.xml
   options:
     labels:
         app.kubernetes.io/name: clickhouse
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-services`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     environment:
         CLICKHOUSE_DB: xapi
         CLICKHOUSE_USER: "{{ CLICKHOUSE_ADMIN_USER }}"
         CLICKHOUSE_PASSWORD: "{{ CLICKHOUSE_ADMIN_PASSWORD }}"
         CLICKHOUSE_DEFAULT_ACCESS_MANAGEMENT: 1
     ports:
         - 8123:{{ CLICKHOUSE_HTTP_PORT }}
-        - 9000:{{ CLICKHOUSE_PORT }}
+        - 9000:{{ CLICKHOUSE_CLIENT_PORT }}
     ulimits:
         nofile:
             soft: 262144
             hard: 262144
     volumes:
         - ../../data/clickhouse:/var/lib/clickhouse/
         - ../../env/plugins/aspects/apps/clickhouse/config:/etc/clickhouse-server/config.d/
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.3.0/tutoraspects/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         ("DOCKER_IMAGE_RALPH", "fundocker/ralph:3.8.0"),
         ("DOCKER_IMAGE_SUPERSET", "edunext/aspects-superset:{{ ASPECTS_VERSION }}"),
         ("DOCKER_IMAGE_VECTOR", "timberio/vector:0.30.0-alpine"),
         (
             "OPENEDX_EXTRA_PIP_REQUIREMENTS",
             [
                 "openedx-event-sink-clickhouse==0.1.0",
-                "edx-event-routing-backends==5.3.1",
+                "edx-event-routing-backends==5.5.0",
             ],
         ),
         # ClickHouse xAPI settings
         ("ASPECTS_XAPI_DATABASE", "xapi"),
         ("ASPECTS_RAW_XAPI_TABLE", "xapi_events_all"),
         ("ASPECTS_XAPI_TRANSFORM_MV", "xapi_events_all_parsed_mv"),
         ("ASPECTS_XAPI_TABLE", "xapi_events_all_parsed"),
@@ -68,17 +68,28 @@
         ("ASPECTS_VECTOR_DATABASE", "openedx"),
         ("ASPECTS_VECTOR_RAW_TRACKING_LOGS_TABLE", "_tracking"),
         ("ASPECTS_VECTOR_RAW_XAPI_TABLE", "xapi_events_all"),
         # Make sure LMS / CMS have event-routing-backends installed
         ######################
         # ClickHouse Settings
         ("CLICKHOUSE_HOST", "clickhouse"),
-        ("CLICKHOUSE_PORT", "9000"),
+        ("CLICKHOUSE_CLIENT_HTTP_PORT", "9000"),
+        ("CLICKHOUSE_CLIENT_HTTPS_PORT", "9440"),
+        (
+            "CLICKHOUSE_CLIENT_PORT",
+            "{% if CLICKHOUSE_SECURE_CONNECTION %}"
+            "{{CLICKHOUSE_CLIENT_HTTPS_PORT}}{% else %}{{CLICKHOUSE_CLIENT_HTTP_PORT}}{% endif %}",
+        ),
         ("CLICKHOUSE_HTTP_PORT", "8123"),
         ("CLICKHOUSE_HTTPS_PORT", "8443"),
+        (
+            "CLICKHOUSE_PORT",
+            "{% if CLICKHOUSE_SECURE_CONNECTION %}"
+            "{{CLICKHOUSE_HTTPS_PORT}}{% else %}{{CLICKHOUSE_HTTP_PORT}}{% endif %}",
+        ),
         # This can be used to override some configuration values in
         # via "docker_config.xml" file, which will be read from a
         # mount on /etc/clickhouse-server/config.d/ on startup.
         # See https://clickhouse.com/docs/en/operations/configuration-files
         #
         # This default allows connecting to Clickhouse when run as a
         # standalone docker container, instead of through docker-compose.
@@ -86,14 +97,27 @@
             "CLICKHOUSE_EXTRA_XML_CONFIG",
             """
     <listen_host>::</listen_host>
     <listen_host>0.0.0.0</listen_host>
     <listen_try>1</listen_try>
         """,
         ),
+        (
+            "CLICKHOUSE_URL",
+            "{{CLICKHOUSE_HOST}}:{{CLICKHOUSE_PORT}}",
+        ),
+        (
+            "CLICKHOUSE_REPORT_URL",
+            "{{ASPECTS_CLICKHOUSE_REPORT_USER}}:{{ASPECTS_CLICKHOUSE_REPORT_PASSWORD}}"
+            "@{{CLICKHOUSE_URL}}/{{ASPECTS_XAPI_DATABASE}}",
+        ),
+        (
+            "CLICKHOUSE_REPORT_SQLALCHEMY_URI",
+            "clickhousedb+connect://{{CLICKHOUSE_REPORT_URL}}",
+        ),
         ######################
         # Ralph Settings
         # Change to https:// if the public interface to it is secure
         ("RALPH_HOST", "ralph"),
         ("RALPH_PORT", "8100"),
         ("RALPH_ENABLE_PUBLIC_URL", False),
         ("RALPH_RUN_HTTPS", False),
@@ -145,35 +169,38 @@
         (
             "SUPERSET_SUPPORTED_LANGUAGES",
             {
                 "en": {"flag": "us", "name": "English"},
                 "es": {"flag": "es", "name": "Spanish"},
             },
         ),
+        ("SUPERSET_EXTRA_JINJA_FILTERS", {}),
         ######################
         # dbt Settings
         # For the most part you shouldn't have to touch these
         # DBT_PROFILE_* settings get passed into the dbt_profile.yml file.
         # For now we are pulling this from github, which should allow maximum
         # flexibility for forking, running branches, specific versions, etc.
         ("DBT_REPOSITORY", "https://github.com/openedx/aspects-dbt"),
         ("DBT_BRANCH", "main"),
         # Path to the dbt project inside the repository
         ("DBT_REPOSITORY_PATH", "aspects-dbt/aspects"),
         # This is a pip compliant list of Python packages to install to run dbt
         # make sure packages with versions are enclosed in double quotes
         ("EXTRA_DBT_PACKAGES", []),
+        # This is the name of the database dbt will write to
+        ("DBT_PROFILE_TARGET_DATABASE", "reporting"),
         # If set, DDL/table operations will be executed with the `ON CLUSTER` clause
         # using this cluster. This has not been tested with Aspects and is unlikely to
         # work.
         ("DBT_PROFILE_CLUSTER", ""),
         # Validate TLS certificate if using TLS/SSL
         ("DBT_PROFILE_VERIFY", "True"),
         # Use TLS (native protocol) or HTTPS (http protocol)
-        ("DBT_PROFILE_SECURE", "False"),
+        ("DBT_PROFILE_SECURE", "{{ CLICKHOUSE_SECURE_CONNECTION }}"),
         # Number of times to retry a "retryable" database exception (such as a 503
         # 'Service Unavailable' error)
         ("DBT_PROFILE_RETRIES", "3"),
         # Use gzip compression if truthy (http), or compression type for a native
         # connection
         ("DBT_PROFILE_COMPRESSION", "lz4"),
         # Timeout in seconds to establish a connection to ClickHouse
@@ -404,17 +431,17 @@
     """
     Job that loads bogus test xAPI data to ClickHouse via Ralph.
     """
     return [
         (
             "aspects",
             "echo 'Making demo xapi script executable...' && "
-            "chmod +x /app/aspects/scripts/aspects/clickhouse-demo-xapi-data.sh && "
+            "chmod +x /app/aspects/scripts/clickhouse-demo-xapi-data.sh && "
             "echo 'Done. Running script...' && "
-            f"bash /app/aspects/scripts/aspects/clickhouse-demo-xapi-data.sh {num_batches}"
+            f"bash /app/aspects/scripts/clickhouse-demo-xapi-data.sh {num_batches}"
             f" {batch_size} && "
             "echo 'Done!';",
         ),
     ]
 
 
 # Ex: "tutor local do dbt "
@@ -439,17 +466,17 @@
     """
     Job that proxies dbt commands to a container which runs them against ClickHouse.
     """
     return [
         (
             "aspects",
             "echo 'Making dbt script executable...' && "
-            "chmod +x /app/aspects/scripts/aspects/dbt.sh && "
+            "chmod +x /app/aspects/scripts/dbt.sh && "
             f"echo 'Running dbt {command}' && "
-            f"bash /app/aspects/scripts/aspects/dbt.sh {command} && "
+            f"bash /app/aspects/scripts/dbt.sh {command} && "
             "echo 'Done!';",
         ),
     ]
 
 
 # Add the command function to CLI_DO_COMMANDS:
 hooks.Filters.CLI_DO_COMMANDS.add_item(load_xapi_test_data)
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Configuration
 RALPH_APP_DIR=/app/.ralph
 
 # ClickHouse database backend
 RALPH_BACKENDS__DATABASE__CLICKHOUSE__HOST={{CLICKHOUSE_HOST}}
-RALPH_BACKENDS__DATABASE__CLICKHOUSE__PORT={% if CLICKHOUSE_SECURE_CONNECTION%}{{CLICKHOUSE_HTTPS_PORT}}{% else %}{{CLICKHOUSE_HTTP_PORT}}{% endif %}
-RALPH_BACKENDS__DATABASE__CLICKHOUSE__XAPI_DATABASE={{ASPECTS_XAPI_DATABASE}}
+RALPH_BACKENDS__DATABASE__CLICKHOUSE__PORT={{CLICKHOUSE_PORT}}
+RALPH_BACKENDS__DATABASE__CLICKHOUSE__DATABASE={{ASPECTS_XAPI_DATABASE}}
 RALPH_BACKENDS__DATABASE__CLICKHOUSE__EVENT_TABLE_NAME={{ASPECTS_RAW_XAPI_TABLE}}
 RALPH_BACKENDS__DATABASE__CLICKHOUSE__TEST_HOST=clickhouse
 RALPH_BACKENDS__DATABASE__CLICKHOUSE__USERNAME={{CLICKHOUSE_ADMIN_USER}}
 RALPH_BACKENDS__DATABASE__CLICKHOUSE__PASSWORD={{CLICKHOUSE_ADMIN_PASSWORD}}
 
 # LRS API
 RALPH_RUNSERVER_BACKEND=clickhouse
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/scripts/aspects/clickhouse-demo-xapi-data.sh` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 . virtualenv/bin/activate
 
 echo "Loading demo xAPI data..."
 xapi-db-load --backend ralph_clickhouse \
     --num_batches $1 \
     --batch_size $2 \
     --db_host "{{ CLICKHOUSE_HOST }}" \
-    --db_port "{{ CLICKHOUSE_HTTP_PORT }}" \
+    --db_port "{{ CLICKHOUSE_PORT }}" \
     --db_username "{{ CLICKHOUSE_ADMIN_USER }}" \
     --db_password "{{ CLICKHOUSE_ADMIN_PASSWORD }}" \
     --db_name "{{ ASPECTS_XAPI_DATABASE }}" \
     --lrs_url "{% if RUN_RALPH %}http://ralph:{{ RALPH_PORT }}{% else %}{% if RALPH_RUN_HTTPS %}https://{% else %}http://{% endif %}{{ RALPH_HOST }}{% endif %}/xAPI/statements/" \
     --lrs_username "{{RALPH_LMS_USERNAME}}" \
     --lrs_password "{{RALPH_LMS_PASSWORD}}"
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/scripts/aspects/profiles.yml` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 aspects: # this needs to match the profile in your dbt_project.yml file
   target: dev
   outputs:
     dev:
       type: clickhouse
-      schema: {{ ASPECTS_XAPI_DATABASE }}
+      schema: {{ DBT_PROFILE_TARGET_DATABASE }}
       host: {{ CLICKHOUSE_HOST }}
-      port: {{ CLICKHOUSE_HTTP_PORT }}
+      port: {{ CLICKHOUSE_PORT }}
       user: {{ CLICKHOUSE_ADMIN_USER }}
       password: '{{ CLICKHOUSE_ADMIN_PASSWORD }}'
 
       # These are ClickHouse provider values and map directly to ClickHouse connection settings.
       cluster: {{ DBT_PROFILE_CLUSTER }}
       verify: {{ DBT_PROFILE_VERIFY }}
       secure: {{ DBT_PROFILE_SECURE }}
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -583,23 +583,429 @@
   slice_name: xAPI events by course
   uuid: c69ab610-f77a-4c54-a5ab-dc3a19a3003e
   version: 1.0.0
   viz_type: echarts_timeseries_bar
 
 - _file_name: OpenedX_Clickhouse.yaml
   database_name: OpenedX Clickhouse
-  sqlalchemy_uri: clickhousedb+connect://{{ASPECTS_CLICKHOUSE_REPORT_USER}}:{{ASPECTS_CLICKHOUSE_REPORT_PASSWORD}}@{{CLICKHOUSE_HOST}}:{% if CLICKHOUSE_SECURE_CONNECTION%}{{CLICKHOUSE_HTTPS_PORT}}{% else %}{{CLICKHOUSE_HTTP_PORT}}{% endif %}/{{ASPECTS_XAPI_DATABASE}}
+  sqlalchemy_uri: {{CLICKHOUSE_REPORT_SQLALCHEMY_URI}}
   cache_timeout: null
   expose_in_sqllab: true
   allow_run_async: false
   allow_ctas: false
   allow_cvas: false
   allow_csv_upload: false
   extra:
     allows_virtual_table_explore: true
     metadata_params: {}
     engine_params: {}
     schemas_allowed_for_csv_upload: []
   uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
   version: 1.0.0
 
+- _file_name: video_plays.yaml
+  cache_timeout: null
+  columns:
+  - advanced_data_type: null
+    column_name: emission_time
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: true
+    python_date_format: null
+    type: DateTime64(6)
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: actor_id
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: course_id
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: video_id
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: org
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
+  default_endpoint: null
+  description: null
+  extra: null
+  fetch_values_predicate: null
+  filter_select_enabled: false
+  main_dttm_col: emission_time
+  metrics:
+  - d3format: null
+    description: null
+    expression: COUNT(distinct actor_id)
+    extra: {}
+    metric_name: distinct_plays
+    metric_type: null
+    verbose_name: Unique video watchers
+    warning_text: null
+  - d3format: null
+    description: null
+    expression: COUNT(*)
+    extra:
+      warning_markdown: ''
+    metric_name: count
+    metric_type: count
+    verbose_name: Total video watches
+    warning_text: null
+  offset: 0
+  params: null
+  schema: {{ DBT_PROFILE_TARGET_DATABASE }}
+  sql: ''
+  table_name: video_plays
+  template_params: null
+  uuid: 14b6e4d0-7345-4477-9a11-85a7359bc3b1
+  version: 1.0.0
+
+- _file_name: transcript_usage.yaml
+  cache_timeout: null
+  columns:
+  - advanced_data_type: null
+    column_name: emission_time
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: true
+    python_date_format: null
+    type: DateTime64(6)
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: actor_id
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: course_id
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: video_id
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: org
+    description: null
+    expression: null
+    extra: {}
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
+  default_endpoint: null
+  description: null
+  extra: null
+  fetch_values_predicate: null
+  filter_select_enabled: false
+  main_dttm_col: emission_time
+  metrics:
+  - d3format: null
+    description: null
+    expression: COUNT(distinct actor_id)
+    extra: {}
+    metric_name: distinct_learners
+    metric_type: null
+    verbose_name: distinct actor_id
+    warning_text: null
+  - d3format: null
+    description: null
+    expression: COUNT(*)
+    extra:
+      warning_markdown: ''
+    metric_name: count
+    metric_type: count
+    verbose_name: COUNT(*)
+    warning_text: null
+  offset: 0
+  params: null
+  schema: {{ DBT_PROFILE_TARGET_DATABASE }}
+  sql: ''
+  table_name: transcript_usage
+  template_params: null
+  uuid: bfbc2c72-4745-40ff-a7db-786711b90321
+  version: 1.0.0
+
+- _file_name: Instructor_dashboard_4.yaml
+  css: ''
+  dashboard_title: Instructor dashboard
+  description: null
+  metadata:
+    chart_configuration: {}
+    color_scheme: ''
+    default_filters: '{}'
+    expanded_slices: {}
+    label_colors: {}
+    native_filter_configuration:
+    - cascadeParentIds: []
+      chartsInScope:
+      - 12
+      controlValues:
+        defaultToFirstItem: true
+        enableEmptyFilter: true
+        inverseSelection: false
+        multiSelect: true
+        searchAllOptions: false
+      defaultDataMask:
+        extraFormData: {}
+        filterState: {}
+        ownState: {}
+      description: ''
+      filterType: filter_select
+      id: NATIVE_FILTER-Vx7HxG8_7
+      name: org
+      requiredFirst: true
+      scope:
+        excluded: []
+        rootPath:
+        - ROOT_ID
+      tabsInScope: []
+      targets:
+      - column:
+          name: org
+        datasetUuid: 14b6e4d0-7345-4477-9a11-85a7359bc3b1
+      type: NATIVE_FILTER
+    - cascadeParentIds:
+      - NATIVE_FILTER-Vx7HxG8_7
+      chartsInScope:
+      - 13
+      controlValues:
+        defaultToFirstItem: true
+        enableEmptyFilter: true
+        inverseSelection: false
+        multiSelect: true
+        searchAllOptions: false
+      defaultDataMask:
+        extraFormData: {}
+        filterState: {}
+        ownState: {}
+      description: ''
+      filterType: filter_select
+      id: NATIVE_FILTER-XPuiTOej4
+      name: course_id
+      requiredFirst: true
+      scope:
+        excluded: []
+        rootPath:
+        - ROOT_ID
+      tabsInScope: []
+      targets:
+      - column:
+          name: course_id
+        datasetUuid: 14b6e4d0-7345-4477-9a11-85a7359bc3b1
+      type: NATIVE_FILTER
+    refresh_frequency: 0
+    shared_label_colors: {}
+    show_native_filters: true
+    timed_refresh_immune_slices: []
+  position:
+    CHART-qKje4F2Q8q:
+      children: []
+      id: CHART-qKje4F2Q8q
+      meta:
+        chartId: 13
+        height: 51
+        sliceName: Watches per video
+        uuid: eaa6dad7-df51-4e51-b300-6baf30b8e330
+        width: 12
+      parents:
+      - ROOT_ID
+      - GRID_ID
+      - ROW-DxLgJisWQW
+      type: CHART
+    CHART-yJYiCvzxJX:
+      children: []
+      id: CHART-yJYiCvzxJX
+      meta:
+        chartId: 14
+        height: 50
+        sliceName: Transcript/closed captioning usage per video
+        uuid: 5593cd9b-81d4-4b9f-b4a7-cd377c92c5e6
+        width: 12
+      parents:
+      - ROOT_ID
+      - GRID_ID
+      - ROW-porCi0mdxp
+      type: CHART
+    DASHBOARD_VERSION_KEY: v2
+    GRID_ID:
+      children:
+      - ROW-DxLgJisWQW
+      - ROW-porCi0mdxp
+      id: GRID_ID
+      parents:
+      - ROOT_ID
+      type: GRID
+    HEADER_ID:
+      id: HEADER_ID
+      meta:
+        text: Instructor dashboard
+      type: HEADER
+    ROOT_ID:
+      children:
+      - GRID_ID
+      id: ROOT_ID
+      type: ROOT
+    ROW-DxLgJisWQW:
+      children:
+      - CHART-qKje4F2Q8q
+      id: ROW-DxLgJisWQW
+      meta:
+        background: BACKGROUND_TRANSPARENT
+      parents:
+      - ROOT_ID
+      - GRID_ID
+      type: ROW
+    ROW-porCi0mdxp:
+      children:
+      - CHART-yJYiCvzxJX
+      id: ROW-porCi0mdxp
+      meta:
+        background: BACKGROUND_TRANSPARENT
+      parents:
+      - ROOT_ID
+      - GRID_ID
+      type: ROW
+  slug: null
+  uuid: 1d6bf904-f53f-47fd-b1c9-6cd7e284d286
+  version: 1.0.0
+
+- _file_name: Watches_per_video_12.yaml
+  cache_timeout: null
+  dataset_uuid: 14b6e4d0-7345-4477-9a11-85a7359bc3b1
+  params:
+    adhoc_filters: []
+    bar_stacked: true
+    bottom_margin: auto
+    color_scheme: supersetColors
+    columns: []
+    datasource: 6__table
+    extra_form_data: {}
+    granularity_sqla: emission_time
+    groupby:
+    - video_id
+    metrics:
+    - distinct_plays
+    - count
+    order_desc: true
+    rich_tooltip: true
+    row_limit: 10000
+    show_legend: true
+    time_range: No filter
+    viz_type: dist_bar
+    x_ticks_layout: auto
+    y_axis_bounds:
+    - null
+    - null
+    y_axis_format: SMART_NUMBER
+  slice_name: Watches per video
+  uuid: eaa6dad7-df51-4e51-b300-6baf30b8e330
+  version: 1.0.0
+  viz_type: dist_bar
+
+- _file_name: Transcript_closed_captioning_usage_per_video_14.yaml
+  cache_timeout: null
+  dataset_uuid: bfbc2c72-4745-40ff-a7db-786711b90321
+  params:
+    adhoc_filters: []
+    bar_stacked: true
+    bottom_margin: auto
+    color_scheme: supersetColors
+    columns: []
+    datasource: 8__table
+    extra_form_data: {}
+    granularity_sqla: emission_time
+    groupby:
+    - video_id
+    metrics:
+    - distinct_learners
+    - count
+    order_desc: true
+    rich_tooltip: true
+    row_limit: 10000
+    show_legend: true
+    time_range: No filter
+    viz_type: dist_bar
+    x_ticks_layout: auto
+    y_axis_bounds:
+    - null
+    - null
+    y_axis_format: SMART_NUMBER
+  slice_name: Transcript/closed captioning usage per video
+  uuid: 5593cd9b-81d4-4b9f-b4a7-cd377c92c5e6
+  version: 1.0.0
+  viz_type: dist_bar
+
+
+
 {{ patch("superset-extra-assets") }}
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,7 +34,9 @@
     # TODO: what happens when the list of courses grows beyond what the query will handle?
     if courses:
         course_id_list = ", ".join(f"'{course_id}'" for course_id in courses)
         return f"{field_name} in ({course_id_list})"
     else:
         # If you're not course staff on any courses, you don't get to see any.
         return NO_COURSES
+
+{{ patch("superset-jinja-filters") }}
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,18 +72,19 @@
 FEATURE_FLAGS = {
     "ALERT_REPORTS": True,
     "ENABLE_TEMPLATE_PROCESSING": True,
     "DASHBOARD_RBAC": True,
 }
 
 # Add this custom template processor which returns the list of courses the current user can access
-from openedx_jinja_filters import can_view_courses
+from openedx_jinja_filters import *
 
 JINJA_CONTEXT_ADDONS = {
     'can_view_courses': can_view_courses,
+    {% for filter in SUPERSET_EXTRA_JINJA_FILTERS %}'{{ filter }}': {{filter}},{% endfor %}
 }
 
 {% if not ENABLE_WEB_PROXY %}
 # Caddy is running behind a proxy: Superset needs to handle x-forwarded-* headers
 # https://flask.palletsprojects.com/en/latest/deploying/proxy_fix/
 ENABLE_PROXY_FIX = True
 {% endif %}
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files 6% similar despite different names*

```diff
@@ -87,28 +87,28 @@
 type = "clickhouse"
 auth.strategy = "basic"
 auth.user = "{{ ASPECTS_CLICKHOUSE_VECTOR_USER }}"
 auth.password = "{{ ASPECTS_CLICKHOUSE_VECTOR_PASSWORD }}"
 # Required: https://github.com/timberio/vector/issues/5797
 encoding.timestamp_format = "unix"
 inputs = ["tracking"]
-endpoint = "{{ CLICKHOUSE_HOST }}:{{ CLICKHOUSE_HTTP_PORT }}"
+endpoint = "{% if CLICKHOUSE_SECURE_CONNECTION %}https{% else %}http{% endif %}://{{ CLICKHOUSE_HOST }}:{{ CLICKHOUSE_PORT }}"
 database = "{{ ASPECTS_VECTOR_DATABASE }}"
 table = "{{ ASPECTS_VECTOR_RAW_TRACKING_LOGS_TABLE }}"
 healthcheck = true
 
 [sinks.clickhouse_xapi]
 type = "clickhouse"
 auth.strategy = "basic"
 auth.user = "{{ ASPECTS_CLICKHOUSE_VECTOR_USER }}"
 auth.password = "{{ ASPECTS_CLICKHOUSE_VECTOR_PASSWORD }}"
 # Required: https://github.com/timberio/vector/issues/5797
 encoding.timestamp_format = "unix"
 # Allows better parsing of date times
 date_time_best_effort = true
 inputs = ["xapi"]
-endpoint = "{{ CLICKHOUSE_HOST }}:{{ CLICKHOUSE_HTTP_PORT }}"
+endpoint = "{% if CLICKHOUSE_SECURE_CONNECTION %}https{% else %}http{% endif %}://{{ CLICKHOUSE_HOST }}:{{ CLICKHOUSE_PORT }}"
 database = "{{ ASPECTS_VECTOR_DATABASE }}"
 table = "{{ ASPECTS_VECTOR_RAW_XAPI_TABLE }}"
 healthcheck = true
 
 {{ patch("vector-common-toml") }}
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 echo "Initialising Clickhouse..."
 ch_connection_max_attempts=10
 ch_connection_attempt=0
-until clickhouse client --user {{ CLICKHOUSE_ADMIN_USER }} --password="{{ CLICKHOUSE_ADMIN_PASSWORD }}" --host "{{ CLICKHOUSE_HOST }}" {% if CLICKHOUSE_SECURE_CONNECTION %} --secure {% else %} --port {{ CLICKHOUSE_PORT }}{% endif %} -q 'exit'
+until clickhouse client --user {{ CLICKHOUSE_ADMIN_USER }} --password="{{ CLICKHOUSE_ADMIN_PASSWORD }}" --host "{{ CLICKHOUSE_HOST }}" {% if CLICKHOUSE_SECURE_CONNECTION %} --secure {% else %} --port {{ CLICKHOUSE_CLIENT_PORT }}{% endif %} -q 'exit'
 do
     ch_connection_attempt=$(expr $ch_connection_attempt + 1)
     echo "    [$ch_connection_attempt/$ch_connection_max_attempts] Waiting for Clickhouse service (this may take a while)..."
     if [ $ch_connection_attempt -eq $ch_connection_max_attempts ]
     then
       echo "Clickhouse initialisation error" 1>&2
       exit 1
     fi
     sleep 10
 done
 echo "Clickhouse is up and running"
 
 echo "Running schema creation scripts..."
-clickhouse client --user "{{ CLICKHOUSE_ADMIN_USER }}" --password="{{ CLICKHOUSE_ADMIN_PASSWORD }}" --host "{{ CLICKHOUSE_HOST }}" {% if CLICKHOUSE_SECURE_CONNECTION %} --secure {% else %} --port {{ CLICKHOUSE_PORT }}{% endif %} --multiquery <<'EOF'
+clickhouse client --user "{{ CLICKHOUSE_ADMIN_USER }}" --password="{{ CLICKHOUSE_ADMIN_PASSWORD }}" --host "{{ CLICKHOUSE_HOST }}" {% if CLICKHOUSE_SECURE_CONNECTION %} --secure {% else %} --port {{ CLICKHOUSE_CLIENT_PORT }}{% endif %} --multiquery <<'EOF'
 -- Allow JSON fields
 SET allow_experimental_object_type=1;
 
 -- Create various non-admin users reporting users
 CREATE USER IF NOT EXISTS {{ ASPECTS_CLICKHOUSE_LRS_USER }} IDENTIFIED WITH sha256_password BY '{{ ASPECTS_CLICKHOUSE_LRS_PASSWORD }}';
 CREATE USER IF NOT EXISTS {{ ASPECTS_CLICKHOUSE_VECTOR_USER }} IDENTIFIED WITH sha256_password BY '{{ ASPECTS_CLICKHOUSE_VECTOR_PASSWORD }}';
 CREATE USER IF NOT EXISTS {{ ASPECTS_CLICKHOUSE_REPORT_USER }} IDENTIFIED WITH sha256_password BY '{{ ASPECTS_CLICKHOUSE_REPORT_PASSWORD }}';
@@ -336,14 +336,18 @@
 -- Grant permissions to the users
 GRANT INSERT, SELECT ON {{ ASPECTS_XAPI_DATABASE }}.* TO '{{ ASPECTS_CLICKHOUSE_LRS_USER }}';
 GRANT SELECT ON {{ ASPECTS_XAPI_DATABASE }}.* TO '{{ ASPECTS_CLICKHOUSE_REPORT_USER }}';
 
 GRANT INSERT, SELECT ON {{ ASPECTS_EVENT_SINK_DATABASE }}.* TO '{{ ASPECTS_CLICKHOUSE_CMS_USER }}';
 GRANT SELECT ON {{ ASPECTS_EVENT_SINK_DATABASE }}.* TO '{{ ASPECTS_CLICKHOUSE_REPORT_USER }}';
 
+-- Create dbt database and grant permissions
+CREATE DATABASE IF NOT EXISTS {{ DBT_PROFILE_TARGET_DATABASE }};
+GRANT CREATE TABLE, DROP TABLE, CREATE VIEW, DROP VIEW, SELECT, INSERT, UPDATE, DELETE ON {{ DBT_PROFILE_TARGET_DATABASE }}.* TO '{{ ASPECTS_CLICKHOUSE_REPORT_USER }}';
+
 -- Vector database and tables
 -- This is just temporary so that Vector has a place to write. Once these are all Alembic migrations
 -- it will be a lot more sane.
 CREATE DATABASE IF NOT EXISTS {{ ASPECTS_VECTOR_DATABASE }};
 
 CREATE TABLE IF NOT EXISTS {{ ASPECTS_VECTOR_DATABASE }}.{{ ASPECTS_VECTOR_RAW_TRACKING_LOGS_TABLE }}
 (
```

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.1.1/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.3.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

