# Comparing `tmp/esmerald-1.2.5.tar.gz` & `tmp/esmerald-1.3.0.tar.gz`

## Comparing `esmerald-1.2.5.tar` & `esmerald-1.3.0.tar`

### file list

```diff
@@ -1,189 +1,185 @@
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/__init__.py
--rw-r--r--   0        0        0    32066 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/concurrency.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/enums.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/exceptions.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/injector.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/logging.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/param_functions.py
--rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/params.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/py.typed
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/staticfiles.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/testclient.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/types.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/typing.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/websockets.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/enums.py
--rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/jwt.py
--rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/openapi.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/session.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/static_files.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/crypto.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/tortoise/__init__.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/tortoise/base_user.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/tortoise/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/databases/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/databases/tortoise/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/apiview.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/parameters.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/path_item.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/request_body.py
--rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/schema.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/types.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/permissions/base.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/template.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/base.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/__init__.py
--rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/base.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/events.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/router.py
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/model.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/utils.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/urls/__init__.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/urls/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/helpers.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/pydantic.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/sync.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/timezone.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/url.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.5/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.5/LICENSE
--rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 esmerald-1.2.5/README.md
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 esmerald-1.2.5/pyproject.toml
--rw-r--r--   0        0        0    20202 2020-02-02 00:00:00.000000 esmerald-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/__init__.py
+-rw-r--r--   0        0        0    32636 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/concurrency.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/enums.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/injector.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/logging.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/param_functions.py
+-rw-r--r--   0        0        0    14464 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/params.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/py.typed
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/testclient.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/types.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/websockets.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    13292 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/session.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/apiview.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/parameters.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/path_item.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/request_body.py
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/schema.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/types.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/utils/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/utils/protocols.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/base.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0    22142 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    22845 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    41247 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/router.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.3.0/LICENSE
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 esmerald-1.3.0/README.md
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 esmerald-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 esmerald-1.3.0/PKG-INFO
```

### Comparing `esmerald-1.2.5/esmerald/__init__.py` & `esmerald-1.3.0/esmerald/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.5"
+__version__ = "1.3.0"
 
 
 from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
```

### Comparing `esmerald-1.2.5/esmerald/applications.py` & `esmerald-1.3.0/esmerald/applications.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,23 @@
     Dict,
     List,
     Optional,
     Sequence,
     Type,
     TypeVar,
     Union,
+    cast,
 )
 
-from openapi_schemas_pydantic.v3_1_0 import License, SecurityRequirement, Server
+from openapi_schemas_pydantic.v3_1_0 import Contact, License, SecurityRequirement, Server, Tag
 from openapi_schemas_pydantic.v3_1_0.open_api import OpenAPI
+from pydantic import AnyUrl
 from starlette.applications import Starlette
 from starlette.middleware import Middleware as StarletteMiddleware  # noqa
-from starlette.types import Lifespan
+from starlette.types import Lifespan, Receive, Scope, Send
 
 from esmerald.conf import settings as esmerald_settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.config import CORSConfig, CSRFConfig, SessionConfig
 from esmerald.config.openapi import OpenAPIConfig
 from esmerald.config.static_files import StaticFilesConfig
 from esmerald.datastructures import State
@@ -41,30 +43,28 @@
 from esmerald.protocols.template import TemplateEngineProtocol
 from esmerald.routing import gateways
 from esmerald.routing.router import HTTPHandler, Include, Router, WebSocketHandler
 from esmerald.types import (
     APIGateHandler,
     ASGIApp,
     Dependencies,
-    ExceptionHandlers,
+    ExceptionHandlerMap,
     LifeSpanHandler,
     Middleware,
     ParentType,
-    Receive,
     ResponseCookies,
     ResponseHeaders,
     ResponseType,
     RouteParent,
     SchedulerType,
-    Scope,
-    Send,
 )
 from esmerald.utils.helpers import is_class_and_subclass
 
 if TYPE_CHECKING:
+    from esmerald.conf import EsmeraldLazySettings
     from esmerald.types import SettingsType, TemplateConfig
 
 AppType = TypeVar("AppType", bound="Esmerald")
 
 
 class Esmerald(Starlette):
     """
@@ -123,24 +123,24 @@
         settings_config: Optional["SettingsType"] = None,
         debug: Optional[bool] = None,
         app_name: Optional[str] = None,
         title: Optional[str] = None,
         version: Optional[str] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
-        contact: Optional[Dict[str, Union[str, Any]]] = None,
-        terms_of_service: Optional[str] = None,
+        contact: Optional[Contact] = None,
+        terms_of_service: Optional[AnyUrl] = None,
         license: Optional[License] = None,
         security: Optional[List[SecurityRequirement]] = None,
         servers: Optional[List[Server]] = None,
         secret_key: Optional[str] = None,
         allowed_hosts: Optional[List[str]] = None,
         allow_origins: Optional[List[str]] = None,
-        permissions: Optional[List["Permission"]] = None,
-        interceptors: Optional[List["Interceptor"]] = None,
+        permissions: Optional[Sequence["Permission"]] = None,
+        interceptors: Optional[Sequence["Interceptor"]] = None,
         dependencies: Optional["Dependencies"] = None,
         csrf_config: Optional["CSRFConfig"] = None,
         openapi_config: Optional["OpenAPIConfig"] = None,
         cors_config: Optional["CORSConfig"] = None,
         static_files_config: Optional["StaticFilesConfig"] = None,
         template_config: Optional["TemplateConfig"] = None,
         session_config: Optional["SessionConfig"] = None,
@@ -148,40 +148,40 @@
         response_cookies: Optional["ResponseCookies"] = None,
         response_headers: Optional["ResponseHeaders"] = None,
         scheduler_class: Optional["SchedulerType"] = None,
         scheduler_tasks: Optional[Dict[str, str]] = None,
         scheduler_configurations: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
         enable_scheduler: Optional[bool] = None,
         timezone: Optional[Union[dtimezone, str]] = None,
-        routes: Optional[List["APIGateHandler"]] = None,
+        routes: Optional[Sequence[Union["APIGateHandler", "Include"]]] = None,
         root_path: Optional[str] = None,
         middleware: Optional[Sequence["Middleware"]] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         on_startup: Optional[List["LifeSpanHandler"]] = None,
         on_shutdown: Optional[List["LifeSpanHandler"]] = None,
         lifespan: Optional[Lifespan[AppType]] = None,
-        tags: Optional[List[str]] = None,
+        tags: Optional[List[Tag]] = None,
         include_in_schema: Optional[bool] = None,
         deprecated: Optional[bool] = None,
         enable_openapi: Optional[bool] = None,
         redirect_slashes: Optional[bool] = None,
         pluggables: Optional[Dict[str, Pluggable]] = None,
-        parent: Optional[Type["Esmerald"]] = None,
+        parent: Optional[Union["ParentType", "Esmerald", "ChildEsmerald"]] = None,
     ) -> None:
         self.settings_config = None
 
         if settings_config:
             if not isinstance(settings_config, EsmeraldAPISettings) and not is_class_and_subclass(
                 settings_config, EsmeraldAPISettings
             ):
                 raise ImproperlyConfigured(
                     "settings_config must be a subclass of EsmeraldSettings"
                 )
             elif isinstance(settings_config, EsmeraldAPISettings):
-                self.settings_config = settings_config
+                self.settings_config = settings_config  # type: ignore
             elif is_class_and_subclass(settings_config, EsmeraldAPISettings):
                 self.settings_config = settings_config()
 
         assert lifespan is None or (
             on_startup is None and on_shutdown is None
         ), "Use either 'lifespan' or 'on_startup'/'on_shutdown', not both."
 
@@ -299,16 +299,16 @@
         self.timezone = timezone or self.get_settings_value(
             self.settings_config, esmerald_settings, "timezone"
         )
         self.root_path = root_path or self.get_settings_value(
             self.settings_config, esmerald_settings, "root_path"
         )
 
-        self.middleware = (
-            middleware
+        self.middleware = (  # type: ignore
+            middleware  # type: ignore
             or self.get_settings_value(self.settings_config, esmerald_settings, "middleware")
             or []
         )
         _exception_handlers = exception_handlers or self.get_settings_value(
             self.settings_config, esmerald_settings, "exception_handlers"
         )
         self.exception_handlers = {} if _exception_handlers is None else dict(_exception_handlers)
@@ -351,15 +351,14 @@
             if pluggables
             else self.get_settings_value(self.settings_config, esmerald_settings, "pluggables")
         )
 
         self.openapi_schema: Optional["OpenAPI"] = None
         self.state = State()
         self.async_exit_config = esmerald_settings.async_exit_config
-        self.parent: Optional[Union["ParentType", "Esmerald", "ChildEsmerald"]] = None
 
         self.router: "Router" = Router(
             on_shutdown=self.on_shutdown,
             on_startup=self.on_startup,
             routes=routes,
             app=self,
             lifespan=self.lifespan,
@@ -385,15 +384,15 @@
                 self.router.routes.append(static_route)
 
         if self.enable_scheduler:
             self.activate_scheduler()
 
         self.activate_openapi()
 
-    def activate_scheduler(self):
+    def activate_scheduler(self) -> None:
         """
         Makes sure the scheduler is accessible.
         """
         try:
             from asyncz.contrib.esmerald.scheduler import EsmeraldScheduler
         except ImportError as e:
             raise ImportError(
@@ -401,98 +400,97 @@
             ) from e
 
         self.scheduler = EsmeraldScheduler(
             app=self,
             scheduler_class=self.scheduler_class,
             tasks=self.scheduler_tasks,
             timezone=self.timezone,
-            configurations=self.scheduler_configurations,
+            configurations=self.scheduler_configurations,  # type: ignore
         )
 
     def get_settings_value(
         self,
-        local_settings: Type["EsmeraldAPISettings"],
-        global_settings: Type["EsmeraldAPISettings"],
+        local_settings: Optional["EsmeraldAPISettings"],
+        global_settings: Union[Type["EsmeraldAPISettings"], Type["EsmeraldLazySettings"]],
         value: str,
     ) -> Any:
         """Obtains the value from a settings module or defaults to the global settings"""
         setting_value = None
 
         if local_settings:
             setting_value = getattr(local_settings, value, None)
         if not setting_value:
             return getattr(global_settings, value, None)
         return setting_value
 
     def activate_openapi(self) -> None:
         if self.openapi_config and self.enable_openapi:
             self.openapi_schema = self.openapi_config.create_openapi_schema_model(self)
-            gateway = gateways.Gateway(handler=self.openapi_config.openapi_apiview)
+            gateway = gateways.Gateway(handler=self.openapi_config.openapi_apiview)  # type: ignore
             self.add_apiview(value=gateway)
 
     def get_template_engine(
         self, template_config: "TemplateConfig"
     ) -> Optional["TemplateEngineProtocol"]:
         """
         Returns the template engine for the application.
         """
         if not template_config:
-            return
+            return None
 
         engine = template_config.engine(template_config.directory)
         return engine
 
     def add_apiview(
         self,
-        value: Union[Type["gateways.Gateway"], Type["gateways.WebSocketGateway"]],
+        value: Union["gateways.Gateway", "gateways.WebSocketGateway"],
     ) -> None:
         """
         Adds an APIView via application instance.
         """
         self.router.add_apiview(value=value)
 
     def add_route(
         self,
         path: str,
         handler: "HTTPHandler",
         router: Optional["Router"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         interceptors: Optional[List["Interceptor"]] = None,
         permissions: Optional[List["Permission"]] = None,
         middleware: Optional[List["Middleware"]] = None,
         name: Optional[str] = None,
         include_in_schema: bool = True,
     ) -> None:
         """
         Adds a route into the router.
         """
         router = router or self.router
-        route = router.add_route(
+        router.add_route(
             path=path,
             handler=handler,
             dependencies=dependencies,
             exception_handlers=exception_handlers,
             interceptors=interceptors,
             permissions=permissions,
             middleware=middleware,
             name=name,
             include_in_schema=include_in_schema,
         )
 
         self.activate_openapi()
-        return route
 
     def add_websocket_route(
         self,
         path: str,
-        handler: "HTTPHandler",
+        handler: "WebSocketHandler",
         router: Optional["Router"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         interceptors: Optional[List["Interceptor"]] = None,
         permissions: Optional[List["Permission"]] = None,
         middleware: Optional[List["Middleware"]] = None,
         name: Optional[str] = None,
     ) -> None:
         router = router or self.router
         return router.add_websocket_route(
@@ -514,46 +512,46 @@
     def add_child_esmerald(
         self,
         path: str,
         child: "ChildEsmerald",
         name: Optional[str] = None,
         middleware: Optional[Sequence["Middleware"]] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         interceptors: Optional[List["Interceptor"]] = None,
         permissions: Optional[List["Permission"]] = None,
         include_in_schema: Optional[bool] = True,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
-    ):
+    ) -> None:
         """
         Adds a child esmerald into the application routers.
         """
         if not isinstance(child, ChildEsmerald):
             raise ImproperlyConfigured("The child must be an instance of a ChildEsmerald.")
 
         self.router.routes.append(
             Include(
                 path=path,
                 name=name,
                 app=child,
                 parent=self.router,
                 dependencies=dependencies,
-                middleware=middleware,
+                middleware=cast("List[Middleware]", middleware),
                 exception_handlers=exception_handlers,
                 interceptors=interceptors,
                 permissions=permissions,
                 include_in_schema=include_in_schema,
                 deprecated=deprecated,
                 security=security,
             )
         )
         self.activate_openapi()
 
-    def add_router(self, router: "Router"):
+    def add_router(self, router: "Router") -> None:
         """
         Adds a router to the application.
         """
         for route in router.routes:
             if isinstance(route, Include):
                 self.router.routes.append(
                     Include(
@@ -561,15 +559,15 @@
                         app=route.app,
                         dependencies=route.dependencies,
                         exception_handlers=route.exception_handlers,
                         name=route.name,
                         middleware=route.middleware,
                         interceptors=route.interceptors,
                         permissions=route.permissions,
-                        routes=route.routes,
+                        routes=cast("Sequence[Union[APIGateHandler, Include]]", route.routes),
                         parent=self.router,
                         security=route.security,
                     )
                 )
                 continue
 
             gateway = (
@@ -619,15 +617,15 @@
         )
         self.exception_handlers.setdefault(
             ValidationErrorException, validation_error_exception_handler
         )
 
     def build_routes_middleware(
         self, route: "RouteParent", middlewares: Optional[List["Middleware"]] = None
-    ):
+    ) -> List["Middleware"]:
         """
         Builds the middleware stack from the top to the bottom of the routes.
 
         The includes are an exception as they are treated as an independent ASGI
         application and therefore handles their own middlewares independently.
         """
         if not middlewares:
@@ -644,52 +642,52 @@
                 middlewares.extend(route.handler.middleware)
 
         return middlewares
 
     def build_routes_exception_handlers(
         self,
         route: "RouteParent",
-        exception_handlers: Optional["ExceptionHandlers"] = None,
-    ):
+        exception_handlers: Optional[Dict[str, Callable[..., Any]]] = None,
+    ) -> Dict[str, Callable[..., Any]]:
         """
         Builds the exception handlers stack from the top to the bottom of the routes.
         """
         if not exception_handlers:
             exception_handlers = {}
 
         if isinstance(route, Include):
-            exception_handlers.update(route.exception_handlers)
+            exception_handlers.update(route.exception_handlers)  # type: ignore
             app = getattr(route, "app", None)
             if app and isinstance(app, (Esmerald, ChildEsmerald)):
                 return exception_handlers
 
             for _route in route.routes:
                 exception_handlers = self.build_routes_exception_handlers(
                     _route, exception_handlers
                 )
 
         if isinstance(route, (gateways.Gateway, gateways.WebSocketGateway)):
-            exception_handlers.update(route.exception_handlers)
+            exception_handlers.update(route.exception_handlers)  # type: ignore
             if route.handler.exception_handlers:
-                exception_handlers.update(route.handler.exception_handlers)
+                exception_handlers.update(route.handler.exception_handlers)  # type: ignore
 
         return exception_handlers
 
     def build_user_middleware_stack(self) -> List["StarletteMiddleware"]:
         """
         Configures all the passed settings
         and wraps inside an exception handler.
 
         CORS, CSRF, TrustedHost and JWT are provided to the __init__ they will wapr the
         handler as well.
 
         It evaluates the middleware passed into the routes from bottom up
         """
         user_middleware = []
-        handlers_middleware = []
+        handlers_middleware: List["Middleware"] = []
 
         if self.allowed_hosts:
             user_middleware.append(
                 StarletteMiddleware(TrustedHostMiddleware, allowed_hosts=self.allowed_hosts)
             )
         if self.cors_config:
             user_middleware.append(StarletteMiddleware(CORSMiddleware, **self.cors_config.dict()))
@@ -701,17 +699,17 @@
                 StarletteMiddleware(SessionMiddleware, **self.session_config.dict())
             )
 
         handlers_middleware += self.router.middleware
         for route in self.routes or []:
             handlers_middleware.extend(self.build_routes_middleware(route))
 
-        self.middleware += handlers_middleware
+        self.middleware += handlers_middleware  # type: ignore
 
-        for middleware in self.middleware or []:
+        for middleware in self.middleware or []:  # type: ignore
             if isinstance(middleware, StarletteMiddleware):
                 user_middleware.append(middleware)
             else:
                 user_middleware.append(StarletteMiddleware(middleware))
         return user_middleware
 
     def build_middleware_stack(self) -> "ASGIApp":
@@ -762,21 +760,21 @@
         )
 
         app: "ASGIApp" = self.router
         for cls, options in reversed(middleware):
             app = cls(app=app, **options)
         return app
 
-    def build_pluggable_stack(self) -> None:
+    def build_pluggable_stack(self) -> Optional["Esmerald"]:
         """
         Validates the pluggable types passed and builds the stack
         and triggers the plug
         """
         if not self.pluggables:
-            return
+            return None
 
         pluggables = {}
 
         for name, extension in self.pluggables.items():
             if not isinstance(name, str):
                 raise ImproperlyConfigured("Pluggable names should be in string format.")
             elif isinstance(extension, Pluggable):
@@ -789,34 +787,35 @@
                 )
             else:
                 pluggables[name] = Pluggable(extension)
 
         app: "ASGIApp" = self
         for name, pluggable in pluggables.items():
             for cls, options in [pluggable]:
-                app: "Extension" = cls(app=app, **options)
-                app.extend(**options)
+                ext: "Extension" = cls(app=app, **options)
+                ext.extend(**options)
                 self.pluggables[name] = cls
-        return app
+        return cast("Esmerald", app)
 
     def add_pluggable(self, name: str, extension: Any) -> None:
         """
         Adds an extension to the application pluggables
         """
         self.pluggables[name] = extension
 
     @property
     def settings(self) -> Type["EsmeraldAPISettings"]:
         """
         Returns the Esmerald settings object for easy access.
         """
-        return self.settings_config if self.settings_config else esmerald_settings
+        general_settings = self.settings_config if self.settings_config else esmerald_settings
+        return cast("Type[EsmeraldAPISettings]", general_settings)
 
     @property
-    def default_settings(self) -> Type["EsmeraldAPISettings"]:
+    def default_settings(self) -> Union[Type["EsmeraldAPISettings"], Type["EsmeraldLazySettings"]]:
         """
         Returns the default global settings.
         """
         return esmerald_settings
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         scope["app"] = self
```

### Comparing `esmerald-1.2.5/esmerald/backgound.py` & `esmerald-1.3.0/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/enums.py` & `esmerald-1.3.0/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/exception_handlers.py` & `esmerald-1.3.0/esmerald/exception_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """
     Default exception handler for StarletteHTTPException and Esmerald HTTPException.
     """
     extra = getattr(exc, "extra", None)
     headers = getattr(exc, "headers", None)
 
     if exc.status_code in {204, 304}:
-        return JSONResponse(status_code=exc.status_code, headers=headers)
+        return JSONResponse(None, status_code=exc.status_code, headers=headers)
 
     if headers and not extra:
         return JSONResponse({"detail": exc.detail}, status_code=exc.status_code, headers=headers)
     elif headers and extra:
         return JSONResponse(
             {"detail": exc.detail, "extra": extra},
             status_code=exc.status_code,
@@ -68,15 +68,15 @@
         else status.HTTP_500_INTERNAL_SERVER_ERROR
     )
     if not status_code:
         status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
 
     content = {"detail": exc.detail}
     if exc.extra:
-        content.update({"extra": exc.extra})
+        content.update({"extra": exc.extra})  # type: ignore[dict-item]
     headers = exc.headers if isinstance(exc, (HTTPException, StarletteHTTPException)) else None
 
     return Response(
         media_type=MediaType.JSON,
         content=content,
         status_code=status_code,
         headers=headers,
```

### Comparing `esmerald-1.2.5/esmerald/exceptions.py` & `esmerald-1.3.0/esmerald/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Type, Union
 
 from pydantic import BaseModel, create_model
 from starlette import status
 from starlette.exceptions import HTTPException as StarletteHTTPException
-from starlette.exceptions import WebSocketException
+from starlette.exceptions import WebSocketException as StarletteWebSocketException
 
 RequestErrorModel: Type[BaseModel] = create_model("Request")
 WebSocketErrorModel: Type[BaseModel] = create_model("WebSocket")
 
 
 class EsmeraldAPIException(Exception):
     def __init__(self, *args: Any, detail: str = ""):
@@ -34,16 +34,16 @@
 
     def __init__(
         self,
         *args: Any,
         detail: Optional[str] = None,
         status_code: Optional[int] = None,
         headers: Optional[Dict[str, Any]] = None,
-        **extra,
-    ):
+        **extra: Any,
+    ) -> None:
         detail = detail or getattr(self, "detail", None)
         status_code = status_code or getattr(self, "status_code", None)
         if not detail:
             detail = args[0] if args else HTTPStatus(status_code or self.status_code).phrase
             args = args[1:]
         super().__init__(status_code=status_code, detail=detail, headers=headers)
         self.detail = detail
@@ -117,15 +117,15 @@
     ...
 
 
 class OpenAPIError(ValueError):
     ...
 
 
-class WebSocketException(WebSocketException):
+class WebSocketException(StarletteWebSocketException):
     ...
 
 
 class AuthenticationError(HTTPException):
     status_code = status.HTTP_401_UNAUTHORIZED
```

### Comparing `esmerald-1.2.5/esmerald/injector.py` & `esmerald-1.3.0/esmerald/injector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import TYPE_CHECKING, Any, Dict, Optional, Type, cast
+from typing import TYPE_CHECKING, Any, Dict, Optional, Type
 
 from esmerald.parsers import ArbitraryHashableBaseModel
 from esmerald.transformers.datastructures import Signature
 from esmerald.typing import Void
 from esmerald.utils.helpers import is_async_callable
 
 if TYPE_CHECKING:
-    from pydantic.typing import AnyCallable, DictAny
+    from pydantic.typing import AnyCallable
 
 
 class Inject(ArbitraryHashableBaseModel):
-    def __init__(self, dependency: "AnyCallable", use_cache: bool = False, **kwargs: "DictAny"):
+    def __init__(self, dependency: "AnyCallable", use_cache: bool = False, **kwargs: Any):
         super().__init__(**kwargs)
-        self.dependency = cast("AnyCallable", dependency)
+        self.dependency = dependency
         self.signature_model: Optional["Type[Signature]"] = None
         self.use_cache = use_cache
         self.value: Any = Void
 
     async def __call__(self, **kwargs: Dict[str, Any]) -> Any:
         if self.use_cache and self.value is not Void:
             return self.value
```

### Comparing `esmerald-1.2.5/esmerald/params.py` & `esmerald-1.3.0/esmerald/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,21 +35,21 @@
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         regex: Optional[str] = None,
         example: Any = Undefined,
         examples: Optional[Dict[str, Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
-    ) -> Any:
+    ) -> None:
         self.deprecated = deprecated
         self.example = example
         self.examples = examples
         self.include_in_schema = include_in_schema
 
-        extra: Dict[Union[str, int], Any] = {}
+        extra: Dict[str, Any] = {}
         extra.update(header=header)
         extra.update(cookie=cookie)
         extra.update(query=query)
         extra.update(path=path)
         extra.update(required=required)
         extra.update(content_encoding=content_encoding)
         extra.update(value_type=value_type)
@@ -103,15 +103,15 @@
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         regex: Optional[str] = None,
         example: Any = Undefined,
         examples: Optional[Dict[str, Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
-    ) -> Any:
+    ) -> None:
         super().__init__(
             default=default,
             header=value,
             alias=alias,
             title=title,
             description=description,
             const=const,
@@ -160,15 +160,15 @@
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         regex: Optional[str] = None,
         example: Any = Undefined,
         examples: Optional[Dict[str, Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
-    ) -> Any:
+    ) -> None:
         super().__init__(
             default=default,
             cookie=value,
             alias=alias,
             title=title,
             description=description,
             const=const,
@@ -217,15 +217,15 @@
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         regex: Optional[str] = None,
         example: Any = Undefined,
         examples: Optional[Dict[str, Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
-    ) -> Any:
+    ) -> None:
         super().__init__(
             default=default,
             query=value,
             alias=alias,
             title=title,
             description=description,
             const=const,
@@ -269,15 +269,15 @@
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         regex: Optional[str] = None,
         example: Any = Undefined,
         examples: Optional[Dict[str, Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
-    ) -> Any:
+    ) -> None:
         super().__init__(
             default=default,
             title=title,
             description=description,
             const=const,
             gt=gt,
             ge=ge,
@@ -303,34 +303,36 @@
         default: Any = Undefined,
         media_type: Union[str, EncodingType] = EncodingType.JSON,
         content_encoding: Optional[str] = None,
         title: Optional[str] = None,
         alias: Optional[str] = None,
         description: Optional[str] = None,
         const: Optional[bool] = None,
+        embed: Optional[bool] = None,
         gt: Optional[float] = None,
         ge: Optional[float] = None,
         lt: Optional[float] = None,
         le: Optional[float] = None,
         multiple_of: Optional[float] = None,
         min_items: Optional[int] = None,
         max_items: Optional[int] = None,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         regex: Optional[str] = None,
         example: Any = Undefined,
         examples: Optional[Dict[str, Any]] = None,
-    ) -> Any:
+    ) -> None:
         extra: Dict[str, Any] = {}
         self.media_type = media_type
         self.content_encoding = content_encoding
         self.example = example
         self.examples = examples
         extra.update(media_type=self.media_type)
         extra.update(content_encoding=self.content_encoding)
+        extra.update(embed=embed)
         super().__init__(
             default=default,
             title=title,
             alias=alias,
             description=description,
             const=const,
             gt=gt,
@@ -363,15 +365,15 @@
         le: Optional[float] = None,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         regex: Optional[str] = None,
         example: Any = Undefined,
         examples: Optional[Dict[str, Any]] = None,
         **extra: Any,
-    ):
+    ) -> None:
         super().__init__(
             default=default,
             embed=True,
             media_type=media_type,
             content_encoding=content_encoding,
             alias=alias,
             title=title,
@@ -405,15 +407,15 @@
         le: Optional[float] = None,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         regex: Optional[str] = None,
         example: Any = Undefined,
         examples: Optional[Dict[str, Any]] = None,
         **extra: Any,
-    ):
+    ) -> None:
         super().__init__(
             default=default,
             embed=True,
             media_type=media_type,
             content_encoding=content_encoding,
             alias=alias,
             title=title,
@@ -458,20 +460,20 @@
 @dataclass
 class DirectInject:
     def __init__(
         self,
         dependency: Optional[Callable[..., Any]] = None,
         *,
         use_cache: bool = True,
-    ):
+    ) -> None:
         self.dependency = dependency
         self.use_cache = use_cache
 
-    def __hash__(self):
-        values = {}
+    def __hash__(self) -> int:
+        values: Dict[str, Any] = {}
         for key, value in self.__dict__.items():
             values[key] = None
             if isinstance(value, (list, set)):
                 values[key] = tuple(value)
             else:
                 values[key] = value
         return hash((type(self),) + tuple(values))
```

### Comparing `esmerald-1.2.5/esmerald/parsers.py` & `esmerald-1.3.0/esmerald/parsers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextlib import suppress
 from json import JSONDecodeError, loads
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Dict
 
 from pydantic import BaseConfig, BaseModel
 from pydantic.fields import SHAPE_LIST, SHAPE_SINGLETON
 
 from esmerald.datastructures import UploadFile
 from esmerald.enums import EncodingType
 
@@ -19,31 +19,31 @@
     Pydantic BaseModel by default doesn't handle with hashable types the same way
     a python object would and therefore there are types that are mutable (list, set)
     not hashable and those need to be handled properly.
 
     HashableBaseModel handles those corner cases.
     """
 
-    def __hash__(self):
-        values = {}
+    def __hash__(self) -> int:
+        values: Dict[str, Any] = {}
         for key, value in self.__dict__.items():
             values[key] = None
             if isinstance(value, (list, set)):
                 values[key] = tuple(value)
             else:
                 values[key] = value
         return hash((type(self),) + tuple(values))
 
 
 class ArbitraryHashableBaseModel(HashableBaseModel):
     """
     Same as HashableBaseModel but allowing arbitrary values
     """
 
-    class Config(HashableBaseModel.Config):
+    class Config:
         extra = "allow"
         arbitrary_types_allowed = True
 
 
 class BaseModelExtra(BaseModel):
     """
     BaseModel that allows extra to be passed.
@@ -58,35 +58,34 @@
     ArbitratyBaseModel that allows arbitrary_types_allowed to be passed.
     """
 
     class Config(BaseConfig):
         arbitrary_types_allowed = True
 
 
-def validate_media_type(field: "ModelField", values: "DictAny"):
+def validate_media_type(field: "ModelField", values: Any) -> Any:
     """
     Validates the media type against the available types.
     """
-    if field.shape in SHAPE_LIST:
+    if field.shape == SHAPE_LIST:
         return list(values.values())
-    if field.shape in SHAPE_SINGLETON and field.type_in[UploadFile] and values:
+    if field.shape == SHAPE_SINGLETON and field.type_in[UploadFile] and values:
         return list(values.values())[0]
 
 
 def parse_form_data(media_type: "EncodingType", form_data: "FormData", field: "ModelField") -> Any:
     values: "DictAny" = {}
     for key, value in form_data.multi_items():
         if not isinstance(value, UploadFile):
             with suppress(JSONDecodeError):
                 value = loads(value)
         if isinstance(value, UploadFile):
             value = UploadFile(
-                filename=value.filename,
                 file=value.file,
-                content_type=value.content_type,
+                filename=value.filename,
                 headers=value.headers,
             )
         if values.get(key):
             if isinstance(values[key], list):
                 values[key].append(value)
             else:
                 values[key] = [values[key], value]
```

### Comparing `esmerald-1.2.5/esmerald/requests.py` & `esmerald-1.3.0/esmerald/requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from json import loads
-from typing import TYPE_CHECKING, Any, TypeVar, cast
+from typing import TYPE_CHECKING, Any, cast
 
-from starlette.datastructures import URL
+from starlette.datastructures import URL  # noqa
 from starlette.requests import ClientDisconnect as ClientDisconnect  # noqa
 from starlette.requests import HTTPConnection as HTTPConnection  # noqa: F401
 from starlette.requests import Request as StarletteRequest  # noqa: F401
 from starlette.requests import empty_receive, empty_send  # noqa
 
-from esmerald.exceptions import ImproperlyConfigured
 from esmerald.typing import Void
 
 if TYPE_CHECKING:
     from esmerald.applications import Esmerald
     from esmerald.conf.global_settings import EsmeraldAPISettings
     from esmerald.types import HTTPMethod, Receive, Scope, Send
 
-User = TypeVar("User")
-
 
 class Request(StarletteRequest):
     def __init__(
         self,
         scope: "Scope",
         receive: "Receive" = empty_receive,
         send: "Send" = empty_send,
@@ -29,22 +26,14 @@
         self._json: Any = Void
 
     @property
     def app(self) -> "Esmerald":
         return cast("Esmerald", self.scope["app"])
 
     @property
-    def user(self) -> User:
-        if "user" not in self.scope:
-            raise ImproperlyConfigured(
-                "'user' is not defined in scope, install an AuthMiddleware to set it"
-            )
-        return cast("User", self.scope["user"])
-
-    @property
     def method(self) -> "HTTPMethod":
         return cast("HTTPMethod", self.scope["method"])
 
     @property
     def global_settings(self) -> Any:
         assert (
             "global_settings" in self.scope
@@ -54,21 +43,19 @@
     @property
     def app_settings(self) -> Any:
         assert (
             "app_settings" in self.scope
         ), "RequestSettingsMiddleware must be added to the middlewares"
         return cast("EsmeraldAPISettings", self.scope["app_settings"])
 
-    async def json(self):
+    async def json(self) -> Any:
         if self._json is Void:
             if "_body" in self.scope:
                 body = self.scope["_body"]
             else:
-                body = self.scope["_body"] = await self.body() or "null".encode("utf-8")
+                body = self.scope["_body"] = await self.body() or b"null"
             self._json = loads(body)
         return self._json
 
-    def url_for(self, __name: str, **path_params: Any) -> URL:
-        url = super().url_for(__name, **path_params)
-        if isinstance(url, URL):
-            return str(url)
-        return url
+    def url_for(self, __name: str, **path_params: Any) -> Any:
+        url: URL = super().url_for(__name, **path_params)
+        return str(url)
```

### Comparing `esmerald-1.2.5/esmerald/testclient.py` & `esmerald-1.3.0/esmerald/testclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     List,
     Optional,
     Union,
     cast,
 )
 
 import httpx  # noqa
+from httpx._client import CookieTypes
 from starlette.testclient import TestClient  # noqa
 
 from esmerald.applications import Esmerald
-from esmerald.conf import settings  # noqa
 from esmerald.utils.crypto import get_random_secret_key
 
 if TYPE_CHECKING:
     from typing_extensions import Literal
 
     from esmerald.config import (
         CORSConfig,
@@ -28,16 +28,15 @@
         StaticFilesConfig,
     )
     from esmerald.interceptors.types import Interceptor
     from esmerald.permissions.types import Permission
     from esmerald.types import (
         APIGateHandler,
         Dependencies,
-        DictStr,
-        ExceptionHandlers,
+        ExceptionHandlerMap,
         LifeSpanHandler,
         Middleware,
         SchedulerType,
         SettingsType,
         TemplateConfig,
     )
 
@@ -49,30 +48,30 @@
         self,
         app: Esmerald,
         base_url: str = "http://testserver",
         raise_server_exceptions: bool = True,
         root_path: str = "",
         backend: "Literal['asyncio', 'trio']" = "asyncio",
         backend_options: Optional[Dict[str, Any]] = None,
-        cookies: Optional[httpx._client.CookieTypes] = None,
-        headers: Optional["DictStr"] = None,
+        cookies: Optional[CookieTypes] = None,
+        headers: Dict[str, str] = None,
     ):
         super().__init__(
             app=app,
             base_url=base_url,
             raise_server_exceptions=raise_server_exceptions,
             root_path=root_path,
             backend=backend,
             backend_options=backend_options,
             cookies=cookies,
             headers=headers,
         )
 
     def __enter__(self, *args: Any, **kwargs: Dict[str, Any]) -> "EsmeraldTestClient":
-        return super().__enter__(*args, **kwargs)
+        return cast("EsmeraldTestClient", super().__enter__(*args, **kwargs))
 
 
 def create_client(
     routes: Union["APIGateHandler", List["APIGateHandler"]],
     *,
     settings_config: Optional["SettingsType"] = None,
     debug: Optional[bool] = None,
@@ -84,30 +83,30 @@
     backend: "Literal['asyncio', 'trio']" = "asyncio",
     backend_options: Optional[Dict[str, Any]] = None,
     interceptors: Optional[List["Interceptor"]] = None,
     permissions: Optional[List["Permission"]] = None,
     dependencies: Optional["Dependencies"] = None,
     middleware: Optional[List["Middleware"]] = None,
     csrf_config: Optional["CSRFConfig"] = None,
-    exception_handlers: Optional["ExceptionHandlers"] = None,
+    exception_handlers: Optional["ExceptionHandlerMap"] = None,
     openapi_config: Optional["OpenAPIConfig"] = None,
     on_shutdown: Optional[List["LifeSpanHandler"]] = None,
     on_startup: Optional[List["LifeSpanHandler"]] = None,
     cors_config: Optional["CORSConfig"] = None,
     session_config: Optional["SessionConfig"] = None,
     scheduler_class: Optional["SchedulerType"] = None,
     scheduler_tasks: Optional[Dict[str, str]] = None,
     scheduler_configurations: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
     enable_scheduler: bool = None,
     raise_server_exceptions: bool = True,
-    root_path: Optional[str] = "",
-    static_files_config: Optional[Union["StaticFilesConfig", List["StaticFilesConfig"]]] = None,
+    root_path: str = "",
+    static_files_config: Optional["StaticFilesConfig"] = None,
     template_config: Optional["TemplateConfig"] = None,
     lifespan: Optional[Callable[["Esmerald"], "AsyncContextManager"]] = None,
-    cookies: Optional[httpx._client.CookieTypes] = None,
+    cookies: Optional[CookieTypes] = None,
     redirect_slashes: Optional[bool] = None,
 ) -> EsmeraldTestClient:
     return EsmeraldTestClient(
         app=Esmerald(
             settings_config=settings_config,
             debug=debug,
             routes=cast("Any", routes if isinstance(routes, list) else [routes]),
```

### Comparing `esmerald-1.2.5/esmerald/types.py` & `esmerald-1.3.0/esmerald/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
-    Coroutine,
     Dict,
     List,
+    Mapping,
     Type,
     TypeVar,
     Union,
+    get_args,
 )
 
 from starlette.middleware import Middleware as StarletteMiddleware  # noqa
 from starlette.responses import Response as StarletteResponse  # noqa
 from starlette.types import ASGIApp  # noqa
 from typing_extensions import Literal
 
 from esmerald.backgound import BackgroundTask, BackgroundTasks
-from esmerald.exceptions import HTTPException, MissingDependency, StarletteHTTPException
+from esmerald.exceptions import MissingDependency
 from esmerald.routing.gateways import WebSocketGateway
 from esmerald.routing.router import Include
 
 try:
     from asyncz.schedulers import AsyncIOScheduler  # noqa
 except ImportError:
-    AsyncIOScheduler = Any
+    AsyncIOScheduler = Any  # type: ignore
 
 try:
     from esmerald.config.template import TemplateConfig as TemplateConfig  # noqa
 except MissingDependency:
-    TemplateConfig = Any
+    TemplateConfig = Any  # type: ignore
 
 if TYPE_CHECKING:
     from esmerald.applications import Esmerald
     from esmerald.conf.global_settings import EsmeraldAPISettings  # noqa
     from esmerald.datastructures import Cookie, ResponseHeader, State  # noqa: TC004
     from esmerald.injector import Inject  # noqa
     from esmerald.protocols.middleware import MiddlewareProtocol
     from esmerald.requests import Request  # noqa
     from esmerald.responses import Response  # noqa
-    from esmerald.routing.router import Gateway, HTTPHandler, Router  # noqa
+    from esmerald.routing.router import Gateway, HTTPHandler, Router, WebSocketHandler  # noqa
     from esmerald.routing.views import APIView  # noqa
     from esmerald.websockets import WebSocket  # noqa
 else:
     HTTPHandler = Any
     Message = Any
     Receive = Any
     Scope = Any
@@ -61,54 +62,51 @@
     MiddlewareProtocol = Any
     APIView = Any
     Gateway = Any
     Esmerald = Any
 
 AsyncAnyCallable = Callable[..., Awaitable[Any]]
 HTTPMethod = Literal["GET", "POST", "DELETE", "PATCH", "PUT", "HEAD"]
+HTTPMethods = get_args(HTTPMethod)
 
 Middleware = Union[
     StarletteMiddleware,
     Type[MiddlewareProtocol],
     Callable[..., ASGIApp],
 ]
 
 ResponseType = Type[Response]
 
 Dependencies = Dict[str, Inject]
 
-CoroutineHandler = Coroutine[Any, Any, Response]
-ExceptionHandler = Union[
-    Callable[
-        [Request, Union[Exception, HTTPException, StarletteHTTPException]],
-        StarletteResponse,
-    ],
-    Callable[[Response, Any], CoroutineHandler],
-]
-ExceptionHandlers = Dict[Union[int, Type[Exception]], ExceptionHandler]
+ExceptionType = TypeVar("ExceptionType", bound=Exception)
+ExceptionHandler = Callable[[Request, ExceptionType], Response]
+ExceptionHandlerMap = Mapping[Union[int, Type[Exception]], ExceptionHandler]
 
-ReservedKwargs = Literal[
+_ReservedKwargs = Literal[
     "request",
     "socket",
     "headers",
     "query",
     "cookies",
     "state",
     "data",
 ]
 
+ReservedKwargs = get_args(_ReservedKwargs)
+
 ResponseHeaders = Dict[str, ResponseHeader]
 ResponseCookies = List[Cookie]
-AsyncAnyCallable = Callable[..., Awaitable[Any]]
+AsyncAnyCallable = Callable[..., Awaitable[Any]]  # type: ignore
 
 
 SchedulerType = AsyncIOScheduler
 DatetimeType = TypeVar("DatetimeType", bound=datetime)
 
-ParentType = Union[APIView, Router]
+ParentType = Union[APIView, Router, Gateway, WebSocketGateway, Esmerald, Include]
 APIGateHandler = Union[
     Gateway,
     WebSocketGateway,
 ]
 
 RouteParent = Union["Router", "Include", "ASGIApp", "Gateway", "WebSocketGateway"]
```

### Comparing `esmerald-1.2.5/esmerald/websockets.py` & `esmerald-1.3.0/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/conf/__init__.py` & `esmerald-1.3.0/esmerald/conf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,22 +29,22 @@
         settings: Any = import_string(settings_module)
 
         for setting, _ in settings().dict().items():
             assert setting.islower(), "%s should be in lowercase." % setting
 
         self._wrapped = settings()
 
-    def __repr__(self: "EsmeraldLazySettings"):
+    def __repr__(self: "EsmeraldLazySettings") -> str:
         # Hardcode the class name as otherwise it yields 'Settings'.
         if self._wrapped is empty:
             return "<EsmeraldLazySettings [Unevaluated]>"
-        return '<EsmeraldLazySettings "%(settings_module)s">' % {
-            "settings_module": self._wrapped.__class__.__name__
-        }
+        return '<EsmeraldLazySettings "{settings_module}">'.format(
+            settings_module=self._wrapped.__class__.__name__
+        )
 
     @property
-    def configured(self):
+    def configured(self) -> Any:
         """Return True if the settings have already been configured."""
         return self._wrapped is not empty
 
 
-settings: APISettings = EsmeraldLazySettings()
+settings: APISettings = EsmeraldLazySettings()  # type: ignore
```

### Comparing `esmerald-1.2.5/esmerald/conf/global_settings.py` & `esmerald-1.3.0/esmerald/conf/global_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Union
 
-from openapi_schemas_pydantic.v3_1_0 import License, SecurityRequirement, Server
-from pydantic import BaseConfig, BaseSettings
+from openapi_schemas_pydantic.v3_1_0 import Contact, License, SecurityRequirement, Server, Tag
+from pydantic import AnyUrl, BaseConfig, BaseSettings
 from starlette.types import Lifespan
 
 from esmerald import __version__
 from esmerald.conf.enums import EnvironmentType
 from esmerald.config import CORSConfig, CSRFConfig, OpenAPIConfig, SessionConfig, StaticFilesConfig
 from esmerald.config.asyncexit import AsyncExitConfig
 from esmerald.interceptors.types import Interceptor
 from esmerald.permissions.types import Permission
 from esmerald.pluggables import Pluggable
 from esmerald.types import (
     APIGateHandler,
     Dependencies,
-    ExceptionHandlers,
+    ExceptionHandlerMap,
     LifeSpanHandler,
     Middleware,
     ResponseCookies,
     ResponseHeaders,
     ResponseType,
-    SchedulerType,
 )
 
 if TYPE_CHECKING:
+    from esmerald.routing.router import Include
     from esmerald.types import TemplateConfig
 
 
 class EsmeraldAPISettings(BaseSettings):
     debug: bool = False
     environment: Optional[str] = EnvironmentType.PRODUCTION
     app_name: str = "Esmerald"
     title: str = "My awesome Esmerald application"
     description: str = "Highly scalable, performant, easy to learn and for every application."
-    contact: Optional[Dict[str, Union[str, Any]]] = {
-        "name": "admin",
-        "email": "admin@myapp.com",
-    }
+    contact: Optional[Contact] = Contact(name="admin", email="admin@myapp.com")
     summary: str = "Esmerald application"
-    terms_of_service: Optional[str] = None
+    terms_of_service: Optional[AnyUrl] = None
     license: Optional[License] = None
     security: Optional[List[SecurityRequirement]] = None
     servers: List[Server] = [Server(url="/")]
     secret_key: str = "my secret"
     version: str = __version__
     allowed_hosts: Optional[List[str]] = ["*"]
     allow_origins: Optional[List[str]] = None
     response_class: Optional[ResponseType] = None
     response_cookies: Optional[ResponseCookies] = None
     response_headers: Optional[ResponseHeaders] = None
     include_in_schema: bool = True
-    tags: Optional[List[str]] = None
+    tags: Optional[List[Tag]] = None
     timezone: str = "UTC"
     use_tz: bool = False
     root_path: Optional[str] = ""
     enable_sync_handlers: bool = True
     enable_scheduler: bool = False
     enable_openapi: bool = True
     redirect_slashes: bool = True
 
     class Config(BaseConfig):
-        extra = "allow"
+        extra = "allow"  # type: ignore
         keep_untouched = (cached_property,)
 
     @property
     def reload(self) -> bool:
         """
         Returns reloading for dev and test environments.
         """
@@ -77,30 +74,30 @@
     def password_hashers(self) -> List[str]:
         return [
             "esmerald.contrib.auth.hashers.PBKDF2PasswordHasher",
             "esmerald.contrib.auth.hashers.PBKDF2SHA1PasswordHasher",
         ]
 
     @property
-    def routes(self) -> List[APIGateHandler]:
+    def routes(self) -> List[Union[APIGateHandler, "Include"]]:
         """
         Property that can be used as an entrypoint for the base app routes and to start the application.
 
         Example:
             from esmerald import Include
 
             class MySettings(EsmeraldAPISettings):
                 @property
                 def routes(self):
                     return Include(path='/api/v1/', namespace='myapp.routes')
         """
         return []
 
     @property
-    def csrf_config(self) -> CSRFConfig:
+    def csrf_config(self) -> Optional[CSRFConfig]:
         """
         Initial Default configuration for the CSRF.
         This can be overwritten in another setting or simply override `secret` or then override
         the `def csrf_config()` property to change the behavior of the whole csrf_config.
 
         Default:
             None
@@ -137,15 +134,15 @@
                 @property
                 def async_exit_config(self) -> AsyncExitConfig:
                     ...
         """
         return AsyncExitConfig()
 
     @property
-    def template_config(self) -> "TemplateConfig":
+    def template_config(self) -> Optional["TemplateConfig"]:
         """
         Initial Default configuration for the TemplateConfig.
         This can be overwritten in another setting or simply override `template_config` or then override
         the `def template_config()` property to change the behavior of the whole template_config.
 
         Esmerald can also support other engines like mako, Diazo, Cheetah. Currently natively
         only supports jinja2 and mako.
@@ -159,15 +156,15 @@
                 @property
                 def template_config(self) -> "TemplateConfig":
                     TemplateConfig(directory='templates', engine=MakoTemplateEngine)
         """
         return None
 
     @property
-    def static_files_config(self) -> StaticFilesConfig:
+    def static_files_config(self) -> Optional[StaticFilesConfig]:
         """
         Simple configuration indicating where the statics will be placed in
         the application.
 
         Default:
             None
 
@@ -177,15 +174,15 @@
                 @property
                 def static_files_config(self) -> StaticFilesConfig:
                     StaticFilesConfig(path='/', directories=...)
         """
         return None
 
     @property
-    def cors_config(self) -> CORSConfig:
+    def cors_config(self) -> Optional[CORSConfig]:
         """
         Initial Default configuration for the CORS.
         This can be overwritten in another setting or simply override `allow_origins` or then override
         the `def cors_config()` property to change the behavior of the whole cors_config.
 
         Default:
             CORSConfig
@@ -200,15 +197,15 @@
                     ...
         """
         if not self.allow_origins:
             return None
         return CORSConfig(allow_origins=self.allow_origins)
 
     @property
-    def session_config(self) -> SessionConfig:
+    def session_config(self) -> Optional[SessionConfig]:
         """
         Initial Default configuration for the SessionConfig.
         This can be overwritten in another setting or simply override `session_config` or then override
         the `def session_config()` property to change the behavior of the whole session_config.
 
         Default:
             None
@@ -252,15 +249,15 @@
             servers=self.servers,
             summary=self.summary,
             security=self.security,
             tags=self.tags,
         )
 
     @property
-    def middleware(self) -> List[Middleware]:
+    def middleware(self) -> Sequence[Middleware]:
         """
         Initial Default configuration for the middleware.
         This can be overwritten in another setting or simply override `def middleware()`.
 
         Example:
 
             class MySettings(EsmeraldAPISettings):
@@ -268,15 +265,15 @@
                 @property
                 def middleware(self) -> List[Middleware]:
                     return [EsmeraldMiddleware]
         """
         return []
 
     @property
-    def scheduler_class(self) -> SchedulerType:
+    def scheduler_class(self) -> Any:
         """
         Scheduler class to be used within the application.
         """
         if not self.enable_scheduler:
             return None
 
         try:
@@ -366,15 +363,15 @@
     def dependencies(self) -> Dependencies:
         """
         Returns the dependencies of Esmerald main app.
         """
         return {}
 
     @property
-    def exception_handlers(self) -> ExceptionHandlers:
+    def exception_handlers(self) -> ExceptionHandlerMap:
         """
         Default exception handlers to be loaded when the application starts
         """
         return {}
 
     @property
     def on_startup(self) -> Union[List[LifeSpanHandler], None]:
@@ -387,15 +384,15 @@
     def on_shutdown(self) -> Union[List[LifeSpanHandler], None]:
         """
         List of events/actions to be done on_shutdown.
         """
         return None
 
     @property
-    def lifespan(self) -> "Lifespan":
+    def lifespan(self) -> Optional["Lifespan"]:
         """
         Custom lifespan that can be passed instead of the default Starlette.
 
         The lifespan context function is a newer style that replaces
         on_startup / on_shutdown handlers. Use one or the other, not both.
         """
         return None
```

### Comparing `esmerald-1.2.5/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-1.3.0/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-1.3.0/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-1.3.0/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from esmerald import Esmerald, Include
 
 
 def build_path():
     """
     Builds the path of the project and project root.
     """
-    Path(__file__).resolve().parent.parent
     SITE_ROOT = os.path.dirname(os.path.realpath(__file__))
 
     if SITE_ROOT not in sys.path:
         sys.path.append(SITE_ROOT)
         sys.path.append(os.path.join(SITE_ROOT, "apps"))
```

### Comparing `esmerald-1.2.5/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-1.3.0/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-1.3.0/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/config/jwt.py` & `esmerald-1.3.0/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/config/openapi.py` & `esmerald-1.3.0/esmerald/config/openapi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import partial
-from typing import TYPE_CHECKING, Dict, List, Optional, Set, Type, Union, cast
+from typing import TYPE_CHECKING, Dict, List, Optional, Set, Type, Union
 
 from openapi_schemas_pydantic import construct_open_api_with_schema_class
 from openapi_schemas_pydantic.v3_1_0 import (
     Components,
     Contact,
     ExternalDocumentation,
     Info,
@@ -67,50 +67,52 @@
                         merged_value_dict.update(value)
                         setattr(merged_components, key, merged_value_dict)
             self.components = merged_components
 
         return OpenAPI(
             externalDocs=self.external_docs,
             security=self.security,
-            components=cast("Components", self.components),
+            components=self.components,
             servers=self.servers,
             tags=self.tags,
             webhooks=self.webhooks,
             info=Info(
                 title=self.title,
                 version=self.version,
                 description=self.description,
                 contact=self.contact,
                 license=self.license,
                 summary=self.summary,
                 termsOfService=self.terms_of_service,
             ),
         )
 
-    def get_http_verb(self, path_item):
+    def get_http_verb(self, path_item: PathItem) -> str:
         if getattr(path_item, "get", None):
             return HttpMethod.GET.value.lower()
         elif getattr(path_item, "post", None):
             return HttpMethod.POST.value.lower()
         elif getattr(path_item, "put", None):
             return HttpMethod.PUT.value.lower()
         elif getattr(path_item, "patch", None):
             return HttpMethod.PATCH.value.lower()
         elif getattr(path_item, "delete", None):
             return HttpMethod.DELETE.value.lower()
         elif getattr(path_item, "header", None):
             return HttpMethod.HEAD.value.lower()
 
-    def create_openapi_schema_model(self, app: Type["Esmerald"]) -> "OpenAPI":
+        return HttpMethod.GET.value.lower()
+
+    def create_openapi_schema_model(self, app: "Esmerald") -> "OpenAPI":
         from esmerald.applications import ChildEsmerald, Esmerald
 
         schema = self.to_openapi_schema()
         schema.paths = {}
 
-        def parse_route(app, prefix=""):
+        def parse_route(app, prefix=""):  # type: ignore
             if getattr(app, "routes", None) is None:
                 return
 
             # Making sure that ChildEsmerald or esmerald
             if hasattr(app, "app"):
                 if (
                     isinstance(app.app, (Esmerald, ChildEsmerald))
@@ -138,34 +140,34 @@
                             handler.include_in_schema
                             for handler, _ in route.handler.route_map.values()
                         )
                         and (route.path_format or "/") not in schema.paths
                     ):
                         path = clean_path(prefix + route.path)
                         path_item = create_path_item(
-                            route=route.handler,
+                            route=route.handler,  # type: ignore
                             create_examples=self.create_examples,
                             use_handler_docstrings=self.use_handler_docstrings,
                         )
                         verb = self.get_http_verb(path_item)
                         if path not in schema.paths:
-                            schema.paths[path] = {}
-                        if verb not in schema.paths[path]:
-                            schema.paths[path][verb] = {}
-                        schema.paths[path][verb] = getattr(path_item, verb, None)
+                            schema.paths[path] = {}  # type: ignore
+                        if verb not in schema.paths[path]:  # type: ignore
+                            schema.paths[path][verb] = {}  # type: ignore
+                        schema.paths[path][verb] = getattr(path_item, verb, None)  # type: ignore
                     continue
 
                 route_app = getattr(route, "app", None)
                 if not route_app:
                     continue
 
                 if isinstance(route_app, partial):
                     try:
                         route_app = route_app.__wrapped__
                     except AttributeError:
                         pass
 
                 path = clean_path(prefix + route.path)
-                parse_route(route, prefix=f"{path}")
+                parse_route(route, prefix=f"{path}")  # type: ignore
 
-        parse_route(app)
+        parse_route(app)  # type: ignore
         return construct_open_api_with_schema_class(schema)
```

### Comparing `esmerald-1.2.5/esmerald/config/session.py` & `esmerald-1.3.0/esmerald/config/session.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class SessionConfig(BaseModel):
     class Config(BaseConfig):
         arbitrary_types_allowed = True
 
     secret_key: Union[str, Secret]
     path: str = "/"
     session_cookie: constr(min_length=1, max_length=256) = "session"  # type: ignore[valid-type]
-    max_age: int = SECONDS_IN_A_DAY * 180  # type: ignore[valid-type]
+    max_age: int = SECONDS_IN_A_DAY * 180
     https_only: bool = False
     same_site: Literal["lax", "strict", "none"] = "lax"
 
     @validator("secret_key", always=True)
     def validate_secret(cls, value: Secret) -> Secret:  # pylint: disable=no-self-argument
         if len(value) not in [16, 24, 32]:
             raise ValueError("secret length must be 16 (128 bit), 24 (192 bit) or 32 (256 bit)")
```

### Comparing `esmerald-1.2.5/esmerald/config/static_files.py` & `esmerald-1.3.0/esmerald/config/static_files.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,18 +26,18 @@
         self,
     ) -> Dict[str, Union[bool, int, DirectoryPath, List[Union[str, Tuple[str, str]]]]]:
         """
         Builds the necessary kwargs to create an StaticFiles object.
         """
         kwargs = {"html": self.html, "check_dir": self.check_dir}
         if self.packages:
-            kwargs.update({"packages": self.packages})
+            kwargs.update({"packages": self.packages})  # type: ignore
         if self.directory:
-            kwargs.update({"directory": str(self.directory)})
-        return kwargs
+            kwargs.update({"directory": str(self.directory)})  # type: ignore
+        return kwargs  # type: ignore
 
     def to_app(self) -> "ASGIApp":
         """
         It can be three scenarios
         """
 
-        return StaticFiles(**self._build_kwargs())
+        return StaticFiles(**self._build_kwargs())  # type: ignore
```

### Comparing `esmerald-1.2.5/esmerald/contrib/encoding.py` & `esmerald-1.3.0/esmerald/contrib/encoding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 import codecs
 import datetime
 import locale
-import typing
 from decimal import Decimal
+from typing import Any, Optional, Union
 from urllib.parse import quote
 
+_PROTECTED_TYPES = (
+    type(None),
+    int,
+    float,
+    Decimal,
+    datetime.datetime,
+    datetime.date,
+    datetime.time,
+)
+
 
 class ExtraUnicodeDecodeError(UnicodeDecodeError):
-    def __init__(self, obj: typing.Any, *args):
+    def __init__(self, obj: Any, *args: Any) -> None:
         self.obj = obj
         super().__init__(*args)
 
-    def __str__(self):
-        return "%s. You passed in %r (%s)" % (
+    def __str__(self) -> str:
+        return "{}. You passed in {!r} ({})".format(
             super().__str__(),
             self.obj,
             type(self.obj),
         )
 
 
 def smart_str(
-    s, encoding: str = "utf-8", strings_only: bool = False, errors: str = "strict"
+    s: Any, encoding: str = "utf-8", strings_only: bool = False, errors: str = "strict"
 ) -> str:
     """
     Return a string representing 's'. Treat bytestrings using the 'encoding'
     codec.
     """
     return force_str(s, encoding, strings_only, errors)
 
 
-_PROTECTED_TYPES = (
-    type(None),
-    int,
-    float,
-    Decimal,
-    datetime.datetime,
-    datetime.date,
-    datetime.time,
-)
-
-
-def is_protected_type(obj: typing.Any) -> bool:
+def is_protected_type(obj: Any) -> bool:
     """Determine if the object instance is of a protected type.
 
     Objects of protected types are preserved as-is when passed to
     force_str(strings_only=True).
     """
     return isinstance(obj, _PROTECTED_TYPES)
 
 
 def force_str(
-    s, encoding: str = "utf-8", strings_only: bool = False, errors: str = "strict"
-) -> str:
+    s: Any, encoding: str = "utf-8", strings_only: bool = False, errors: str = "strict"
+) -> Union[Any, str]:
     """
     Similar to smart_str(), except that lazy instances are resolved to
     strings, rather than kept as lazy objects.
 
     If strings_only is True, don't convert (some) non-string-like objects.
     """
     # Handle the common case first for performance reasons.
@@ -70,25 +69,25 @@
             s = str(s)
     except UnicodeDecodeError as e:
         raise ExtraUnicodeDecodeError(s, *e.args) from e
     return s
 
 
 def smart_bytes(
-    s, encoding: str = "utf-8", strings_only: bool = False, errors: str = "strict"
+    s: Any, encoding: str = "utf-8", strings_only: bool = False, errors: str = "strict"
 ) -> bytes:
     """
     Return a bytestring version of 's', encoded as specified in 'encoding'.
     """
     return force_bytes(s, encoding, strings_only, errors)
 
 
 def force_bytes(
-    s, encoding: str = "utf-8", strings_only: bool = False, errors: str = "strict"
-) -> bytes:
+    s: Any, encoding: str = "utf-8", strings_only: bool = False, errors: str = "strict"
+) -> Union[Any, bytes]:
     """
     Similar to smart_bytes, except that lazy instances are resolved to
     strings, rather than kept as lazy objects.
 
     If strings_only is True, don't convert (some) non-string-like objects.
     """
     # Handle the common case first for performance reasons.
@@ -115,15 +114,15 @@
 }
 # And then everything above 128, because bytes ≥ 128 are part of multibyte
 # Unicode characters.
 _hexdig = "0123456789ABCDEFabcdef"
 _hextobyte.update({(a + b).encode(): bytes.fromhex(a + b) for a in _hexdig[8:] for b in _hexdig})
 
 
-def uri_to_iri(uri: typing.Union[str, bytes]) -> typing.Union[str, bytes]:
+def uri_to_iri(uri: Optional[Union[str, bytes]] = None) -> Union[str, bytes, None]:
     """
     Convert a Uniform Resource Identifier(URI) into an Internationalized
     Resource Identifier(IRI).
 
     This is the algorithm from section 3.2 of RFC 3987, excluding step 4.
 
     Take an URI in ASCII bytes (e.g. '/I%20%E2%99%A5%20Django/') and return
@@ -133,15 +132,15 @@
         return uri
     uri = force_bytes(uri)
     # Fast selective unquote: First, split on '%' and then starting with the
     # second block, decode the first 2 bytes if they represent a hex code to
     # decode. The rest of the block is the part after '%AB', not containing
     # any '%'. Add that to the output without further processing.
     # deepcode ignore BadMixOfStrAndBytes: False positive
-    bits = uri.split(bytes("%"))
+    bits = uri.split(b"%")
     if len(bits) == 1:
         iri = uri
     else:
         parts = [bits[0]]
         append = parts.append
         hextobyte = _hextobyte
         for item in bits[1:]:
@@ -149,18 +148,18 @@
             if _hex in hextobyte:
                 append(hextobyte[item[:2]])
                 append(item[2:])
             else:
                 append(b"%")
                 append(item)
         iri = b"".join(parts)
-    return repercent_broken_unicode(iri).decode()
+    return repercent_broken_unicode(iri).decode()  # type: ignore
 
 
-def escape_uri_path(path: str) -> typing.Union[str, bytes]:
+def escape_uri_path(path: str) -> Union[str, bytes]:
     """
     Escape the unsafe characters from the path portion of a Uniform Resource
     Identifier (URI).
     """
     # These are the "reserved" and "unreserved" characters specified in
     # sections 2.2 and 2.3 of RFC 2396:
     #   reserved    = ";" | "/" | "?" | ":" | "@" | "&" | "=" | "+" | "$" | ","
@@ -169,38 +168,39 @@
     # The list of safe characters here is constructed subtracting ";", "=",
     # and "?" according to section 3.3 of RFC 2396.
     # The reason for not subtracting and escaping "/" is that we are escaping
     # the entire path, not a path segment.
     return quote(path, safe="/:@&+$,-_.!~*'()")
 
 
-def punycode(domain: typing.Union[str, bytes]) -> str:
+def punycode(domain: bytes) -> str:
     """Return the Punycode of the given domain if it's non-ASCII."""
-    return domain.encode("idna").decode("ascii")
+    domain = domain.encode("idna")
+    return domain.decode("ascii")
 
 
 def repercent_broken_unicode(path: str) -> str:
     """
     As per section 3.2 of RFC 3987, step three of converting a URI into an IRI,
     repercent-encode any octet produced that is not part of a strictly legal
     UTF-8 octet sequence.
     """
     while True:
         try:
             path.decode()
         except UnicodeDecodeError as e:
             # CVE-2019-14235: A recursion shouldn't be used since the exception
             # handling uses massive amounts of memory
-            repercent = quote(path[e.start : e.end], safe=b"/#%[]=:;$&()+,!?*@'~")  # noqa: E203
-            path = path[: e.start] + repercent.encode() + path[e.end :]  # noqa: E203
+            repercent = quote(path[e.start : e.end], safe=b"/#%[]=:;$&()+,!?*@'~")
+            path = path[: e.start] + repercent.encode() + path[e.end :]  # type: ignore
         else:
             return path
 
 
-def filepath_to_uri(path: str) -> str:
+def filepath_to_uri(path: Optional[str] = None) -> Union[str, None]:
     """Convert a file system path to a URI portion that is suitable for
     inclusion in a URL.
 
     Encode certain chars that would normally be recognized as special chars
     for URIs. Do not encode the ' character, as it is a valid character
     within URIs. See the encodeURIComponent() JavaScript function for details.
     """
```

### Comparing `esmerald-1.2.5/esmerald/contrib/auth/hashers.py` & `esmerald-1.3.0/esmerald/contrib/auth/hashers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,65 @@
-"""
-Esmerald is a great framework to create microservices.
-These hashers and the way it was implemented was heavily
-based on the clean design done by Django but we used
-"""
-
 import functools
 import hashlib
 import math
 import secrets
 import warnings
+from typing import Any, Callable, Dict, Optional, Sequence, Union
 
 from passlib.context import CryptContext
 
 from esmerald.conf import settings
 from esmerald.exceptions import ImproperlyConfigured
 from esmerald.utils.module_loading import import_string
 
 from .constants import (
     RANDOM_STRING_CHARS,
     UNUSABLE_PASSWORD_PREFIX,
     UNUSABLE_PASSWORD_SUFFIX_LENGTH,
 )
 
 
-def is_password_usable(encoded):
+def is_password_usable(encoded: Optional[str]) -> bool:
     """
     Return True if this password wasn't generated by
     User.set_unusable_password(), i.e. make_password(None).
     """
     return encoded is None or not encoded.startswith(UNUSABLE_PASSWORD_PREFIX)
 
 
-def check_password(password, encoded, setter=None, preferred="default"):
+def check_password(
+    password: str, encoded: str, setter: Callable[..., Any] = None, preferred: str = "default"
+) -> bool:
     """
     Return a boolean of whether the raw password matches the three
     part encoded digest.
 
     If setter is specified, it'll be called when you need to
     regenerate the password.
     """
     if password is None or not is_password_usable(encoded):
         return False
 
-    preferred = get_hasher(preferred)
+    preferred_hasher: BasePasswordHasher = get_hasher(preferred)
     try:
         hasher_handler = identify_hasher(encoded)
     except ValueError:
         # encoded is gibberish or uses a hasher that's no longer installed.
         return False
 
-    hasher_changed = hasher_handler.algorithm != preferred.algorithm
-    must_update = hasher_changed or preferred.must_update(encoded)
-    is_correct = hasher_handler.hasher.verify(password, encoded)
+    hasher_changed = hasher_handler.algorithm != preferred_hasher.algorithm
+    must_update: bool = hasher_changed or preferred_hasher.must_update(encoded)
+    is_correct: bool = hasher_handler.hasher.verify(password, encoded)
 
     if setter and is_correct and must_update:
         setter(password)
     return is_correct
 
 
-def make_password(password, hasher="default"):
+def make_password(password: Optional[str], hasher: str = "default") -> str:
     """
     Turn a plain-text password into a hash for database storage
 
     Same as encode() but generate a new random salt. If password is None then
     return a concatenation of UNUSABLE_PASSWORD_PREFIX and a random string,
     which disallows logins. Additional random string reduces chances of gaining
     access to staff or superuser accounts. See ticket #20079 for more info.
@@ -70,23 +67,23 @@
     if password is None:
         return UNUSABLE_PASSWORD_PREFIX + get_random_string(UNUSABLE_PASSWORD_SUFFIX_LENGTH)
     if not isinstance(password, (bytes, str)):
         raise TypeError(
             "Password must be a string or bytes, got %s." % type(password).__qualname__
         )
 
-    hasher_handler = get_hasher(hasher)
+    hasher_handler: BasePasswordHasher = get_hasher(hasher)
 
     # Passlib includes salt in almost every hash
     return hasher_handler.get_hashed_password(password)
 
 
 @functools.lru_cache
-def get_hashers():
-    hashers = []
+def get_hashers() -> Sequence["BasePasswordHasher"]:
+    hashers: Sequence["BasePasswordHasher"] = []
 
     password_hashers = getattr(settings, "password_hashers", None)
     if not password_hashers:
         warnings.warn("`password_hashers` missing from settings.", stacklevel=2)
         return hashers
 
     for hasher_path in settings.password_hashers:
@@ -97,63 +94,60 @@
                 "hasher doesn't specify an algorithm name: %s" % hasher_path
             )
         hashers.append(hasher)
     return hashers
 
 
 @functools.lru_cache
-def get_hashers_by_algorithm():
+def get_hashers_by_algorithm() -> Dict[str, "BasePasswordHasher"]:
     return {hasher.algorithm_name: hasher for hasher in get_hashers()}
 
 
-def must_update_salt(salt, expected_entropy):
+def must_update_salt(salt: str, expected_entropy: int) -> bool:
     # Each character in the salt provides log_2(len(alphabet)) bits of entropy.
     return len(salt) * math.log2(len(RANDOM_STRING_CHARS)) < expected_entropy
 
 
-def get_random_string(length, allowed_chars=RANDOM_STRING_CHARS):
+def get_random_string(length: int, allowed_chars: str = RANDOM_STRING_CHARS) -> str:
     """
     Return a securely generated random string.
 
     The bit length of the returned value can be calculated with the formula:
         log_2(len(allowed_chars)^length)
 
     For example, with default `allowed_chars` (26+26+10), this gives:
       * length: 12, bit length =~ 71 bits
       * length: 22, bit length =~ 131 bits
     """
     return "".join(secrets.choice(allowed_chars) for _ in range(length))  # pragma no cover
 
 
-def get_hasher(algorithm="default"):
+def get_hasher(algorithm: str = "default") -> "BasePasswordHasher":
     """
     Return an instance of a loaded password hasher.
 
     If algorithm is 'default', return the default hasher. Lazily import hashers
     specified in the project's settings config if needed.
     """
-    if hasattr(algorithm, "algorithm"):
-        return algorithm
-
-    elif algorithm == "default":
+    if algorithm == "default":
         return get_hashers()[0]
 
     else:
         hashers = get_hashers_by_algorithm()
         try:
             return hashers[algorithm]
         except KeyError as e:
             raise ValueError(
                 "Unknown password hashing algorithm '%s'. "
                 "Did you specify it in your settings? "
                 "setting?" % algorithm
             ) from e
 
 
-def identify_hasher(encoded):
+def identify_hasher(encoded: str) -> "BasePasswordHasher":
     """
     Return an instance of a loaded password hasher.
 
     Identify hasher algorithm by examining encoded hash, and call
     get_hasher() to return hasher. Raise ValueError if
     algorithm cannot be identified, or if hasher is not loaded.
     """
@@ -167,84 +161,84 @@
         algorithm = "unsalted_sha1"
     else:
         algorithm = encoded.split("$", 1)[0]
     return get_hasher(algorithm)
 
 
 class BasePasswordHasher:
-    hasher = None
-    algorithm = None
-    algorithm_name = None
-    digest = None
+    hasher: CryptContext
+    algorithm: str
+    algorithm_name: str
+    digest: Any
     library = None
-    salt_entropy = 128
+    salt_entropy: int = 128
 
-    def __init__(self) -> None:
-        if not self.algorithm or not self.algorithm_name:
+    def __init__(self, **kwargs: Any) -> None:
+        if self.algorithm is None or self.algorithm_name is None:
             raise NotImplementedError(
                 "subclasses of BasePasswordHasher must provide an algorithm and algorithm_name."
             )
         self.hasher = CryptContext(schemes=[self.algorithm], deprecated="auto")
 
-    def get_hashed_password(self, password: str) -> str:
+    def get_hashed_password(self, password: str) -> Union[str, Any]:
         return self.hasher.hash(password)
 
-    def salt(self):
+    def salt(self) -> str:
         """
         Generate a cryptographically secure nonce salt in ASCII with an entropy
         of at least `salt_entropy` bits.
         """
         # Each character in the salt provides
         # log_2(len(alphabet)) bits of entropy.
         char_count = math.ceil(self.salt_entropy / math.log2(len(RANDOM_STRING_CHARS)))
         return get_random_string(char_count, allowed_chars=RANDOM_STRING_CHARS)
 
-    def decode(self, encoded):
+    def decode(self, encoded: str) -> Dict[str, Any]:
         """
         Return a decoded database value.
 
         The result is a dictionary and should contain `algorithm`, `hash`, and
         `salt`. Extra keys can be algorithm specific like `iterations` or
         `work_factor`.
         """
         raise NotImplementedError(
             "subclasses of BasePasswordHasher must provide a decode() method."
         )
 
-    def _check_encode_args(self, password, salt):
+    def _check_encode_args(self, password: str, salt: str) -> None:
         if password is None:
             raise TypeError("password must be provided.")
         if not salt or "$" in salt:
             raise ValueError("salt must be provided and cannot contain $.")
 
-    def must_update(self, encoded=None):
+    def must_update(self, encoded: str) -> bool:
         return False
 
 
 class PBKDF2PasswordHasher(BasePasswordHasher):
     """
     Handles PBKDF2 passwords
     """
 
     algorithm = "django_pbkdf2_sha256"
     algorithm_name = "pbkdf2_sha256"
     iterations = 390000
     digest = hashlib.sha256
 
-    def decode(self, encoded):
+    def decode(self, encoded: str) -> Dict[str, Any]:
         algorithm, iterations, salt, _hash = encoded.split("$", 3)
         assert algorithm == self.algorithm_name
         return {
             "algorithm": algorithm,
             "hash": _hash,
             "iterations": int(iterations),
             "salt": salt,
         }
 
-    def must_update(self, encoded):
+    def must_update(self, encoded: str) -> bool:
         decoded = self.decode(encoded)
         update_salt = must_update_salt(decoded["salt"], self.salt_entropy)
         return (decoded["iterations"] != self.iterations) or update_salt
 
 
 class PBKDF2SHA1PasswordHasher(PBKDF2PasswordHasher):
     """
```

### Comparing `esmerald-1.2.5/esmerald/contrib/auth/common/middleware.py` & `esmerald-1.3.0/esmerald/contrib/auth/common/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, TypeVar
+from typing import TypeVar
 
 from jose import JWSError, JWTError
 from starlette.requests import HTTPConnection
 from starlette.types import ASGIApp
 
 from esmerald.config.jwt import JWTConfig
 from esmerald.exceptions import AuthenticationError, NotAuthorized
@@ -17,15 +17,15 @@
     The simple JWT authentication Middleware.
     """
 
     def __init__(
         self,
         app: "ASGIApp",
         config: "JWTConfig",
-        user_model: Generic[T],
+        user_model: T,
     ):
         super().__init__(app)
         """
         The user is simply the class type to be queried from the Tortoise ORM.
 
         Example how to use:
 
@@ -75,15 +75,15 @@
 
         if token_type not in self.config.auth_header_types:
             raise NotAuthorized(detail=f"{token_type} is not an authorized header type")
 
         try:
             token = Token.decode(
                 token=auth_token, key=self.config.signing_key, algorithms=[self.config.algorithm]
-            )
+            )  # type: ignore
         except (JWSError, JWTError) as e:
             raise AuthenticationError(str(e)) from e
 
         user = await self.retrieve_user(token.sub)
         if not user:
             raise AuthenticationError("User not found.")
         return AuthResult(user=user)
```

### Comparing `esmerald-1.2.5/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-1.3.0/esmerald/contrib/auth/saffier/base_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 import saffier
 
 from esmerald.contrib.auth.hashers import check_password, is_password_usable, make_password
 
 
 class AbstractUser(saffier.Model):
     """
@@ -22,70 +24,84 @@
     # be passed to password_changed() after the model is saved.
     _password = None
 
     class Meta:
         abstract = True
 
     @property
-    async def is_authenticated(self):
+    async def is_authenticated(self) -> bool:
         """
         Always return True.
         """
         return True
 
-    async def set_password(self, raw_password):
-        self.password = make_password(raw_password)
+    async def set_password(self, raw_password: str) -> None:
+        self.password = make_password(raw_password)  # type: ignore
         self._password = raw_password
         await self.update(password=make_password(raw_password))
 
-    async def check_password(self, raw_password):
+    async def check_password(self, raw_password: str) -> bool:
         """
         Return a boolean of whether the raw_password was correct. Handles
         hashing formats behind the scenes.
         """
 
-        async def setter(raw_password):
-            self.set_password(raw_password)
+        async def setter(raw_password: str) -> None:
+            await self.set_password(raw_password)
             # Password hash upgrades shouldn't be considered password changes.
             self._password = None
             await self.update(password=self.password)
 
-        return check_password(raw_password, self.password, setter)
+        return check_password(raw_password, str(self.password), setter)
 
-    async def set_unusable_password(self):
+    async def set_unusable_password(self) -> None:
         # Set a value that will never be a valid hash
-        self.password = make_password(None)
+        self.password = make_password(None)  # type: ignore
 
-    async def has_usable_password(self):
+    async def has_usable_password(self) -> bool:
         """
         Return False if set_unusable_password() has been called for this user.
         """
-        return is_password_usable(self.password)
+        return is_password_usable(self.password)  # type: ignore
 
     @classmethod
-    async def _create_user(cls, username, email, password, **extra_fields):
+    async def _create_user(
+        cls, username: str, email: str, password: str, **extra_fields: Any
+    ) -> "AbstractUser":
         """
         Create and save a user with the given username, email, and password.
         """
         if not username:
             raise ValueError("The given username must be set")
         password = make_password(password)
-        user = await cls.query.create(
+        user: AbstractUser = await cls.query.create(
             username=username, email=email, password=password, **extra_fields
         )
         return user
 
     @classmethod
-    async def create_user(cls, username, email=None, password=None, **extra_fields):
+    async def create_user(
+        cls,
+        username: str,
+        email: str,
+        password: str,
+        **extra_fields: Any,
+    ) -> "AbstractUser":
         extra_fields.setdefault("is_staff", False)
         extra_fields.setdefault("is_superuser", False)
         return await cls._create_user(username, email, password, **extra_fields)
 
     @classmethod
-    async def create_superuser(cls, username, email=None, password=None, **extra_fields):
+    async def create_superuser(
+        cls,
+        username: str,
+        email: str,
+        password: str,
+        **extra_fields: Any,
+    ) -> "AbstractUser":
         extra_fields.setdefault("is_staff", True)
         extra_fields.setdefault("is_superuser", True)
 
         if extra_fields.get("is_staff") is not True:
             raise ValueError("Superuser must have is_staff=True.")
         if extra_fields.get("is_superuser") is not True:
             raise ValueError("Superuser must have is_superuser=True.")
```

### Comparing `esmerald-1.2.5/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-1.3.0/esmerald/contrib/auth/saffier/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Generic, TypeVar
+from typing import Any, TypeVar
 
 from saffier.exceptions import DoesNotFound
 from starlette.types import ASGIApp
 
 from esmerald.config.jwt import JWTConfig
 from esmerald.contrib.auth.common.middleware import CommonJWTAuthMiddleware
 from esmerald.exceptions import AuthenticationError, NotAuthorized
@@ -15,15 +15,15 @@
     The simple JWT authentication Middleware.
     """
 
     def __init__(
         self,
         app: "ASGIApp",
         config: "JWTConfig",
-        user_model: Generic[T],
+        user_model: T,
     ):
         super().__init__(app, config, user_model)
         """
         The user is simply the class type to be queried from the Saffier ORM.
 
         Example how to use:
 
@@ -52,24 +52,24 @@
                 app = Esmerald(routes=[...], middleware=[CustomJWTMidleware])
 
         """
         self.app = app
         self.config = config
         self.user_model = user_model
 
-    async def retrieve_user(self, token_sub: Any) -> Generic[T]:
+    async def retrieve_user(self, token_sub: Any) -> T:
         """
         Retrieves a user from the database using the given token id.
         """
         try:
             sub = int(token_sub)
             token_sub = sub
         except (TypeError, ValueError):
             ...  # noqa
 
         user_field = {self.config.user_id_field: token_sub}
         try:
-            return await self.user_model.query.get(**user_field)
+            return await self.user_model.query.get(**user_field)  # type: ignore
         except DoesNotFound:
             raise NotAuthorized() from None
         except Exception as e:
             raise AuthenticationError(detail=str(e)) from e
```

### Comparing `esmerald-1.2.5/esmerald/core/directives/base.py` & `esmerald-1.3.0/esmerald/core/directives/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,33 +15,34 @@
 printer = Print()
 
 
 class BaseDirective(BaseModel, ABC):
     """The base class from which all directrives derive"""
 
     help: str = ""
-    suppressed_base_arguments = set()
 
     def get_version(self) -> str:
         """
         Returns the current version of Esmerald.
         """
         return esmerald.__version__
 
     def add_arguments(self, parser: Type["argparse.ArgumentParser"]) -> Any:
         """
         Entrypoint for directives and custom arguments
         """
         ...
 
-    def create_parser(self, name: str, subdirective: str, **kwargs):
+    def create_parser(self, name: str, subdirective: str, **kwargs: Any) -> DirectiveParser:
         parser = DirectiveParser(
-            prog="%s %s" % (os.path.basename(name), subdirective), description=self.help, **kwargs
+            prog="{} {}".format(os.path.basename(name), subdirective),
+            description=self.help,
+            **kwargs,
         )
-        self.add_arguments(parser)
+        self.add_arguments(parser)  # type: ignore
         return parser
 
     async def execute_from_command(self, argv: Any, program_name: str, position: int = 5) -> None:
         """
         Executes dynamically the directive from the command line and passing the parameters
         """
         parser = self.create_parser(program_name, argv[position])
@@ -50,15 +51,15 @@
         cmd_options = vars(options)
 
         # Move positional args out of options to mimic legacy optparse
         args = cmd_options.pop("args", ())
         try:
             await self.run(*args, **cmd_options)
         except DirectiveError as e:
-            printer.write_error("%s: %s" % (e.__class__.__name__, e))
+            printer.write_error("{}: {}".format(e.__class__.__name__, e))
             sys.exit(e.returncode)
 
     async def run(self, *args: Any, **options: Any) -> Any:
         """
         Executes the handle()
         """
         if not is_async_callable(self.handle):
@@ -71,9 +72,9 @@
 
     @abstractmethod
     def handle(self, *args: Any, **options: Any) -> Any:
         """The logic of the directive. Subclasses must implement this method"""
         raise NotImplementedError("subclasses of BaseDirective must provide a handle() method.")
 
     class Config(BaseConfig):
-        extra = "allow"
+        extra = "allow"  # type: ignore
         arbitrary_types_allowed = True
```

### Comparing `esmerald-1.2.5/esmerald/core/directives/cli.py` & `esmerald-1.3.0/esmerald/core/directives/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 import os
 import sys
 import typing
 from functools import wraps
+from typing import Callable, TypeVar
 
 import click
 
 from esmerald.core.directives.constants import (
     APP_PARAMETER,
     EXCLUDED_DIRECTIVES,
     HELP_PARAMETER,
@@ -19,40 +20,41 @@
     list,
     run,
     runserver,
     show_urls,
 )
 from esmerald.core.directives.operations._constants import ESMERALD_SETTINGS_MODULE
 from esmerald.core.terminal.print import Print
-from esmerald.exceptions import EnvironmentError
+
+T = TypeVar("T")
 
 printer = Print()
 
 
 class DirectiveGroup(click.Group):
     """Custom directive group to handle with the context and directives commands"""
 
     def add_command(self, cmd: click.Command, name: typing.Optional[str] = None) -> None:
         if cmd.callback:
             cmd.callback = self.wrap_args(cmd.callback)
         return super().add_command(cmd, name)
 
-    def wrap_args(self, func: typing.Any) -> typing.Any:
+    def wrap_args(self, func: Callable[..., T]) -> Callable[..., T]:
         params = inspect.signature(func).parameters
 
         @wraps(func)
-        def wrapped(ctx: click.Context, /, *args: typing, **kwargs: typing) -> typing:
+        def wrapped(ctx: click.Context, /, *args: typing.Any, **kwargs: typing.Any) -> T:
             scaffold = ctx.ensure_object(DirectiveEnv)
             if "env" in params:
                 kwargs["env"] = scaffold
             return func(*args, **kwargs)
 
         return click.pass_context(wrapped)
 
-    def process_settings(self, ctx: click.Context):
+    def process_settings(self, ctx: click.Context) -> None:
         """
         Process the settings context" if any is passed.
 
         Exports any ESMERALD_SETTINGS_MODULE to the environment if --settings is passed and exists
         as one of the params of any subcommand.
         """
         args = [*ctx.protected_args, *ctx.args]
@@ -77,15 +79,15 @@
         if HELP_PARAMETER not in sys.argv and not any(
             value in sys.argv for value in EXCLUDED_DIRECTIVES
         ):
             try:
                 directive = DirectiveEnv()
                 app_env = directive.load_from_env(path=path)
                 ctx.obj = app_env
-            except EnvironmentError as e:
+            except OSError as e:
                 if not any(value in sys.argv for value in IGNORE_DIRECTIVES):
                     printer.write_error(str(e))
                     sys.exit(1)
         return super().invoke(ctx)
 
 
 @click.group(
```

### Comparing `esmerald-1.2.5/esmerald/core/directives/env.py` & `esmerald-1.3.0/esmerald/core/directives/env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import os
 import sys
 import typing
 from dataclasses import dataclass
 from importlib import import_module
 from pathlib import Path
 
-from esmerald import Esmerald
+from esmerald import ChildEsmerald, Esmerald
 from esmerald.core.directives.constants import (
     DISCOVERY_FILES,
     DISCOVERY_FUNCTIONS,
     ESMERALD_DISCOVER_APP,
 )
 from esmerald.core.terminal import Print
-from esmerald.exceptions import EnvironmentError
 
 printer = Print()
 
 
 @dataclass
 class Scaffold:
     """
     Simple Application scaffold that holds the
     information about the app and the path to
     the same app.
     """
 
     path: str
-    app: typing.Any
+    app: typing.Union[Esmerald, ChildEsmerald]
 
 
 @dataclass
 class DirectiveEnv:
     """
     Loads an arbitraty application into the object
     and returns the App.
     """
 
     path: typing.Optional[str] = None
-    app: typing.Optional[typing.Any] = None
+    app: typing.Optional[typing.Union[Esmerald, ChildEsmerald]] = None
     command_path: typing.Optional[str] = None
 
     def load_from_env(self, path: typing.Optional[str] = None) -> "DirectiveEnv":
         """
         Loads the environment variables into the scaffold.
         """
         # Adds the current path where the command is being invoked
@@ -60,31 +59,29 @@
         _path = os.getenv(ESMERALD_DISCOVER_APP) if not path else path
         _app = self.find_app(path=_path, cwd=cwd)
 
         return DirectiveEnv(path=_app.path, app=_app.app, command_path=command_path)
 
     def import_app_from_string(cls, path: typing.Optional[str] = None) -> Scaffold:
         if path is None:
-            raise EnvironmentError(
-                detail="Path cannot be None. Set env `ESMERALD_DEFAULT_APP` or use `--app` instead."
+            raise OSError(
+                "Path cannot be None. Set env `ESMERALD_DEFAULT_APP` or use `--app` instead."
             )
         module_str_path, app_name = path.split(":")
         module = import_module(module_str_path)
         app = getattr(module, app_name)
         return Scaffold(path=path, app=app)
 
     def _get_folders(self, path: Path) -> typing.List[str]:
         """
         Lists all the folders and checks if there is any file from the DISCOVERY_FILES available
         """
         return [directory.path for directory in os.scandir(path) if directory.is_dir()]
 
-    def _find_app_in_folder(
-        self, path: Path, cwd: Path
-    ) -> typing.Union[typing.NoReturn, typing.Callable[..., typing.Any]]:
+    def _find_app_in_folder(self, path: Path, cwd: Path) -> typing.Union[Scaffold, None]:
         """
         Iterates inside the folder and looks up to the DISCOVERY_FILES.
         """
         for discovery_file in DISCOVERY_FILES:
             filename = f"{str(path)}/{discovery_file}"
             if not os.path.exists(filename):
                 continue
@@ -103,26 +100,27 @@
 
             # Iterate over default pattern application functions
             for func in DISCOVERY_FUNCTIONS:
                 if hasattr(module, func):
                     app_path = f"{dotted_path}:{func}"
                     fn = getattr(module, func)
                     return Scaffold(app=fn(), path=app_path)
+        return None
 
     def find_app(self, path: typing.Optional[str], cwd: Path) -> Scaffold:
         """
         Loads the application based on the path provided via env var.
 
         If no --app is provided, goes into auto discovery up to one level.
         """
 
         if path:
             return self.import_app_from_string(path)
 
-        scaffold: Scaffold = None
+        scaffold: typing.Union[Scaffold, None] = None
 
         # Check current folder
         scaffold = self._find_app_in_folder(cwd, cwd)
         if scaffold:
             return scaffold
 
         # Goes into auto discovery mode for one level, only.
@@ -133,10 +131,10 @@
             scaffold = self._find_app_in_folder(folder_path, cwd)
 
             if not scaffold:
                 continue
             break
 
         if not scaffold:
-            raise EnvironmentError(detail="Could not find an Esmerald application.")
+            raise OSError("Could not find an Esmerald application.")
 
         return scaffold
```

### Comparing `esmerald-1.2.5/esmerald/core/directives/templates.py` & `esmerald-1.3.0/esmerald/core/directives/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 import stat
 from importlib import import_module
 from pathlib import Path
-from typing import Any, Dict, Union
+from typing import Any, Dict, Optional, Union
 
 from jinja2 import Environment, FileSystemLoader
 
 import esmerald
 from esmerald.core.directives.base import BaseDirective
 from esmerald.core.directives.exceptions import DirectiveError
 from esmerald.core.terminal import Print
@@ -28,26 +28,25 @@
         (".e-tpl", ""),
     )
 
     def handle(self, app_or_project: str, name: str, **options: Any) -> Any:
         self.app_or_project = app_or_project
         self.name = name
         self.a_or_an = "an" if app_or_project == "app" else "a"
-        self.paths_to_remove = []
         self.verbosity = options["verbosity"]
 
         self.validate_name(name)
 
         top_dir = os.path.join(os.getcwd(), name)
         try:
             os.makedirs(top_dir)
         except FileExistsError:
             raise DirectiveError(f"{top_dir} already exists.") from None
         except OSError as e:
-            raise DirectiveError(e) from e
+            raise DirectiveError(detail=str(e)) from e
 
         base_name = f"{app_or_project}_name"
         base_subdir = f"{app_or_project}_template"
 
         context = {
             base_name: name,
             "esmerald_version": self.get_version(),
@@ -109,28 +108,28 @@
 
     def manage_template_variables(
         self,
         template: Union[str, Path],
         destination: Union[str, Path],
         template_dir: Union[str, Path],
         context: Dict[str, Any],
-    ):
+    ) -> None:
         """
         Goes through every file generated and replaces the variables with the given
         context variables.
         """
         environment = Environment(loader=FileSystemLoader(template_dir), autoescape=True)
-        template = environment.get_template(template)
-        rendered_template = template.render(context)
+        template = environment.get_template(template)  # type: ignore
+        rendered_template = template.render(context)  # type: ignore
         if os.path.isfile(destination):
             os.unlink(destination)
         with open(destination, "w") as f:
             f.write(rendered_template)
 
-    def validate_name(self, name, name_or_dir="name"):
+    def validate_name(self, name: Optional[str], name_or_dir: str = "name") -> None:
         if name is None:
             raise DirectiveError(
                 "you must provide {an} {app} name".format(
                     an=self.a_or_an,
                     app=self.app_or_project,
                 )
             )
@@ -156,21 +155,21 @@
                     name=name,
                     an=self.a_or_an,
                     app=self.app_or_project,
                     type=name_or_dir,
                 )
             )
 
-    def apply_umask(self, old_path: Union[str, Path], new_path: Union[str, Path]):
+    def apply_umask(self, old_path: Union[str, Path], new_path: Union[str, Path]) -> None:
         current_umask = os.umask(0)
         os.umask(current_umask)
         current_mode = stat.S_IMODE(os.stat(old_path).st_mode)
         os.chmod(new_path, current_mode & ~current_umask)
 
-    def make_file_writable(self, filename: str):
+    def make_file_writable(self, filename: str) -> None:
         """
         Make sure that the file is writeable.
         Useful if our source is read-only.
         """
         if not os.access(filename, os.W_OK):
             st = os.stat(filename)
             new_permissions = stat.S_IMODE(st.st_mode) | stat.S_IWUSR
```

### Comparing `esmerald-1.2.5/esmerald/core/directives/utils.py` & `esmerald-1.3.0/esmerald/core/directives/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import importlib
 import os
 import pkgutil
 import sys
 import typing
 from difflib import get_close_matches
 from importlib import import_module
-from typing import Any
+from typing import Any, Optional
 
 from esmerald.core.directives.base import BaseDirective
 from esmerald.core.directives.exceptions import DirectiveError
 from esmerald.core.terminal import Print
 
 printer = Print()
 
@@ -32,28 +32,30 @@
     for _, name, is_package in pkgutil.iter_modules([directive_dir]):
         if not is_package and not name.startswith("_"):
             if name not in EXCUDED_DIRECTIVES:
                 directive_list.append(name)
     return directive_list
 
 
-def find_application_directives(management_dir: str) -> typing.List[str]:
+def find_application_directives(
+    management_dir: str,
+) -> typing.Sequence[typing.Union[typing.Dict[Any, Any], str]]:
     """
     Iterates through the application tree and finds the directives available
     to run.
     """
     directive_list = []
     for root, folders, _ in os.walk(management_dir):
         if OPERATIONS not in folders:
             continue
 
         directive_dir = os.path.join(root, "operations")
         for location, name, is_package in pkgutil.iter_modules([directive_dir]):
             if not is_package and not name.startswith("_"):
-                directive_list.append({"name": name, "location": location.path})
+                directive_list.append({"name": name, "location": location.path})  # type: ignore
     return directive_list
 
 
 def load_directive_class(app_name: str, name: str) -> Any:
     """
     Loads the directive class from native Esmerald.
     """
@@ -74,34 +76,38 @@
         sys.exit(1)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     return module.Directive()
 
 
 @functools.lru_cache(maxsize=None)
-def get_directives(location: str) -> typing.List[str]:
+def get_directives(location: str) -> typing.Sequence[typing.Union[typing.Dict[Any, Any], str]]:
     command_list = find_directives(location)
     directives = []
 
     for name in command_list:
         directives.append({name: "esmerald.core", "location": None})
     return directives
 
 
 @functools.lru_cache(maxsize=None)
-def get_application_directives(location: str) -> typing.List[str]:
+def get_application_directives(
+    location: str,
+) -> typing.Sequence[typing.Dict[Any, Any]]:
     command_list = find_application_directives(location)
     directives = []
 
     for value in command_list:
-        directives.append({value["name"]: "application", "location": value["location"]})
+        directives.append(
+            {value["name"]: "application", "location": value["location"]}  # type: ignore
+        )
     return directives
 
 
-def fetch_custom_directive(subdirective: Any, location: str) -> Any:
+def fetch_custom_directive(subdirective: Any, location: Optional[str]) -> Any:
     """Fetches the directive classes custom and native"""
     directives = get_application_directives(location)
 
     counter = 0
     matches = []
     app_name = None
 
@@ -137,15 +143,15 @@
     klass = load_directive_class_by_filename(app_name, name)
 
     if not isinstance(klass, BaseDirective):
         raise DirectiveError(detail="The directive must be a subclass of BaseDirective")
     return klass
 
 
-def fetch_directive(subdirective: Any, location: str, is_custom: bool = False) -> Any:
+def fetch_directive(subdirective: Any, location: Optional[str], is_custom: bool = False) -> Any:
     """Fetches the directive classes custom and native"""
     if not is_custom:
         directives = get_directives(location)
     else:
         return fetch_custom_directive(subdirective, location)
 
     counter = 0
@@ -153,15 +159,15 @@
 
     for directive in directives:
         try:
             app_name = directive[subdirective]
         except KeyError:
             counter += 1
 
-            directive = {k: v for k, v in directive.items() if k != "location"}
+            directive = {k: v for k, v in directive.items() if k != "location"}  # type: ignore
             matches.extend(get_close_matches(subdirective, directive))
 
             if matches and len(directives) == counter:
                 printer.write_error("Did you mean %s?" % matches[0])
 
             if len(directives) == counter:
                 return None
```

### Comparing `esmerald-1.2.5/esmerald/core/directives/operations/createapp.py` & `esmerald-1.3.0/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/core/directives/operations/createproject.py` & `esmerald-1.3.0/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/core/directives/operations/list.py` & `esmerald-1.3.0/esmerald/core/directives/operations/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     if getattr(env, "app", None) is not None:
         app_directives = get_application_directives(env.command_path)
         if app_directives:
             directives.extend(app_directives)
 
     directives_dict = defaultdict(lambda: [])
     for directive in directives:
-        for name, app in directive.items():
+        for name, app in directive.items():  # type: ignore
             if name == "location":
                 continue
 
             if app == "esmerald.core":
                 app = "esmerald"
             else:
                 app = app.rpartition(".")[-1]
```

### Comparing `esmerald-1.2.5/esmerald/core/directives/operations/run.py` & `esmerald-1.3.0/esmerald/core/directives/operations/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import os
 import sys
 from enum import Enum
-from typing import Any
+from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union
 
 import click
 from starlette.types import Lifespan
 
 from esmerald.core.directives.constants import APP_PARAMETER, ESMERALD_DISCOVER_APP
 from esmerald.core.directives.env import DirectiveEnv
 from esmerald.core.directives.utils import fetch_directive
 from esmerald.core.terminal.print import Print
 from esmerald.routing.events import generate_lifespan_events
 from esmerald.utils.sync import execsync
 
+if TYPE_CHECKING:
+    from esmerald.applications import ChildEsmerald, Esmerald
+
+T = TypeVar("T")
+
 printer = Print()
 
 
 class Position(int, Enum):
     DEFAULT = 5
     BACK = 3
 
@@ -61,30 +66,34 @@
     # The arguments for the directives start at the position 6
     position = get_position()
     program_name = " ".join(value for value in sys.argv[:position])
 
     ## Check if application is up and execute any event
     # Shutting down after
     lifespan = generate_lifespan_events(env.app.on_startup, env.app.on_shutdown, env.app.lifespan)
-    execsync(execute_lifespan)(env.app, lifespan, directive, program_name, position)
+    execsync(execute_lifespan)(env.app, lifespan, directive, program_name, position)  # type: ignore
 
 
-def get_position():
+def get_position() -> int:
     """
     Gets the position of the arguments to read and pass them
     onto the directive.
     """
     if os.getenv(ESMERALD_DISCOVER_APP) is None and APP_PARAMETER in sys.argv:
         return Position.DEFAULT
     elif os.getenv(ESMERALD_DISCOVER_APP) is not None and APP_PARAMETER in sys.argv:
         return Position.DEFAULT
     return Position.BACK
 
 
 async def execute_lifespan(
-    app, lifespan: Lifespan, directive: Any, program_name: str, position: int
-):
+    app: Optional[Union["Esmerald", "ChildEsmerald"]],
+    lifespan: Lifespan,
+    directive: Any,
+    program_name: str,
+    position: int,
+) -> None:
     """
     Executes the lifespan events and the directive.
     """
     async with lifespan(app):
         await directive.execute_from_command(sys.argv[:], program_name, position)
```

### Comparing `esmerald-1.2.5/esmerald/core/directives/operations/runserver.py` & `esmerald-1.3.0/esmerald/core/directives/operations/runserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import sys
+from typing import TYPE_CHECKING
 
 import click
 
 from esmerald.core.directives.env import DirectiveEnv
 from esmerald.core.directives.exceptions import DirectiveError
 from esmerald.core.terminal import OutputColour, Print, Terminal
 
+if TYPE_CHECKING:
+    pass
+
 printer = Print()
 terminal = Terminal()
 
 
 @click.option(
     "-p",
     "--port",
@@ -52,30 +56,23 @@
 @click.option(
     "--lifespan",
     type=str,
     default="on",
     help="Enable lifespan events.",
     show_default=True,
 )
-@click.option(
-    "--settings",
-    type=str,
-    help="Start the server with specific settings.",
-    required=False,
-)
 @click.command(name="runserver")
 def runserver(
     env: DirectiveEnv,
     port: int,
     reload: bool,
     host: str,
     debug: bool,
     log_level: str,
     lifespan: str,
-    settings: str,
 ) -> None:
     """Starts the Esmerald development server.
 
     The --app can be passed in the form of <module>.<submodule>:<app> or be set
     as environment variable ESMERALD_DEFAULT_APP.
 
     Alternatively, if none is passed, Esmerald will perform the application discovery.
@@ -94,23 +91,25 @@
         sys.exit(1)
 
     try:
         import uvicorn
     except ImportError:
         raise DirectiveError(detail="Uvicorn needs to be installed to run Esmerald.") from None
 
+    app = env.app
+    settings = app.settings
     message = terminal.write_info(
-        f"Starting {env.app.settings.environment} server @ {host}", colour=OutputColour.BRIGHT_CYAN
+        f"Starting {settings.environment} server @ {host}", colour=OutputColour.BRIGHT_CYAN
     )
     terminal.rule(message, align="center")
 
     if debug:
-        env.app.debug = debug
+        app.debug = debug
 
     uvicorn.run(
         app=env.path,
         port=port,
         host=host,
         reload=reload,
-        lifespan=lifespan,
+        lifespan=lifespan,  # type: ignore
         log_level=log_level,
     )
```

### Comparing `esmerald-1.2.5/esmerald/core/directives/operations/show_urls.py` & `esmerald-1.3.0/esmerald/core/directives/operations/show_urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import inspect
 import os
 import sys
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 import click
 from rich.console import Console
 from rich.table import Table
 
-from esmerald import Gateway
+from esmerald import APIView, Gateway
 from esmerald.core.directives.constants import ESMERALD_DISCOVER_APP
 from esmerald.core.directives.env import DirectiveEnv
 from esmerald.core.terminal import OutputColour, Print, Terminal
 from esmerald.enums import HttpMethod
 from esmerald.utils.url import clean_path
 
+if TYPE_CHECKING:
+    from starlette.routing import BaseRoute
+
+    from esmerald.applications import ChildEsmerald, Esmerald
+    from esmerald.routing.router import Router
+
 printer = Print()
 writer = Terminal()
 console = Console()
 
 DOCS_ELEMENTS = [
     "/swagger",
     "/redoc",
@@ -37,14 +43,15 @@
         return HttpMethod.PUT.value
     elif getattr(mapping, "patch", None):
         return HttpMethod.PATCH.value
     elif getattr(mapping, "delete", None):
         return HttpMethod.DELETE.value
     elif getattr(mapping, "header", None):
         return HttpMethod.HEAD.value
+    return HttpMethod.GET.value
 
 
 @click.command(name="show_urls")
 def show_urls(env: DirectiveEnv) -> None:
     """Shows the information regarding the urls of a given application
 
     How to run: `esmerald show_urls`
@@ -61,51 +68,57 @@
 
     app = env.app
     table = Table(title=app.app_name)
     table = get_routes_table(app, table)
     printer.write(table)
 
 
-def get_routes_table(app, table: Table) -> None:
+def get_routes_table(app: Optional[Union["Esmerald", "ChildEsmerald"]], table: Table) -> Table:
     """Prints the routing system"""
-    table.add_column("Path", style=OutputColour.GREEN, vertical="center")
-    table.add_column("Path Parameters", style=OutputColour.BRIGHT_CYAN, vertical="center")
-    table.add_column("Name", style=OutputColour.CYAN, vertical="center")
-    table.add_column("Type", style=OutputColour.YELLOW, vertical="center")
-    table.add_column("HTTP Methods", style=OutputColour.RED, vertical="center")
-
-    def parse_routes(app, table: table, route: Optional[Any] = None, prefix: Optional[str] = ""):
+    table.add_column("Path", style=OutputColour.GREEN, vertical="middle")
+    table.add_column("Path Parameters", style=OutputColour.BRIGHT_CYAN, vertical="middle")
+    table.add_column("Name", style=OutputColour.CYAN, vertical="middle")
+    table.add_column("Type", style=OutputColour.YELLOW, vertical="middle")
+    table.add_column("HTTP Methods", style=OutputColour.RED, vertical="middle")
+
+    def parse_routes(
+        app: Optional[Union["Esmerald", "ChildEsmerald", "Router", "BaseRoute"]],
+        table: Table,
+        route: Optional[Any] = None,
+        prefix: Optional[str] = "",
+    ) -> None:
         if getattr(app, "routes", None) is None:
             return
 
-        for route in app.routes:
+        for route in app.routes:  # type: ignore
             if isinstance(route, Gateway):
                 # Path
                 path = clean_path(prefix + route.path)
 
                 if any(element in path for element in DOCS_ELEMENTS):
                     continue
 
                 # Type
-                if inspect.iscoroutinefunction(route.handler.fn):
-                    fn_type = "async"
-                else:
-                    fn_type = "sync"
+                if not isinstance(route.handler, APIView):
+                    if inspect.iscoroutinefunction(route.handler.fn):
+                        fn_type = "async"
+                    else:
+                        fn_type = "sync"
 
                 # Http methods
                 http_methods = ", ".join(sorted(route.methods))
                 parameters = ", ".join(sorted(route.stringify_parameters))
                 table.add_row(path, parameters, route.name, fn_type, http_methods)
                 continue
 
             route_app = getattr(route, "app", None)
             if not route_app:
                 continue
 
-            path = clean_path(prefix + route.path)
+            path = clean_path(prefix + route.path)  # type: ignore
             if any(element in path for element in DOCS_ELEMENTS):
                 continue
 
             parse_routes(route, table, prefix=f"{path}")
 
     parse_routes(app, table)
     return table
```

### Comparing `esmerald-1.2.5/esmerald/core/terminal/base.py` & `esmerald-1.3.0/esmerald/core/terminal/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Any
+from typing import Any, Union
 
 from rich.console import Console
 
 console = Console()
 
 
 class OutputColour(str, Enum):
@@ -244,43 +244,43 @@
     GREY85 = "grey85"
     GRAY85 = "gray85"
     GREY89 = "grey89"
     GRAY89 = "gray89"
     GREY93 = "grey93"
     GRAY93 = "gray93"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.value
 
     def __repr__(self) -> str:
         return str(self)
 
 
 class Base(ABC, Console):
     """Base output class for the terminal"""
 
     @abstractmethod
-    def write_success(self, message: str, colour: str = OutputColour.SUCCESS) -> None:
+    def write_success(self, message: str, colour: str = OutputColour.SUCCESS) -> Union[str, None]:
         raise NotImplementedError()
 
     @abstractmethod
-    def write_info(self, message: str, colour: str = OutputColour.INFO) -> None:
+    def write_info(self, message: str, colour: str = OutputColour.INFO) -> Union[str, None]:
         """Outputs the info to the console"""
         raise NotImplementedError()
 
     @abstractmethod
-    def write_warning(self, message: str, colour: str = OutputColour.WARNING) -> None:
+    def write_warning(self, message: str, colour: str = OutputColour.WARNING) -> Union[str, None]:
         """Outputs the warnings to the console"""
 
     @abstractmethod
-    def write_error(self, message: str, colour: str = OutputColour.ERROR) -> None:
+    def write_error(self, message: str, colour: str = OutputColour.ERROR) -> Union[str, None]:
         """Outputs the errors to the console"""
         raise NotImplementedError()
 
-    def write_plain(self, message: str, colour: str = OutputColour.WHITE) -> None:
+    def write_plain(self, message: str, colour: str = OutputColour.WHITE) -> Union[str, None]:
         """Outputs the custom plain"""
         raise NotImplementedError()
 
     def write(self, message: Any) -> None:
         self.print(message)
 
     def message(self, message: str, colour: str) -> str:
```

### Comparing `esmerald-1.2.5/esmerald/core/terminal/print.py` & `esmerald-1.3.0/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/core/terminal/terminal.py` & `esmerald-1.3.0/esmerald/core/terminal/terminal.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 class Terminal(Base):
     """Base output class for the terminal"""
 
     def write_success(
         self,
         message: str,
         colour: str = OutputColour.SUCCESS,
-    ) -> None:
+    ) -> str:
         """Outputs the successes to the console"""
         message = self.message(message, colour)
         return message
 
     def write_info(
         self,
         message: str,
         colour: str = OutputColour.INFO,
-    ) -> None:
+    ) -> str:
         """Outputs the info to the console"""
         message = self.message(message, colour)
         return message
 
     def write_warning(
         self,
         message: str,
         colour: str = OutputColour.WARNING,
-    ) -> None:
+    ) -> str:
         """Outputs the warnings to the console"""
         message = self.message(message, colour)
         return message
 
     def write_error(
         self,
         message: str,
         colour: str = OutputColour.ERROR,
-    ) -> None:
+    ) -> str:
         """Outputs the errors to the console"""
         message = self.message(message, colour)
         return message
 
-    def write_plain(self, message: str, colour: str = OutputColour.WHITE) -> None:
+    def write_plain(self, message: str, colour: str = OutputColour.WHITE) -> str:
         message = self.message(message, colour)
         return message
```

### Comparing `esmerald-1.2.5/esmerald/datastructures/__init__.py` & `esmerald-1.3.0/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/datastructures/base.py` & `esmerald-1.3.0/esmerald/datastructures/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from copy import copy
 from http.cookies import SimpleCookie
-from typing import TYPE_CHECKING, Any, Dict, Generic, List, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, Generic, List, Optional, Type, TypeVar, Union
 
 from pydantic import BaseConfig, BaseModel, validator  # noqa
 from pydantic.generics import GenericModel  # noqa
 from starlette.datastructures import URL as URL  # noqa: F401
 from starlette.datastructures import Address as Address  # noqa: F401
 from starlette.datastructures import FormData as FormData  # noqa: F401
 from starlette.datastructures import Headers as Headers  # noqa: F401
@@ -46,15 +46,15 @@
 
 class State(StarletteStateClass):
     state: Dict[str, Any]
 
     def __copy__(self) -> "State":
         return self.__class__(copy(self._state))
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._state)
 
     def __getattr__(self, key: str) -> Any:
         try:
             return self._state[key]
         except KeyError as e:
             raise AttributeError(f"State has no key '{key}'") from e
@@ -100,15 +100,15 @@
 
     @abstractmethod
     def to_response(
         self,
         headers: Dict[str, Any],
         media_type: Union["MediaType", str],
         status_code: int,
-        app: "Esmerald",
+        app: Type["Esmerald"],
     ) -> R:  # pragma: no cover
         raise NotImplementedError("not implemented")
 
 
 class ResponseHeader(BaseModel):
     value: Any = None
```

### Comparing `esmerald-1.2.5/esmerald/datastructures/encoders.py` & `esmerald-1.3.0/esmerald/datastructures/encoders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import TYPE_CHECKING, Any, Dict, Optional, Type, Union
 
-from esmerald.datastructures.base import ResponseContainer  # noqa
+from esmerald.datastructures.base import ResponseContainer
 
 if TYPE_CHECKING:
     from esmerald.applications import Esmerald
     from esmerald.enums import MediaType
 
 try:
     from esmerald.responses.encoders import ORJSONResponse
 except ImportError:
-    ORJSONResponse = None
+    ORJSONResponse = None  # type: ignore
 
 try:
     from esmerald.responses.encoders import UJSONResponse
 except ImportError:
-    UJSONResponse = None
+    UJSONResponse = None  # type: ignore
 
 
 class OrJSON(ResponseContainer[ORJSONResponse]):
     content: Optional[Dict[str, Any]] = None
     status_code: Optional[int] = None
 
     def __init__(
         self,
         content: Optional[Dict[str, Any]] = None,
         status_code: Optional[int] = None,
-        **kwargs: Dict[str, Any],
-    ):
+        **kwargs: Any,
+    ) -> None:
         super().__init__(**kwargs)
         self.content = content
         self.status_code = status_code
 
     def to_response(
         self,
         headers: Dict[str, Any],
@@ -56,16 +56,16 @@
     content: Optional[Dict[str, Any]] = None
     status_code: Optional[int] = None
 
     def __init__(
         self,
         content: Optional[Dict[str, Any]] = None,
         status_code: Optional[int] = None,
-        **kwargs: Dict[str, Any],
-    ):
+        **kwargs: Any,
+    ) -> None:
         super().__init__(**kwargs)
         self.content = content
         self.status_code = status_code
 
     def to_response(
         self,
         headers: Dict[str, Any],
```

### Comparing `esmerald-1.2.5/esmerald/datastructures/file.py` & `esmerald-1.3.0/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/datastructures/json.py` & `esmerald-1.3.0/esmerald/datastructures/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     content: Optional[Dict[str, Any]] = None
     status_code: Optional[int] = None
 
     def __init__(
         self,
         content: Optional[Dict[str, Any]] = None,
         status_code: Optional[int] = None,
-        **kwargs: Dict[str, Any],
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.content = content
         self.status_code = status_code
 
     def to_response(
         self,
```

### Comparing `esmerald-1.2.5/esmerald/datastructures/redirect.py` & `esmerald-1.3.0/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/datastructures/stream.py` & `esmerald-1.3.0/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/datastructures/template.py` & `esmerald-1.3.0/esmerald/datastructures/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ) -> "TemplateResponse":
         from esmerald.exceptions import ImproperlyConfigured
         from esmerald.responses import TemplateResponse
 
         if not app.template_engine:
             raise ImproperlyConfigured("Template engine is not configured")
 
-        data = {
+        data: Dict[str, Any] = {
             "background": self.background,
             "context": self.context,
             "headers": headers,
             "status_code": status_code,
             "template_engine": app.template_engine,
             "media_type": media_type,
         }
```

### Comparing `esmerald-1.2.5/esmerald/interceptors/interceptor.py` & `esmerald-1.3.0/esmerald/interceptors/interceptor.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 
 
 class EsmeraldInterceptor(ABC, InterceptorProtocol):
     """Base class for any Esmerald interceptor in the system."""
 
     async def intercept(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
         """
-        The abstract method that needs to be implemented for any interceptor.
+        The method that needs to be implemented for any interceptor.
         """
         raise NotImplementedError("intercept must be implemented")
```

### Comparing `esmerald-1.2.5/esmerald/middleware/__init__.py` & `esmerald-1.3.0/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/middleware/_exception_handlers.py` & `esmerald-1.3.0/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/middleware/asyncexitstack.py` & `esmerald-1.3.0/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/middleware/authentication.py` & `esmerald-1.3.0/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/middleware/basic.py` & `esmerald-1.3.0/esmerald/middleware/basic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from typing import TypeVar
+
 from starlette.middleware.base import BaseHTTPMiddleware  # noqa
 from starlette.middleware.base import RequestResponseEndpoint as RequestResponseEndpoint  # noqa
+from starlette.requests import Request as StarletteRequest
+from starlette.responses import Response
 
 from esmerald.requests import Request
-from esmerald.responses import Response
+
+Req = TypeVar("Req", Request, StarletteRequest)
 
 
 class BasicHTTPMiddleware(BaseHTTPMiddleware):
     """
     BaseHTTPMiddleware of all Esmerald applications.
     """
 
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
+    async def dispatch(self, request: Req, call_next: RequestResponseEndpoint) -> Response:
         response = await call_next(request)
         return response
```

### Comparing `esmerald-1.2.5/esmerald/middleware/csrf.py` & `esmerald-1.3.0/esmerald/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/middleware/errors.py` & `esmerald-1.3.0/esmerald/middleware/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import traceback
+from typing import TypeVar
 
 from starlette.middleware.errors import ServerErrorMiddleware as StarletteServerErrorMiddleware
+from starlette.requests import Request as StarletteRequest
 from starlette.responses import HTMLResponse, PlainTextResponse, Response
 
-from esmerald.requests import Request
+from esmerald.requests import Request as _Request
+
+Request = TypeVar("Request", _Request, StarletteRequest)
 
 
 class ServerErrorMiddleware(StarletteServerErrorMiddleware):
     """
     Handles returning 500 responses when a server error occurs.
 
     If 'debug' is set, then traceback responses will be returned,
```

### Comparing `esmerald-1.2.5/esmerald/middleware/exceptions.py` & `esmerald-1.3.0/esmerald/middleware/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from esmerald.enums import MediaType, ScopeType
 from esmerald.exception_handlers import http_exception_handler
 from esmerald.exceptions import HTTPException, WebSocketException
 from esmerald.middleware._exception_handlers import wrap_app_handling_exceptions
 from esmerald.requests import Request
 from esmerald.responses import Response
-from esmerald.types import ExceptionHandler, ExceptionHandlers
+from esmerald.types import ExceptionHandler, ExceptionHandlerMap
 from esmerald.websockets import WebSocket
 
 
 class ExceptionMiddleware(StarletteExceptionMiddleware):
     """
     Reimplementation of the Exception Middleware.
     """
@@ -36,15 +36,15 @@
         self._exception_handlers: Dict[Type[Exception], Callable] = {
             HTTPException: http_exception_handler,
             StarletteHTTPException: http_exception_handler,
             WebSocketException: self.websocket_exception,
         }
         if handlers is not None:
             for key, value in handlers.items():
-                self.add_exception_handler(key, value)
+                self.add_exception_handler(key, value)  # type: ignore
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         if scope["type"] not in ("http", "websocket"):
             await self.app(scope, receive, send)
             return
 
         scope["starlette.exception_handlers"] = (
@@ -69,15 +69,15 @@
 
 
 class EsmeraldAPIExceptionMiddleware:
     def __init__(
         self,
         app: "ASGIApp",
         debug: bool,
-        exception_handlers: "ExceptionHandlers",
+        exception_handlers: "ExceptionHandlerMap",
         error_handler: Optional[Callable] = None,
     ) -> None:
         self.app = app
         self.exception_handlers = exception_handlers
         self.debug = debug
         self.error_handler = error_handler
 
@@ -113,16 +113,16 @@
         """Default handler for exceptions subclassed from HTTPException."""
         status_code = (
             exc.status_code
             if isinstance(exc, StarletteHTTPException)
             else status.HTTP_500_INTERNAL_SERVER_ERROR
         )
         if status_code == status.HTTP_500_INTERNAL_SERVER_ERROR and self.debug:
-            server_error = ServerErrorMiddleware(app=self.app, handler=self.error_handler)  # type: ignore[arg-type]
-            return server_error.debug_response(request=request, exc=exc)  # type: ignore[arg-type]
+            server_error = ServerErrorMiddleware(app=self.app, handler=self.error_handler)
+            return server_error.debug_response(request=request, exc=exc)
         return self.create_exception_response(exc)
 
     def create_exception_response(self, exc: Exception) -> Response:
         if isinstance(exc, (HTTPException, StarletteHTTPException)):
             content = ResponseContent(detail=exc.detail, status_code=exc.status_code)
             if isinstance(exc, HTTPException):
                 extra = exc.extra.get("extra", {})
@@ -137,17 +137,17 @@
             headers=exc.headers
             if isinstance(exc, (HTTPException, StarletteHTTPException))
             else None,
         )
 
     def get_exception_handler(
         self,
-        exception_handlers: Dict[Union[int, Type[Exception]], "ExceptionHandlers"],
+        exception_handlers: ExceptionHandlerMap,
         exc: Exception,
-    ) -> Optional[ExceptionHandler]:
+    ) -> Union[ExceptionHandler, None]:
         if not exception_handlers:
             return None
 
         if not isinstance(exc, HTTPException) and exc.__class__ in exception_handlers:
             return exception_handlers[exc.__class__]
 
         if isinstance(exc, HTTPException) and exc.__class__ in exception_handlers:
```

### Comparing `esmerald-1.2.5/esmerald/middleware/settings_middleware.py` & `esmerald-1.3.0/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/openapi/apiview.py` & `esmerald-1.3.0/esmerald/openapi/apiview.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/openapi/enums.py` & `esmerald-1.3.0/esmerald/openapi/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/openapi/parameters.py` & `esmerald-1.3.0/esmerald/openapi/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     else:
         param_in = ParamType.QUERY
         parameter_name = extra.get(ParamType.QUERY) or parameter_name
 
     if not schema:
         schema = create_schema(field=model_field, create_examples=create_examples)
 
-    return Parameter(
+    return Parameter(  # type: ignore[call-arg]
         name=parameter_name,
         param_in=param_in,
         required=is_required,
         param_schema=schema,
         description=schema.description,
     )
 
@@ -94,15 +94,15 @@
 def get_recursive_handler_parameters(
     field_name: str,
     model_field: "ModelField",
     dependencies: "Dependencies",
     handler: "HTTPHandler",
     path_parameters: Any,
     create_examples: bool,
-):
+) -> List[Parameter]:
     if field_name not in dependencies:
         return [
             create_parameter(
                 model_field=model_field,
                 parameter_name=field_name,
                 path_paramaters=path_parameters,
                 create_examples=create_examples,
@@ -116,16 +116,16 @@
 
 
 def create_parameter_for_handler(
     handler: "HTTPHandler",
     handler_fields: Dict[str, "ModelField"],
     path_parameters: Any,
     create_examples: bool,
-):
-    parameters = ParameterCollection(handler=handler)
+) -> List[Parameter]:
+    parameters = ParameterCollection(handler=cast("Type[HTTPHandler]", handler))
     dependencies = handler.get_dependencies()
 
     filtered = [
         item
         for item in handler_fields.items()
         if item[0] not in RESERVED_KWARGS and item[0] not in {}
     ]
```

### Comparing `esmerald-1.2.5/esmerald/openapi/path_item.py` & `esmerald-1.3.0/esmerald/openapi/path_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, cast
+from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Union, cast
 
 from openapi_schemas_pydantic.v3_1_0.operation import Operation
+from openapi_schemas_pydantic.v3_1_0.parameter import Parameter
 from openapi_schemas_pydantic.v3_1_0.path_item import PathItem
+from openapi_schemas_pydantic.v3_1_0.reference import Reference
 from starlette.routing import get_name
 
 from esmerald.enums import HttpMethod
 from esmerald.openapi.parameters import create_parameter_for_handler
 from esmerald.openapi.request_body import create_request_body
 from esmerald.openapi.responses import create_responses
 
 if TYPE_CHECKING:
     from openapi_schemas_pydantic.v3_1_0 import SecurityRequirement
     from pydantic import BaseModel
+    from pydantic.typing import AnyCallable
 
     from esmerald.routing.handlers import HTTPHandler
-    from esmerald.types import AnyCallable
+
+
+OptionalRef = Optional[List[Union[Parameter, Reference]]]
 
 
 def get_description_for_handler(
     handler: "HTTPHandler", use_handler_docstrings: bool
 ) -> Optional[str]:
     description = handler.description
     if description is None and use_handler_docstrings:
@@ -82,12 +87,12 @@
                 deprecated=handler.deprecated,
                 responses=create_responses(
                     handler=handler,
                     raises_validation_error=raises_validation_error,
                     create_examples=create_examples,
                 ),
                 requestBody=request_body,
-                parameters=parameters,
+                parameters=cast("OptionalRef", parameters),
                 security=security,
             )
             setattr(path_item, http_method.lower(), operation)
     return path_item
```

### Comparing `esmerald-1.2.5/esmerald/openapi/request_body.py` & `esmerald-1.3.0/esmerald/openapi/request_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     """
     Gets the request body of the handler.
     """
     media_type = field.field_info.extra.get("media_type", EncodingType.JSON)
     schema = create_schema(field=field, create_examples=create_examples)
     update_schema_field_info(schema=schema, field_info=field.field_info)
     return RequestBody(
-        required=True, content={media_type: OpenAPIMediaType(media_type_schema=schema)}
+        required=True, content={media_type: OpenAPIMediaType(media_type_schema=schema)}  # type: ignore[call-arg]
     )
```

### Comparing `esmerald-1.2.5/esmerald/openapi/responses.py` & `esmerald-1.3.0/esmerald/openapi/responses.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from http import HTTPStatus
 from inspect import Signature
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Type, cast
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Type, Union, cast
 
 from openapi_schemas_pydantic.v3_1_0 import Response
 from openapi_schemas_pydantic.v3_1_0.header import Header
 from openapi_schemas_pydantic.v3_1_0.media_type import MediaType as OpenAPISchemaMediaType
+from openapi_schemas_pydantic.v3_1_0.reference import Reference
 from openapi_schemas_pydantic.v3_1_0.schema import Schema
 from starlette.routing import get_name
 from typing_extensions import get_args, get_origin
 
 from esmerald.datastructures import File, Redirect, Stream, Template
 from esmerald.enums import MediaType
 from esmerald.exceptions import HTTPException, ImproperlyConfigured, ValidationErrorException
@@ -60,52 +61,52 @@
         elif get_origin(signature.return_annotation) is EsmeraldResponse:
             return_annotation = get_args(signature.return_annotation)[0] or Any
         as_parsed_model_field = create_parsed_model_field(return_annotation)
         schema = create_schema(field=as_parsed_model_field, create_examples=create_examples)
         schema.contentEncoding = handler.content_encoding
         schema.contentMediaType = handler.content_media_type
         response = Response(
-            content={handler.media_type: OpenAPISchemaMediaType(media_type_schema=schema)},
+            content={handler.media_type: OpenAPISchemaMediaType(media_type_schema=schema)},  # type: ignore[call-arg]
             description=description,
         )
     elif signature.return_annotation is Redirect:
         response = Response(
             content=None,
             description=description,
             headers={
-                "location": Header(
+                "location": Header(  # type: ignore[call-arg]
                     param_schema=Schema(type=OpenAPIType.STRING),
                     description="target path for redirect",
                 )
             },
         )
     elif signature.return_annotation in (File, Stream):
         response = Response(
             content={
-                handler.media_type: OpenAPISchemaMediaType(
+                handler.media_type: OpenAPISchemaMediaType(  # type: ignore[call-arg]
                     media_type_schema=Schema(
                         type=OpenAPIType.STRING,
                         contentEncoding=handler.content_encoding or "application/octet-stream",
                         contentMediaType=handler.content_media_type,
                     )
                 )
             },
             description=description,
             headers={
-                "content-length": Header(
+                "content-length": Header(  # type: ignore[call-arg]
                     param_schema=Schema(type=OpenAPIType.STRING),
                     description="File size in bytes",
                 ),
-                "last-modified": Header(
-                    param_schema=Schema(
+                "last-modified": Header(  # type: ignore[call-arg]
+                    param_schema=Schema(  # type: ignore[call-arg]
                         type=OpenAPIType.STRING, schema_format=OpenAPIFormat.DATE_TIME
                     ),
                     description="Last modified data-time in RFC 2822 format",
                 ),
-                "etag": Header(
+                "etag": Header(  # type: ignore[call-arg]
                     param_schema=Schema(type=OpenAPIType.STRING),
                     description="Entity tag",
                 ),
             },
         )
     else:
         response = Response(content=None, description=description)
@@ -118,61 +119,61 @@
         for attribute_name, attribute_value in value.dict(exclude_none=True).items():
             if attribute_name == "value":
                 model_field = create_parsed_model_field(type(attribute_value))
                 header.param_schema = create_schema(field=model_field, create_examples=False)
         response.headers[key] = header
     cookies = handler.get_response_cookies()
     if cookies:
-        response.headers["Set-Cookie"] = Header(
-            param_schema=Schema(allOF=[create_cookie_schema(cookie=cookie) for cookie in cookies])
+        response.headers["Set-Cookie"] = Header(  # type: ignore[call-arg]
+            param_schema=Schema(allOf=[create_cookie_schema(cookie=cookie) for cookie in cookies])
         )
     return response
 
 
 def create_error_responses(
     exceptions: List[Type[HTTPException]],
 ) -> Iterator[Tuple[str, Response]]:
     grouped_exceptions: Dict[int, List[Type[HTTPException]]] = {}
     for exc in exceptions:
         if not grouped_exceptions.get(exc.status_code):
             grouped_exceptions[exc.status_code] = []
         grouped_exceptions[exc.status_code].append(exc)
 
     for status_code, exception_group in grouped_exceptions.items():
-        exception_schemas = [
+        exception_schemas: Optional[List[Union[Reference, Schema]]] = [
             Schema(
                 type=OpenAPIType.OBJECT,
                 required=["detail", "status_code"],
                 properties={
                     "status_code": Schema(type=OpenAPIType.INTEGER),
                     "detail": Schema(type=OpenAPIType.STRING),
                     "extra": Schema(
                         type=[OpenAPIType.NULL, OpenAPIType.OBJECT, OpenAPIType.ARRAY],
                         additionalProperties=Schema(),
                     ),
                 },
-                description=pascal_case_to_text((get_name(exc))),
+                description=pascal_case_to_text(get_name(exc)),
                 examples=[
                     {
                         "status_code": status_code,
                         "detail": HTTPStatus(status_code).phrase,
                         "extra": {},
                     }
                 ],
             )
             for exc in exception_group
         ]
 
         if len(exception_schemas) > 1:
             schema = Schema(oneOf=exception_schemas)
         else:
-            schema = exception_schemas[0]
+            schema = cast("Schema", exception_schemas[0])
         yield str(status_code), Response(
             description=HTTPStatus(status_code).description,
-            content={MediaType.JSON: OpenAPISchemaMediaType(media_type_schema=schema)},
+            content={MediaType.JSON: OpenAPISchemaMediaType(media_type_schema=schema)},  # type: ignore[call-arg]
         )
 
 
 def create_additional_responses(
     handler: "HTTPHandler",
 ) -> Iterator[Tuple[str, Response]]:
     if not handler.responses:
@@ -183,15 +184,15 @@
         schema = create_schema(
             field=model_field, create_examples=additional_response.create_examples
         )
 
         yield str(status_code), Response(
             description=additional_response.description,
             content={
-                additional_response.media_type: OpenAPISchemaMediaType(media_type_schema=schema)
+                additional_response.media_type: OpenAPISchemaMediaType(media_type_schema=schema)  # type: ignore[call-arg]
             },
         )
 
 
 def create_responses(
     handler: "HTTPHandler", raises_validation_error: bool, create_examples: bool
 ) -> Optional["Responses"]:
```

### Comparing `esmerald-1.2.5/esmerald/openapi/schema.py` & `esmerald-1.3.0/esmerald/openapi/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from dataclasses import is_dataclass
 from decimal import Decimal
 from enum import Enum, EnumMeta
+from re import Pattern
 from typing import Any, List, Optional, Type, Union
 
 from openapi_schemas_pydantic.utils.constants import (
     EXTRA_TO_OPENAPI_PROPERTY_MAP,
     PYDANTIC_TO_OPENAPI_PROPERTY_MAP,
     TYPE_MAP,
 )
 from openapi_schemas_pydantic.utils.utils import OpenAPI310PydanticSchema
 from openapi_schemas_pydantic.v3_1_0.example import Example
+from openapi_schemas_pydantic.v3_1_0.reference import Reference
 from openapi_schemas_pydantic.v3_1_0.schema import Schema
 from pydantic import (
     BaseModel,
     ConstrainedBytes,
     ConstrainedDecimal,
     ConstrainedFloat,
     ConstrainedInt,
     ConstrainedList,
     ConstrainedSet,
     ConstrainedStr,
 )
 from pydantic.fields import FieldInfo, ModelField, Undefined
-from pydantic_factories import ModelFactory
-from pydantic_factories.exceptions import ParameterError
-from pydantic_factories.utils import is_optional, is_pydantic_model, is_union
+from pyfactories import ModelFactory
+from pyfactories.exceptions import ParameterError
+from pyfactories.utils import is_optional, is_pydantic_model, is_union
 
 from esmerald.datastructures import UploadFile
 from esmerald.datastructures.types import EncoderType
 from esmerald.openapi.enums import OpenAPIType
 from esmerald.openapi.utils import get_openapi_type_for_complex_type
 from esmerald.utils.helpers import is_class_and_subclass
 from esmerald.utils.model import convert_dataclass_to_model, create_parsed_model_field
 
 
-def clean_values_from_example(value: Any):
+def clean_values_from_example(value: Any) -> Any:
     if isinstance(value, (Decimal, float)):
         value = round(float(value), 3)
 
     if isinstance(value, Enum):
         value = value.value
 
     if is_dataclass(value):
@@ -85,15 +87,15 @@
     field_type: Union[Type[ConstrainedStr], Type[ConstrainedBytes]]
 ) -> Schema:
     schema = Schema(type=OpenAPIType.STRING)
     if field_type.min_length:
         schema.minLength = field_type.min_length
     if field_type.max_length:
         schema.maxLength = field_type.max_length
-    if issubclass(field_type, ConstrainedStr) and field_type.regex is not None:
+    if hasattr(field_type, "regex") and isinstance(field_type.regex, Pattern):
         schema.pattern = field_type.regex.pattern
     if field_type.to_lower:
         schema.description = "must be in lower case"
     return schema
 
 
 def create_collection_constrained_field_schema(
@@ -105,17 +107,19 @@
     if field_type.min_items:
         schema.minItems = field_type.min_items
     if field_type.max_items:
         schema.maxItems = field_type.max_items
     if issubclass(field_type, ConstrainedSet):
         schema.uniqueItems = True
     if sub_fields:
-        items = [create_schema(field=sub_field, create_examples=False) for sub_field in sub_fields]
+        items: List[Union[Reference, Schema]] = [
+            create_schema(field=sub_field, create_examples=False) for sub_field in sub_fields
+        ]
         if len(items) > 1:
-            schema.items = Schema(oneOf=items)  # type: ignore[arg-type]
+            schema.items = Schema(oneOf=items)
         else:
             schema.items = items[0]
     else:
         parsed_model_field = create_parsed_model_field(field_type.item_type)
         schema.items = create_schema(field=parsed_model_field, create_examples=False)
     return schema
 
@@ -188,15 +192,17 @@
     try:
         value = clean_values_from_example(ExampleFactory.get_field_value(field))
         return [Example(description=f"Example {field.name} value", value=value)]
     except ParameterError:
         return []
 
 
-def create_schema(field: ModelField, create_examples: bool, ignore_optional: bool = False):
+def create_schema(
+    field: ModelField, create_examples: bool, ignore_optional: bool = False
+) -> Schema:
     if is_optional(field) and not ignore_optional:
         non_optional_schema = create_schema(
             field=field, create_examples=False, ignore_optional=True
         )
 
         schema = Schema(
             oneOf=[
@@ -215,21 +221,21 @@
                 for sub_field in field.sub_fields or []
             ]
         )
 
     elif ModelFactory.is_constrained_field(field.type_):
         field.outer_type_ = field.type_
         schema = create_constrained_field_schema(
-            field_type=field.outer_type_, sub_fields=field.sub_fields
+            field_type=field.outer_type_, sub_fields=field.sub_fields  # type: ignore
         )
     elif field.sub_fields:
         openapi_type = get_openapi_type_for_complex_type(field)
         schema = Schema(type=openapi_type)
         if openapi_type == OpenAPIType.ARRAY:
-            items = [
+            items: List[Union[Reference, Schema]] = [  # type: ignore
                 create_schema(field=sub_field, create_examples=False)
                 for sub_field in field.sub_fields
             ]
             if len(items) > 1:
                 schema.items = Schema(oneOf=items)
             else:
                 schema.items = items[0]
```

### Comparing `esmerald-1.2.5/esmerald/openapi/utils.py` & `esmerald-1.3.0/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/permissions/base.py` & `esmerald-1.3.0/esmerald/permissions/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,116 +1,116 @@
 """Esmerald permission system"""
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from esmerald.exceptions import ImproperlyConfigured
 
 if TYPE_CHECKING:
     from esmerald.requests import Request
     from esmerald.types import APIGateHandler
 
 SAFE_METHODS = ("GET", "HEAD", "OPTIONS")
 
 
 class BaseOperationHolder:
-    def __and__(self, other):
+    def __and__(self, other: Any) -> "OperandHolder":
         return OperandHolder(AND, self, other)
 
-    def __or__(self, other):
+    def __or__(self, other: "Any") -> "OperandHolder":
         return OperandHolder(OR, self, other)
 
-    def __rand__(self, other):
+    def __rand__(self, other: Any) -> "OperandHolder":
         return OperandHolder(AND, other, self)
 
-    def __ror__(self, other):
+    def __ror__(self, other: "BasePermission") -> "OperandHolder":
         return OperandHolder(OR, other, self)
 
-    def __invert__(self):
+    def __invert__(self) -> "SingleOperand":
         return SingleOperand(NOT, self)
 
 
 class SingleOperand(BaseOperationHolder):
-    def __init__(self, operator_class, op1_class):
+    def __init__(self, operator_class: Any, op1_class: Any) -> None:
         self.operator_class = operator_class
         self.op1_class = op1_class
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
         op1 = self.op1_class(*args, **kwargs)
         return self.operator_class(op1)
 
 
 class OperandHolder(BaseOperationHolder):
-    def __init__(self, operator_class, op1_class, op2_class):
+    def __init__(self, operator_class: Any, op1_class: Any, op2_class: Any) -> None:
         self.operator_class = operator_class
         self.op1_class = op1_class
         self.op2_class = op2_class
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
         op1 = self.op1_class(*args, **kwargs)
         op2 = self.op2_class(*args, **kwargs)
         return self.operator_class(op1, op2)
 
 
 class AND:
-    def __init__(self, op1, op2):
+    def __init__(self, op1: "BasePermission", op2: "BasePermission") -> None:
         self.op1 = op1
         self.op2 = op2
 
     def has_permission(
         self,
         request: "Request",
         apiview: "APIGateHandler",
     ) -> bool:
         return self.op1.has_permission(request, apiview) and self.op2.has_permission(
             request, apiview
         )
 
 
 class OR:
-    def __init__(self, op1, op2):
+    def __init__(self, op1: "BasePermission", op2: "BasePermission") -> None:
         self.op1 = op1
         self.op2 = op2
 
     def has_permission(
         self,
         request: "Request",
         apiview: "APIGateHandler",
     ) -> bool:
         return self.op1.has_permission(request, apiview) or self.op2.has_permission(
             request, apiview
         )
 
 
 class NOT:
-    def __init__(self, op1):
+    def __init__(self, op1: "BasePermission") -> None:
         self.op1 = op1
 
     def has_permission(
         self,
         request: "Request",
         apiview: "APIGateHandler",
     ) -> bool:
         return not self.op1.has_permission(request, apiview)
 
 
-class BasePermissionMetaclass(BaseOperationHolder, type):
+class BasePermissionMetaclass(BaseOperationHolder, type):  # type: ignore[misc]
     ...
 
 
 class BasePermission(metaclass=BasePermissionMetaclass):
     """
     A base class from which all permission classes should inherit.
     """
 
     def has_permission(
         self,
         request: "Request",
         apiview: "APIGateHandler",
-    ):
+    ) -> bool:
         """
         Return `True` if permission is granted, `False` otherwise.
         """
         return True
 
 
 class BaseAbstractUserPermission(ABC):
@@ -120,15 +120,15 @@
 
     def has_permission(
         self,
         request: "Request",
         apiview: "APIGateHandler",
     ) -> bool:
         try:
-            hasattr(request, "user")
+            return hasattr(request, "user")
         except ImproperlyConfigured:
             return False
 
     @abstractmethod
     def is_user_authenticated(self, request: "Request") -> bool:
         """
         This method must be overridden by subclasses.
```

### Comparing `esmerald-1.2.5/esmerald/permissions/utils.py` & `esmerald-1.3.0/esmerald/permissions/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import TYPE_CHECKING, List, Optional  # noqa
+from typing import TYPE_CHECKING, List, Optional
 
-from esmerald.exceptions import PermissionDenied  # noqa
+from esmerald.exceptions import PermissionDenied
 
 if TYPE_CHECKING:
-    from esmerald.permissions.types import Permission  # noqa
-    from esmerald.requests import Request  # noqa
-    from esmerald.types import APIGateHandler  # noqa
+    from esmerald.permissions import BasePermission
+    from esmerald.permissions.types import Permission
+    from esmerald.requests import Request
+    from esmerald.types import APIGateHandler
 
 
 def check_permissions(
     request: "Request",
     apiview: "APIGateHandler",
     permissions: List["Permission"],
 ) -> None:
@@ -24,21 +25,21 @@
                 message=getattr(permission, "message", None),
             )
 
 
 def continue_or_raise_permission_exception(
     request: "Request",
     apiview: "APIGateHandler",
-    permission: "Permission",
-):
-    if not permission.has_permission(request, apiview):
+    permission: "BasePermission",
+) -> None:
+    if not permission.has_permission(request=request, apiview=apiview):
         permission_denied(
             request,
             message=getattr(permission, "message", None),
         )
 
 
-def permission_denied(request: "Request", message: Optional[str] = None) -> PermissionDenied:
+def permission_denied(request: "Request", message: Optional[str] = None) -> None:
     """
     If request is not permitted, determine what kind of exception to raise.
     """
     raise PermissionDenied(detail=message, status_code=403)
```

### Comparing `esmerald-1.2.5/esmerald/pluggables/base.py` & `esmerald-1.3.0/esmerald/pluggables/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Iterator, Optional
 
 from esmerald.protocols.extension import ExtensionProtocol
 
 if TYPE_CHECKING:
-    pass
-
     from esmerald.applications import Esmerald
     from esmerald.types import DictAny
 
 
 class Pluggable:
     """
     The class object used to manage pluggables for esmerald.
 
     A pluggable is whatever adds extra level of functionality to
     your an Esmerald application and is used as support for your application.
     """
 
-    def __init__(self, cls: type, **options: Any):
+    def __init__(self, cls: "Extension", **options: Any):
         self.cls = cls
         self.options = options
 
     def __iter__(self) -> Iterator:
         iterator = (self.cls, self.options)
         return iter(iterator)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         name = self.__class__.__name__
         options = [f"{key}={value!r}" for key, value in self.options.items()]
         args = ", ".join([self.__class__.__name__] + options)
         return f"{name}({args})"
 
 
 class BaseExtension(ABC, ExtensionProtocol):
```

### Comparing `esmerald-1.2.5/esmerald/protocols/asyncdao.py` & `esmerald-1.3.0/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/protocols/dao.py` & `esmerald-1.3.0/esmerald/protocols/dao.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from typing import TYPE_CHECKING, Any, List, TypeVar
+from typing import TYPE_CHECKING, Any, List
 
 from typing_extensions import Protocol, runtime_checkable
 
 if TYPE_CHECKING:
     from esmerald.types import DictAny
 
-T = TypeVar("T")
-
 
 @runtime_checkable
 class DaoProtocol(Protocol):  # pragma: no cover
     """
     Data Access Object (DAO) is an abstract pattern widely used to
     separate the underlying logic of the database from the business logic.
```

### Comparing `esmerald-1.2.5/esmerald/protocols/interceptor.py` & `esmerald-1.3.0/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/protocols/template.py` & `esmerald-1.3.0/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/responses/base.py` & `esmerald-1.3.0/esmerald/responses/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class Response(StarletteResponse, Generic[T]):
     def __init__(
         self,
         content: T,
         *,
-        status_code: Optional[int] = status.HTTP_200_OK,
+        status_code: int = status.HTTP_200_OK,
         media_type: Optional[Union["MediaType", str]] = MediaType.JSON,
         background: Optional[Union["BackgroundTask", "BackgroundTasks"]] = None,
         headers: Optional[Dict[str, Any]] = None,
         cookies: Optional["ResponseCookies"] = None,
     ) -> None:
         super().__init__(
             content=content,
```

### Comparing `esmerald-1.2.5/esmerald/responses/encoders.py` & `esmerald-1.3.0/esmerald/responses/encoders.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import Any
 
-from starlette.responses import JSONResponse as JSONResponse  # noqa
+from starlette.responses import JSONResponse as JSONResponse
 
 from esmerald.responses.json import BaseJSONResponse
 
 try:
     import orjson
-    from orjson import OPT_OMIT_MICROSECONDS  # noqa
-    from orjson import OPT_SERIALIZE_NUMPY
-except ImportError:  # pragma: nocover
+    from orjson import OPT_OMIT_MICROSECONDS, OPT_SERIALIZE_NUMPY
+except ImportError:
     orjson = None
 
 try:
     import ujson
-except ImportError:  # pragma: nocover
+except ImportError:
     ujson = None
 
 
 class ORJSONResponse(BaseJSONResponse):
     def render(self, content: Any) -> bytes:
         assert orjson is not None, "You must install the encoders or orjson to use ORJSONResponse"
         return orjson.dumps(
```

### Comparing `esmerald-1.2.5/esmerald/responses/template.py` & `esmerald-1.3.0/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/routing/base.py` & `esmerald-1.3.0/esmerald/routing/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     Optional,
     Set,
-    Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 from uuid import UUID
 
@@ -37,32 +36,34 @@
 from esmerald.permissions.utils import continue_or_raise_permission_exception
 from esmerald.requests import Request
 from esmerald.responses import JSONResponse, Response
 from esmerald.routing.views import APIView
 from esmerald.transformers.model import TransformerModel
 from esmerald.transformers.signature import SignatureFactory
 from esmerald.transformers.utils import get_signature
-from esmerald.typing import Void
+from esmerald.typing import Void, VoidType
 from esmerald.utils.helpers import is_async_callable, is_class_and_subclass
 from esmerald.utils.sync import AsyncCallable
 
 if TYPE_CHECKING:
     from pydantic.typing import AnyCallable
 
     from esmerald.applications import Esmerald
+    from esmerald.interceptors.interceptor import EsmeraldInterceptor
     from esmerald.interceptors.types import Interceptor
+    from esmerald.permissions import BasePermission
     from esmerald.permissions.types import Permission
-    from esmerald.routing.router import HTTPHandler, WebSocketHandler
+    from esmerald.routing.router import HTTPHandler
     from esmerald.types import (
+        APIGateHandler,
         AsyncAnyCallable,
-        ExceptionHandlers,
-        ParentType,
+        Dependencies,
+        ExceptionHandlerMap,
         ResponseCookies,
         ResponseHeaders,
-        ResponseType,
     )
 
 param_type_map = {
     "str": str,
     "int": int,
     "float": float,
     "uuid": UUID,
@@ -83,15 +84,15 @@
 class PathParameterSchema(TypedDict):
     name: str
     full: str
     type: Type
 
 
 class OpenAPIDefinitionMixin:
-    def parse_path(self, path: str) -> Tuple[str, str, List[Union[str, PathParameterSchema]]]:
+    def parse_path(self, path: str) -> List[Union[str, PathParameterSchema]]:
         """
         Using the Starlette CONVERTORS and the application registered convertors,
         transforms the path into a PathParameterSchema used for the OpenAPI definition.
         """
         _, path, variables = compile_path(path)
 
         parsed_components: List[Union[str, PathParameterSchema]] = []
@@ -158,19 +159,19 @@
         headers: Dict[str, Any],
         media_type: str,
         status_code: int,
     ) -> "AsyncAnyCallable":
         """Creates a handler for ResponseContainer Types"""
 
         async def response_content(
-            data: ResponseContainer, app: "Esmerald", **kwargs: Dict[str, Any]
+            data: ResponseContainer, app: Type["Esmerald"], **kwargs: Dict[str, Any]
         ) -> StarletteResponse:
             _headers = {**self.get_headers(headers), **data.headers}
             _cookies = self.get_cookies(data.cookies, cookies)
-            response = data.to_response(
+            response: Response = data.to_response(
                 app=app,
                 headers=_headers,
                 status_code=status_code,
                 media_type=media_type,
             )
             for cookie in _cookies:
                 response.set_cookie(**cookie)
@@ -252,25 +253,25 @@
                 **self.allow_header,
             }
             for cookie in _cookies:
                 data.set_cookie(**cookie)
 
             for header, value in _headers.items():
                 data.headers[header] = value
-            return data  # type: ignore
+            return data
 
         return response_content
 
-    def handler(
+    def _handler(
         self,
         background: Optional[Union["BackgroundTask", "BackgroundTasks"]],
         cookies: "ResponseCookies",
         headers: Dict[str, Any],
         media_type: str,
-        response_class: "ResponseType",
+        response_class: Any,
         status_code: int,
     ) -> "AsyncAnyCallable":
         async def response_content(data: Any, **kwargs: Dict[str, Any]) -> StarletteResponse:
             data = await self.get_response_data(data=data)
             _cookies = self.get_cookies(cookies, [])
             if isinstance(data, JSONResponse):
                 response = data
@@ -283,23 +284,23 @@
                     headers=headers,
                     media_type=media_type,
                     status_code=status_code,
                 )
 
             for cookie in _cookies:
                 response.set_cookie(**cookie)
-            return response  # type: ignore
+            return response
 
         return response_content
 
     async def get_response_for_request(
         self,
         scope: "Scope",
         request: Request,
-        route: Union["HTTPHandler", "WebSocketHandler"],
+        route: "HTTPHandler",
         parameter_model: "TransformerModel",
     ) -> "StarletteResponse":
         response: Optional["StarletteResponse"] = None
         if not response:
             response = await self.call_handler_function(
                 scope=scope,
                 request=request,
@@ -309,17 +310,17 @@
 
         return response
 
     async def call_handler_function(
         self,
         scope: "Scope",
         request: Request,
-        route: Union["HTTPHandler", "WebSocketHandler"],
+        route: "HTTPHandler",
         parameter_model: "TransformerModel",
-    ) -> "StarletteResponse":
+    ) -> Any:
         response_data = await self._get_response_data(
             route=route,
             parameter_model=parameter_model,
             request=request,
         )
 
         return await self.to_response(
@@ -403,15 +404,15 @@
                 )
             elif is_class_and_subclass(self.signature.return_annotation, StarletteResponse):
                 handler = self.starlette_response_handler(
                     cookies=cookies,
                     headers=headers,
                 )
             else:
-                handler = self.handler(
+                handler = self._handler(
                     background=self.background,
                     cookies=cookies,
                     headers=headers,
                     media_type=media_type,
                     response_class=response_class,
                     status_code=self.status_code,
                 )
@@ -441,36 +442,38 @@
         """
         parameters = set()
         for param_name, _ in self.param_convertors.items():
             parameters.add(param_name)
         return parameters
 
     @property
-    def normalised_path_params(self) -> List[Dict[str, str]]:
+    def normalised_path_params(self) -> List[PathParameterSchema]:
         """
         Gets the path parameters in a PathParameterSchema format and it is
         only used for OpenAPI documentation purposes only.
         """
         path_components = self.parse_path(self.path)
         parameters = [component for component in path_components if isinstance(component, dict)]
         return parameters
 
     @property
-    def stringify_parameters(self) -> List[Dict[str, str]]:
+    def stringify_parameters(self) -> List[str]:
         """
         Gets the param:type in string like list.
         """
         path_components = self.parse_path(self.path)
         parameters = [component for component in path_components if isinstance(component, dict)]
 
-        parameters = [f"{param['name']}:{param['type'].__name__}" for param in parameters]
-        return parameters
+        stringified_parameters = [
+            f"{param['name']}:{param['type'].__name__}" for param in parameters
+        ]
+        return stringified_parameters
 
     @property
-    def parent_levels(self) -> List[Union[T, "ParentType"]]:
+    def parent_levels(self) -> List[Any]:
         """
         Returns the handler from the app down to the route handler.
 
         Who is the parent of a given layer/level.
 
         Example:
 
@@ -494,67 +497,68 @@
     @property
     def dependency_names(self) -> Set[str]:
         """A unique set of all dependency names provided in the handlers parent
         levels."""
         level_dependencies = (level.dependencies or {} for level in self.parent_levels)
         return {name for level in level_dependencies for name in level.keys()}
 
-    def get_permissions(self) -> List["Permission"]:
+    def get_permissions(self) -> List["AsyncCallable"]:
         """
         Returns all the permissions in the handler scope from the ownsership layers.
         """
         if self._permissions is Void:
-            self._permissions = []
+            self._permissions: Union[List["Permission"], "VoidType"] = []
             for layer in self.parent_levels:
                 self._permissions.extend(layer.permissions or [])
             self._permissions = cast(
                 "List[Permission]",
                 [AsyncCallable(permissions) for permissions in self._permissions],
             )
-        return cast("List[Permission]", self._permissions)
+        return cast("List[AsyncCallable]", self._permissions)
 
-    def get_dependencies(self) -> Dict[str, Inject]:
+    def get_dependencies(self) -> "Dependencies":
         """
         Returns all dependencies of the handler function's starting from the parent levels.
         """
         if not self.signature_model:
             raise RuntimeError(
                 "get_dependencies cannot be called before a signature model has been generated"
             )
-        if self._dependencies is Void:
-            self._dependencies = {}
+
+        if not self._dependencies or self._dependencies is Void:
+            self._dependencies: "Dependencies" = {}
             for level in self.parent_levels:
                 for key, value in (level.dependencies or {}).items():
                     self.is_unique_dependency(
                         dependencies=self._dependencies,
                         key=key,
                         injector=value,
                     )
                     self._dependencies[key] = value
-        return cast("Dict[str, Inject]", self._dependencies)
+        return self._dependencies
 
     @staticmethod
-    def is_unique_dependency(dependencies: Dict[str, Inject], key: str, injector: Inject) -> None:
+    def is_unique_dependency(dependencies: "Dependencies", key: str, injector: Inject) -> None:
         """
         Validates that a given inject has not been already defined under a
         different key in any of the levels.
         """
         for dependency_key, value in dependencies.items():
             if injector == value:
                 raise ImproperlyConfigured(
                     f"Injector for key {key} is already defined under the different key {dependency_key}. "
                     f"If you wish to override a inject, it must have the same key."
                 )
 
-    def get_exception_handlers(self) -> "ExceptionHandlers":
+    def get_exception_handlers(self) -> "ExceptionHandlerMap":
         """
         Resolves the exception_handlers by starting from the route handler
         and moving up.
         """
-        resolved_exception_handlers = {}
+        resolved_exception_handlers: "ExceptionHandlerMap" = {}
         for level in self.parent_levels:
             resolved_exception_handlers.update(level.exception_handlers or {})
         return resolved_exception_handlers
 
     def get_cookies(
         self, local_cookies: "ResponseCookies", other_cookies: "ResponseCookies"
     ) -> List[Dict[str, Any]]:
@@ -589,35 +593,37 @@
         Validates the connection.
 
         Handles with the permissions for each view (get, put, post, delete, patch, route...) after the request.
 
         Raises a PermissionDenied exception if not allowed..
         """
         for permission in self.get_permissions():
-            permission = await permission()
-            permission.has_permission(connection, self)
-            continue_or_raise_permission_exception(connection, self, permission)
+            awaitable: "BasePermission" = cast("BasePermission", await permission())
+            request: "Request" = cast("Request", connection)
+            handler = cast("APIGateHandler", self)
+            awaitable.has_permission(request, handler)
+            continue_or_raise_permission_exception(request, handler, awaitable)
 
 
 class BaseInterceptorMixin(BaseHandlerMixin):
-    def get_interceptors(self) -> List["Interceptor"]:
+    def get_interceptors(self) -> List["AsyncCallable"]:
         """
         Returns all the interceptors in the handler scope from the ownsership layers.
         """
         if self._interceptors is Void:
-            self._interceptors = []
+            self._interceptors: Union[List["Interceptor"], "VoidType"] = []
             for layer in self.parent_levels:
                 self._interceptors.extend(layer.interceptors or [])
             self._interceptors = cast(
                 "List[Interceptor]",
                 [AsyncCallable(interceptors) for interceptors in self._interceptors],
             )
-        return cast("List[Interceptor]", self._interceptors)
+        return cast("List[AsyncCallable]", self._interceptors)
 
     async def intercept(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
         """
         Checks for every interceptor on each level and runs them all before reaching any
         of the handlers.
         """
         for interceptor in self.get_interceptors():
-            interceptor = await interceptor()
-            await interceptor.intercept(scope, receive, send)
+            awaitable: "EsmeraldInterceptor" = await interceptor()
+            await awaitable.intercept(scope, receive, send)
```

### Comparing `esmerald-1.2.5/esmerald/routing/events.py` & `esmerald-1.3.0/esmerald/routing/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Callable, List, Optional, Sequence, TypeVar
+from typing import TYPE_CHECKING, Any, Optional, Sequence, TypeVar
 
 from starlette._utils import is_async_callable
 from starlette.types import Lifespan, Receive, Scope, Send
 
 if TYPE_CHECKING:
     from esmerald.types import DictAny, LifeSpanHandler
 
@@ -22,43 +22,45 @@
     This aims to provide a similar functionality but by generating
     a lifespan event based on the values from the on_startup and on_shutdown
     lists.
     """
 
     def __init__(
         self,
-        on_shutdown: Optional[List["LifeSpanHandler"]] = None,
-        on_startup: Optional[List["LifeSpanHandler"]] = None,
+        on_shutdown: Optional[Sequence["LifeSpanHandler"]] = None,
+        on_startup: Optional[Sequence["LifeSpanHandler"]] = None,
     ) -> None:
         self.on_startup = [] if on_startup is None else list(on_startup)
         self.on_shutdown = [] if on_shutdown is None else list(on_shutdown)
 
     def __call__(self: _T, app: object) -> _T:
         return self
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> None:
         """Runs the functions on startup"""
         for handler in self.on_startup:
             if is_async_callable(handler):
-                await handler()
+                await handler()  # type: ignore[call-arg]
             else:
-                handler()
+                handler()  # type: ignore[call-arg]
 
-    async def __aexit__(self, scope: Scope, receive: Receive, send: Send, **kwargs: "DictAny"):
+    async def __aexit__(
+        self, scope: Scope, receive: Receive, send: Send, **kwargs: "DictAny"
+    ) -> None:
         """Runs the functions on shutdown"""
         for handler in self.on_shutdown:
             if is_async_callable(handler):
-                await handler()
+                await handler()  # type: ignore[call-arg]
             else:
-                handler()
+                handler()  # type: ignore[call-arg]
 
 
 def handle_lifespan_events(
-    on_startup: Optional[Sequence[Callable]] = None,
-    on_shutdown: Optional[Sequence[Callable]] = None,
+    on_startup: Optional[Sequence["LifeSpanHandler"]] = None,
+    on_shutdown: Optional[Sequence["LifeSpanHandler"]] = None,
     lifespan: Optional[Lifespan[Any]] = None,
 ) -> Any:
     """Handles with the lifespan events in the new Starlette format of lifespan.
     This adds a mask that keeps the old `on_startup` and `on_shutdown` events variable
     declaration for legacy and comprehension purposes and build the async context manager
     for the lifespan.
     """
@@ -66,14 +68,14 @@
         return AyncLifespanContextManager(on_startup=on_startup, on_shutdown=on_shutdown)
     elif lifespan:
         return lifespan
     return None
 
 
 def generate_lifespan_events(
-    on_startup: Optional[Sequence[Callable]] = None,
-    on_shutdown: Optional[Sequence[Callable]] = None,
+    on_startup: Optional[Sequence["LifeSpanHandler"]] = None,
+    on_shutdown: Optional[Sequence["LifeSpanHandler"]] = None,
     lifespan: Optional[Lifespan[Any]] = None,
 ) -> Any:
     if lifespan:
         return lifespan
     return AyncLifespanContextManager(on_startup=on_startup, on_shutdown=on_shutdown)
```

### Comparing `esmerald-1.2.5/esmerald/routing/gateways.py` & `esmerald-1.3.0/esmerald/routing/gateways.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import re
-from typing import TYPE_CHECKING, Callable, List, Optional, Type, Union
+from typing import TYPE_CHECKING, Callable, List, Optional, Sequence, Union, cast
 
 from starlette.routing import Route as StarletteRoute
 from starlette.routing import WebSocketRoute as StarletteWebSocketRoute
 from starlette.routing import compile_path
 from starlette.types import Receive, Scope, Send
 
 from esmerald.routing.base import BaseInterceptorMixin
 from esmerald.routing.views import APIView
-from esmerald.typing import Void
+from esmerald.typing import Void, VoidType
 from esmerald.utils.helpers import clean_string, is_class_and_subclass
 from esmerald.utils.url import clean_path
 
 if TYPE_CHECKING:
     from esmerald.interceptors.types import Interceptor
     from esmerald.permissions.types import Permission
     from esmerald.routing.router import HTTPHandler, WebSocketHandler
-    from esmerald.types import Dependencies, ExceptionHandlers, Middleware, ParentType
+    from esmerald.types import Dependencies, ExceptionHandlerMap, Middleware, ParentType
 
 
 class Gateway(StarletteRoute, BaseInterceptorMixin):
     __slots__ = (
         "_interceptors",
         "path",
         "handler",
@@ -35,61 +35,62 @@
         "deprecated",
     )
 
     def __init__(
         self,
         path: Optional[str] = None,
         *,
-        handler: Union[Type["HTTPHandler"], Type["APIView"], Type[Callable]],
+        handler: Union["HTTPHandler", APIView],
         name: Optional[str] = None,
         include_in_schema: bool = True,
         parent: Optional["ParentType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        middleware: Optional["Middleware"] = None,
-        interceptors: Optional["Interceptor"] = None,
-        permissions: Optional["Permission"] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
+        middleware: Optional[Sequence["Middleware"]] = None,
+        interceptors: Optional[Sequence["Interceptor"]] = None,
+        permissions: Optional[Sequence["Permission"]] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         deprecated: Optional[bool] = None,
         is_from_router: bool = False,
     ) -> None:
         if not path:
             path = "/"
         if is_class_and_subclass(handler, APIView):
-            handler = handler(parent=self)
+            handler = handler(parent=self)  # type: ignore
 
         if not is_from_router:
             self.path = clean_path(path + handler.path)
         else:
             self.path = clean_path(path)
+
         self.methods = getattr(handler, "methods", None)
 
         if not name:
             if not isinstance(handler, APIView):
                 name = clean_string(handler.fn.__name__)
             else:
                 name = clean_string(handler.__class__.__name__)
 
         super().__init__(
             path=self.path,
-            endpoint=handler,
+            endpoint=cast("Callable", handler),
             include_in_schema=include_in_schema,
             name=name,
-            methods=self.methods,
+            methods=cast("List[str]", self.methods),
         )
         """
         A "bridge" to a handler and router mapping functionality.
         Since the default Starlette Route endpoint does not understand the Esmerald handlers,
         the Gateway bridges both functionalities and adds an extra "flair" to be compliant with both class based views and decorated function views.
         """
-        self._interceptors: Union[List["Interceptor"], "Void"] = Void
+        self._interceptors: Union[List["Interceptor"], "VoidType"] = Void
 
         self.handler = handler
         self.dependencies = dependencies or {}
-        self.interceptors = interceptors or []
-        self.permissions = permissions or []
+        self.interceptors: Sequence["Interceptor"] = interceptors or []
+        self.permissions: Sequence["Permission"] = permissions or []
         self.middleware = middleware or []
         self.exception_handlers = exception_handlers or {}
         self.response_class = None
         self.response_cookies = None
         self.response_headers = None
         self.deprecated = deprecated
         self.parent = parent
@@ -112,15 +113,15 @@
         Handles the interception of messages and calls from the API.
         """
         if self.get_interceptors():
             await self.intercept(scope, receive, send)
 
         await self.handler.handle(scope, receive, send)
 
-    def generate_operation_id(self):
+    def generate_operation_id(self) -> str:
         """
         Generates an unique operation if for the handler
         """
         operation_id = self.name + self.handler.path_format
         operation_id = re.sub(r"\W", "_", operation_id)
         methods = list(self.handler.methods)
         operation_id = f"{operation_id}_{methods[0].lower()}"
@@ -141,52 +142,53 @@
         "parent",
     )
 
     def __init__(
         self,
         path: Optional[str] = None,
         *,
-        handler: Union[Type["WebSocketHandler"], Type["APIView"], Type[Callable]],
+        handler: Union["WebSocketHandler", APIView],
         name: Optional[str] = None,
         parent: Optional["ParentType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        middleware: Optional[List["Middleware"]] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
+        middleware: Optional[Sequence["Middleware"]] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         interceptors: Optional[List["Interceptor"]] = None,
         permissions: Optional[List["Permission"]] = None,
     ) -> None:
         if not path:
             path = "/"
         if is_class_and_subclass(handler, APIView):
-            handler = handler(parent=self)
+            handler = handler(parent=self)  # type: ignore
         self.path = clean_path(path + handler.path)
 
         if not name:
             if not isinstance(handler, APIView):
                 name = clean_string(handler.fn.__name__)
             else:
                 name = clean_string(handler.__class__.__name__)
 
         super().__init__(
             path=self.path,
-            endpoint=handler,
+            endpoint=cast("Callable", handler),
             name=name,
         )
         """
         A "bridge" to a handler and router mapping functionality.
         Since the default Starlette Route endpoint does not understand the Esmerald handlers,
         the Gateway bridges both functionalities and adds an extra "flair" to be compliant with both class based views and decorated function views.
         """
-        self._interceptors: Union[List["Interceptor"], "Void"] = Void
+        self._interceptors: Union[List["Interceptor"], "VoidType"] = Void
         self.handler = handler
         self.dependencies = dependencies or {}
         self.interceptors = interceptors or []
         self.permissions = permissions or []
         self.middleware = middleware or []
         self.exception_handlers = exception_handlers or {}
+        self.include_in_schema = False
         self.parent = parent
         (
             handler.path_regex,
             handler.path_format,
             handler.param_convertors,
         ) = compile_path(self.path)
```

### Comparing `esmerald-1.2.5/esmerald/routing/handlers.py` & `esmerald-1.3.0/esmerald/routing/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-from enum import Enum
-from typing import TYPE_CHECKING, Dict, List, Optional, Type, Union
+from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Type, Union
 
 from starlette import status
 
 from esmerald.enums import HttpMethod, MediaType
 from esmerald.exceptions import HTTPException, ImproperlyConfigured
 from esmerald.openapi.datastructures import ResponseSpecification
 from esmerald.permissions.types import Permission
 from esmerald.routing.router import HTTPHandler, WebSocketHandler
 from esmerald.types import (
     BackgroundTaskType,
     Dependencies,
-    ExceptionHandler,
-    ExceptionHandlers,
-    HTTPMethod,
+    ExceptionHandlerMap,
     Middleware,
     ResponseCookies,
     ResponseHeaders,
     ResponseType,
 )
 from esmerald.utils.constants import AVAILABLE_METHODS
 
@@ -37,22 +34,22 @@
         description: Optional[str] = None,
         status_code: Optional[int] = status.HTTP_200_OK,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[ExceptionHandlers] = None,
+        exception_handlers: Optional[ExceptionHandlerMap] = None,
         permissions: Optional[List[Permission]] = None,
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
         responses: Optional[Dict[int, ResponseSpecification]] = None,
     ) -> None:
@@ -93,22 +90,22 @@
         description: Optional[str] = None,
         status_code: Optional[int] = status.HTTP_200_OK,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[ExceptionHandlers] = None,
+        exception_handlers: Optional[ExceptionHandlerMap] = None,
         permissions: Optional[List[Permission]] = None,
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
         responses: Optional[Dict[int, ResponseSpecification]] = None,
     ) -> None:
@@ -149,22 +146,22 @@
         description: Optional[str] = None,
         status_code: Optional[int] = status.HTTP_200_OK,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[ExceptionHandlers] = None,
+        exception_handlers: Optional[ExceptionHandlerMap] = None,
         permissions: Optional[List[Permission]] = None,
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
         responses: Optional[Dict[int, ResponseSpecification]] = None,
     ) -> None:
@@ -205,22 +202,22 @@
         description: Optional[str] = None,
         status_code: Optional[int] = status.HTTP_200_OK,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[ExceptionHandlers] = None,
+        exception_handlers: Optional[ExceptionHandlerMap] = None,
         permissions: Optional[List[Permission]] = None,
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
         responses: Optional[Dict[int, ResponseSpecification]] = None,
     ) -> None:
@@ -261,22 +258,22 @@
         description: Optional[str] = None,
         status_code: Optional[int] = status.HTTP_201_CREATED,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[ExceptionHandlers] = None,
+        exception_handlers: Optional[ExceptionHandlerMap] = None,
         permissions: Optional[List[Permission]] = None,
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
         responses: Optional[Dict[int, ResponseSpecification]] = None,
     ) -> None:
@@ -317,22 +314,22 @@
         description: Optional[str] = None,
         status_code: Optional[int] = status.HTTP_200_OK,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[ExceptionHandlers] = None,
+        exception_handlers: Optional[ExceptionHandlerMap] = None,
         permissions: Optional[List[Permission]] = None,
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
         responses: Optional[Dict[int, ResponseSpecification]] = None,
     ) -> None:
@@ -373,22 +370,22 @@
         description: Optional[str] = None,
         status_code: Optional[int] = status.HTTP_200_OK,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[ExceptionHandlers] = None,
+        exception_handlers: Optional[ExceptionHandlerMap] = None,
         permissions: Optional[List[Permission]] = None,
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
         responses: Optional[Dict[int, ResponseSpecification]] = None,
     ) -> None:
@@ -429,22 +426,22 @@
         description: Optional[str] = None,
         status_code: Optional[int] = status.HTTP_204_NO_CONTENT,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[ExceptionHandlers] = None,
+        exception_handlers: Optional[ExceptionHandlerMap] = None,
         permissions: Optional[List[Permission]] = None,
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
         responses: Optional[Dict[int, ResponseSpecification]] = None,
     ) -> None:
@@ -477,31 +474,31 @@
 
 
 class route(HTTPHandler):
     def __init__(
         self,
         path: Optional[str] = None,
         *,
-        methods: List["HTTPMethod"] = None,
+        methods: List[str] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
         status_code: Optional[int] = status.HTTP_200_OK,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[ExceptionHandlers] = None,
+        exception_handlers: Optional[ExceptionHandlerMap] = None,
         permissions: Optional[List[Permission]] = None,
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
         responses: Optional[Dict[int, ResponseSpecification]] = None,
     ) -> None:
@@ -549,18 +546,18 @@
             responses=responses,
         )
 
 
 class websocket(WebSocketHandler):
     def __init__(
         self,
-        path: Union[Optional[str], Optional[List[str]]] = None,
+        path: Optional[str] = None,
         *,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[Dict[Union[int, Type[Exception]], "ExceptionHandler"]] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         permissions: Optional[List["Permission"]] = None,
         middleware: Optional[List["Middleware"]] = None,
     ):
         super().__init__(
             path=path,
             dependencies=dependencies,
             exception_handlers=exception_handlers,
```

### Comparing `esmerald-1.2.5/esmerald/routing/router.py` & `esmerald-1.3.0/esmerald/routing/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 import inspect
 from copy import copy
-from enum import Enum, IntEnum
+from enum import IntEnum
 from inspect import Signature
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
+    Mapping,
     NoReturn,
     Optional,
+    Sequence,
     Set,
     Tuple,
     Type,
     Union,
     cast,
 )
 
 from starlette import status
+from starlette.datastructures import URLPath
 from starlette.middleware import Middleware as StarletteMiddleware
 from starlette.requests import HTTPConnection
 from starlette.responses import JSONResponse
 from starlette.responses import Response as StarletteResponse
 from starlette.routing import BaseRoute as StarletteBaseRoute
 from starlette.routing import Host, Mount, NoMatchFound
 from starlette.routing import Route as StarletteRoute
 from starlette.routing import Router as StarletteRouter
 from starlette.routing import WebSocketRoute as StarletteWebSocketRoute
 from starlette.routing import compile_path
 from starlette.types import ASGIApp, Lifespan, Receive, Scope, Send
+from typing_extensions import Self
 
 from esmerald.conf import settings
-from esmerald.datastructures import File, Redirect, URLPath
+from esmerald.core.urls import include
+from esmerald.datastructures import File, Redirect
 from esmerald.enums import HttpMethod, MediaType
 from esmerald.exceptions import (
     ImproperlyConfigured,
     MethodNotAllowed,
     NotFound,
     ValidationErrorException,
 )
-from esmerald.injector import Inject
 from esmerald.interceptors.types import Interceptor
 from esmerald.openapi.datastructures import ResponseSpecification
 from esmerald.requests import Request
 from esmerald.responses import Response
 from esmerald.routing.base import BaseHandlerMixin
 from esmerald.routing.events import handle_lifespan_events
 from esmerald.routing.gateways import Gateway, WebSocketGateway
 from esmerald.routing.views import APIView
 from esmerald.transformers.datastructures import EsmeraldSignature as SignatureModel
 from esmerald.transformers.model import TransformerModel
 from esmerald.transformers.utils import get_signature
 from esmerald.typing import Void, VoidType
-from esmerald.urls import include
 from esmerald.utils.constants import DATA, REDIRECT_STATUS_CODES, REQUEST, SOCKET
 from esmerald.utils.helpers import is_async_callable, is_class_and_subclass
 from esmerald.utils.url import clean_path
 from esmerald.websockets import WebSocket, WebSocketClose
 
 if TYPE_CHECKING:
     from openapi_schemas_pydantic.v3_1_0 import SecurityRequirement
@@ -66,31 +69,28 @@
     from esmerald.applications import Esmerald
     from esmerald.exceptions import HTTPException
     from esmerald.permissions.types import Permission
     from esmerald.types import (
         APIGateHandler,
         AsyncAnyCallable,
         BackgroundTaskType,
-        CoroutineHandler,
         Dependencies,
-        ExceptionHandler,
-        ExceptionHandlers,
-        HTTPMethod,
+        ExceptionHandlerMap,
         LifeSpanHandler,
         Middleware,
         ParentType,
         ResponseCookies,
         ResponseHeaders,
         ResponseType,
         RouteParent,
     )
 
 
 class Parent:
-    def create_signature_models(self, route: "RouteParent"):
+    def create_signature_models(self, route: "RouteParent") -> None:
         """
         Creates the signature models for the given routes.
 
         Args:
             route: The route for the signature model to be created.
         """
         if isinstance(route, (Include, Host)):
@@ -107,38 +107,39 @@
                 route.handler.create_signature_model()
 
         if isinstance(route, WebSocketGateway):
             route.handler.create_signature_model(is_websocket=True)
 
     def validate_root_route_parent(
         self,
-        value: Union["Router", "Include", "ASGIApp", "Gateway", "WebSocketGateway"],
+        value: Union["Router", "Include", "Gateway", "WebSocketGateway"],
         override: bool = False,
-    ):
+    ) -> None:
         """
         Handles everything parent from the root. When in the root, the parent must be setup.
         Appends the route path if exists.
         """
         # Getting the value of the router for the path
         value.path = clean_path(self.path + getattr(value, "path", "/"))
         if isinstance(value, (Include, Gateway, WebSocketGateway)):
             if not value.parent and not override:
-                value.parent = self
+                value.parent = cast("Union[Router, Include, Gateway, WebSocketGateway]", self)
 
         if isinstance(value, (Gateway, WebSocketGateway)):
             if not is_class_and_subclass(value.handler, APIView) and not isinstance(
                 value.handler, APIView
             ):
                 if not value.handler.parent:
                     value.handler.parent = value
             else:
                 if not value.handler.parent:
-                    value(parent=self)
+                    value(parent=self)  # type: ignore
 
-                route_handlers = value.handler.get_route_handlers()
+                handler: APIView = cast("APIView", value.handler)
+                route_handlers = handler.get_route_handlers()
                 for route_handler in route_handlers:
                     gateway = (
                         Gateway
                         if not isinstance(route_handler, WebSocketHandler)
                         else WebSocketGateway
                     )
 
@@ -183,33 +184,33 @@
         "security",
     )
 
     def __init__(
         self,
         path: Optional[str] = None,
         app: Optional["Esmerald"] = None,
-        parent: Optional["Router"] = None,
-        on_shutdown: Optional[List["LifeSpanHandler"]] = None,
-        on_startup: Optional[List["LifeSpanHandler"]] = None,
+        parent: Optional["ParentType"] = None,
+        on_shutdown: Optional[Sequence["LifeSpanHandler"]] = None,
+        on_startup: Optional[Sequence["LifeSpanHandler"]] = None,
         redirect_slashes: bool = True,
         default: Optional["ASGIApp"] = None,
-        routes: Optional[List[Union["APIGateHandler", "Include"]]] = None,
+        routes: Optional[Sequence[Union["APIGateHandler", "Include"]]] = None,
         name: Optional[str] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
-        interceptors: Optional[List["Interceptor"]] = None,
-        permissions: Optional[List["Permission"]] = None,
-        middleware: Optional[List["Middleware"]] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
+        interceptors: Optional[Sequence["Interceptor"]] = None,
+        permissions: Optional[Sequence["Permission"]] = None,
+        middleware: Optional[Sequence["Middleware"]] = None,
         response_class: Optional["ResponseType"] = None,
         response_cookies: Optional["ResponseCookies"] = None,
         response_headers: Optional["ResponseHeaders"] = None,
         lifespan: Optional[Lifespan[Any]] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[Sequence["SecurityRequirement"]] = None,
     ):
         self.app = app
         if not path:
             path = "/"
         else:
             assert path.startswith("/"), "A path prefix must start with '/'"
             assert not path.endswith(
@@ -226,15 +227,14 @@
                     StarletteBaseRoute,
                     Mount,
                     Host,
                     Router,
                 ),
             ):
                 raise ImproperlyConfigured(f"The route {route} must be of type Gateway or Include")
-        routes = routes or []
 
         assert lifespan is None or (
             on_startup is None and on_shutdown is None
         ), "Use either 'lifespan' or 'on_startup'/'on_shutdown', not both."
 
         self.esmerald_lifespan = handle_lifespan_events(
             on_startup=on_startup, on_shutdown=on_shutdown, lifespan=lifespan
@@ -242,24 +242,25 @@
 
         super().__init__(
             redirect_slashes=redirect_slashes,
             routes=routes,
             default=default,
             lifespan=self.esmerald_lifespan,
         )
+
         self.path = path
         self.on_startup = [] if on_startup is None else list(on_startup)
         self.on_shutdown = [] if on_shutdown is None else list(on_shutdown)
-        self.parent: Optional["Router"] = parent or self.app
+        self.parent: Optional["ParentType"] = parent or self.app
         self.dependencies = dependencies or {}
         self.exception_handlers = exception_handlers or {}
-        self.interceptors = interceptors or []
-        self.permissions = permissions or []
+        self.interceptors: Sequence["Interceptor"] = interceptors or []
+        self.permissions: Sequence["Permission"] = permissions or []
+        self.routes: Any = routes or []
         self.middleware = middleware or []
-        self.routes = routes
         self.tags = tags or []
         self.name = name
         self.response_class = response_class
         self.response_cookies = response_cookies or []
         self.response_headers = response_headers or {}
         self.deprecated = deprecated
         self.security = security or []
@@ -269,30 +270,33 @@
             self.validate_root_route_parent(route)
 
         for route in self.routes or []:
             self.create_signature_models(route)
 
         self.activate()
 
-    def reorder_routes(self):
+    def reorder_routes(self) -> List[Sequence[Union["APIGateHandler", "Include"]]]:
         return sorted(
             self.routes,
             key=lambda router: router.path != "" and router.path != "/",
             reverse=True,
         )
 
-    def activate(self):
+    def activate(self) -> None:
         self.routes = self.reorder_routes()
 
-    def add_apiview(self, value: Type["APIView"]):
+    def add_apiview(self, value: Union["Gateway", "WebSocketGateway"]) -> None:
+        """Adds a Gateway/WebSocketGateway coming containing the handler of type APIView.
+        Generates the signature model for it and sorts the routing list.
+        """
         routes = []
         if not value.handler.parent:
-            value(parent=self)
+            value.handler(parent=self)  # type: ignore
 
-        route_handlers = value.handler.get_route_handlers()
+        route_handlers: List[Union[HTTPHandler, WebSocketHandler]] = value.handler.get_route_handlers()  # type: ignore
         for route_handler in route_handlers:
             gateway = (
                 Gateway if not isinstance(route_handler, WebSocketHandler) else WebSocketGateway
             )
             gate = gateway(
                 path=value.path,
                 handler=route_handler,
@@ -307,17 +311,17 @@
         for route in routes or []:
             self.create_signature_models(route)
         self.activate()
 
     def add_route(
         self,
         path: str,
-        handler: Type["HTTPHandler"],
+        handler: "HTTPHandler",
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         interceptors: Optional[List["Interceptor"]] = None,
         permissions: Optional[List["Permission"]] = None,
         middleware: Optional[List["Middleware"]] = None,
         name: Optional[str] = None,
         include_in_schema: bool = True,
         deprecated: Optional[bool] = None,
     ) -> None:
@@ -332,34 +336,34 @@
             )
         gateway = Gateway(
             path=self.path + path,
             handler=handler,
             name=name,
             include_in_schema=include_in_schema,
             dependencies=dependencies,
-            exception_handlers=exception_handlers,
+            exception_handlers=cast("ExceptionHandlerMap", exception_handlers),
             interceptors=interceptors,
             permissions=permissions,
             middleware=middleware,
             deprecated=deprecated,
         )
         self.validate_root_route_parent(gateway)
         self.create_signature_models(gateway)
         self.routes.append(gateway)
 
     def add_websocket_route(
         self,
         path: str,
-        handler: Type["WebSocketHandler"],
+        handler: "WebSocketHandler",
         name: Optional[str] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         interceptors: Optional[List["Interceptor"]] = None,
         permissions: Optional[List["Permission"]] = None,
-        middleware: Optional[List["Middleware"]] = None,
+        middleware: Optional[Sequence["Middleware"]] = None,
     ) -> None:
         if not isinstance(handler, WebSocketHandler):
             raise ImproperlyConfigured(
                 f"handler must be a instance of WebSocketHandler and not {handler.__class__.__name__}. "
                 "Example: websocket()."
             )
         websocket_gateway = WebSocketGateway(
@@ -395,23 +399,24 @@
         else:
             response = JSONResponse({"detail": "Not Found"}, status_code=status.HTTP_404_NOT_FOUND)
         await response(scope, receive, send)
 
     def url_path_for(self, name: str, **path_params: Any) -> URLPath:
         for route in self.routes or []:
             try:
-                return route.url_path_for(name, **path_params)
+                return cast("URLPath", route.url_path_for(name, **path_params))
             except NoMatchFound:
-                pass
+                ...
 
             if isinstance(route, (Gateway, WebSocketGateway)):
+                handler = cast("Union[HTTPHandler, WebSocketHandler]", route.handler)
                 try:
-                    return route.handler.url_path_for(name, **path_params)
+                    return handler.url_path_for(name, **path_params)
                 except NoMatchFound:
-                    pass
+                    ...
 
         raise NoMatchFound(name, path_params)
 
     def add_event_handler(self, event_type: str, func: Callable) -> None:  # pragma: no cover
         assert event_type in ("startup", "shutdown")
 
         if event_type == "startup":
@@ -433,14 +438,15 @@
         "path",
         "_permissions",
         "_dependencies",
         "_response_handler",
         "methods",
         "status_code",
         "content_encoding",
+        "media_type",
         "content_media_type",
         "summary",
         "description",
         "include_in_schema",
         "dependencies",
         "exception_handlers",
         "permissions",
@@ -455,48 +461,49 @@
         "operation_id",
         "raise_exceptions",
     )
 
     def __init__(
         self,
         path: Optional[str] = None,
-        endpoint: Callable[..., "CoroutineHandler"] = None,
+        endpoint: Callable[..., Any] = None,
         *,
-        methods: Optional[List["HTTPMethod"]] = None,
+        methods: Optional[Sequence[str]] = None,
         status_code: Optional[int] = None,
         content_encoding: Optional[str] = None,
         content_media_type: Optional[str] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
         include_in_schema: bool = True,
         background: Optional["BackgroundTaskType"] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional["ExceptionHandlers"] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         permissions: Optional[List["Permission"]] = None,
         middleware: Optional[List["Middleware"]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional["ResponseType"] = None,
         response_cookies: Optional["ResponseCookies"] = None,
         response_headers: Optional["ResponseHeaders"] = None,
-        tags: Optional[List[Union[str, Enum]]] = None,
+        tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         response_description: Optional[str] = "Successful Response",
         responses: Optional[Dict[int, ResponseSpecification]] = None,
         security: Optional[List["SecurityRequirement"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
     ) -> None:
         if not path:
             path = "/"
         super().__init__(path=path, endpoint=endpoint, include_in_schema=include_in_schema)
         """
         Handles the "handler" or "apiview" of the platform. A handler can be any get, put, patch, post, delete or route.
         """
         self._permissions: Union[List["Permission"], "VoidType"] = Void
-        self._dependencies: Union[Dict[str, Inject], "VoidType"] = Void
+        self._dependencies: "Dependencies" = {}
+
         self._response_handler: Union[
             "Callable[[Any], Awaitable[StarletteResponse]]", VoidType
         ] = Void
 
         self.parent: "ParentType" = None
         self.path = path
         self.endpoint = endpoint
@@ -521,15 +528,15 @@
         self.methods: Set[str] = {HttpMethod[method].value for method in methods}
 
         if isinstance(status_code, IntEnum):
             status_code = int(status_code)
         self.status_code = status_code
 
         self.exception_handlers = exception_handlers or {}
-        self.dependencies = dependencies or {}
+        self.dependencies: "Dependencies" = dependencies or {}
         self.description = description or inspect.cleandoc(self.endpoint.__doc__ or "")
         self.permissions = list(permissions) if permissions else []
         self.middleware = list(middleware) if middleware else []
         self.description = self.description.split("\f")[0]
         self.media_type = media_type
         self.response_class = response_class
         self.response_cookies = response_cookies
@@ -541,15 +548,15 @@
         self.responses = responses or {}
         self.content_encoding = content_encoding
         self.content_media_type = content_media_type
         self.raise_exceptions = raise_exceptions
 
         self.fn: Optional["AnyCallable"] = None
         self.app: Optional["ASGIApp"] = None
-        self.route_map: Dict["HTTPMethod" : Tuple["HTTPHandler", "TransformerModel"]] = {}
+        self.route_map: Dict[str, Tuple["HTTPHandler", "TransformerModel"]] = {}
         self.path_regex, self.path_format, self.param_convertors = compile_path(path)
 
     @property
     def http_methods(self) -> List[str]:
         """
         Converts the methods set into a list of methods.
         """
@@ -563,23 +570,23 @@
         a MethodNotAllowed if otherwise.
         """
         for method in methods:
             if method not in self.http_methods:
                 raise MethodNotAllowed(detail=f"Method {method.upper()} not allowed.")
 
     @property
-    def allow_header(self):
+    def allow_header(self) -> Mapping[str, str]:
         """
         Default allow header to be injected in the Response and Starlette Response type
         handlers.
         """
         return {"allow": str(self.methods)}
 
     @property
-    def permission_names(self):
+    def permission_names(self) -> Sequence[str]:
         """
         List of permissions for the route. This is used for OpenAPI Spec purposes only.
         """
         return [permission.__name__ for permission in self.permissions]
 
     def get_response_class(self) -> Type["Response"]:
         """
@@ -592,15 +599,15 @@
                 response_class = layer.response_class
         return response_class
 
     def get_response_headers(self) -> "ResponseHeaders":
         """
         Returns all header parameters in the scope of the handler function.
         """
-        resolved_response_headers = {}
+        resolved_response_headers: "ResponseHeaders" = {}
         for layer in self.parent_levels:
             resolved_response_headers.update(layer.response_headers or {})
         return resolved_response_headers
 
     def get_response_cookies(self) -> "ResponseCookies":
         """Returns a list of Cookie instances. Filters the list to ensure each
         cookie key is unique.
@@ -633,15 +640,15 @@
             scope=scope,
             request=request,
             route=route_handler,
             parameter_model=parameter_model,
         )
         await response(scope, receive, send)
 
-    def __call__(self, fn: "AnyCallable") -> "ASGIApp":
+    def __call__(self, fn: "AnyCallable") -> "HTTPHandler":
         self.fn = fn
         self.endpoint = fn
         self.validate_handler()
         return self
 
     def check_handler_function(self) -> None:
         """Validates the route handler function once it's set by inspecting its
@@ -674,15 +681,15 @@
         if not settings.enable_sync_handlers:
             fn = cast("AnyCallable", self.fn)
             if not is_async_callable(fn):
                 raise ImproperlyConfigured(
                     "Functions decorated with 'route, websocket, get, patch, put, post and delete' must be async functions"
                 )
 
-    def validate_annotations(self):
+    def validate_annotations(self) -> None:
         """
         Validate annotations of the handlers.
         """
         return_annotation = self.signature.return_annotation
 
         if return_annotation is Signature.empty:
             raise ImproperlyConfigured(
@@ -707,32 +714,32 @@
             )
         if is_class_and_subclass(return_annotation, File) and self.media_type in [
             MediaType.JSON,
             MediaType.HTML,
         ]:
             self.media_type = MediaType.TEXT
 
-    def validate_reserved_kwargs(self):
+    def validate_reserved_kwargs(self) -> None:
         """
         Validates if special words are in the signature.
         """
         if DATA in self.signature.parameters and "GET" in self.methods:
             raise ImproperlyConfigured("'data' argument is unsupported for 'GET' request handlers")
 
         if SOCKET in self.signature.parameters:
             raise ImproperlyConfigured("The 'socket' argument is not supported with http handlers")
 
-    def validate_handler(self):
+    def validate_handler(self) -> None:
         self.check_handler_function()
         self.validate_annotations()
         self.validate_reserved_kwargs()
 
     async def to_response(self, app: "Esmerald", data: Any) -> StarletteResponse:
         response_handler = self.get_response_handler()
-        return await response_handler(app=app, data=data)
+        return await response_handler(app=app, data=data)  # type: ignore[call-arg]
 
 
 class WebSocketHandler(BaseHandlerMixin, StarletteWebSocketRoute):
     """
     Websocket handler object representation.
     """
 
@@ -743,47 +750,50 @@
         "permissions",
         "middleware",
         "parent",
     )
 
     def __init__(
         self,
-        path: Union[Optional[str], Optional[List[str]]] = None,
+        path: Optional[str] = None,
         *,
-        endpoint: Callable[..., "CoroutineHandler"] = None,
+        endpoint: Callable[..., Any] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[Dict[Union[int, Type[Exception]], "ExceptionHandler"]] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
         permissions: Optional[List["Permission"]] = None,
         middleware: Optional[List["Middleware"]] = None,
     ):
         if not path:
             path = "/"
         super().__init__(path=path, endpoint=endpoint)
         self._permissions: Union[List["Permission"], "VoidType"] = Void
-        self._dependencies: Union[Dict[str, Inject], "VoidType"] = Void
+        self._dependencies: "Dependencies" = {}
         self._response_handler: Union[
             "Callable[[Any], Awaitable[StarletteResponse]]", VoidType
         ] = Void
 
         self.endpoint = endpoint
         self.parent: "ParentType" = None
         self.dependencies = dependencies
         self.exception_handlers = exception_handlers
         self.permissions = permissions
         self.middleware = middleware
         self.signature_model: Optional[Type["SignatureModel"]] = None
         self.websocket_parameter_model: Optional["TransformerModel"] = None
+        self.include_in_schema = None
+        self.fn: Optional["AnyCallable"] = None
+        self.tags: Sequence[str] = []
 
-    def __call__(self, fn: "AnyCallable") -> "ASGIApp":
+    def __call__(self, fn: "AnyCallable") -> "WebSocketHandler":
         self.fn = fn
         self.endpoint = fn
         self.validate_websocket_handler_function()
         return self
 
-    def validate_reserved_words(self, signature: "Signature"):
+    def validate_reserved_words(self, signature: "Signature") -> None:
         """
         Validates if special words are in the signature.
         """
         if signature.return_annotation is not None:
             raise ImproperlyConfigured("Websocket functions should return 'None'.")
 
         unsupported_kwargs = [REQUEST, DATA]
@@ -876,26 +886,26 @@
     )
 
     def __init__(
         self,
         path: Optional[str] = None,
         app: Optional["ASGIApp"] = None,
         name: Optional[str] = None,
-        routes: Optional[List[StarletteBaseRoute]] = None,
+        routes: Optional[Sequence[Union["APIGateHandler", "Include"]]] = None,
         namespace: Optional[str] = None,
         pattern: Optional[str] = None,
-        parent: Optional["Router"] = None,
+        parent: Optional[Union["Self", "Router"]] = None,
         dependencies: Optional["Dependencies"] = None,
-        exception_handlers: Optional[Dict[Union[int, Type[Exception]], "ExceptionHandler"]] = None,
-        interceptors: Optional[List["Interceptor"]] = None,
-        permissions: Optional[List["Permission"]] = None,
+        exception_handlers: Optional["ExceptionHandlerMap"] = None,
+        interceptors: Optional[Sequence["Interceptor"]] = None,
+        permissions: Optional[Sequence["Permission"]] = None,
         middleware: Optional[List["Middleware"]] = None,
         include_in_schema: Optional[bool] = True,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[Sequence["SecurityRequirement"]] = None,
     ) -> None:
         self.path = path
         if not path:
             self.path = "/"
 
         if namespace and routes:
             raise ImproperlyConfigured("It can only be namespace or routes, not both.")
@@ -906,71 +916,76 @@
         if pattern and not isinstance(pattern, str):
             raise ImproperlyConfigured("Pattern must be a string. Example: 'route_patterns'.")
 
         if pattern and routes:
             raise ImproperlyConfigured("Pattern must be used only with namespace.")
 
         if namespace:
-            routes: List["APIGateHandler"] = include(namespace, pattern)
+            routes = include(namespace, pattern)
 
         self.app = app
         self.name = name
         self.namespace = namespace
         self.pattern = pattern
         self.include_in_schema = include_in_schema
         self.dependencies = dependencies or {}
-        self.interceptors = interceptors or []
-        self.permissions = permissions or []
+        self.interceptors: Sequence["Interceptor"] = interceptors or []
+        self.permissions: Sequence["Permission"] = permissions or []
         self.middleware = middleware or []
         self.exception_handlers = exception_handlers or {}
         self.deprecated = deprecated
         self.response_class = None
         self.response_cookies = None
         self.response_headers = None
         self.parent = parent
         self.security = security or []
 
         if routes:
             routes = self.resolve_route_path_handler(routes)
 
         # Build the middleware from the routes
-        routes_middleware = []
+        routes_middleware: List["Middleware"] = []
         for route in routes or []:
-            routes_middleware = self.build_routes_middleware(route)
+            routes_middleware = cast("List[Middleware]", self.build_routes_middleware(route))
 
         # Add the middleware to the include
         self.middleware += routes_middleware
-        include_middleware = []
+        include_middleware: Sequence["Middleware"] = []
 
-        if self.middleware:
-            for middleware in self.middleware:
-                if isinstance(middleware, StarletteMiddleware):
-                    include_middleware.append(middleware)
-                else:
-                    include_middleware.append(StarletteMiddleware(middleware))
+        for _middleware in self.middleware:
+            if isinstance(_middleware, StarletteMiddleware):
+                include_middleware.append(_middleware)  # type: ignore
+            else:
+                include_middleware.append(
+                    StarletteMiddleware(cast("Type[StarletteMiddleware]", _middleware))
+                )
 
         app = self.resolve_app_parent(app=app)
 
         super().__init__(
-            self.path, app=self.app, routes=routes, name=name, middleware=include_middleware
+            self.path,
+            app=self.app,
+            routes=routes,
+            name=name,
+            middleware=cast("Sequence[StarletteMiddleware]", include_middleware),
         )
 
-    def resolve_app_parent(self, app: Optional[Any]):
+    def resolve_app_parent(self, app: Optional[Any]) -> Optional[Any]:
         """
         Resolves the owner of ChildEsmerald or Esmerald iself.
         """
         from esmerald import ChildEsmerald, Esmerald
 
         if app is not None and isinstance(app, (Esmerald, ChildEsmerald)):
             app.parent = self
         return app
 
     def build_routes_middleware(
-        self, route: "RouteParent", middlewares: Optional[List["Middleware"]] = None
-    ):
+        self, route: "RouteParent", middlewares: Optional[Sequence["Middleware"]] = None
+    ) -> Sequence["Middleware"]:
         """
         Builds the middleware stack from the top to the bottom of the routes.
         """
         from esmerald import ChildEsmerald, Esmerald
 
         if not middlewares:
             middlewares = []
@@ -983,15 +998,17 @@
         if isinstance(route, (Gateway, WebSocketGateway)):
             middlewares.extend(route.middleware)
             if route.handler.middleware:
                 middlewares.extend(route.handler.middleware)
 
         return middlewares
 
-    def resolve_route_path_handler(self, routes: List[StarletteBaseRoute]):
+    def resolve_route_path_handler(
+        self, routes: Sequence[Union["APIGateHandler", "Include"]]
+    ) -> List[Union["Gateway", "WebSocketGateway", "Include"]]:
         """
         Make sure the paths are properly configured from the handler endpoint.
         The handler can be a Starlette function, an APIView or a HTTPHandler.
 
         Mount() has a limitation of not allowing nested Mount().
 
         Example:
@@ -1031,56 +1048,58 @@
 
             route_patterns = [
                 Gateway(path='/last-example', handler=another_endpoint, name='example')
                 ...
             ]
 
         """
-        routing = []
+        routing: List[Union[Gateway, WebSocketGateway, Include]] = []
 
         for route in routes:
-            if not isinstance(route, (Include, Gateway, WebSocketGateway, Mount)):
+            if not isinstance(route, (Include, Gateway, WebSocketGateway)):
                 raise ImproperlyConfigured("The route must be of type Gateway or Include")
 
             route.parent = self
             if isinstance(route, Include):
                 routing.append(route)
-            else:
-                if isinstance(route.handler, (HTTPHandler, WebSocketHandler)):
-                    route.handler.parent = route
-                    routing.append(route)
-                    continue
-
-                if is_class_and_subclass(route.handler, APIView) or isinstance(
-                    route.handler, APIView
-                ):
-                    if not route.handler.parent:
-                        route.handler = route.handler(parent=self)
-                    route_handlers = route.handler.get_route_handlers()
-
-                    for route_handler in route_handlers:
-                        gateway = (
-                            Gateway
-                            if not isinstance(route_handler, WebSocketHandler)
-                            else WebSocketGateway
-                        )
+                continue
 
-                        gate = gateway(
-                            path=route.path,
-                            handler=route_handler,
-                            name=route_handler.fn.__name__,
-                            middleware=route.middleware,
-                            interceptors=self.interceptors,
-                            permissions=route.permissions,
-                            exception_handlers=route.exception_handlers,
-                        )
+            if isinstance(route.handler, (HTTPHandler, WebSocketHandler)):
+                route.handler.parent = route
+                routing.append(route)
+                continue
+
+            if is_class_and_subclass(route.handler, APIView) or isinstance(route.handler, APIView):
+                if not route.handler.parent:
+                    route.handler = route.handler(parent=self)  # type: ignore
+
+                route_handlers: List[
+                    Union[HTTPHandler, WebSocketHandler]
+                ] = route.handler.get_route_handlers()  # type: ignore[union-attr]
 
-                        if isinstance(gate, Gateway):
-                            include_in_schema = (
-                                route.include_in_schema
-                                if route.include_in_schema is not None
-                                else route_handler.include_in_schema
-                            )
-                            gate.include_in_schema = include_in_schema
+                for route_handler in route_handlers:
+                    gateway = (
+                        Gateway
+                        if not isinstance(route_handler, WebSocketHandler)
+                        else WebSocketGateway
+                    )
+
+                    gate = gateway(
+                        path=route.path,
+                        handler=route_handler,
+                        name=route_handler.fn.__name__,
+                        middleware=route.middleware,
+                        interceptors=self.interceptors,
+                        permissions=route.permissions,
+                        exception_handlers=route.exception_handlers,
+                    )
+
+                    if isinstance(gate, Gateway):
+                        include_in_schema = (
+                            route.include_in_schema
+                            if route.include_in_schema is not None
+                            else route_handler.include_in_schema
+                        )
+                        gate.include_in_schema = include_in_schema
 
-                        routing.append(gate)
+                    routing.append(gate)
         return routing
```

### Comparing `esmerald-1.2.5/esmerald/routing/views.py` & `esmerald-1.3.0/esmerald/routing/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from copy import copy
-from typing import TYPE_CHECKING, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Tuple, Union, cast
 
 from starlette.routing import compile_path
+from starlette.types import Receive, Scope, Send
 
 from esmerald.utils.url import clean_path
 
 if TYPE_CHECKING:
+    from esmerald.interceptors.types import Interceptor
     from esmerald.permissions.types import Permission
-    from esmerald.routing.router import HTTPHandler, Router, WebSocketHandler
+    from esmerald.routing.gateways import Gateway, WebSocketGateway
+    from esmerald.routing.router import HTTPHandler, WebSocketHandler
+    from esmerald.transformers.model import TransformerModel
     from esmerald.types import (
         Dependencies,
-        ExceptionHandlers,
+        ExceptionHandlerMap,
         Middleware,
         ResponseCookies,
         ResponseHeaders,
         ResponseType,
     )
 
 
@@ -37,38 +41,44 @@
         "response_headers",
         "tags",
         "path_regex",
         "path_format",
         "param_convertors",
         "deprecated",
         "include_in_schema",
+        "route_map",
+        "operation_id",
+        "methods",
     )
 
     path: str
     dependencies: Optional["Dependencies"]
-    exception_handlers: Optional["ExceptionHandlers"]
+    exception_handlers: Optional["ExceptionHandlerMap"]
     permissions: Optional[List["Permission"]]
     middleware: Optional[List["Middleware"]]
-    parent: "Router"
+    parent: Union["Gateway", "WebSocketGateway"]
     response_class: Optional["ResponseType"]
     response_cookies: Optional["ResponseCookies"]
     response_headers: Optional["ResponseHeaders"]
     tags: Optional[List[str]]
     deprecated: Optional[bool]
     include_in_schema: Optional[bool]
 
-    def __init__(self, parent: "Router") -> None:
+    def __init__(self, parent: Union["Gateway", "WebSocketGateway"]) -> None:
         for key in self.__slots__:
             if not hasattr(self, key):
                 setattr(self, key, None)
 
         self.path = clean_path(self.path or "/")
         self.path_regex, self.path_format, self.param_convertors = compile_path(self.path)
         self.parent = parent
-        self.interceptors = []
+        self.interceptors: Sequence["Interceptor"] = []
+        self.route_map: Dict[str, Tuple["HTTPHandler", "TransformerModel"]] = {}
+        self.operation_id: Optional[str] = None
+        self.methods: List[str] = []
 
     def get_filtered_handler(self) -> List[str]:
         """
         Filters out the names of the functions that are not part of the handler itself.
         """
         from esmerald.routing.router import HTTPHandler, WebSocketHandler
 
@@ -115,26 +125,30 @@
             if self.tags or []:
                 for tag in reversed(self.tags):
                     route_handler.tags.insert(0, tag)
             route_handlers.append(route_handler)
 
         return route_handlers
 
-    def get_route_middleware(
-        self, handler: Union["HTTPHandler", "WebSocketHandler"]
-    ) -> List["Middleware"]:
+    def get_route_middleware(self, handler: Union["HTTPHandler", "WebSocketHandler"]) -> None:
         """
         Gets the list of extended middlewares for the handler starting from the last
         to the first by reversing the list
         """
         for middleware in reversed(self.middleware):
             handler.middleware.insert(0, middleware)
 
     def get_exception_handlers(
         self, handler: Union["HTTPHandler", "WebSocketHandler"]
-    ) -> "ExceptionHandlers":
+    ) -> "ExceptionHandlerMap":
         """
         Gets the dict of extended exception handlers for the handler starting from the last
         to the first by reversing the list
         """
         exception_handlers = {**self.exception_handlers, **handler.exception_handlers}
-        return exception_handlers
+        return cast("ExceptionHandlerMap", exception_handlers)
+
+    async def handle(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+        raise NotImplementedError("APIView object does not implement handle()")
+
+    def create_signature_model(self, is_websocket: bool = False) -> None:
+        raise NotImplementedError("APIView object does not implement create_signature_model()")
```

### Comparing `esmerald-1.2.5/esmerald/security/jwt/token.py` & `esmerald-1.3.0/esmerald/security/jwt/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, timezone
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from jose import JWSError, JWTError, jwt
 from jose.exceptions import JWSAlgorithmError, JWSSignatureError
 from pydantic import BaseModel, Field, constr, validator
 
 from esmerald.exceptions import ImproperlyConfigured
 from esmerald.security.utils import convert_time
@@ -12,15 +12,15 @@
 class Token(BaseModel):
     """
     Classic representation of a token via pydantic model.
     """
 
     exp: datetime
     iat: datetime = Field(default_factory=lambda: convert_time(datetime.now(timezone.utc)))
-    sub: constr(min_length=1)
+    sub: constr(min_length=1)  # type: ignore
     iss: Optional[str] = None
     aud: Optional[str] = None
     jti: Optional[str] = None
 
     @validator("exp", always=True)
     def validate_expiration(cls, date: datetime) -> datetime:
         """
@@ -35,15 +35,15 @@
     def validate_iat(cls, date: datetime) -> datetime:  # pylint: disable=no-self-argument
         """Ensures that the `Issued At` it's nt bigger than the current time."""
         date = convert_time(date)
         if date.timestamp() <= convert_time(datetime.now(timezone.utc)).timestamp():
             return date
         raise ValueError("iat must be a current or past time")
 
-    def encode(self, key: str, algorithm: str) -> str:
+    def encode(self, key: str, algorithm: str) -> Union[str, Any]:
         """
         Encodes the token into a proper str formatted and allows passing kwargs.
         """
         try:
             return jwt.encode(
                 claims=self.dict(exclude_none=True),
                 key=key,
```

### Comparing `esmerald-1.2.5/esmerald/template/jinja.py` & `esmerald-1.3.0/esmerald/template/jinja.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from os import PathLike
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, List, Union
 
 from esmerald.exceptions import MissingDependency, TemplateNotFound
 from esmerald.protocols.template import TemplateEngineProtocol
 
 if TYPE_CHECKING:
     from pydantic import DirectoryPath
@@ -19,29 +20,29 @@
     import jinja2
 
     if hasattr(jinja2, "pass_context"):
         pass_context = jinja2.pass_context
     else:  # pragma: nocover
         pass_context = jinja2.contextfunction  # type: ignore[attr-defined]
 except ImportError:  # pragma: nocover
-    jinja2 = None  # type: ignore
+    jinja2 = None
 
 
 class JinjaTemplateEngine(TemplateEngineProtocol[JinjaTemplate]):
     def __init__(
         self, directory: Union["DirectoryPath", List["DirectoryPath"]], **env_options: Any
     ) -> None:
         super().__init__(directory)
         self.env = self._create_environment(directory, **env_options)
 
     def _create_environment(
-        self, directory: Union[str, PathLike], **env_options: Any
-    ) -> "jinja2.Environment":
+        self, directory: Union[str, PathLike, List[Path]], **env_options: Any
+    ) -> "Environment":
         @pass_context
-        def url_for(context: dict, name: str, **path_params: Any) -> str:
+        def url_for(context: dict, name: str, **path_params: Any) -> Any:
             request = context["request"]
             return request.url_for(name, **path_params)
 
         loader = FileSystemLoader(directory)
         env_options.setdefault("loader", loader)
 
         env = Environment(autoescape=True, **env_options)
```

### Comparing `esmerald-1.2.5/esmerald/template/mako.py` & `esmerald-1.3.0/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/transformers/datastructures.py` & `esmerald-1.3.0/esmerald/transformers/datastructures.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 from esmerald.utils.helpers import is_optional_union
 from esmerald.websockets import WebSocket
 
 if TYPE_CHECKING:
     from pydantic.error_wrappers import ErrorDict
     from pydantic.typing import DictAny
 
-IntValError = Union[InternalServerError, ValidationError]
-
 
 class EsmeraldSignature(BaseModel):
     dependency_names: ClassVar[Set[str]]
     return_annotation: ClassVar[Any]
 
     class Config:
         arbitrary_types_allowed = True
@@ -42,15 +40,15 @@
             return values
         except ValidationError as e:
             raise cls.build_exception(connection, e) from e
 
     @classmethod
     def build_exception(
         cls, connection: Union[Request, WebSocket], exception: ValidationError
-    ) -> IntValError:
+    ) -> Union[InternalServerError, ValidationErrorException]:
         server_errors = []
         client_errors = []
 
         for err in exception.errors():
             if not cls.is_server_error(err):
                 client_errors.append(err)
             else:
```

### Comparing `esmerald-1.2.5/esmerald/transformers/helpers.py` & `esmerald-1.3.0/esmerald/transformers/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,16 @@
     ConstrainedFrozenSet,
     ConstrainedInt,
     ConstrainedList,
     ConstrainedSet,
     ConstrainedStr,
 )
 
-from esmerald.transformers.types import ConstrainedField
 
-
-def is_pydantic_constrained_field(value: Any) -> ConstrainedField:
+def is_pydantic_constrained_field(value: Any) -> Any:
     return inspect.isclass(value) and any(
         issubclass(value, _type)
         for _type in (
             ConstrainedBytes,
             ConstrainedDate,
             ConstrainedDecimal,
             ConstrainedFloat,
```

### Comparing `esmerald-1.2.5/esmerald/transformers/model.py` & `esmerald-1.3.0/esmerald/transformers/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Dict, Optional, Set, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, Mapping, Optional, Set, Tuple, Type, Union, cast
 
 from pydantic.fields import (
     SHAPE_DEQUE,
     SHAPE_FROZENSET,
     SHAPE_LIST,
     SHAPE_SEQUENCE,
     SHAPE_SET,
@@ -21,42 +21,41 @@
     ParamSetting,
     create_parameter_setting,
     get_request_params,
     get_signature,
     merge_sets,
 )
 from esmerald.utils.constants import RESERVED_KWARGS
-from esmerald.utils.pydantic import is_field_optional
+from esmerald.utils.pydantic.schema import is_field_optional
 
 if TYPE_CHECKING:
-    from pydantic.typing import DictAny
-
-    from esmerald.types import Dependencies, ReservedKwargs
+    from esmerald.types import Dependencies
     from esmerald.websockets import WebSocket
 
 
 MEDIA_TYPES = [EncodingType.MULTI_PART, EncodingType.URL_ENCODED]
+MappingUnion = Mapping[Union[int, str], Any]
 
 
 class TransformerModel(BaseModelExtra):
     class Config(BaseModelExtra.Config):
         arbitrary_types_allowed = True
 
     def __init__(
         self,
         cookies: Set[ParamSetting],
         dependencies: Set[Dependency],
         form_data: Optional[Tuple[EncodingType, ModelField]],
         headers: Set[ParamSetting],
         path_params: Set[ParamSetting],
         query_params: Set[ParamSetting],
-        reserved_kwargs: Set["ReservedKwargs"],
-        query_param_names: Set[str],
+        reserved_kwargs: Set[str],
+        query_param_names: Set[ParamSetting],
         is_optional: bool,
-        **kwargs: "DictAny",
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.cookies = cookies
         self.dependencies = dependencies
         self.form_data = form_data
         self.headers = headers
         self.path_params = path_params
@@ -227,22 +226,22 @@
         )
 
     @classmethod
     def update_parameters(
         cls,
         global_dependencies: "Dependencies",
         local_dependencies: Set["Dependency"],
-        path_params: "DictAny",
-        query_params: "DictAny",
-        cookies: "DictAny",
-        headers: "DictAny",
-        reserved_kwargs: "DictAny",
-        path_parameters: "DictAny",
-        form_data: "DictAny",
-    ) -> Tuple["DictAny", "DictAny", "DictAny", "DictAny", "DictAny"]:
+        path_params: Any,
+        query_params: Any,
+        cookies: Any,
+        headers: Any,
+        reserved_kwargs: Any,
+        path_parameters: Any,
+        form_data: Any,
+    ) -> Tuple[Any, Any, Any, Any, Any]:
         for dependency in local_dependencies:
             dependency_model = cls.create_signature(
                 signature_model=get_signature(dependency.inject),
                 dependencies=global_dependencies,
                 path_parameters=path_parameters,
             )
             path_params = merge_sets(path_params, dependency_model.path_params)
@@ -252,32 +251,40 @@
 
             if "data" in reserved_kwargs and "data" in dependency_model.reserved_kwargs:
                 cls.validate_data(form_data, dependency_model)
             reserved_kwargs.update(dependency_model.reserved_kwargs)
 
         return path_params, query_params, cookies, headers, reserved_kwargs
 
-    def to_kwargs(self, connection: Union["WebSocket", "Request"]) -> "DictAny":
+    def to_kwargs(self, connection: Union["WebSocket", "Request"]) -> Any:
         connection_params = {}
         for key, value in connection.query_params.items():
             if key not in self.query_param_names and len(value) == 1:
                 value = value[0]
                 connection_params[key] = value
 
         query_params = get_request_params(
-            params=connection.query_params, expected=self.query_params, url=connection.url
+            params=cast("MappingUnion", connection.query_params),
+            expected=self.query_params,
+            url=connection.url,
         )
         path_params = get_request_params(
-            params=connection.path_params, expected=self.path_params, url=connection.url
+            params=cast("MappingUnion", connection.path_params),
+            expected=self.path_params,
+            url=connection.url,
         )
         headers = get_request_params(
-            params=connection.headers, expected=self.headers, url=connection.url
+            params=cast("MappingUnion", connection.headers),
+            expected=self.headers,
+            url=connection.url,
         )
         cookies = get_request_params(
-            params=connection.cookies, expected=self.cookies, url=connection.url
+            params=cast("MappingUnion", connection.cookies),
+            expected=self.cookies,
+            url=connection.url,
         )
 
         if not self.reserved_kwargs:
             return {**query_params, **path_params, **headers, **cookies}
 
         return self.handle_reserved_kwargs(
             connection=connection,
@@ -287,23 +294,23 @@
             headers=headers,
             cookies=cookies,
         )
 
     def handle_reserved_kwargs(
         self,
         connection: Union["WebSocket", "Request"],
-        connection_params: "DictAny",
-        path_params: "DictAny",
-        query_params: "DictAny",
-        headers: "DictAny",
-        cookies: "DictAny",
-    ) -> "DictAny":
-        reserved_kwargs: "DictAny" = {}
+        connection_params: Any,
+        path_params: Any,
+        query_params: Any,
+        headers: Any,
+        cookies: Any,
+    ) -> Any:
+        reserved_kwargs: Any = {}
         if "data" in self.reserved_kwargs:
-            reserved_kwargs["data"] = self.get_request_data(request=connection)
+            reserved_kwargs["data"] = self.get_request_data(request=cast("Request", connection))
         if "request" in self.reserved_kwargs:
             reserved_kwargs["request"] = connection
         if "socket" in self.reserved_kwargs:
             reserved_kwargs["socket"] = connection
         if "headers" in self.reserved_kwargs:
             reserved_kwargs["headers"] = connection.headers
         if "cookies" in self.reserved_kwargs:
@@ -384,15 +391,15 @@
         parsed_form = parse_form_data(media_type, form_data, field)
         return parsed_form if parsed_form or not self.is_optional else None
 
     async def get_dependencies(
         self,
         dependency: "Dependency",
         connection: Union["WebSocket", "Request"],
-        **kwargs: "DictAny",
+        **kwargs: Any,
     ) -> Any:
         signature_model = get_signature(dependency.inject)
         for _dependency in dependency.dependencies:
             kwargs[_dependency.key] = await self.get_dependencies(
                 dependency=_dependency, connection=connection, **kwargs
             )
         dependency_kwargs = signature_model.parse_values_for_connection(
```

### Comparing `esmerald-1.2.5/esmerald/transformers/signature.py` & `esmerald-1.3.0/esmerald/transformers/signature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-"""
-Signature is widely used by Pydantic and comes from the inpect library.
-A lot of great work was done using the Signature and Esmerald is no exception.
-"""
-
 from inspect import Signature as InspectSignature
-from typing import TYPE_CHECKING, Any, Generator, Set, Type
+from typing import TYPE_CHECKING, Any, Dict, Generator, Optional, Set, Type
 
 from pydantic import create_model
 from pydantic.fields import Undefined
 
 from esmerald.exceptions import ImproperlyConfigured
 from esmerald.parsers import BaseModelExtra
 from esmerald.transformers.constants import CLASS_SPECIAL_WORDS, VALIDATION_NAMES
 from esmerald.transformers.datastructures import EsmeraldSignature, Parameter
 from esmerald.transformers.helpers import is_pydantic_constrained_field
 from esmerald.transformers.utils import get_field_definition_from_param
 from esmerald.utils.dependency import is_dependency_field, should_skip_dependency_validation
 
 if TYPE_CHECKING:
-    from pydantic.typing import AnyCallable, DictAny
+    from pydantic.typing import AnyCallable
 
 
 class SignatureFactory(BaseModelExtra):
     class Config(BaseModelExtra.Config):
         arbitrary_types_allowed = True
 
-    def __init__(self, fn: "AnyCallable", dependency_names: Set[str], **kwargs: "DictAny") -> None:
+    def __init__(
+        self, fn: Optional["AnyCallable"], dependency_names: Set[str], **kwargs: Any
+    ) -> None:
         super().__init__(**kwargs)
-        if not fn or fn is None:
+        if not fn:
             raise ImproperlyConfigured("Parameter 'fn' to SignatureFactory cannot be `None`.")
         self.fn = fn
         self.signature = InspectSignature.from_callable(self.fn)
         self.fn_name = fn.__name__ if hasattr(fn, "__name__") else "anonymous"
-        self.defaults = {}
+        self.defaults: Dict[str, Any] = {}
         self.dependency_names = dependency_names
-        self.field_definitions = {}
+        self.field_definitions: Dict[Any, Any] = {}
 
     def validate_missing_dependency(self, param: Any) -> None:
         if param.optional:
             return
         if not is_dependency_field(param.default):
             return
         field = param.default
```

### Comparing `esmerald-1.2.5/esmerald/transformers/types.py` & `esmerald-1.3.0/esmerald/transformers/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/transformers/utils.py` & `esmerald-1.3.0/esmerald/transformers/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 from esmerald.enums import ParamType, ScopeType
 from esmerald.exceptions import ImproperlyConfigured, ValidationErrorException
 from esmerald.parsers import BaseModelExtra, HashableBaseModel
 from esmerald.requests import Request
 from esmerald.utils.constants import REQUIRED
 
 if TYPE_CHECKING:
-    from pydantic.typing import DictAny, MappingIntStrAny
+    from pydantic.typing import MappingIntStrAny
 
     from esmerald.injector import Inject
     from esmerald.transformers.datastructures import EsmeraldSignature, Parameter
-    from esmerald.typing import ConnectionType
+    from esmerald.types import ConnectionType
 
 
 class ParamSetting(NamedTuple):
     default_value: Any
     field_alias: str
     field_name: str
     is_required: bool
     is_sequence: bool
     param_type: ParamType
     field_info: FieldInfo
 
 
 class Dependency(HashableBaseModel, BaseModelExtra):
     def __init__(
-        self, key: str, inject: "Inject", dependencies: List["Dependency"], **kwargs: "DictAny"
+        self, key: str, inject: "Inject", dependencies: List["Dependency"], **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
         self.key = key
         self.inject = inject
         self.dependencies = dependencies
 
     class Config(BaseModelExtra.Config):
@@ -87,17 +87,15 @@
         field_info=field_info,
         is_sequence=is_sequence,
         is_required=is_required and (default_value is None and not allow_none),
     )
     return param_settings
 
 
-def get_request_params(
-    params: "MappingIntStrAny", expected: Set[ParamSetting], url: URL
-) -> "DictAny":
+def get_request_params(params: "MappingIntStrAny", expected: Set[ParamSetting], url: URL) -> Any:
     """
     Gather the parameters from the request.
     """
     _params = []
     for param in expected:
         if param.is_required and param.field_alias not in params:
             _params.append(param.field_alias)
```

### Comparing `esmerald-1.2.5/esmerald/urls/base.py` & `esmerald-1.3.0/esmerald/core/urls/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 """
 Functions to use with the Router.
 """
 from importlib import import_module
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any, Optional, Sequence, Union
 
 from esmerald.exceptions import ImproperlyConfigured
 
+if TYPE_CHECKING:
+    from esmerald.routing.gateways import Gateway, WebSocketGateway
+    from esmerald.routing.router import Include
+
 DEFAULT_PATTERN = "route_patterns"
 
 
-def include(arg: Any, pattern: Optional[str] = DEFAULT_PATTERN):
+def include(
+    arg: Any, pattern: Optional[str] = DEFAULT_PATTERN
+) -> Sequence[Union["Gateway", "WebSocketGateway", "Include"]]:
     """Simple retrieve functionality to make it easier to include
     routes in the urls. Example, nested routes.
 
     Example:
 
         # myapp.routes.py
```

### Comparing `esmerald-1.2.5/esmerald/utils/constants.py` & `esmerald-1.3.0/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/utils/crypto.py` & `esmerald-1.3.0/esmerald/utils/crypto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import hashlib
 import random
 import time
 
 from esmerald.conf import settings
 
 try:
-    random = random.SystemRandom()
+    _random = random.SystemRandom()
     using_sysrandom = True
 except NotImplementedError:
     import warnings
 
     warnings.warn(
         "A secure pseudo-random number generator is not available "
         "on your system. Falling back to Mersenne Twister.",
@@ -30,21 +30,23 @@
     if not using_sysrandom:
         # This is ugly, and a hack, but it makes things better than
         # the alternative of predictability. This re-seeds the PRNG
         # using a value that is hard for an attacker to predict, every
         # time a random string is required. This may change the
         # properties of the chosen random sequence slightly, but this
         # is better than absolute predictability.
-        random.seed(
+        _random.seed(
             hashlib.sha256(
-                ("%s%s%s" % (random.getstate(), time.time(), settings.secret_key)).encode("utf-8")
+                ("{}{}{}".format(random.getstate(), time.time(), settings.secret_key)).encode(
+                    "utf-8"
+                )
             ).digest()
         )
     return "".join(random.choice(allowed_chars) for _ in range(length))
 
 
-def get_random_secret_key():
+def get_random_secret_key() -> str:
     """
     Return a 50 character random string usable as a SECRET_KEY setting value.
     """
     chars = "abcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*(-_=+)"
     return get_random_string(32, chars)
```

### Comparing `esmerald-1.2.5/esmerald/utils/functional.py` & `esmerald-1.3.0/esmerald/utils/functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import copy
 import operator
-from typing import Any
+from typing import Any, Callable, TypeVar
 
 empty = object()
+RT = TypeVar("RT")  # return type
 
 
-def new_method_proxy(func):
-    def inner(self, *args):
+def new_method_proxy(func: Callable[..., RT]) -> Callable[..., RT]:
+    def inner(self, *args: Any) -> RT:  # type: ignore
         if self._wrapped is empty:
             self._setup()
         return func(self._wrapped, *args)
 
     return inner
 
 
@@ -21,18 +22,18 @@
     By subclassing, you have the opportunity to intercept and alter the
     instantiation. If you don't need to do that, use SimpleLazyObject.
     """
 
     # Avoid infinite recursion when tracing __init__ (#19456).
     _wrapped = None
 
-    def __init__(self):
+    def __init__(self) -> None:
         # Note: if a subclass overrides __init__(), it will likely need to
         # override __copy__() and __deepcopy__() as well.
-        self._wrapped: Any = empty
+        self._wrapped = empty
 
     def __getattribute__(self, name: str) -> Any:
         if name == "_wrapped":
             # Avoid recursion when getting wrapped object.
             return super().__getattribute__(name)
         value: Any = super().__getattribute__(name)
         # If attribute is a proxy method, raise an AttributeError to call
@@ -55,15 +56,15 @@
     def __delattr__(self, name: str) -> None:
         if name == "_wrapped":
             raise TypeError("can't delete _wrapped.")
         if self._wrapped is empty:
             self._setup()
         delattr(self._wrapped, name)
 
-    def _setup(self):
+    def _setup(self) -> Any:
         """
         Must be implemented by subclasses to initialize the wrapped object.
         """
         raise NotImplementedError("subclasses of LazyObject must provide a _setup() method")
 
     # Because we have messed with __class__ below, we confuse pickle as to what
     # class we are pickling. We're going to have to initialize the wrapped
@@ -89,15 +90,15 @@
             # If uninitialized, copy the wrapper. Use type(self), not
             # self.__class__, because the latter is proxied.
             return type(self)()
         else:
             # If initialized, return a copy of the wrapped object.
             return copy.copy(self._wrapped)
 
-    def __deepcopy__(self, memo) -> Any:
+    def __deepcopy__(self, memo: Any) -> Any:
         if self._wrapped is empty:
             # We have to use type(self), not self.__class__, because the
             # latter is proxied.
             result = type(self)()
             memo[id(self)] = result
             return result
         return copy.deepcopy(self._wrapped, memo)
@@ -107,15 +108,15 @@
     __bool__: Any = new_method_proxy(bool)
 
     # Introspection support
     __dir__: Any = new_method_proxy(dir)
 
     # Need to pretend to be the wrapped class, for the sake of objects that
     # care about this (especially in equality tests)
-    __class__ = property(new_method_proxy(operator.attrgetter("__class__")))
+    __class__ = property(new_method_proxy(operator.attrgetter("__class__")))  # type: ignore
     __eq__: Any = new_method_proxy(operator.eq)
     __lt__: Any = new_method_proxy(operator.lt)
     __gt__: Any = new_method_proxy(operator.gt)
     __ne__: Any = new_method_proxy(operator.ne)
     __hash__: Any = new_method_proxy(hash)
 
     # List/Tuple/Dictionary methods support
@@ -138,53 +139,53 @@
 class SimpleLazyObject(LazyObject):
     """
     A lazy object initialized from any function.
     Designed for compound objects of unknown type. For builtins or objects of
     known type, use django.utils.functional.lazy.
     """
 
-    def __init__(self, func):
+    def __init__(self, func: Callable[..., RT]) -> None:
         """
         Pass in a callable that returns the object to be wrapped.
         If copies are made of the resulting SimpleLazyObject, which can happen
         in various circumstances within Django, then you must ensure that the
         callable can be safely run more than once and will return the same
         value.
         """
         self.__dict__["_setupfunc"] = func
         super().__init__()
 
-    def _setup(self):
+    def _setup(self) -> Any:
         self._wrapped = self._setupfunc()
 
     # Return a meaningful representation of the lazy object for debugging
     # without evaluating the wrapped object.
-    def __repr__(self):
+    def __repr__(self) -> str:
         if self._wrapped is empty:
             repr_attr = self._setupfunc
         else:
             repr_attr = self._wrapped
-        return "<%s: %r>" % (type(self).__name__, repr_attr)
+        return "<{}: {!r}>".format(type(self).__name__, repr_attr)
 
-    def __copy__(self):
+    def __copy__(self) -> Any:
         if self._wrapped is empty:
             # If uninitialized, copy the wrapper. Use SimpleLazyObject, not
             # self.__class__, because the latter is proxied.
             return SimpleLazyObject(self._setupfunc)
         else:
             # If initialized, return a copy of the wrapped object.
             return copy.copy(self._wrapped)
 
-    def __deepcopy__(self, memo):
+    def __deepcopy__(self, memo: Any) -> Any:
         if self._wrapped is empty:
             # We have to use SimpleLazyObject, not self.__class__, because the
             # latter is proxied.
             result = SimpleLazyObject(self._setupfunc)
             memo[id(self)] = result
             return result
         return copy.deepcopy(self._wrapped, memo)
 
     __add__ = new_method_proxy(operator.add)
 
     @new_method_proxy
-    def __radd__(self, other):
+    def __radd__(self, other: Any) -> Any:
         return other + self
```

### Comparing `esmerald-1.2.5/esmerald/utils/helpers.py` & `esmerald-1.3.0/esmerald/utils/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 T = TypeVar("T")
 
 
 def is_async_callable(value: Callable[P, T]) -> TypeGuard[Callable[P, Awaitable[T]]]:
     while isinstance(value, functools.partial):
         value = value.func  # type: ignore[unreachable]
 
-    return asyncio.iscoroutinefunction(value) or asyncio.iscoroutinefunction(value.__call__)  # ty
+    return asyncio.iscoroutinefunction(value) or asyncio.iscoroutinefunction(value.__call__)  # type: ignore
 
 
 def is_class_and_subclass(value: typing.Any, _type: typing.Any) -> bool:
     original = get_origin(value)
     if not original and not isclass(value):
         return False
 
@@ -36,12 +36,12 @@
             return original and issubclass(original, _type)
         return issubclass(value, _type)
     except TypeError:
         return False
 
 
 def clean_string(value: str) -> str:
-    return slugify.slugify(value, separator="_")
+    return slugify.slugify(value, separator="_")  # type: ignore
 
 
 def is_optional_union(annotation: Any) -> bool:
     return get_origin(annotation) in UNION_TYPES and type(None) in get_args(annotation)
```

### Comparing `esmerald-1.2.5/esmerald/utils/model.py` & `esmerald-1.3.0/esmerald/utils/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from inspect import isclass
 from typing import TYPE_CHECKING, Any, Dict, Type, cast
 
 from pydantic import BaseConfig, BaseModel, create_model
-from pydantic_factories.utils import create_model_from_dataclass
+from pyfactories.utils import create_model_from_dataclass
 
 if TYPE_CHECKING:
     from pydantic.fields import ModelField
 
 
 class Config(BaseConfig):
     arbitrary_types_allowed = True
```

### Comparing `esmerald-1.2.5/esmerald/utils/module_loading.py` & `esmerald-1.3.0/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/esmerald/utils/pydantic.py` & `esmerald-1.3.0/esmerald/utils/pydantic/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from typing import TYPE_CHECKING, Any, cast
+from decimal import Decimal
+from typing import TYPE_CHECKING, Any, TypeVar, cast
+
+T = TypeVar("T", int, float, Decimal)
 
 if TYPE_CHECKING:
     from pydantic.fields import ModelField
 
 
 def is_field_optional(field: "ModelField") -> bool:
     """
```

### Comparing `esmerald-1.2.5/LICENSE` & `esmerald-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.5/README.md` & `esmerald-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 <a href="https://pypi.org/project/esmerald" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/esmerald.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 </p>
 
 ---
 
-**Documentation**: [https://esmerald.dev](https://www,esmerald.dev) 📚
+**Documentation**: [https://esmerald.dev](https://www.esmerald.dev) 📚
 
 **Source Code**: [https://github.com/dymmond/esmerald](https://github.com/dymmond/esmerald)
 
 ---
 
 Esmerald is a modern, powerful, flexible, high performant, web framework designed to build not only APIs
 but also full scalable applications from the smallest to enterprise level.
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # Esmerald
                                   [Esmerald]
   ð Highly scalable, performant, easy to learn, easy to code and for every
                                application. ð
           [Test_Suite] [Package_version] [Supported_Python_versions]
---- **Documentation**: [https://esmerald.dev](https://www,esmerald.dev) ð
+--- **Documentation**: [https://esmerald.dev](https://www.esmerald.dev) ð
 **Source Code**: [https://github.com/dymmond/esmerald](https://github.com/
 dymmond/esmerald) --- Esmerald is a modern, powerful, flexible, high
 performant, web framework designed to build not only APIs but also full
 scalable applications from the smallest to enterprise level. Esmerald is
 designed to build with python 3.8+ and based on standard python type hints and
 on the top of the heavily known [Starlette](https://github.com/encode/
 starlette) and [Pydantic](https://github.com/samuelcolvin/pydantic). Check out
```

### Comparing `esmerald-1.2.5/pyproject.toml` & `esmerald-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     "awesome-slugify>=1.6.5,<2",
     "httpx>=0.24.0,<0.30.0",
     "itsdangerous>=2.1.2,<3.0.0",
     "jinja2>=3.1.2,<4.0.0",
     "jsonschema_rs>=0.16.2,<0.20.0",
     "loguru>=0.6.0,<0.7.0",
     "pydantic>=1.10.9,<2.0.0",
-    "pydantic-factories==1.17.2",
+    "pyfactories>=1.0.0",
     "python-multipart>=0.0.5,<0.0.7",
     "openapi-schemas-pydantic>=1.1.0",
     "rich>=13.3.1,<14.0.0",
     "starlette>=0.28.0,<1.0",
 ]
 keywords = [
     "api",
@@ -89,32 +89,32 @@
 Source = "https://github.com/dymmond/esmerald"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.3.1,<8.0.0",
     "pytest-cov>=2.12.0,<5.0.0",
     "pytest-asyncio>=0.19.0",
-    "mypy==1.1.1",
+    "mypy>=1.4.1",
     "flake8>=5.0.4",
     "black== 23.3.0",
     "isort>=5.0.6,<6.0.0",
     "aiofiles>=0.8.0,<24",
     "a2wsgi>=1.7.0,<2",
-    "asyncz>=0.2.0",
+    "asyncz>=0.3.1",
     "anyio[trio]>=3.6.2,<4.0.0",
     "asyncio[trio]>=3.4.3,<4.0.0",
     "brotli>=1.0.9,<2.0.0",
     "jinja2>=3.1.2,<4.0.0",
     "flask>=1.1.2,<3.0.0",
     "freezegun>=1.2.2,<2.0.0",
     "mock==5.0.1",
     "passlib==1.7.4",
     "python-jose>=3.3.0,<4",
     "orjson>=3.8.5,<4.0.0",
-    "saffier[postgres]>=0.7.4",
+    "saffier[postgres]>=0.13.0",
     "requests>=2.28.2,<3.0.0",
     "ruff>=0.0.256,<1.0.0",
     "ujson>=5.7.0,<6",
 
     # types
     "types-ujson==5.7.0.5",
     "types-orjson==3.6.2",
@@ -153,27 +153,31 @@
 esmerald = "esmerald.core.directives.cli:esmerald_cli"
 
 [tool.isort]
 profile = "black"
 known_third_party = ["esmerald", "pydantic", "starlette"]
 
 [tool.mypy]
+strict = true
 warn_unused_configs = true
 warn_unreachable = true
 warn_return_any = true
-strict = true
 disallow_untyped_decorators = true
 disallow_any_generics = false
 implicit_reexport = false
 show_error_codes = true
 disallow_incomplete_defs = true
-disable_error_code = "attr-defined"
+disable_error_code = "attr-defined,has-type,override"
 exclude = "esmerald/conf,esmerald/utils"
 warn_unused_ignores = true
 warn_redundant_casts = true
+no_implicit_optional = false
+strict_equality = false
+strict_optional = false
+
 
 [tool.ruff]
 select = [
     "E", # pycodestyle errors
     "W", # pycodestyle warnings
     "F", # pyflakes
     "C", # flake8-comprehensions
@@ -196,19 +200,22 @@
 [[tool.mypy.overrides]]
 module = "docs_src.*"
 ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = [
     "sqlalchemy.*",
-    "asyncpg",
-    "alembic",
     "sqlalchemy_utils.*",
-    "slugify",
+    "slugify.*",
     "pytz",
+    "jose.*",
+    "mako.*",
+    "passlib.*",
+    "esmerald.contrib.auth.saffier.*",
+    "openapi_schemas_pydantic.*",
 ]
 ignore_missing_imports = true
 ignore_errors = true
 
 [tool.pytest.ini_options]
 addopts = ["--strict-config", "--strict-markers"]
 xfail_strict = true
```

### Comparing `esmerald-1.2.5/PKG-INFO` & `esmerald-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 1.2.5
+Version: 1.3.0
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -42,16 +42,16 @@
 Requires-Dist: awesome-slugify<2,>=1.6.5
 Requires-Dist: httpx<0.30.0,>=0.24.0
 Requires-Dist: itsdangerous<3.0.0,>=2.1.2
 Requires-Dist: jinja2<4.0.0,>=3.1.2
 Requires-Dist: jsonschema-rs<0.20.0,>=0.16.2
 Requires-Dist: loguru<0.7.0,>=0.6.0
 Requires-Dist: openapi-schemas-pydantic>=1.1.0
-Requires-Dist: pydantic-factories==1.17.2
 Requires-Dist: pydantic<2.0.0,>=1.10.9
+Requires-Dist: pyfactories>=1.0.0
 Requires-Dist: python-multipart<0.0.7,>=0.0.5
 Requires-Dist: rich<14.0.0,>=13.3.1
 Requires-Dist: starlette<1.0,>=0.28.0
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8<6.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.0.4; extra == 'dev'
@@ -76,33 +76,33 @@
 Provides-Extra: templates
 Requires-Dist: mako==1.2.4; extra == 'templates'
 Provides-Extra: test
 Requires-Dist: a2wsgi<2,>=1.7.0; extra == 'test'
 Requires-Dist: aiofiles<24,>=0.8.0; extra == 'test'
 Requires-Dist: anyio[trio]<4.0.0,>=3.6.2; extra == 'test'
 Requires-Dist: asyncio[trio]<4.0.0,>=3.4.3; extra == 'test'
-Requires-Dist: asyncz>=0.2.0; extra == 'test'
+Requires-Dist: asyncz>=0.3.1; extra == 'test'
 Requires-Dist: black==23.3.0; extra == 'test'
 Requires-Dist: brotli<2.0.0,>=1.0.9; extra == 'test'
 Requires-Dist: flake8>=5.0.4; extra == 'test'
 Requires-Dist: flask<3.0.0,>=1.1.2; extra == 'test'
 Requires-Dist: freezegun<2.0.0,>=1.2.2; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: jinja2<4.0.0,>=3.1.2; extra == 'test'
 Requires-Dist: mock==5.0.1; extra == 'test'
-Requires-Dist: mypy==1.1.1; extra == 'test'
+Requires-Dist: mypy>=1.4.1; extra == 'test'
 Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'test'
 Requires-Dist: passlib==1.7.4; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.3.1; extra == 'test'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.28.2; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
-Requires-Dist: saffier[postgres]>=0.7.4; extra == 'test'
+Requires-Dist: saffier[postgres]>=0.13.0; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
 Requires-Dist: types-ujson==5.7.0.5; extra == 'test'
 Requires-Dist: ujson<6,>=5.7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Esmerald
 
@@ -126,15 +126,15 @@
 <a href="https://pypi.org/project/esmerald" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/esmerald.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 </p>
 
 ---
 
-**Documentation**: [https://esmerald.dev](https://www,esmerald.dev) 📚
+**Documentation**: [https://esmerald.dev](https://www.esmerald.dev) 📚
 
 **Source Code**: [https://github.com/dymmond/esmerald](https://github.com/dymmond/esmerald)
 
 ---
 
 Esmerald is a modern, powerful, flexible, high performant, web framework designed to build not only APIs
 but also full scalable applications from the smallest to enterprise level.
```

