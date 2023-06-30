# Comparing `tmp/djangofoundry-0.0.7.tar.gz` & `tmp/djangofoundry-0.0.8.tar.gz`

## Comparing `djangofoundry-0.0.7.tar` & `djangofoundry-0.0.8.tar`

### file list

```diff
@@ -1,122 +1,125 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/.dockerignore
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/.prospector.yaml
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/docker-compose.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/logging.conf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/package.json
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/requirements.txt
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/urls.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/controllers/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/controllers/angular.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/controllers/detail.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/controllers/generic.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/controllers/list.py
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/controllers/memory.py
--rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/controllers/responses.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/decorators/__init__.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/decorators/queryset_filter.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/decorators/retry.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/decorators/timeout.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/exceptions/__init__.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/exceptions/app.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/logging.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/progress.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/encoders/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/encoders/json.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/exceptions.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/hook.py
--rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/hooks.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/waypoint.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/meta/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/meta/constants.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/meta/types.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/queue/__init__.py
--rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/queue/queue.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/queue/signals.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/__init__.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/template.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/__init__.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/css.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/javascript.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/template.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/python/model.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/python/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/meta/__init__.py
--rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/helpers/render/meta/model.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/matching/__init__.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/matching/engine.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/matching/fuzzy/__init__.py
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/matching/fuzzy/thefuzz.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/mixins/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/mixins/dirtyfields.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/mixins/hasParams.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/mixins/hookable.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/mixins/jsonResponse.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/__init__.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/choices.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/manager.py
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/model.py
--rw-r--r--   0        0        0    53639 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/queryset.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/serializer.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/viewset.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/exceptions/__init__.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/exceptions/get.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/fields/__init__.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/fields/boolean.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/fields/char.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/fields/date.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/fields/number.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/fields/objects.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/models/fields/relationships.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/options/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/options/request.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/README.md
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/__init__.py
--rw-r--r--   0        0        0    20463 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/app.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/build.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/db.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/imports.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/lint.py
--rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/summarize.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/conf/sample-settings.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/utils/README.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/utils/__init__.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/utils/action.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/utils/exceptions.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/utils/settings.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/scripts/utils/types.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/signals/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/signals/abstract.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/templates/memory.html
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/templates/angular/base.html
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/templates/jinja/model.py.jinja
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/templatetags/__init__.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/src/djangofoundry/templatetags/syntax_highlight.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/test_matching.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/controllers/__init__.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/controllers/test_mixins.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/decorators/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/decorators/test_timeout.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/helpers/__init__.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/helpers/test_hooks.py
--rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/helpers/test_queue.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/models/__init__.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/models/test_choices.py
--rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/tests/foundry/models/test_queryset.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/.gitignore
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/LICENSE.md
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/README.md
--rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/.dockerignore
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/.prospector.yaml
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/docker-compose.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/logging.conf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/package.json
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/urls.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/controllers/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/controllers/angular.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/controllers/detail.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/controllers/generic.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/controllers/list.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/controllers/memory.py
+-rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/controllers/responses.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/decorators/__init__.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/decorators/queryset_filter.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/decorators/retry.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/decorators/timeout.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/exceptions/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/exceptions/app.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/logging.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/progress.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/encoders/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/encoders/json.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/exceptions.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/hook.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/hooks.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/waypoint.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/meta/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/meta/constants.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/meta/types.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/queue/__init__.py
+-rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/queue/queue.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/queue/signals.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/__init__.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/template.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/__init__.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/__init__.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/css.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/javascript.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/template.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/python/model.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/python/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/meta/__init__.py
+-rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/helpers/render/meta/model.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/matching/__init__.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/matching/engine.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/matching/fuzzy/__init__.py
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/matching/fuzzy/thefuzz.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/mixins/__init__.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/mixins/dirtyfields.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/mixins/hasParams.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/mixins/hookable.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/mixins/jsonResponse.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/__init__.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/choices.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/manager.py
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/model.py
+-rw-r--r--   0        0        0    53639 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/queryset.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/serializer.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/viewset.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/exceptions/__init__.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/exceptions/get.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/fields/__init__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/fields/boolean.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/fields/char.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/fields/date.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/fields/number.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/fields/objects.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/models/fields/relationships.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/options/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/options/request.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/README.md
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/__init__.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/build.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/db.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/imports.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/lint.py
+-rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/summarize.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/app/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/app/actions.py
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/app/app.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/app/entry.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/conf/sample-settings.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/utils/README.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/utils/__init__.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/utils/action.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/utils/exceptions.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/utils/settings.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/scripts/utils/types.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/signals/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/signals/abstract.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/templates/memory.html
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/templates/angular/base.html
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/templates/jinja/model.py.jinja
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/templatetags/__init__.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/src/djangofoundry/templatetags/syntax_highlight.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/test_matching.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/controllers/__init__.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/controllers/test_mixins.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/decorators/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/decorators/test_timeout.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/helpers/__init__.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/helpers/test_hooks.py
+-rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/helpers/test_queue.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/models/__init__.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/models/test_choices.py
+-rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/tests/foundry/models/test_queryset.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/LICENSE.md
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/README.md
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.8/PKG-INFO
```

### Comparing `djangofoundry-0.0.7/.prospector.yaml` & `djangofoundry-0.0.8/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/Dockerfile` & `djangofoundry-0.0.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/package.json` & `djangofoundry-0.0.8/package.json`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/.devcontainer/devcontainer.json` & `djangofoundry-0.0.8/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/.devcontainer/docker-compose.yml` & `djangofoundry-0.0.8/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/urls.py` & `djangofoundry-0.0.8/src/djangofoundry/urls.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/controllers/__init__.py` & `djangofoundry-0.0.8/src/djangofoundry/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/controllers/angular.py` & `djangofoundry-0.0.8/src/djangofoundry/controllers/angular.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/controllers/detail.py` & `djangofoundry-0.0.8/src/djangofoundry/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/controllers/generic.py` & `djangofoundry-0.0.8/src/djangofoundry/controllers/generic.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/controllers/list.py` & `djangofoundry-0.0.8/src/djangofoundry/controllers/list.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/controllers/memory.py` & `djangofoundry-0.0.8/src/djangofoundry/controllers/memory.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/controllers/responses.py` & `djangofoundry-0.0.8/src/djangofoundry/controllers/responses.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/decorators/queryset_filter.py` & `djangofoundry-0.0.8/src/djangofoundry/decorators/queryset_filter.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/decorators/retry.py` & `djangofoundry-0.0.8/src/djangofoundry/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/decorators/timeout.py` & `djangofoundry-0.0.8/src/djangofoundry/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/exceptions/app.py` & `djangofoundry-0.0.8/src/djangofoundry/exceptions/app.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/logging.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/progress.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/progress.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/__init__.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/exceptions.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/hook.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/hooks.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/hooks.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/waypoint.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/waypoint.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/meta/constants.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/meta/constants.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/hooks/meta/types.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/hooks/meta/types.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/queue/queue.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/queue/queue.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/queue/signals.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/queue/signals.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/render/template.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/render/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/template.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/css.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/css.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/javascript.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/javascript.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/template.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/python/model.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/python/model.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/render/jinja/code/python/template.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/render/jinja/code/python/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/helpers/render/meta/model.py` & `djangofoundry-0.0.8/src/djangofoundry/helpers/render/meta/model.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/matching/engine.py` & `djangofoundry-0.0.8/src/djangofoundry/matching/engine.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/matching/fuzzy/thefuzz.py` & `djangofoundry-0.0.8/src/djangofoundry/matching/fuzzy/thefuzz.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/mixins/dirtyfields.py` & `djangofoundry-0.0.8/src/djangofoundry/mixins/dirtyfields.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/mixins/hasParams.py` & `djangofoundry-0.0.8/src/djangofoundry/mixins/hasParams.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/mixins/hookable.py` & `djangofoundry-0.0.8/src/djangofoundry/mixins/hookable.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/mixins/jsonResponse.py` & `djangofoundry-0.0.8/src/djangofoundry/mixins/jsonResponse.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/__init__.py` & `djangofoundry-0.0.8/src/djangofoundry/models/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/choices.py` & `djangofoundry-0.0.8/src/djangofoundry/models/choices.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/manager.py` & `djangofoundry-0.0.8/src/djangofoundry/models/manager.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/model.py` & `djangofoundry-0.0.8/src/djangofoundry/models/model.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/queryset.py` & `djangofoundry-0.0.8/src/djangofoundry/models/queryset.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/serializer.py` & `djangofoundry-0.0.8/src/djangofoundry/models/serializer.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/viewset.py` & `djangofoundry-0.0.8/src/djangofoundry/models/viewset.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/exceptions/get.py` & `djangofoundry-0.0.8/src/djangofoundry/models/exceptions/get.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/fields/__init__.py` & `djangofoundry-0.0.8/src/djangofoundry/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/fields/char.py` & `djangofoundry-0.0.8/src/djangofoundry/models/fields/char.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/fields/date.py` & `djangofoundry-0.0.8/src/djangofoundry/models/fields/date.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/fields/number.py` & `djangofoundry-0.0.8/src/djangofoundry/models/fields/number.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/fields/objects.py` & `djangofoundry-0.0.8/src/djangofoundry/models/fields/objects.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/models/fields/relationships.py` & `djangofoundry-0.0.8/src/djangofoundry/models/fields/relationships.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/__init__.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/app.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/app/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -36,46 +36,19 @@
 import psutil
 from jinja2 import Environment, FileSystemLoader
 
 # Our imports
 from djangofoundry.scripts.utils.exceptions import DbStartError, UnsupportedCommandError
 from djangofoundry.scripts.utils.settings import Settings
 from djangofoundry.scripts.db import Db
+from djangofoundry.scripts.app.actions import Actions
 
 logging.basicConfig(level=logging.DEBUG, stream=sys.stdout)
 logger = logging.getLogger(__name__)
 
-class Actions(Enum):
-	"""
-	Defines the commands that can be used to interact with django.
-
-	Attributes:
-		start:
-			start the django server
-		test:
-			runs our unit/integration tests
-	"""
-	START = "runserver"
-	TEST = "test"
-	STOP = "stop"
-	RESTART = "restart"
-	STATUS = "status"
-	SETUP = 'setup'
-	PAGE = 'page'
-	MODEL = 'model'
-
-	def __str__(self):
-		"""
-		Turns an option into a string representation
-		"""
-		return self.value
-
-	def __repr__(self):
-		return self.value
-
 class App:
 	"""
 	Our main application class. This script allows us to start, stop, and restart our django server.
 	"""
 	_command : Actions
 	_output_buffer : str = ''
 	project_name : str
@@ -97,62 +70,328 @@
 		"""
 		Get the currently executing command. This is typically set by self.perform()
 		"""
 		if self._command is None:
 			raise ValueError('Command has not been set yet')
 		return self._command
 
+	def get_argument(self, argument_name : str, args : tuple, kwargs : dict ) -> Any:
+		"""
+		Retrieves an argument from args/kwargs.
+
+		This is useful for methods like self.perform() where we want to pass arguments to an arbitrary method, which may be different per command.
+
+		Args:
+			argument_name (str):
+				The name of the argument to retrieve
+			args (tuple):
+				The list of arguments passed to the method
+			kwargs (dict):
+				The dictionary of keyword arguments passed to the method
+
+		Returns:
+			The argument value, if it exists. Otherwise, None.
+
+		Examples:
+			>>> class Foo(App):
+			>>> 	def change_page(self, *args, **kwargs):
+			>>> 		argument = self.get_argument('page_name', args, kwargs)
+			>>> 		print('page_name = ' + argument)
+			>>> foo = Foo()
+			>>> foo.change_page('home')
+			page_name = home
+		"""
+		if len(args) == 1:
+			return args[0]
+		else:
+			return kwargs.get(argument_name, None)
+		
+	def pip_install(self, package_name : str) -> bool:
+		"""
+		Install a python package using pip, and add it (with version) to requirements.txt. 
+
+		Args:
+			pip_package (str): The name of the package(s) to install, separated by a space
+
+		Returns:
+			bool: True if the package was installed successfully, False otherwise.
+
+		Examples:
+			>>> app = App()
+			>>> app.pip_install('requests')
+			True
+
+			>>> app.pip_install('requests==2.26.0')
+			True
+		"""
+		# If the package_name contains multiple packages, split them and install them individually
+		if ' ' in package_name:
+			for single_package_name in package_name.split(' '):
+				if not self.pip_install(single_package_name):
+					return False
+			return True
+		
+
+		# Check if the package is already in requirements.txt
+		# TODO: this ignores version numbers (therefore not handling updates)
+		with open('requirements.txt', 'r') as f:
+			if package_name in f.read():
+				logger.info(f'{package_name} already in requirements.txt. Skipping pip install.')
+				return True
+
+		# Install the package, capture output so that we can determine the version number of the package
+		logger.info(f'Installing {package_name}...')
+		install_output = subprocess.check_output([sys.executable, '-m', 'pip', 'install', package_name], stderr=subprocess.STDOUT).decode('utf-8')
+
+		# Grab the version number from the output
+		output = re.search(r'Successfully installed (.*)', install_output)
+
+		if not output:
+			logger.warning(f'Could not find a version number after installing {package_name}. Output: {install_output}')
+			return False
+		
+		version = output.group(1).split('-')[-1]
+
+		if version is None:
+			logger.warning(f'Could not determine version number for {package_name}')
+			return False
+		
+		# Ensure version is a valid version number
+		if not re.match(r'^\d+\.\d+\.\d+$', version):
+			logger.warning(f'Version number for {package_name} is not valid: {version}')
+			return False
+
+		# Add package (and version #) to requirements.txt. 
+		logger.info(f'Adding {package_name} to requirements.txt...')
+		with open('requirements.txt', 'a') as f:
+			f.write(f'{package_name}>={version}\n')
+
+		return True
+
 	def django_setup(self) -> str:
 		"""
 		Setup the Django project and app with given names.
 
 		Note: This is a work in progress.
 
 		Returns:
 			A string indicating the status of the setup.
 		"""
-		os.makedirs(self.backend_dir, exist_ok=True)
-		os.chdir(self.backend_dir) # Switch to the backend directory before running Django commands
-		self.run_subprocess(["pip", "install", "django"])
-		self.run_subprocess(["django-admin", "startproject", self.project_name, '.'])
-		self.run_subprocess(["python", "manage.py", "startapp", self.project_name])
-		os.chdir(self.directory) # Switch back to the original directory
+		try:
+			os.makedirs(self.backend_dir, exist_ok=True)
+			# Switch to the backend directory before running Django commands
+			os.chdir(self.backend_dir) 
+			self.run_subprocess(["pip", "install", "django"])
+			self.run_subprocess(["django-admin", "startproject", self.project_name, '.'])
+			self.run_subprocess(["python", "manage.py", "startapp", self.project_name])
+		finally:
+			# Switch back to the original directory
+			os.chdir(self.directory) 
+
 		return f"Django setup completed for {self.project_name}"
+	
+	def setup_frontend(self) -> str:
+		"""
+		Setup the frontend (including package.json) for an arbitrary frontend framework.
+	
+		Returns:
+			A string indicating the status of the setup.
+		"""
+		try:
+			os.makedirs(self.frontend_dir, exist_ok=True)
+			# Switch to the frontend directory before installing npm packages
+			os.chdir(self.frontend_dir) 
+			self.run_subprocess(["npm", "init", "-y"])
+
+			with open('package.json', encoding="utf-8") as f:
+				data = json.load(f)
+
+			# Modify the existing package.json file to include our params
+			data['name'] = self.project_name
+			data['version'] = '1.0.0'
+			data['description'] = f'{self.project_name} - an Angular-Django project'
+			data['main'] = 'index.js'
+			data['scripts'] = { 'test': 'echo "Error: no test specified" && exit 1' }
+			data['author'] = getpass.getuser()
+			data['license'] = 'BSD-3-Clause'
+
+			with open('package.json', 'w', encoding="utf-8") as f:
+				json.dump(data, f, indent=2)
+
+			# TODO 3 sparate npm commands can likely be consolidated into 2 or 1.
+			self.run_subprocess(["npm", "install"])
+		finally:
+			os.chdir(self.directory) # Switch back to the original directory
+
+		return f"Frontend setup completed for {self.project_name}"
 
 	def angular_setup(self) -> str:
 		"""
 		Setup the Angular project and app with given names.
 
 		Returns:
 			A string indicating the status of the setup.
 		"""
-		os.makedirs(self.frontend_dir, exist_ok=True)
-		os.chdir(self.frontend_dir) # Switch to the frontend directory before running Angular commands
-		self.run_subprocess(["npm", "init", "-y"])
-
-		with open('package.json', encoding="utf-8") as f:
-			data = json.load(f)
-
-		data['name'] = self.project_name
-		data['version'] = '1.0.0'
-		data['description'] = f'{self.project_name} - an Angular-Django project'
-		data['main'] = 'index.js'
-		data['scripts'] = { 'test': 'echo "Error: no test specified" && exit 1' }
-		data['author'] = getpass.getuser()
-		data['license'] = 'BSD-3-Clause'
-
-		with open('package.json', 'w', encoding="utf-8") as f:
-			json.dump(data, f, indent=2)
-
-		# TODO 3 sparate npm commands can likely be consolidated into 2 or 1.
-		self.run_subprocess(["npm", "install"])
-		self.run_subprocess(["npm", "install", "@angular/cli"])
-		self.run_subprocess(["ng", "new", self.project_name, "--skip-git", "--skip-install"])
-		os.chdir(self.directory) # Switch back to the original directory
+		self.setup_frontend()
+
+		try:
+			os.chdir(self.frontend_dir) 
+
+			# TODO 3 sparate npm commands can likely be consolidated into 2 or 1.
+			self.run_subprocess(["npm", "install"])
+			self.run_subprocess(["npm", "install", "@angular/cli"])
+			self.run_subprocess(["ng", "new", self.project_name, "--skip-git", "--skip-install"])
+		finally:
+			# Switch back to the original directory
+			os.chdir(self.directory) 
+
 		return f"Angular setup completed for {self.project_name}"
+	
+	def append_django_apps(self, app_name: str) -> bool:
+		"""
+		Add the app to the INSTALLED_APPS list in the settings/base.py file
+		"""
+		settings_file = f'{self.backend_dir}/{self.project_name}/settings/base.py'
+
+		# Load the entire settings/base.py file into memory
+		# TODO try catch
+		with open(settings_file, 'r') as f:
+			contents = f.read()
+
+			# Get the installed apps list
+			codeblock = re.search(r'INSTALLED_APPS = \[(.*)\]', contents, re.DOTALL)
+			if not codeblock:
+				# TODO better exception
+				raise Exception(f'Could not find INSTALLED_APPS in {settings_file}')
+			
+			installed_apps = codeblock.group(1)
+			if not installed_apps:
+				# TODO better exception
+				raise Exception(f'No apps found in INSTALLED_APPS. Settings file: {settings_file}')
+			
+			installed_apps = installed_apps.strip()
+
+			# Check if the app is already in INSTALLED_APPS
+			if re.search(rf"'{app_name}'", installed_apps):
+				logger.info(f'{app_name} is already in INSTALLED_APPS')
+				return True
+			
+			# Modify contents with regex to include the app at the end of the list
+			contents = re.sub(r'INSTALLED_APPS = \[(.*)\]', rf'INSTALLED_APPS = [\1, \'{app_name}\']', contents, re.DOTALL)
+		
+		# Write the new contents
+		with open(settings_file, 'w') as f:
+			f.write(contents)
+
+		return True
+	
+	def append_django_middleware(self, middleware_name: str) -> bool:
+		"""
+		Add the middleware to the MIDDLEWARE list in the settings/base.py file
+		"""
+		settings_file = f'{self.backend_dir}/{self.project_name}/settings/base.py'
+
+		# Load the entire settings/base.py file into memory
+		# TODO try catch
+		with open(settings_file, 'r') as f:
+			contents = f.read()
+
+			# Get the installed apps list
+			codeblock = re.search(r'MIDDLEWARE = \[(.*)\]', contents, re.DOTALL)
+			if not codeblock:
+				# TODO better exception
+				raise Exception(f'Could not find MIDDLEWARE in {settings_file}')
+			
+			middleware = codeblock.group(1)
+			if not middleware:
+				# TODO better exception
+				raise Exception(f'No middleware found in MIDDLEWARE. Settings file: {settings_file}')
+			
+			middleware = middleware.strip()
+
+			# Check if the middleware is already in MIDDLEWARE
+			if re.search(rf"'{middleware_name}'", middleware):
+				logger.info(f'{middleware_name} is already in MIDDLEWARE')
+				return True
+			
+			# Modify contents with regex to include the middleware at the end of the list
+			contents = re.sub(r'MIDDLEWARE = \[(.*)\]', rf'MIDDLEWARE = [\1, \'{middleware_name}\']', contents, re.DOTALL)
+		
+		# Write the new contents
+		with open(settings_file, 'w') as f:
+			f.write(contents)
+
+		return True
+	
+	def nuxt_setup(self) -> str:
+		"""
+		Setup the Nuxt project and app with given names.
+
+		Returns:
+			A string indicating the status of the setup.
+		"""
+		self.setup_frontend()
+
+		# Handle dependencies for nuxt
+		self.run_subprocess(["npm", "install", "@nuxtjs/auth"])
+		self.pip_install('django-rest-framework dj-rest-auth django-allauth django-cors-headers djangorestframework-simplejwt')
+
+		# Setup the Nuxt project
+		self.run_subprocess(["npx", "create-nuxt-app", self.frontend_dir])
+
+		# Append necessary django apps to the settings file
+		for app_name in ['corsheaders', 'rest_framework']:
+			self.append_django_apps(app_name)
+
+		# Append middleware to the settings file
+		for middleware_name in ['corsheaders.middleware.CorsMiddleware']:
+			self.append_django_middleware(middleware_name)
+
+		"""
+		Remaining tasks to do:
+		* Add the following lines to enable JWT Authentication:
+		REST_FRAMEWORK = {
+            'DEFAULT_AUTHENTICATION_CLASSES': (
+                'rest_framework_simplejwt.authentication.JWTAuthentication',
+            ),
+        }
+	
+		* Configure Django URLs
+			urlpatterns = [
+				path('admin/', admin.site.urls),
+				path('api/v1/', include('dj_rest_auth.urls')),
+			]
+
+		* Add the following lines to nuxt.config.js
+		    modules: [
+				'@nuxtjs/auth',
+			],
+			auth: {
+				strategies: {
+					local: {
+						endpoints: {
+							login: { url: '/api/v1/login/', method: 'post', propertyName: 'token' },
+							logout: { url: '/api/v1/logout/', method: 'post' },
+							user: { url: '/api/v1/user/', method: 'get', propertyName: 'user' }
+						},
+						tokenRequired: true,
+						tokenType: 'Bearer',
+					}
+				}
+			}
+
+		* For new nuxtjs components:
+		    this.$auth.loginWith('local', {
+				data: {
+					username: this.username,
+					password: this.password
+				}
+			})
+		"""
+		return f"Nuxt setup completed for {self.project_name}"
 
 	def install_dependencies(self) -> None:
 		"""
 		Check if npm is installed and call install_npm() if it's not.
 
 		Returns:
 			None
@@ -169,19 +408,20 @@
 			A string indicating the status of the installation.
 		"""
 		os_name = platform.system()
 
 		# If ubuntu, install with apt
 		if os_name == 'Linux' and shutil.which('apt'):
 			try:
-				self.run_subprocess(['apt', 'install', 'npm'])
+				self.run_subprocess(['apt', 'install', 'npm', 'npx'])
 				return "npm installed successfully on Ubuntu"
 			except subprocess.CalledProcessError as process_e:
 				raise EnvironmentError(f"Error installing npm on Ubuntu: {process_e}") from process_e
 		
+		# Otherwise, check for other variants of linux
 		if os_name in ['Linux', 'Darwin']:
 			try:
 				self.run_subprocess(['curl', 'https://www.npmjs.com/install.sh', '|', 'sh'])
 				return "npm installed successfully on Linux or macOS"
 			except subprocess.CalledProcessError as process_e:
 				raise EnvironmentError(f"Error installing npm on Linux or macOS: {process_e}") from process_e
 		
@@ -264,15 +504,15 @@
 			None
 		"""
 		os.makedirs(self.directory, exist_ok=True)
 
 		self.check_environment()
 		self.install_dependencies()
 		self.django_setup()
-		self.angular_setup()
+		self.nuxt_setup()
 		self.confirm_setup()
 
 	def run(self, command : Actions, callback : Optional[Callable] = None, *args, **kwargs) -> str:
 		"""
 		Run a django command in a similar way to manage.py
 
 		Args:
@@ -394,15 +634,15 @@
 	@property
 	def status(self) -> bool:
 		"""
 		Determine the status of our application.
 		"""
 		server_process_names = ["runserver", "gunicorn", "daphne"]
 		for process in psutil.process_iter(['name']):
-			if process.info['name'] in server_process_names:
+			if process.name() in server_process_names:
 				return True
 
 		return False
 
 	def sync_browser(self):
 		"""
 		Start a process to sync the browser with the application state.
@@ -452,15 +692,15 @@
 			print(value)
 
 		match value.lower():
 			case 'quit the server with ctrl-break.':
 				logger.debug('Django started successfully')
 				self.on_django_started()
 
-	def perform(self, command: Actions, page_name: str = None, model_name: str = None) -> Any:
+	def perform(self, command: Actions, *args, **kwargs) -> Any:
 		"""
 		Perform an action given a (string) command
 
 		Args:
 			command (Actions): The action to perform.
 			page_name (str): The name of the page to create.
 			model_name (str): The name of the model to create.
@@ -484,22 +724,30 @@
 				return self.setup()
 			case Actions.STOP:
 				# Stop our app
 				return self.stop()
 			case Actions.STATUS:
 				# Determine the status of our app
 				return self.status
+			case Actions.INSTALL:
+				# Install a python package using pip, and add it (with version) to requirements.txt.
+				package_name = self.get_argument('package_name', args, kwargs)
+				return self.pip_install(package_name)
 			case Actions.PAGE:
+				# Ensure we have either one *arg, or a page_name **kwarg
+				page_name = self.get_argument('page_name', args, kwargs)
+					
 				if page_name:
 					return self.create_new_page(page_name)
 				else:
 					raise ValueError("Page name is required for 'page' action.")
 			case Actions.MODEL:
+				model_name : str = self.get_argument('model_name', args, kwargs)
 				if model_name:
-					return self.create_django_model(model_name, model_name.capitalize())
+					return self.create_new_model(model_name)
 				else:
 					raise ValueError("Model name is required for 'model' action.")
 			case _:
 				raise UnsupportedCommandError(f"Unknown command {command}.")
 
 	def _start_db(self) -> None:
 		"""
@@ -627,49 +875,50 @@
 		for template_name in env.list_templates():
 			template = env.get_template(template_name)
 			rendered_template = template.render(model_name=model_name)
 			output_file = os.path.join(model_dir, template_name.replace(".jinja", ".py"))
 			with open(output_file, "w") as file:
 				file.write(rendered_template)
 
-
 def main():
-	"""
-	This code is only run when this script is called directly (i.e. python bin/app.py)
-	"""
-	parser = argparse.ArgumentParser(description='Setup and manage the Django application.')
-	parser.add_argument('action', choices=[e.value for e in Actions], help='The action to perform.')
-	parser.add_argument('-p', '--project-name', default='myproject', help='The name of the project.')
-	parser.add_argument('-a', '--author-name', help='The name of the author.')
-	parser.add_argument('-d', '--directory', default='.', help='The directory for the project.')
-	parser.add_argument('-f', '--frontend-dir', default='frontend', help='The directory for the frontend (relative to -d).')
-	parser.add_argument('-b', '--backend-dir', default='backend', help='The directory for the backend (relative to -d).')
-	parser.add_argument('-s', '--settings', default='conf/settings.yaml', help='The settings file to use.')
-	parser.add_argument('--page-name', help='The name of the page to create.')
-	parser.add_argument('--model-name', help='The name of the model to create.')
-	args = parser.parse_args()
-
-	# Load settings
-	settings = Settings(args.settings)
-
-	app = App(args.project_name, args.author_name, settings, args.directory, args.frontend_dir, args.backend_dir)
-	command = Actions(args.action)
-
-	result = app.perform(command, args.page_name, args.model_name)
-	if result is not None:
-		print(f'App returned ({result})')
-
-if __name__ == '__main__':
 	try:
-		main()
+		parser = argparse.ArgumentParser(description='Setup and manage the Django application.')
+		parser.add_argument('action', choices=[e.value for e in Actions], help='The action to perform.')
+		parser.add_argument('-p', '--project-name', default='myproject', help='The name of the project.')
+		parser.add_argument('-a', '--author-name', help='The name of the author.')
+		parser.add_argument('-d', '--directory', default='.', help='The directory for the project.')
+		parser.add_argument('-f', '--frontend-dir', default='frontend', help='The directory for the frontend (relative to -d).')
+		parser.add_argument('-b', '--backend-dir', default='backend', help='The directory for the backend (relative to -d).')
+		parser.add_argument('-s', '--settings', default='conf/settings.yaml', help='The settings file to use.')
+		parser.add_argument('--page-name', help='The name of the page to create.')
+		parser.add_argument('--model-name', help='The name of the model to create.')
+		parser.add_argument('--package-name', help='The name of the package to create.')
+		args = parser.parse_args()
+
+		# Load settings
+		settings = Settings(args.settings)
+
+		app = App(args.project_name, args.author_name, settings, args.directory, args.frontend_dir, args.backend_dir)
+		command = Actions(args.action)
+
+		result = app.perform(command, page_name=args.page_name, model_name=args.model_name, package_name=args.package_name)
+		if result is not None:
+			print(f'App returned ({result})')
+
 	except KeyboardInterrupt:
 		logger.info('Shutting down server...')
 		sys.exit(0)
 	except DbStartError:
 		logger.error('Could not start DB. Cannot continue')
 		sys.exit(0)
 	except EnvironmentError as env_error:
 		logger.error(f'Cannot run script in the current environment. {env_error}')
 		sys.exit(0)
 	except Exception as e:
 		print(f"Error: {e}")
 		sys.exit(0)
+
+if __name__ == '__main__':
+	"""
+	This code is only run when this script is called directly (i.e. python bin/app.py)
+	"""
+	main()
```

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/build.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/build.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/db.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/db.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/imports.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/imports.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/lint.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/lint.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/summarize.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/summarize.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/conf/sample-settings.yaml` & `djangofoundry-0.0.8/src/djangofoundry/scripts/conf/sample-settings.yaml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/utils/__init__.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/utils/action.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/utils/action.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/utils/exceptions.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/utils/settings.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/utils/settings.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/scripts/utils/types.py` & `djangofoundry-0.0.8/src/djangofoundry/scripts/utils/types.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/signals/abstract.py` & `djangofoundry-0.0.8/src/djangofoundry/signals/abstract.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/templates/memory.html` & `djangofoundry-0.0.8/src/djangofoundry/templates/memory.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/templates/angular/base.html` & `djangofoundry-0.0.8/src/djangofoundry/templates/angular/base.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/templates/jinja/model.py.jinja` & `djangofoundry-0.0.8/src/djangofoundry/templates/jinja/model.py.jinja`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/src/djangofoundry/templatetags/syntax_highlight.py` & `djangofoundry-0.0.8/src/djangofoundry/templatetags/syntax_highlight.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/tests/foundry/test_matching.py` & `djangofoundry-0.0.8/tests/foundry/test_matching.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/tests/foundry/controllers/test_mixins.py` & `djangofoundry-0.0.8/tests/foundry/controllers/test_mixins.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/tests/foundry/decorators/test_timeout.py` & `djangofoundry-0.0.8/tests/foundry/decorators/test_timeout.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/tests/foundry/helpers/test_hooks.py` & `djangofoundry-0.0.8/tests/foundry/helpers/test_hooks.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/tests/foundry/helpers/test_queue.py` & `djangofoundry-0.0.8/tests/foundry/helpers/test_queue.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/tests/foundry/models/test_choices.py` & `djangofoundry-0.0.8/tests/foundry/models/test_choices.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/tests/foundry/models/test_queryset.py` & `djangofoundry-0.0.8/tests/foundry/models/test_queryset.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/LICENSE.md` & `djangofoundry-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/README.md` & `djangofoundry-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.7/pyproject.toml` & `djangofoundry-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "djangofoundry"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Jess Mann", email="jess.a.mann+df@gmail.com" },
 ]
 description = "A collection of classes built on Django to make it easier to build web applications."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `djangofoundry-0.0.7/PKG-INFO` & `djangofoundry-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangofoundry
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of classes built on Django to make it easier to build web applications.
 Project-URL: Homepage, https://github.com/avranu/Django-Foundry
 Project-URL: Bug Tracker, https://github.com/avranu/Django-Foundry/issues
 Author-email: Jess Mann <jess.a.mann+df@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

