# Comparing `tmp/fastapi_jsonapi-1.0.1.tar.gz` & `tmp/fastapi_jsonapi-1.1.0.tar.gz`

## Comparing `fastapi_jsonapi-1.0.1.tar` & `fastapi_jsonapi-1.1.0.tar`

### file list

```diff
@@ -1,113 +1,118 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/__init__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/custom_filter_example.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/asgi.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/config.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/main.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/urls.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/__init__.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/base.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/child.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/parent.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/post.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/user.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/user_bio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/extensions/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/exceptions.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/faker.py
--rw-r--r--   0        0        0     9053 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/meta_base.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/post.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/user.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/user_bio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/__init__.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/meta_base.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/update_post.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/update_user.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/child.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/enums.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/parent.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/parent_child_association.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/post.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/post_comment.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/user.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/user_bio.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/__init__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/child.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/parent.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/post.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/post_comment.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/user.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/user_bio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/asgi.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/main.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/urls.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/api/__init__.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/api/user.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/faker.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/enums.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/pydantic/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/pydantic/user.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/tortoise/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/tortoise/user.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/__init__.py
--rw-r--r--   0        0        0    22987 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/api.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/jsonapi_typing.py
--rw-r--r--   0        0        0    15106 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/methods.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/querystring.py
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/schema.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/schema_base.py
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/signature.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/splitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/__init__.py
--rw-r--r--   0        0        0    14282 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/base.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/data_typing.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/orm.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/shared.py
--rw-r--r--   0        0        0    24198 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sqlalchemy_engine.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/tortoise_orm_engine.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/fields/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/fields/enum.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/fields/mixins.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/__init__.py
--rw-r--r--   0        0        0    10236 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/__init__.py
--rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/base.py
--rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/json_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/detail_view.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/list_view.py
--rw-r--r--   0        0        0    13121 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/view_base.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/LICENSE
--rw-r--r--   0        0        0     7059 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/README.md
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/custom_filter_example.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/asgi.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/config.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/main.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/urls.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/api/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/api/child.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/api/parent.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/api/post.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/api/user.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/api/user_bio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/extensions/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/factories/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/factories/faker.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/factories/post.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/factories/user.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/factories/user_bio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/updaters/__init__.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/updaters/update_post.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/updaters/update_user.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/child.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/enums.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/parent.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/parent_child_association.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/post.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/post_comment.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/user.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/user_bio.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/__init__.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/child.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/parent.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/post.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/user.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/asgi.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/main.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/urls.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/api/__init__.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/api/user.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/factories/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/factories/faker.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/factories/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/models/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/models/enums.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/models/pydantic/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/models/pydantic/user.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/models/tortoise/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/models/tortoise/user.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/__init__.py
+-rw-r--r--   0        0        0    22987 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/api.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/jsonapi_typing.py
+-rw-r--r--   0        0        0    15106 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/methods.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/querystring.py
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/schema.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/schema_base.py
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/signature.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/splitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/__init__.py
+-rw-r--r--   0        0        0    14282 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/base.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/data_typing.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/orm.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/shared.py
+-rw-r--r--   0        0        0    24198 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/sqlalchemy_engine.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/tortoise_orm_engine.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/fields/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/fields/enum.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/fields/mixins.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/filtering/__init__.py
+-rw-r--r--   0        0        0    10236 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/sorting/__init__.py
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/exceptions/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/exceptions/base.py
+-rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/exceptions/json_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/factories/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/factories/exceptions.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/factories/meta_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/generics/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/generics/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/updaters/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/updaters/exceptions.py
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/updaters/meta_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/views/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/views/detail_view.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/views/list_view.py
+-rw-r--r--   0        0        0    13121 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/fastapi_jsonapi/views/view_base.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7059 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/README.md
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.1.0/PKG-INFO
```

### Comparing `fastapi_jsonapi-1.0.1/examples/custom_filter_example.py` & `fastapi_jsonapi-1.1.0/examples/custom_filter_example.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/main.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/urls.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/urls.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/post.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/api/post.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from fastapi import Depends
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.ext.asyncio import AsyncSession
 from starlette import status
 
-from examples.api_for_sqlalchemy.api.base import DetailViewBaseGeneric, ListViewBaseGeneric
 from examples.api_for_sqlalchemy.extensions.sqlalchemy import Connector
-from examples.api_for_sqlalchemy.helpers.factories.meta_base import FactoryUseMode
 from examples.api_for_sqlalchemy.helpers.factories.post import ErrorCreatePostObject, PostFactory
 from examples.api_for_sqlalchemy.models.schemas import (
     PostInSchema,
 )
 from fastapi_jsonapi import SqlalchemyEngine
 from fastapi_jsonapi.exceptions import (
     BadRequest,
     HTTPException,
 )
+from fastapi_jsonapi.misc.sqla.factories.meta_base import FactoryUseMode
+from fastapi_jsonapi.misc.sqla.generics.base import DetailViewBaseGeneric, ListViewBaseGeneric
 from fastapi_jsonapi.querystring import QueryStringManager
 from fastapi_jsonapi.schema import JSONAPIResultDetailSchema
 
 
 class PostDetail(DetailViewBaseGeneric):
-    ...
+    session_dependency = Depends(Connector.get_session)
 
 
 class PostList(ListViewBaseGeneric):
+    session_dependency = Depends(Connector.get_session)
+
     async def post(
         self,
         data: PostInSchema,
         query_params: QueryStringManager,
-        session: AsyncSession = Depends(Connector.get_session),
+        session: AsyncSession = session_dependency,
     ) -> JSONAPIResultDetailSchema:
         try:
             post_obj = await PostFactory.create(
                 data=data.dict(),
                 mode=FactoryUseMode.production,
                 header=query_params.headers,
                 session=session,
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/api/user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from fastapi import Depends, status
 from sqlalchemy.ext.asyncio import AsyncSession
 
-from examples.api_for_sqlalchemy.api.base import DetailViewBaseGeneric, ListViewBaseGeneric
 from examples.api_for_sqlalchemy.extensions.sqlalchemy import Connector
-from examples.api_for_sqlalchemy.helpers.factories.meta_base import FactoryUseMode
 from examples.api_for_sqlalchemy.helpers.factories.user import ErrorCreateUserObject, UserFactory
-from examples.api_for_sqlalchemy.helpers.updaters.exceptions import ObjectNotFound
 from examples.api_for_sqlalchemy.helpers.updaters.update_user import ErrorUpdateUserObject, UpdateUser
 from examples.api_for_sqlalchemy.models import User
 from examples.api_for_sqlalchemy.models.schemas import UserPatchSchema, UserSchema
 from examples.api_for_sqlalchemy.models.schemas.user import UserInSchema
 from fastapi_jsonapi import SqlalchemyEngine
 from fastapi_jsonapi.exceptions import (
     BadRequest,
     HTTPException,
 )
+from fastapi_jsonapi.misc.sqla.factories.meta_base import FactoryUseMode
+from fastapi_jsonapi.misc.sqla.generics.base import DetailViewBaseGeneric, ListViewBaseGeneric
+from fastapi_jsonapi.misc.sqla.updaters.exceptions import ObjectNotFound
 from fastapi_jsonapi.querystring import QueryStringManager
 from fastapi_jsonapi.schema import JSONAPIResultDetailSchema
 
 
 class UserDetail(DetailViewBaseGeneric):
+    session_dependency = Depends(Connector.get_session)
+
     @classmethod
     async def patch(
         cls,
         obj_id,
         data: UserPatchSchema,
         query_params: QueryStringManager,
-        session: AsyncSession = Depends(Connector.get_session),
+        session: AsyncSession = session_dependency,
     ) -> UserSchema:
         user_obj: User
         try:
             user_obj = await UpdateUser.update(
                 obj_id,
                 data.dict(exclude_unset=True),
                 query_params.headers,
@@ -42,19 +44,21 @@
             raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=ex.description)
 
         user = UserSchema.from_orm(user_obj)
         return user
 
 
 class UserList(ListViewBaseGeneric):
+    session_dependency = Depends(Connector.get_session)
+
     async def post(
         self,
         data: UserInSchema,
         query_params: QueryStringManager,
-        session: AsyncSession = Depends(Connector.get_session),
+        session: AsyncSession = session_dependency,
     ) -> JSONAPIResultDetailSchema:
         user_obj: User = await UserFactory.create_object_generic(
             data_as_schema=data,
             query_params=query_params,
             session=session,
             exc=ErrorCreateUserObject,
             factory_mode=FactoryUseMode.production,
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/extensions/sqlalchemy.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/exceptions.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Create exceptions module."""
 
-from typing import Type, TypeVar
+from typing import Type
 
-from examples.api_for_sqlalchemy.extensions.sqlalchemy import Base
-
-TypeModel = TypeVar("TypeModel", bound=Base)
+from tortoise import models
 
 
 class ErrorCreateObject(Exception):
     """Base create object exception."""
 
-    def __init__(self, model: Type[TypeModel], description: str, field: str = ""):
+    def __init__(self, model: Type[models.Model], description: str, field: str = ""):
         """For a custom exception, you can define the model and error description."""
         self.model = model
         self.message = description
         self.field = field
         self.description = description
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/meta_base.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/factories/meta_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,28 @@
     Type,
     TypeVar,
     Union,
 )
 
 from pydantic import BaseModel
 from sqlalchemy.ext.asyncio import AsyncSession
+from sqlalchemy.ext.declarative import declarative_base
 
-from examples.api_for_sqlalchemy.extensions.sqlalchemy import Base
 from fastapi_jsonapi import BadRequest
 from fastapi_jsonapi.data_layers.fields.enum import Enum
 from fastapi_jsonapi.querystring import HeadersQueryStringManager, QueryStringManager
 
 from .exceptions import (
     ErrorCreateObject,
     ExceptionAfterCommit,
     ExceptionBeforeCreate,
     ExceptionNotFactory,
 )
 
+Base = declarative_base()
 TypeModel = TypeVar("TypeModel", bound=Base)
 
 
 class FactoryUseMode(Enum):
     """Effects the creation of an object in a factory. In test mode data generated randomly."""
 
     test = 1  # for tests, that is, data is generated randomly (unless specified explicitly)
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/post.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/factories/post.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import (
     Any,
     Dict,
     Union,
 )
 
 from examples.api_for_sqlalchemy.models import Post, User
-from fastapi_jsonapi.querystring import HeadersQueryStringManager
-
-from .exceptions import ErrorCreateObject
-from .faker import fake
-from .meta_base import (
+from fastapi_jsonapi.misc.sqla.factories.exceptions import ErrorCreateObject
+from fastapi_jsonapi.misc.sqla.factories.meta_base import (
     BaseFactory,
     FactoryUseMode,
 )
+from fastapi_jsonapi.querystring import HeadersQueryStringManager
+
+from .faker import fake
 
 
 class ErrorCreatePostObject(ErrorCreateObject):
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while creating object."""
         super().__init__(Post, description, field)
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/factories/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
     Any,
     Dict,
     Union,
 )
 
 from examples.api_for_sqlalchemy.models import User
 from examples.api_for_sqlalchemy.models.enums import UserStatusEnum
-from fastapi_jsonapi.querystring import HeadersQueryStringManager
-
-from .exceptions import ErrorCreateObject
-from .faker import fake
-from .meta_base import (
+from fastapi_jsonapi.misc.sqla.factories.exceptions import ErrorCreateObject
+from fastapi_jsonapi.misc.sqla.factories.meta_base import (
     BaseFactory,
     FactoryUseMode,
 )
+from fastapi_jsonapi.querystring import HeadersQueryStringManager
+
+from .faker import fake
 
 
 class ErrorCreateUserObject(ErrorCreateObject):
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while creating object."""
         super().__init__(User, description, field)
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/user_bio.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/factories/user_bio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import (
     Any,
     Dict,
     Union,
 )
 
 from examples.api_for_sqlalchemy.models import User, UserBio
-from fastapi_jsonapi.querystring import HeadersQueryStringManager
-
-from .exceptions import ErrorCreateObject
-from .faker import fake
-from .meta_base import (
+from fastapi_jsonapi.misc.sqla.factories.exceptions import ErrorCreateObject
+from fastapi_jsonapi.misc.sqla.factories.meta_base import (
     BaseFactory,
     FactoryUseMode,
 )
+from fastapi_jsonapi.querystring import HeadersQueryStringManager
+
+from .faker import fake
 
 
 class ErrorCreateUserBioObject(ErrorCreateObject):
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while creating object."""
         super().__init__(UserBio, description, field)
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/meta_base.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/updaters/meta_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,28 @@
     Type,
     TypeVar,
     Union,
 )
 
 from sqlalchemy import select
 from sqlalchemy.ext.asyncio import AsyncSession
-from tortoise import models
-from tortoise.exceptions import DoesNotExist
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm.exc import NoResultFound
 
 from fastapi_jsonapi.querystring import HeadersQueryStringManager
 
 from .exceptions import (
     ExceptionBeforeUpdate,
     ExceptionNotUpdater,
     ObjectNotFound,
 )
 
-TYPE_VAR = TypeVar("TYPE_VAR")
-TypeModel = TypeVar("TypeModel", bound=models.Model)
+Base = declarative_base()
+
+TypeModel = TypeVar("TypeModel", bound=Base)
 empty = object()
 
 
 class _BaseUpdater(Generic[TypeModel]):
     class Meta(object):
         model: Any
 
@@ -78,15 +79,15 @@
         :return: Model. Returns model from initialization or preloaded model.
         :raises ObjectNotFound: if object does not found.
         """
         if isinstance(model_or_id, int):
             try:
                 stmt = select(cls.Meta.model).where(cls.Meta.model.id == model_or_id)
                 model_instance = (await session.execute(stmt)).scalar_one()
-            except DoesNotExist:
+            except NoResultFound:
                 raise ObjectNotFound(cls.Meta.model, description="Object does not exist")
 
             return model_instance
         else:
             return model_or_id
 
     @classmethod
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/update_post.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/updaters/update_post.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 from typing import (
     Any,
     Dict,
     Union,
 )
 
 from examples.api_for_sqlalchemy.models import Post
-from fastapi_jsonapi.querystring import HeadersQueryStringManager
-
-from .exceptions import ErrorUpdateObject
-from .meta_base import (
+from fastapi_jsonapi.misc.sqla.updaters.exceptions import ErrorUpdateObject
+from fastapi_jsonapi.misc.sqla.updaters.meta_base import (
     BaseUpdater,
 )
+from fastapi_jsonapi.querystring import HeadersQueryStringManager
 
 
 class ErrorUpdatePostObject(ErrorUpdateObject):
     """Exception class for user update helper."""
 
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while updating object."""
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/update_user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 from typing import (
     Any,
     Dict,
     Optional,
     Union,
 )
 
-from examples.api_for_sqlalchemy.models import User
-from examples.api_for_sqlalchemy.models.enums import UserStatusEnum
 from fastapi_jsonapi.querystring import HeadersQueryStringManager
-
 from .exceptions import ErrorUpdateObject
 from .meta_base import (
     BaseUpdater,
 )
+from ...models.enums import UserStatusEnum
+from ...models.tortoise import User
 
 
 class ErrorUpdateUserObject(ErrorUpdateObject):
     """Exception class for user update helper."""
 
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while updating object."""
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/__init__.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/child.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/child.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/parent.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/parent.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/parent_child_association.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/parent_child_association.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/post.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/post.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/post_comment.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/post_comment.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/user_bio.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/user_bio.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/__init__.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/parent.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/parent.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/post.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/post.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/post_comment.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/user_bio.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/main.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/urls.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/urls.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/api/user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/api/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/exceptions.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/factories/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Create exceptions module."""
 
-from typing import Type
+from typing import Type, TypeVar
 
-from tortoise import models
+from sqlalchemy.ext.declarative import declarative_base
+
+Base = declarative_base()
+TypeModel = TypeVar("TypeModel", bound=Base)
 
 
 class ErrorCreateObject(Exception):
     """Base create object exception."""
 
-    def __init__(self, model: Type[models.Model], description: str, field: str = ""):
+    def __init__(self, model: Type[TypeModel], description: str, field: str = ""):
         """For a custom exception, you can define the model and error description."""
         self.model = model
         self.message = description
         self.field = field
         self.description = description
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/meta_base.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/factories/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/misc/sqla/updaters/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/update_user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_sqlalchemy/helpers/updaters/update_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from typing import (
     Any,
     Dict,
     Optional,
     Union,
 )
 
-from fastapi_jsonapi.querystring import HeadersQueryStringManager
-from .exceptions import ErrorUpdateObject
-from .meta_base import (
+from examples.api_for_sqlalchemy.models import User
+from examples.api_for_sqlalchemy.models.enums import UserStatusEnum
+from fastapi_jsonapi.misc.sqla.updaters.exceptions import ErrorUpdateObject
+from fastapi_jsonapi.misc.sqla.updaters.meta_base import (
     BaseUpdater,
 )
-from ...models.enums import UserStatusEnum
-from ...models.tortoise import User
+from fastapi_jsonapi.querystring import HeadersQueryStringManager
 
 
 class ErrorUpdateUserObject(ErrorUpdateObject):
     """Exception class for user update helper."""
 
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while updating object."""
```

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/pydantic/user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/models/pydantic/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/tortoise/user.py` & `fastapi_jsonapi-1.1.0/examples/api_for_tortoise_orm/models/tortoise/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/api.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/api.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/methods.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/methods.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/querystring.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/querystring.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/schema.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/schema_base.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/schema_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/signature.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/signature.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/base.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/shared.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/shared.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sqlalchemy_engine.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/sqlalchemy_engine.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/tortoise_orm_engine.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/tortoise_orm_engine.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/fields/mixins.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/__init__.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/base.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/json_api.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/exceptions/json_api.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/list_view.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/views/list_view.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/view_base.py` & `fastapi_jsonapi-1.1.0/fastapi_jsonapi/views/view_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/LICENSE` & `fastapi_jsonapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/README.md` & `fastapi_jsonapi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-1.0.1/pyproject.toml` & `fastapi_jsonapi-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 [tool.hatch.build.targets.wheel]
 packages = [
     "fastapi_jsonapi"
 ]
 
 [tool.poetry]
 name = "fastapi-jsonapi"
-version = "1.0.1"
+version = "1.1.0"
 description = "FastAPI extension to create REST web api according to JSON:API specification"
 authors = [
     "Aleksei Nekrasov <nekrasov.aleks@mail.ru>",
     "Suren Khorenyan <surenkhorenyan@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `fastapi_jsonapi-1.0.1/PKG-INFO` & `fastapi_jsonapi-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastAPI-JSONAPI
-Version: 1.0.1
+Version: 1.1.0
 Summary: FastAPI extension to create REST web api according to JSON:API 1.0 specification with FastAPI, Pydantic and data provider of your choice (SQLAlchemy, Tortoise ORM)
 Project-URL: Documentation, https://fastapi-jsonapi.readthedocs.io/
 Project-URL: Source, https://github.com/mts-ai/FastAPI-JSONAPI
 Author-email: Aleksey Nekrasov <a.nekrasov@mts.ai>, Suren Khorenyan <s.khorenyan@mts.ai>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: fastapi,json:api,jsonapi
```

