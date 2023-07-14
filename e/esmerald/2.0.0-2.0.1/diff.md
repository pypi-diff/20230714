# Comparing `tmp/esmerald-2.0.0.tar.gz` & `tmp/esmerald-2.0.1.tar.gz`

## Comparing `esmerald-2.0.0.tar` & `esmerald-2.0.1.tar`

### file list

```diff
@@ -1,186 +1,186 @@
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/__init__.py
--rw-r--r--   0        0        0    39505 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/concurrency.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/enums.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/exceptions.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/injector.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/logging.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/param_functions.py
--rw-r--r--   0        0        0    21321 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/params.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/py.typed
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/staticfiles.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/testclient.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/types.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/typing.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/websockets.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/enums.py
--rw-r--r--   0        0        0    14737 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/jwt.py
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/openapi.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/session.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/static_files.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/urls/__init__.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/urls/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/_internal.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/constants.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/docs.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/models.py
--rw-r--r--   0        0        0    17266 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/openapi.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/params.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/permissions/base.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/utils/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/utils/protocols.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/base.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/__init__.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/_internal.py
--rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/base.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/events.py
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    22735 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    42063 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/router.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14628 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/model.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/helpers.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/pydantic/__init__.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/pydantic/schema.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-2.0.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-2.0.0/LICENSE
--rw-r--r--   0        0        0    15810 2020-02-02 00:00:00.000000 esmerald-2.0.0/README.md
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 esmerald-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    21018 2020-02-02 00:00:00.000000 esmerald-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/__init__.py
+-rw-r--r--   0        0        0    39505 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/concurrency.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/enums.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/injector.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/logging.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/param_functions.py
+-rw-r--r--   0        0        0    21321 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/params.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/py.typed
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/testclient.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/types.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/websockets.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    14737 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/session.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/_internal.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/constants.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/docs.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/models.py
+-rw-r--r--   0        0        0    17266 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/openapi.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/params.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/utils/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/utils/protocols.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/base.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/_internal.py
+-rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    22735 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    42063 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/router.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14628 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-2.0.1/LICENSE
+-rw-r--r--   0        0        0    15936 2020-02-02 00:00:00.000000 esmerald-2.0.1/README.md
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 esmerald-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    21144 2020-02-02 00:00:00.000000 esmerald-2.0.1/PKG-INFO
```

### Comparing `esmerald-2.0.0/esmerald/__init__.py` & `esmerald-2.0.1/esmerald/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 
 from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
```

### Comparing `esmerald-2.0.0/esmerald/applications.py` & `esmerald-2.0.1/esmerald/applications.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/backgound.py` & `esmerald-2.0.1/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/enums.py` & `esmerald-2.0.1/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/exception_handlers.py` & `esmerald-2.0.1/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/exceptions.py` & `esmerald-2.0.1/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/injector.py` & `esmerald-2.0.1/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/logging.py` & `esmerald-2.0.1/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/params.py` & `esmerald-2.0.1/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/parsers.py` & `esmerald-2.0.1/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/requests.py` & `esmerald-2.0.1/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/testclient.py` & `esmerald-2.0.1/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/types.py` & `esmerald-2.0.1/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/websockets.py` & `esmerald-2.0.1/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/conf/__init__.py` & `esmerald-2.0.1/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/conf/global_settings.py` & `esmerald-2.0.1/esmerald/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-2.0.1/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-2.0.1/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-2.0.1/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-2.0.1/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-2.0.1/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/config/jwt.py` & `esmerald-2.0.1/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/config/openapi.py` & `esmerald-2.0.1/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/config/session.py` & `esmerald-2.0.1/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/config/static_files.py` & `esmerald-2.0.1/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/contrib/encoding.py` & `esmerald-2.0.1/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/contrib/auth/hashers.py` & `esmerald-2.0.1/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/contrib/auth/common/middleware.py` & `esmerald-2.0.1/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-2.0.1/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-2.0.1/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/base.py` & `esmerald-2.0.1/esmerald/core/directives/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/cli.py` & `esmerald-2.0.1/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/env.py` & `esmerald-2.0.1/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/templates.py` & `esmerald-2.0.1/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/utils.py` & `esmerald-2.0.1/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/operations/createapp.py` & `esmerald-2.0.1/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/operations/createproject.py` & `esmerald-2.0.1/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/operations/list.py` & `esmerald-2.0.1/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/operations/run.py` & `esmerald-2.0.1/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/operations/runserver.py` & `esmerald-2.0.1/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/directives/operations/show_urls.py` & `esmerald-2.0.1/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/terminal/base.py` & `esmerald-2.0.1/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/terminal/print.py` & `esmerald-2.0.1/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/terminal/terminal.py` & `esmerald-2.0.1/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/core/urls/base.py` & `esmerald-2.0.1/esmerald/core/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/datastructures/__init__.py` & `esmerald-2.0.1/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/datastructures/base.py` & `esmerald-2.0.1/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/datastructures/encoders.py` & `esmerald-2.0.1/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/datastructures/file.py` & `esmerald-2.0.1/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/datastructures/json.py` & `esmerald-2.0.1/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/datastructures/redirect.py` & `esmerald-2.0.1/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/datastructures/stream.py` & `esmerald-2.0.1/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/datastructures/template.py` & `esmerald-2.0.1/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/interceptors/interceptor.py` & `esmerald-2.0.1/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/middleware/__init__.py` & `esmerald-2.0.1/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/middleware/_exception_handlers.py` & `esmerald-2.0.1/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/middleware/asyncexitstack.py` & `esmerald-2.0.1/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/middleware/authentication.py` & `esmerald-2.0.1/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/middleware/basic.py` & `esmerald-2.0.1/esmerald/middleware/basic.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/middleware/csrf.py` & `esmerald-2.0.1/esmerald/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/middleware/errors.py` & `esmerald-2.0.1/esmerald/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/middleware/exceptions.py` & `esmerald-2.0.1/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/middleware/settings_middleware.py` & `esmerald-2.0.1/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/openapi/_internal.py` & `esmerald-2.0.1/esmerald/openapi/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/openapi/docs.py` & `esmerald-2.0.1/esmerald/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/openapi/models.py` & `esmerald-2.0.1/esmerald/openapi/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/openapi/openapi.py` & `esmerald-2.0.1/esmerald/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/openapi/responses.py` & `esmerald-2.0.1/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/openapi/utils.py` & `esmerald-2.0.1/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/permissions/base.py` & `esmerald-2.0.1/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/permissions/utils.py` & `esmerald-2.0.1/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/pluggables/base.py` & `esmerald-2.0.1/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/protocols/asyncdao.py` & `esmerald-2.0.1/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/protocols/dao.py` & `esmerald-2.0.1/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/protocols/interceptor.py` & `esmerald-2.0.1/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/protocols/template.py` & `esmerald-2.0.1/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/responses/base.py` & `esmerald-2.0.1/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/responses/encoders.py` & `esmerald-2.0.1/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/responses/json.py` & `esmerald-2.0.1/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/responses/template.py` & `esmerald-2.0.1/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/routing/_internal.py` & `esmerald-2.0.1/esmerald/routing/_internal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import cached_property
-from typing import Any, Dict
+from typing import Any, Dict, List
 
 from esmerald.openapi.params import ResponseParam
 from esmerald.params import Body
 from esmerald.utils.constants import DATA
 
 
 class FieldInfoMixin:
@@ -12,22 +12,37 @@
     OpenAPI parsing.
     """
 
     @cached_property
     def response_models(self) -> Dict[int, Any]:
         """
         The models converted into pydantic fields with the model used for OpenAPI.
+
+        The response models can be a list representation or a single object representation.
+        If another type of object is passed through the `model`, an Assertation error is raised.
         """
         responses: Dict[int, ResponseParam] = {}
         if self.responses:
             for status_code, response in self.responses.items():
+                annotation = (
+                    List[response.model[0]]  # type: ignore
+                    if isinstance(response.model, list)
+                    else response.model
+                )
+
+                name = (
+                    response.model[0].__name__
+                    if isinstance(response.model, list)
+                    else response.model.__name__
+                )
+
                 responses[status_code] = ResponseParam(
-                    annotation=response.model,
+                    annotation=annotation,
                     description=response.description,
-                    alias=response.model.__name__,
+                    alias=name,
                 )
         return responses
 
     @cached_property
     def data_field(self) -> Any:
         """The field used for the payload body"""
         if DATA in self.signature_model.model_fields:
```

### Comparing `esmerald-2.0.0/esmerald/routing/base.py` & `esmerald-2.0.1/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/routing/events.py` & `esmerald-2.0.1/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/routing/gateways.py` & `esmerald-2.0.1/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/routing/handlers.py` & `esmerald-2.0.1/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/routing/router.py` & `esmerald-2.0.1/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/routing/views.py` & `esmerald-2.0.1/esmerald/routing/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/security/jwt/token.py` & `esmerald-2.0.1/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/template/jinja.py` & `esmerald-2.0.1/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/template/mako.py` & `esmerald-2.0.1/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/transformers/datastructures.py` & `esmerald-2.0.1/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/transformers/helpers.py` & `esmerald-2.0.1/esmerald/transformers/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/transformers/model.py` & `esmerald-2.0.1/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/transformers/signature.py` & `esmerald-2.0.1/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/transformers/types.py` & `esmerald-2.0.1/esmerald/transformers/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/transformers/utils.py` & `esmerald-2.0.1/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/utils/constants.py` & `esmerald-2.0.1/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/utils/crypto.py` & `esmerald-2.0.1/esmerald/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/utils/dependency.py` & `esmerald-2.0.1/esmerald/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/utils/functional.py` & `esmerald-2.0.1/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/utils/helpers.py` & `esmerald-2.0.1/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/utils/model.py` & `esmerald-2.0.1/esmerald/utils/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/utils/module_loading.py` & `esmerald-2.0.1/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/utils/sync.py` & `esmerald-2.0.1/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/esmerald/utils/pydantic/schema.py` & `esmerald-2.0.1/esmerald/utils/pydantic/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/LICENSE` & `esmerald-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.0/README.md` & `esmerald-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -503,17 +503,20 @@
 the settings and makes Swagger and ReDoc available to you out of the box.
 
 To access the OpenAPI, simply start your local development and access:
 
 * **Swagger** - `/docs/swagger`.
 * **Redoc** - `/docs/redoc`.
 
-There are more details about [how to configure the OpenAPIConfig](https://esmerald.dev/configurations/openapi/config.md)
+There are more details about [how to configure the OpenAPIConfig](https://esmerald.dev/configurations/openapi/config)
 within the documentation.
 
+There is also a good explanation on how to use the [OpenAPIResponse](https://esmerald.dev/responses#openapi-responses)
+as well.
+
 ## Notes
 
 This is just a very high-level demonstration of how to start quickly and what Esmerald can do.
 There are plenty more things you can do with Esmerald. Enjoy! 😊
 
 ## Sponsors
```

#### html2text {}

```diff
@@ -181,14 +181,15 @@
 docs integrated. For those used to that, this is roughly the same and to make
 it happen, there were inspirations that helped Esmerald getting there fast.
 Esmerald starts automatically the OpenAPI documentation by injecting the
 OpenAPIConfig default from the settings and makes Swagger and ReDoc available
 to you out of the box. To access the OpenAPI, simply start your local
 development and access: * **Swagger** - `/docs/swagger`. * **Redoc** - `/docs/
 redoc`. There are more details about [how to configure the OpenAPIConfig]
-(https://esmerald.dev/configurations/openapi/config.md) within the
-documentation. ## Notes This is just a very high-level demonstration of how to
-start quickly and what Esmerald can do. There are plenty more things you can do
-with Esmerald. Enjoy! ð ## Sponsors Currently there are no sponsors of
-Esmerald but you can financially help and support the author though [GitHub
-sponsors](https://github.com/sponsors/tarsil) and become a **Special one** or a
-**Legend**.
+(https://esmerald.dev/configurations/openapi/config) within the documentation.
+There is also a good explanation on how to use the [OpenAPIResponse](https://
+esmerald.dev/responses#openapi-responses) as well. ## Notes This is just a very
+high-level demonstration of how to start quickly and what Esmerald can do.
+There are plenty more things you can do with Esmerald. Enjoy! ð ## Sponsors
+Currently there are no sponsors of Esmerald but you can financially help and
+support the author though [GitHub sponsors](https://github.com/sponsors/tarsil)
+and become a **Special one** or a **Legend**.
```

### Comparing `esmerald-2.0.0/pyproject.toml` & `esmerald-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     "loguru>=0.7.0,<0.8.0",
     "pydantic>=2.0.1,<3.0.0",
     "pydantic-extra-types>=2.0.0,<3.0.0",
     "pydantic-settings>=2.0.0,<3.0.0",
     "python-multipart>=0.0.5,<0.0.7",
     "openapi-schemas-pydantic>=2.0.0",
     "rich>=13.3.1,<14.0.0",
-    "starlette>=0.29.0,<1.0",
+    "starlette>=0.30.0,<1.0",
 ]
 keywords = [
     "api",
     "rest",
     "http",
     "asgi",
     "pydantic",
@@ -109,15 +109,15 @@
     "flask>=1.1.2,<3.0.0",
     "freezegun>=1.2.2,<2.0.0",
     "mock==5.0.1",
     "passlib==1.7.4",
     "polyfactory>=2.5.0,<3.0.0",
     "python-jose>=3.3.0,<4",
     "orjson>=3.8.5,<4.0.0",
-    "saffier[postgres]>=0.14.0",
+    "saffier[postgres]>=0.15.0",
     "requests>=2.28.2,<3.0.0",
     "ruff>=0.0.256,<1.0.0",
     "ujson>=5.7.0,<6",
 
     # types
     "types-ujson==5.8.0.0",
     "types-orjson==3.6.2",
```

### Comparing `esmerald-2.0.0/PKG-INFO` & `esmerald-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 2.0.0
+Version: 2.0.1
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -48,15 +48,15 @@
 Requires-Dist: loguru<0.8.0,>=0.7.0
 Requires-Dist: openapi-schemas-pydantic>=2.0.0
 Requires-Dist: pydantic-extra-types<3.0.0,>=2.0.0
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0
 Requires-Dist: pydantic<3.0.0,>=2.0.1
 Requires-Dist: python-multipart<0.0.7,>=0.0.5
 Requires-Dist: rich<14.0.0,>=13.3.1
-Requires-Dist: starlette<1.0,>=0.29.0
+Requires-Dist: starlette<1.0,>=0.30.0
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8<6.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.0.4; extra == 'dev'
 Requires-Dist: uvicorn[standard]>=0.19.0; extra == 'dev'
 Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
@@ -97,15 +97,15 @@
 Requires-Dist: polyfactory<3.0.0,>=2.5.0; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.3.1; extra == 'test'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.28.2; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
-Requires-Dist: saffier[postgres]>=0.14.0; extra == 'test'
+Requires-Dist: saffier[postgres]>=0.15.0; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
 Requires-Dist: types-ujson==5.8.0.0; extra == 'test'
 Requires-Dist: ujson<6,>=5.7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Esmerald
 
@@ -612,17 +612,20 @@
 the settings and makes Swagger and ReDoc available to you out of the box.
 
 To access the OpenAPI, simply start your local development and access:
 
 * **Swagger** - `/docs/swagger`.
 * **Redoc** - `/docs/redoc`.
 
-There are more details about [how to configure the OpenAPIConfig](https://esmerald.dev/configurations/openapi/config.md)
+There are more details about [how to configure the OpenAPIConfig](https://esmerald.dev/configurations/openapi/config)
 within the documentation.
 
+There is also a good explanation on how to use the [OpenAPIResponse](https://esmerald.dev/responses#openapi-responses)
+as well.
+
 ## Notes
 
 This is just a very high-level demonstration of how to start quickly and what Esmerald can do.
 There are plenty more things you can do with Esmerald. Enjoy! 😊
 
 ## Sponsors
```

