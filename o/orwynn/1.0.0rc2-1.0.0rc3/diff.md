# Comparing `tmp/orwynn-1.0.0rc2.tar.gz` & `tmp/orwynn-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orwynn-1.0.0rc2.tar", max compression
+gzip compressed data, was "orwynn-1.0.0rc3.tar", max compression
```

## Comparing `orwynn-1.0.0rc2.tar` & `orwynn-1.0.0rc3.tar`

### file list

```diff
@@ -1,276 +1,276 @@
--rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0      307 2023-05-22 08:29:05.173562 orwynn-1.0.0rc2/README.md
--rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0rc2/orwynn/__init__.py
--rw-r--r--   0        0        0     1920 2023-06-08 13:46:47.770769 orwynn-1.0.0rc2/orwynn/apiversion/__init__.py
--rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/apiversion/errors.py
--rw-r--r--   0        0        0     4873 2023-07-10 13:45:40.443311 orwynn-1.0.0rc2/orwynn/apiversion/test_main.py
--rw-r--r--   0        0        0       77 2023-06-08 13:47:49.293428 orwynn-1.0.0rc2/orwynn/app/__init__.py
--rw-r--r--   0        0        0      400 2023-06-08 13:48:58.389784 orwynn-1.0.0rc2/orwynn/app/apirouter.py
--rw-r--r--   0        0        0     1484 2023-06-08 13:47:28.661538 orwynn-1.0.0rc2/orwynn/app/apiwebsocketroute.py
--rw-r--r--   0        0        0     2594 2023-06-09 12:20:44.292995 orwynn-1.0.0rc2/orwynn/app/app.py
--rw-r--r--   0        0        0      188 2023-06-09 10:55:27.417944 orwynn-1.0.0rc2/orwynn/app/config.py
--rw-r--r--   0        0        0     1560 2023-06-08 13:47:12.703403 orwynn-1.0.0rc2/orwynn/app/core.py
--rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0rc2/orwynn/app/mode.py
--rw-r--r--   0        0        0     2367 2023-07-10 13:45:40.440312 orwynn-1.0.0rc2/orwynn/app/test_main.py
--rw-r--r--   0        0        0       98 2023-06-09 11:05:03.703488 orwynn-1.0.0rc2/orwynn/app/types.py
--rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0rc2/orwynn/app/utils.py
--rw-r--r--   0        0        0       56 2023-06-08 13:49:42.996486 orwynn-1.0.0rc2/orwynn/apprc/__init__.py
--rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0rc2/orwynn/apprc/apprc.py
--rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0rc2/orwynn/apprc/constants.py
--rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/apprc/errors.py
--rw-r--r--   0        0        0     3493 2023-06-08 13:49:43.002486 orwynn-1.0.0rc2/orwynn/apprc/parse.py
--rw-r--r--   0        0        0     2724 2023-07-10 12:01:27.295418 orwynn-1.0.0rc2/orwynn/apprc/test_main.py
--rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0rc2/orwynn/base/__init__.py
--rw-r--r--   0        0        0       27 2023-06-08 13:49:50.224117 orwynn-1.0.0rc2/orwynn/base/config/__init__.py
--rw-r--r--   0        0        0     1109 2023-06-09 05:54:54.979178 orwynn-1.0.0rc2/orwynn/base/config/config.py
--rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0rc2/orwynn/base/config/test_config.py
--rw-r--r--   0        0        0       35 2023-06-08 13:50:00.474596 orwynn-1.0.0rc2/orwynn/base/controller/__init__.py
--rw-r--r--   0        0        0     2211 2023-07-06 09:35:56.327943 orwynn-1.0.0rc2/orwynn/base/controller/controller.py
--rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0rc2/orwynn/base/controller/errors.py
--rw-r--r--   0        0        0       31 2023-06-08 13:50:07.129259 orwynn-1.0.0rc2/orwynn/base/database/__init__.py
--rw-r--r--   0        0        0      629 2023-06-08 13:55:40.340226 orwynn-1.0.0rc2/orwynn/base/database/database.py
--rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0rc2/orwynn/base/database/errors.py
--rw-r--r--   0        0        0      203 2023-06-09 06:20:20.113767 orwynn-1.0.0rc2/orwynn/base/error/__init__.py
--rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0rc2/orwynn/base/error/code.py
--rw-r--r--   0        0        0      284 2023-06-08 13:54:00.170896 orwynn-1.0.0rc2/orwynn/base/error/errors.py
--rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.112767 orwynn-1.0.0rc2/orwynn/base/error/test_main.py
--rw-r--r--   0        0        0      436 2023-06-08 13:50:50.520080 orwynn-1.0.0rc2/orwynn/base/error/test_utils.py
--rw-r--r--   0        0        0     2006 2023-06-08 13:54:17.686071 orwynn-1.0.0rc2/orwynn/base/error/utils.py
--rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0rc2/orwynn/base/error/valueschema.py
--rw-r--r--   0        0        0       39 2023-06-08 13:54:42.338917 orwynn-1.0.0rc2/orwynn/base/errorhandler/__init__.py
--rw-r--r--   0        0        0     2354 2023-07-10 16:06:16.709892 orwynn-1.0.0rc2/orwynn/base/errorhandler/errorhandler.py
--rw-r--r--   0        0        0       82 2023-06-08 13:55:03.438934 orwynn-1.0.0rc2/orwynn/base/middleware/__init__.py
--rw-r--r--   0        0        0       94 2023-06-08 13:55:03.438934 orwynn-1.0.0rc2/orwynn/base/middleware/globalsetup.py
--rw-r--r--   0        0        0     2919 2023-04-21 09:59:20.018394 orwynn-1.0.0rc2/orwynn/base/middleware/middleware.py
--rw-r--r--   0        0        0     1281 2023-07-10 13:45:40.445311 orwynn-1.0.0rc2/orwynn/base/middleware/test_main.py
--rw-r--r--   0        0        0       25 2023-06-08 13:55:11.806546 orwynn-1.0.0rc2/orwynn/base/model/__init__.py
--rw-r--r--   0        0        0     1423 2023-07-06 09:10:08.307376 orwynn-1.0.0rc2/orwynn/base/model/model.py
--rw-r--r--   0        0        0      791 2023-06-09 06:20:20.110767 orwynn-1.0.0rc2/orwynn/base/model/test_model.py
--rw-r--r--   0        0        0       27 2023-06-08 13:55:21.285106 orwynn-1.0.0rc2/orwynn/base/module/__init__.py
--rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0rc2/orwynn/base/module/errors.py
--rw-r--r--   0        0        0     7183 2023-06-08 13:55:37.034379 orwynn-1.0.0rc2/orwynn/base/module/module.py
--rw-r--r--   0        0        0      950 2023-06-08 13:55:21.291106 orwynn-1.0.0rc2/orwynn/base/module/test_module.py
--rw-r--r--   0        0        0       69 2023-06-08 13:55:40.340226 orwynn-1.0.0rc2/orwynn/base/service/__init__.py
--rw-r--r--   0        0        0      396 2023-06-08 13:55:40.342226 orwynn-1.0.0rc2/orwynn/base/service/framework.py
--rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0rc2/orwynn/base/service/service.py
--rw-r--r--   0        0        0       27 2023-06-08 13:55:46.418946 orwynn-1.0.0rc2/orwynn/base/worker/__init__.py
--rw-r--r--   0        0        0      212 2023-06-09 05:57:10.064779 orwynn-1.0.0rc2/orwynn/base/worker/worker.py
--rw-r--r--   0        0        0       54 2023-06-08 13:56:30.127942 orwynn-1.0.0rc2/orwynn/boot/__init__.py
--rw-r--r--   0        0        0    12600 2023-07-10 13:48:28.037990 orwynn-1.0.0rc2/orwynn/boot/boot.py
--rw-r--r--   0        0        0      716 2023-06-09 05:54:54.987177 orwynn-1.0.0rc2/orwynn/boot/config.py
--rw-r--r--   0        0        0       95 2023-06-08 13:58:33.909354 orwynn-1.0.0rc2/orwynn/boot/errors.py
--rw-r--r--   0        0        0     5375 2023-07-10 12:56:58.086353 orwynn-1.0.0rc2/orwynn/boot/test_main.py
--rw-r--r--   0        0        0      154 2023-06-09 06:20:20.102768 orwynn-1.0.0rc2/orwynn/bootscript/__init__.py
--rw-r--r--   0        0        0      278 2023-07-10 12:10:57.216627 orwynn-1.0.0rc2/orwynn/bootscript/bootscript.py
--rw-r--r--   0        0        0      114 2023-07-10 13:25:24.969000 orwynn-1.0.0rc2/orwynn/bootscript/callable.py
--rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0rc2/orwynn/bootscript/calltime.py
--rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0rc2/orwynn/bootscript/errors.py
--rw-r--r--   0        0        0     1384 2023-07-10 13:45:40.440312 orwynn-1.0.0rc2/orwynn/bootscript/test_main.py
--rw-r--r--   0        0        0     2523 2023-07-10 13:45:40.438311 orwynn-1.0.0rc2/orwynn/bootscript/worker.py
--rw-r--r--   0        0        0       31 2023-07-10 13:55:28.842455 orwynn-1.0.0rc2/orwynn/cli/__init__.py
--rw-r--r--   0        0        0       79 2023-07-11 07:12:44.820534 orwynn-1.0.0rc2/orwynn/cli/__main__.py
--rw-r--r--   0        0        0     2298 2023-07-10 14:23:02.733708 orwynn-1.0.0rc2/orwynn/cli/cli.py
--rw-r--r--   0        0        0      363 2023-07-10 14:08:27.708229 orwynn-1.0.0rc2/orwynn/cli/enums.py
--rw-r--r--   0        0        0      394 2023-07-10 14:08:51.966173 orwynn-1.0.0rc2/orwynn/cli/models.py
--rw-r--r--   0        0        0       73 2023-06-08 13:59:41.390353 orwynn-1.0.0rc2/orwynn/context/__init__.py
--rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/context/errors.py
--rw-r--r--   0        0        0      643 2023-06-08 13:59:41.391353 orwynn-1.0.0rc2/orwynn/context/manager.py
--rw-r--r--   0        0        0     2656 2023-06-08 13:55:46.418946 orwynn-1.0.0rc2/orwynn/context/storage.py
--rw-r--r--   0        0        0       97 2023-06-08 14:06:22.928960 orwynn-1.0.0rc2/orwynn/di/__init__.py
--rw-r--r--   0        0        0       69 2023-07-06 09:39:22.689224 orwynn-1.0.0rc2/orwynn/di/acceptor.py
--rw-r--r--   0        0        0     3780 2023-06-09 06:21:27.250456 orwynn-1.0.0rc2/orwynn/di/availability.py
--rw-r--r--   0        0        0     1742 2023-07-10 11:27:13.013752 orwynn-1.0.0rc2/orwynn/di/collecting/acceptordependencies.py
--rw-r--r--   0        0        0     1219 2023-06-08 14:24:49.757165 orwynn-1.0.0rc2/orwynn/di/collecting/errors.py
--rw-r--r--   0        0        0     3128 2023-06-09 06:20:20.113767 orwynn-1.0.0rc2/orwynn/di/collecting/helpers.py
--rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0rc2/orwynn/di/collecting/modulecollector.py
--rw-r--r--   0        0        0        0 2023-06-09 06:31:34.417910 orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/__init__.py
--rw-r--r--   0        0        0     3229 2023-06-09 06:20:20.111767 orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/collect.py
--rw-r--r--   0        0        0     2341 2023-06-09 07:32:02.380043 orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/map.py
--rw-r--r--   0        0        0     1759 2023-07-10 13:45:40.439311 orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/test_main.py
--rw-r--r--   0        0        0     1084 2023-06-09 06:20:20.103768 orwynn-1.0.0rc2/orwynn/di/collecting/test_modules.py
--rw-r--r--   0        0        0      840 2023-06-08 14:24:49.775165 orwynn-1.0.0rc2/orwynn/di/constants.py
--rw-r--r--   0        0        0     5895 2023-06-09 07:32:02.385042 orwynn-1.0.0rc2/orwynn/di/container.py
--rw-r--r--   0        0        0     4694 2023-07-10 12:27:55.169185 orwynn-1.0.0rc2/orwynn/di/di.py
--rw-r--r--   0        0        0     1260 2023-06-08 14:25:37.475430 orwynn-1.0.0rc2/orwynn/di/errors.py
--rw-r--r--   0        0        0     6756 2023-06-09 06:20:20.110767 orwynn-1.0.0rc2/orwynn/di/init/acceptors.py
--rw-r--r--   0        0        0     4115 2023-06-09 06:22:50.702901 orwynn-1.0.0rc2/orwynn/di/init/providers.py
--rw-r--r--   0        0        0     3093 2023-07-10 13:45:40.439311 orwynn-1.0.0rc2/orwynn/di/init/test_acceptors.py
--rw-r--r--   0        0        0      492 2023-07-10 13:45:40.436311 orwynn-1.0.0rc2/orwynn/di/init/test_providers.py
--rw-r--r--   0        0        0      327 2023-06-08 14:06:45.172014 orwynn-1.0.0rc2/orwynn/di/isacceptor.py
--rw-r--r--   0        0        0      325 2023-06-08 14:09:24.648261 orwynn-1.0.0rc2/orwynn/di/isprovider.py
--rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0rc2/orwynn/di/object.py
--rw-r--r--   0        0        0       45 2023-07-06 09:39:13.705327 orwynn-1.0.0rc2/orwynn/di/provider.py
--rw-r--r--   0        0        0      535 2023-07-10 12:53:28.658639 orwynn-1.0.0rc2/orwynn/di/testing.py
--rw-r--r--   0        0        0       93 2023-07-10 14:34:03.676610 orwynn-1.0.0rc2/orwynn/helpers/address/__init__.py
--rw-r--r--   0        0        0     2080 2023-07-11 07:12:44.820534 orwynn-1.0.0rc2/orwynn/helpers/address/address.py
--rw-r--r--   0        0        0      200 2023-07-10 14:27:26.222387 orwynn-1.0.0rc2/orwynn/helpers/address/errors.py
--rw-r--r--   0        0        0      419 2023-07-11 07:13:16.868307 orwynn-1.0.0rc2/orwynn/helpers/address/regex.py
--rw-r--r--   0        0        0     1076 2023-07-11 07:12:44.821534 orwynn-1.0.0rc2/orwynn/helpers/address/test_main.py
--rw-r--r--   0        0        0      877 2023-06-09 06:03:05.647671 orwynn-1.0.0rc2/orwynn/helpers/constants.py
--rw-r--r--   0        0        0      813 2023-07-10 12:47:57.896389 orwynn-1.0.0rc2/orwynn/helpers/errors.py
--rw-r--r--   0        0        0     1130 2023-07-10 16:06:16.709892 orwynn-1.0.0rc2/orwynn/helpers/web.py
--rw-r--r--   0        0        0     1118 2023-06-09 06:20:20.105768 orwynn-1.0.0rc2/orwynn/http/__init__.py
--rw-r--r--   0        0        0      922 2023-06-09 06:20:20.109768 orwynn-1.0.0rc2/orwynn/http/constants.py
--rw-r--r--   0        0        0        0 2023-06-09 06:36:32.323279 orwynn-1.0.0rc2/orwynn/http/context/__init__.py
--rw-r--r--   0        0        0      959 2023-07-05 09:50:46.449134 orwynn-1.0.0rc2/orwynn/http/context/id.py
--rw-r--r--   0        0        0      617 2023-06-09 05:50:36.441513 orwynn-1.0.0rc2/orwynn/http/context/middleware/builtin.py
--rw-r--r--   0        0        0      754 2023-06-09 05:50:36.430513 orwynn-1.0.0rc2/orwynn/http/context/middleware/contextbuiltin.py
--rw-r--r--   0        0        0     1039 2023-07-10 13:45:40.440312 orwynn-1.0.0rc2/orwynn/http/context/test_main.py
--rw-r--r--   0        0        0        0 2023-06-09 06:36:14.697646 orwynn-1.0.0rc2/orwynn/http/controller/__init__.py
--rw-r--r--   0        0        0     5438 2023-07-10 16:06:16.713892 orwynn-1.0.0rc2/orwynn/http/controller/controller.py
--rw-r--r--   0        0        0        0 2023-06-09 06:36:46.319189 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/__init__.py
--rw-r--r--   0        0        0     1130 2023-06-09 05:49:31.580107 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/container.py
--rw-r--r--   0        0        0     1231 2023-06-09 05:49:40.023769 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/endpoint.py
--rw-r--r--   0        0        0      215 2023-06-09 05:51:12.418075 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/response.py
--rw-r--r--   0        0        0     2346 2023-07-10 12:57:39.935615 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/test_main.py
--rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/http/controller/errors.py
--rw-r--r--   0        0        0     8099 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/http/controller/test_main.py
--rw-r--r--   0        0        0        0 2023-06-09 12:19:12.185278 orwynn-1.0.0rc2/orwynn/http/cors/__init__.py
--rw-r--r--   0        0        0      429 2023-06-09 11:03:10.108801 orwynn-1.0.0rc2/orwynn/http/cors/cors.py
--rw-r--r--   0        0        0     3666 2023-07-10 13:45:40.443311 orwynn-1.0.0rc2/orwynn/http/cors/test_main.py
--rw-r--r--   0        0        0        0 2023-06-09 06:37:51.749042 orwynn-1.0.0rc2/orwynn/http/errorhandler/__init__.py
--rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.110767 orwynn-1.0.0rc2/orwynn/http/errorhandler/default.py
--rw-r--r--   0        0        0     1094 2023-06-09 05:50:36.426514 orwynn-1.0.0rc2/orwynn/http/errorhandler/middleware.py
--rw-r--r--   0        0        0     6448 2023-07-10 13:45:40.438311 orwynn-1.0.0rc2/orwynn/http/errorhandler/test_main.py
--rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0rc2/orwynn/http/errors.py
--rw-r--r--   0        0        0     4525 2023-06-09 05:47:03.116046 orwynn-1.0.0rc2/orwynn/http/log/logger.py
--rw-r--r--   0        0        0     1145 2023-06-09 05:50:42.043289 orwynn-1.0.0rc2/orwynn/http/log/middleware.py
--rw-r--r--   0        0        0        0 2023-06-09 06:38:13.602306 orwynn-1.0.0rc2/orwynn/http/middleware/__init__.py
--rw-r--r--   0        0        0      274 2023-06-09 05:50:36.430513 orwynn-1.0.0rc2/orwynn/http/middleware/builtinmiddleware.py
--rw-r--r--   0        0        0      652 2023-06-09 05:50:36.430513 orwynn-1.0.0rc2/orwynn/http/middleware/middleware.py
--rw-r--r--   0        0        0      327 2023-06-09 05:47:03.114046 orwynn-1.0.0rc2/orwynn/http/middleware/nextcall.py
--rw-r--r--   0        0        0     2285 2023-07-10 12:11:25.635467 orwynn-1.0.0rc2/orwynn/http/middleware/test_main.py
--rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0rc2/orwynn/http/requests.py
--rw-r--r--   0        0        0      577 2023-05-22 07:24:03.129227 orwynn-1.0.0rc2/orwynn/http/responses.py
--rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0rc2/orwynn/http/schema/validationvalue.py
--rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0rc2/orwynn/http/schema/value.py
--rw-r--r--   0        0        0      928 2023-07-10 13:45:40.442311 orwynn-1.0.0rc2/orwynn/http/test_responses.py
--rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0rc2/orwynn/http/testing.py
--rw-r--r--   0        0        0      145 2023-06-09 06:20:20.111767 orwynn-1.0.0rc2/orwynn/indication/__init__.py
--rw-r--r--   0        0        0      231 2023-06-09 05:51:42.027891 orwynn-1.0.0rc2/orwynn/indication/default.py
--rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/indication/errors.py
--rw-r--r--   0        0        0      186 2023-06-08 13:55:11.806546 orwynn-1.0.0rc2/orwynn/indication/indicatable.py
--rw-r--r--   0        0        0    11518 2023-06-09 07:31:49.349629 orwynn-1.0.0rc2/orwynn/indication/indication.py
--rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0rc2/orwynn/indication/indicator.py
--rw-r--r--   0        0        0     3422 2023-06-09 07:31:58.353224 orwynn-1.0.0rc2/orwynn/indication/test_main.py
--rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0rc2/orwynn/indication/type.py
--rw-r--r--   0        0        0      120 2023-06-09 06:20:20.115767 orwynn-1.0.0rc2/orwynn/log/__init__.py
--rw-r--r--   0        0        0      152 2023-06-09 05:51:55.299360 orwynn-1.0.0rc2/orwynn/log/config.py
--rw-r--r--   0        0        0     1972 2023-06-09 07:45:46.128730 orwynn-1.0.0rc2/orwynn/log/configure.py
--rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0rc2/orwynn/log/constants.py
--rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/log/errors.py
--rw-r--r--   0        0        0      870 2023-06-09 07:50:28.243651 orwynn-1.0.0rc2/orwynn/log/handler.py
--rw-r--r--   0        0        0      540 2023-06-09 05:52:01.299120 orwynn-1.0.0rc2/orwynn/log/helpers.py
--rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0rc2/orwynn/log/log.py
--rw-r--r--   0        0        0     1857 2023-07-10 13:48:38.598021 orwynn-1.0.0rc2/orwynn/log/test_main.py
--rw-r--r--   0        0        0     3774 2023-07-10 12:05:44.416709 orwynn-1.0.0rc2/orwynn/log/test_middleware.py
--rw-r--r--   0        0        0     1498 2023-07-10 12:05:51.324037 orwynn-1.0.0rc2/orwynn/log/test_websocketmiddleware.py
--rw-r--r--   0        0        0       83 2023-06-09 07:50:59.221569 orwynn-1.0.0rc2/orwynn/log/types.py
--rw-r--r--   0        0        0       29 2023-06-09 05:52:49.668187 orwynn-1.0.0rc2/orwynn/mapping/__init__.py
--rw-r--r--   0        0        0      667 2023-07-05 09:49:27.438110 orwynn-1.0.0rc2/orwynn/mapping/errors.py
--rw-r--r--   0        0        0     1808 2023-07-05 09:47:23.970713 orwynn-1.0.0rc2/orwynn/mapping/mapping.py
--rw-r--r--   0        0        0      504 2023-07-05 09:49:15.096266 orwynn-1.0.0rc2/orwynn/mapping/test_main.py
--rw-r--r--   0        0        0      216 2023-07-04 11:01:21.049070 orwynn-1.0.0rc2/orwynn/mongo/__init__.py
--rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0rc2/orwynn/mongo/clientsession.py
--rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0rc2/orwynn/mongo/config.py
--rw-r--r--   0        0        0     7634 2023-07-06 08:54:40.455677 orwynn-1.0.0rc2/orwynn/mongo/document/__init__.py
--rw-r--r--   0        0        0      578 2023-07-06 07:33:03.897136 orwynn-1.0.0rc2/orwynn/mongo/document/errors.py
--rw-r--r--   0        0        0     1134 2023-07-05 09:33:28.956933 orwynn-1.0.0rc2/orwynn/mongo/document/helpers.py
--rw-r--r--   0        0        0     1367 2023-07-05 09:33:28.955933 orwynn-1.0.0rc2/orwynn/mongo/document/test_converttoobjectid.py
--rw-r--r--   0        0        0      219 2023-07-10 13:45:40.437312 orwynn-1.0.0rc2/orwynn/mongo/document/test_create.py
--rw-r--r--   0        0        0      742 2023-07-06 07:53:44.416182 orwynn-1.0.0rc2/orwynn/mongo/document/test_get.py
--rw-r--r--   0        0        0      703 2023-07-06 08:55:42.984735 orwynn-1.0.0rc2/orwynn/mongo/document/test_inc.py
--rw-r--r--   0        0        0      275 2023-07-06 07:46:04.044931 orwynn-1.0.0rc2/orwynn/mongo/document/test_refresh.py
--rw-r--r--   0        0        0      230 2023-07-06 06:48:10.593442 orwynn-1.0.0rc2/orwynn/mongo/document/test_remove.py
--rw-r--r--   0        0        0      829 2023-07-06 08:55:42.984735 orwynn-1.0.0rc2/orwynn/mongo/document/test_set.py
--rw-r--r--   0        0        0     1312 2023-07-06 07:42:00.340990 orwynn-1.0.0rc2/orwynn/mongo/document/test_updateoperators.py
--rw-r--r--   0        0        0      708 2023-07-06 08:51:37.969595 orwynn-1.0.0rc2/orwynn/mongo/document/testing.py
--rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0rc2/orwynn/mongo/entity.py
--rw-r--r--   0        0        0      882 2023-07-05 09:49:15.103266 orwynn-1.0.0rc2/orwynn/mongo/errors.py
--rw-r--r--   0        0        0     3567 2023-06-09 05:54:25.941338 orwynn-1.0.0rc2/orwynn/mongo/mongo.py
--rw-r--r--   0        0        0     1354 2023-07-04 11:01:22.010065 orwynn-1.0.0rc2/orwynn/mongo/test_main.py
--rw-r--r--   0        0        0      430 2023-07-10 12:58:56.726342 orwynn-1.0.0rc2/orwynn/mongo/testing.py
--rw-r--r--   0        0        0     2829 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/proxy/boot.py
--rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0rc2/orwynn/proxy/indicationonly.py
--rw-r--r--   0        0        0       27 2023-06-09 05:56:44.921784 orwynn-1.0.0rc2/orwynn/router/__init__.py
--rw-r--r--   0        0        0     4039 2023-07-11 07:16:51.954798 orwynn-1.0.0rc2/orwynn/router/errorhandlermanager.py
--rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/router/errors.py
--rw-r--r--   0        0        0    14253 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/router/register/controller.py
--rw-r--r--   0        0        0     9646 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/router/register/middleware.py
--rw-r--r--   0        0        0     2565 2023-06-09 11:05:03.696488 orwynn-1.0.0rc2/orwynn/router/router.py
--rw-r--r--   0        0        0     2640 2023-07-10 13:45:40.441311 orwynn-1.0.0rc2/orwynn/router/test_globalroute.py
--rw-r--r--   0        0        0       86 2023-07-11 07:49:30.101961 orwynn-1.0.0rc2/orwynn/server/__init__.py
--rw-r--r--   0        0        0      215 2023-07-11 07:41:29.452106 orwynn-1.0.0rc2/orwynn/server/engine.py
--rw-r--r--   0        0        0     1834 2023-07-11 07:47:19.222962 orwynn-1.0.0rc2/orwynn/server/server.py
--rw-r--r--   0        0        0       33 2023-06-09 05:57:10.064779 orwynn-1.0.0rc2/orwynn/singleton/__init__.py
--rw-r--r--   0        0        0     1318 2023-06-09 06:27:33.730658 orwynn-1.0.0rc2/orwynn/singleton/singleton.py
--rw-r--r--   0        0        0      203 2023-06-09 06:20:20.112767 orwynn-1.0.0rc2/orwynn/sql/__init__.py
--rw-r--r--   0        0        0     1964 2023-06-09 06:00:27.751246 orwynn-1.0.0rc2/orwynn/sql/config.py
--rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0rc2/orwynn/sql/databasekind.py
--rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0rc2/orwynn/sql/poolclass.py
--rw-r--r--   0        0        0     3878 2023-06-09 06:00:31.786840 orwynn-1.0.0rc2/orwynn/sql/sql.py
--rw-r--r--   0        0        0     2636 2023-07-05 09:50:46.449134 orwynn-1.0.0rc2/orwynn/sql/table.py
--rw-r--r--   0        0        0     5895 2023-07-10 12:06:27.480702 orwynn-1.0.0rc2/orwynn/sql/test_main.py
--rw-r--r--   0        0        0      721 2023-06-09 06:00:51.915024 orwynn-1.0.0rc2/orwynn/testing/__init__.py
--rw-r--r--   0        0        0    11287 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/testing/client.py
--rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0rc2/orwynn/testing/embeddedclient.py
--rw-r--r--   0        0        0     2180 2023-07-10 13:45:40.441311 orwynn-1.0.0rc2/orwynn/testing/test_main.py
--rw-r--r--   0        0        0     1106 2023-05-22 08:13:58.515604 orwynn-1.0.0rc2/orwynn/testingtools/__init__.py
--rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0rc2/orwynn/utils/basesubclassable.py
--rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0rc2/orwynn/utils/crypto/__init__.py
--rw-r--r--   0        0        0      508 2023-06-09 07:42:13.220704 orwynn-1.0.0rc2/orwynn/utils/dt/__init__.py
--rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0rc2/orwynn/utils/fmt/__init__.py
--rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0rc2/orwynn/utils/fmt/test_main.py
--rw-r--r--   0        0        0     1973 2023-06-09 06:01:29.753531 orwynn-1.0.0rc2/orwynn/utils/klass/__init__.py
--rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0rc2/orwynn/utils/klass/errors.py
--rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0rc2/orwynn/utils/klass/test_klass.py
--rw-r--r--   0        0        0     2544 2023-06-09 06:01:41.912390 orwynn-1.0.0rc2/orwynn/utils/mp/__init__.py
--rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0rc2/orwynn/utils/mp/dictpp.py
--rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0rc2/orwynn/utils/mp/location.py
--rw-r--r--   0        0        0     1737 2023-06-09 06:01:41.912390 orwynn-1.0.0rc2/orwynn/utils/mp/test_main.py
--rw-r--r--   0        0        0      131 2023-07-05 09:50:46.441135 orwynn-1.0.0rc2/orwynn/utils/rnd/__init__.py
--rw-r--r--   0        0        0       90 2023-07-05 09:50:46.449134 orwynn-1.0.0rc2/orwynn/utils/rnd/test_main.py
--rw-r--r--   0        0        0      171 2023-07-10 16:06:21.903818 orwynn-1.0.0rc2/orwynn/utils/scheme.py
--rw-r--r--   0        0        0      423 2023-07-10 11:23:30.134562 orwynn-1.0.0rc2/orwynn/utils/types.py
--rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0rc2/orwynn/utils/uio.py
--rw-r--r--   0        0        0      680 2023-07-10 14:29:34.142049 orwynn-1.0.0rc2/orwynn/utils/url/__init__.py
--rw-r--r--   0        0        0     1921 2023-06-09 06:20:20.108768 orwynn-1.0.0rc2/orwynn/utils/url/helpers.py
--rw-r--r--   0        0        0     1405 2023-06-09 06:02:47.710864 orwynn-1.0.0rc2/orwynn/utils/url/test_utils.py
--rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0rc2/orwynn/utils/url/url.py
--rw-r--r--   0        0        0      419 2023-06-09 06:02:30.816698 orwynn-1.0.0rc2/orwynn/utils/url/utils.py
--rw-r--r--   0        0        0      253 2023-06-09 06:02:47.709865 orwynn-1.0.0rc2/orwynn/utils/url/vars.py
--rw-r--r--   0        0        0     9565 2023-07-10 12:38:01.181313 orwynn-1.0.0rc2/orwynn/utils/validation/__init__.py
--rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0rc2/orwynn/utils/validation/errors.py
--rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0rc2/orwynn/utils/validation/validator.py
--rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0rc2/orwynn/utils/yml/__init__.py
--rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/utils/yml/errors.py
--rw-r--r--   0        0        0      638 2023-06-09 06:20:20.115767 orwynn-1.0.0rc2/orwynn/websocket/__init__.py
--rw-r--r--   0        0        0      995 2023-06-09 06:20:20.113767 orwynn-1.0.0rc2/orwynn/websocket/constants.py
--rw-r--r--   0        0        0        0 2023-06-09 06:40:48.176846 orwynn-1.0.0rc2/orwynn/websocket/context/__init__.py
--rw-r--r--   0        0        0     1028 2023-07-05 09:50:46.450135 orwynn-1.0.0rc2/orwynn/websocket/context/id.py
--rw-r--r--   0        0        0      550 2023-06-09 06:20:10.146480 orwynn-1.0.0rc2/orwynn/websocket/context/middleware/builtin.py
--rw-r--r--   0        0        0      768 2023-06-09 06:20:10.146480 orwynn-1.0.0rc2/orwynn/websocket/context/middleware/contextbuiltin.py
--rw-r--r--   0        0        0     1296 2023-07-10 13:45:40.444311 orwynn-1.0.0rc2/orwynn/websocket/context/test_main.py
--rw-r--r--   0        0        0     3966 2023-06-09 06:20:10.146480 orwynn-1.0.0rc2/orwynn/websocket/controller/controller.py
--rw-r--r--   0        0        0      146 2023-06-08 13:55:11.806546 orwynn-1.0.0rc2/orwynn/websocket/controller/eventhandlermethod.py
--rw-r--r--   0        0        0     4067 2023-07-10 13:45:40.446311 orwynn-1.0.0rc2/orwynn/websocket/controller/test_controller.py
--rw-r--r--   0        0        0     3062 2023-07-10 12:08:27.941623 orwynn-1.0.0rc2/orwynn/websocket/controller/test_globalroute.py
--rw-r--r--   0        0        0      410 2023-06-09 06:16:27.158191 orwynn-1.0.0rc2/orwynn/websocket/errorhandler/default.py
--rw-r--r--   0        0        0     3514 2023-06-09 06:20:20.115767 orwynn-1.0.0rc2/orwynn/websocket/errorhandler/middleware.py
--rw-r--r--   0        0        0     1788 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/websocket/errorhandler/test_default.py
--rw-r--r--   0        0        0     1706 2023-06-09 06:16:27.191193 orwynn-1.0.0rc2/orwynn/websocket/log/logger.py
--rw-r--r--   0        0        0      910 2023-06-09 06:20:10.150480 orwynn-1.0.0rc2/orwynn/websocket/log/middleware.py
--rw-r--r--   0        0        0      303 2023-06-09 06:20:10.150480 orwynn-1.0.0rc2/orwynn/websocket/middleware/builtin.py
--rw-r--r--   0        0        0      856 2023-06-09 06:20:10.150480 orwynn-1.0.0rc2/orwynn/websocket/middleware/connectionbuiltin.py
--rw-r--r--   0        0        0      737 2023-06-09 06:20:10.149480 orwynn-1.0.0rc2/orwynn/websocket/middleware/middleware.py
--rw-r--r--   0        0        0      279 2023-06-09 06:16:27.159191 orwynn-1.0.0rc2/orwynn/websocket/middleware/nextcall.py
--rw-r--r--   0        0        0     1108 2023-07-10 13:45:40.443311 orwynn-1.0.0rc2/orwynn/websocket/middleware/test_main.py
--rw-r--r--   0        0        0      220 2023-06-09 06:16:27.190193 orwynn-1.0.0rc2/orwynn/websocket/routing/dispatchfn.py
--rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0rc2/orwynn/websocket/routing/genericfn.py
--rw-r--r--   0        0        0      427 2023-06-09 06:15:15.485170 orwynn-1.0.0rc2/orwynn/websocket/routing/handlers.py
--rw-r--r--   0        0        0     5607 2023-06-09 07:32:02.386042 orwynn-1.0.0rc2/orwynn/websocket/routing/helpers.py
--rw-r--r--   0        0        0     1880 2023-06-09 06:20:20.114767 orwynn-1.0.0rc2/orwynn/websocket/routing/nextcall.py
--rw-r--r--   0        0        0     6065 2023-06-09 06:16:27.192193 orwynn-1.0.0rc2/orwynn/websocket/routing/stack.py
--rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0rc2/orwynn/websocket/websocket.py
--rw-r--r--   0        0        0      928 2023-07-11 07:50:01.310419 orwynn-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 orwynn-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0rc3/LICENSE
+-rw-r--r--   0        0        0      307 2023-05-22 08:29:05.173562 orwynn-1.0.0rc3/README.md
+-rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0rc3/orwynn/__init__.py
+-rw-r--r--   0        0        0     1920 2023-06-08 13:46:47.770769 orwynn-1.0.0rc3/orwynn/apiversion/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0rc3/orwynn/apiversion/errors.py
+-rw-r--r--   0        0        0     4873 2023-07-10 13:45:40.443311 orwynn-1.0.0rc3/orwynn/apiversion/test_main.py
+-rw-r--r--   0        0        0       77 2023-06-08 13:47:49.293428 orwynn-1.0.0rc3/orwynn/app/__init__.py
+-rw-r--r--   0        0        0      400 2023-06-08 13:48:58.389784 orwynn-1.0.0rc3/orwynn/app/apirouter.py
+-rw-r--r--   0        0        0     1484 2023-06-08 13:47:28.661538 orwynn-1.0.0rc3/orwynn/app/apiwebsocketroute.py
+-rw-r--r--   0        0        0     2594 2023-06-09 12:20:44.292995 orwynn-1.0.0rc3/orwynn/app/app.py
+-rw-r--r--   0        0        0      188 2023-06-09 10:55:27.417944 orwynn-1.0.0rc3/orwynn/app/config.py
+-rw-r--r--   0        0        0     1560 2023-06-08 13:47:12.703403 orwynn-1.0.0rc3/orwynn/app/core.py
+-rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0rc3/orwynn/app/mode.py
+-rw-r--r--   0        0        0     2367 2023-07-10 13:45:40.440312 orwynn-1.0.0rc3/orwynn/app/test_main.py
+-rw-r--r--   0        0        0       98 2023-06-09 11:05:03.703488 orwynn-1.0.0rc3/orwynn/app/types.py
+-rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0rc3/orwynn/app/utils.py
+-rw-r--r--   0        0        0       56 2023-06-08 13:49:42.996486 orwynn-1.0.0rc3/orwynn/apprc/__init__.py
+-rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0rc3/orwynn/apprc/apprc.py
+-rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0rc3/orwynn/apprc/constants.py
+-rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0rc3/orwynn/apprc/errors.py
+-rw-r--r--   0        0        0     3493 2023-06-08 13:49:43.002486 orwynn-1.0.0rc3/orwynn/apprc/parse.py
+-rw-r--r--   0        0        0     2724 2023-07-10 12:01:27.295418 orwynn-1.0.0rc3/orwynn/apprc/test_main.py
+-rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0rc3/orwynn/base/__init__.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:49:50.224117 orwynn-1.0.0rc3/orwynn/base/config/__init__.py
+-rw-r--r--   0        0        0     1109 2023-06-09 05:54:54.979178 orwynn-1.0.0rc3/orwynn/base/config/config.py
+-rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0rc3/orwynn/base/config/test_config.py
+-rw-r--r--   0        0        0       35 2023-06-08 13:50:00.474596 orwynn-1.0.0rc3/orwynn/base/controller/__init__.py
+-rw-r--r--   0        0        0     2211 2023-07-06 09:35:56.327943 orwynn-1.0.0rc3/orwynn/base/controller/controller.py
+-rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0rc3/orwynn/base/controller/errors.py
+-rw-r--r--   0        0        0       31 2023-06-08 13:50:07.129259 orwynn-1.0.0rc3/orwynn/base/database/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-08 13:55:40.340226 orwynn-1.0.0rc3/orwynn/base/database/database.py
+-rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0rc3/orwynn/base/database/errors.py
+-rw-r--r--   0        0        0      203 2023-06-09 06:20:20.113767 orwynn-1.0.0rc3/orwynn/base/error/__init__.py
+-rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0rc3/orwynn/base/error/code.py
+-rw-r--r--   0        0        0      284 2023-06-08 13:54:00.170896 orwynn-1.0.0rc3/orwynn/base/error/errors.py
+-rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.112767 orwynn-1.0.0rc3/orwynn/base/error/test_main.py
+-rw-r--r--   0        0        0      436 2023-06-08 13:50:50.520080 orwynn-1.0.0rc3/orwynn/base/error/test_utils.py
+-rw-r--r--   0        0        0     2006 2023-06-08 13:54:17.686071 orwynn-1.0.0rc3/orwynn/base/error/utils.py
+-rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0rc3/orwynn/base/error/valueschema.py
+-rw-r--r--   0        0        0       39 2023-06-08 13:54:42.338917 orwynn-1.0.0rc3/orwynn/base/errorhandler/__init__.py
+-rw-r--r--   0        0        0     2354 2023-07-10 16:06:16.709892 orwynn-1.0.0rc3/orwynn/base/errorhandler/errorhandler.py
+-rw-r--r--   0        0        0       82 2023-06-08 13:55:03.438934 orwynn-1.0.0rc3/orwynn/base/middleware/__init__.py
+-rw-r--r--   0        0        0       94 2023-06-08 13:55:03.438934 orwynn-1.0.0rc3/orwynn/base/middleware/globalsetup.py
+-rw-r--r--   0        0        0     2919 2023-04-21 09:59:20.018394 orwynn-1.0.0rc3/orwynn/base/middleware/middleware.py
+-rw-r--r--   0        0        0     1281 2023-07-10 13:45:40.445311 orwynn-1.0.0rc3/orwynn/base/middleware/test_main.py
+-rw-r--r--   0        0        0       25 2023-06-08 13:55:11.806546 orwynn-1.0.0rc3/orwynn/base/model/__init__.py
+-rw-r--r--   0        0        0     1423 2023-07-06 09:10:08.307376 orwynn-1.0.0rc3/orwynn/base/model/model.py
+-rw-r--r--   0        0        0      791 2023-06-09 06:20:20.110767 orwynn-1.0.0rc3/orwynn/base/model/test_model.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:55:21.285106 orwynn-1.0.0rc3/orwynn/base/module/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0rc3/orwynn/base/module/errors.py
+-rw-r--r--   0        0        0     7183 2023-06-08 13:55:37.034379 orwynn-1.0.0rc3/orwynn/base/module/module.py
+-rw-r--r--   0        0        0      950 2023-06-08 13:55:21.291106 orwynn-1.0.0rc3/orwynn/base/module/test_module.py
+-rw-r--r--   0        0        0       69 2023-06-08 13:55:40.340226 orwynn-1.0.0rc3/orwynn/base/service/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-08 13:55:40.342226 orwynn-1.0.0rc3/orwynn/base/service/framework.py
+-rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0rc3/orwynn/base/service/service.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:55:46.418946 orwynn-1.0.0rc3/orwynn/base/worker/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-09 05:57:10.064779 orwynn-1.0.0rc3/orwynn/base/worker/worker.py
+-rw-r--r--   0        0        0       54 2023-06-08 13:56:30.127942 orwynn-1.0.0rc3/orwynn/boot/__init__.py
+-rw-r--r--   0        0        0    12600 2023-07-10 13:48:28.037990 orwynn-1.0.0rc3/orwynn/boot/boot.py
+-rw-r--r--   0        0        0      716 2023-06-09 05:54:54.987177 orwynn-1.0.0rc3/orwynn/boot/config.py
+-rw-r--r--   0        0        0       95 2023-06-08 13:58:33.909354 orwynn-1.0.0rc3/orwynn/boot/errors.py
+-rw-r--r--   0        0        0     5375 2023-07-10 12:56:58.086353 orwynn-1.0.0rc3/orwynn/boot/test_main.py
+-rw-r--r--   0        0        0      154 2023-06-09 06:20:20.102768 orwynn-1.0.0rc3/orwynn/bootscript/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-10 12:10:57.216627 orwynn-1.0.0rc3/orwynn/bootscript/bootscript.py
+-rw-r--r--   0        0        0      114 2023-07-10 13:25:24.969000 orwynn-1.0.0rc3/orwynn/bootscript/callable.py
+-rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0rc3/orwynn/bootscript/calltime.py
+-rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0rc3/orwynn/bootscript/errors.py
+-rw-r--r--   0        0        0     1384 2023-07-10 13:45:40.440312 orwynn-1.0.0rc3/orwynn/bootscript/test_main.py
+-rw-r--r--   0        0        0     2523 2023-07-10 13:45:40.438311 orwynn-1.0.0rc3/orwynn/bootscript/worker.py
+-rw-r--r--   0        0        0       31 2023-07-10 13:55:28.842455 orwynn-1.0.0rc3/orwynn/cli/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-11 07:12:44.820534 orwynn-1.0.0rc3/orwynn/cli/__main__.py
+-rw-r--r--   0        0        0     2298 2023-07-10 14:23:02.733708 orwynn-1.0.0rc3/orwynn/cli/cli.py
+-rw-r--r--   0        0        0      363 2023-07-10 14:08:27.708229 orwynn-1.0.0rc3/orwynn/cli/enums.py
+-rw-r--r--   0        0        0      394 2023-07-10 14:08:51.966173 orwynn-1.0.0rc3/orwynn/cli/models.py
+-rw-r--r--   0        0        0       73 2023-06-08 13:59:41.390353 orwynn-1.0.0rc3/orwynn/context/__init__.py
+-rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0rc3/orwynn/context/errors.py
+-rw-r--r--   0        0        0      643 2023-06-08 13:59:41.391353 orwynn-1.0.0rc3/orwynn/context/manager.py
+-rw-r--r--   0        0        0     2656 2023-06-08 13:55:46.418946 orwynn-1.0.0rc3/orwynn/context/storage.py
+-rw-r--r--   0        0        0       97 2023-06-08 14:06:22.928960 orwynn-1.0.0rc3/orwynn/di/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-06 09:39:22.689224 orwynn-1.0.0rc3/orwynn/di/acceptor.py
+-rw-r--r--   0        0        0     3780 2023-06-09 06:21:27.250456 orwynn-1.0.0rc3/orwynn/di/availability.py
+-rw-r--r--   0        0        0     1742 2023-07-10 11:27:13.013752 orwynn-1.0.0rc3/orwynn/di/collecting/acceptordependencies.py
+-rw-r--r--   0        0        0     1219 2023-06-08 14:24:49.757165 orwynn-1.0.0rc3/orwynn/di/collecting/errors.py
+-rw-r--r--   0        0        0     3128 2023-06-09 06:20:20.113767 orwynn-1.0.0rc3/orwynn/di/collecting/helpers.py
+-rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0rc3/orwynn/di/collecting/modulecollector.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:31:34.417910 orwynn-1.0.0rc3/orwynn/di/collecting/providerdependencies/__init__.py
+-rw-r--r--   0        0        0     3229 2023-06-09 06:20:20.111767 orwynn-1.0.0rc3/orwynn/di/collecting/providerdependencies/collect.py
+-rw-r--r--   0        0        0     2341 2023-06-09 07:32:02.380043 orwynn-1.0.0rc3/orwynn/di/collecting/providerdependencies/map.py
+-rw-r--r--   0        0        0     1759 2023-07-10 13:45:40.439311 orwynn-1.0.0rc3/orwynn/di/collecting/providerdependencies/test_main.py
+-rw-r--r--   0        0        0     1084 2023-06-09 06:20:20.103768 orwynn-1.0.0rc3/orwynn/di/collecting/test_modules.py
+-rw-r--r--   0        0        0      840 2023-06-08 14:24:49.775165 orwynn-1.0.0rc3/orwynn/di/constants.py
+-rw-r--r--   0        0        0     5895 2023-06-09 07:32:02.385042 orwynn-1.0.0rc3/orwynn/di/container.py
+-rw-r--r--   0        0        0     4694 2023-07-10 12:27:55.169185 orwynn-1.0.0rc3/orwynn/di/di.py
+-rw-r--r--   0        0        0     1260 2023-06-08 14:25:37.475430 orwynn-1.0.0rc3/orwynn/di/errors.py
+-rw-r--r--   0        0        0     6756 2023-06-09 06:20:20.110767 orwynn-1.0.0rc3/orwynn/di/init/acceptors.py
+-rw-r--r--   0        0        0     4115 2023-06-09 06:22:50.702901 orwynn-1.0.0rc3/orwynn/di/init/providers.py
+-rw-r--r--   0        0        0     3093 2023-07-10 13:45:40.439311 orwynn-1.0.0rc3/orwynn/di/init/test_acceptors.py
+-rw-r--r--   0        0        0      492 2023-07-10 13:45:40.436311 orwynn-1.0.0rc3/orwynn/di/init/test_providers.py
+-rw-r--r--   0        0        0      327 2023-06-08 14:06:45.172014 orwynn-1.0.0rc3/orwynn/di/isacceptor.py
+-rw-r--r--   0        0        0      325 2023-06-08 14:09:24.648261 orwynn-1.0.0rc3/orwynn/di/isprovider.py
+-rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0rc3/orwynn/di/object.py
+-rw-r--r--   0        0        0       45 2023-07-06 09:39:13.705327 orwynn-1.0.0rc3/orwynn/di/provider.py
+-rw-r--r--   0        0        0      535 2023-07-10 12:53:28.658639 orwynn-1.0.0rc3/orwynn/di/testing.py
+-rw-r--r--   0        0        0       93 2023-07-10 14:34:03.676610 orwynn-1.0.0rc3/orwynn/helpers/address/__init__.py
+-rw-r--r--   0        0        0     2080 2023-07-11 07:12:44.820534 orwynn-1.0.0rc3/orwynn/helpers/address/address.py
+-rw-r--r--   0        0        0      200 2023-07-10 14:27:26.222387 orwynn-1.0.0rc3/orwynn/helpers/address/errors.py
+-rw-r--r--   0        0        0      419 2023-07-11 07:13:16.868307 orwynn-1.0.0rc3/orwynn/helpers/address/regex.py
+-rw-r--r--   0        0        0     1076 2023-07-11 07:12:44.821534 orwynn-1.0.0rc3/orwynn/helpers/address/test_main.py
+-rw-r--r--   0        0        0      877 2023-06-09 06:03:05.647671 orwynn-1.0.0rc3/orwynn/helpers/constants.py
+-rw-r--r--   0        0        0      813 2023-07-10 12:47:57.896389 orwynn-1.0.0rc3/orwynn/helpers/errors.py
+-rw-r--r--   0        0        0     1130 2023-07-10 16:06:16.709892 orwynn-1.0.0rc3/orwynn/helpers/web.py
+-rw-r--r--   0        0        0     1118 2023-06-09 06:20:20.105768 orwynn-1.0.0rc3/orwynn/http/__init__.py
+-rw-r--r--   0        0        0      922 2023-06-09 06:20:20.109768 orwynn-1.0.0rc3/orwynn/http/constants.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:32.323279 orwynn-1.0.0rc3/orwynn/http/context/__init__.py
+-rw-r--r--   0        0        0      959 2023-07-05 09:50:46.449134 orwynn-1.0.0rc3/orwynn/http/context/id.py
+-rw-r--r--   0        0        0      617 2023-06-09 05:50:36.441513 orwynn-1.0.0rc3/orwynn/http/context/middleware/builtin.py
+-rw-r--r--   0        0        0      754 2023-06-09 05:50:36.430513 orwynn-1.0.0rc3/orwynn/http/context/middleware/contextbuiltin.py
+-rw-r--r--   0        0        0     1039 2023-07-10 13:45:40.440312 orwynn-1.0.0rc3/orwynn/http/context/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:14.697646 orwynn-1.0.0rc3/orwynn/http/controller/__init__.py
+-rw-r--r--   0        0        0     5438 2023-07-10 16:06:16.713892 orwynn-1.0.0rc3/orwynn/http/controller/controller.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:46.319189 orwynn-1.0.0rc3/orwynn/http/controller/endpoint/__init__.py
+-rw-r--r--   0        0        0     1130 2023-06-09 05:49:31.580107 orwynn-1.0.0rc3/orwynn/http/controller/endpoint/container.py
+-rw-r--r--   0        0        0     1231 2023-06-09 05:49:40.023769 orwynn-1.0.0rc3/orwynn/http/controller/endpoint/endpoint.py
+-rw-r--r--   0        0        0      215 2023-06-09 05:51:12.418075 orwynn-1.0.0rc3/orwynn/http/controller/endpoint/response.py
+-rw-r--r--   0        0        0     2346 2023-07-10 12:57:39.935615 orwynn-1.0.0rc3/orwynn/http/controller/endpoint/test_main.py
+-rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0rc3/orwynn/http/controller/errors.py
+-rw-r--r--   0        0        0     8099 2023-07-10 16:06:16.720892 orwynn-1.0.0rc3/orwynn/http/controller/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:19:12.185278 orwynn-1.0.0rc3/orwynn/http/cors/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-09 11:03:10.108801 orwynn-1.0.0rc3/orwynn/http/cors/cors.py
+-rw-r--r--   0        0        0     3666 2023-07-10 13:45:40.443311 orwynn-1.0.0rc3/orwynn/http/cors/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:37:51.749042 orwynn-1.0.0rc3/orwynn/http/errorhandler/__init__.py
+-rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.110767 orwynn-1.0.0rc3/orwynn/http/errorhandler/default.py
+-rw-r--r--   0        0        0     1094 2023-06-09 05:50:36.426514 orwynn-1.0.0rc3/orwynn/http/errorhandler/middleware.py
+-rw-r--r--   0        0        0     6448 2023-07-10 13:45:40.438311 orwynn-1.0.0rc3/orwynn/http/errorhandler/test_main.py
+-rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0rc3/orwynn/http/errors.py
+-rw-r--r--   0        0        0     4525 2023-06-09 05:47:03.116046 orwynn-1.0.0rc3/orwynn/http/log/logger.py
+-rw-r--r--   0        0        0     1145 2023-06-09 05:50:42.043289 orwynn-1.0.0rc3/orwynn/http/log/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:13.602306 orwynn-1.0.0rc3/orwynn/http/middleware/__init__.py
+-rw-r--r--   0        0        0      274 2023-06-09 05:50:36.430513 orwynn-1.0.0rc3/orwynn/http/middleware/builtinmiddleware.py
+-rw-r--r--   0        0        0      652 2023-06-09 05:50:36.430513 orwynn-1.0.0rc3/orwynn/http/middleware/middleware.py
+-rw-r--r--   0        0        0      327 2023-06-09 05:47:03.114046 orwynn-1.0.0rc3/orwynn/http/middleware/nextcall.py
+-rw-r--r--   0        0        0     2285 2023-07-10 12:11:25.635467 orwynn-1.0.0rc3/orwynn/http/middleware/test_main.py
+-rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0rc3/orwynn/http/requests.py
+-rw-r--r--   0        0        0      577 2023-05-22 07:24:03.129227 orwynn-1.0.0rc3/orwynn/http/responses.py
+-rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0rc3/orwynn/http/schema/validationvalue.py
+-rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0rc3/orwynn/http/schema/value.py
+-rw-r--r--   0        0        0      928 2023-07-10 13:45:40.442311 orwynn-1.0.0rc3/orwynn/http/test_responses.py
+-rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0rc3/orwynn/http/testing.py
+-rw-r--r--   0        0        0      145 2023-06-09 06:20:20.111767 orwynn-1.0.0rc3/orwynn/indication/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-09 05:51:42.027891 orwynn-1.0.0rc3/orwynn/indication/default.py
+-rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0rc3/orwynn/indication/errors.py
+-rw-r--r--   0        0        0      186 2023-06-08 13:55:11.806546 orwynn-1.0.0rc3/orwynn/indication/indicatable.py
+-rw-r--r--   0        0        0    11518 2023-06-09 07:31:49.349629 orwynn-1.0.0rc3/orwynn/indication/indication.py
+-rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0rc3/orwynn/indication/indicator.py
+-rw-r--r--   0        0        0     3422 2023-06-09 07:31:58.353224 orwynn-1.0.0rc3/orwynn/indication/test_main.py
+-rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0rc3/orwynn/indication/type.py
+-rw-r--r--   0        0        0      120 2023-06-09 06:20:20.115767 orwynn-1.0.0rc3/orwynn/log/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-09 05:51:55.299360 orwynn-1.0.0rc3/orwynn/log/config.py
+-rw-r--r--   0        0        0     1972 2023-06-09 07:45:46.128730 orwynn-1.0.0rc3/orwynn/log/configure.py
+-rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0rc3/orwynn/log/constants.py
+-rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0rc3/orwynn/log/errors.py
+-rw-r--r--   0        0        0      870 2023-06-09 07:50:28.243651 orwynn-1.0.0rc3/orwynn/log/handler.py
+-rw-r--r--   0        0        0      540 2023-06-09 05:52:01.299120 orwynn-1.0.0rc3/orwynn/log/helpers.py
+-rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0rc3/orwynn/log/log.py
+-rw-r--r--   0        0        0     1857 2023-07-10 13:48:38.598021 orwynn-1.0.0rc3/orwynn/log/test_main.py
+-rw-r--r--   0        0        0     3774 2023-07-10 12:05:44.416709 orwynn-1.0.0rc3/orwynn/log/test_middleware.py
+-rw-r--r--   0        0        0     1498 2023-07-10 12:05:51.324037 orwynn-1.0.0rc3/orwynn/log/test_websocketmiddleware.py
+-rw-r--r--   0        0        0       83 2023-06-09 07:50:59.221569 orwynn-1.0.0rc3/orwynn/log/types.py
+-rw-r--r--   0        0        0       29 2023-06-09 05:52:49.668187 orwynn-1.0.0rc3/orwynn/mapping/__init__.py
+-rw-r--r--   0        0        0      667 2023-07-05 09:49:27.438110 orwynn-1.0.0rc3/orwynn/mapping/errors.py
+-rw-r--r--   0        0        0     1808 2023-07-05 09:47:23.970713 orwynn-1.0.0rc3/orwynn/mapping/mapping.py
+-rw-r--r--   0        0        0      504 2023-07-05 09:49:15.096266 orwynn-1.0.0rc3/orwynn/mapping/test_main.py
+-rw-r--r--   0        0        0      216 2023-07-04 11:01:21.049070 orwynn-1.0.0rc3/orwynn/mongo/__init__.py
+-rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0rc3/orwynn/mongo/clientsession.py
+-rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0rc3/orwynn/mongo/config.py
+-rw-r--r--   0        0        0     7634 2023-07-06 08:54:40.455677 orwynn-1.0.0rc3/orwynn/mongo/document/__init__.py
+-rw-r--r--   0        0        0      578 2023-07-06 07:33:03.897136 orwynn-1.0.0rc3/orwynn/mongo/document/errors.py
+-rw-r--r--   0        0        0     1134 2023-07-05 09:33:28.956933 orwynn-1.0.0rc3/orwynn/mongo/document/helpers.py
+-rw-r--r--   0        0        0     1367 2023-07-05 09:33:28.955933 orwynn-1.0.0rc3/orwynn/mongo/document/test_converttoobjectid.py
+-rw-r--r--   0        0        0      219 2023-07-10 13:45:40.437312 orwynn-1.0.0rc3/orwynn/mongo/document/test_create.py
+-rw-r--r--   0        0        0      742 2023-07-06 07:53:44.416182 orwynn-1.0.0rc3/orwynn/mongo/document/test_get.py
+-rw-r--r--   0        0        0      703 2023-07-06 08:55:42.984735 orwynn-1.0.0rc3/orwynn/mongo/document/test_inc.py
+-rw-r--r--   0        0        0      275 2023-07-06 07:46:04.044931 orwynn-1.0.0rc3/orwynn/mongo/document/test_refresh.py
+-rw-r--r--   0        0        0      230 2023-07-06 06:48:10.593442 orwynn-1.0.0rc3/orwynn/mongo/document/test_remove.py
+-rw-r--r--   0        0        0      829 2023-07-06 08:55:42.984735 orwynn-1.0.0rc3/orwynn/mongo/document/test_set.py
+-rw-r--r--   0        0        0     1312 2023-07-06 07:42:00.340990 orwynn-1.0.0rc3/orwynn/mongo/document/test_updateoperators.py
+-rw-r--r--   0        0        0      708 2023-07-06 08:51:37.969595 orwynn-1.0.0rc3/orwynn/mongo/document/testing.py
+-rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0rc3/orwynn/mongo/entity.py
+-rw-r--r--   0        0        0      882 2023-07-05 09:49:15.103266 orwynn-1.0.0rc3/orwynn/mongo/errors.py
+-rw-r--r--   0        0        0     3567 2023-06-09 05:54:25.941338 orwynn-1.0.0rc3/orwynn/mongo/mongo.py
+-rw-r--r--   0        0        0     1354 2023-07-04 11:01:22.010065 orwynn-1.0.0rc3/orwynn/mongo/test_main.py
+-rw-r--r--   0        0        0      430 2023-07-10 12:58:56.726342 orwynn-1.0.0rc3/orwynn/mongo/testing.py
+-rw-r--r--   0        0        0     2829 2023-07-10 16:06:16.720892 orwynn-1.0.0rc3/orwynn/proxy/boot.py
+-rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0rc3/orwynn/proxy/indicationonly.py
+-rw-r--r--   0        0        0       27 2023-06-09 05:56:44.921784 orwynn-1.0.0rc3/orwynn/router/__init__.py
+-rw-r--r--   0        0        0     4039 2023-07-11 07:16:51.954798 orwynn-1.0.0rc3/orwynn/router/errorhandlermanager.py
+-rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0rc3/orwynn/router/errors.py
+-rw-r--r--   0        0        0    14253 2023-07-10 16:06:16.720892 orwynn-1.0.0rc3/orwynn/router/register/controller.py
+-rw-r--r--   0        0        0     9646 2023-07-10 16:06:16.720892 orwynn-1.0.0rc3/orwynn/router/register/middleware.py
+-rw-r--r--   0        0        0     2565 2023-06-09 11:05:03.696488 orwynn-1.0.0rc3/orwynn/router/router.py
+-rw-r--r--   0        0        0     2640 2023-07-10 13:45:40.441311 orwynn-1.0.0rc3/orwynn/router/test_globalroute.py
+-rw-r--r--   0        0        0       86 2023-07-11 07:49:30.101961 orwynn-1.0.0rc3/orwynn/server/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-11 07:41:29.452106 orwynn-1.0.0rc3/orwynn/server/engine.py
+-rw-r--r--   0        0        0     1834 2023-07-11 07:47:19.222962 orwynn-1.0.0rc3/orwynn/server/server.py
+-rw-r--r--   0        0        0       33 2023-06-09 05:57:10.064779 orwynn-1.0.0rc3/orwynn/singleton/__init__.py
+-rw-r--r--   0        0        0     1318 2023-06-09 06:27:33.730658 orwynn-1.0.0rc3/orwynn/singleton/singleton.py
+-rw-r--r--   0        0        0      203 2023-06-09 06:20:20.112767 orwynn-1.0.0rc3/orwynn/sql/__init__.py
+-rw-r--r--   0        0        0     1964 2023-06-09 06:00:27.751246 orwynn-1.0.0rc3/orwynn/sql/config.py
+-rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0rc3/orwynn/sql/databasekind.py
+-rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0rc3/orwynn/sql/poolclass.py
+-rw-r--r--   0        0        0     3878 2023-06-09 06:00:31.786840 orwynn-1.0.0rc3/orwynn/sql/sql.py
+-rw-r--r--   0        0        0     2636 2023-07-05 09:50:46.449134 orwynn-1.0.0rc3/orwynn/sql/table.py
+-rw-r--r--   0        0        0     5895 2023-07-10 12:06:27.480702 orwynn-1.0.0rc3/orwynn/sql/test_main.py
+-rw-r--r--   0        0        0      721 2023-06-09 06:00:51.915024 orwynn-1.0.0rc3/orwynn/testing/__init__.py
+-rw-r--r--   0        0        0    11287 2023-07-10 16:06:16.720892 orwynn-1.0.0rc3/orwynn/testing/client.py
+-rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0rc3/orwynn/testing/embeddedclient.py
+-rw-r--r--   0        0        0     2180 2023-07-10 13:45:40.441311 orwynn-1.0.0rc3/orwynn/testing/test_main.py
+-rw-r--r--   0        0        0     1106 2023-05-22 08:13:58.515604 orwynn-1.0.0rc3/orwynn/testingtools/__init__.py
+-rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0rc3/orwynn/utils/basesubclassable.py
+-rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0rc3/orwynn/utils/crypto/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-09 07:42:13.220704 orwynn-1.0.0rc3/orwynn/utils/dt/__init__.py
+-rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0rc3/orwynn/utils/fmt/__init__.py
+-rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0rc3/orwynn/utils/fmt/test_main.py
+-rw-r--r--   0        0        0     1973 2023-06-09 06:01:29.753531 orwynn-1.0.0rc3/orwynn/utils/klass/__init__.py
+-rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0rc3/orwynn/utils/klass/errors.py
+-rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0rc3/orwynn/utils/klass/test_klass.py
+-rw-r--r--   0        0        0     2544 2023-06-09 06:01:41.912390 orwynn-1.0.0rc3/orwynn/utils/mp/__init__.py
+-rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0rc3/orwynn/utils/mp/dictpp.py
+-rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0rc3/orwynn/utils/mp/location.py
+-rw-r--r--   0        0        0     1737 2023-06-09 06:01:41.912390 orwynn-1.0.0rc3/orwynn/utils/mp/test_main.py
+-rw-r--r--   0        0        0      131 2023-07-05 09:50:46.441135 orwynn-1.0.0rc3/orwynn/utils/rnd/__init__.py
+-rw-r--r--   0        0        0       90 2023-07-05 09:50:46.449134 orwynn-1.0.0rc3/orwynn/utils/rnd/test_main.py
+-rw-r--r--   0        0        0      171 2023-07-10 16:06:21.903818 orwynn-1.0.0rc3/orwynn/utils/scheme.py
+-rw-r--r--   0        0        0      423 2023-07-10 11:23:30.134562 orwynn-1.0.0rc3/orwynn/utils/types.py
+-rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0rc3/orwynn/utils/uio.py
+-rw-r--r--   0        0        0      680 2023-07-10 14:29:34.142049 orwynn-1.0.0rc3/orwynn/utils/url/__init__.py
+-rw-r--r--   0        0        0     1921 2023-06-09 06:20:20.108768 orwynn-1.0.0rc3/orwynn/utils/url/helpers.py
+-rw-r--r--   0        0        0     1405 2023-06-09 06:02:47.710864 orwynn-1.0.0rc3/orwynn/utils/url/test_utils.py
+-rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0rc3/orwynn/utils/url/url.py
+-rw-r--r--   0        0        0      419 2023-06-09 06:02:30.816698 orwynn-1.0.0rc3/orwynn/utils/url/utils.py
+-rw-r--r--   0        0        0      253 2023-06-09 06:02:47.709865 orwynn-1.0.0rc3/orwynn/utils/url/vars.py
+-rw-r--r--   0        0        0     9565 2023-07-10 12:38:01.181313 orwynn-1.0.0rc3/orwynn/utils/validation/__init__.py
+-rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0rc3/orwynn/utils/validation/errors.py
+-rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0rc3/orwynn/utils/validation/validator.py
+-rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0rc3/orwynn/utils/yml/__init__.py
+-rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0rc3/orwynn/utils/yml/errors.py
+-rw-r--r--   0        0        0      638 2023-06-09 06:20:20.115767 orwynn-1.0.0rc3/orwynn/websocket/__init__.py
+-rw-r--r--   0        0        0      995 2023-06-09 06:20:20.113767 orwynn-1.0.0rc3/orwynn/websocket/constants.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:40:48.176846 orwynn-1.0.0rc3/orwynn/websocket/context/__init__.py
+-rw-r--r--   0        0        0     1028 2023-07-05 09:50:46.450135 orwynn-1.0.0rc3/orwynn/websocket/context/id.py
+-rw-r--r--   0        0        0      550 2023-06-09 06:20:10.146480 orwynn-1.0.0rc3/orwynn/websocket/context/middleware/builtin.py
+-rw-r--r--   0        0        0      768 2023-06-09 06:20:10.146480 orwynn-1.0.0rc3/orwynn/websocket/context/middleware/contextbuiltin.py
+-rw-r--r--   0        0        0     1296 2023-07-10 13:45:40.444311 orwynn-1.0.0rc3/orwynn/websocket/context/test_main.py
+-rw-r--r--   0        0        0     3966 2023-06-09 06:20:10.146480 orwynn-1.0.0rc3/orwynn/websocket/controller/controller.py
+-rw-r--r--   0        0        0      146 2023-06-08 13:55:11.806546 orwynn-1.0.0rc3/orwynn/websocket/controller/eventhandlermethod.py
+-rw-r--r--   0        0        0     4067 2023-07-10 13:45:40.446311 orwynn-1.0.0rc3/orwynn/websocket/controller/test_controller.py
+-rw-r--r--   0        0        0     3062 2023-07-10 12:08:27.941623 orwynn-1.0.0rc3/orwynn/websocket/controller/test_globalroute.py
+-rw-r--r--   0        0        0      410 2023-06-09 06:16:27.158191 orwynn-1.0.0rc3/orwynn/websocket/errorhandler/default.py
+-rw-r--r--   0        0        0     3514 2023-06-09 06:20:20.115767 orwynn-1.0.0rc3/orwynn/websocket/errorhandler/middleware.py
+-rw-r--r--   0        0        0     1788 2023-07-10 16:06:16.720892 orwynn-1.0.0rc3/orwynn/websocket/errorhandler/test_default.py
+-rw-r--r--   0        0        0     1706 2023-06-09 06:16:27.191193 orwynn-1.0.0rc3/orwynn/websocket/log/logger.py
+-rw-r--r--   0        0        0      910 2023-06-09 06:20:10.150480 orwynn-1.0.0rc3/orwynn/websocket/log/middleware.py
+-rw-r--r--   0        0        0      303 2023-06-09 06:20:10.150480 orwynn-1.0.0rc3/orwynn/websocket/middleware/builtin.py
+-rw-r--r--   0        0        0      856 2023-06-09 06:20:10.150480 orwynn-1.0.0rc3/orwynn/websocket/middleware/connectionbuiltin.py
+-rw-r--r--   0        0        0      737 2023-06-09 06:20:10.149480 orwynn-1.0.0rc3/orwynn/websocket/middleware/middleware.py
+-rw-r--r--   0        0        0      279 2023-06-09 06:16:27.159191 orwynn-1.0.0rc3/orwynn/websocket/middleware/nextcall.py
+-rw-r--r--   0        0        0     1108 2023-07-10 13:45:40.443311 orwynn-1.0.0rc3/orwynn/websocket/middleware/test_main.py
+-rw-r--r--   0        0        0      220 2023-06-09 06:16:27.190193 orwynn-1.0.0rc3/orwynn/websocket/routing/dispatchfn.py
+-rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0rc3/orwynn/websocket/routing/genericfn.py
+-rw-r--r--   0        0        0      427 2023-06-09 06:15:15.485170 orwynn-1.0.0rc3/orwynn/websocket/routing/handlers.py
+-rw-r--r--   0        0        0     5607 2023-06-09 07:32:02.386042 orwynn-1.0.0rc3/orwynn/websocket/routing/helpers.py
+-rw-r--r--   0        0        0     1880 2023-06-09 06:20:20.114767 orwynn-1.0.0rc3/orwynn/websocket/routing/nextcall.py
+-rw-r--r--   0        0        0     6065 2023-06-09 06:16:27.192193 orwynn-1.0.0rc3/orwynn/websocket/routing/stack.py
+-rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0rc3/orwynn/websocket/websocket.py
+-rw-r--r--   0        0        0      928 2023-07-14 15:16:20.087958 orwynn-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 orwynn-1.0.0rc3/PKG-INFO
```

### Comparing `orwynn-1.0.0rc2/LICENSE` & `orwynn-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/apiversion/__init__.py` & `orwynn-1.0.0rc3/orwynn/apiversion/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/apiversion/test_main.py` & `orwynn-1.0.0rc3/orwynn/apiversion/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/app/apiwebsocketroute.py` & `orwynn-1.0.0rc3/orwynn/app/apiwebsocketroute.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/app/app.py` & `orwynn-1.0.0rc3/orwynn/app/app.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/app/core.py` & `orwynn-1.0.0rc3/orwynn/app/core.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/app/test_main.py` & `orwynn-1.0.0rc3/orwynn/app/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/app/utils.py` & `orwynn-1.0.0rc3/orwynn/app/utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/apprc/parse.py` & `orwynn-1.0.0rc3/orwynn/apprc/parse.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/apprc/test_main.py` & `orwynn-1.0.0rc3/orwynn/apprc/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/config/config.py` & `orwynn-1.0.0rc3/orwynn/base/config/config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/controller/controller.py` & `orwynn-1.0.0rc3/orwynn/base/controller/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/database/database.py` & `orwynn-1.0.0rc3/orwynn/base/database/database.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/database/errors.py` & `orwynn-1.0.0rc3/orwynn/base/database/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/error/code.py` & `orwynn-1.0.0rc3/orwynn/base/error/code.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/error/test_main.py` & `orwynn-1.0.0rc3/orwynn/base/error/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/error/utils.py` & `orwynn-1.0.0rc3/orwynn/base/error/utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/errorhandler/errorhandler.py` & `orwynn-1.0.0rc3/orwynn/base/errorhandler/errorhandler.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/middleware/middleware.py` & `orwynn-1.0.0rc3/orwynn/base/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/middleware/test_main.py` & `orwynn-1.0.0rc3/orwynn/base/middleware/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/model/model.py` & `orwynn-1.0.0rc3/orwynn/base/model/model.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/model/test_model.py` & `orwynn-1.0.0rc3/orwynn/base/model/test_model.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/module/module.py` & `orwynn-1.0.0rc3/orwynn/base/module/module.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/base/module/test_module.py` & `orwynn-1.0.0rc3/orwynn/base/module/test_module.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/boot/boot.py` & `orwynn-1.0.0rc3/orwynn/boot/boot.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/boot/config.py` & `orwynn-1.0.0rc3/orwynn/boot/config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/boot/test_main.py` & `orwynn-1.0.0rc3/orwynn/boot/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/bootscript/test_main.py` & `orwynn-1.0.0rc3/orwynn/bootscript/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/bootscript/worker.py` & `orwynn-1.0.0rc3/orwynn/bootscript/worker.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/cli/cli.py` & `orwynn-1.0.0rc3/orwynn/cli/cli.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/context/manager.py` & `orwynn-1.0.0rc3/orwynn/context/manager.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/context/storage.py` & `orwynn-1.0.0rc3/orwynn/context/storage.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/availability.py` & `orwynn-1.0.0rc3/orwynn/di/availability.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/collecting/acceptordependencies.py` & `orwynn-1.0.0rc3/orwynn/di/collecting/acceptordependencies.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/collecting/errors.py` & `orwynn-1.0.0rc3/orwynn/di/collecting/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/collecting/helpers.py` & `orwynn-1.0.0rc3/orwynn/di/collecting/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/collecting/modulecollector.py` & `orwynn-1.0.0rc3/orwynn/di/collecting/modulecollector.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/collect.py` & `orwynn-1.0.0rc3/orwynn/di/collecting/providerdependencies/collect.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/map.py` & `orwynn-1.0.0rc3/orwynn/di/collecting/providerdependencies/map.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/test_main.py` & `orwynn-1.0.0rc3/orwynn/di/collecting/providerdependencies/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/collecting/test_modules.py` & `orwynn-1.0.0rc3/orwynn/di/collecting/test_modules.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/constants.py` & `orwynn-1.0.0rc3/orwynn/di/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/container.py` & `orwynn-1.0.0rc3/orwynn/di/container.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/di.py` & `orwynn-1.0.0rc3/orwynn/di/di.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/errors.py` & `orwynn-1.0.0rc3/orwynn/di/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/init/acceptors.py` & `orwynn-1.0.0rc3/orwynn/di/init/acceptors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/init/providers.py` & `orwynn-1.0.0rc3/orwynn/di/init/providers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/init/test_acceptors.py` & `orwynn-1.0.0rc3/orwynn/di/init/test_acceptors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/di/testing.py` & `orwynn-1.0.0rc3/orwynn/di/testing.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/helpers/address/address.py` & `orwynn-1.0.0rc3/orwynn/helpers/address/address.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/helpers/address/test_main.py` & `orwynn-1.0.0rc3/orwynn/helpers/address/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/helpers/constants.py` & `orwynn-1.0.0rc3/orwynn/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/helpers/errors.py` & `orwynn-1.0.0rc3/orwynn/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/helpers/web.py` & `orwynn-1.0.0rc3/orwynn/helpers/web.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/__init__.py` & `orwynn-1.0.0rc3/orwynn/http/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/constants.py` & `orwynn-1.0.0rc3/orwynn/http/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/context/id.py` & `orwynn-1.0.0rc3/orwynn/http/context/id.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/context/middleware/builtin.py` & `orwynn-1.0.0rc3/orwynn/http/context/middleware/builtin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/context/middleware/contextbuiltin.py` & `orwynn-1.0.0rc3/orwynn/http/context/middleware/contextbuiltin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/context/test_main.py` & `orwynn-1.0.0rc3/orwynn/http/context/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/controller/controller.py` & `orwynn-1.0.0rc3/orwynn/http/controller/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/controller/endpoint/container.py` & `orwynn-1.0.0rc3/orwynn/http/controller/endpoint/container.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/controller/endpoint/endpoint.py` & `orwynn-1.0.0rc3/orwynn/http/controller/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/controller/endpoint/test_main.py` & `orwynn-1.0.0rc3/orwynn/http/controller/endpoint/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/controller/test_main.py` & `orwynn-1.0.0rc3/orwynn/http/controller/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/cors/test_main.py` & `orwynn-1.0.0rc3/orwynn/http/cors/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/errorhandler/default.py` & `orwynn-1.0.0rc3/orwynn/http/errorhandler/default.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/errorhandler/middleware.py` & `orwynn-1.0.0rc3/orwynn/http/errorhandler/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/errorhandler/test_main.py` & `orwynn-1.0.0rc3/orwynn/http/errorhandler/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/log/logger.py` & `orwynn-1.0.0rc3/orwynn/http/log/logger.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/log/middleware.py` & `orwynn-1.0.0rc3/orwynn/http/log/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/middleware/middleware.py` & `orwynn-1.0.0rc3/orwynn/http/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/middleware/test_main.py` & `orwynn-1.0.0rc3/orwynn/http/middleware/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/responses.py` & `orwynn-1.0.0rc3/orwynn/http/responses.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/http/test_responses.py` & `orwynn-1.0.0rc3/orwynn/http/test_responses.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/indication/indication.py` & `orwynn-1.0.0rc3/orwynn/indication/indication.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/indication/test_main.py` & `orwynn-1.0.0rc3/orwynn/indication/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/log/configure.py` & `orwynn-1.0.0rc3/orwynn/log/configure.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/log/handler.py` & `orwynn-1.0.0rc3/orwynn/log/handler.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/log/helpers.py` & `orwynn-1.0.0rc3/orwynn/log/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/log/test_main.py` & `orwynn-1.0.0rc3/orwynn/log/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/log/test_middleware.py` & `orwynn-1.0.0rc3/orwynn/log/test_middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/log/test_websocketmiddleware.py` & `orwynn-1.0.0rc3/orwynn/log/test_websocketmiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mapping/errors.py` & `orwynn-1.0.0rc3/orwynn/mapping/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mapping/mapping.py` & `orwynn-1.0.0rc3/orwynn/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/document/__init__.py` & `orwynn-1.0.0rc3/orwynn/mongo/document/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/document/errors.py` & `orwynn-1.0.0rc3/orwynn/mongo/document/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/document/helpers.py` & `orwynn-1.0.0rc3/orwynn/mongo/document/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/document/test_converttoobjectid.py` & `orwynn-1.0.0rc3/orwynn/mongo/document/test_converttoobjectid.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/document/test_get.py` & `orwynn-1.0.0rc3/orwynn/mongo/document/test_get.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/document/test_inc.py` & `orwynn-1.0.0rc3/orwynn/mongo/document/test_inc.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/document/test_set.py` & `orwynn-1.0.0rc3/orwynn/mongo/document/test_set.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/document/test_updateoperators.py` & `orwynn-1.0.0rc3/orwynn/mongo/document/test_updateoperators.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/document/testing.py` & `orwynn-1.0.0rc3/orwynn/mongo/document/testing.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/errors.py` & `orwynn-1.0.0rc3/orwynn/mongo/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/mongo.py` & `orwynn-1.0.0rc3/orwynn/mongo/mongo.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/mongo/test_main.py` & `orwynn-1.0.0rc3/orwynn/mongo/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/proxy/boot.py` & `orwynn-1.0.0rc3/orwynn/proxy/boot.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/router/errorhandlermanager.py` & `orwynn-1.0.0rc3/orwynn/router/errorhandlermanager.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/router/register/controller.py` & `orwynn-1.0.0rc3/orwynn/router/register/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/router/register/middleware.py` & `orwynn-1.0.0rc3/orwynn/router/register/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/router/router.py` & `orwynn-1.0.0rc3/orwynn/router/router.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/router/test_globalroute.py` & `orwynn-1.0.0rc3/orwynn/router/test_globalroute.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/server/server.py` & `orwynn-1.0.0rc3/orwynn/server/server.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/singleton/singleton.py` & `orwynn-1.0.0rc3/orwynn/singleton/singleton.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/sql/config.py` & `orwynn-1.0.0rc3/orwynn/sql/config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/sql/sql.py` & `orwynn-1.0.0rc3/orwynn/sql/sql.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/sql/table.py` & `orwynn-1.0.0rc3/orwynn/sql/table.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/sql/test_main.py` & `orwynn-1.0.0rc3/orwynn/sql/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/testing/__init__.py` & `orwynn-1.0.0rc3/orwynn/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/testing/client.py` & `orwynn-1.0.0rc3/orwynn/testing/client.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/testing/test_main.py` & `orwynn-1.0.0rc3/orwynn/testing/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/testingtools/__init__.py` & `orwynn-1.0.0rc3/orwynn/testingtools/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/crypto/__init__.py` & `orwynn-1.0.0rc3/orwynn/utils/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/fmt/__init__.py` & `orwynn-1.0.0rc3/orwynn/utils/fmt/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/fmt/test_main.py` & `orwynn-1.0.0rc3/orwynn/utils/fmt/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/klass/__init__.py` & `orwynn-1.0.0rc3/orwynn/utils/klass/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/klass/test_klass.py` & `orwynn-1.0.0rc3/orwynn/utils/klass/test_klass.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/mp/__init__.py` & `orwynn-1.0.0rc3/orwynn/utils/mp/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/mp/location.py` & `orwynn-1.0.0rc3/orwynn/utils/mp/location.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/mp/test_main.py` & `orwynn-1.0.0rc3/orwynn/utils/mp/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/url/__init__.py` & `orwynn-1.0.0rc3/orwynn/utils/url/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/url/helpers.py` & `orwynn-1.0.0rc3/orwynn/utils/url/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/url/test_utils.py` & `orwynn-1.0.0rc3/orwynn/utils/url/test_utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/validation/__init__.py` & `orwynn-1.0.0rc3/orwynn/utils/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/validation/errors.py` & `orwynn-1.0.0rc3/orwynn/utils/validation/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/utils/yml/__init__.py` & `orwynn-1.0.0rc3/orwynn/utils/yml/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/__init__.py` & `orwynn-1.0.0rc3/orwynn/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/constants.py` & `orwynn-1.0.0rc3/orwynn/websocket/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/context/id.py` & `orwynn-1.0.0rc3/orwynn/websocket/context/id.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/context/middleware/builtin.py` & `orwynn-1.0.0rc3/orwynn/websocket/context/middleware/builtin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/context/middleware/contextbuiltin.py` & `orwynn-1.0.0rc3/orwynn/websocket/context/middleware/contextbuiltin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/context/test_main.py` & `orwynn-1.0.0rc3/orwynn/websocket/context/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/controller/controller.py` & `orwynn-1.0.0rc3/orwynn/websocket/controller/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/controller/test_controller.py` & `orwynn-1.0.0rc3/orwynn/websocket/controller/test_controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/controller/test_globalroute.py` & `orwynn-1.0.0rc3/orwynn/websocket/controller/test_globalroute.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/errorhandler/middleware.py` & `orwynn-1.0.0rc3/orwynn/websocket/errorhandler/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/errorhandler/test_default.py` & `orwynn-1.0.0rc3/orwynn/websocket/errorhandler/test_default.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/log/logger.py` & `orwynn-1.0.0rc3/orwynn/websocket/log/logger.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/log/middleware.py` & `orwynn-1.0.0rc3/orwynn/websocket/log/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/middleware/connectionbuiltin.py` & `orwynn-1.0.0rc3/orwynn/websocket/middleware/connectionbuiltin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/middleware/middleware.py` & `orwynn-1.0.0rc3/orwynn/websocket/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/middleware/test_main.py` & `orwynn-1.0.0rc3/orwynn/websocket/middleware/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/routing/helpers.py` & `orwynn-1.0.0rc3/orwynn/websocket/routing/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/routing/nextcall.py` & `orwynn-1.0.0rc3/orwynn/websocket/routing/nextcall.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/orwynn/websocket/routing/stack.py` & `orwynn-1.0.0rc3/orwynn/websocket/routing/stack.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc2/pyproject.toml` & `orwynn-1.0.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "orwynn"
-version = "1.0.0rc2"
+version = "1.0.0rc3"
 description = "Scalable web-framework with out-of-the-box architecture"
 authors = ["ryzhovalex <thed4rkof@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.88.0"
 uvicorn = {extras = ["standard"], version = "^0.20.0"}
 loguru = "^0.6.0"
 pyyaml = "^6.0"
 pyjwt = "^2.6.0"
-httpx = "^0.23.1"
+httpx = "^0.24.1"
 colorama = "^0.4.6"
 pymongo = "^4.3.3"
 python-dotenv = "^0.21.0"
 bcrypt = "^4.0.1"
 websockets = "^10.4"
 dictdiffer = "^0.9.0"
 python-benedict = "^0.28.1"
```

### Comparing `orwynn-1.0.0rc2/PKG-INFO` & `orwynn-1.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: orwynn
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Scalable web-framework with out-of-the-box architecture
 Author: ryzhovalex
 Author-email: thed4rkof@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
 Requires-Dist: fastapi (>=0.88.0,<0.89.0)
-Requires-Dist: httpx (>=0.23.1,<0.24.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: python-benedict (>=0.28.1,<0.29.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
```

