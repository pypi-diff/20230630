# Comparing `tmp/flask-rebar-2.4.0.tar.gz` & `tmp/flask-rebar-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-rebar-2.4.0.tar", last modified: Tue May 16 17:29:34 2023, max compression
+gzip compressed data, was "flask-rebar-2.4.1.tar", last modified: Fri Jun 30 18:44:49 2023, max compression
```

## Comparing `flask-rebar-2.4.0.tar` & `flask-rebar-2.4.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.750270 flask-rebar-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-16 17:29:34.750270 flask-rebar-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.718270 flask-rebar-2.4.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.722270 flask-rebar-2.4.0/examples/todo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/generate_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.722270 flask-rebar-2.4.0/examples/todo/todo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.722270 flask-rebar-2.4.0/examples/todo/todo/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/handlers/todo_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/authenticators/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/authenticators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/authenticators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/authenticators/header_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/rebar.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/request_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/swagger_generation/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/authenticator_to_swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/marshmallow_to_swagger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_words.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/swagger_ui/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.746270 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/oauth2-redirect.html
--rw-r--r--   0 runner    (1001) docker     (123)  1534401 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123) 11349827 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   330779 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)  2226997 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    33055 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   349441 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)  2222505 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.746270 flask-rebar-2.4.0/flask_rebar/swagger_ui/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/templates/index.html.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.746270 flask-rebar-2.4.0/flask_rebar/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85712 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/testing/swagger_jsonschema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.746270 flask-rebar-2.4.0/flask_rebar/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/marshmallow_objects_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 17:29:34.750270 flask-rebar-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.750270 flask-rebar-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_deprecation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29629 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_rebar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_request_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.395123 flask-rebar-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-30 18:44:49.395123 flask-rebar-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.371123 flask-rebar-2.4.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.371123 flask-rebar-2.4.1/examples/todo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/examples/todo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/examples/todo/generate_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.375123 flask-rebar-2.4.1/examples/todo/todo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/examples/todo/todo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/examples/todo/todo/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/examples/todo/todo/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.375123 flask-rebar-2.4.1/examples/todo/todo/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/examples/todo/todo/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/examples/todo/todo/handlers/todo_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/examples/todo/todo/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/examples/todo/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.375123 flask-rebar-2.4.1/flask_rebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.375123 flask-rebar-2.4.1/flask_rebar/authenticators/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/authenticators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/authenticators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/authenticators/header_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/rebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/request_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.375123 flask-rebar-2.4.1/flask_rebar/swagger_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/authenticator_to_swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20720 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/marshmallow_to_swagger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.375123 flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_generator_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_generator_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_words.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.375123 flask-rebar-2.4.1/flask_rebar/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.391123 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1534401 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123) 11349827 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   330779 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2226997 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    33055 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   349441 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2222505 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.395123 flask-rebar-2.4.1/flask_rebar/swagger_ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/swagger_ui/templates/index.html.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.395123 flask-rebar-2.4.1/flask_rebar/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85712 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/testing/swagger_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.395123 flask-rebar-2.4.1/flask_rebar/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/utils/marshmallow_objects_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/utils/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/flask_rebar/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.375123 flask-rebar-2.4.1/flask_rebar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-30 18:44:49.000000 flask-rebar-2.4.1/flask_rebar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-30 18:44:49.000000 flask-rebar-2.4.1/flask_rebar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:44:49.000000 flask-rebar-2.4.1/flask_rebar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-30 18:44:49.000000 flask-rebar-2.4.1/flask_rebar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 18:44:49.000000 flask-rebar-2.4.1/flask_rebar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 18:44:49.395123 flask-rebar-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:49.395123 flask-rebar-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/tests/test_deprecation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29561 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/tests/test_rebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/tests/test_request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-06-30 18:44:44.000000 flask-rebar-2.4.1/tests/test_validation.py
```

### Comparing `flask-rebar-2.4.0/LICENSE` & `flask-rebar-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/PKG-INFO` & `flask-rebar-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rebar
-Version: 2.4.0
+Version: 2.4.1
 Summary: Flask-Rebar combines flask, marshmallow, and swagger for robust REST services.
 Home-page: https://github.com/plangrid/flask-rebar
 Author: Barak Alon
 Author-email: barak.s.alon@gmail.com
 License: MIT
 Keywords: flask,rest,marshmallow,openapi,swagger
 Classifier: Environment :: Web Environment
```

### Comparing `flask-rebar-2.4.0/README.rst` & `flask-rebar-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/examples/todo/generate_output.py` & `flask-rebar-2.4.1/examples/todo/generate_output.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/examples/todo/todo/app.py` & `flask-rebar-2.4.1/examples/todo/todo/app.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/examples/todo/todo/handlers/todo_handlers.py` & `flask-rebar-2.4.1/examples/todo/todo/handlers/todo_handlers.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/examples/todo/todo/schemas.py` & `flask-rebar-2.4.1/examples/todo/todo/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/__init__.py` & `flask-rebar-2.4.1/flask_rebar/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/authenticators/base.py` & `flask-rebar-2.4.1/flask_rebar/authenticators/base.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/authenticators/header_api_key.py` & `flask-rebar-2.4.1/flask_rebar/authenticators/header_api_key.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/compat.py` & `flask-rebar-2.4.1/flask_rebar/compat.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/errors.py` & `flask-rebar-2.4.1/flask_rebar/errors.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/messages.py` & `flask-rebar-2.4.1/flask_rebar/messages.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/rebar.py` & `flask-rebar-2.4.1/flask_rebar/rebar.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_generation/__init__.py` & `flask-rebar-2.4.1/flask_rebar/swagger_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_generation/authenticator_to_swagger.py` & `flask-rebar-2.4.1/flask_rebar/swagger_generation/authenticator_to_swagger.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_generation/generator_utils.py` & `flask-rebar-2.4.1/flask_rebar/swagger_generation/generator_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_generation/marshmallow_to_swagger.py` & `flask-rebar-2.4.1/flask_rebar/swagger_generation/marshmallow_to_swagger.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,20 +299,20 @@
             jsonschema_obj["nullable"] = True
 
         return jsonschema_obj
 
     @sets_swagger_attr(sw.default)
     def get_default(self, obj, context):
         if (
-            obj.missing is not m.missing
+            obj.load_default is not m.missing
             # Marshmallow accepts a callable for the default. This is tricky
             # to handle, so let's just ignore this for now.
-            and not callable(obj.missing)
+            and not callable(obj.load_default)
         ):
-            return obj.missing
+            return obj.load_default
         else:
             return UNSET
 
     @sets_swagger_attr(sw.nullable)
     def get_nullable(self, obj, context):
         if context.openapi_version == 2 and obj.allow_none is not False:
             return True
```

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_base.py` & `flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_generator_base.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_v2.py` & `flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_generator_v2.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_v3.py` & `flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_generator_v3.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_objects.py` & `flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_objects.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_words.py` & `flask-rebar-2.4.1/flask_rebar/swagger_generation/swagger_words.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/blueprint.py` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/favicon-32x32.png` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/oauth2-redirect.html` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/static/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.css` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.js` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.js.map` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/static/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/swagger_ui/templates/index.html.jinja2` & `flask-rebar-2.4.1/flask_rebar/swagger_ui/templates/index.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/testing/swagger_jsonschema.py` & `flask-rebar-2.4.1/flask_rebar/testing/swagger_jsonschema.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/utils/deprecation.py` & `flask-rebar-2.4.1/flask_rebar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/utils/marshmallow_objects_helpers.py` & `flask-rebar-2.4.1/flask_rebar/utils/marshmallow_objects_helpers.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/utils/request_utils.py` & `flask-rebar-2.4.1/flask_rebar/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar/validation.py` & `flask-rebar-2.4.1/flask_rebar/validation.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/flask_rebar.egg-info/PKG-INFO` & `flask-rebar-2.4.1/flask_rebar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rebar
-Version: 2.4.0
+Version: 2.4.1
 Summary: Flask-Rebar combines flask, marshmallow, and swagger for robust REST services.
 Home-page: https://github.com/plangrid/flask-rebar
 Author: Barak Alon
 Author-email: barak.s.alon@gmail.com
 License: MIT
 Keywords: flask,rest,marshmallow,openapi,swagger
 Classifier: Environment :: Web Environment
```

### Comparing `flask-rebar-2.4.0/flask_rebar.egg-info/SOURCES.txt` & `flask-rebar-2.4.1/flask_rebar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/setup.py` & `flask-rebar-2.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 
 # packages required for local development and testing
 development = [
-    "black==22.3.0",
+    "black==23.3.0",
     "bumpversion==0.5.3",
     "click>=8.1.3,<9.0.0",
-    "flake8==4.0.1",
+    "flake8==6.0.0",
     "gitchangelog>=3.0.4,<4.0.0",
     "jsonschema==3.0.2",
     "marshmallow-objects~=2.3",
     "parametrize==0.1.1",
     "pre-commit>=1.14.4",
     "pytest~=6.2",
     "pytest-order~=1.0",
     "Sphinx==1.7.0",
     "sphinx_rtd_theme==0.2.4",
 ]
 
 if __name__ == "__main__":
     setup(
         name="flask-rebar",
-        version="2.4.0",
+        version="2.4.1",
         author="Barak Alon",
         author_email="barak.s.alon@gmail.com",
         description="Flask-Rebar combines flask, marshmallow, and swagger for robust REST services.",
         long_description=open("README.rst").read(),
         keywords=["flask", "rest", "marshmallow", "openapi", "swagger"],
         license="MIT",
         packages=find_packages(exclude=("test*", "examples")),
```

### Comparing `flask-rebar-2.4.0/tests/test_deprecation_utils.py` & `flask-rebar-2.4.1/tests/test_deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/tests/test_errors.py` & `flask-rebar-2.4.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/tests/test_rebar.py` & `flask-rebar-2.4.1/tests/test_rebar.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,23 +66,19 @@
 
 
 class FooListModel(mo.Model):
     name = mo.fields.String(required=True)
 
 
 class HeadersSchema(m.Schema):
-    name = set_data_key(
-        field=m.fields.String(load_from="x-name", required=True), key="x-name"
-    )
+    name = set_data_key(field=m.fields.String(required=True), key="x-name")
 
 
 class HeadersModel(mo.Model):
-    name = set_data_key(
-        field=mo.fields.String(load_from="x-name", required=True), key="x-name"
-    )
+    name = set_data_key(field=mo.fields.String(required=True), key="x-name")
 
 
 class MeSchema(m.Schema):
     user_name = m.fields.String()
 
 
 class DefaultResponseSchema(
```

### Comparing `flask-rebar-2.4.0/tests/test_request_utils.py` & `flask-rebar-2.4.1/tests/test_request_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.4.0/tests/test_validation.py` & `flask-rebar-2.4.1/tests/test_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 
 
 class RequireOnDumpMixinSchema(NoRequireOnDumpMixinSchema, RequireOnDumpMixin):
     pass
 
 
 class InnerNested(Schema, RequireOnDumpMixin):
-    inner_dump_only = fields.String(default="Inner dump-only", dump_only=True)
+    inner_dump_only = fields.String(dump_default="Inner dump-only", dump_only=True)
     inner_nested = fields.Nested(RequireOnDumpMixinSchema)
     inner_nested_dump_only = fields.Nested(RequireOnDumpMixinSchema, dump_only=True)
     inner_nested_list = fields.List(fields.Nested(RequireOnDumpMixinSchema))
     validated = fields.Integer(required=False, validate=Range(42, 99))
 
 
 class OuterNested(Schema, RequireOnDumpMixin):
-    outer_dump_only = fields.String(default="Outer dump-only", dump_only=True)
+    outer_dump_only = fields.String(dump_default="Outer dump-only", dump_only=True)
     nested = fields.Nested(InnerNested)
     nested_list = fields.List(fields.Nested(InnerNested))
 
 
 class OuterNestedNone(Schema, RequireOnDumpMixin):
     nested = fields.Nested(InnerNested, allow_none=True)
```

