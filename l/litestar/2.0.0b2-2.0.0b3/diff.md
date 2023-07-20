# Comparing `tmp/litestar-2.0.0b2.tar.gz` & `tmp/litestar-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar-2.0.0b2.tar", max compression
+gzip compressed data, was "litestar-2.0.0b3.tar", max compression
```

## Comparing `litestar-2.0.0b2.tar` & `litestar-2.0.0b3.tar`

### file list

```diff
@@ -1,317 +1,312 @@
--rw-r--r--   0        0        0     1092 2023-06-24 19:32:57.844417 litestar-2.0.0b2/LICENSE
--rw-r--r--   0        0        0    51236 2023-06-24 19:32:57.848417 litestar-2.0.0b2/docs/PYPI_README.md
--rw-r--r--   0        0        0      744 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/__init__.py
--rw-r--r--   0        0        0      228 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/__main__.py
--rw-r--r--   0        0        0       77 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     6395 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0      349 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7823 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5977 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1267 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1528 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/utils.py
--rw-r--r--   0        0        0       66 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3842 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4239 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    14894 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20450 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2759 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_layers/utils.py
--rw-r--r--   0        0        0     5922 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_multipart.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0     9429 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5536 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     1213 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0     9629 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/responses.py
--rw-r--r--   0        0        0       64 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     3190 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2254 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    30936 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0      524 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    11000 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5240 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7685 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     1464 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/utils.py
--rw-r--r--   0        0        0     2338 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_parsers.py
--rw-r--r--   0        0        0      182 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/__init__.py
--rw-r--r--   0        0        0     7121 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/field.py
--rw-r--r--   0        0        0     4516 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/metadata.py
--rw-r--r--   0        0        0       64 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/models/__init__.py
--rw-r--r--   0        0        0    17165 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/models/attrs_signature_model.py
--rw-r--r--   0        0        0     5585 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/models/base.py
--rw-r--r--   0        0        0     7300 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/models/pydantic_signature_model.py
--rw-r--r--   0        0        0     5556 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/utils.py
--rw-r--r--   0        0        0    36404 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/app.py
--rw-r--r--   0        0        0     2200 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/background_tasks.py
--rw-r--r--   0        0        0      176 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     1300 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     2768 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     9422 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0    15726 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4647 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/channels/subscriber.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/__init__.py
--rw-r--r--   0        0        0    12711 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/_utils.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0     6630 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2568 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2381 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0     2125 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    11442 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/app.py
--rw-r--r--   0        0        0     2742 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/compression.py
--rw-r--r--   0        0        0     5182 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/csrf.py
--rw-r--r--   0        0        0     1991 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/connection/__init__.py
--rw-r--r--   0        0        0    10826 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/connection/base.py
--rw-r--r--   0        0        0     7698 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/connection/request.py
--rw-r--r--   0        0        0    11274 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/connection/websocket.py
--rw-r--r--   0        0        0     1363 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/constants.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4916 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4059 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     6408 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0     2557 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jinja.py
--rw-r--r--   0        0        0      521 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28722 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     4463 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     6986 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3983 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/mako.py
--rw-r--r--   0        0        0     2167 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/msgspec.py
--rw-r--r--   0        0        0      180 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4235 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2214 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0      207 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     2733 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/prometheus/config.py
--rw-r--r--   0        0        0     1646 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/prometheus/controller.py
--rw-r--r--   0        0        0     6766 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/prometheus/middleware.py
--rw-r--r--   0        0        0     2341 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/pydantic.py
--rw-r--r--   0        0        0      364 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0      162 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/abc/__init__.py
--rw-r--r--   0        0        0     8889 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/abc/_async.py
--rw-r--r--   0        0        0     8907 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/abc/_sync.py
--rw-r--r--   0        0        0      328 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0     2064 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      641 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/testing/__init__.py
--rw-r--r--   0        0        0    26054 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5535 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0     8773 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      941 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      319 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/_slots_base.py
--rw-r--r--   0        0        0      504 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      458 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0     4575 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0    11423 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0    11500 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0     3787 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0     1647 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0     1441 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0      288 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/__init__.py
--rw-r--r--   0        0        0    22904 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_async.py
--rw-r--r--   0        0        0    22646 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_sync.py
--rw-r--r--   0        0        0     1033 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_util.py
--rw-r--r--   0        0        0      754 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/types.py
--rw-r--r--   0        0        0     6359 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0     9545 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/controller.py
--rw-r--r--   0        0        0    16539 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/data_extractors.py
--rw-r--r--   0        0        0      883 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3762 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    17352 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     2977 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9646 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/state.py
--rw-r--r--   0        0        0     3310 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7273 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/url.py
--rw-r--r--   0        0        0     3117 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/di.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/__init__.py
--rw-r--r--   0        0        0      240 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/__init__.py
--rw-r--r--   0        0        0      245 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/__init__.py
--rw-r--r--   0        0        0    18286 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/abc.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/msgspec/__init__.py
--rw-r--r--   0        0        0     1327 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/msgspec/backend.py
--rw-r--r--   0        0        0     1691 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/msgspec/utils.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/pydantic/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/pydantic/backend.py
--rw-r--r--   0        0        0     1936 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/pydantic/utils.py
--rw-r--r--   0        0        0     3704 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/types.py
--rw-r--r--   0        0        0    14227 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/utils.py
--rw-r--r--   0        0        0     7692 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/abc.py
--rw-r--r--   0        0        0     1405 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/config.py
--rw-r--r--   0        0        0     3291 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/data_structures.py
--rw-r--r--   0        0        0      313 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/exc.py
--rw-r--r--   0        0        0     1388 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/field.py
--rw-r--r--   0        0        0       65 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/stdlib/__init__.py
--rw-r--r--   0        0        0     2144 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/stdlib/dataclass.py
--rw-r--r--   0        0        0      363 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/types.py
--rw-r--r--   0        0        0     4457 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/utils.py
--rw-r--r--   0        0        0     4442 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/interface.py
--rw-r--r--   0        0        0      309 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/types.py
--rw-r--r--   0        0        0     1728 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/enums.py
--rw-r--r--   0        0        0      201 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/events/__init__.py
--rw-r--r--   0        0        0     4371 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/events/emitter.py
--rw-r--r--   0        0        0     1313 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/events/listener.py
--rw-r--r--   0        0        0     1165 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1702 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0     4629 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5344 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/file_system.py
--rw-r--r--   0        0        0      559 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3868 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    20199 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     6450 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    26346 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    62224 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      340 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     7151 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    19091 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     3605 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/logging/_utils.py
--rw-r--r--   0        0        0    12050 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/logging/picologging.py
--rw-r--r--   0        0        0      860 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2081 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     3094 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3430 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5284 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/base.py
--rw-r--r--   0        0        0     8454 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/compression.py
--rw-r--r--   0        0        0     2573 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6466 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7210 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0     9435 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13330 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10811 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0       70 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     7935 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10365 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     8558 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      183 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5226 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/config.py
--rw-r--r--   0        0        0    15866 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/controller.py
--rw-r--r--   0        0        0      898 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1915 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2936 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      974 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      752 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4028 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6242 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    34574 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0    11029 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/pagination.py
--rw-r--r--   0        0        0    14893 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/params.py
--rw-r--r--   0        0        0     7097 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/partial.py
--rw-r--r--   0        0        0     3905 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/plugins.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/py.typed
--rw-r--r--   0        0        0      208 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/__init__.py
--rw-r--r--   0        0        0    15236 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/base.py
--rw-r--r--   0        0        0    14298 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/file.py
--rw-r--r--   0        0        0     5440 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/redirect.py
--rw-r--r--   0        0        0     7956 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/streaming.py
--rw-r--r--   0        0        0     5229 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/template.py
--rw-r--r--   0        0        0    15001 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/router.py
--rw-r--r--   0        0        0      191 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1719 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6437 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/base.py
--rw-r--r--   0        0        0    13244 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/http.py
--rw-r--r--   0        0        0     3002 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/__init__.py
--rw-r--r--   0        0        0     7165 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/base.py
--rw-r--r--   0        0        0      188 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5602 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     4978 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0     7714 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/serialization.py
--rw-r--r--   0        0        0      158 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5046 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/static_files/base.py
--rw-r--r--   0        0        0     3598 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/static_files/config.py
--rw-r--r--   0        0        0     9536 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/status_codes.py
--rw-r--r--   0        0        0        0 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4396 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/base.py
--rw-r--r--   0        0        0     5430 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/file.py
--rw-r--r--   0        0        0     3625 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/memory.py
--rw-r--r--   0        0        0     6231 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/redis.py
--rw-r--r--   0        0        0     2233 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/template/__init__.py
--rw-r--r--   0        0        0     4083 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/template/base.py
--rw-r--r--   0        0        0     1894 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/template/config.py
--rw-r--r--   0        0        0      581 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17562 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     5145 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19671 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0    30009 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2540 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    21927 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     8056 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/transport.py
--rw-r--r--   0        0        0     8564 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4073 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/__init__.py
--rw-r--r--   0        0        0     8930 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      566 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2962 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1872 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/composite_types.py
--rw-r--r--   0        0        0      272 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/empty.py
--rw-r--r--   0        0        0     2635 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/file_types.py
--rw-r--r--   0        0        0      781 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1924 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2984 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/protocols.py
--rw-r--r--   0        0        0     2005 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/serialization.py
--rw-r--r--   0        0        0     6479 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/typing.py
--rw-r--r--   0        0        0     2001 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/compat.py
--rw-r--r--   0        0        0     3645 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3520 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/deprecation.py
--rw-r--r--   0        0        0     3351 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/helpers.py
--rw-r--r--   0        0        0      723 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/path.py
--rw-r--r--   0        0        0    12066 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/predicates.py
--rw-r--r--   0        0        0     2823 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/scope.py
--rw-r--r--   0        0        0     1003 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/sequence.py
--rw-r--r--   0        0        0     8410 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/signature.py
--rw-r--r--   0        0        0     4374 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/sync.py
--rw-r--r--   0        0        0     8279 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/typing.py
--rw-r--r--   0        0        0     1921 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/version.py
--rw-r--r--   0        0        0     1992 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/warnings.py
--rw-r--r--   0        0        0    12929 2023-06-24 19:32:57.900416 litestar-2.0.0b2/pyproject.toml
--rw-r--r--   0        0        0    55447 1970-01-01 00:00:00.000000 litestar-2.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-20 13:51:29.954681 litestar-2.0.0b3/LICENSE
+-rw-r--r--   0        0        0    16756 2023-07-20 13:51:29.954681 litestar-2.0.0b3/docs/PYPI_README.md
+-rw-r--r--   0        0        0      744 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/__main__.py
+-rw-r--r--   0        0        0       77 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     6395 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7780 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5932 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1244 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3842 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4234 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    14983 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20484 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2808 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_layers/utils.py
+-rw-r--r--   0        0        0     6165 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_multipart.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0     9202 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     5536 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     1231 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0     9743 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     3250 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2250 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    24613 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0      524 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10909 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5220 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7664 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1460 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0     2396 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_parsers.py
+-rw-r--r--   0        0        0      126 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0    10095 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_signature/model.py
+-rw-r--r--   0        0        0     2718 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_signature/utils.py
+-rw-r--r--   0        0        0    36944 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/app.py
+-rw-r--r--   0        0        0     2200 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/background_tasks.py
+-rw-r--r--   0        0        0      176 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     1300 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     2750 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     9395 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0    15702 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4647 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0      119 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    12672 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6631 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2314 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2413 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0     2183 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    11706 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/app.py
+-rw-r--r--   0        0        0     2742 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/compression.py
+-rw-r--r--   0        0        0     5178 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/csrf.py
+-rw-r--r--   0        0        0     2005 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    10791 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/connection/base.py
+-rw-r--r--   0        0        0     7756 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/connection/request.py
+-rw-r--r--   0        0        0    11530 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/connection/websocket.py
+-rw-r--r--   0        0        0     1622 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/constants.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/attrs/__init__.py
+-rw-r--r--   0        0        0     2096 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/attrs/attrs_schema_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4800 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4167 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     6408 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2557 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28722 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     4373 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6953 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3983 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/mako.py
+-rw-r--r--   0        0        0      683 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/msgspec.py
+-rw-r--r--   0        0        0      180 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4235 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2214 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     3168 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/piccolo.py
+-rw-r--r--   0        0        0      207 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     2733 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/prometheus/config.py
+-rw-r--r--   0        0        0     1646 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/prometheus/controller.py
+-rw-r--r--   0        0        0     6873 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/prometheus/middleware.py
+-rw-r--r--   0        0        0      808 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0     3011 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_dto_factory.py
+-rw-r--r--   0        0        0     4571 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_init_plugin.py
+-rw-r--r--   0        0        0     8802 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_schema_plugin.py
+-rw-r--r--   0        0        0      364 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0      162 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/abc/__init__.py
+-rw-r--r--   0        0        0     8889 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/abc/_async.py
+-rw-r--r--   0        0        0     8907 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/abc/_sync.py
+-rw-r--r--   0        0        0      328 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     2064 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      641 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    25918 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5668 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0    11318 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      941 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      319 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/_slots_base.py
+-rw-r--r--   0        0        0      504 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      458 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     4541 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0    11423 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0    11483 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     3753 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0     1647 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0     1505 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0      288 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/__init__.py
+-rw-r--r--   0        0        0    28708 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_async.py
+-rw-r--r--   0        0        0    28402 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_sync.py
+-rw-r--r--   0        0        0     1033 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_util.py
+-rw-r--r--   0        0        0      754 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/types.py
+-rw-r--r--   0        0        0     6327 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0     9762 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/controller.py
+-rw-r--r--   0        0        0    16456 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/data_extractors.py
+-rw-r--r--   0        0        0      883 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3770 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    18809 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9646 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     2695 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7285 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/url.py
+-rw-r--r--   0        0        0     3117 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/di.py
+-rw-r--r--   0        0        0      645 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/__init__.py
+-rw-r--r--   0        0        0    21671 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/_backend.py
+-rw-r--r--   0        0        0     4261 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/_types.py
+-rw-r--r--   0        0        0    20517 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/_utils.py
+-rw-r--r--   0        0        0     7288 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/base_factory.py
+-rw-r--r--   0        0        0     2501 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/config.py
+-rw-r--r--   0        0        0     4858 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/data_structures.py
+-rw-r--r--   0        0        0     2507 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/dataclass_dto_factory.py
+-rw-r--r--   0        0        0     1325 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/factory/__init__.py
+-rw-r--r--   0        0        0      701 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/factory/stdlib/dataclass.py
+-rw-r--r--   0        0        0     1388 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/field.py
+-rw-r--r--   0        0        0     4948 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/interface.py
+-rw-r--r--   0        0        0     2113 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/msgspec_dto_factory.py
+-rw-r--r--   0        0        0      516 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/types.py
+-rw-r--r--   0        0        0     1728 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/enums.py
+-rw-r--r--   0        0        0      201 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4371 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/events/emitter.py
+-rw-r--r--   0        0        0     1313 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/events/listener.py
+-rw-r--r--   0        0        0     1302 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1721 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0      331 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/dto_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5344 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/file_system.py
+-rw-r--r--   0        0        0      559 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3868 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    21575 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     6450 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    26309 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    62224 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      340 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     7217 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    19092 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     3605 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    12215 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2079 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     3021 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3430 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5284 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/base.py
+-rw-r--r--   0        0        0     8454 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/compression.py
+-rw-r--r--   0        0        0     2554 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6438 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7141 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     9435 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13307 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10817 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7941 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10352 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8540 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      183 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0     5600 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/config.py
+-rw-r--r--   0        0        0    15653 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      724 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1885 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4028 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34581 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0    11029 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/pagination.py
+-rw-r--r--   0        0        0    15113 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/params.py
+-rw-r--r--   0        0        0     7433 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/partial.py
+-rw-r--r--   0        0        0     3923 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/plugins.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/py.typed
+-rw-r--r--   0        0        0      208 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/__init__.py
+-rw-r--r--   0        0        0    15238 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/base.py
+-rw-r--r--   0        0        0    14298 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/file.py
+-rw-r--r--   0        0        0     5440 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/redirect.py
+-rw-r--r--   0        0        0     7956 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/streaming.py
+-rw-r--r--   0        0        0     5229 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/template.py
+-rw-r--r--   0        0        0    15308 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/router.py
+-rw-r--r--   0        0        0      191 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1719 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6788 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/base.py
+-rw-r--r--   0        0        0    13224 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/http.py
+-rw-r--r--   0        0        0     3002 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/base.py
+-rw-r--r--   0        0        0      188 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4956 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0      348 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/serialization/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/serialization/_msgspec_utils.py
+-rw-r--r--   0        0        0     7755 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/serialization/msgspec_hooks.py
+-rw-r--r--   0        0        0      158 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5046 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/static_files/base.py
+-rw-r--r--   0        0        0     3598 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/static_files/config.py
+-rw-r--r--   0        0        0     9536 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/status_codes.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4396 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/base.py
+-rw-r--r--   0        0        0     5430 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/memory.py
+-rw-r--r--   0        0        0     6208 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2216 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/template/__init__.py
+-rw-r--r--   0        0        0     4083 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/template/base.py
+-rw-r--r--   0        0        0     1894 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17562 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     5145 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19671 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0    29713 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2540 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    22456 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     8056 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8564 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4171 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8937 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      566 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2962 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1782 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      286 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/empty.py
+-rw-r--r--   0        0        0     2635 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/file_types.py
+-rw-r--r--   0        0        0      918 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1751 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2984 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/protocols.py
+-rw-r--r--   0        0        0     2039 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/serialization.py
+-rw-r--r--   0        0        0    20917 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/typing.py
+-rw-r--r--   0        0        0     2167 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3763 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3553 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     3334 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/path.py
+-rw-r--r--   0        0        0    12498 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/predicates.py
+-rw-r--r--   0        0        0     2789 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/scope.py
+-rw-r--r--   0        0        0      983 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/sequence.py
+-rw-r--r--   0        0        0     5521 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/signature.py
+-rw-r--r--   0        0        0     4374 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/sync.py
+-rw-r--r--   0        0        0     8299 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1921 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/version.py
+-rw-r--r--   0        0        0     1992 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/warnings.py
+-rw-r--r--   0        0        0    14275 2023-07-20 13:51:29.998682 litestar-2.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0    21325 1970-01-01 00:00:00.000000 litestar-2.0.0b3/PKG-INFO
```

### Comparing `litestar-2.0.0b2/LICENSE` & `litestar-2.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/__init__.py` & `litestar-2.0.0b3/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/_asgi/asgi_router.py` & `litestar-2.0.0b3/litestar/_asgi/asgi_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.0.0b3/litestar/_asgi/routing_trie/mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,18 +81,17 @@
         route: The route that is being added.
 
     Returns:
         A RouteTrieNode instance.
     """
     current_node = root_node
 
-    is_mount = hasattr(route, "route_handler") and getattr(route.route_handler, "is_mount", False)  # pyright: ignore
     has_path_parameters = bool(route.path_parameters)
 
-    if is_mount:  # pyright: ignore
+    if (route_handler := getattr(route, "route_handler", None)) and getattr(route_handler, "is_mount", False):
         current_node = add_mount_route(
             current_node=current_node,
             mount_routes=mount_routes,
             root_node=root_node,
             route=cast("ASGIRoute", route),
         )
```

### Comparing `litestar-2.0.0b2/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.0.0b3/litestar/_asgi/routing_trie/traversal.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,15 @@
             if current_node.is_path_type:
                 path_params.append(normalize_path("/".join(path_components[i:])))
                 break
 
             path_params.append(component)
             continue
 
-        if i != len(path_components) - 1 or not current_node.children:
-            raise NotFoundException()
+        raise NotFoundException()
 
     if not current_node.asgi_handlers:
         raise NotFoundException()
 
     return current_node, path_params, path
 
 
@@ -139,15 +138,17 @@
 
         if mount_paths_regex and (match := mount_paths_regex.search(path)):
             mount_path = path[match.start() : match.end()]
             mount_node = mount_routes[mount_path]
             remaining_path = path[match.end() :]
             # since we allow regular handlers under static paths, we must validate that the request does not match
             # any such handler.
-            if not mount_node.children or not any(sub_route in path for sub_route in mount_node.children):  # type: ignore
+            if not mount_node.children or all(
+                sub_route not in path for sub_route in mount_node.children  # type: ignore
+            ):
                 asgi_app, handler = parse_node_handlers(node=mount_node, method=method)
                 remaining_path = remaining_path or "/"
                 if not mount_node.is_static:
                     remaining_path = remaining_path if remaining_path.endswith("/") else f"{remaining_path}/"
                 return asgi_app, handler, remaining_path, {}
 
         node, path_parameters, path = traverse_route_map(
```

### Comparing `litestar-2.0.0b2/litestar/_asgi/routing_trie/types.py` & `litestar-2.0.0b3/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/_asgi/routing_trie/validate.py` & `litestar-2.0.0b3/litestar/_asgi/routing_trie/validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     if node.is_asgi and bool(set(node.asgi_handlers).difference({"asgi"})):
         raise ImproperlyConfiguredException("ASGI handlers must have a unique path not shared by other route handlers.")
 
     if (
         node.is_mount
         and node.children
         and any(
-            v
-            for v in chain.from_iterable(
+            chain.from_iterable(
                 list(child.path_parameters.values())
                 if isinstance(child.path_parameters, dict)
                 else child.path_parameters
                 for child in node.children.values()
             )
         )
     ):
```

### Comparing `litestar-2.0.0b2/litestar/_asgi/utils.py` & `litestar-2.0.0b3/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/_kwargs/cleanup.py` & `litestar-2.0.0b3/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/_kwargs/dependencies.py` & `litestar-2.0.0b3/litestar/_kwargs/dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from inspect import isasyncgen, isgenerator
 from typing import TYPE_CHECKING, Any
 
-from litestar._signature.utils import get_signature_model
+from litestar._signature import get_signature_model
 from litestar.utils.compat import async_next
 
 __all__ = ("Dependency", "create_dependency_batches", "map_dependencies_recursively", "resolve_dependency")
 
 
 if TYPE_CHECKING:
     from litestar._kwargs.cleanup import DependencyCleanupGroup
@@ -57,15 +57,15 @@
             :class:`WebSocket <litestar.connection.WebSocket>`.
         kwargs: Any kwargs to pass to the dependency, the result will be stored here as well.
         cleanup_group: DependencyCleanupGroup to which generators returned by ``dependency`` will be added
     """
     signature_model = get_signature_model(dependency.provide)
     dependency_kwargs = (
         signature_model.parse_values_from_connection_kwargs(connection=connection, **kwargs)
-        if signature_model.fields
+        if signature_model._fields
         else {}
     )
     value = await dependency.provide(**dependency_kwargs)
 
     if isgenerator(value):
         cleanup_group.add(value)
         value = next(value)
```

### Comparing `litestar-2.0.0b2/litestar/_kwargs/extractors.py` & `litestar-2.0.0b3/litestar/_kwargs/extractors.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 from litestar.exceptions import ValidationException
 from litestar.params import BodyKwarg
 from litestar.types import Empty
 
 if TYPE_CHECKING:
     from litestar._kwargs import KwargsModel
     from litestar._kwargs.parameter_definition import ParameterDefinition
-    from litestar._signature.field import SignatureField
     from litestar.connection import ASGIConnection, Request
     from litestar.dto.interface import DTOInterface
+    from litestar.typing import FieldDefinition
+
 
 __all__ = (
     "body_extractor",
     "cookies_extractor",
     "create_connection_value_extractor",
     "create_data_extractor",
     "create_multipart_extractor",
@@ -64,17 +65,17 @@
     """
 
     alias_and_key_tuple = tuple(
         (p.field_alias.lower() if p.param_type == ParamType.HEADER else p.field_alias, p.field_name)
         for p in expected_params
     )
     alias_defaults = {
-        p.field_alias.lower() if p.param_type == ParamType.HEADER else p.field_alias: p.default_value
+        p.field_alias.lower() if p.param_type == ParamType.HEADER else p.field_alias: p.default
         for p in expected_params
-        if not (p.is_required or p.default_value is Ellipsis)
+        if not (p.is_required or p.default is Ellipsis)
     }
 
     def extractor(values: dict[str, Any], connection: ASGIConnection) -> None:
         data = parser(connection, kwargs_model) if parser else getattr(connection, connection_key, {})
 
         try:
             connection_mapping: dict[str, Any] = {
@@ -284,29 +285,29 @@
     Returns:
         The MessagePack value.
     """
     return await connection.msgpack()
 
 
 def create_multipart_extractor(
-    signature_field: SignatureField, is_data_optional: bool, dto_type: type[DTOInterface] | None
+    field_definition: FieldDefinition, is_data_optional: bool, dto_type: type[DTOInterface] | None
 ) -> Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]:
     """Create a multipart form-data extractor.
 
     Args:
-        signature_field: A SignatureField instance.
+        field_definition: A FieldDefinition instance.
         is_data_optional: Boolean dictating whether the field is optional.
         dto_type: The DTO type, if configured for handler.
 
     Returns:
         An extractor function.
     """
     body_kwarg_multipart_form_part_limit: int | None = None
-    if signature_field.kwarg_model and isinstance(signature_field.kwarg_model, BodyKwarg):
-        body_kwarg_multipart_form_part_limit = signature_field.kwarg_model.multipart_form_part_limit
+    if field_definition.kwarg_definition and isinstance(field_definition.kwarg_definition, BodyKwarg):
+        body_kwarg_multipart_form_part_limit = field_definition.kwarg_definition.multipart_form_part_limit
 
     async def extract_multipart(
         connection: Request[Any, Any, Any],
     ) -> Any:
         multipart_form_part_limit = (
             body_kwarg_multipart_form_part_limit
             if body_kwarg_multipart_form_part_limit is not None
@@ -315,21 +316,22 @@
         connection.scope["_form"] = form_values = (  # type: ignore[typeddict-unknown-key]
             connection.scope["_form"]  # type: ignore[typeddict-item]
             if "_form" in connection.scope
             else parse_multipart_form(
                 body=await connection.body(),
                 boundary=connection.content_type[-1].get("boundary", "").encode(),
                 multipart_form_part_limit=multipart_form_part_limit,
+                type_decoders=connection.route_handler.resolve_type_decoders(),
             )
         )
 
-        if signature_field.is_non_string_sequence:
+        if field_definition.is_non_string_sequence:
             return list(form_values.values())
-        if signature_field.is_simple_type and signature_field.field_type is UploadFile and form_values:
-            return [v for v in form_values.values() if isinstance(v, UploadFile)][0]
+        if field_definition.is_simple_type and field_definition.annotation is UploadFile and form_values:
+            return next(v for v in form_values.values() if isinstance(v, UploadFile))
 
         if not form_values and is_data_optional:
             return None
 
         if dto_type:
             ctx = ConnectionContext.from_connection(connection)
             return dto_type(ctx).builtins_to_data_type(form_values)
@@ -381,19 +383,19 @@
         kwargs_model: The KwargsModel instance.
 
     Returns:
         An extractor for the request's body.
     """
 
     if kwargs_model.expected_form_data:
-        media_type, signature_field, dto_type = kwargs_model.expected_form_data
+        media_type, field_definition, dto_type = kwargs_model.expected_form_data
 
         if media_type == RequestEncodingType.MULTI_PART:
             data_extractor = create_multipart_extractor(
-                signature_field=signature_field,
+                field_definition=field_definition,
                 is_data_optional=kwargs_model.is_data_optional,
                 dto_type=dto_type,
             )
         else:
             data_extractor = create_url_encoded_data_extractor(
                 is_data_optional=kwargs_model.is_data_optional, dto_type=dto_type
             )
```

### Comparing `litestar-2.0.0b2/litestar/_kwargs/kwargs_model.py` & `litestar-2.0.0b3/litestar/_kwargs/kwargs_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 )
 from litestar._kwargs.parameter_definition import (
     ParameterDefinition,
     create_parameter_definition,
     merge_parameter_sets,
 )
 from litestar._signature import SignatureModel, get_signature_model
-from litestar._signature.field import SignatureField
 from litestar.constants import RESERVED_KWARGS
 from litestar.enums import ParamType, RequestEncodingType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.params import BodyKwarg, ParameterKwarg
+from litestar.typing import FieldDefinition
 
 __all__ = ("KwargsModel",)
 
 
 if TYPE_CHECKING:
     from litestar.connection import ASGIConnection
     from litestar.di import Provide
@@ -70,16 +70,16 @@
 
     def __init__(
         self,
         *,
         expected_cookie_params: set[ParameterDefinition],
         expected_dto_data: type[DTOInterface] | None,
         expected_dependencies: set[Dependency],
-        expected_form_data: tuple[RequestEncodingType | str, SignatureField, type[DTOInterface] | None] | None,
-        expected_msgpack_data: SignatureField | None,
+        expected_form_data: tuple[RequestEncodingType | str, FieldDefinition, type[DTOInterface] | None] | None,
+        expected_msgpack_data: FieldDefinition | None,
         expected_header_params: set[ParameterDefinition],
         expected_path_params: set[ParameterDefinition],
         expected_query_params: set[ParameterDefinition],
         expected_reserved_kwargs: set[str],
         sequence_query_parameter_names: set[str],
         is_data_optional: bool,
     ) -> None:
@@ -180,74 +180,72 @@
             )
         return extractors
 
     @classmethod
     def _get_param_definitions(
         cls,
         path_parameters: set[str],
-        layered_parameters: dict[str, SignatureField],
+        layered_parameters: dict[str, FieldDefinition],
         dependencies: dict[str, Provide],
-        signature_fields: dict[str, SignatureField],
+        field_definitions: dict[str, FieldDefinition],
     ) -> tuple[set[ParameterDefinition], set[Dependency]]:
         """Get parameter_definitions for the construction of KwargsModel instance.
 
         Args:
             path_parameters: Any expected path parameters.
             layered_parameters: A string keyed dictionary of layered parameters.
             dependencies: A string keyed dictionary mapping dependency providers.
-            signature_fields: The SignatureModel fields.
+            field_definitions: The SignatureModel fields.
 
         Returns:
             A Tuple of sets
         """
         expected_dependencies = {
             cls._create_dependency_graph(key=key, dependencies=dependencies)
             for key in dependencies
-            if key in signature_fields
+            if key in field_definitions
         }
         ignored_keys = {*RESERVED_KWARGS, *(dependency.key for dependency in expected_dependencies)}
 
         param_definitions = {
             *(
                 create_parameter_definition(
-                    signature_field=signature_field,
+                    field_definition=field_definition,
                     field_name=field_name,
                     path_parameters=path_parameters,
                 )
-                for field_name, signature_field in layered_parameters.items()
-                if field_name not in ignored_keys and field_name not in signature_fields
+                for field_name, field_definition in layered_parameters.items()
+                if field_name not in ignored_keys and field_name not in field_definitions
             ),
             *(
                 create_parameter_definition(
-                    signature_field=signature_field,
+                    field_definition=field_definition,
                     field_name=field_name,
                     path_parameters=path_parameters,
                 )
-                for field_name, signature_field in signature_fields.items()
+                for field_name, field_definition in field_definitions.items()
                 if field_name not in ignored_keys and field_name not in layered_parameters
             ),
         }
 
-        for field_name, signature_field in (
-            (k, v) for k, v in signature_fields.items() if k not in ignored_keys and k in layered_parameters
+        for field_name, field_definition in (
+            (k, v) for k, v in field_definitions.items() if k not in ignored_keys and k in layered_parameters
         ):
             layered_parameter = layered_parameters[field_name]
-            field = signature_field if signature_field.is_parameter_field else layered_parameter
-            default_value = (
-                signature_field.default_value if not signature_field.is_empty else layered_parameter.default_value
-            )
+            field = field_definition if field_definition.is_parameter_field else layered_parameter
+            default = field_definition.default if field_definition.has_default else layered_parameter.default
 
             param_definitions.add(
                 create_parameter_definition(
-                    signature_field=SignatureField(
+                    field_definition=FieldDefinition.from_kwarg(
                         name=field.name,
-                        default_value=default_value,
-                        children=field.children,
-                        field_type=field.field_type,
-                        kwarg_model=field.kwarg_model,
+                        default=default,
+                        inner_types=field.inner_types,
+                        annotation=field.annotation,
+                        kwarg_definition=field.kwarg_definition,
                         extra=field.extra,
                     ),
                     field_name=field_name,
                     path_parameters=path_parameters,
                 )
             )
 
@@ -256,15 +254,15 @@
     @classmethod
     def create_for_signature_model(
         cls,
         signature_model: type[SignatureModel],
         parsed_signature: ParsedSignature,
         dependencies: dict[str, Provide],
         path_parameters: set[str],
-        layered_parameters: dict[str, SignatureField],
+        layered_parameters: dict[str, FieldDefinition],
         data_dto: type[DTOInterface] | None,
     ) -> KwargsModel:
         """Pre-determine what parameters are required for a given combination of route + route handler. It is executed
         during the application bootstrap process.
 
         Args:
             signature_model: A :class:`SignatureModel <litestar._signature.SignatureModel>` subclass.
@@ -275,54 +273,54 @@
             data_dto: A :class:`DTOInterface <litestar._dto.DTOInterface>` subclass if one is declared
                 for the route handler, or ``None``.
 
         Returns:
             An instance of KwargsModel
         """
 
-        signature_fields = signature_model.fields
+        field_definitions = signature_model._fields
 
         cls._validate_raw_kwargs(
             path_parameters=path_parameters,
             dependencies=dependencies,
-            signature_fields=signature_fields,
+            field_definitions=field_definitions,
             layered_parameters=layered_parameters,
         )
 
         param_definitions, expected_dependencies = cls._get_param_definitions(
             path_parameters=path_parameters,
             layered_parameters=layered_parameters,
             dependencies=dependencies,
-            signature_fields=signature_fields,
+            field_definitions=field_definitions,
         )
 
-        expected_reserved_kwargs = {field_name for field_name in signature_fields if field_name in RESERVED_KWARGS}
+        expected_reserved_kwargs = {field_name for field_name in field_definitions if field_name in RESERVED_KWARGS}
         expected_path_parameters = {p for p in param_definitions if p.param_type == ParamType.PATH}
         expected_header_parameters = {p for p in param_definitions if p.param_type == ParamType.HEADER}
         expected_cookie_parameters = {p for p in param_definitions if p.param_type == ParamType.COOKIE}
         expected_query_parameters = {p for p in param_definitions if p.param_type == ParamType.QUERY}
         sequence_query_parameter_names = {p.field_alias for p in expected_query_parameters if p.is_sequence}
 
-        expected_form_data: tuple[RequestEncodingType | str, SignatureField, type[DTOInterface] | None] | None = None
-        expected_msgpack_data: SignatureField | None = None
+        expected_form_data: tuple[RequestEncodingType | str, FieldDefinition, type[DTOInterface] | None] | None = None
+        expected_msgpack_data: FieldDefinition | None = None
         expected_dto_data: type[DTOInterface] | None = None
 
-        data_signature_field = signature_fields.get("data")
+        data_field_definition = field_definitions.get("data")
 
         media_type: RequestEncodingType | str | None = None
-        if data_signature_field and isinstance(data_signature_field.kwarg_model, BodyKwarg):
-            media_type = data_signature_field.kwarg_model.media_type
+        if data_field_definition:
+            if isinstance(data_field_definition.kwarg_definition, BodyKwarg):
+                media_type = data_field_definition.kwarg_definition.media_type
 
-        if data_signature_field:
             if media_type in (RequestEncodingType.MULTI_PART, RequestEncodingType.URL_ENCODED):
-                expected_form_data = (media_type, data_signature_field, data_dto)
+                expected_form_data = (media_type, data_field_definition, data_dto)
             elif data_dto:
                 expected_dto_data = data_dto
             elif media_type == RequestEncodingType.MESSAGEPACK:
-                expected_msgpack_data = data_signature_field
+                expected_msgpack_data = data_field_definition
 
         for dependency in expected_dependencies:
             dependency_kwargs_model = cls.create_for_signature_model(
                 signature_model=get_signature_model(dependency.provide),
                 parsed_signature=parsed_signature,
                 dependencies=dependencies,
                 path_parameters=path_parameters,
@@ -357,15 +355,15 @@
             expected_dto_data=expected_dto_data,
             expected_form_data=expected_form_data,
             expected_header_params=expected_header_parameters,
             expected_msgpack_data=expected_msgpack_data,
             expected_path_params=expected_path_parameters,
             expected_query_params=expected_query_parameters,
             expected_reserved_kwargs=expected_reserved_kwargs,
-            is_data_optional=signature_fields["data"].is_optional if "data" in expected_reserved_kwargs else False,
+            is_data_optional=field_definitions["data"].is_optional if "data" in expected_reserved_kwargs else False,
             sequence_query_parameter_names=sequence_query_parameter_names,
         )
 
     def to_kwargs(self, connection: ASGIConnection) -> dict[str, Any]:
         """Return a dictionary of kwargs. Async values, i.e. CoRoutines, are not resolved to ensure this function is
         sync.
 
@@ -403,25 +401,25 @@
 
     @classmethod
     def _create_dependency_graph(cls, key: str, dependencies: dict[str, Provide]) -> Dependency:
         """Create a graph like structure of dependencies, with each dependency including its own dependencies as a
         list.
         """
         provide = dependencies[key]
-        sub_dependency_keys = [k for k in get_signature_model(provide).fields if k in dependencies]
+        sub_dependency_keys = [k for k in get_signature_model(provide)._fields if k in dependencies]
         return Dependency(
             key=key,
             provide=provide,
             dependencies=[cls._create_dependency_graph(key=k, dependencies=dependencies) for k in sub_dependency_keys],
         )
 
     @classmethod
     def _validate_dependency_data(
         cls,
-        expected_form_data: tuple[RequestEncodingType | str, SignatureField, type[DTOInterface] | None] | None,
+        expected_form_data: tuple[RequestEncodingType | str, FieldDefinition, type[DTOInterface] | None] | None,
         dependency_kwargs_model: KwargsModel,
     ) -> None:
         """Validate that the 'data' kwarg is compatible across dependencies."""
         if bool(expected_form_data) != bool(dependency_kwargs_model.expected_form_data):
             raise ImproperlyConfiguredException(
                 "Dependencies have incompatible 'data' kwarg types: one expects JSON and the other expects form-data"
             )
@@ -434,28 +432,28 @@
                 )
 
     @classmethod
     def _validate_raw_kwargs(
         cls,
         path_parameters: set[str],
         dependencies: dict[str, Provide],
-        signature_fields: dict[str, SignatureField],
-        layered_parameters: dict[str, SignatureField],
+        field_definitions: dict[str, FieldDefinition],
+        layered_parameters: dict[str, FieldDefinition],
     ) -> None:
         """Validate that there are no ambiguous kwargs, that is, kwargs declared using the same key in different
         places.
         """
         dependency_keys = set(dependencies.keys())
 
         parameter_names = {
             *(
                 k
-                for k, f in signature_fields.items()
-                if isinstance(f.kwarg_model, ParameterKwarg)
-                and (f.kwarg_model.header or f.kwarg_model.query or f.kwarg_model.cookie)
+                for k, f in field_definitions.items()
+                if isinstance(f.kwarg_definition, ParameterKwarg)
+                and (f.kwarg_definition.header or f.kwarg_definition.query or f.kwarg_definition.cookie)
             ),
             *list(layered_parameters.keys()),
         }
 
         for intersection in (
             path_parameters.intersection(dependency_keys)
             or path_parameters.intersection(parameter_names)
@@ -463,13 +461,16 @@
         ):
             if intersection:
                 raise ImproperlyConfiguredException(
                     f"Kwarg resolution ambiguity detected for the following keys: {', '.join(intersection)}. "
                     f"Make sure to use distinct keys for your dependencies, path parameters and aliased parameters."
                 )
 
-        used_reserved_kwargs = {*parameter_names, *path_parameters, *dependency_keys}.intersection(RESERVED_KWARGS)
-        if used_reserved_kwargs:
+        if used_reserved_kwargs := {
+            *parameter_names,
+            *path_parameters,
+            *dependency_keys,
+        }.intersection(RESERVED_KWARGS):
             raise ImproperlyConfiguredException(
                 f"Reserved kwargs ({', '.join(RESERVED_KWARGS)}) cannot be used for dependencies and parameter arguments. "
                 f"The following kwargs have been used: {', '.join(used_reserved_kwargs)}"
             )
```

### Comparing `litestar-2.0.0b2/litestar/_layers/utils.py` & `litestar-2.0.0b3/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/_multipart.py` & `litestar-2.0.0b3/litestar/_multipart.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 SOFTWARE.
 """
 from __future__ import annotations
 
 import re
 from collections import defaultdict
 from email.utils import decode_rfc2231
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from urllib.parse import unquote
 
 from litestar.datastructures.upload_file import UploadFile
 from litestar.exceptions import SerializationException, ValidationException
 from litestar.serialization import decode_json
 
 __all__ = ("parse_body", "parse_content_header", "parse_multipart_form")
 
 
+if TYPE_CHECKING:
+    from litestar.types import TypeDecodersSequence
+
 _token = r"([\w!#$%&'*+\-.^_`|~]+)"  # noqa: S105
 _quoted = r'"([^"]*)"'
 _param = re.compile(rf";\s*{_token}=(?:{_token}|{_quoted})", re.ASCII)
 _firefox_quote_escape = re.compile(r'\\"(?!; |\s*$)')
 
 
 def parse_content_header(value: str) -> tuple[str, dict[str, str]]:
@@ -86,21 +89,27 @@
             f"number of multipart components exceeds the allowed limit of {multipart_form_part_limit}, "
             f"this potentially indicates a DoS attack"
         )
 
     return form_parts
 
 
-def parse_multipart_form(body: bytes, boundary: bytes, multipart_form_part_limit: int = 1000) -> dict[str, Any]:
+def parse_multipart_form(
+    body: bytes,
+    boundary: bytes,
+    multipart_form_part_limit: int = 1000,
+    type_decoders: TypeDecodersSequence | None = None,
+) -> dict[str, Any]:
     """Parse multipart form data.
 
     Args:
         body: Body of the request.
         boundary: Boundary of the multipart message.
         multipart_form_part_limit: Limit of the number of parts allowed.
+        type_decoders: A sequence of type decoders to use.
 
     Returns:
         A dictionary of parsed results.
     """
 
     fields: defaultdict[str, list[Any]] = defaultdict(list)
 
@@ -119,15 +128,15 @@
 
             if not form_line:
                 break
 
             line_index = line_end_index + 2
             colon_index = form_line.index(":")
             current_idx = colon_index + 2
-            form_header_field = form_line[0:colon_index].lower()
+            form_header_field = form_line[:colon_index].lower()
             form_header_value, form_parameters = parse_content_header(form_line[current_idx:])
 
             if form_header_field == "content-disposition":
                 field_name = form_parameters.get("name")
                 file_name = form_parameters.get("filename")
 
                 if file_name is None and (filename_with_asterisk := form_parameters.get("filename*")):
@@ -144,12 +153,12 @@
             if file_name:
                 form_file = UploadFile(
                     content_type=content_type, filename=file_name, file_data=post_data, headers=dict(headers)
                 )
                 fields[field_name].append(form_file)
             else:
                 try:
-                    fields[field_name].append(decode_json(post_data))
+                    fields[field_name].append(decode_json(post_data, type_decoders=type_decoders))
                 except SerializationException:
                     fields[field_name].append(post_data.decode(content_charset))
 
     return {k: v if len(v) > 1 else v[0] for k, v in fields.items()}
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/parameters.py` & `litestar-2.0.0b3/litestar/_openapi/parameters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
+from dataclasses import replace
 from typing import TYPE_CHECKING
 
 from litestar.constants import RESERVED_KWARGS
 from litestar.enums import ParamType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.openapi.spec.parameter import Parameter
 from litestar.openapi.spec.schema import Schema
 from litestar.params import DependencyKwarg, ParameterKwarg
 from litestar.types import Empty
 
 __all__ = ("create_parameter_for_handler",)
 
+from litestar.typing import FieldDefinition
 
 if TYPE_CHECKING:
     from litestar._openapi.schema_generation import SchemaCreator
-    from litestar._signature.field import SignatureField
     from litestar.di import Provide
     from litestar.handlers.base import BaseRouteHandler
     from litestar.openapi.spec import Reference
     from litestar.types.internal_types import PathParameterDefinition
 
 
 class ParameterCollection:
@@ -63,141 +64,133 @@
 
     def list(self) -> list[Parameter]:
         """Return a list of all ``Parameter``'s in the collection."""
         return list(self._parameters.values())
 
 
 def create_parameter(
-    signature_field: SignatureField,
+    field_definition: FieldDefinition,
     parameter_name: str,
     path_parameters: tuple[PathParameterDefinition, ...],
     schema_creator: SchemaCreator,
 ) -> Parameter:
     """Create an OpenAPI Parameter instance."""
-    from litestar._signature.field import SignatureField
 
     result: Schema | Reference | None = None
-    kwargs_model = signature_field.kwarg_model if isinstance(signature_field.kwarg_model, ParameterKwarg) else None
+    kwarg_definition = (
+        field_definition.kwarg_definition if isinstance(field_definition.kwarg_definition, ParameterKwarg) else None
+    )
 
     if any(path_param.name == parameter_name for path_param in path_parameters):
         param_in = ParamType.PATH
         is_required = True
-        path_parameter = [p for p in path_parameters if parameter_name in p.name][0]
-        result = schema_creator.for_field(
-            SignatureField(
-                children=None,
-                default_value=signature_field.default_value,
-                extra=signature_field.extra,
-                field_type=path_parameter.type,
-                kwarg_model=signature_field.kwarg_model,
-                name=signature_field.name,
-            )
-        )
-    elif kwargs_model and kwargs_model.header:
-        parameter_name = kwargs_model.header
+        path_parameter = next(p for p in path_parameters if parameter_name in p.name)
+        result = schema_creator.for_field_definition(replace(field_definition, annotation=path_parameter.type))
+    elif kwarg_definition and kwarg_definition.header:
+        parameter_name = kwarg_definition.header
         param_in = ParamType.HEADER
-        is_required = signature_field.is_required
-    elif kwargs_model and kwargs_model.cookie:
-        parameter_name = kwargs_model.cookie
+        is_required = field_definition.is_required
+    elif kwarg_definition and kwarg_definition.cookie:
+        parameter_name = kwarg_definition.cookie
         param_in = ParamType.COOKIE
-        is_required = signature_field.is_required
+        is_required = field_definition.is_required
     else:
-        is_required = signature_field.is_required
+        is_required = field_definition.is_required
         param_in = ParamType.QUERY
-        parameter_name = kwargs_model.query if kwargs_model and kwargs_model.query else parameter_name
+        parameter_name = kwarg_definition.query if kwarg_definition and kwarg_definition.query else parameter_name
 
     if not result:
-        result = schema_creator.for_field(signature_field)
+        result = schema_creator.for_field_definition(field_definition)
 
     schema = result if isinstance(result, Schema) else schema_creator.schemas[result.value]
 
     return Parameter(
         description=schema.description,
         name=parameter_name,
         param_in=param_in,
         required=is_required,
         schema=result,
     )
 
 
 def get_recursive_handler_parameters(
     field_name: str,
-    signature_field: SignatureField,
+    field_definition: FieldDefinition,
     dependency_providers: dict[str, Provide],
     route_handler: BaseRouteHandler,
     path_parameters: tuple[PathParameterDefinition, ...],
     schema_creator: SchemaCreator,
 ) -> list[Parameter]:
     """Create and return parameters for a handler.
 
     If the provided field is not a dependency, a normal parameter is created and returned as a list, otherwise
     `create_parameter_for_handler()` is called to generate parameters for the dependency.
     """
 
     if field_name not in dependency_providers:
         return [
             create_parameter(
-                signature_field=signature_field,
+                field_definition=field_definition,
                 parameter_name=field_name,
                 path_parameters=path_parameters,
                 schema_creator=schema_creator,
             )
         ]
 
-    dependency_fields = dependency_providers[field_name].signature_model.fields
+    dependency_fields = dependency_providers[field_name].signature_model._fields
     return create_parameter_for_handler(
         route_handler=route_handler,
         handler_fields=dependency_fields,
         path_parameters=path_parameters,
         schema_creator=schema_creator,
     )
 
 
 def get_layered_parameter(
     field_name: str,
-    signature_field: SignatureField,
-    layered_parameters: dict[str, SignatureField],
+    field_definition: FieldDefinition,
+    layered_parameters: dict[str, FieldDefinition],
     path_parameters: tuple[PathParameterDefinition, ...],
     schema_creator: SchemaCreator,
 ) -> Parameter:
     """Create a layered parameter for a given signature model field.
 
     Layer info is extracted from the provided ``layered_parameters`` dict and set as the field's ``field_info`` attribute.
     """
     layer_field = layered_parameters[field_name]
 
-    field = signature_field if signature_field.is_parameter_field else layer_field
-    default_value = signature_field.default_value if not signature_field.is_empty else layer_field.default_value
-    field_type = signature_field.field_type if signature_field is not Empty else layer_field.field_type  # type: ignore
+    field = field_definition if field_definition.is_parameter_field else layer_field
+    default = layer_field.default if field_definition.has_default else field_definition.default
+    annotation = field_definition.annotation if field_definition is not Empty else layer_field.annotation
 
     parameter_name = field_name
-    if isinstance(field.kwarg_model, ParameterKwarg):
-        parameter_name = field.kwarg_model.query or field.kwarg_model.header or field.kwarg_model.cookie or field_name
-
-    from litestar._signature.field import SignatureField
+    if isinstance(field.kwarg_definition, ParameterKwarg):
+        parameter_name = (
+            field.kwarg_definition.query or field.kwarg_definition.header or field.kwarg_definition.cookie or field_name
+        )
 
-    signature_field = SignatureField.create(
-        children=field.children,
-        default_value=default_value,
+    field_definition = FieldDefinition.from_kwarg(
+        inner_types=field.inner_types,
+        default=default,
         extra=field.extra,
-        field_type=field_type,
-        kwarg_model=field.kwarg_model,
+        annotation=annotation,
+        kwarg_definition=field.kwarg_definition,
         name=field_name,
     )
     return create_parameter(
-        signature_field=signature_field,
+        field_definition=field_definition,
         parameter_name=parameter_name,
         path_parameters=path_parameters,
         schema_creator=schema_creator,
     )
 
 
 def create_parameter_for_handler(
     route_handler: BaseRouteHandler,
-    handler_fields: dict[str, SignatureField],
+    handler_fields: dict[str, FieldDefinition],
     path_parameters: tuple[PathParameterDefinition, ...],
     schema_creator: SchemaCreator,
 ) -> list[Parameter]:
     """Create a list of path/query/header Parameter models for the given PathHandler."""
     parameters = ParameterCollection(route_handler=route_handler)
     dependency_providers = route_handler.resolve_dependencies()
 
@@ -209,44 +202,44 @@
     unique_layered_fields = tuple(
         (k, v) for k, v in layered_parameters.items() if k not in RESERVED_KWARGS and k not in handler_fields
     )
     intersection_fields = tuple(
         (k, v) for k, v in handler_fields.items() if k not in RESERVED_KWARGS and k in layered_parameters
     )
 
-    for field_name, signature_field in unique_handler_fields:
-        if isinstance(signature_field.kwarg_model, DependencyKwarg) and field_name not in dependency_providers:
+    for field_name, field_definition in unique_handler_fields:
+        if isinstance(field_definition.kwarg_definition, DependencyKwarg) and field_name not in dependency_providers:
             # never document explicit dependencies
             continue
 
         for parameter in get_recursive_handler_parameters(
             field_name=field_name,
-            signature_field=signature_field,
+            field_definition=field_definition,
             dependency_providers=dependency_providers,
             route_handler=route_handler,
             path_parameters=path_parameters,
             schema_creator=schema_creator,
         ):
             parameters.add(parameter)
 
-    for field_name, signature_field in unique_layered_fields:
+    for field_name, field_definition in unique_layered_fields:
         parameters.add(
             create_parameter(
-                signature_field=signature_field,
+                field_definition=field_definition,
                 parameter_name=field_name,
                 path_parameters=path_parameters,
                 schema_creator=schema_creator,
             )
         )
 
-    for field_name, signature_field in intersection_fields:
+    for field_name, field_definition in intersection_fields:
         parameters.add(
             get_layered_parameter(
                 field_name=field_name,
-                signature_field=signature_field,
+                field_definition=field_definition,
                 layered_parameters=layered_parameters,
                 path_parameters=path_parameters,
                 schema_creator=schema_creator,
             )
         )
 
     return parameters.list()
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/path_item.py` & `litestar-2.0.0b3/litestar/_openapi/path_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,20 +84,20 @@
     Returns:
         A tuple containing the path item and a list of operation ids.
     """
     path_item = PathItem()
     operation_ids: list[str] = []
 
     request_schema_creator = SchemaCreator(create_examples, plugins, schemas, prefer_alias=True)
-    response_schema_creator = SchemaCreator(create_examples, plugins, schemas, prefer_alias=False)
+    response_schema_creator = SchemaCreator(create_examples, plugins, schemas, prefer_alias=True)
     for http_method, handler_tuple in route.route_handler_map.items():
         route_handler, _ = handler_tuple
 
         if route_handler.include_in_schema:
-            handler_fields = route_handler.signature_model.fields if route_handler.signature_model else {}
+            handler_fields = route_handler.signature_model._fields if route_handler.signature_model else {}
             parameters = (
                 create_parameter_for_handler(
                     route_handler=route_handler,
                     handler_fields=handler_fields,
                     path_parameters=route.path_parameters,
                     schema_creator=request_schema_creator,
                 )
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/request_body.py` & `litestar-2.0.0b3/litestar/_openapi/request_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 from litestar.params import BodyKwarg
 
 __all__ = ("create_request_body",)
 
 
 if TYPE_CHECKING:
     from litestar._openapi.schema_generation import SchemaCreator
-    from litestar._signature.field import SignatureField
     from litestar.handlers import BaseRouteHandler
+    from litestar.typing import FieldDefinition
 
 
 def create_request_body(
-    route_handler: BaseRouteHandler, field: SignatureField, schema_creator: SchemaCreator
+    route_handler: BaseRouteHandler, field: FieldDefinition, schema_creator: SchemaCreator
 ) -> RequestBody | None:
     """Create a RequestBody model for the given RouteHandler or return None."""
     media_type: RequestEncodingType | str = RequestEncodingType.JSON
-    if isinstance(field.kwarg_model, BodyKwarg) and field.kwarg_model.media_type:
-        media_type = field.kwarg_model.media_type
+    if isinstance(field.kwarg_definition, BodyKwarg) and field.kwarg_definition.media_type:
+        media_type = field.kwarg_definition.media_type
 
     if dto := route_handler.resolve_dto():
         schema = dto.create_openapi_schema("data", str(route_handler), schema_creator)
     else:
-        schema = schema_creator.for_field(field)
+        schema = schema_creator.for_field_definition(field)
 
     return RequestBody(required=True, content={media_type: OpenAPIMediaType(schema=schema)})
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/responses.py` & `litestar-2.0.0b3/litestar/_openapi/responses.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from copy import copy
 from dataclasses import asdict
 from http import HTTPStatus
 from inspect import Signature
 from operator import attrgetter
 from typing import TYPE_CHECKING, Any, Iterator
 
-from litestar._signature.field import SignatureField
 from litestar.enums import MediaType
 from litestar.exceptions import HTTPException, ValidationException
 from litestar.openapi.spec import OpenAPIResponse
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.header import OpenAPIHeader
 from litestar.openapi.spec.media_type import OpenAPIMediaType
 from litestar.openapi.spec.schema import Schema
@@ -23,14 +22,15 @@
     Template,
 )
 from litestar.response import (
     Response as LitestarResponse,
 )
 from litestar.response.base import ASGIResponse
 from litestar.types.builtin_types import NoneType
+from litestar.typing import FieldDefinition
 from litestar.utils import get_enum_string_value, get_name
 
 if TYPE_CHECKING:
     from litestar._openapi.schema_generation import SchemaCreator
     from litestar.datastructures.cookie import Cookie
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.openapi.spec.responses import Responses
@@ -94,15 +94,15 @@
         elif return_type.is_subclass_of(LitestarResponse):
             return_annotation = return_type.inner_types[0].annotation if return_type.inner_types else Any
             media_type = media_type or MediaType.JSON
 
         if dto := route_handler.resolve_return_dto():
             result = dto.create_openapi_schema("return", str(route_handler), schema_creator)
         else:
-            result = schema_creator.for_field(SignatureField.create(return_annotation))
+            result = schema_creator.for_field_definition(FieldDefinition.from_annotation(return_annotation))
 
         schema = result if isinstance(result, Schema) else schema_creator.schemas[result.value]
 
         schema.content_encoding = route_handler.content_encoding
         schema.content_media_type = route_handler.content_media_type
 
         response = OpenAPIResponse(
@@ -154,15 +154,17 @@
         response.headers = {}
 
     no_examples_schema_creator = schema_creator.not_generating_examples
     for response_header in route_handler.resolve_response_headers():
         header = OpenAPIHeader()
         for attribute_name, attribute_value in ((k, v) for k, v in asdict(response_header).items() if v is not None):
             if attribute_name == "value":
-                header.schema = no_examples_schema_creator.for_field(SignatureField.create(type(attribute_value)))
+                header.schema = no_examples_schema_creator.for_field_definition(
+                    FieldDefinition.from_annotation(type(attribute_value))
+                )
             elif attribute_name != "documentation_only":
                 setattr(header, attribute_name, attribute_value)
 
         response.headers[response_header.name] = header
 
     if cookies := route_handler.resolve_response_cookies():
         response.headers["Set-Cookie"] = OpenAPIHeader(
@@ -214,15 +216,17 @@
     """Create the schema for additional responses, if any."""
     if not route_handler.responses:
         return
 
     schema_creator = copy(schema_creator)
     for status_code, additional_response in route_handler.responses.items():
         schema_creator.generate_examples = additional_response.generate_examples
-        schema = schema_creator.for_field(SignatureField.create(additional_response.data_container))
+        schema = schema_creator.for_field_definition(
+            FieldDefinition.from_annotation(additional_response.data_container)
+        )
         yield str(status_code), OpenAPIResponse(
             description=additional_response.description,
             content={additional_response.media_type: OpenAPIMediaType(schema=schema)},
         )
 
 
 def create_responses(
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.0.0b3/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,58 +6,57 @@
 
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.schema import Schema
 
 if TYPE_CHECKING:
     from _decimal import Decimal
 
-    from litestar.params import BodyKwarg, ParameterKwarg
-
+    from litestar.params import KwargDefinition
 
 __all__ = (
     "create_date_constrained_field_schema",
     "create_numerical_constrained_field_schema",
     "create_string_constrained_field_schema",
 )
 
 
 def create_numerical_constrained_field_schema(
     field_type: type[int] | type[float] | type[Decimal],
-    kwargs_model: ParameterKwarg | BodyKwarg,
+    kwarg_definition: KwargDefinition,
 ) -> Schema:
     """Create Schema from Constrained Int/Float/Decimal field."""
     schema = Schema(type=OpenAPIType.INTEGER if issubclass(field_type, int) else OpenAPIType.NUMBER)
-    if kwargs_model.le is not None:
-        schema.maximum = float(kwargs_model.le)
-    if kwargs_model.lt is not None:
-        schema.exclusive_maximum = float(kwargs_model.lt)
-    if kwargs_model.ge is not None:
-        schema.minimum = float(kwargs_model.ge)
-    if kwargs_model.gt is not None:
-        schema.exclusive_minimum = float(kwargs_model.gt)
-    if kwargs_model.multiple_of is not None:
-        schema.multiple_of = float(kwargs_model.multiple_of)
+    if kwarg_definition.le is not None:
+        schema.maximum = float(kwarg_definition.le)
+    if kwarg_definition.lt is not None:
+        schema.exclusive_maximum = float(kwarg_definition.lt)
+    if kwarg_definition.ge is not None:
+        schema.minimum = float(kwarg_definition.ge)
+    if kwarg_definition.gt is not None:
+        schema.exclusive_minimum = float(kwarg_definition.gt)
+    if kwarg_definition.multiple_of is not None:
+        schema.multiple_of = float(kwarg_definition.multiple_of)
     return schema
 
 
 def create_date_constrained_field_schema(
     field_type: type[date] | type[datetime],
-    kwargs_model: ParameterKwarg | BodyKwarg,
+    kwarg_definition: KwargDefinition,
 ) -> Schema:
     """Create Schema from Constrained Date Field."""
     schema = Schema(
         type=OpenAPIType.STRING, format=OpenAPIFormat.DATE if issubclass(field_type, date) else OpenAPIFormat.DATE_TIME
     )
-    for kwargs_model_attr, schema_attr in [
+    for kwarg_definition_attr, schema_attr in [
         ("le", "maximum"),
         ("lt", "exclusive_maximum"),
         ("ge", "minimum"),
         ("gt", "exclusive_minimum"),
     ]:
-        if attr := getattr(kwargs_model, kwargs_model_attr):
+        if attr := getattr(kwarg_definition, kwarg_definition_attr):
             setattr(
                 schema,
                 schema_attr,
                 datetime.combine(
                     datetime.fromtimestamp(attr, tz=timezone.utc) if isinstance(attr, (float, int)) else attr,
                     datetime.min.time(),
                     tzinfo=timezone.utc,
@@ -65,26 +64,26 @@
             )
 
     return schema
 
 
 def create_string_constrained_field_schema(
     field_type: type[str] | type[bytes],
-    kwargs_model: ParameterKwarg | BodyKwarg,
+    kwarg_definition: KwargDefinition,
 ) -> Schema:
     """Create Schema from Constrained Str/Bytes field."""
     schema = Schema(type=OpenAPIType.STRING)
     if issubclass(field_type, bytes):
         schema.content_encoding = "utf-8"
-    if kwargs_model.min_length:
-        schema.min_length = kwargs_model.min_length
-    if kwargs_model.max_length:
-        schema.max_length = kwargs_model.max_length
-    if kwargs_model.pattern:
+    if kwarg_definition.min_length:
+        schema.min_length = kwarg_definition.min_length
+    if kwarg_definition.max_length:
+        schema.max_length = kwarg_definition.max_length
+    if kwarg_definition.pattern:
         schema.pattern = (
-            kwargs_model.pattern.pattern if isinstance(kwargs_model.pattern, Pattern) else kwargs_model.pattern  # type: ignore[attr-defined,unreachable]
+            kwarg_definition.pattern.pattern if isinstance(kwarg_definition.pattern, Pattern) else kwarg_definition.pattern  # type: ignore[attr-defined,unreachable]
         )
-    if kwargs_model.lower_case:
+    if kwarg_definition.lower_case:
         schema.description = "must be in lower case"
-    if kwargs_model.upper_case:
+    if kwarg_definition.upper_case:
         schema.description = "must be in upper case"
     return schema
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/schema_generation/examples.py` & `litestar-2.0.0b3/litestar/_openapi/schema_generation/examples.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,55 +16,56 @@
 try:
     from polyfactory.factories.pydantic_factory import ModelFactory as Factory
 except ImportError:
     from polyfactory.factories import DataclassFactory as Factory  # type: ignore[assignment]
 
 
 if TYPE_CHECKING:
-    from litestar._signature.field import SignatureField
+    from litestar.typing import FieldDefinition
 
 
 Factory.seed_random(10)
 
 
 def _normalize_example_value(value: Any) -> Any:
     """Normalize the example value to make it look a bit prettier."""
     value = unwrap_annotation(annotation=value, random=Factory.__random__)
     if isinstance(value, (Decimal, float)):
         value = round(float(value), 2)
     if isinstance(value, Enum):
         value = value.value
     if is_pydantic_model_instance(value):
-        value = value.dict()
+        from litestar.contrib.pydantic import _model_dump
+
+        value = _model_dump(value)
     if isinstance(value, (list, set)):
         value = [_normalize_example_value(v) for v in value]
     if isinstance(value, dict):
         for k, v in value.items():
             value[k] = _normalize_example_value(v)
     return value
 
 
-def _create_field_meta(field: SignatureField) -> FieldMeta:
+def _create_field_meta(field: FieldDefinition) -> FieldMeta:
     return FieldMeta.from_type(
-        annotation=field.field_type,
-        constraints={"constant": field.is_const},
-        default=field.default_value if field.default_value is not Empty else Null,
+        annotation=field.annotation,
+        default=field.default if field.default is not Empty else Null,
         name=field.name,
         random=Factory.__random__,
     )
 
 
-def create_examples_for_field(field: SignatureField) -> list[Example]:
+def create_examples_for_field(field: FieldDefinition) -> list[Example]:
     """Create an OpenAPI Example instance.
 
     Args:
         field: A signature field.
 
     Returns:
         A list including a single example.
     """
     try:
-        field_meta = _create_field_meta(replace(field, field_type=_normalize_example_value(field.field_type)))
+        field_meta = _create_field_meta(replace(field, annotation=_normalize_example_value(field.annotation)))
         value = Factory.get_field_value(field_meta)
         return [Example(description=f"Example {field.name} value", value=value)]
     except ParameterException:
         return []
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/schema_generation/utils.py` & `litestar-2.0.0b3/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.0.0b3/litestar/_openapi/typescript_converter/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,16 @@
     """
     cookie_params: list[TypeScriptProperty] = []
     header_params: list[TypeScriptProperty] = []
     path_params: list[TypeScriptProperty] = []
     query_params: list[TypeScriptProperty] = []
 
     for param in params:
-        if param.schema and (schema := get_openapi_type(param.schema, components)):
+        if param.schema:
+            schema = get_openapi_type(param.schema, components)
             ts_prop = TypeScriptProperty(
                 key=normalize_typescript_namespace(param.name, allow_quoted=True),
                 required=param.required,
                 value=parse_schema(schema),
             )
             if param.param_in == ParamType.COOKIE:
                 cookie_params.append(ts_prop)
@@ -193,20 +194,19 @@
     Returns:
         A TypeScript type.
     """
     undefined = TypeScriptPrimitive("undefined")
     if not body.content:
         return TypeScriptType("RequestBody", undefined)
 
-    if (content := [get_openapi_type(v.schema, components) for v in body.content.values() if v.schema]) and (
-        schema := content[0]
-    ):
+    if content := [get_openapi_type(v.schema, components) for v in body.content.values() if v.schema]:
+        schema = content[0]
         return TypeScriptType(
             "RequestBody",
-            parse_schema(schema) if body.required else TypeScriptUnion((parse_schema(content[0]), undefined)),
+            parse_schema(schema) if body.required else TypeScriptUnion((parse_schema(schema), undefined)),
         )
 
     return TypeScriptType("RequestBody", undefined)
 
 
 def parse_responses(responses: Responses, components: Components) -> tuple[TypeScriptNamespace, ...]:
     """Parse a given Operation's Responses object.
@@ -218,18 +218,16 @@
     Returns:
         A tuple of namespaces, mapping response codes to data.
     """
     result: list[TypeScriptNamespace] = []
     for http_status, response in [
         (status, get_openapi_type(res, components=components)) for status, res in responses.items()
     ]:
-        if (
-            response
-            and response.content
-            and (content := [get_openapi_type(v.schema, components) for v in response.content.values() if v.schema])
+        if response.content and (
+            content := [get_openapi_type(v.schema, components) for v in response.content.values() if v.schema]
         ):
             ts_type = parse_schema(content[0])
         else:
             ts_type = TypeScriptPrimitive("undefined")
 
         containers = [
             TypeScriptType("ResponseBody", ts_type),
@@ -269,26 +267,25 @@
     if not openapi_schema.components:  # pragma: no cover
         raise ValueError("OpenAPI schema has no components")
 
     operations: list[TypeScriptNamespace] = []
 
     for path_item in openapi_schema.paths.values():
         shared_params = [
-            get_openapi_type(p, components=openapi_schema.components) for p in (path_item.parameters or []) if p
+            get_openapi_type(p, components=openapi_schema.components) for p in (path_item.parameters or [])
         ]
         for method in HttpMethod:
             if (
                 operation := cast("Operation | None", getattr(path_item, method.lower(), "None"))
             ) and operation.operation_id:
                 params = parse_params(
                     [
                         *(
                             get_openapi_type(p, components=openapi_schema.components)
                             for p in (operation.parameters or [])
-                            if p
                         ),
                         *shared_params,
                     ],
                     components=openapi_schema.components,
                 )
                 request_body = (
                     parse_request_body(
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.0.0b3/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,18 @@
     Args:
         value: A string to normalize.
         allow_quoted: Whether to allow quoting the value.
 
     Returns:
         A normalized value
     """
-    if not allow_quoted and not (value[0].isalpha() or value[0] in {"_", "$"}):
+    if not allow_quoted and not value[0].isalpha() and value[0] not in {"_", "$"}:
         raise ValueError(f"invalid typescript namespace {value}")
     if allow_quoted:
-        if allowed_key_re.fullmatch(value):
-            return value
-        return f'"{value}"'
+        return value if allowed_key_re.fullmatch(value) else f'"{value}"'
     return invalid_namespace_re.sub("", value)
 
 
 def is_schema_value(value: Any) -> TypeGuard[Schema]:
     """Typeguard for a schema value.
 
     Args:
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/typescript_converter/types.py` & `litestar-2.0.0b3/litestar/_openapi/typescript_converter/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,20 @@
     "TypeScriptType",
     "TypeScriptUnion",
 )
 
 
 def _as_string(value: Any) -> str:
     if isinstance(value, str):
-        return '"' + value + '"'
+        return f'"{value}"'
 
     if isinstance(value, bool):
         return "true" if value else "false"
 
-    if value is None:
-        return "null"
-
-    return str(value)
+    return "null" if value is None else str(value)
 
 
 class TypeScriptElement(ABC):
     """A class representing a TypeScript type element."""
 
     @abstractmethod
     def write(self) -> str:
```

### Comparing `litestar-2.0.0b2/litestar/_openapi/utils.py` & `litestar-2.0.0b3/litestar/_openapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,12 +35,12 @@
     handler_namespace = (
         http_method.title() + route_handler.handler_name.title()
         if len(route_handler.http_methods) > 1
         else route_handler.handler_name.title()
     )
 
     components_namespace = ""
-    for component in (c if not isinstance(c, PathParameterDefinition) else c.name for c in path_components):
+    for component in (c.name if isinstance(c, PathParameterDefinition) else c for c in path_components):
         if component.title() not in components_namespace:
             components_namespace += component.title()
 
     return SEPARATORS_CLEANUP_PATTERN.sub("", components_namespace + handler_namespace)
```

### Comparing `litestar-2.0.0b2/litestar/_parsers.py` & `litestar-2.0.0b3/litestar/_parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Args:
         encoded_data: The encoded byte string.
 
     Returns:
         A parsed dict.
     """
-    return parse_url_encoded_dict(encoded_data)
+    return parse_url_encoded_dict(qs=encoded_data, parse_numbers=False)
 
 
 @lru_cache(1024)
 def parse_query_string(query_string: bytes) -> tuple[tuple[str, Any], ...]:
     """Parse a query string into a tuple of key value pairs.
 
     Args:
@@ -43,18 +43,22 @@
 
     Args:
         cookie_string: A cookie string.
 
     Returns:
         A string keyed dictionary of values
     """
-    output: dict[str, str] = {}
     cookies = [cookie.split("=", 1) if "=" in cookie else ("", cookie) for cookie in cookie_string.split(";")]
-    for k, v in filter(lambda x: x[0] or x[1], ((k.strip(), v.strip()) for k, v in cookies)):
-        output[k] = unquote(unquote_cookie(v))
+    output: dict[str, str] = {
+        k: unquote(unquote_cookie(v))
+        for k, v in filter(
+            lambda x: x[0] or x[1],
+            ((k.strip(), v.strip()) for k, v in cookies),
+        )
+    }
     return output
 
 
 @lru_cache(1024)
 def _parse_headers(headers: tuple[tuple[bytes, bytes], ...]) -> dict[str, str]:
     """Parse ASGI headers into a dict of string keys and values.
```

### Comparing `litestar-2.0.0b2/litestar/app.py` & `litestar-2.0.0b3/litestar/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from __future__ import annotations
 
 import inspect
 import logging
 import os
-from contextlib import AbstractAsyncContextManager, AsyncExitStack, asynccontextmanager
+from contextlib import AbstractAsyncContextManager, AsyncExitStack, asynccontextmanager, suppress
 from datetime import date, datetime, time, timedelta
 from functools import partial
 from itertools import chain
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Literal, Mapping, Sequence, TypedDict, cast
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Mapping, Sequence, TypedDict, cast
 
 from litestar._asgi import ASGIRouter
 from litestar._asgi.utils import get_route_handlers, wrap_in_exception_handler
 from litestar._openapi.path_item import create_path_item
 from litestar.config.allowed_hosts import AllowedHostsConfig
 from litestar.config.app import AppConfig
 from litestar.config.response_cache import ResponseCacheConfig
 from litestar.connection import Request, WebSocket
 from litestar.constants import OPENAPI_NOT_INITIALIZED
 from litestar.datastructures.state import State
 from litestar.events.emitter import BaseEventEmitterBackend, SimpleEventEmitter
 from litestar.exceptions import (
     ImproperlyConfiguredException,
+    MissingDependencyException,
     NoRouteMatchFoundException,
 )
 from litestar.logging.config import LoggingConfig, get_logger_placeholder
 from litestar.middleware.cors import CORSMiddleware
 from litestar.openapi.config import OpenAPIConfig
 from litestar.openapi.spec.components import Components
 from litestar.plugins import (
@@ -33,17 +34,17 @@
     OpenAPISchemaPluginProtocol,
     SerializationPluginProtocol,
 )
 from litestar.router import Router
 from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
 from litestar.static_files.base import StaticFiles
 from litestar.stores.registry import StoreRegistry
-from litestar.types import Empty
+from litestar.types import Empty, TypeDecodersSequence
 from litestar.types.internal_types import PathParameterDefinition
-from litestar.utils import AsyncCallable, join_paths, unique, warn_deprecation
+from litestar.utils import AsyncCallable, join_paths, unique
 from litestar.utils.dataclass import extract_dataclass_items
 from litestar.utils.predicates import is_async_callable
 from litestar.utils.warnings import warn_pdb_on_exception
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
@@ -125,15 +126,14 @@
     and Route Handlers should be registered on it.
     """
 
     __slots__ = (
         "_lifespan_managers",
         "_debug",
         "_openapi_schema",
-        "_preferred_validation_backend",
         "after_exception",
         "allowed_hosts",
         "asgi_handler",
         "asgi_router",
         "before_send",
         "compression_config",
         "cors_config",
@@ -202,18 +202,18 @@
         signature_namespace: Mapping[str, Any] | None = None,
         state: State | None = None,
         static_files_config: OptionalSequence[StaticFilesConfig] | None = None,
         stores: StoreRegistry | dict[str, Store] | None = None,
         tags: Sequence[str] | None = None,
         template_config: TemplateConfig | None = None,
         type_encoders: TypeEncodersMap | None = None,
+        type_decoders: TypeDecodersSequence | None = None,
         websocket_class: type[WebSocket] | None = None,
         lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
         pdb_on_exception: bool | None = None,
-        _preferred_validation_backend: Literal["attrs", "pydantic"] | None = None,
     ) -> None:
         """Initialize a ``Litestar`` application.
 
         Args:
             after_exception: A sequence of :class:`exception hook handlers <.types.AfterExceptionHookHandler>`. This
                 hook is called after an exception occurs. In difference to exception handlers, it is not meant to
                 return a response - only to process the exception (e.g. log it, send it to Sentry etc.).
@@ -289,33 +289,27 @@
                 application. If this is a dictionary to it will be passed to a
                 :class:`StoreRegistry <.stores.registry.StoreRegistry>`. If it is a
                 :class:`StoreRegistry <.stores.registry.StoreRegistry>`, this instance will be used directly.
             tags: A sequence of string tags that will be appended to the schema of all route handlers under the
                 application.
             template_config: An instance of :class:`TemplateConfig <.template.TemplateConfig>`
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
+            type_decoders: A sequence of tuples, each composed of a predicate testing for type identity and a msgspec hook for deserialization.
             websocket_class: An optional subclass of :class:`WebSocket <.connection.WebSocket>` to use for websocket
                 connections.
         """
         if logging_config is Empty:
             logging_config = LoggingConfig()
 
         if debug is None:
             debug = os.getenv("LITESTAR_DEBUG", "0") == "1"
 
         if pdb_on_exception is None:
             pdb_on_exception = os.getenv("LITESTAR_PDB", "0") == "1"
 
-        if _preferred_validation_backend is not None:
-            warn_deprecation(
-                version="2.0.0beta1",
-                kind="parameter",
-                deprecated_name="_preferred_validation_backend",
-            )
-
         config = AppConfig(
             after_exception=list(after_exception or []),
             after_request=after_request,
             after_response=after_response,
             allowed_hosts=allowed_hosts if isinstance(allowed_hosts, AllowedHostsConfig) else list(allowed_hosts or []),
             before_request=before_request,
             before_send=list(before_send or []),
@@ -337,15 +331,20 @@
             multipart_form_part_limit=multipart_form_part_limit,
             on_shutdown=list(on_shutdown or []),
             on_startup=list(on_startup or []),
             openapi_config=openapi_config,
             opt=dict(opt or {}),
             parameters=parameters or {},
             pdb_on_exception=pdb_on_exception,
-            plugins=list(plugins or []),
+            plugins=list(
+                chain(
+                    plugins or [],
+                    self.default_plugins,
+                )
+            ),
             request_class=request_class,
             response_cache_config=response_cache_config or ResponseCacheConfig(),
             response_class=response_class,
             response_cookies=response_cookies or [],
             response_headers=response_headers or [],
             return_dto=return_dto,
             route_handlers=list(route_handlers) if route_handlers is not None else [],
@@ -353,14 +352,15 @@
             signature_namespace=dict(signature_namespace or {}),
             state=state or State(),
             static_files_config=list(static_files_config or []),
             stores=stores,
             tags=list(tags or []),
             template_config=template_config,
             type_encoders=type_encoders,
+            type_decoders=type_decoders,
             websocket_class=websocket_class,
         )
         for handler in chain(
             on_app_init or [],
             (p.on_app_init for p in config.plugins if isinstance(p, InitPluginProtocol)),
         ):
             config = handler(config)  # pyright: ignore
@@ -384,15 +384,14 @@
         self.event_emitter = config.event_emitter_backend(listeners=config.listeners)
         self.logging_config = config.logging_config
         self.multipart_form_part_limit = config.multipart_form_part_limit
         self.on_shutdown = config.on_shutdown
         self.on_startup = config.on_startup
         self.openapi_config = config.openapi_config
         self.openapi_schema_plugins = [p for p in config.plugins if isinstance(p, OpenAPISchemaPluginProtocol)]
-        self._preferred_validation_backend: Literal["attrs", "pydantic"] = _preferred_validation_backend or "pydantic"
         self.request_class = config.request_class or Request
         self.response_cache_config = config.response_cache_config
         self.serialization_plugins = [p for p in config.plugins if isinstance(p, SerializationPluginProtocol)]
         self.state = config.state
         self.static_files_config = config.static_files_config
         self.template_engine = config.template_config.engine_instance if config.template_config else None
         self.websocket_class = config.websocket_class or WebSocket
@@ -422,14 +421,15 @@
             return_dto=config.return_dto,
             # route handlers are registered below
             route_handlers=[],
             security=config.security,
             signature_namespace=config.signature_namespace,
             tags=config.tags,
             type_encoders=config.type_encoders,
+            type_decoders=config.type_decoders,
         )
 
         for route_handler in config.route_handlers:
             self.register(route_handler)
 
         if self.logging_config:
             self.get_logger = self.logging_config.configure()
@@ -444,14 +444,28 @@
         self.asgi_handler = self._create_asgi_handler()
 
         self.stores: StoreRegistry = (
             config.stores if isinstance(config.stores, StoreRegistry) else StoreRegistry(config.stores)
         )
 
     @property
+    def default_plugins(self) -> list[PluginProtocol]:
+        default_plugins: list[PluginProtocol] = []
+        with suppress(MissingDependencyException):
+            from litestar.contrib.pydantic import PydanticInitPlugin, PydanticSchemaPlugin
+
+            default_plugins.extend((PydanticInitPlugin(), PydanticSchemaPlugin()))
+
+        with suppress(MissingDependencyException):
+            from litestar.contrib.attrs import AttrsSchemaPlugin
+
+            default_plugins.append(AttrsSchemaPlugin())
+        return default_plugins
+
+    @property
     def debug(self) -> bool:
         return self._debug
 
     @debug.setter
     def debug(self, value: bool) -> None:
         if self.logger:
             self.logger.setLevel(logging.DEBUG if value else logging.INFO)
@@ -646,34 +660,35 @@
             A fully formatted url path.
         """
         handler_index = self.get_handler_index_by_name(name)
         if handler_index is None:
             raise NoRouteMatchFoundException(f"Route {name} can not be found")
 
         allow_str_instead = {datetime, date, time, timedelta, float, Path}
-        output: list[str] = []
-
         routes = sorted(
             self.asgi_router.route_mapping[handler_index["identifier"]],
             key=lambda r: len(r.path_parameters),
             reverse=True,
         )
         passed_parameters = set(path_parameters.keys())
 
-        selected_route = routes[-1]
-        for route in routes:
-            if passed_parameters.issuperset({param.name for param in route.path_parameters}):
-                selected_route = route
-                break
-
+        selected_route = next(
+            (
+                route
+                for route in routes
+                if passed_parameters.issuperset({param.name for param in route.path_parameters})
+            ),
+            routes[-1],
+        )
+        output: list[str] = []
         for component in selected_route.path_components:
             if isinstance(component, PathParameterDefinition):
                 val = path_parameters.get(component.name)
-                if not (
-                    isinstance(val, component.type) or (component.type in allow_str_instead and isinstance(val, str))
+                if not isinstance(val, component.type) and (
+                    component.type not in allow_str_instead or not isinstance(val, str)
                 ):
                     raise NoRouteMatchFoundException(
                         f"Received type for path parameter {component.name} doesn't match declared type {component.type}"
                     )
                 output.append(str(val))
             else:
                 output.append(component)
@@ -721,18 +736,17 @@
     @property
     def route_handler_method_view(self) -> dict[str, list[str]]:
         """Map route handlers to paths.
 
         Returns:
             A dictionary of router handlers and lists of paths as strings
         """
-        route_map: dict[str, list[str]] = {}
-        for handler, routes in self.asgi_router.route_mapping.items():
-            route_map[handler] = [route.path for route in routes]
-
+        route_map: dict[str, list[str]] = {
+            handler: [route.path for route in routes] for handler, routes in self.asgi_router.route_mapping.items()
+        }
         return route_map
 
     def _create_asgi_handler(self) -> ASGIApp:
         """Create an ASGIApp that wraps the ASGI router inside an exception handler.
 
         If CORS or TrustedHost configs are provided to the constructor, they will wrap the router as well.
         """
```

### Comparing `litestar-2.0.0b2/litestar/background_tasks.py` & `litestar-2.0.0b3/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/channels/backends/base.py` & `litestar-2.0.0b3/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/channels/backends/memory.py` & `litestar-2.0.0b3/litestar/channels/backends/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     async def subscribe(self, channels: Iterable[str]) -> None:
         """Subscribe to ``channels``, and enable publishing to them"""
         self._channels.update(channels)
 
     async def unsubscribe(self, channels: Iterable[str]) -> None:
         """Unsubscribe from ``channels``"""
-        self._channels = self._channels - (set(channels))
+        self._channels -= set(channels)
         try:
             for channel in channels:
                 del self._history[channel]
         except KeyError:
             pass
 
     async def stream_events(self) -> AsyncGenerator[tuple[str, Any], None]:
```

### Comparing `litestar-2.0.0b2/litestar/channels/backends/redis.py` & `litestar-2.0.0b3/litestar/channels/backends/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
     async def subscribe(self, channels: Iterable[str]) -> None:
         """Subscribe to ``channels``"""
         self._subscribed_channels.update(channels)
 
     async def unsubscribe(self, channels: Iterable[str]) -> None:
         """Unsubscribe from ``channels``"""
-        self._subscribed_channels = self._subscribed_channels - set(channels)
+        self._subscribed_channels -= set(channels)
 
     async def publish(self, data: bytes, channels: Iterable[str]) -> None:
         """Publish ``data`` to ``channels``.
 
         .. note::
             This operation is performed atomically, using a Lua script
         """
```

### Comparing `litestar-2.0.0b2/litestar/channels/plugin.py` & `litestar-2.0.0b3/litestar/channels/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,18 +98,15 @@
         self._channels: dict[str, set[Subscriber]] = {channel: set() for channel in channels or []}
 
     def encode_data(self, data: LitestarEncodableType) -> bytes:
         """Encode data before storing it in the backend"""
         if isinstance(data, bytes):
             return data
 
-        if isinstance(data, str):
-            return data.encode()
-
-        return self._encode_json(data)
+        return data.encode() if isinstance(data, str) else self._encode_json(data)
 
     def on_app_init(self, app_config: AppConfig) -> AppConfig:
         """Plugin hook. Set up a ``channels`` dependency, add route handlers and register application hooks"""
         app_config.dependencies["channels"] = Provide(lambda: self, use_cache=True, sync_to_thread=False)
         app_config.lifespan.append(self)
         app_config.signature_namespace.update(ChannelsPlugin=ChannelsPlugin)
 
@@ -228,15 +225,15 @@
                 channel_subscribers.remove(subscriber)
             except KeyError:  # subscriber was not subscribed to this channel. This may happen if channels is None
                 continue
 
             if not channel_subscribers:
                 channels_to_unsubscribe.add(channel)
 
-        if not any(subscriber in queues for queues in self._channels.values()):
+        if all(subscriber not in queues for queues in self._channels.values()):
             await subscriber.put(None)  # this will stop any running task or generator by breaking the inner loop
             if subscriber.is_running:
                 await subscriber.stop()
 
         if channels_to_unsubscribe:
             await self._backend.unsubscribe(channels_to_unsubscribe)
```

### Comparing `litestar-2.0.0b2/litestar/channels/subscriber.py` & `litestar-2.0.0b3/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/cli/_utils.py` & `litestar-2.0.0b3/litestar/cli/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import contextlib
 import importlib
 import inspect
 import sys
 from dataclasses import dataclass
 from functools import wraps
 from itertools import chain
 from os import getenv
@@ -96,21 +97,18 @@
         If ``python-dotenv`` is installed, use it to populate environment first
         """
         cwd = Path().cwd()
         cwd_str_path = str(cwd)
         if cwd_str_path not in sys.path:
             sys.path.append(cwd_str_path)
 
-        try:
+        with contextlib.suppress(ImportError):
             import dotenv
 
             dotenv.load_dotenv()
-        except ImportError:
-            pass
-
         app_path = app_path or getenv("LITESTAR_APP")
         if app_path:
             console.print(f"Using Litestar app from env: [bright_blue]{app_path!r}")
             loaded_app = _load_app_from_path(app_path)
         else:
             loaded_app = _autodiscover_app(cwd)
 
@@ -226,15 +224,15 @@
                 kwargs["env"] = env
 
         if "ctx" in params:
             kwargs["ctx"] = ctx
 
         return func(*args, **kwargs)
 
-    return pass_context(wrapped)
+    return pass_context(wrapped)  # pyright: ignore
 
 
 def _wrap_commands(commands: Iterable[Command]) -> None:
     for command in commands:
         if isinstance(command, Group):
             _wrap_commands(command.commands.values())
         elif command.callback:
@@ -318,17 +316,15 @@
                 return LoadedApp(app=value(), app_path=f"{app_string}", is_factory=True)
 
     raise LitestarCLIException("Could not find a Litestar app or factory")
 
 
 def _format_is_enabled(value: Any) -> str:
     """Return a coloured string `"Enabled" if ``value`` is truthy, else "Disabled"."""
-    if value:
-        return "[green]Enabled[/]"
-    return "[red]Disabled[/]"
+    return "[green]Enabled[/]" if value else "[red]Disabled[/]"
 
 
 def show_app_info(app: Litestar) -> None:  # pragma: no cover
     """Display basic information about the application and its configuration."""
 
     table = Table(show_header=False)
     table.add_column("title", style="cyan")
@@ -352,20 +348,19 @@
     table.add_row("Compression", app.compression_config.backend if app.compression_config else "[red]Disabled")
 
     if app.template_engine:
         table.add_row("Template engine", type(app.template_engine).__name__)
 
     if app.static_files_config:
         static_files_configs = app.static_files_config
-        static_files_info = []
-        for static_files in static_files_configs:
-            static_files_info.append(
-                f"path=[yellow]{static_files.path}[/] dirs=[yellow]{', '.join(map(str, static_files.directories))}[/] "
-                f"html_mode={_format_is_enabled(static_files.html_mode)}",
-            )
+        static_files_info = [
+            f"path=[yellow]{static_files.path}[/] dirs=[yellow]{', '.join(map(str, static_files.directories))}[/] "
+            f"html_mode={_format_is_enabled(static_files.html_mode)}"
+            for static_files in static_files_configs
+        ]
         table.add_row("Static files", "\n".join(static_files_info))
 
     middlewares = []
     for middleware in app.middleware:
         updated_middleware = middleware.middleware if isinstance(middleware, DefineMiddleware) else middleware
         middlewares.append(get_name(updated_middleware))
     if middlewares:
```

### Comparing `litestar-2.0.0b2/litestar/cli/commands/core.py` & `litestar-2.0.0b3/litestar/cli/commands/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,28 @@
 if TYPE_CHECKING or not RICH_CLICK_INSTALLED:
     import click
     from click import Context, command, option
 else:
     import rich_click as click
     from rich_click import Context, command, option
 
-
 __all__ = ("info_command", "routes_command", "run_command")
 
 if TYPE_CHECKING:
     from litestar import Litestar
 
 
 def _convert_uvicorn_args(args: dict[str, Any]) -> list[str]:
     process_args = []
     for arg, value in args.items():
         if isinstance(value, bool):
             if value:
                 process_args.append(f"--{arg}")
         elif isinstance(value, tuple):
-            for item in value:
-                process_args.append(f"--{arg}={item}")
+            process_args.extend(f"--{arg}={item}" for item in value)
         else:
             process_args.append(f"--{arg}={value}")
 
     return process_args
 
 
 @command(name="version")
@@ -57,74 +55,76 @@
     """Show information about the detected Litestar app."""
 
     show_app_info(app)
 
 
 @command(name="run")
 @option("-r", "--reload", help="Reload server on changes", default=False, is_flag=True)
+@option("-R", "--reload-dir", help="Directories to watch for file changes", multiple=True)
 @option("-p", "--port", help="Serve under this port", type=int, default=8000, show_default=True)
 @option(
-    "-wc",
+    "-W",
+    "--wc",
     "--web-concurrency",
     help="The number of HTTP workers to launch",
     type=click.IntRange(min=1, max=multiprocessing.cpu_count() + 1),
     show_default=True,
     default=1,
 )
-@option("--host", help="Server under this host", default="127.0.0.1", show_default=True)
+@option("-H", "--host", help="Server under this host", default="127.0.0.1", show_default=True)
 @option(
+    "-F",
     "--fd",
     "--file-descriptor",
     help="Bind to a socket from this file descriptor.",
     type=int,
     default=None,
     show_default=True,
 )
-@option("--uds", "--unix-domain-socket", help="Bind to a UNIX domain socket.", default=None, show_default=True)
-@option("--debug", help="Run app in debug mode", is_flag=True)
-@option("--pdb", "use_pdb", help="Drop into PDB on an exception", is_flag=True)
-@option("--reload-dir", help="Directories to watch for file changes", multiple=True)
+@option("-U", "--uds", "--unix-domain-socket", help="Bind to a UNIX domain socket.", default=None, show_default=True)
+@option("-d", "--debug", help="Run app in debug mode", is_flag=True)
+@option("-P", "--pdb", "--use-pdb", help="Drop into PDB on an exception", is_flag=True)
 def run_command(
     reload: bool,
     port: int,
-    web_concurrency: int,
+    wc: int,
     host: str,
     fd: int | None,
     uds: str | None,
     debug: bool,
     reload_dir: tuple[str, ...],
-    use_pdb: bool,
+    pdb: bool,
     ctx: Context,
 ) -> None:
     """Run a Litestar app.
 
     The app can be either passed as a module path in the form of <module name>.<submodule>:<app instance or factory>,
     set as an environment variable LITESTAR_APP with the same format or automatically discovered from one of these
     canonical paths: app.py, asgi.py, application.py or app/__init__.py. When auto-discovering application factories,
     functions with the name ``create_app`` are considered, or functions that are annotated as returning a ``Litestar``
     instance.
     """
 
     if debug:
         os.environ["LITESTAR_DEBUG"] = "1"
 
-    if use_pdb:
+    if pdb:
         os.environ["LITESTAR_PDB"] = "1"
 
     env = cast(LitestarEnv, ctx.obj())
     app = env.app
 
     reload_dirs = env.reload_dirs or reload_dir
 
     host = env.host or host
     port = env.port if env.port is not None else port
     fd = env.fd if env.fd is not None else fd
     uds = env.uds or uds
     reload = env.reload or reload or bool(reload_dirs)
-    workers = env.web_concurrency or web_concurrency
+    workers = env.web_concurrency or wc
 
     console.rule("[yellow]Starting server process", align="left")
 
     show_app_info(app)
 
     if workers == 1 and not reload:
         uvicorn.run(
```

### Comparing `litestar-2.0.0b2/litestar/cli/commands/sessions.py` & `litestar-2.0.0b3/litestar/cli/commands/sessions.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,29 +32,29 @@
 
 
 @group(cls=LitestarGroup, name="sessions")
 def sessions_group() -> None:
     """Manage server-side sessions."""
 
 
-@sessions_group.command("delete")
+@sessions_group.command("delete")  # type: ignore
 @argument("session-id")
 def delete_session_command(session_id: str, app: Litestar) -> None:
     """Delete a specific session."""
     import anyio
 
     backend = get_session_backend(app)
     store = backend.config.get_store_from_app(app)
 
     if Confirm.ask(f"Delete session {session_id!r}?"):
         anyio.run(backend.delete, session_id, store)
         console.print(f"[green]Deleted session {session_id!r}")
 
 
-@sessions_group.command("clear")
+@sessions_group.command("clear")  # type: ignore
 def clear_sessions_command(app: Litestar) -> None:
     """Delete all sessions."""
     import anyio
 
     backend = get_session_backend(app)
     store = backend.config.get_store_from_app(app)
     if not hasattr(store, "delete_all"):
```

### Comparing `litestar-2.0.0b2/litestar/cli/main.py` & `litestar-2.0.0b3/litestar/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     click.rich_click.SHOW_METAVARS_COLUMN = True
     click.rich_click.APPEND_METAVARS_HELP = True
 
 
 __all__ = ("litestar_group",)
 
 
-@group(cls=LitestarExtensionGroup)
+@group(cls=LitestarExtensionGroup, context_settings={"help_option_names": ["-h", "--help"]})
 @option("--app", "app_path", help="Module path to a Litestar application")
 @option(
     "--app-dir",
     help="Look for APP in the specified directory, by adding this to the PYTHONPATH. Defaults to the current working directory.",
     default=None,
     type=ClickPath(dir_okay=True, file_okay=False, path_type=Path),
     show_default=False,
```

### Comparing `litestar-2.0.0b2/litestar/config/allowed_hosts.py` & `litestar-2.0.0b3/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/config/app.py` & `litestar-2.0.0b3/litestar/config/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         Middleware,
         ParametersMap,
         ResponseCookies,
         ResponseType,
         TypeEncodersMap,
     )
     from litestar.types.callable_types import LifespanHook
+    from litestar.types.composite_types import TypeDecodersSequence
     from litestar.types.empty import EmptyType
 
 
 __all__ = ("AppConfig",)
 
 
 @dataclass
@@ -184,14 +185,16 @@
     """
     tags: list[str] = field(default_factory=list)
     """A list of string tags that will be appended to the schema of all route handlers under the application."""
     template_config: TemplateConfig | None = field(default=None)
     """An instance of :class:`TemplateConfig <.template.TemplateConfig>`."""
     type_encoders: TypeEncodersMap | None = field(default=None)
     """A mapping of types to callables that transform them into types supported for serialization."""
+    type_decoders: TypeDecodersSequence | None = field(default=None)
+    """A sequence of tuples, each composed of a predicate testing for type identity and a msgspec hook for deserialization."""
     websocket_class: type[WebSocket] | None = field(default=None)
     """An optional subclass of :class:`WebSocket <.connection.WebSocket>` to use for websocket connections."""
     multipart_form_part_limit: int = field(default=1000)
     """The maximal number of allowed parts in a multipart/formdata request. This limit is intended to protect from
     DoS attacks."""
 
     def __post_init__(self) -> None:
```

### Comparing `litestar-2.0.0b2/litestar/config/compression.py` & `litestar-2.0.0b3/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/config/cors.py` & `litestar-2.0.0b3/litestar/config/cors.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,17 +108,17 @@
         if not self.is_allow_all_headers:
             headers["Access-Control-Allow-Headers"] = ", ".join(
                 sorted(set(self.allow_headers) | DEFAULT_ALLOWED_CORS_HEADERS)  # pyright: ignore
             )
         if self.allow_methods:
             headers["Access-Control-Allow-Methods"] = ", ".join(
                 sorted(
-                    set(self.allow_methods)
-                    if not self.is_allow_all_methods
-                    else {"DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"}
+                    {"DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"}
+                    if self.is_allow_all_methods
+                    else set(self.allow_methods)
                 )
             )
         return headers
 
     @cached_property
     def simple_headers(self) -> dict[str, str]:
         """Get cached simple headers.
```

### Comparing `litestar-2.0.0b2/litestar/config/csrf.py` & `litestar-2.0.0b3/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/config/response_cache.py` & `litestar-2.0.0b3/litestar/config/response_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, final
 from urllib.parse import urlencode
 
 __all__ = ("ResponseCacheConfig", "default_cache_key_builder", "CACHE_FOREVER")
 
 
 if TYPE_CHECKING:
     from litestar import Litestar
     from litestar.connection import Request
     from litestar.stores.base import Store
     from litestar.types import CacheKeyBuilder
 
 
+@final
 class CACHE_FOREVER:  # noqa: N801
     """Sentinel value indicating that a cached response should be stored without an expiration, explicitly skipping the
     default expiration
     """
 
 
 def default_cache_key_builder(request: Request[Any, Any, Any]) -> str:
```

### Comparing `litestar-2.0.0b2/litestar/connection/__init__.py` & `litestar-2.0.0b3/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/connection/base.py` & `litestar-2.0.0b3/litestar/connection/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 
 __all__ = ("ASGIConnection", "empty_receive", "empty_send")
 
 
 if TYPE_CHECKING:
     from typing import NoReturn
 
-    from pydantic import BaseModel
-
     from litestar.app import Litestar
-    from litestar.types import EmptyType
+    from litestar.types import DataContainerType, EmptyType
     from litestar.types.asgi_types import Message, Receive, Scope, Send
     from litestar.types.protocols import Logger
 
 UserT = TypeVar("UserT")
 AuthT = TypeVar("AuthT")
 HandlerT = TypeVar("HandlerT")
 StateT = TypeVar("StateT", bound=State)
@@ -180,17 +178,15 @@
         """Return the ``cookies`` of this connection's ``Scope``.
 
         Returns:
             Returns any cookies stored in the header as a parsed dictionary.
         """
         if self._cookies is Empty:
             cookies: dict[str, str] = {}
-            cookie_header = self.headers.get("cookie")
-
-            if cookie_header:
+            if cookie_header := self.headers.get("cookie"):
                 cookies = parse_cookie_string(cookie_header)
 
             self._cookies = self.scope["_cookies"] = cookies  # type: ignore[typeddict-unknown-key]
 
         return cast("dict[str, str]", self._cookies)
 
     @property
@@ -258,15 +254,15 @@
             A ``Logger`` instance.
 
         Raises:
             ImproperlyConfiguredException: if ``log_config`` has not been passed to the Litestar constructor.
         """
         return self.app.get_logger()
 
-    def set_session(self, value: dict[str, Any] | BaseModel | EmptyType) -> None:
+    def set_session(self, value: dict[str, Any] | DataContainerType | EmptyType) -> None:
         """Set the session in the connection's ``Scope``.
 
         If the :class:`SessionMiddleware <.middleware.session.base.SessionMiddleware>` is enabled, the session will be added
         to the response as a cookie header.
 
         Args:
             value: Dictionary or pydantic model instance for the session data.
```

### Comparing `litestar-2.0.0b2/litestar/connection/request.py` & `litestar-2.0.0b3/litestar/connection/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,55 +100,54 @@
         """Retrieve the json request body from the request.
 
         Returns:
             An arbitrary value
         """
         if self._json is Empty:
             body = await self.body()
-            self._json = self.scope["_json"] = decode_json(body or b"null")  # type: ignore[typeddict-unknown-key]
+            self._json = self.scope["_json"] = decode_json(body or b"null", type_decoders=self.route_handler.resolve_type_decoders())  # type: ignore[typeddict-unknown-key]
         return self._json
 
     async def msgpack(self) -> Any:
         """Retrieve the MessagePack request body from the request.
 
         Returns:
             An arbitrary value
         """
         if self._msgpack is Empty:
             body = await self.body()
-            self._msgpack = self.scope["_msgpack"] = decode_msgpack(body or b"\xc0")  # type: ignore[typeddict-unknown-key]
+            self._msgpack = self.scope["_msgpack"] = decode_msgpack(body or b"\xc0", type_decoders=self.route_handler.resolve_type_decoders())  # type: ignore[typeddict-unknown-key]
         return self._msgpack
 
     async def stream(self) -> AsyncGenerator[bytes, None]:
         """Return an async generator that streams chunks of bytes.
 
         Returns:
             An async generator.
 
         Raises:
             RuntimeError: if the stream is already consumed
         """
         if self._body is Empty:
-            if self.is_connected:
-                while event := await self.receive():
-                    if event["type"] == "http.request":
-                        if event["body"]:
-                            yield event["body"]
-
-                        if not event.get("more_body", False):
-                            break
+            if not self.is_connected:
+                raise InternalServerException("stream consumed")
+            while event := await self.receive():
+                if event["type"] == "http.request":
+                    if event["body"]:
+                        yield event["body"]
 
-                    if event["type"] == "http.disconnect":
-                        raise InternalServerException("client disconnected prematurely")
+                    if not event.get("more_body", False):
+                        break
 
-                self.is_connected = False
-                yield b""
+                if event["type"] == "http.disconnect":
+                    raise InternalServerException("client disconnected prematurely")
+
+            self.is_connected = False
+            yield b""
 
-            else:
-                raise InternalServerException("stream consumed")
         else:
             yield self._body
             yield b""
             return
 
     async def body(self) -> bytes:
         """Return the body of the request.
@@ -164,42 +163,43 @@
         """Retrieve form data from the request. If the request is either a 'multipart/form-data' or an
         'application/x-www-form- urlencoded', return a FormMultiDict instance populated with the values sent in the
         request, otherwise, an empty instance.
 
         Returns:
             A FormMultiDict instance
         """
-        if self._form is Empty:
-            content_type, options = self.content_type
-            if content_type == RequestEncodingType.MULTI_PART:
-                self._form = self.scope["_form"] = form_values = parse_multipart_form(  # type: ignore[typeddict-unknown-key]
-                    body=await self.body(),
-                    boundary=options.get("boundary", "").encode(),
-                    multipart_form_part_limit=self.app.multipart_form_part_limit,
-                )
-                return FormMultiDict(form_values)
-            if content_type == RequestEncodingType.URL_ENCODED:
-                self._form = self.scope["_form"] = form_values = parse_url_encoded_form_data(  # type: ignore[typeddict-unknown-key]
-                    await self.body(),
-                )
-                return FormMultiDict(form_values)
-            return FormMultiDict()
-        return FormMultiDict(self._form)
+        if self._form is not Empty:
+            return FormMultiDict(self._form)
+        content_type, options = self.content_type
+        if content_type == RequestEncodingType.MULTI_PART:
+            self._form = self.scope["_form"] = form_values = parse_multipart_form(  # type: ignore[typeddict-unknown-key]
+                body=await self.body(),
+                boundary=options.get("boundary", "").encode(),
+                multipart_form_part_limit=self.app.multipart_form_part_limit,
+            )
+            return FormMultiDict(form_values)
+        if content_type == RequestEncodingType.URL_ENCODED:
+            self._form = self.scope["_form"] = form_values = parse_url_encoded_form_data(  # type: ignore[typeddict-unknown-key]
+                await self.body(),
+            )
+            return FormMultiDict(form_values)
+        return FormMultiDict()
 
     async def send_push_promise(self, path: str) -> None:
         """Send a push promise.
 
         This method requires the `http.response.push` extension to be sent from the ASGI server.
 
         Args:
             path: Path to send the promise to.
 
         Returns:
             None
         """
         extensions: dict[str, dict[Any, Any]] = self.scope.get("extensions") or {}
         if "http.response.push" in extensions:
-            raw_headers = []
+            raw_headers: list[tuple[bytes, bytes]] = []
             for name in SERVER_PUSH_HEADERS:
-                for value in self.headers.getall(name, []):
-                    raw_headers.append((name.encode("latin-1"), value.encode("latin-1")))
+                raw_headers.extend(
+                    (name.encode("latin-1"), value.encode("latin-1")) for value in self.headers.getall(name, [])
+                )
             await self.send({"type": "http.response.push", "path": path, "headers": raw_headers})
```

### Comparing `litestar-2.0.0b2/litestar/connection/websocket.py` & `litestar-2.0.0b3/litestar/connection/websocket.py`

 * *Files 6% similar despite different names*

```diff
@@ -213,47 +213,47 @@
         Args:
             mode: Either ``text`` or ``binary``.
 
         Returns:
             An arbitrary value
         """
         data = await self.receive_data(mode=mode)
-        return decode_json(data)
+        return decode_json(value=data, type_decoders=self.route_handler.resolve_type_decoders())
 
     async def receive_msgpack(self) -> Any:
         """Receive data and decode it as MessagePack.
 
         Note that since MessagePack is a binary format, this method will always receive
         data in ``binary`` mode.
 
         Returns:
             An arbitrary value
         """
         data = await self.receive_data(mode="binary")
-        return decode_msgpack(data)
+        return decode_msgpack(value=data, type_decoders=self.route_handler.resolve_type_decoders())
 
     async def iter_json(self, mode: WebSocketMode = "text") -> AsyncGenerator[Any, None]:
         """Continuously receive data and yield it, decoding it as JSON in the process.
 
         Args:
             mode: Socket mode to use. Either ``text`` or ``binary``
         """
         async for data in self.iter_data(mode):
-            yield decode_json(data)
+            yield decode_json(value=data, type_decoders=self.route_handler.resolve_type_decoders())
 
     async def iter_msgpack(self) -> AsyncGenerator[Any, None]:
         """Continuously receive data and yield it, decoding it as MessagePack in the
         process.
 
         Note that since MessagePack is a binary format, this method will always receive
         data in ``binary`` mode.
 
         """
         async for data in self.iter_data(mode="binary"):
-            yield decode_msgpack(data)
+            yield decode_msgpack(value=data, type_decoders=self.route_handler.resolve_type_decoders())
 
     async def send_data(self, data: str | bytes, mode: WebSocketMode = "text", encoding: str = "utf-8") -> None:
         """Send a 'websocket.send' event.
 
         Args:
             data: Data to send.
             mode: The respective event key to use.
```

### Comparing `litestar-2.0.0b2/litestar/contrib/htmx/_utils.py` & `litestar-2.0.0b3/litestar/contrib/htmx/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,23 +58,22 @@
     TRIGGER_ID = "HX-Trigger"  # noqa: PIE796
     TRIGGER_NAME = "HX-Trigger-Name"
     TRIGGERING_EVENT = "Triggering-Event"
 
 
 def get_trigger_event_headers(trigger_event: TriggerEventType) -> dict[str, Any]:
     """Return headers for trigger event response."""
-    params = trigger_event["params"] or {}
     after_params: dict[EventAfterType, str] = {
         "receive": HTMXHeaders.TRIGGER_EVENT.value,
         "settle": HTMXHeaders.TRIGGER_AFTER_SETTLE.value,
         "swap": HTMXHeaders.TRIGGER_AFTER_SWAP.value,
     }
 
     if trigger_header := after_params.get(trigger_event["after"]):
-        return {trigger_header: encode_json({trigger_event["name"]: params}).decode()}
+        return {trigger_header: encode_json({trigger_event["name"]: trigger_event["params"] or {}}).decode()}
 
     raise ImproperlyConfiguredException(
         "invalid value for 'after' param- allowed values are 'receive', 'settle' or 'swap'."
     )
 
 
 def get_redirect_header(url: str) -> dict[str, Any]:
@@ -96,39 +95,32 @@
     """Return headers for replace url in browser tab response."""
     url = (url if url != "False" else "false") if isinstance(url, str) else "false"
     return {HTMXHeaders.REPLACE_URL: url}
 
 
 def get_refresh_header(refresh: bool) -> dict[str, Any]:
     """Return headers for client refresh response."""
-    value = ""
-    if refresh:
-        value = "true"
-    return {HTMXHeaders.REFRESH.value: value}
+    return {HTMXHeaders.REFRESH.value: "true" if refresh else ""}
 
 
 def get_reswap_header(method: ReSwapMethod) -> dict[str, Any]:
     """Return headers for change swap method response."""
     return {HTMXHeaders.RE_SWAP.value: method}
 
 
 def get_retarget_header(target: str) -> dict[str, Any]:
     """Return headers for change target element response."""
     return {HTMXHeaders.RE_TARGET.value: target}
 
 
 def get_location_headers(location: LocationType) -> dict[str, Any]:
     """Return headers for redirect without page-reload response."""
-    spec: dict[str, Any] = {}
-    for key, value in location.items():
-        if value:
-            spec[key] = value
-    if not spec:
-        raise ValueError("redirect_to is required parameter.")
-    return {HTMXHeaders.LOCATION.value: encode_json(spec).decode()}
+    if spec := {key: value for key, value in location.items() if value}:
+        return {HTMXHeaders.LOCATION.value: encode_json(spec).decode()}
+    raise ValueError("redirect_to is required parameter.")
 
 
 def get_headers(hx_headers: HtmxHeaderType) -> dict[str, Any]:
     """Return headers for HTMX responses."""
     if not hx_headers:
         raise ValueError("Value for hx_headers cannot be None.")
     htmx_headers_dict: dict[str, Callable] = {
```

### Comparing `litestar-2.0.0b2/litestar/contrib/htmx/request.py` & `litestar-2.0.0b3/litestar/contrib/htmx/request.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from contextlib import suppress
 from functools import cached_property
 from typing import TYPE_CHECKING, Any
 from urllib.parse import unquote, urlsplit, urlunsplit
 
 from litestar import Request
 from litestar.contrib.htmx._utils import HTMXHeaders
 from litestar.exceptions import SerializationException
@@ -19,23 +20,24 @@
 class HTMXDetails:
     """HTMXDetails holds all the values sent by HTMX client in headers and provide convenient properties."""
 
     def __init__(self, request: Request) -> None:
         """Initialize :class:`HTMXDetails`"""
         self.request = request
 
-    def _get_header_value(self, name: str) -> str | None:
+    def _get_header_value(self, name: HTMXHeaders) -> str | None:
         """Parse request header
 
         Check for uri encoded header and unquotes it in readable format.
         """
-        value = self.request.headers.get(name) or None
-        if value and self.request.headers.get(name + "-URI-AutoEncoded") == "true":
-            return unquote(value)
-        return value
+
+        if value := self.request.headers.get(name.value.lower()):
+            is_uri_encoded = self.request.headers.get(f"{name.value.lower()}-uri-autoencoded") == "true"
+            return unquote(value) if is_uri_encoded else value
+        return None
 
     def __bool__(self) -> bool:
         """Check if request is sent by an HTMX client."""
         return self._get_header_value(HTMXHeaders.REQUEST) == "true"
 
     @cached_property
     def boosted(self) -> bool:
@@ -89,21 +91,18 @@
 
     @cached_property
     def triggering_event(self) -> Any:
         """Name of the triggered event.
 
         This value is added by ``event-header`` extension of HTMX to the ``Triggering-Event`` header to requests.
         """
-        value = self._get_header_value(HTMXHeaders.TRIGGERING_EVENT)
-        if value is not None:
-            try:
-                value = decode_json(value)
-            except SerializationException:
-                value = None
-        return value
+        if value := self._get_header_value(HTMXHeaders.TRIGGERING_EVENT):
+            with suppress(SerializationException):
+                return decode_json(value=value, type_decoders=self.request.route_handler.resolve_type_decoders())
+        return None
 
 
 class HTMXRequest(Request):
     """HTMX Request class to work with HTMX client."""
 
     __slots__ = ("htmx",)
```

### Comparing `litestar-2.0.0b2/litestar/contrib/htmx/response.py` & `litestar-2.0.0b3/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/htmx/types.py` & `litestar-2.0.0b3/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/jinja.py` & `litestar-2.0.0b3/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/jwt/__init__.py` & `litestar-2.0.0b3/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/jwt/jwt_auth.py` & `litestar-2.0.0b3/litestar/contrib/jwt/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/jwt/jwt_token.py` & `litestar-2.0.0b3/litestar/contrib/jwt/jwt_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 from dataclasses import asdict, dataclass, field
 from datetime import datetime, timezone
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any
 
 from jose import JWSError, JWTError, jwt
 
 from litestar.exceptions import ImproperlyConfiguredException, NotAuthorizedException
 
 if TYPE_CHECKING:
     from typing_extensions import Self
@@ -51,24 +51,24 @@
     """Extra fields that were found on the JWT token."""
 
     def __post_init__(self) -> None:
         if len(self.sub) < 1:
             raise ImproperlyConfiguredException("sub must be a string with a length greater than 0")
 
         if isinstance(self.exp, datetime) and (
-            (exp := _normalize_datetime(self.exp))
-            and exp.timestamp() >= _normalize_datetime(datetime.now(timezone.utc)).timestamp()
+            (exp := _normalize_datetime(self.exp)).timestamp()
+            >= _normalize_datetime(datetime.now(timezone.utc)).timestamp()
         ):
             self.exp = exp
         else:
             raise ImproperlyConfiguredException("exp value must be a datetime in the future")
 
         if isinstance(self.iat, datetime) and (
-            (iat := _normalize_datetime(self.iat))
-            and iat.timestamp() <= _normalize_datetime(datetime.now(timezone.utc)).timestamp()
+            (iat := _normalize_datetime(self.iat)).timestamp()
+            <= _normalize_datetime(datetime.now(timezone.utc)).timestamp()
         ):
             self.iat = iat
         else:
             raise ImproperlyConfiguredException("iat must be a current or past time")
 
     @classmethod
     def decode(cls, encoded_token: str, secret: str | dict[str, str], algorithm: str) -> Self:
@@ -108,15 +108,12 @@
         Returns:
             An encoded token string.
 
         Raises:
             ImproperlyConfiguredException: If encoding fails.
         """
         try:
-            return cast(
-                "str",
-                jwt.encode(
-                    claims={k: v for k, v in asdict(self).items() if v is not None}, key=secret, algorithm=algorithm
-                ),
+            return jwt.encode(
+                claims={k: v for k, v in asdict(self).items() if v is not None}, key=secret, algorithm=algorithm
             )
         except (JWTError, JWSError) as e:
             raise ImproperlyConfiguredException("Failed to encode token") from e
```

### Comparing `litestar-2.0.0b2/litestar/contrib/jwt/middleware.py` & `litestar-2.0.0b3/litestar/contrib/jwt/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Awaitable
+from typing import TYPE_CHECKING
 
 from litestar.contrib.jwt.jwt_token import Token
 from litestar.exceptions import NotAuthorizedException
 from litestar.middleware.authentication import (
     AbstractAuthenticationMiddleware,
     AuthenticationResult,
 )
@@ -29,15 +29,15 @@
     def __init__(
         self,
         app: ASGIApp,
         algorithm: str,
         auth_header: str,
         exclude: str | list[str] | None,
         exclude_opt_key: str,
-        retrieve_user_handler: AsyncCallable[[Token, ASGIConnection[Any, Any, Any, Any]], Awaitable[Any]],
+        retrieve_user_handler: AsyncCallable[[Token, ASGIConnection[Any, Any, Any, Any]], Any],
         scopes: Scopes,
         token_secret: str,
     ) -> None:
         """Check incoming requests for an encoded token in the auth header specified, and if present retrieve the user
         from persistence using the provided function.
 
         Args:
@@ -113,15 +113,15 @@
         self,
         algorithm: str,
         app: ASGIApp,
         auth_cookie_key: str,
         auth_header: str,
         exclude: str | list[str] | None,
         exclude_opt_key: str,
-        retrieve_user_handler: AsyncCallable[[Token, ASGIConnection[Any, Any, Any, Any]], Awaitable[Any]],
+        retrieve_user_handler: AsyncCallable[[Token, ASGIConnection[Any, Any, Any, Any]], Any],
         scopes: Scopes,
         token_secret: str,
     ) -> None:
         """Check incoming requests for an encoded token in the auth header or cookie name specified, and if present
         retrieves the user from persistence using the provided function.
 
         Args:
```

### Comparing `litestar-2.0.0b2/litestar/contrib/mako.py` & `litestar-2.0.0b3/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/msgspec.py` & `litestar-2.0.0b3/litestar/dto/msgspec_dto_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,58 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Generic, TypeVar, cast
+from dataclasses import replace
+from typing import TYPE_CHECKING, Collection, Generic, TypeVar, cast
 
 from msgspec import NODEFAULT, Struct, inspect
 
-from litestar.dto.factory.abc import AbstractDTOFactory
-from litestar.dto.factory.data_structures import FieldDefinition
-from litestar.dto.factory.field import DTO_FIELD_META_KEY, DTOField
-from litestar.dto.factory.utils import get_model_type_hints
+from litestar.dto._utils import get_model_type_hints
+from litestar.dto.base_factory import AbstractDTOFactory
+from litestar.dto.data_structures import DTOFieldDefinition
+from litestar.dto.field import DTO_FIELD_META_KEY, DTOField
 from litestar.types.empty import Empty
 from litestar.utils.helpers import get_fully_qualified_class_name
 
 if TYPE_CHECKING:
-    from typing import Any, ClassVar, Collection, Generator
+    from typing import Any, ClassVar, Generator
+
+    from litestar.typing import FieldDefinition
 
-    from litestar.typing import ParsedType
 
 __all__ = ("MsgspecDTO",)
 
 T = TypeVar("T", bound="Struct | Collection[Struct]")
 
 
 class MsgspecDTO(AbstractDTOFactory[T], Generic[T]):
     """Support for domain modelling with Msgspec."""
 
     __slots__ = ()
 
     model_type: ClassVar[type[Struct]]
 
     @classmethod
-    def generate_field_definitions(cls, model_type: type[Struct]) -> Generator[FieldDefinition, None, None]:
+    def generate_field_definitions(cls, model_type: type[Struct]) -> Generator[DTOFieldDefinition, None, None]:
         msgspec_fields = {f.name: f for f in cast("inspect.StructType", inspect.type_info(model_type)).fields}
 
         def default_or_empty(value: Any) -> Any:
-            if value is NODEFAULT:
-                return Empty
-            return value
+            return Empty if value is NODEFAULT else value
 
-        for key, parsed_type in get_model_type_hints(model_type).items():
+        for key, field_definition in get_model_type_hints(model_type).items():
             msgspec_field = msgspec_fields[key]
+            dto_field = (field_definition.extra or {}).pop(DTO_FIELD_META_KEY, DTOField())
 
-            if isinstance(msgspec_field.type, inspect.Metadata):
-                dto_field = (msgspec_field.type.extra or {}).get(DTO_FIELD_META_KEY, DTOField())
-            else:
-                dto_field = DTOField()
-
-            field_def = FieldDefinition(
-                name=key,
+            yield replace(
+                DTOFieldDefinition.from_field_definition(
+                    field_definition=field_definition,
+                    dto_field=dto_field,
+                    unique_model_name=get_fully_qualified_class_name(model_type),
+                    default_factory=default_or_empty(msgspec_field.default_factory),
+                    dto_for=None,
+                ),
                 default=default_or_empty(msgspec_field.default),
-                parsed_type=parsed_type,
-                default_factory=default_or_empty(msgspec_field.default_factory),
-                dto_field=dto_field,
-                unique_model_name=get_fully_qualified_class_name(model_type),
-                dto_for=None,
+                name=key,
             )
 
-            yield field_def
-
     @classmethod
-    def detect_nested_field(cls, parsed_type: ParsedType) -> bool:
-        return parsed_type.is_subclass_of(Struct)
+    def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
+        return field_definition.is_subclass_of(Struct)
```

### Comparing `litestar-2.0.0b2/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.0.0b3/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/opentelemetry/config.py` & `litestar-2.0.0b3/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.0.0b3/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/prometheus/config.py` & `litestar-2.0.0b3/litestar/contrib/prometheus/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/prometheus/controller.py` & `litestar-2.0.0b3/litestar/contrib/prometheus/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/prometheus/middleware.py` & `litestar-2.0.0b3/litestar/contrib/prometheus/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import time
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, cast
 
 from litestar.connection.request import Request
+from litestar.enums import ScopeType
 from litestar.exceptions import MissingDependencyException
 from litestar.middleware.base import AbstractMiddleware
 
 __all__ = ("PrometheusMiddleware",)
 
 from litestar.status_codes import HTTP_500_INTERNAL_SERVER_ERROR
 
@@ -111,15 +112,15 @@
             request: The request object.
 
         Returns:
             A dictionary of default labels.
         """
 
         return {
-            "method": request.method,
+            "method": request.method if request.scope["type"] == ScopeType.HTTP else request.scope["type"],
             "path": request.url.path,
             "status_code": 200,
             "app_name": self._config.app_name,
         }
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
```

### Comparing `litestar-2.0.0b2/litestar/contrib/pydantic.py` & `litestar-2.0.0b3/litestar/dto/dataclass_dto_factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 from __future__ import annotations
 
+from dataclasses import MISSING, fields, replace
 from typing import TYPE_CHECKING, Generic, TypeVar
 
-from pydantic import BaseModel
-
-from litestar.dto.factory.abc import AbstractDTOFactory
-from litestar.dto.factory.data_structures import FieldDefinition
-from litestar.dto.factory.field import DTO_FIELD_META_KEY, DTOField
-from litestar.dto.factory.utils import get_model_type_hints
+from litestar.dto._utils import get_model_type_hints
+from litestar.dto.base_factory import AbstractDTOFactory
+from litestar.dto.data_structures import DTOFieldDefinition
+from litestar.dto.field import DTO_FIELD_META_KEY, DTOField
+from litestar.params import DependencyKwarg, KwargDefinition
 from litestar.types.empty import Empty
 from litestar.utils.helpers import get_fully_qualified_class_name
 
 if TYPE_CHECKING:
-    from typing import Any, ClassVar, Collection, Generator
+    from typing import ClassVar, Collection, Generator
 
-    from pydantic.fields import ModelField
+    from litestar.types.protocols import DataclassProtocol
+    from litestar.typing import FieldDefinition
 
-    from litestar.typing import ParsedType
 
-__all__ = ("PydanticDTO",)
+__all__ = ("DataclassDTO", "T")
 
-T = TypeVar("T", bound="BaseModel | Collection[BaseModel]")
+T = TypeVar("T", bound="DataclassProtocol | Collection[DataclassProtocol]")
+AnyDataclass = TypeVar("AnyDataclass", bound="DataclassProtocol")
 
 
-class PydanticDTO(AbstractDTOFactory[T], Generic[T]):
-    """Support for domain modelling with Pydantic."""
+class DataclassDTO(AbstractDTOFactory[T], Generic[T]):
+    """Support for domain modelling with dataclasses."""
 
     __slots__ = ()
 
-    model_type: ClassVar[type[BaseModel]]
+    model_type: ClassVar[type[DataclassProtocol]]
 
     @classmethod
-    def generate_field_definitions(cls, model_type: type[BaseModel]) -> Generator[FieldDefinition, None, None]:
-        model_parsed_types = get_model_type_hints(model_type)
-        for key, model_field in model_type.__fields__.items():
-            parsed_type = model_parsed_types[key]
-            model_field = model_type.__fields__[key]
-            dto_field = model_field.field_info.extra.get(DTO_FIELD_META_KEY, DTOField())
-
-            def determine_default(_parsed_type: ParsedType, _model_field: ModelField) -> Any:
-                if (
-                    _model_field.default is Ellipsis
-                    or _model_field.default_factory is not None
-                    or (_model_field.default is None and not _parsed_type.is_optional)
-                ):
-                    return Empty
-
-                return _model_field.default
-
-            field_def = FieldDefinition(
+    def generate_field_definitions(
+        cls, model_type: type[DataclassProtocol]
+    ) -> Generator[DTOFieldDefinition, None, None]:
+        dc_fields = {f.name: f for f in fields(model_type)}
+        for key, field_definition in get_model_type_hints(model_type).items():
+            if not (dc_field := dc_fields.get(key)):
+                continue
+
+            default = dc_field.default if dc_field.default is not MISSING else Empty
+            default_factory = dc_field.default_factory if dc_field.default_factory is not MISSING else None
+            field_defintion = replace(
+                DTOFieldDefinition.from_field_definition(
+                    field_definition=field_definition,
+                    default_factory=default_factory,
+                    dto_field=dc_field.metadata.get(DTO_FIELD_META_KEY, DTOField()),
+                    unique_model_name=get_fully_qualified_class_name(model_type),
+                    dto_for=None,
+                ),
                 name=key,
-                default=determine_default(parsed_type, model_field),
-                parsed_type=parsed_type,
-                default_factory=model_field.default_factory or Empty,
-                dto_field=dto_field,
-                unique_model_name=get_fully_qualified_class_name(model_type),
-                dto_for=None,
+                default=default,
             )
 
-            yield field_def
+            yield replace(field_defintion, default=Empty, kwarg_definition=default) if isinstance(
+                default, (KwargDefinition, DependencyKwarg)
+            ) else field_defintion
 
     @classmethod
-    def detect_nested_field(cls, parsed_type: ParsedType) -> bool:
-        return parsed_type.is_subclass_of(BaseModel)
+    def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
+        return hasattr(field_definition.annotation, "__dataclass_fields__")
```

### Comparing `litestar-2.0.0b2/litestar/contrib/repository/abc/_async.py` & `litestar-2.0.0b3/litestar/contrib/repository/abc/_async.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/repository/abc/_sync.py` & `litestar-2.0.0b3/litestar/contrib/repository/abc/_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/repository/filters.py` & `litestar-2.0.0b3/litestar/contrib/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/repository/handlers.py` & `litestar-2.0.0b3/litestar/contrib/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/repository/testing/generic_mock_repository.py` & `litestar-2.0.0b3/litestar/contrib/repository/testing/generic_mock_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     def _now(self) -> datetime:
         return datetime.now(tz=self.tz).replace(tzinfo=None)
 
     def _update_audit_attributes(self, data: ModelT, now: datetime | None = None, do_created: bool = False) -> ModelT:
         now = now or self._now()
         if self._model_has_updated_at:
             data.updated_at = now  # type:ignore[attr-defined]
-        if self._model_has_updated_at and do_created:
-            data.created_at = now  # type:ignore[attr-defined]
+            if do_created:
+                data.created_at = now  # type:ignore[attr-defined]
         return data
 
     async def add(self, data: ModelT) -> ModelT:
         """Add ``data`` to the collection.
 
         Args:
             data: Instance to be added to the collection.
@@ -187,15 +187,15 @@
             match_fields: a list of keys to use to match the existing model.  When empty, all fields are matched.
             **kwargs: Identifier of the instance to be retrieved.
 
         Returns:
             a tuple that includes the instance and whether it needed to be created.
 
         """
-        match_fields = match_fields if match_fields else self.match_fields
+        match_fields = match_fields or self.match_fields
         if isinstance(match_fields, str):
             match_fields = [match_fields]
         if match_fields:
             match_filter = {
                 field_name: field_value
                 for field_name in match_fields
                 if (field_value := kwargs.get(field_name)) is not None
@@ -425,16 +425,16 @@
     def _now(self) -> datetime:
         return datetime.now(tz=self.tz).replace(tzinfo=None)
 
     def _update_audit_attributes(self, data: ModelT, now: datetime | None = None, do_created: bool = False) -> ModelT:
         now = now or self._now()
         if self._model_has_updated_at:
             data.updated_at = now  # type:ignore[attr-defined]
-        if self._model_has_updated_at and do_created:
-            data.created_at = now  # type:ignore[attr-defined]
+            if do_created:
+                data.created_at = now  # type:ignore[attr-defined]
         return data
 
     def add(self, data: ModelT) -> ModelT:
         """Add ``data`` to the collection.
 
         Args:
             data: Instance to be added to the collection.
@@ -497,16 +497,15 @@
 
         Returns:
             The deleted instances.
 
         """
         instances: list[ModelT] = []
         for item_id in item_ids:
-            obj = self.get_one_or_none(**{self.id_attribute: item_id})
-            if obj:
+            if obj := self.get_one_or_none(**{self.id_attribute: item_id}):
                 obj = self.delete(obj.id)
                 instances.append(obj)
         return instances
 
     def exists(self, **kwargs: Any) -> bool:
         """Return true if the object specified by ``kwargs`` exists.
 
@@ -542,27 +541,26 @@
             match_fields: a list of keys to use to match the existing model.  When empty, all fields are matched.
             **kwargs: Identifier of the instance to be retrieved.
 
         Returns:
             a tuple that includes the instance and whether it needed to be created.
 
         """
-        match_fields = match_fields if match_fields else self.match_fields
+        match_fields = match_fields or self.match_fields
         if isinstance(match_fields, str):
             match_fields = [match_fields]
         if match_fields:
             match_filter = {
                 field_name: field_value
                 for field_name in match_fields
                 if (field_value := kwargs.get(field_name)) is not None
             }
         else:
             match_filter = kwargs
-        existing = self.get_one_or_none(**match_filter)
-        if existing:
+        if existing := self.get_one_or_none(**match_filter):
             for field_name, new_field_value in kwargs.items():
                 field = getattr(existing, field_name, None)
                 if field and field != new_field_value:
                     setattr(existing, field_name, new_field_value)
 
             return existing, False
         return self.add(self.model_type(**kwargs)), True  # pyright: ignore[reportGeneralTypeIssues]
@@ -660,17 +658,15 @@
         Returns:
             The updated or created instance.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
         """
         item_id = self.get_id_attribute_value(data)
-        if item_id in self.collection:
-            return self.update(data)
-        return self.add(data)
+        return self.update(data) if item_id in self.collection else self.add(data)
 
     def list_and_count(
         self,
         *filters: FilterTypes,
         **kwargs: Any,
     ) -> tuple[list[ModelT], int]:
         """Get a list of instances, optionally filtered with a total row count.
```

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/base.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     Args:
         session: The sync :class:`Session <sqlalchemy.orm.Session>` instance that underlies the async
             session.
     """
     for instance in session.dirty:
         if hasattr(instance, "updated_at"):
-            instance.updated = (datetime.now(timezone.utc),)
+            instance.updated_at = datetime.now(timezone.utc)
 
 
 @runtime_checkable
 class ModelProtocol(Protocol):
     """The base SQLAlchemy model protocol."""
 
     __table__: FromClause
@@ -87,22 +87,24 @@
 
 class UUIDPrimaryKey:
     """UUID Primary Key Field Mixin."""
 
     id: Mapped[UUID] = mapped_column(default=uuid4, primary_key=True)  # pyright: ignore
     """UUID Primary key column."""
 
+    # noinspection PyMethodParameters
     @declared_attr
     def _sentinel(cls) -> Mapped[int]:
-        return orm_insert_sentinel()
+        return orm_insert_sentinel(name="sa_orm_sentinel")
 
 
 class BigIntPrimaryKey:
     """BigInt Primary Key Field Mixin."""
 
+    # noinspection PyMethodParameters
     @declared_attr
     def id(cls) -> Mapped[int]:
         """BigInt Primary key column."""
         return mapped_column(
             BigIntIdentity,
             Sequence(f"{cls.__tablename__}_id_seq", optional=False),  # type: ignore[attr-defined] # pyright: ignore
             primary_key=True,
@@ -110,20 +112,20 @@
 
 
 class AuditColumns:
     """Created/Updated At Fields Mixin."""
 
     created_at: Mapped[datetime] = mapped_column(  # pyright: ignore
         DateTimeUTC(timezone=True),
-        default=datetime.now(timezone.utc),
+        default=lambda: datetime.now(timezone.utc),
     )
     """Date/time of instance creation."""
     updated_at: Mapped[datetime] = mapped_column(  # pyright: ignore
         DateTimeUTC(timezone=True),
-        default=datetime.now(timezone.utc),
+        default=lambda: datetime.now(timezone.utc),
     )
     """Date/time of instance last update."""
 
 
 class CommonTableAttributes:
     """Common attributes for SQLALchemy tables."""
 
@@ -139,15 +141,15 @@
 
     def to_dict(self, exclude: set[str] | None = None) -> dict[str, Any]:
         """Convert model to dictionary.
 
         Returns:
             dict[str, Any]: A dict representation of the model
         """
-        exclude = {"_sentinel"}.union(self._sa_instance_state.unloaded).union(exclude or [])  # type: ignore[attr-defined]
+        exclude = {"sa_orm_sentinel", "_sentinel"}.union(self._sa_instance_state.unloaded).union(exclude or [])  # type: ignore[attr-defined]
         return {field.name: getattr(self, field.name) for field in self.__table__.columns if field.name not in exclude}
 
 
 def create_registry() -> registry:
     """Create a new SQLAlchemy registry."""
     meta = MetaData(naming_convention=convention)
     return registry(
```

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 
 async def default_before_send_handler(message: Message, scope: Scope) -> None:
     """Handle closing and cleaning up sessions before sending.
 
     Args:
         message: ASGI-``Message``
-        _: A ``State`` (not used)
         scope: An ASGI-``Scope``
 
     Returns:
         None
     """
     session = cast("AsyncSession | None", get_litestar_scope_state(scope, SESSION_SCOPE_KEY))
     if session and message["type"] in SESSION_TERMINUS_ASGI_EVENTS:
```

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/common.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/common.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/engine.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from litestar.exceptions import MissingDependencyException
 from litestar.serialization import decode_json, encode_json
 from litestar.types import Empty
 
 try:
     import sqlalchemy  # noqa: F401
 except ImportError as e:
-    raise MissingDependencyException("sqlalchemy is not installed") from e
+    raise MissingDependencyException("sqlalchemy") from e
 
 if TYPE_CHECKING:
     from typing import Any, Mapping
 
     from sqlalchemy.engine.interfaces import IsolationLevel
     from sqlalchemy.pool import Pool
     from typing_extensions import TypeAlias
```

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 
 def default_before_send_handler(message: Message, scope: Scope) -> None:
     """Handle closing and cleaning up sessions before sending.
 
     Args:
         message: ASGI-``Message``
-        _: A ``State`` (not used)
         scope: An ASGI-``Scope``
 
     Returns:
         None
     """
     session = cast("Session | None", get_litestar_scope_state(scope, SESSION_SCOPE_KEY))
     if session and message["type"] in SESSION_TERMINUS_ASGI_EVENTS:
```

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/plugin.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/serialization.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/serialization.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,36 +6,37 @@
 
 from litestar.contrib.sqlalchemy.dto import SQLAlchemyDTO
 from litestar.plugins import SerializationPluginProtocol
 
 from . import _slots_base
 
 if TYPE_CHECKING:
-    from litestar.typing import ParsedType
+    from litestar.typing import FieldDefinition
 
 
 class SQLAlchemySerializationPlugin(SerializationPluginProtocol, _slots_base.SlotsBase):
     __slots__ = ()
 
     def __init__(self) -> None:
         self._type_dto_map: dict[type[DeclarativeBase], type[SQLAlchemyDTO[Any]]] = {}
 
-    def supports_type(self, parsed_type: ParsedType) -> bool:
+    def supports_type(self, field_definition: FieldDefinition) -> bool:
         return (
-            parsed_type.is_collection and parsed_type.has_inner_subclass_of(DeclarativeBase)
-        ) or parsed_type.is_subclass_of(DeclarativeBase)
+            field_definition.is_collection and field_definition.has_inner_subclass_of(DeclarativeBase)
+        ) or field_definition.is_subclass_of(DeclarativeBase)
 
-    def create_dto_for_type(self, parsed_type: ParsedType) -> type[SQLAlchemyDTO[Any]]:
+    def create_dto_for_type(self, field_definition: FieldDefinition) -> type[SQLAlchemyDTO[Any]]:
         # assumes that the type is a container of SQLAlchemy models or a single SQLAlchemy model
-        for inner_type in parsed_type.inner_types:
-            if inner_type.is_subclass_of(DeclarativeBase):
-                annotation = inner_type.annotation
-                break
-        else:
-            annotation = parsed_type.annotation
-
+        annotation = next(
+            (
+                inner_type.annotation
+                for inner_type in field_definition.inner_types
+                if inner_type.is_subclass_of(DeclarativeBase)
+            ),
+            field_definition.annotation,
+        )
         if annotation in self._type_dto_map:
             return self._type_dto_map[annotation]
 
         self._type_dto_map[annotation] = dto_type = SQLAlchemyDTO[annotation]  # type:ignore[valid-type]
 
         return dto_type
```

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_util.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_util.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/types.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/contrib/sqlalchemy/types.py` & `litestar-2.0.0b3/litestar/contrib/sqlalchemy/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,25 +104,21 @@
     def coerce_compared_value(self, op: Any, value: Any) -> Any:
         return self.impl.coerce_compared_value(op=op, value=value)  # type: ignore
 
     def load_dialect_impl(self, dialect: Dialect) -> TypeEngine[Any]:
         return dialect.type_descriptor(ORA_BLOB())
 
     def process_bind_param(self, value: Any, dialect: Dialect) -> Any | None:
-        if value is None:
-            return value
-        return encode_json(value)
+        return value if value is None else encode_json(value)
 
     def process_result_value(self, value: bytes | None, dialect: Dialect) -> Any | None:
-        if value is None:
-            return value
-        return decode_json(value)
+        return value if value is None else decode_json(value=value)
 
     def _should_create_constraint(self, compiler: Any, **kw: Any) -> bool:
-        return bool(compiler.dialect.name == "oracle")
+        return cast("bool", compiler.dialect.name == "oracle")
 
     def _variant_mapping_for_set_table(self, column: Any) -> dict | None:
         if column.type._variant_mapping:
             variant_mapping = dict(column.type._variant_mapping)
             variant_mapping["_default"] = column.type
         else:
             variant_mapping = None
```

### Comparing `litestar-2.0.0b2/litestar/controller.py` & `litestar-2.0.0b3/litestar/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         Guard,
         Middleware,
         OptionalSequence,
         ParametersMap,
         ResponseCookies,
         TypeEncodersMap,
     )
-    from litestar.types.composite_types import ResponseHeaders
+    from litestar.types.composite_types import ResponseHeaders, TypeDecodersSequence
     from litestar.types.empty import EmptyType
 
 
 class Controller:
     """The Litestar Controller class.
 
     Subclass this class to create 'view' like components and utilize OOP.
@@ -63,14 +63,15 @@
         "response_cookies",
         "response_headers",
         "return_dto",
         "security",
         "signature_namespace",
         "tags",
         "type_encoders",
+        "type_decoders",
     )
 
     after_request: AfterRequestHookHandler | None
     """A sync or async function executed before a :class:`Request <.connection.Request>` is passed to any route handler.
 
     If this function returns a value, the request will not reach the route handler, and instead this value will be used.
     """
@@ -138,14 +139,16 @@
     """A sequence of string tags that will be appended to the schema of all route handlers under the controller."""
     security: OptionalSequence[SecurityRequirement]
     """A sequence of dictionaries that to the schema of all route handlers under the controller."""
     signature_namespace: dict[str, Any]
     """A mapping of names to types for use in forward reference resolution during signature modelling."""
     type_encoders: TypeEncodersMap | None
     """A mapping of types to callables that transform them into types supported for serialization."""
+    type_decoders: TypeDecodersSequence | None
+    """A sequence of tuples, each composed of a predicate testing for type identity and a msgspec hook for deserialization."""
 
     def __init__(self, owner: Router) -> None:
         """Initialize a controller.
 
         Should only be called by routers as part of controller registration.
 
         Args:
@@ -184,15 +187,15 @@
         from litestar import websocket_listener
 
         route_handlers: list[BaseRouteHandler] = []
 
         for field_name in set(dir(self)) - set(dir(Controller)):
             if (attr := getattr(self, field_name, None)) and isinstance(attr, BaseRouteHandler):
                 # we are special casing here because the websocket_listener context cannot be deep copied without breaking
-                route_handler = deepcopy(attr) if not isinstance(attr, websocket_listener) else copy(attr)
+                route_handler = copy(attr) if isinstance(attr, websocket_listener) else deepcopy(attr)
                 route_handler.fn.value = partial(route_handler.fn.value, self)
                 route_handler.owner = self
                 route_handlers.append(route_handler)
 
         self.validate_route_handlers(route_handlers=route_handlers)
 
         return route_handlers
```

### Comparing `litestar-2.0.0b2/litestar/data_extractors.py` & `litestar-2.0.0b3/litestar/data_extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,27 +264,25 @@
 
         Args:
             request: A :class:`Request <litestar.connection.Request>` instance.
 
         Returns:
             Either the parsed request body or the raw byte-string.
         """
-        if request.method != HttpMethod.GET:
-            if not self.parse_body:
-                return await request.body()
-            request_encoding_type = request.content_type[0]
-            if request_encoding_type == RequestEncodingType.JSON:
-                return await request.json()
-            form_data = await request.form()
-            if request_encoding_type == RequestEncodingType.URL_ENCODED:
-                return dict(form_data)
-            return {
-                key: repr(value) if isinstance(value, UploadFile) else value for key, value in form_data.multi_items()
-            }
-        return None
+        if request.method == HttpMethod.GET:
+            return None
+        if not self.parse_body:
+            return await request.body()
+        request_encoding_type = request.content_type[0]
+        if request_encoding_type == RequestEncodingType.JSON:
+            return await request.json()
+        form_data = await request.form()
+        if request_encoding_type == RequestEncodingType.URL_ENCODED:
+            return dict(form_data)
+        return {key: repr(value) if isinstance(value, UploadFile) else value for key, value in form_data.multi_items()}
 
 
 class ExtractedResponseData(TypedDict, total=False):
     """Dictionary representing extracted response data."""
 
     body: bytes
     status_code: int
@@ -402,14 +400,13 @@
             messages: A tuple containing
                 :class:`HTTPResponseStartEvent <litestar.types.asgi_types.HTTPResponseStartEvent>`
                 and :class:`HTTPResponseBodyEvent <litestar.types.asgi_types.HTTPResponseBodyEvent>`.
 
         Returns:
             The Response's cookies dict.
         """
-        cookie_string = ";".join(
+        if cookie_string := ";".join(
             [x[1].decode("latin-1") for x in filter(lambda x: x[0].lower() == b"set-cookie", messages[0]["headers"])]
-        )
-        if cookie_string:
+        ):
             parsed_cookies = parse_cookie_string(cookie_string)
             return _obfuscate(parsed_cookies, self.obfuscate_cookies) if self.obfuscate_cookies else parsed_cookies
         return {}
```

### Comparing `litestar-2.0.0b2/litestar/datastructures/__init__.py` & `litestar-2.0.0b3/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/datastructures/cookie.py` & `litestar-2.0.0b3/litestar/datastructures/cookie.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         namespace = simple_cookie[self.key]
         for key, value in self.dict.items():
             if key in {"key", "value"}:
                 continue
             if value is not None:
                 updated_key = key
-                if key == "max_age":
+                if updated_key == "max_age":
                     updated_key = "max-age"
                 namespace[updated_key] = value
 
         return simple_cookie
 
     def to_header(self, **kwargs: Any) -> str:
         """Return a string representation suitable to be sent as HTTP headers.
```

### Comparing `litestar-2.0.0b2/litestar/datastructures/headers.py` & `litestar-2.0.0b3/litestar/datastructures/headers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 import re
 from abc import ABC, abstractmethod
 from contextlib import suppress
 from copy import copy
+from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Dict,
     Iterable,
     Iterator,
     List,
     Mapping,
     MutableMapping,
     Optional,
+    Pattern,
     Tuple,
     Union,
     cast,
 )
 
 from multidict import CIMultiDict, CIMultiDictProxy, MultiMapping
-from pydantic import BaseModel, Extra, Field, ValidationError, validator
-from typing_extensions import Annotated
+from typing_extensions import get_type_hints
 
 from litestar._multipart import parse_content_header
 from litestar._parsers import parse_headers
 from litestar.datastructures.multi_dicts import MultiMixin
-from litestar.exceptions import ImproperlyConfiguredException
+from litestar.dto._utils import resolve_model_type
+from litestar.exceptions import ImproperlyConfiguredException, ValidationException
 
 __all__ = ("Accept", "CacheControlHeader", "ETag", "Header", "Headers", "MutableScopeHeaders")
 
+from litestar.typing import FieldDefinition
+from litestar.utils.dataclass import simple_asdict
 
 if TYPE_CHECKING:
     from litestar.types.asgi_types import (
         HeaderScope,
         Message,
         RawHeaders,
         RawHeadersList,
     )
 
 ETAG_RE = re.compile(r'([Ww]/)?"(.+)"')
+PRINTABLE_ASCII_RE: Pattern[str] = re.compile(r"^[ -~]+$")
 
 
 def _encode_headers(headers: Iterable[Tuple[str, str]]) -> "RawHeadersList":
     return [(key.lower().encode("latin-1"), value.encode("latin-1")) for key, value in headers]
 
 
 class Headers(CIMultiDictProxy[str], MultiMixin[str]):
@@ -87,20 +92,17 @@
     def to_header_list(self) -> "RawHeadersList":
         """Raw header value.
 
         Returns:
             A list of tuples contain the header and header-value as bytes
         """
         # Since ``Headers`` are immutable, this can be cached
-        header_list = self._header_list
-        if not header_list:
-            header_list = self._header_list = _encode_headers(
-                (key, value) for key in set(self) for value in self.getall(key)
-            )
-        return header_list
+        if not self._header_list:
+            self._header_list = _encode_headers((key, value) for key in set(self) for value in self.getall(key))
+        return self._header_list
 
 
 class MutableScopeHeaders(MutableMapping):
     """A case-insensitive, multidict-like structure that can be used to mutate headers within a
     :class:`Scope <.types.Scope>`
     """
 
@@ -208,21 +210,20 @@
         name = key.lower()
         return [i for i, (name_, _) in enumerate(self.headers) if name_.decode("latin-1").lower() == name]
 
     def __setitem__(self, key: str, value: str) -> None:
         """Set a header in the scope, overwriting duplicates."""
         name_encoded = key.lower().encode("latin-1")
         value_encoded = value.encode("latin-1")
-        indices = self._find_indices(key)
-        if not indices:
-            self.headers.append((name_encoded, value_encoded))
-        else:
+        if indices := self._find_indices(key):
             for i in indices[1:]:
                 del self.headers[i]
             self.headers[indices[0]] = (name_encoded, value_encoded)
+        else:
+            self.headers.append((name_encoded, value_encoded))
 
     def __delitem__(self, key: str) -> None:
         """Delete all headers matching ``name``"""
         indices = self._find_indices(key)
         for i in indices[::-1]:
             del self.headers[i]
 
@@ -231,28 +232,20 @@
         return len(self.headers)
 
     def __iter__(self) -> Iterator[str]:
         """Create an iterator of header names including duplicates."""
         return iter(h[0].decode("latin-1") for h in self.headers)
 
 
-class Header(BaseModel, ABC):
+@dataclass
+class Header(ABC):
     """An abstract type for HTTP headers."""
 
     HEADER_NAME: ClassVar[str] = ""
 
-    class Config:
-        allow_population_by_field_name = True
-        extra = Extra.forbid
-
-        @classmethod
-        def alias_generator(cls, field_name: str) -> str:
-            """Generate field-aliases by replacing dashes with underscores in header-names."""
-            return field_name.replace("_", "-")
-
     documentation_only: bool = False
     """Defines the header instance as for OpenAPI documentation purpose only."""
 
     @abstractmethod
     def _get_header_value(self) -> str:
         """Get the header value as string."""
         raise NotImplementedError
@@ -273,14 +266,15 @@
 
         if not self.HEADER_NAME:
             raise ImproperlyConfiguredException("Missing header name")
 
         return (f"{self.HEADER_NAME}: " if include_header_name else "") + self._get_header_value()
 
 
+@dataclass
 class CacheControlHeader(Header):
     """A ``cache-control`` header."""
 
     HEADER_NAME: ClassVar[str] = "cache-control"
 
     max_age: Optional[int] = None
     """Accessor for the ``max-age`` directive."""
@@ -303,23 +297,23 @@
     must_understand: Optional[bool] = None
     """Accessor for the ``must-understand`` directive."""
     immutable: Optional[bool] = None
     """Accessor for the ``immutable`` directive."""
     stale_while_revalidate: Optional[int] = None
     """Accessor for the ``stale-while-revalidate`` directive."""
 
+    _field_definitions: ClassVar[Optional[Dict[str, FieldDefinition]]] = None
+
     def _get_header_value(self) -> str:
         """Get the header value as string."""
 
-        cc_items = []
-        for key, value in self.dict(
-            exclude_unset=True, exclude_none=True, by_alias=True, exclude={"documentation_only"}
-        ).items():
-            cc_items.append(key if isinstance(value, bool) else f"{key}={value}")
-
+        cc_items = [
+            key.replace("_", "-") if isinstance(value, bool) else f"{key.replace('_', '-')}={value}"
+            for key, value in simple_asdict(self, exclude_none=True, exclude={"documentation_only"}).items()
+        ]
         return ", ".join(cc_items)
 
     @classmethod
     def from_header(cls, header_value: str) -> "CacheControlHeader":
         """Create a ``CacheControlHeader`` instance from the header value.
 
         Args:
@@ -327,72 +321,113 @@
 
         Returns:
             An instance of ``CacheControlHeader``
         """
 
         cc_items = [v.strip() for v in header_value.split(",")]
         kwargs: Dict[str, Any] = {}
+        field_definitions = cls._get_field_definitions()
         for cc_item in cc_items:
             key_value = cc_item.split("=")
+            key_value[0] = key_value[0].replace("-", "_")
             if len(key_value) == 1:
                 kwargs[key_value[0]] = True
             elif len(key_value) == 2:
-                kwargs[key_value[0]] = key_value[1]
+                key, value = key_value
+                if key not in field_definitions:
+                    raise ImproperlyConfiguredException("Invalid cache-control header")
+                kwargs[key] = cls._convert_to_type(value, field_definition=field_definitions[key])
             else:
                 raise ImproperlyConfiguredException("Invalid cache-control header value")
 
         try:
             return CacheControlHeader(**kwargs)
-        except ValidationError as exc:
+        except TypeError as exc:
             raise ImproperlyConfiguredException from exc
 
     @classmethod
     def prevent_storing(cls) -> "CacheControlHeader":
         """Create a ``cache-control`` header with the ``no-store`` directive which indicates that any caches of any kind
         (private or shared) should not store this response.
         """
 
         return cls(no_store=True)
 
+    @classmethod
+    def _get_field_definitions(cls) -> Dict[str, FieldDefinition]:
+        """Get the type annotations for the ``CacheControlHeader`` class properties.
+
+        This is needed due to the conversion from pydantic models to dataclasses. Dataclasses do not support
+        automatic conversion of types like pydantic models do.
+
+        Returns:
+            A dictionary of type annotations
 
+        """
+
+        if cls._field_definitions is None:
+            cls._field_definitions = {}
+            for key, value in get_type_hints(cls, include_extras=True).items():
+                definition = FieldDefinition.from_kwarg(annotation=value, name=key)
+                # resolve_model_type so that field_definition.raw has the real raw type e.g. <class 'bool'>
+                cls._field_definitions[key] = resolve_model_type(definition)
+        return cls._field_definitions
+
+    @classmethod
+    def _convert_to_type(cls, value: str, field_definition: FieldDefinition) -> Any:
+        """Convert the value to the expected type.
+
+        Args:
+            value: the value of the cache-control directive
+            field_definition: the field definition for the value to convert
+
+        Returns:
+            The value converted to the expected type
+        """
+        # bool values shouldn't be initiated since they should have been caught earlier in the from_header method and
+        # set with a value of True
+        expected_type = field_definition.raw
+        if expected_type is bool:
+            raise ImproperlyConfiguredException("Invalid cache-control header value")
+        return expected_type(value)
+
+
+@dataclass
 class ETag(Header):
     """An ``etag`` header."""
 
     HEADER_NAME: ClassVar[str] = "etag"
 
     weak: bool = False
-    value: Annotated[Optional[str], Field(regex=r"^[ -~]+$")] = None  # only ASCII characters
+    value: Optional[str] = None  # only ASCII characters
 
     def _get_header_value(self) -> str:
         value = f'"{self.value}"'
-        if self.weak:
-            return f"W/{value}"
-        return value
+        return f"W/{value}" if self.weak else value
 
     @classmethod
     def from_header(cls, header_value: str) -> "ETag":
         """Construct an ``etag`` header from its string representation.
 
         Note that this will unquote etag-values
         """
         match = ETAG_RE.match(header_value)
         if not match:
             raise ImproperlyConfiguredException
         weak, value = match.group(1, 2)
         try:
             return cls(weak=bool(weak), value=value)
-        except ValidationError as exc:
+        except ValueError as exc:
             raise ImproperlyConfiguredException from exc
 
-    @validator("value", always=True)
-    def validate_value(cls, value: Any, values: Dict[str, Any]) -> Any:
-        """Ensure that either value is set or the instance is for ``documentation_only``."""
-        if values.get("documentation_only") or value is not None:
-            return value
-        raise ValueError("value must be set if documentation_only is false")
+    def __post_init__(self) -> None:
+        if self.documentation_only is False and self.value is None:
+            raise ValidationException("value must be set if documentation_only is false")
+        if self.value and not PRINTABLE_ASCII_RE.fullmatch(self.value):
+            raise ValidationException("value must only contain ASCII printable characters")
 
 
 class MediaTypeHeader:
     """A helper class for ``Accept`` header parsing."""
 
     __slots__ = ("maintype", "subtype", "params", "_params_str")
 
@@ -425,29 +460,20 @@
             specificity = 2
         else:
             specificity = 3
 
         return quality, specificity
 
     def match(self, other: "MediaTypeHeader") -> bool:
-        # Check parameters first, ignore the weight parameter 'q'.
-        # Additional parameters on other are also ignored.
-        for key, value in self.params.items():
-            if key != "q" and value != other.params.get(key):
-                return False
-
-        # Then check if the subtypes match, ignoring the wildcard '*'
-        if self.subtype != "*" and other.subtype != "*" and self.subtype != other.subtype:
-            return False
-
-        # Lastly check the main type, also ignoring the wildcard '*'
-        if self.maintype != "*" and other.maintype != "*" and self.maintype != other.maintype:
-            return False
-
-        return True
+        return next(
+            (False for key, value in self.params.items() if key != "q" and value != other.params.get(key)),
+            False
+            if self.subtype != "*" and other.subtype != "*" and self.subtype != other.subtype
+            else self.maintype == "*" or other.maintype == "*" or self.maintype == other.maintype,
+        )
 
 
 class Accept:
     """An ``Accept`` header."""
 
     __slots__ = ("_accepted_types",)
```

### Comparing `litestar-2.0.0b2/litestar/datastructures/multi_dicts.py` & `litestar-2.0.0b3/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/datastructures/response_header.py` & `litestar-2.0.0b3/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/datastructures/state.py` & `litestar-2.0.0b3/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/datastructures/upload_file.py` & `litestar-2.0.0b3/litestar/datastructures/upload_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 from __future__ import annotations
 
 from tempfile import SpooledTemporaryFile
-from typing import TYPE_CHECKING, Any
 
 from anyio.to_thread import run_sync
 
 from litestar.constants import ONE_MEGABYTE
-from litestar.openapi.spec.enums import OpenAPIType
 
 __all__ = ("UploadFile",)
 
 
-if TYPE_CHECKING:
-    from pydantic.fields import ModelField
-
-
 class UploadFile:
     """Representation of a file upload"""
 
     __slots__ = ("filename", "file", "content_type", "headers")
 
     def __init__(
         self,
@@ -102,21 +96,7 @@
         """
         if self.rolled_to_disk:
             return await run_sync(self.file.close)
         return self.file.close()
 
     def __repr__(self) -> str:
         return f"{self.filename} - {self.content_type}"
-
-    @classmethod
-    def __modify_schema__(cls, field_schema: dict[str, Any], field: ModelField | None) -> None:
-        """Create a pydantic JSON schema.
-
-        Args:
-            field_schema: The schema being generated for the field.
-            field: the model class field.
-
-        Returns:
-            None
-        """
-        if field:
-            field_schema.update({"type": OpenAPIType.STRING.value, "contentMediaType": "application/octet-stream"})
```

### Comparing `litestar-2.0.0b2/litestar/datastructures/url.py` & `litestar-2.0.0b3/litestar/datastructures/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,21 +169,23 @@
             A URL
         """
         scheme = scope.get("scheme", "http")
         server = scope.get("server")
         path = scope.get("root_path", "") + scope["path"]
         query_string = scope.get("query_string", b"")
 
-        # # we use iteration here because it's faster, and headers might not yet be cached
-        # # in the scope
-        host = ""
-        for header_name, header_value in scope.get("headers", []):
-            if header_name == b"host":
-                host = header_value.decode("latin-1")
-                break
+        # we use iteration here because it's faster, and headers might not yet be cached
+        host = next(
+            (
+                header_value.decode("latin-1")
+                for header_name, header_value in scope.get("headers", [])
+                if header_name == b"host"
+            ),
+            "",
+        )
         if server and not host:
             host, port = server
             default_port = _DEFAULT_SCHEME_PORTS[scheme]
             if port != default_port:
                 host = f"{host}:{port}"
 
         return cls.from_components(
```

### Comparing `litestar-2.0.0b2/litestar/di.py` & `litestar-2.0.0b3/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/dto/factory/_backends/abc.py` & `litestar-2.0.0b3/litestar/dto/_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,466 +1,521 @@
-"""DTO backends do the heavy lifting of decoding and validating raw bytes into domain models, and
-back again, to bytes.
-"""
 from __future__ import annotations
 
-import secrets
-from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Final, Generic, TypeVar, cast
-
-from litestar._signature.field import SignatureField
-from litestar.dto.factory import DTOData, Mark
-from litestar.typing import ParsedType
-from litestar.utils.helpers import get_fully_qualified_class_name
+import typing
+from inspect import getmodule
+from typing import TYPE_CHECKING, Collection, Mapping, TypeVar, Union, cast
 
-from .types import (
+from msgspec import UNSET, Struct, UnsetType, defstruct, field
+from typing_extensions import get_origin, get_type_hints
+
+from litestar.dto._types import (
     CollectionType,
     CompositeType,
     MappingType,
     NestedFieldInfo,
     SimpleType,
-    TransferFieldDefinition,
+    TransferType,
     TupleType,
     UnionType,
 )
-from .utils import (
-    RenameStrategies,
-    build_annotation_for_backend,
-    should_exclude_field,
-    should_ignore_field,
-    should_mark_private,
-    transfer_data,
-)
+from litestar.dto.config import DTOConfig
+from litestar.dto.data_structures import DTOData
+from litestar.dto.field import Mark
+from litestar.dto.types import ForType, RenameStrategy
+from litestar.enums import RequestEncodingType
+from litestar.types import Empty
+from litestar.types.builtin_types import NoneType
+from litestar.types.composite_types import TypeEncodersMap
+from litestar.types.protocols import InstantiableCollection
+from litestar.typing import FieldDefinition
+from litestar.utils import find_index
 
 if TYPE_CHECKING:
-    from typing import AbstractSet, Callable, Generator
+    from typing import AbstractSet, Any, Iterable
+
+    from litestar.dto._types import FieldDefinitionsType, TransferDTOFieldDefinition
+    from litestar.dto.data_structures import DTOFieldDefinition
+
+__all__ = (
+    "RenameStrategies",
+    "build_annotation_for_backend",
+    "create_msgspec_field",
+    "create_struct_for_field_definitions",
+    "create_transfer_model_type_annotation",
+    "get_dto_config_from_annotated_type",
+    "get_model_type_hints",
+    "resolve_generic_wrapper_type",
+    "resolve_model_type",
+    "should_exclude_field",
+    "should_ignore_field",
+    "should_mark_private",
+    "transfer_data",
+    "transfer_nested_union_type_data",
+)
+
+T = TypeVar("T")
+StructT = TypeVar("StructT", bound=Struct)
+
 
-    from litestar._openapi.schema_generation import SchemaCreator
-    from litestar.dto.factory import DTOConfig
-    from litestar.dto.factory.data_structures import FieldDefinition
-    from litestar.dto.interface import ConnectionContext
-    from litestar.dto.types import ForType
-    from litestar.openapi.spec import Reference, Schema
-    from litestar.types.serialization import LitestarEncodableType
-
-    from .types import FieldDefinitionsType
-
-__all__ = ("AbstractDTOBackend", "BackendContext")
-
-BackendT = TypeVar("BackendT")
-
-
-class BackendContext:
-    """Context required by DTO backends to perform their work."""
-
-    __slots__ = (
-        "config",
-        "dto_for",
-        "field_definition_generator",
-        "is_nested_field_predicate",
-        "model_type",
-        "parsed_type",
-        "wrapper_attribute_name",
+def get_model_type_hints(model_type: type[Any], namespace: dict[str, Any] | None = None) -> dict[str, FieldDefinition]:
+    """Retrieve type annotations for ``model_type``.
+
+    Args:
+        model_type: Any type-annotated class.
+        namespace: Optional namespace to use for resolving type hints.
+
+    Returns:
+        Parsed type hints for ``model_type`` resolved within the scope of its module.
+    """
+    namespace = namespace or {}
+    namespace.update(vars(typing))
+    namespace.update(
+        {
+            "TypeEncodersMap": TypeEncodersMap,
+            "ForType": ForType,
+            "DTOConfig": DTOConfig,
+            "RenameStrategy": RenameStrategy,
+            "RequestEncodingType": RequestEncodingType,
+        }
     )
 
-    def __init__(
-        self,
-        dto_config: DTOConfig,
-        dto_for: ForType,
-        parsed_type: ParsedType,
-        field_definition_generator: Callable[[Any], Generator[FieldDefinition, None, None]],
-        is_nested_field_predicate: Callable[[ParsedType], bool],
-        model_type: type[Any],
-        wrapper_attribute_name: str | None,
-    ) -> None:
-        """Create a backend context.
+    if model_module := getmodule(model_type):
+        namespace.update(vars(model_module))
 
-        Args:
-            dto_config: DTO config.
-            dto_for: "data" or "return"
-            parsed_type: Parsed type.
-            field_definition_generator: Generator that produces
-                :class:`FieldDefinition <.dto.factory.types.FieldDefinition>` instances given ``model_type``.
-            is_nested_field_predicate: Function that detects if a field is nested.
-            model_type: Model type.
-            wrapper_attribute_name: If the data that DTO should operate upon is wrapped in a generic datastructure, this is the
-                name of the attribute that the data is stored in.
-        """
-        self.config: Final[DTOConfig] = dto_config
-        self.dto_for: Final[ForType] = dto_for
-        self.parsed_type: Final[ParsedType] = parsed_type
-        self.field_definition_generator: Final[
-            Callable[[Any], Generator[FieldDefinition, None, None]]
-        ] = field_definition_generator
-        self.is_nested_field_predicate: Final[Callable[[ParsedType], bool]] = is_nested_field_predicate
-        self.model_type: Final[type[Any]] = model_type
-        self.wrapper_attribute_name = wrapper_attribute_name
-
-
-class NestedDepthExceededError(Exception):
-    """Raised when a nested type exceeds the maximum allowed depth.
-
-    Not an exception that is intended to be raised into userland, rather a signal to the process that is iterating over
-    the field definitions that the current field should be skipped.
+    return {
+        k: FieldDefinition.from_kwarg(annotation=v, name=k)
+        for k, v in get_type_hints(model_type, localns=namespace, include_extras=True).items()
+    }
+
+
+def get_dto_config_from_annotated_type(field_definition: FieldDefinition) -> DTOConfig | None:
+    """Extract data type and config instances from ``Annotated`` annotation.
+
+    Args:
+        field_definition: A parsed type annotation that represents the annotation used to narrow the DTO type.
+
+    Returns:
+        The type and config object extracted from the annotation.
     """
+    if configs := [item for item in field_definition.metadata if isinstance(item, DTOConfig)]:
+        return configs[0]
+    return None
 
 
-class AbstractDTOBackend(ABC, Generic[BackendT]):
-    __slots__ = (
-        "annotation",
-        "context",
-        "dto_data_type",
-        "parsed_field_definitions",
-        "reverse_name_map",
-        "transfer_model_type",
-    )
+def resolve_model_type(field_definition: FieldDefinition) -> FieldDefinition:
+    """Resolve the data model type from a parsed type.
 
-    def __init__(self, context: BackendContext) -> None:
-        """Create dto backend instance.
+    Args:
+        field_definition: A parsed type annotation that represents the annotation used to narrow the DTO type.
 
-        Args:
-            context: context of the type represented by this backend.
-        """
-        self.context = context
-        self.parsed_field_definitions = self.parse_model(context.model_type, context.config.exclude)
-        self.transfer_model_type = self.create_transfer_model_type(
-            get_fully_qualified_class_name(context.model_type), self.parsed_field_definitions
+    Returns:
+        A :class:`FieldDefinition <.typing.FieldDefinition>` that represents the data model type.
+    """
+    if field_definition.is_optional:
+        return resolve_model_type(next(t for t in field_definition.inner_types if not t.is_subclass_of(NoneType)))
+
+    if field_definition.is_subclass_of(DTOData):
+        return resolve_model_type(field_definition.inner_types[0])
+
+    if field_definition.is_collection:
+        if field_definition.is_mapping:
+            return resolve_model_type(field_definition.inner_types[1])
+
+        if field_definition.is_tuple:
+            if any(t is Ellipsis for t in field_definition.args):
+                return resolve_model_type(field_definition.inner_types[0])
+        elif field_definition.is_non_string_collection:
+            return resolve_model_type(field_definition.inner_types[0])
+
+    return field_definition
+
+
+def resolve_generic_wrapper_type(
+    field_definition: FieldDefinition, dto_specialized_type: type[Any]
+) -> tuple[FieldDefinition, FieldDefinition, str] | None:
+    """Handle where DTO supported data is wrapped in a generic container type.
+
+    Args:
+        field_definition: A parsed type annotation that represents the annotation used to narrow the DTO type.
+        dto_specialized_type: The type used to specialize the DTO.
+
+    Returns:
+        The data model type.
+    """
+    if (origin := field_definition.origin) and (parameters := getattr(origin, "__parameters__", None)):
+        param_index = find_index(
+            field_definition.inner_types, lambda x: resolve_model_type(x).is_subclass_of(dto_specialized_type)
         )
-        self.dto_data_type: type[DTOData] | None = None
-        if context.parsed_type.is_subclass_of(DTOData):
-            self.dto_data_type = context.parsed_type.annotation
-            annotation = self.context.parsed_type.inner_types[0].annotation
-        else:
-            annotation = context.parsed_type.annotation
-        self.annotation = build_annotation_for_backend(annotation, self.transfer_model_type)
 
-    def parse_model(self, model_type: Any, exclude: AbstractSet[str], nested_depth: int = 0) -> FieldDefinitionsType:
-        """Reduce :attr:`model_type` to :class:`FieldDefinitionsType`.
+        if param_index == -1:
+            return None
 
-        .. important::
-            Implementations must respect the :attr:`config` object. For example:
-                - fields marked private must never be included in the field definitions.
-                - if a ``purpose`` is declared, then read-only fields must be taken into account.
-                - field renaming must be implemented.
-                - additional fields must be included, subject to ``purpose``.
-                - nested depth and nested recursion depth must be adhered to.
+        inner_type = field_definition.inner_types[param_index]
+        model_type = resolve_model_type(inner_type)
+        type_var = parameters[param_index]
 
-        Returns:
-            Fields for data transfer.
+        for attr, attr_type in get_model_type_hints(origin).items():
+            if attr_type.annotation is type_var or any(t.annotation is type_var for t in attr_type.inner_types):
+                if attr_type.is_non_string_collection:
+                    # the inner type of the collection type is the type var, so we need to specialize the
+                    # collection type with the DTO supported type.
+                    specialized_annotation = attr_type.safe_generic_origin[model_type.annotation]
+                    return model_type, FieldDefinition.from_annotation(specialized_annotation), attr
+                return model_type, inner_type, attr
 
-            Key is the name of the new field, and value is a tuple of type and default value pairs.
+    return None
 
-            Add a new field called "new_field", that is a string, and required:
-            {"new_field": (str, ...)}
 
-            Add a new field called "new_field", that is a string, and not-required:
-            {"new_field": (str, "default")}
+def build_annotation_for_backend(annotation: Any, model: type[T]) -> type[T] | type[Iterable[T]]:
+    """A helper to re-build a generic outer type with new inner type.
 
-            Add a new field called "new_field", that may be `None`:
-            {"new_field": (str | None, None)}
-        """
-        defined_fields = []
-        for field_definition in self.context.field_definition_generator(model_type):
-            if should_ignore_field(field_definition, self.context.dto_for):
-                continue
-
-            if should_mark_private(field_definition, self.context.config.underscore_fields_private):
-                field_definition.dto_field.mark = Mark.PRIVATE
-
-            try:
-                transfer_type = self._create_transfer_type(
-                    field_definition.parsed_type,
-                    exclude,
-                    field_definition.name,
-                    field_definition.unique_name(),
-                    nested_depth,
-                )
-            except NestedDepthExceededError:
-                continue
-
-            if rename := self.context.config.rename_fields.get(field_definition.name):
-                serialization_name = rename
-            elif self.context.config.rename_strategy:
-                serialization_name = RenameStrategies(self.context.config.rename_strategy)(field_definition.name)
-            else:
-                serialization_name = field_definition.name
-
-            transfer_field_definition = TransferFieldDefinition.from_field_definition(
-                field_definition=field_definition,
-                serialization_name=serialization_name,
-                transfer_type=transfer_type,
-                is_partial=self.context.config.partial,
-                is_excluded=should_exclude_field(field_definition, exclude, self.context.dto_for),
-            )
-            defined_fields.append(transfer_field_definition)
-        return tuple(defined_fields)
+    Args:
+        annotation: The original annotation on the handler signature
+        model: The data container type
 
-    @abstractmethod
-    def create_transfer_model_type(self, unique_name: str, field_definitions: FieldDefinitionsType) -> type[BackendT]:
-        """Create a model for data transfer.
+    Returns:
+        Annotation with new inner type if applicable.
+    """
+    origin = get_origin(annotation)
+    if not origin:
+        return model
+    try:
+        return origin[model]  # type:ignore[no-any-return]
+    except TypeError:  # pragma: no cover
+        return annotation.copy_with((model,))  # type:ignore[no-any-return]
+
+
+def should_mark_private(field_definition: DTOFieldDefinition, underscore_fields_private: bool) -> bool:
+    """Returns ``True`` where a field should be marked as private.
+
+    Fields should be marked as private when:
+    - the ``underscore_fields_private`` flag is set.
+    - the field is not already marked.
+    - the field name is prefixed with an underscore
+
+    Args:
+        field_definition: defined DTO field
+        underscore_fields_private: whether fields prefixed with an underscore should be marked as private.
+    """
+    return bool(
+        underscore_fields_private and field_definition.dto_field.mark is None and field_definition.name.startswith("_")
+    )
 
-        Args:
-            unique_name: name for the type that should be unique across all transfer types.
-            field_definitions: field definitions for the container type.
 
-        Returns:
-            A ``BackendT`` class.
-        """
+def should_exclude_field(
+    field_definition: DTOFieldDefinition, exclude: AbstractSet[str], include: AbstractSet[str], dto_for: ForType
+) -> bool:
+    """Returns ``True`` where a field should be excluded from data transfer.
+
+    Args:
+        field_definition: defined DTO field
+        exclude: names of fields to exclude
+        include: names of fields to exclude
+        dto_for: indicates whether the DTO is for the request body or response.
 
-    @abstractmethod
-    def parse_raw(self, raw: bytes, connection_context: ConnectionContext) -> Any:
-        """Parse raw bytes into transfer model type.
+    Returns:
+        ``True`` if the field should not be included in any data transfer.
+    """
+    field_name = field_definition.name
+    if field_name in exclude:
+        return True
+    if include and field_name not in include and not (any(f.startswith(f"{field_name}.") for f in include)):
+        return True
+    if field_definition.dto_field.mark is Mark.PRIVATE:
+        return True
+    if dto_for == "data" and field_definition.dto_field.mark is Mark.READ_ONLY:
+        return True
+    return dto_for == "return" and field_definition.dto_field.mark is Mark.WRITE_ONLY
+
+
+def should_ignore_field(field_definition: DTOFieldDefinition, dto_for: ForType) -> bool:
+    """Returns ``True`` where a field should be ignored.
 
-        Args:
-            raw: bytes
-            connection_context: Information about the active connection.
+    An ignored field is different to an excluded one in that we do not produce a
+    ``TransferFieldDefinition`` for it at all.
 
-        Returns:
-            The raw bytes parsed into transfer model type.
-        """
+    This allows ``AbstractDTOFactory`` concrete types to generate multiple field definitions
+    for the same field name, each for a different transfer direction.
 
-    @abstractmethod
-    def parse_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
-        """Parse builtin types into transfer model type.
+    One example of this is the :class:`sqlalchemy.ext.hybrid.hybrid_property` which, might have
+    a different type accepted by its setter method, than is returned by its getter method.
+    """
+    return field_definition.dto_for is not None and field_definition.dto_for != dto_for
 
-        Args:
-            builtins: Builtin type.
-            connection_context: Information about the active connection.
 
-        Returns:
-            The builtin type parsed into transfer model type.
-        """
+class RenameStrategies:
+    """Useful renaming strategies than be used with :class:`DTOConfig`"""
 
-    def populate_data_from_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
-        """Populate model instance from builtin types.
+    def __init__(self, renaming_strategy: RenameStrategy) -> None:
+        self.renaming_strategy = renaming_strategy
 
-        Args:
-            builtins: Builtin type.
-            connection_context: Information about the active connection.
+    def __call__(self, field_name: str) -> str:
+        if not isinstance(self.renaming_strategy, str):
+            return self.renaming_strategy(field_name)
 
-        Returns:
-            Instance or collection of ``model_type`` instances.
-        """
-        if self.dto_data_type:
-            return self.dto_data_type(
-                backend=self,
-                data_as_builtins=transfer_data(
-                    dict,
-                    self.parse_builtins(builtins, connection_context),
-                    self.parsed_field_definitions,
-                    "data",
-                    self.context.parsed_type,
-                ),
-            )
-        return self.transfer_data_from_builtins(self.parse_builtins(builtins, connection_context))
+        return cast(str, getattr(self, self.renaming_strategy)(field_name))
 
-    def transfer_data_from_builtins(self, builtins: Any) -> Any:
-        """Populate model instance from builtin types.
+    @staticmethod
+    def upper(field_name: str) -> str:
+        return field_name.upper()
 
-        Args:
-            builtins: Builtin type.
+    @staticmethod
+    def lower(field_name: str) -> str:
+        return field_name.lower()
 
-        Returns:
-            Instance or collection of ``model_type`` instances.
-        """
-        return transfer_data(
-            self.context.model_type, builtins, self.parsed_field_definitions, "data", self.context.parsed_type
-        )
+    @staticmethod
+    def camel(field_name: str) -> str:
+        return RenameStrategies._camelize(field_name)
 
-    def populate_data_from_raw(self, raw: bytes, connection_context: ConnectionContext) -> Any:
-        """Parse raw bytes into instance of `model_type`.
+    @staticmethod
+    def pascal(field_name: str) -> str:
+        return RenameStrategies._camelize(field_name, capitalize_first_letter=True)
 
-        Args:
-            raw: bytes
-            connection_context: Information about the active connection.
+    @staticmethod
+    def _camelize(string: str, capitalize_first_letter: bool = False) -> str:
+        """Convert a string to camel case.
 
+        Args:
+            string (str): The string to convert
+            capitalize_first_letter (bool): Default is False, a True value will convert to PascalCase
         Returns:
-            Instance or collection of ``model_type`` instances.
+            str: The string converted to camel case or Pascal case
         """
-        if self.dto_data_type:
-            return self.dto_data_type(
-                backend=self,
-                data_as_builtins=transfer_data(
-                    dict,
-                    self.parse_raw(raw, connection_context),
-                    self.parsed_field_definitions,
-                    "data",
-                    self.context.parsed_type,
-                ),
-            )
-        return transfer_data(
-            self.context.model_type,
-            self.parse_raw(raw, connection_context),
-            self.parsed_field_definitions,
-            "data",
-            self.context.parsed_type,
+        return "".join(
+            word if index == 0 and not capitalize_first_letter else word.capitalize()
+            for index, word in enumerate(string.split("_"))
         )
 
-    def encode_data(self, data: Any, connection_context: ConnectionContext) -> LitestarEncodableType:
-        """Encode data into a ``LitestarEncodableType``.
 
-        Args:
-            data: Data to encode.
-            connection_context: Information about the active connection.
+def transfer_data(
+    destination_type: type[T],
+    source_data: Any | Collection[Any],
+    field_definitions: FieldDefinitionsType,
+    dto_for: ForType,
+    field_definition: FieldDefinition,
+) -> T | InstantiableCollection[T]:
+    """Create instance or iterable of instances of ``destination_type``.
+
+    Args:
+        destination_type: the model type received by the DTO on type narrowing.
+        source_data: data that has been parsed and validated via the backend.
+        field_definitions: model field definitions.
+        dto_for: indicates whether the DTO is for the request body or response.
+        field_definition: the parsed type that represents the handler annotation for which the DTO is being applied.
 
-        Returns:
-            Encoded data.
-        """
-        if self.context.wrapper_attribute_name:
-            setattr(
-                data,
-                self.context.wrapper_attribute_name,
-                transfer_data(
-                    destination_type=self.transfer_model_type,
-                    source_data=getattr(data, self.context.wrapper_attribute_name),
-                    field_definitions=self.parsed_field_definitions,
-                    dto_for="return",
-                    parsed_type=self.context.parsed_type,
-                ),
+    Returns:
+        Data parsed into ``destination_type``.
+    """
+    if field_definition.is_non_string_collection and not field_definition.is_mapping:
+        origin = field_definition.instantiable_origin
+        if not issubclass(origin, InstantiableCollection):  # pragma: no cover
+            raise RuntimeError(
+                f"Unexpected origin type '{field_definition.instantiable_origin}', expected collection type"
             )
-            # cast() here because we take for granted that whatever ``data`` is, it must be something
-            # that litestar can natively encode.
-            return cast("LitestarEncodableType", data)
-
-        return transfer_data(
-            destination_type=self.transfer_model_type,  # type: ignore[arg-type]
-            source_data=data,
-            field_definitions=self.parsed_field_definitions,
-            dto_for="return",
-            parsed_type=self.context.parsed_type,
-        )
 
-    def create_openapi_schema(self, schema_creator: SchemaCreator) -> Reference | Schema:
-        """Create a RequestBody model for the given RouteHandler or return None."""
-        return schema_creator.for_field(SignatureField.create(self.annotation))
-
-    def _create_transfer_type(
-        self, parsed_type: ParsedType, exclude: AbstractSet[str], field_name: str, unique_name: str, nested_depth: int
-    ) -> CompositeType | SimpleType:
-        exclude = _filter_exclude(exclude, field_name)
-
-        if parsed_type.is_union:
-            return self._create_union_type(parsed_type, exclude, unique_name, nested_depth)
-
-        if parsed_type.is_tuple:
-            if len(parsed_type.inner_types) == 2 and parsed_type.inner_types[1].annotation is Ellipsis:
-                return self._create_collection_type(parsed_type, exclude, unique_name, nested_depth)
-            return self._create_tuple_type(parsed_type, exclude, unique_name, nested_depth)
-
-        if parsed_type.is_mapping:
-            return self._create_mapping_type(parsed_type, exclude, unique_name, nested_depth)
-
-        if parsed_type.is_non_string_collection:
-            return self._create_collection_type(parsed_type, exclude, unique_name, nested_depth)
-
-        transfer_model: NestedFieldInfo | None = None
-        if self.context.is_nested_field_predicate(parsed_type):
-            if nested_depth == self.context.config.max_nested_depth:
-                raise NestedDepthExceededError()
-
-            nested_field_definitions = self.parse_model(parsed_type.annotation, exclude, nested_depth + 1)
-            transfer_model = NestedFieldInfo(
-                model=self.create_transfer_model_type(unique_name, nested_field_definitions),
-                field_definitions=nested_field_definitions,
-            )
+        return origin(  # type:ignore[no-any-return]
+            transfer_data(destination_type, item, field_definitions, dto_for, field_definition.inner_types[0])
+            for item in source_data
+        )
+    return transfer_instance_data(destination_type, source_data, field_definitions, dto_for)
+
+
+def transfer_instance_data(
+    destination_type: type[T], source_instance: Any, field_definitions: FieldDefinitionsType, dto_for: ForType
+) -> T:
+    """Create instance of ``destination_type`` with data from ``source_instance``.
+
+    Args:
+        destination_type: the model type received by the DTO on type narrowing.
+        source_instance: primitive data that has been parsed and validated via the backend.
+        field_definitions: model field definitions.
+        dto_for: indicates whether the DTO is for the request body or response.
 
-        return SimpleType(parsed_type, nested_field_info=transfer_model)
+    Returns:
+        Data parsed into ``model_type``.
+    """
+    unstructured_data = {}
+    source_is_mapping = isinstance(source_instance, Mapping)
 
-    def _create_collection_type(
-        self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
-    ) -> CollectionType:
-        inner_types = parsed_type.inner_types
-        inner_type = self._create_transfer_type(
-            parsed_type=ParsedType(Any) if not inner_types else inner_types[0],
-            exclude=exclude,
-            field_name="0",
-            unique_name=_enumerate_name(unique_name, 0),
-            nested_depth=nested_depth,
-        )
-        return CollectionType(
-            parsed_type=parsed_type, inner_type=inner_type, has_nested=_determine_has_nested(inner_type)
-        )
+    def has(source: Any, key: str) -> bool:
+        return key in source if source_is_mapping else hasattr(source, key)
 
-    def _create_mapping_type(
-        self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
-    ) -> MappingType:
-        inner_types = parsed_type.inner_types
-        key_type = self._create_transfer_type(
-            parsed_type=ParsedType(Any) if not inner_types else inner_types[0],
-            exclude=exclude,
-            field_name="0",
-            unique_name=_enumerate_name(unique_name, 0),
-            nested_depth=nested_depth,
-        )
-        value_type = self._create_transfer_type(
-            parsed_type=ParsedType(Any) if not inner_types else inner_types[1],
-            exclude=exclude,
-            field_name="1",
-            unique_name=_enumerate_name(unique_name, 1),
-            nested_depth=nested_depth,
-        )
-        return MappingType(
-            parsed_type=parsed_type,
-            key_type=key_type,
-            value_type=value_type,
-            has_nested=_determine_has_nested(key_type) or _determine_has_nested(value_type),
+    def get(source: Any, key: str) -> Any:
+        return source[key] if source_is_mapping else getattr(source, key)
+
+    def filter_missing(value: Any) -> bool:
+        return value is UNSET
+
+    for field_definition in field_definitions:
+        source_name = field_definition.serialization_name if dto_for == "data" else field_definition.name
+
+        if should_skip_transfer(dto_for, field_definition, has(source_instance, source_name)):
+            continue
+
+        transfer_type = field_definition.transfer_type
+        destination_name = field_definition.name if dto_for == "data" else field_definition.serialization_name
+        source_value = get(source_instance, source_name)
+
+        if field_definition.is_partial and dto_for == "data" and filter_missing(source_value):
+            continue
+
+        unstructured_data[destination_name] = transfer_type_data(
+            source_value, transfer_type, dto_for, nested_as_dict=destination_type is dict
         )
+    return destination_type(**unstructured_data)
+
+
+def should_skip_transfer(
+    dto_for: ForType,
+    field_definition: TransferDTOFieldDefinition,
+    source_has_value: bool,
+) -> bool:
+    """Returns ``True`` where a field should be excluded from data transfer.
 
-    def _create_tuple_type(
-        self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
-    ) -> TupleType:
-        inner_types = tuple(
-            self._create_transfer_type(
-                parsed_type=inner_type,
-                exclude=exclude,
-                field_name=str(i),
-                unique_name=_enumerate_name(unique_name, i),
-                nested_depth=nested_depth,
+    We should skip transfer when:
+    - the field is excluded and the DTO is for the return data.
+    - the DTO is for request data, and the field is not in the source instance.
+
+    Args:
+        dto_for: indicates whether the DTO is for the request body or response.
+        field_definition: model field definition.
+        source_has_value: indicates whether the source instance has a value for the field.
+    """
+    return (dto_for == "return" and field_definition.is_excluded) or (dto_for == "data" and not source_has_value)
+
+
+def transfer_type_data(
+    source_value: Any, transfer_type: TransferType, dto_for: ForType, nested_as_dict: bool = False
+) -> Any:
+    if isinstance(transfer_type, SimpleType) and transfer_type.nested_field_info:
+        if nested_as_dict:
+            dest_type = dict
+        else:
+            dest_type = (
+                transfer_type.field_definition.annotation
+                if dto_for == "data"
+                else transfer_type.nested_field_info.model
             )
-            for i, inner_type in enumerate(parsed_type.inner_types)
-        )
-        return TupleType(
-            parsed_type=parsed_type,
-            inner_types=inner_types,
-            has_nested=any(_determine_has_nested(t) for t in inner_types),
-        )
 
-    def _create_union_type(
-        self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
-    ) -> UnionType:
-        inner_types = tuple(
-            self._create_transfer_type(
-                parsed_type=inner_type,
-                exclude=exclude,
-                field_name=str(i),
-                unique_name=_enumerate_name(unique_name, i),
-                nested_depth=nested_depth,
+        return transfer_nested_simple_type_data(dest_type, transfer_type.nested_field_info, dto_for, source_value)
+    if isinstance(transfer_type, UnionType) and transfer_type.has_nested:
+        return transfer_nested_union_type_data(transfer_type, dto_for, source_value)
+    if isinstance(transfer_type, CollectionType):
+        if transfer_type.has_nested:
+            return transfer_nested_collection_type_data(
+                transfer_type.field_definition.instantiable_origin, transfer_type, dto_for, source_value
             )
-            for i, inner_type in enumerate(parsed_type.inner_types)
-        )
-        return UnionType(
-            parsed_type=parsed_type,
-            inner_types=inner_types,
-            has_nested=any(_determine_has_nested(t) for t in inner_types),
-        )
+        return transfer_type.field_definition.instantiable_origin(source_value)
+    return source_value
 
-    def _gen_unique_name_id(self, unique_name: str, size: int = 12) -> str:
-        # Generate a unique ID
-        # Convert the ID to a short alphanumeric string
-        return f"{unique_name}-{secrets.token_hex(8)}"
 
+def transfer_nested_collection_type_data(
+    origin_type: type[Any], transfer_type: CollectionType, dto_for: ForType, source_value: Any
+) -> Any:
+    return origin_type(transfer_type_data(item, transfer_type.inner_type, dto_for) for item in source_value)
+
+
+def transfer_nested_simple_type_data(
+    destination_type: type[T],  # pyright: ignore
+    nested_field_info: NestedFieldInfo,
+    dto_for: ForType,
+    source_value: Any,
+) -> Any:
+    return transfer_instance_data(destination_type, source_value, nested_field_info.field_definitions, dto_for)
+
+
+def transfer_nested_union_type_data(transfer_type: UnionType, dto_for: ForType, source_value: Any) -> Any:
+    for inner_type in transfer_type.inner_types:
+        if isinstance(inner_type, CompositeType):
+            raise RuntimeError("Composite inner types not (yet) supported for nested unions.")
+
+        if inner_type.nested_field_info and isinstance(
+            source_value,
+            inner_type.nested_field_info.model if dto_for == "data" else inner_type.field_definition.annotation,
+        ):
+            return transfer_instance_data(
+                inner_type.field_definition.annotation if dto_for == "data" else inner_type.nested_field_info.model,
+                source_value,
+                inner_type.nested_field_info.field_definitions,
+                dto_for,
+            )
+    return source_value
 
-def _filter_exclude(exclude: AbstractSet[str], field_name: str) -> AbstractSet[str]:
-    """Filter exclude set to only include exclusions for the given field name."""
-    return {split[1] for s in exclude if (split := s.split(".", 1))[0] == field_name and len(split) > 1}
 
+def create_transfer_model_type_annotation(transfer_type: TransferType) -> Any:
+    """Create a type annotation for a transfer model.
 
-def _enumerate_name(name: str, index: int) -> str:
-    """Enumerate ``name`` with ``index``."""
-    return f"{name}_{index}"
+    Uses the parsed type that originates from the data model and the transfer model generated to represent a nested
+    type to reconstruct the type annotation for the transfer model.
+    """
+    if isinstance(transfer_type, SimpleType):
+        if transfer_type.nested_field_info:
+            return transfer_type.nested_field_info.model
+        return transfer_type.field_definition.annotation
 
+    if isinstance(transfer_type, CollectionType):
+        return create_transfer_model_collection_type(transfer_type)
 
-def _determine_has_nested(transfer_type: SimpleType | CompositeType) -> bool:
-    """Determine if a transfer type has nested types."""
-    if isinstance(transfer_type, SimpleType):
-        return bool(transfer_type.nested_field_info)
-    return transfer_type.has_nested
+    if isinstance(transfer_type, MappingType):
+        return create_transfer_model_mapping_type(transfer_type)
+
+    if isinstance(transfer_type, TupleType):
+        return create_transfer_model_tuple_type(transfer_type)
+
+    if isinstance(transfer_type, UnionType):
+        return create_transfer_model_union_type(transfer_type)
+
+    raise RuntimeError(f"Unexpected transfer type: {type(transfer_type)}")
+
+
+def create_transfer_model_collection_type(transfer_type: CollectionType) -> Any:
+    generic_collection_type = transfer_type.field_definition.safe_generic_origin
+    inner_type = create_transfer_model_type_annotation(transfer_type.inner_type)
+    if transfer_type.field_definition.origin is tuple:
+        return generic_collection_type[inner_type, ...]
+    return generic_collection_type[inner_type]
+
+
+def create_transfer_model_tuple_type(transfer_type: TupleType) -> Any:
+    inner_types = tuple(create_transfer_model_type_annotation(t) for t in transfer_type.inner_types)
+    return transfer_type.field_definition.safe_generic_origin[inner_types]
+
+
+def create_transfer_model_union_type(transfer_type: UnionType) -> Any:
+    inner_types = tuple(create_transfer_model_type_annotation(t) for t in transfer_type.inner_types)
+    return transfer_type.field_definition.safe_generic_origin[inner_types]
+
+
+def create_transfer_model_mapping_type(transfer_type: MappingType) -> Any:
+    key_type = create_transfer_model_type_annotation(transfer_type.key_type)
+    value_type = create_transfer_model_type_annotation(transfer_type.value_type)
+    return transfer_type.field_definition.safe_generic_origin[key_type, value_type]
+
+
+def create_msgspec_field(field_definition: TransferDTOFieldDefinition) -> Any:
+    kwargs: dict[str, Any] = {}
+    if field_definition.is_partial:
+        kwargs["default"] = UNSET
+
+    elif field_definition.default is not Empty:
+        kwargs["default"] = field_definition.default
+
+    elif field_definition.default_factory is not None:
+        kwargs["default_factory"] = field_definition.default_factory
+
+    return field(**kwargs)
+
+
+def create_struct_for_field_definitions(model_name: str, field_definitions: FieldDefinitionsType) -> type[Struct]:
+    struct_fields: list[tuple[str, type] | tuple[str, type, type]] = []
+    for field_def in field_definitions:
+        if field_def.is_excluded:
+            continue
+
+        field_name = field_def.serialization_name or field_def.name
+
+        field_type = create_transfer_model_type_annotation(field_def.transfer_type)
+        if field_def.is_partial:
+            field_type = Union[field_type, UnsetType]
+
+        struct_fields.append((field_name, field_type, create_msgspec_field(field_def)))
+    return defstruct(model_name, struct_fields, frozen=True, kw_only=True)
```

### Comparing `litestar-2.0.0b2/litestar/dto/factory/_backends/types.py` & `litestar-2.0.0b3/litestar/dto/_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
-from litestar.dto.factory.data_structures import FieldDefinition
+from litestar.dto.data_structures import DTOFieldDefinition
 
 if TYPE_CHECKING:
     from typing import Any
 
     from typing_extensions import Self, TypeAlias
 
-    from litestar.typing import ParsedType
+    from litestar.typing import FieldDefinition
 
 
 @dataclass(frozen=True)
 class NestedFieldInfo:
     """Type for representing fields and model type of nested model type."""
 
     __slots__ = ("model", "field_definitions")
@@ -23,17 +23,17 @@
     field_definitions: FieldDefinitionsType
 
 
 @dataclass(frozen=True)
 class TransferType:
     """Type for representing model types for data transfer."""
 
-    __slots__ = ("parsed_type",)
+    __slots__ = ("field_definition",)
 
-    parsed_type: ParsedType
+    field_definition: FieldDefinition
 
 
 @dataclass(frozen=True)
 class SimpleType(TransferType):
     """Represents indivisible, non-composite types."""
 
     __slots__ = ("nested_field_info",)
@@ -86,15 +86,15 @@
     __slots__ = ("key_type", "value_type")
 
     key_type: CompositeType | SimpleType
     value_type: CompositeType | SimpleType
 
 
 @dataclass(frozen=True)
-class TransferFieldDefinition(FieldDefinition):
+class TransferDTOFieldDefinition(DTOFieldDefinition):
     __slots__ = (
         "default_factory",
         "dto_field",
         "dto_for",
         "unique_model_name",
         "is_excluded",
         "is_partial",
@@ -109,32 +109,42 @@
     """Name of the field as it should feature on the transfer model."""
     is_partial: bool
     """Whether the field is optional for transfer."""
     is_excluded: bool
     """Whether the field should be excluded from transfer."""
 
     @classmethod
-    def from_field_definition(
+    def from_dto_field_definition(
         cls,
-        field_definition: FieldDefinition,
+        field_definition: DTOFieldDefinition,
         transfer_type: TransferType,
         serialization_name: str,
         is_partial: bool,
         is_excluded: bool,
     ) -> Self:
         return cls(
-            name=field_definition.name,
+            annotation=field_definition.annotation,
+            args=field_definition.args,
             default=field_definition.default,
-            parsed_type=field_definition.parsed_type,
             default_factory=field_definition.default_factory,
-            serialization_name=serialization_name,
-            unique_model_name=field_definition.unique_model_name,
-            transfer_type=transfer_type,
             dto_field=field_definition.dto_field,
-            is_partial=is_partial,
-            is_excluded=is_excluded,
             dto_for=field_definition.dto_for,
+            extra=field_definition.extra,
+            inner_types=field_definition.inner_types,
+            instantiable_origin=field_definition.instantiable_origin,
+            is_excluded=is_excluded,
+            is_partial=is_partial,
+            kwarg_definition=field_definition.kwarg_definition,
+            metadata=field_definition.metadata,
+            name=field_definition.name,
+            origin=field_definition.origin,
+            raw=field_definition.raw,
+            safe_generic_origin=field_definition.safe_generic_origin,
+            serialization_name=serialization_name,
+            transfer_type=transfer_type,
+            type_wrappers=field_definition.type_wrappers,
+            unique_model_name=field_definition.unique_model_name,
         )
 
 
-FieldDefinitionsType: TypeAlias = "tuple[TransferFieldDefinition, ...]"
+FieldDefinitionsType: TypeAlias = "tuple[TransferDTOFieldDefinition, ...]"
 """Generic representation of names and types."""
```

### Comparing `litestar-2.0.0b2/litestar/dto/factory/abc.py` & `litestar-2.0.0b3/litestar/dto/base_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,98 +1,87 @@
 from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
+from abc import abstractmethod
 from typing import TYPE_CHECKING, Generic, TypeVar
 
-from litestar.dto.interface import ConnectionContext, DTOInterface
-from litestar.enums import RequestEncodingType
-from litestar.typing import ParsedType
-
-from ._backends import MsgspecDTOBackend, PydanticDTOBackend
-from ._backends.abc import BackendContext
-from .config import DTOConfig
-from .exc import InvalidAnnotation
-from .utils import (
-    parse_configs_from_annotation,
+from litestar.dto._backend import BackendContext, DTOBackend
+from litestar.dto._utils import (
+    get_dto_config_from_annotated_type,
     resolve_generic_wrapper_type,
     resolve_model_type,
 )
+from litestar.dto.config import DTOConfig
+from litestar.dto.interface import ConnectionContext, DTOInterface
+from litestar.exceptions.dto_exceptions import InvalidAnnotationException
+from litestar.typing import FieldDefinition
 
 if TYPE_CHECKING:
     from typing import Any, ClassVar, Collection, Generator
 
     from typing_extensions import Self
 
     from litestar._openapi.schema_generation import SchemaCreator
+    from litestar.dto.data_structures import DTOFieldDefinition
     from litestar.dto.interface import HandlerContext
     from litestar.dto.types import ForType
+    from litestar.enums import RequestEncodingType
     from litestar.openapi.spec import Reference, Schema
     from litestar.types.serialization import LitestarEncodableType
 
-    from ._backends import AbstractDTOBackend
-    from .data_structures import FieldDefinition
-
 __all__ = ("AbstractDTOFactory",)
 
 T = TypeVar("T")
 
 
-class AbstractDTOFactory(DTOInterface, Generic[T], metaclass=ABCMeta):
+class AbstractDTOFactory(DTOInterface, Generic[T]):
     """Base class for DTO types."""
 
     __slots__ = ("connection_context",)
 
     config: ClassVar[DTOConfig]
     """Config objects to define properties of the DTO."""
     model_type: ClassVar[type[Any]]
     """If ``annotation`` is an iterable, this is the inner type, otherwise will be the same as ``annotation``."""
 
-    _type_backend_map: ClassVar[dict[tuple[ForType, ParsedType, RequestEncodingType | str | None], AbstractDTOBackend]]
-    _handler_backend_map: ClassVar[dict[tuple[ForType, str], AbstractDTOBackend]]
+    _type_backend_map: ClassVar[dict[tuple[ForType, FieldDefinition, RequestEncodingType | str | None], DTOBackend]]
+    _handler_backend_map: ClassVar[dict[tuple[ForType, str], DTOBackend]]
 
     def __init__(self, connection_context: ConnectionContext) -> None:
         """Create an AbstractDTOFactory type.
 
         Args:
             connection_context: A :class:`ConnectionContext <.ConnectionContext>` instance, which provides
                 information about the connection.
         """
-        self.connection_context = connection_context
+        super().__init__(connection_context=connection_context)
 
     def __class_getitem__(cls, annotation: Any) -> type[Self]:
-        parsed_type = ParsedType(annotation)
+        field_definition = FieldDefinition.from_annotation(annotation)
 
-        if (parsed_type.is_optional and len(parsed_type.args) > 2) or (
-            parsed_type.is_union and not parsed_type.is_optional
+        if (field_definition.is_optional and len(field_definition.args) > 2) or (
+            field_definition.is_union and not field_definition.is_optional
         ):
-            raise InvalidAnnotation(
+            raise InvalidAnnotationException(
                 "Unions are currently not supported as type argument to DTO. Want this? Open an issue."
             )
 
-        if parsed_type.is_forward_ref:
-            raise InvalidAnnotation("Forward references are not supported as type argument to DTO")
+        if field_definition.is_forward_ref:
+            raise InvalidAnnotationException("Forward references are not supported as type argument to DTO")
 
         # if a configuration is not provided, and the type narrowing is a type var, we don't want to create a subclass
-        configs = parse_configs_from_annotation(parsed_type)
-        if parsed_type.is_type_var and not configs:
-            return cls
-
-        if configs:
-            # provided config is always preferred
-            config = configs[0]
-        elif hasattr(cls, "config"):
-            # if no config is provided, but the class has one assigned, use that
-            config = cls.config
-        else:
-            # otherwise, create a new config
-            config = DTOConfig()
+        config = get_dto_config_from_annotated_type(field_definition)
+
+        if not config:
+            if field_definition.is_type_var:
+                return cls
+            config = cls.config if hasattr(cls, "config") else DTOConfig()
 
         cls_dict: dict[str, Any] = {"config": config, "_type_backend_map": {}, "_handler_backend_map": {}}
-        if not parsed_type.is_type_var:
-            cls_dict.update(model_type=parsed_type.annotation)
+        if not field_definition.is_type_var:
+            cls_dict.update(model_type=field_definition.annotation)
 
         return type(f"{cls.__name__}[{annotation}]", (cls,), cls_dict)
 
     def builtins_to_data_type(self, builtins: Any) -> Any:
         """Coerce the unstructured data into the data type."""
         backend = self._get_backend("data", self.connection_context.handler_id)
         return backend.populate_data_from_builtins(builtins, self.connection_context)
@@ -104,70 +93,63 @@
 
     def data_to_encodable_type(self, data: T | Collection[T]) -> LitestarEncodableType:
         backend = self._get_backend("return", self.connection_context.handler_id)
         return backend.encode_data(data, self.connection_context)
 
     @classmethod
     @abstractmethod
-    def generate_field_definitions(cls, model_type: type[Any]) -> Generator[FieldDefinition, None, None]:
+    def generate_field_definitions(cls, model_type: type[Any]) -> Generator[DTOFieldDefinition, None, None]:
         """Generate ``FieldDefinition`` instances from ``model_type``.
 
         Yields:
             ``FieldDefinition`` instances.
         """
 
     @classmethod
     @abstractmethod
-    def detect_nested_field(cls, parsed_type: ParsedType) -> bool:
+    def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
         """Return ``True`` if ``field_definition`` represents a nested model field.
 
         Args:
-            parsed_type: inspect type to determine if field represents a nested model.
+            field_definition: inspect type to determine if field represents a nested model.
 
         Returns:
-            ``True`` if ``parsed_type`` represents a nested model field.
+            ``True`` if ``field_definition`` represents a nested model field.
         """
 
     @classmethod
     def on_registration(cls, handler_context: HandlerContext) -> None:
         """Called each time the DTO type is encountered during signature modelling.
 
         Args:
             handler_context: A :class:`HandlerContext <.HandlerContext>` instance. Provides information about the
                 handler and application of the DTO.
         """
-        parsed_type = handler_context.parsed_type
-        model_type = resolve_model_type(parsed_type)
+        field_definition = handler_context.field_definition
+        model_type = resolve_model_type(field_definition)
         wrapper_attribute_name: str | None = None
 
         if not model_type.is_subclass_of(cls.model_type):
             resolved_generic_result = resolve_generic_wrapper_type(model_type, cls.model_type)
             if resolved_generic_result is not None:
-                model_type, parsed_type, wrapper_attribute_name = resolved_generic_result
+                model_type, field_definition, wrapper_attribute_name = resolved_generic_result
             else:
-                raise InvalidAnnotation(
-                    f"DTO narrowed with '{cls.model_type}', handler type is '{parsed_type.annotation}'"
+                raise InvalidAnnotationException(
+                    f"DTO narrowed with '{cls.model_type}', handler type is '{field_definition.annotation}'"
                 )
 
-        key = (handler_context.dto_for, parsed_type, handler_context.request_encoding_type)
+        key = (handler_context.dto_for, field_definition, handler_context.request_encoding_type)
         backend = cls._type_backend_map.get(key)
         if backend is None:
-            backend_type: type[AbstractDTOBackend]
-            if handler_context.request_encoding_type in {
-                RequestEncodingType.URL_ENCODED,
-                RequestEncodingType.MULTI_PART,
-            }:
-                backend_type = PydanticDTOBackend
-            else:
-                backend_type = MsgspecDTOBackend
+            backend_type: type[DTOBackend] = DTOBackend
 
             backend_context = BackendContext(
                 dto_config=cls.config,
                 dto_for=handler_context.dto_for,
-                parsed_type=parsed_type,
+                field_definition=field_definition,
                 field_definition_generator=cls.generate_field_definitions,
                 is_nested_field_predicate=cls.detect_nested_field,
                 model_type=model_type.annotation,
                 wrapper_attribute_name=wrapper_attribute_name,
             )
             backend = cls._type_backend_map.setdefault(key, backend_type(backend_context))
         cls._handler_backend_map[(handler_context.dto_for, handler_context.handler_id)] = backend
@@ -180,10 +162,10 @@
 
         Returns:
             OpenAPI request body.
         """
         return cls._get_backend(dto_for, handler_id).create_openapi_schema(schema_creator)
 
     @classmethod
-    def _get_backend(cls, dto_for: ForType, handler_id: str) -> AbstractDTOBackend:
+    def _get_backend(cls, dto_for: ForType, handler_id: str) -> DTOBackend:
         """Return the backend for the handler/dto_for combo."""
         return cls._handler_backend_map[(dto_for, handler_id)]
```

### Comparing `litestar-2.0.0b2/litestar/dto/factory/data_structures.py` & `litestar-2.0.0b3/litestar/middleware/allowed_hosts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,79 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Generic, TypeVar
+import re
+from typing import TYPE_CHECKING, Pattern
+
+from litestar.datastructures import URL, MutableScopeHeaders
+from litestar.middleware.base import AbstractMiddleware
+from litestar.response.base import ASGIResponse
+from litestar.response.redirect import ASGIRedirectResponse
+from litestar.status_codes import HTTP_400_BAD_REQUEST
+
+__all__ = ("AllowedHostsMiddleware",)
 
-from litestar.utils.signature import ParsedParameter
 
 if TYPE_CHECKING:
-    from typing import Any, Callable
+    from litestar.config.allowed_hosts import AllowedHostsConfig
+    from litestar.types import ASGIApp, Receive, Scope, Send
 
-    from litestar.dto.factory import DTOField
-    from litestar.dto.factory._backends.abc import AbstractDTOBackend
-    from litestar.dto.types import ForType
 
-T = TypeVar("T")
+class AllowedHostsMiddleware(AbstractMiddleware):
+    """Middleware ensuring the host of a request originated in a trusted host."""
 
+    def __init__(self, app: ASGIApp, config: AllowedHostsConfig) -> None:
+        """Initialize ``AllowedHostsMiddleware``.
 
-class DTOData(Generic[T]):
-    """DTO validated data and utility methods."""
+        Args:
+            app: The ``next`` ASGI app to call.
+            config: An instance of AllowedHostsConfig.
+        """
 
-    __slots__ = ("_backend", "_data_as_builtins")
+        super().__init__(app=app, exclude=config.exclude, exclude_opt_key=config.exclude_opt_key, scopes=config.scopes)
 
-    def __init__(self, backend: AbstractDTOBackend[Any], data_as_builtins: Any) -> None:
-        self._backend = backend
-        self._data_as_builtins = data_as_builtins
+        self.allowed_hosts_regex: Pattern | None = None
+        self.redirect_domains: Pattern | None = None
 
-    def create_instance(self, **kwargs: Any) -> T:
-        """Create an instance of the DTO validated data.
+        if any(host == "*" for host in config.allowed_hosts):
+            return
 
-        Args:
-            **kwargs: Additional data to create the instance with. Takes precedence over DTO validated data.
-        """
-        data = dict(self._data_as_builtins)
-        for k, v in kwargs.items():
-            _set_nested_dict_value(data, k.split("__"), v)
-        return self._backend.transfer_data_from_builtins(data)  # type:ignore[no-any-return]
+        allowed_hosts: set[str] = {
+            rf".*\.{host.replace('*.', '')}$" if host.startswith("*.") else host for host in config.allowed_hosts
+        }
+
+        self.allowed_hosts_regex = re.compile("|".join(sorted(allowed_hosts)))  # pyright: ignore
 
-    def update_instance(self, instance: T, **kwargs: Any) -> T:
-        """Update an instance with the DTO validated data.
+        if config.www_redirect and (
+            redirect_domains := {host.replace("www.", "") for host in config.allowed_hosts if host.startswith("www.")}
+        ):
+            self.redirect_domains = re.compile("|".join(sorted(redirect_domains)))  # pyright: ignore
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
+        """ASGI callable.
 
         Args:
-            instance: The instance to update.
-            **kwargs: Additional data to update the instance with. Takes precedence over DTO validated data.
+            scope: The ASGI connection scope.
+            receive: The ASGI receive function.
+            send: The ASGI send function.
+
+        Returns:
+            None
         """
-        data = {**self._data_as_builtins, **kwargs}
-        for k, v in data.items():
-            setattr(instance, k, v)
-        return instance
-
-    def as_builtins(self) -> Any:
-        """Return the DTO validated data as builtins."""
-        return self._data_as_builtins
-
-
-def _set_nested_dict_value(d: dict[str, Any], keys: list[str], value: Any) -> None:
-    if len(keys) == 1:
-        d[keys[0]] = value
-    else:
-        key = keys[0]
-        d.setdefault(key, {})
-        _set_nested_dict_value(d[key], keys[1:], value)
-
-
-@dataclass(frozen=True)
-class FieldDefinition(ParsedParameter):
-    """A model field representation for purposes of generating a DTO backend model type."""
-
-    __slots__ = (
-        "default_factory",
-        "dto_field",
-        "dto_for",
-        "unique_model_name",
-    )
-
-    unique_model_name: str
-    """Unique identifier of model that owns the field."""
-    default_factory: Callable[[], Any] | None
-    """Default factory of the field."""
-    dto_field: DTOField
-    """DTO field configuration."""
-    dto_for: ForType | None
-    """Direction of transfer for field.
-
-    Specify if the field definition should only be added to models for only the request (``"data"``) or response
-    (``"return"``). If there should be no such distinction, set to ``None``.
-
-    This is to support special cases where the type to set an attribute may be different to the type received when
-    retrieving its value. For example, a :class:`sqlalchemy.ext.hybrid.hybrid_property` may be set with a ``str`` but
-    retrieved as some other type.
-
-    The difference between this, and marking a field as read-only or private, is that it cannot be overridden by the end
-    user.
-    """
+        if self.allowed_hosts_regex is None:
+            await self.app(scope, receive, send)
+            return
+
+        headers = MutableScopeHeaders(scope=scope)
+        if host := headers.get("host", headers.get("x-forwarded-host", "")).split(":")[0]:
+            if self.allowed_hosts_regex.fullmatch(host):
+                await self.app(scope, receive, send)
+                return
+
+            if self.redirect_domains is not None and self.redirect_domains.fullmatch(host):
+                url = URL.from_scope(scope)
+                redirect_url = url.with_replacements(netloc=f"www.{url.netloc}")
+                redirect_response = ASGIRedirectResponse(path=str(redirect_url))
+                await redirect_response(scope, receive, send)
+                return
 
-    def unique_name(self) -> str:
-        return f"{self.unique_model_name}.{self.name}"
+        response = ASGIResponse(body=b'{"message":"invalid host header"}', status_code=HTTP_400_BAD_REQUEST)
+        await response(scope, receive, send)
```

### Comparing `litestar-2.0.0b2/litestar/dto/factory/field.py` & `litestar-2.0.0b3/litestar/dto/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/dto/factory/stdlib/dataclass.py` & `litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_dto_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,80 @@
 from __future__ import annotations
 
-from dataclasses import MISSING, fields
-from typing import TYPE_CHECKING, Generic, TypeVar
+from dataclasses import replace
+from typing import TYPE_CHECKING, Collection, Generic, TypeVar
 
-from litestar.dto.factory.abc import AbstractDTOFactory
-from litestar.dto.factory.data_structures import FieldDefinition
-from litestar.dto.factory.field import DTO_FIELD_META_KEY, DTOField
-from litestar.dto.factory.utils import get_model_type_hints
+from litestar.dto._utils import get_model_type_hints
+from litestar.dto.base_factory import AbstractDTOFactory
+from litestar.dto.data_structures import DTOFieldDefinition
+from litestar.dto.field import DTO_FIELD_META_KEY, DTOField
+from litestar.exceptions import MissingDependencyException
 from litestar.types.empty import Empty
 from litestar.utils.helpers import get_fully_qualified_class_name
 
 if TYPE_CHECKING:
-    from typing import ClassVar, Collection, Generator
+    from typing import ClassVar, Generator
 
-    from litestar.types.protocols import DataclassProtocol
-    from litestar.typing import ParsedType
+    from litestar.typing import FieldDefinition
 
-__all__ = ("DataclassDTO", "T")
 
-T = TypeVar("T", bound="DataclassProtocol | Collection[DataclassProtocol]")
-AnyDataclass = TypeVar("AnyDataclass", bound="DataclassProtocol")
+try:
+    import pydantic
 
+    if pydantic.VERSION.startswith("2"):
+        from pydantic_core import PydanticUndefined
+    else:  # pragma: no cover
+        from pydantic.fields import Undefined as PydanticUndefined  # type: ignore
+except ImportError as e:
+    raise MissingDependencyException("pydantic") from e
 
-class DataclassDTO(AbstractDTOFactory[T], Generic[T]):
-    """Support for domain modelling with dataclasses."""
+__all__ = ("PydanticDTO",)
+
+T = TypeVar("T", bound="pydantic.BaseModel | Collection[pydantic.BaseModel]")
+
+
+class PydanticDTO(AbstractDTOFactory[T], Generic[T]):
+    """Support for domain modelling with Pydantic."""
 
     __slots__ = ()
 
-    model_type: ClassVar[type[DataclassProtocol]]
+    model_type: ClassVar[type[pydantic.BaseModel]]
 
     @classmethod
-    def generate_field_definitions(cls, model_type: type[DataclassProtocol]) -> Generator[FieldDefinition, None, None]:
-        dc_fields = {f.name: f for f in fields(model_type)}
-        for key, parsed_type in get_model_type_hints(model_type).items():
-            if not (dc_field := dc_fields.get(key)):
-                continue
-
-            default = dc_field.default if dc_field.default is not MISSING else Empty
-
-            default_factory = dc_field.default_factory if dc_field.default_factory is not MISSING else None
-
-            field_def = FieldDefinition(
-                name=key,
-                parsed_type=parsed_type,
+    def generate_field_definitions(
+        cls, model_type: type[pydantic.BaseModel]
+    ) -> Generator[DTOFieldDefinition, None, None]:
+        model_field_definitions = get_model_type_hints(model_type)
+
+        if pydantic.VERSION.startswith("1"):  # pragma: no cover
+            model_fields: dict[str, pydantic.fields.FieldInfo] = {k: model_field.field_info for k, model_field in model_type.__fields__.items()}  # type: ignore
+        else:
+            model_fields = dict(model_type.model_fields)
+
+        for field_name, field_info in model_fields.items():
+            field_definition = model_field_definitions[field_name]
+            dto_field = (field_definition.extra or {}).pop(DTO_FIELD_META_KEY, DTOField())
+
+            if field_info.default is not PydanticUndefined:
+                default = field_info.default
+            elif field_definition.is_optional:
+                default = None
+            else:
+                default = Empty
+
+            yield replace(
+                DTOFieldDefinition.from_field_definition(
+                    field_definition=field_definition,
+                    dto_field=dto_field,
+                    unique_model_name=get_fully_qualified_class_name(model_type),
+                    default_factory=field_info.default_factory
+                    if field_info.default_factory and field_info.default_factory is not PydanticUndefined  # type: ignore[comparison-overlap]
+                    else Empty,
+                    dto_for=None,
+                ),
                 default=default,
-                default_factory=default_factory,
-                dto_field=dc_field.metadata.get(DTO_FIELD_META_KEY, DTOField()),
-                unique_model_name=get_fully_qualified_class_name(model_type),
-                dto_for=None,
+                name=field_name,
             )
 
-            yield field_def
-
     @classmethod
-    def detect_nested_field(cls, parsed_type: ParsedType) -> bool:
-        return hasattr(parsed_type.annotation, "__dataclass_fields__")
+    def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
+        return field_definition.is_subclass_of(pydantic.BaseModel)
```

### Comparing `litestar-2.0.0b2/litestar/dto/interface.py` & `litestar-2.0.0b3/litestar/dto/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,81 @@
 from __future__ import annotations
 
-from abc import abstractmethod
-from typing import TYPE_CHECKING, Protocol, runtime_checkable
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Callable
 
 from litestar.enums import RequestEncodingType
-from litestar.openapi.spec import Schema
 
 if TYPE_CHECKING:
     from typing import Any, Final
 
     from typing_extensions import Self
 
     from litestar._openapi.schema_generation import SchemaCreator
-    from litestar.openapi.spec import Reference
-    from litestar.types import LitestarEncodableType
-    from litestar.types.internal_types import AnyConnection
-    from litestar.typing import ParsedType
+    from litestar.connection import ASGIConnection
+    from litestar.openapi.spec import Reference, Schema
+    from litestar.types import LitestarEncodableType, TypeDecodersSequence
+    from litestar.typing import FieldDefinition
 
     from .types import ForType
 
 __all__ = (
     "ConnectionContext",
     "DTOInterface",
     "HandlerContext",
 )
 
 
 class HandlerContext:
     """Context object passed to the ``on_registration`` method of a DTO."""
 
-    __slots__ = ("dto_for", "handler_id", "parsed_type", "request_encoding_type")
+    __slots__ = ("dto_for", "handler_id", "field_definition", "request_encoding_type")
 
     def __init__(
         self,
+        *,
         dto_for: ForType,
         handler_id: str,
-        parsed_type: ParsedType,
+        field_definition: FieldDefinition,
         request_encoding_type: RequestEncodingType | str = RequestEncodingType.JSON,
     ) -> None:
         self.dto_for: Final[ForType] = dto_for
         self.handler_id: Final[str] = handler_id
-        self.parsed_type: Final[ParsedType] = parsed_type
+        self.field_definition: Final[FieldDefinition] = field_definition
         self.request_encoding_type: Final[RequestEncodingType | str] = request_encoding_type
 
 
 class ConnectionContext:
     """Context object passed to the ``__init__`` method of a DTO."""
 
-    __slots__ = ("handler_id", "request_encoding_type")
+    __slots__ = ("handler_id", "request_encoding_type", "default_deserializer", "type_decoders")
 
-    def __init__(self, handler_id: str, request_encoding_type: RequestEncodingType | str) -> None:
+    def __init__(
+        self,
+        handler_id: str,
+        request_encoding_type: RequestEncodingType | str,
+        default_deserializer: Callable[[Any, Any], Any],
+        type_decoders: TypeDecodersSequence | None,
+    ) -> None:
         self.handler_id: Final[str] = handler_id
         self.request_encoding_type: Final[RequestEncodingType | str] = request_encoding_type
+        self.default_deserializer: Final[Callable[[Any, Any], Any]] = default_deserializer
+        self.type_decoders = type_decoders
 
     @classmethod
-    def from_connection(cls, connection: AnyConnection) -> Self:
+    def from_connection(cls, connection: ASGIConnection[Any, Any, Any, Any]) -> Self:
         return cls(
             handler_id=str(connection.route_handler),
             request_encoding_type=getattr(connection, "content_type", (RequestEncodingType.JSON,))[0],
+            default_deserializer=connection.route_handler.default_deserializer,
+            type_decoders=connection.route_handler.resolve_type_decoders(),
         )
 
 
-@runtime_checkable
-class DTOInterface(Protocol):
+class DTOInterface(ABC):
     __slots__ = ("connection_context",)
 
     connection_context: ConnectionContext
 
     def __init__(self, connection_context: ConnectionContext) -> None:
         """Initialize the DTO.
 
@@ -105,31 +114,32 @@
             raw: Raw bytes of the payload.
 
         Returns:
             Data type that the DTO represents.
         """
 
     @classmethod
+    @abstractmethod
     def create_openapi_schema(
         cls, dto_for: ForType, handler_id: str, schema_creator: SchemaCreator
     ) -> Reference | Schema:
         """Create an OpenAPI request body for the DTO.
 
         Returns:
             An optional :class:`RequestBody <.openapi.spec.request_body.RequestBody>` instance.
         """
-        return Schema()
 
     @classmethod
+    @abstractmethod
     def on_registration(cls, handler_context: HandlerContext) -> None:
         """Receive information about the handler and application of the DTO.
 
-        At this point, if the DTO type does not support the annotated type of ``handler_context.parsed_type``, it should
+        At this point, if the DTO type does not support the annotated type of ``handler_context.field_definition``, it should
         raise an ``UnsupportedType`` exception.
 
         Args:
             handler_context: A :class:`HandlerContext <.HandlerContext>` instance. Provides information about the
                 handler and application of the DTO.
 
         Raises:
-            UnsupportedType: If the DTO type does not support the annotated type of ``parsed_type``.
+            UnsupportedType: If the DTO type does not support the annotated type of ``field_definition``.
         """
```

### Comparing `litestar-2.0.0b2/litestar/enums.py` & `litestar-2.0.0b3/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/events/emitter.py` & `litestar-2.0.0b3/litestar/events/emitter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/events/listener.py` & `litestar-2.0.0b3/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/exceptions/__init__.py` & `litestar-2.0.0b3/litestar/exceptions/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .base_exceptions import LitestarException, LitestarWarning, MissingDependencyException, SerializationException
+from .dto_exceptions import DTOFactoryException, InvalidAnnotationException
 from .http_exceptions import (
     ClientException,
     HTTPException,
     ImproperlyConfiguredException,
     InternalServerException,
     MethodNotAllowedException,
     NoRouteMatchFoundException,
@@ -14,17 +15,19 @@
     TooManyRequestsException,
     ValidationException,
 )
 from .websocket_exceptions import WebSocketDisconnect, WebSocketException
 
 __all__ = (
     "ClientException",
+    "DTOFactoryException",
     "HTTPException",
     "ImproperlyConfiguredException",
     "InternalServerException",
+    "InvalidAnnotationException",
     "LitestarException",
     "LitestarWarning",
     "MethodNotAllowedException",
     "MissingDependencyException",
     "NoRouteMatchFoundException",
     "NotAuthorizedException",
     "NotFoundException",
```

### Comparing `litestar-2.0.0b2/litestar/exceptions/base_exceptions.py` & `litestar-2.0.0b3/litestar/exceptions/base_exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any
 
-__all__ = ("MissingDependencyException", "SerializationException", "LitestarException")
+__all__ = ("MissingDependencyException", "SerializationException", "LitestarException", "LitestarWarning")
 
 
 class LitestarException(Exception):
     """Base exception class from which all Litestar exceptions inherit."""
 
     detail: str
```

### Comparing `litestar-2.0.0b2/litestar/exceptions/http_exceptions.py` & `litestar-2.0.0b3/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/exceptions/websocket_exceptions.py` & `litestar-2.0.0b3/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/file_system.py` & `litestar-2.0.0b3/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/handlers/__init__.py` & `litestar-2.0.0b3/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/handlers/asgi_handlers.py` & `litestar-2.0.0b3/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/handlers/base.py` & `litestar-2.0.0b3/litestar/handlers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 from __future__ import annotations
 
 from copy import copy
-from typing import TYPE_CHECKING, Any, Mapping, Sequence, cast
+from functools import partial
+from typing import TYPE_CHECKING, Any, Callable, Mapping, Sequence, cast
 
-from litestar._signature import create_signature_model
-from litestar._signature.field import SignatureField
+from litestar._signature import SignatureModel
 from litestar.di import Provide
 from litestar.dto.interface import HandlerContext
 from litestar.exceptions import ImproperlyConfiguredException
-from litestar.types import Dependencies, Empty, ExceptionHandlersMap, Guard, MaybePartial, Middleware, TypeEncodersMap
+from litestar.serialization import default_deserializer
+from litestar.types import (
+    Dependencies,
+    Empty,
+    ExceptionHandlersMap,
+    Guard,
+    MaybePartial,
+    Middleware,
+    TypeDecodersSequence,
+    TypeEncodersMap,
+)
+from litestar.typing import FieldDefinition
 from litestar.utils import AsyncCallable, Ref, async_partial, get_name, normalize_path
 from litestar.utils.helpers import unwrap_partial
 from litestar.utils.predicates import is_async_callable
-from litestar.utils.signature import ParsedSignature, infer_request_encoding_from_parameter
+from litestar.utils.signature import ParsedSignature, infer_request_encoding_from_field_definition
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from litestar import Litestar
-    from litestar._signature.models import SignatureModel
     from litestar.connection import ASGIConnection
     from litestar.controller import Controller
     from litestar.dto.interface import DTOInterface
     from litestar.params import ParameterKwarg
     from litestar.plugins import SerializationPluginProtocol
     from litestar.router import Router
     from litestar.types import AnyCallable, AsyncAnyCallable, ExceptionHandler
@@ -42,27 +52,29 @@
         "_parsed_fn_signature",
         "_resolved_dependencies",
         "_resolved_dto",
         "_resolved_guards",
         "_resolved_layered_parameters",
         "_resolved_return_dto",
         "_resolved_signature_namespace",
+        "_resolved_type_decoders",
         "_resolved_type_encoders",
         "dependencies",
         "dto",
         "exception_handlers",
         "guards",
         "middleware",
         "name",
         "opt",
         "owner",
         "paths",
         "return_dto",
         "signature_model",
         "signature_namespace",
+        "type_decoders",
         "type_encoders",
     )
 
     def __init__(
         self,
         path: str | Sequence[str] | None = None,
         *,
@@ -72,14 +84,15 @@
         guards: Sequence[Guard] | None = None,
         middleware: Sequence[Middleware] | None = None,
         name: str | None = None,
         opt: Mapping[str, Any] | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         type_encoders: TypeEncodersMap | None = None,
+        type_decoders: TypeDecodersSequence | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``HTTPRouteHandler``.
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults
                 to ``/``
@@ -94,24 +107,26 @@
                 wherever you have access to :class:`Request <.connection.Request>` or
                 :class:`ASGI Scope <.types.Scope>`.
             return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature
                 modelling.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
+            type_decoders: A sequence of tuples, each composed of a predicate testing for type identity and a msgspec hook for deserialization.
             **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
         self._parsed_fn_signature: ParsedSignature | EmptyType = Empty
         self._resolved_dependencies: dict[str, Provide] | EmptyType = Empty
         self._resolved_dto: type[DTOInterface] | None | EmptyType = Empty
         self._resolved_guards: list[Guard] | EmptyType = Empty
-        self._resolved_layered_parameters: dict[str, SignatureField] | EmptyType = Empty
+        self._resolved_layered_parameters: dict[str, FieldDefinition] | EmptyType = Empty
         self._resolved_return_dto: type[DTOInterface] | None | EmptyType = Empty
         self._resolved_signature_namespace: dict[str, Any] | EmptyType = Empty
         self._resolved_type_encoders: TypeEncodersMap | EmptyType = Empty
+        self._resolved_type_decoders: TypeDecodersSequence | EmptyType = Empty
 
         self.dependencies = dependencies
         self.dto = dto
         self.exception_handlers = exception_handlers
         self.guards = guards
         self.middleware = middleware
         self.name = name
@@ -123,21 +138,32 @@
         self.paths = (
             {normalize_path(p) for p in path}
             if path and isinstance(path, list)
             else {normalize_path(path or "/")}  # type: ignore
         )
         self.opt.update(**kwargs)
         self.type_encoders = type_encoders
+        self.type_decoders = type_decoders
 
     def __call__(self, fn: AsyncAnyCallable) -> Self:
         """Replace a function with itself."""
         self._fn = Ref["MaybePartial[AsyncAnyCallable]"](fn)
         return self
 
     @property
+    def default_deserializer(self) -> Callable[[Any, Any], Any]:
+        """Get a default serializer for the route handler.
+
+        Returns:
+            A default serializer for the route handler.
+
+        """
+        return partial(default_deserializer, type_decoders=self.resolve_type_decoders())
+
+    @property
     def fn(self) -> Ref[MaybePartial[AsyncAnyCallable]]:
         """Get the handler function.
 
         Raises:
             ImproperlyConfiguredException: if handler fn is not set.
 
         Returns:
@@ -208,30 +234,44 @@
             self._resolved_type_encoders = {}
 
             for layer in self.ownership_layers:
                 if type_encoders := getattr(layer, "type_encoders", None):
                     self._resolved_type_encoders.update(type_encoders)
         return cast("TypeEncodersMap", self._resolved_type_encoders)
 
-    def resolve_layered_parameters(self) -> dict[str, SignatureField]:
+    def resolve_type_decoders(self) -> TypeDecodersSequence:
+        """Return a merged type_encoders mapping.
+
+        This method is memoized so the computation occurs only once.
+
+        Returns:
+            A dict of type encoders
+        """
+        if self._resolved_type_decoders is Empty:
+            self._resolved_type_decoders = []
+
+            for layer in self.ownership_layers:
+                if type_decoders := getattr(layer, "type_decoders", None):
+                    self._resolved_type_decoders.extend(list(type_decoders))
+        return cast("TypeDecodersSequence", self._resolved_type_decoders)
+
+    def resolve_layered_parameters(self) -> dict[str, FieldDefinition]:
         """Return all parameters declared above the handler."""
         if self._resolved_layered_parameters is Empty:
             parameter_kwargs: dict[str, ParameterKwarg] = {}
 
             for layer in self.ownership_layers:
                 parameter_kwargs.update(getattr(layer, "parameters", {}) or {})
 
             self._resolved_layered_parameters = {
-                key: SignatureField.create(
-                    name=key, field_type=parameter.value_type, default_value=parameter.default, kwarg_model=parameter
-                )
+                key: FieldDefinition.from_kwarg(name=key, annotation=parameter.annotation, kwarg_definition=parameter)
                 for key, parameter in parameter_kwargs.items()
             }
 
-        return cast("dict[str, SignatureField]", self._resolved_layered_parameters)
+        return cast("dict[str, FieldDefinition]", self._resolved_layered_parameters)
 
     def resolve_guards(self) -> list[Guard]:
         """Return all guards in the handlers scope, starting from highest to current layer."""
         if self._resolved_guards is Empty:
             self._resolved_guards = []
 
             for layer in self.ownership_layers:
@@ -358,20 +398,27 @@
         self._resolved_return_dto = dto
 
     def _init_handler_dtos(self) -> None:
         """Initialize the data and return DTOs for the handler."""
         if (dto := self.resolve_dto()) and (data_parameter := self.parsed_fn_signature.parameters.get("data")):
             dto.on_registration(
                 HandlerContext(
-                    "data", str(self), data_parameter.parsed_type, infer_request_encoding_from_parameter(data_parameter)
+                    dto_for="data",
+                    handler_id=str(self),
+                    field_definition=data_parameter,
+                    request_encoding_type=infer_request_encoding_from_field_definition(data_parameter),
                 )
             )
 
         if return_dto := self.resolve_return_dto():
-            return_dto.on_registration(HandlerContext("return", str(self), self.parsed_fn_signature.return_type))
+            return_dto.on_registration(
+                HandlerContext(
+                    dto_for="return", handler_id=str(self), field_definition=self.parsed_fn_signature.return_type
+                )
+            )
 
     async def authorize_connection(self, connection: ASGIConnection) -> None:
         """Ensure the connection is authorized by running all the route guards in scope."""
         for guard in self.resolve_guards():
             await guard(connection, copy(self))  # type: ignore
 
     @staticmethod
@@ -412,30 +459,28 @@
                     provider.dependency.value = async_partial(provider.dependency.value)
                 else:
                     provider.has_sync_callable = True
 
     def _create_signature_model(self, app: Litestar) -> None:
         """Create signature model for handler function."""
         if not self.signature_model:
-            self.signature_model = create_signature_model(
+            self.signature_model = SignatureModel.create(
                 dependency_name_set=self.dependency_name_set,
                 fn=cast("AnyCallable", self.fn.value),
-                preferred_validation_backend=app._preferred_validation_backend,
                 parsed_signature=self.parsed_fn_signature,
                 has_data_dto=bool(self.resolve_dto()),
             )
 
     def _create_provider_signature_models(self, app: Litestar) -> None:
         """Create signature models for dependency providers."""
         for provider in self.resolve_dependencies().values():
             if not getattr(provider, "signature_model", None):
-                provider.signature_model = create_signature_model(
+                provider.signature_model = SignatureModel.create(
                     dependency_name_set=self.dependency_name_set,
                     fn=provider.dependency.value,
-                    preferred_validation_backend=app._preferred_validation_backend,
                     parsed_signature=ParsedSignature.from_fn(
                         unwrap_partial(provider.dependency.value), self.resolve_signature_namespace()
                     ),
                     has_data_dto=bool(self.resolve_dto()),
                 )
 
     def _handle_serialization_plugins(self, plugins: list[SerializationPluginProtocol]) -> None:
@@ -446,16 +491,16 @@
             for plugin in plugins:
                 if plugin.supports_type(return_type):
                     self._set_return_dto(plugin.create_dto_for_type(return_type))
                     break
 
         if (data_param := self.parsed_fn_signature.parameters.get("data")) and self.resolve_dto() is None:
             for plugin in plugins:
-                if plugin.supports_type(data_param.parsed_type):
-                    self._set_dto(plugin.create_dto_for_type(data_param.parsed_type))
+                if plugin.supports_type(data_param):
+                    self._set_dto(plugin.create_dto_for_type(data_param))
                     break
 
     def __str__(self) -> str:
         """Return a unique identifier for the route handler.
 
         Returns:
             A string
```

### Comparing `litestar-2.0.0b2/litestar/handlers/http_handlers/_utils.py` & `litestar-2.0.0b3/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/handlers/http_handlers/base.py` & `litestar-2.0.0b3/litestar/handlers/http_handlers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     from typing import Any, Awaitable, Callable, Sequence
 
     from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.config.response_cache import CACHE_FOREVER
     from litestar.connection import Request
     from litestar.datastructures import CacheControlHeader, ETag
-    from litestar.datastructures.headers import Header
     from litestar.dto.interface import DTOInterface
     from litestar.openapi.datastructures import ResponseSpec
     from litestar.openapi.spec import SecurityRequirement
 
 __all__ = ("HTTPRouteHandler", "route")
 
 
@@ -295,18 +294,22 @@
         """Return the closest custom Response class in the owner graph or the default Response class.
 
         This method is memoized so the computation occurs only once.
 
         Returns:
             The default :class:`Response <.response.Response>` class for the route handler.
         """
-        for layer in list(reversed(self.ownership_layers)):
-            if layer.response_class is not None:
-                return layer.response_class
-        return Response
+        return next(
+            (
+                layer.response_class
+                for layer in list(reversed(self.ownership_layers))
+                if layer.response_class is not None
+            ),
+            Response,
+        )
 
     def resolve_response_headers(self) -> frozenset[ResponseHeader]:
         """Return all header parameters in the scope of the handler function.
 
         Returns:
             A dictionary mapping keys to :class:`ResponseHeader <.datastructures.ResponseHeader>` instances.
         """
@@ -319,16 +322,15 @@
                     # type-checking error on everything but the controller. We cover this case nevertheless
                     resolved_response_headers.update(
                         {name: ResponseHeader(name=name, value=value) for name, value in layer_response_headers.items()}
                     )
                 else:
                     resolved_response_headers.update({h.name: h for h in layer_response_headers})
             for extra_header in ("cache_control", "etag"):
-                header_model: Header | None = getattr(layer, extra_header, None)
-                if header_model:
+                if header_model := getattr(layer, extra_header, None):
                     resolved_response_headers[header_model.HEADER_NAME] = ResponseHeader(
                         name=header_model.HEADER_NAME,
                         value=header_model.to_header(),
                         documentation_only=header_model.documentation_only,
                     )
 
         return frozenset(resolved_response_headers.values())
```

### Comparing `litestar-2.0.0b2/litestar/handlers/http_handlers/decorators.py` & `litestar-2.0.0b3/litestar/handlers/http_handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.0.0b3/litestar/handlers/websocket_handlers/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 return received_data.encode("utf-8")
             return received_data
 
     else:
 
         async def handle_receive(socket: WebSocket, dto: DTOInterface | None) -> Any:
             received_data = await socket.receive_data(mode=receive_mode)
-            return decode_json(received_data)
+            return decode_json(value=received_data, type_decoders=socket.route_handler.resolve_type_decoders())
 
     return handle_receive
 
 
 def create_handle_send(
     resolved_return_dto: type[DTOInterface] | None,
     json_encoder: JsonEncoder,
```

### Comparing `litestar-2.0.0b2/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.0.0b3/litestar/handlers/websocket_handlers/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Optional,
     cast,
     overload,
 )
 
 from msgspec.json import Encoder as JsonEncoder
 
-from litestar._signature import create_signature_model
+from litestar._signature import SignatureModel
 from litestar.connection import WebSocket
 from litestar.dto.interface import HandlerContext
 from litestar.exceptions import ImproperlyConfiguredException, WebSocketDisconnect
 from litestar.serialization import default_serializer
 from litestar.types import (
     AnyCallable,
     Dependencies,
@@ -260,19 +260,21 @@
         # since none of the validation rules of WebsocketRouteHandler apply here, this is let empty. Validation of the
         # user supplied method happens at init time of this handler instead in __call__
 
     def _init_handler_dtos(self) -> None:
         """Initialize the data and return DTOs for the handler."""
         if dto := self.resolve_dto():
             data_parameter = self._listener_context.listener_callback_signature.parameters["data"]
-            dto.on_registration(HandlerContext("data", str(self), data_parameter.parsed_type))
+            dto.on_registration(HandlerContext(dto_for="data", handler_id=str(self), field_definition=data_parameter))
 
         if return_dto := self.resolve_return_dto():
             return_type = self._listener_context.listener_callback_signature.return_type
-            return_dto.on_registration(HandlerContext("return", str(self), return_type))
+            return_dto.on_registration(
+                HandlerContext(dto_for="return", handler_id=str(self), field_definition=return_type)
+            )
 
     def __call__(self, listener_callback: AnyCallable) -> websocket_listener:
         self._listener_context.listener_callback = listener_callback
         self._listener_context.handler_function = handler_function = create_handler_function(
             listener_context=self._listener_context,
             lifespan_manager=self._connection_lifespan or self.default_connection_lifespan,
         )
@@ -284,18 +286,17 @@
 
     def _create_signature_model(self, app: Litestar) -> None:
         """Create signature model for handler function."""
         if not self.signature_model:
             new_signature = create_handler_signature(
                 self._listener_context.listener_callback_signature.original_signature
             )
-            self.signature_model = create_signature_model(
+            self.signature_model = SignatureModel.create(
                 dependency_name_set=self.dependency_name_set,
                 fn=cast("AnyCallable", self.fn.value),
-                preferred_validation_backend=app._preferred_validation_backend,
                 parsed_signature=ParsedSignature.from_signature(new_signature, self.resolve_signature_namespace()),
             )
 
     def _set_listener_context(self) -> None:
         listener_callback_signature = ParsedSignature.from_fn(
             self._listener_context.listener_callback, self.resolve_signature_namespace()
         )
```

### Comparing `litestar-2.0.0b2/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.0.0b3/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/logging/_utils.py` & `litestar-2.0.0b3/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/logging/config.py` & `litestar-2.0.0b3/litestar/logging/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,29 +226,33 @@
 
             values = {k: v for k, v in asdict(self).items() if v is not None}
 
         config.dictConfig(values)
         return cast("Callable[[str], Logger]", getLogger)
 
 
+def default_json_serializer(value: Any, default: Callable[[Any], Any] | None = None) -> bytes:
+    return encode_json(value=value, serializer=default)
+
+
 def default_structlog_processors() -> list[Processor] | None:  # pyright: ignore
     """Set the default processors for structlog.
 
     Returns:
         An optional list of processors.
     """
     try:
         import structlog
 
         return [
             structlog.contextvars.merge_contextvars,
             structlog.processors.add_log_level,
             structlog.processors.format_exc_info,
             structlog.processors.TimeStamper(fmt="iso"),
-            structlog.processors.JSONRenderer(serializer=encode_json),
+            structlog.processors.JSONRenderer(serializer=default_json_serializer),
         ]
     except ImportError:  # pragma: no cover
         return None
 
 
 def default_wrapper_class() -> type[BindableLogger] | None:  # pyright: ignore
     """Set the default wrapper class for structlog.
```

### Comparing `litestar-2.0.0b2/litestar/logging/picologging.py` & `litestar-2.0.0b3/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/logging/standard.py` & `litestar-2.0.0b3/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/middleware/_utils.py` & `litestar-2.0.0b3/litestar/middleware/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,12 +53,13 @@
     """
     if scope["type"] not in scopes:
         return True
 
     if exclude_opt_key and scope["route_handler"].opt.get(exclude_opt_key):
         return True
 
-    if exclude_path_pattern and exclude_path_pattern.findall(
-        scope["path"] if not getattr(scope.get("route_handler", {}), "is_mount", False) else scope["raw_path"].decode()
-    ):
-        return True
-    return False
+    return bool(
+        exclude_path_pattern
+        and exclude_path_pattern.findall(
+            scope["raw_path"].decode() if getattr(scope.get("route_handler", {}), "is_mount", False) else scope["path"]
+        )
+    )
```

### Comparing `litestar-2.0.0b2/litestar/middleware/allowed_hosts.py` & `litestar-2.0.0b3/litestar/middleware/authentication.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,96 @@
 from __future__ import annotations
 
-import re
-from typing import TYPE_CHECKING, Pattern
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any
+
+from litestar.connection import ASGIConnection
+from litestar.enums import ScopeType
+from litestar.middleware._utils import (
+    build_exclude_path_pattern,
+    should_bypass_middleware,
+)
 
-from litestar.datastructures import URL, MutableScopeHeaders
-from litestar.middleware.base import AbstractMiddleware
-from litestar.response.base import ASGIResponse
-from litestar.response.redirect import ASGIRedirectResponse
-from litestar.status_codes import HTTP_400_BAD_REQUEST
-
-__all__ = ("AllowedHostsMiddleware",)
+__all__ = ("AbstractAuthenticationMiddleware", "AuthenticationResult")
 
 
 if TYPE_CHECKING:
-    from litestar.config.allowed_hosts import AllowedHostsConfig
-    from litestar.types import ASGIApp, Receive, Scope, Send
-
+    from litestar.types import ASGIApp, Receive, Scope, Scopes, Send
 
-class AllowedHostsMiddleware(AbstractMiddleware):
-    """Middleware ensuring the host of a request originated in a trusted host."""
 
-    def __init__(self, app: ASGIApp, config: AllowedHostsConfig) -> None:
-        """Initialize ``AllowedHostsMiddleware``.
+@dataclass
+class AuthenticationResult:
+    """Pydantic model for authentication data."""
+
+    __slots__ = ("user", "auth")
+
+    user: Any
+    """The user model, this can be any value corresponding to a user of the API."""
+    auth: Any
+    """The auth value, this can for example be a JWT token."""
+
+
+class AbstractAuthenticationMiddleware(ABC):
+    """Abstract AuthenticationMiddleware that allows users to create their own AuthenticationMiddleware by extending it
+    and overriding :meth:`AbstractAuthenticationMiddleware.authenticate_request`.
+    """
+
+    def __init__(
+        self,
+        app: ASGIApp,
+        exclude: str | list[str] | None = None,
+        exclude_from_auth_key: str = "exclude_from_auth",
+        scopes: Scopes | None = None,
+    ) -> None:
+        """Initialize ``AbstractAuthenticationMiddleware``.
 
         Args:
-            app: The ``next`` ASGI app to call.
-            config: An instance of AllowedHostsConfig.
+            app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
+            exclude: A pattern or list of patterns to skip in the authentication middleware.
+            exclude_from_auth_key: An identifier to use on routes to disable authentication for a particular route.
+            scopes: ASGI scopes processed by the authentication middleware.
         """
-
-        super().__init__(app=app, exclude=config.exclude, exclude_opt_key=config.exclude_opt_key, scopes=config.scopes)
-
-        self.allowed_hosts_regex: Pattern | None = None
-        self.redirect_domains: Pattern | None = None
-
-        if any(host == "*" for host in config.allowed_hosts):
-            return
-
-        allowed_hosts: set[str] = {
-            rf".*\.{host.replace('*.', '')}$" if host.startswith("*.") else host for host in config.allowed_hosts
-        }
-
-        self.allowed_hosts_regex = re.compile("|".join(sorted(allowed_hosts)))  # pyright: ignore
-
-        if config.www_redirect:
-            redirect_domains: set[str] = {
-                host.replace("www.", "") for host in config.allowed_hosts if host.startswith("www.")
-            }
-            if redirect_domains:
-                self.redirect_domains = re.compile("|".join(sorted(redirect_domains)))  # pyright: ignore
+        self.app = app
+        self.scopes = scopes or {ScopeType.HTTP, ScopeType.WEBSOCKET}
+        self.exclude_opt_key = exclude_from_auth_key
+        self.exclude = build_exclude_path_pattern(exclude=exclude)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
         Returns:
             None
         """
-        if self.allowed_hosts_regex is None:
-            await self.app(scope, receive, send)
-            return
-
-        headers = MutableScopeHeaders(scope=scope)
-        host = headers.get("host", headers.get("x-forwarded-host", "")).split(":")[0]
-
-        if host:
-            if self.allowed_hosts_regex.fullmatch(host):
-                await self.app(scope, receive, send)
-                return
-
-            if self.redirect_domains is not None and self.redirect_domains.fullmatch(host):
-                url = URL.from_scope(scope)
-                redirect_url = url.with_replacements(netloc="www." + url.netloc)
-                redirect_response = ASGIRedirectResponse(path=str(redirect_url))
-                await redirect_response(scope, receive, send)
-                return
+        if not should_bypass_middleware(
+            scope=scope,
+            scopes=self.scopes,
+            exclude_path_pattern=self.exclude,
+            exclude_opt_key=self.exclude_opt_key,
+        ):
+            auth_result = await self.authenticate_request(ASGIConnection(scope))
+            scope["user"] = auth_result.user
+            scope["auth"] = auth_result.auth
+        await self.app(scope, receive, send)
+
+    @abstractmethod
+    async def authenticate_request(self, connection: ASGIConnection) -> AuthenticationResult:  # pragma: no cover
+        """Receive the http connection and return an :class:`AuthenticationResult`.
 
-        response = ASGIResponse(body=b'{"message":"invalid host header"}', status_code=HTTP_400_BAD_REQUEST)
-        await response(scope, receive, send)
+        Notes:
+            - This method must be overridden by subclasses.
+
+        Args:
+            connection: An :class:`ASGIConnection <litestar.connection.ASGIConnection>` instance.
+
+        Raises:
+            NotAuthorizedException | PermissionDeniedException: if authentication fails.
+
+        Returns:
+            An instance of :class:`AuthenticationResult <litestar.middleware.authentication.AuthenticationResult>`.
+        """
+        raise NotImplementedError("authenticate_request must be overridden by subclasses")
```

### Comparing `litestar-2.0.0b2/litestar/middleware/base.py` & `litestar-2.0.0b3/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/middleware/compression.py` & `litestar-2.0.0b3/litestar/middleware/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/middleware/cors.py` & `litestar-2.0.0b3/litestar/middleware/cors.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,18 @@
             receive: The ASGI receive function.
             send: The ASGI send function.
 
         Returns:
             None
         """
         headers = Headers.from_scope(scope=scope)
-        origin = headers.get("origin")
-
-        if not origin:
-            await self.app(scope, receive, send)
-        else:
+        if origin := headers.get("origin"):
             await self.app(scope, receive, self.send_wrapper(send=send, origin=origin, has_cookie="cookie" in headers))
+        else:
+            await self.app(scope, receive, send)
 
     def send_wrapper(self, send: Send, origin: str, has_cookie: bool) -> Send:
         """Wrap ``send`` to ensure that state is not disconnected.
 
         Args:
             has_cookie: Boolean flag dictating if the connection has a cookie set.
             origin: The value of the ``Origin`` header.
```

### Comparing `litestar-2.0.0b2/litestar/middleware/csrf.py` & `litestar-2.0.0b3/litestar/middleware/csrf.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,18 +168,15 @@
         """Decode a CSRF token and validate its HMAC."""
         if len(token) < CSRF_SECRET_LENGTH + 1:
             return None
 
         token_secret = token[:CSRF_SECRET_LENGTH]
         existing_hash = token[CSRF_SECRET_LENGTH:]
         expected_hash = generate_csrf_hash(token=token_secret, secret=self.config.secret)
-        if not compare_digest(existing_hash, expected_hash):
-            return None
-
-        return token_secret
+        return token_secret if compare_digest(existing_hash, expected_hash) else None
 
     def _csrf_tokens_match(self, request_csrf_token: str | None, cookie_csrf_token: str | None) -> bool:
         """Take the CSRF tokens from the request and the cookie and verify both are valid and identical."""
         if not (request_csrf_token and cookie_csrf_token):
             return False
 
         decoded_request_token = self._decode_csrf_token(request_csrf_token)
```

### Comparing `litestar-2.0.0b2/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.0.0b3/litestar/middleware/exceptions/_debug_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,18 +91,17 @@
         collapsed: Flag controlling whether frame should be collapsed on the page load.
 
     Returns:
         A string containing HTML representation of the execution frame.
     """
     frame_tpl = (tpl_dir / "frame.html").read_text()
 
-    code_lines: list[str] = []
-    for idx, line in enumerate(frame.code_context or []):
-        code_lines.append(create_line_html(line, frame.lineno, frame.index or 0, idx))  # pyright: ignore
-
+    code_lines: list[str] = [
+        create_line_html(line, frame.lineno, frame.index or 0, idx) for idx, line in enumerate(frame.code_context or [])
+    ]
     data = {
         "file": escape(frame.filename),
         "line": frame.lineno,
         "symbol_name": escape(get_symbol_name(frame)),
         "code": "".join(code_lines),
         "frame_class": "collapsed" if collapsed else "",
     }
@@ -116,18 +115,15 @@
         exc: An Exception instance to generate.
         line_limit: Number of lines of code context to return, which are centered around the executed line.
 
     Returns:
         A string containing HTML representation of the execution frames related to the exception.
     """
     frames = getinnerframes(exc.__traceback__, line_limit) if exc.__traceback__ else []
-    result = []
-    for idx, frame in enumerate(reversed(frames)):
-        result.append(create_frame_html(frame=frame, collapsed=idx > 0))
-
+    result = [create_frame_html(frame=frame, collapsed=idx > 0) for idx, frame in enumerate(reversed(frames))]
     return "".join(result)
 
 
 def create_html_response_content(exc: Exception, request: Request, line_limit: int = 15) -> str:
     """Given an exception, produces its traceback in HTML.
 
     Args:
```

### Comparing `litestar-2.0.0b2/litestar/middleware/exceptions/middleware.py` & `litestar-2.0.0b3/litestar/middleware/exceptions/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,20 +54,20 @@
         Optional exception handler callable.
     """
     if not exception_handlers:
         return None
     status_code: int | None = getattr(exc, "status_code", None)
     if status_code and (exception_handler := exception_handlers.get(status_code)):
         return exception_handler
-    for cls in getmro(type(exc)):
-        if cls in exception_handlers:
-            return exception_handlers[cast("Type[Exception]", cls)]
-    if not hasattr(exc, "status_code") and HTTP_500_INTERNAL_SERVER_ERROR in exception_handlers:
-        return exception_handlers[HTTP_500_INTERNAL_SERVER_ERROR]
-    return None
+    return next(
+        (exception_handlers[cast("Type[Exception]", cls)] for cls in getmro(type(exc)) if cls in exception_handlers),
+        exception_handlers[HTTP_500_INTERNAL_SERVER_ERROR]
+        if not hasattr(exc, "status_code") and HTTP_500_INTERNAL_SERVER_ERROR in exception_handlers
+        else None,
+    )
 
 
 @dataclass
 class ExceptionResponseContent:
     """Represent the contents of an exception-response."""
 
     status_code: int
```

### Comparing `litestar-2.0.0b2/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.0.0b3/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.0.0b3/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/middleware/logging.py` & `litestar-2.0.0b3/litestar/middleware/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,17 +157,15 @@
             value_strings = [f"{key}={value}" for key, value in values.items()]
             log_message = f"{message}: {', '.join(value_strings)}"
             self.logger.info(log_message)
 
     def _serialize_value(self, serializer: Serializer | None, value: Any) -> Any:
         if not self.is_struct_logger and isinstance(value, (dict, list, tuple, set)):
             value = encode_json(value, serializer)
-        if isinstance(value, bytes):
-            return value.decode("utf-8")
-        return value
+        return value.decode("utf-8") if isinstance(value, bytes) else value
 
     async def extract_request_data(self, request: Request) -> dict[str, Any]:
         """Create a dictionary of values for the message.
 
         Args:
             request: A :class:`Request <litestar.connection.Request>` instance.
```

### Comparing `litestar-2.0.0b2/litestar/middleware/rate_limit.py` & `litestar-2.0.0b3/litestar/middleware/rate_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         Returns:
             An :class:`CacheObject`.
         """
         duration = DURATION_VALUES[self.unit]
         now = int(time())
         cached_string = await store.get(key)
         if cached_string:
-            cache_object = CacheObject(**decode_json(cached_string))
+            cache_object = CacheObject(**decode_json(value=cached_string))
             if cache_object.reset <= now:
                 return CacheObject(history=[], reset=now + duration)
 
             while cache_object.history and cache_object.history[-1] <= now - duration:
                 cache_object.history.pop()
             return cache_object
```

### Comparing `litestar-2.0.0b2/litestar/middleware/session/base.py` & `litestar-2.0.0b3/litestar/middleware/session/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
         Args:
             data: Data to be deserialized
 
         Returns:
             Deserialized data as a dictionary
         """
-        return cast("dict[str, Any]", decode_json(data))
+        return cast("dict[str, Any]", decode_json(value=data))
 
     @abstractmethod
     async def store_in_message(self, scope_session: ScopeSession, message: Message, connection: ASGIConnection) -> None:
         """Store the necessary information in the outgoing ``Message``
 
         Args:
             scope_session: Current session to store
```

### Comparing `litestar-2.0.0b2/litestar/middleware/session/client_side.py` & `litestar-2.0.0b3/litestar/middleware/session/client_side.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         Returns:
             A deserialized session value.
         """
         decoded = b64decode(b"".join(data))
         nonce = decoded[:NONCE_SIZE]
         aad_starts_from = decoded.find(AAD)
         associated_data = decoded[aad_starts_from:].replace(AAD, b"") if aad_starts_from != -1 else None
-        if associated_data and decode_json(associated_data)["expires_at"] > round(time.time()):
+        if associated_data and decode_json(value=associated_data)["expires_at"] > round(time.time()):
             encrypted_session = decoded[NONCE_SIZE:aad_starts_from]
             decrypted = self.aesgcm.decrypt(nonce, encrypted_session, associated_data=associated_data)
             return self.deserialize_data(decrypted)
         return {}
 
     def get_cookie_keys(self, connection: ASGIConnection) -> list[str]:
         """Return a list of cookie-keys from the connection if they match the session-cookie pattern.
@@ -182,16 +182,15 @@
 
         Args:
             connection: Originating ASGIConnection
 
         Returns:
             The session data
         """
-        cookie_keys = self.get_cookie_keys(connection)
-        if cookie_keys:
+        if cookie_keys := self.get_cookie_keys(connection):
             data = [connection.cookies[key].encode("utf-8") for key in cookie_keys]
             # If these exceptions occur, the session must remain empty so do nothing.
             with contextlib.suppress(InvalidTag, binascii.Error):
                 return self.load_data(data)
         return {}
```

### Comparing `litestar-2.0.0b2/litestar/middleware/session/server_side.py` & `litestar-2.0.0b3/litestar/middleware/session/server_side.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,15 @@
 
         Args:
             connection: An ASGIConnection instance
 
         Returns:
             The current session data
         """
-        session_id = connection.cookies.get(self.config.key)
-        if session_id:
+        if session_id := connection.cookies.get(self.config.key):
             store = self.config.get_store_from_app(connection.scope["app"])
             data = await self.get(session_id, store=store)
             if data is not None:
                 return self.deserialize_data(data)
         return {}
```

### Comparing `litestar-2.0.0b2/litestar/openapi/config.py` & `litestar-2.0.0b3/litestar/openapi/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     OpenAPI,
     PathItem,
     Reference,
     SecurityRequirement,
     Server,
     Tag,
 )
+from litestar.utils.path import normalize_path
 
 __all__ = ("OpenAPIConfig",)
 
 
 if TYPE_CHECKING:
     from litestar.types.callable_types import OperationIDCreator
 
@@ -90,14 +91,21 @@
     """The static schema generator to use for the "root" path of `/schema/`."""
     enabled_endpoints: set[str] = field(
         default_factory=lambda: {"redoc", "swagger", "elements", "openapi.json", "openapi.yaml"}
     )
     """A set of the enabled documentation sites and schema download endpoints."""
     operation_id_creator: OperationIDCreator = default_operation_id_creator
     """A callable that generates unique operation ids"""
+    path: str | None = field(default=None)
+    """Base path for the OpenAPI documentation endpoints."""
+
+    def __post_init__(self) -> None:
+        if self.path:
+            self.path = normalize_path(self.path)
+            self.openapi_controller = type("OpenAPIController", (self.openapi_controller,), {"path": self.path})
 
     def to_openapi_schema(self) -> OpenAPI:
         """Return an ``OpenAPI`` instance from the values stored in ``self``.
 
         Returns:
             An instance of :class:`OpenAPI <litestar.openapi.spec.open_api.OpenAPI>`.
         """
```

### Comparing `litestar-2.0.0b2/litestar/openapi/controller.py` & `litestar-2.0.0b3/litestar/openapi/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
     path: str = "/schema"
     """Base path for the OpenAPI documentation endpoints."""
     style: str = "body { margin: 0; padding: 0 }"
     """Base styling of the html body."""
     redoc_version: str = "next"
     """Redoc version to download from the CDN."""
-    swagger_ui_version: str = "5.0.0"
+    swagger_ui_version: str = "5.1.3"
     """SwaggerUI version to download from the CDN."""
-    stoplight_elements_version: str = "7.7.5"
+    stoplight_elements_version: str = "7.7.18"
     """StopLight Elements version to download from the CDN."""
     favicon_url: str = ""
     """URL to download a favicon from."""
     redoc_google_fonts: bool = True
     """Download google fonts via CDN.
 
     Should be set to ``False`` when not using a CDN.
@@ -63,17 +63,14 @@
     )
     """Download url for the Stoplight Elements JS bundle."""
 
     # internal
     _dumped_schema: str = ""
     # until swagger-ui supports v3.1.* of OpenAPI officially, we need to modify the schema for it and keep it
     # separate from the redoc version of the schema, which is unmodified.
-    _dumped_modified_schema: str = ""
-    # set the dto types to `None` to ensure that if a dto is supplied at the application layer, they don't apply to
-    # this controller.
     dto = None
     return_dto = None
 
     @staticmethod
     def get_schema_from_request(request: Request[Any, Any, Any]) -> OpenAPI:
         """Return the OpenAPI pydantic model from the request instance.
 
@@ -106,18 +103,15 @@
         root_path = set(filter(None, self.path.split("/")))
 
         config = request.app.openapi_config
 
         if request_path == root_path and config.root_schema_site in config.enabled_endpoints:
             return True
 
-        if request_path & config.enabled_endpoints:
-            return True
-
-        return False
+        return bool(request_path & config.enabled_endpoints)
 
     @property
     def favicon(self) -> str:
         """Return favicon ``<link>`` tag, if applicable.
 
         Returns:
             A ``<link>`` tag if ``self.favicon_url`` is not empty, otherwise returns a placeholder meta tag.
```

### Comparing `litestar-2.0.0b2/litestar/openapi/datastructures.py` & `litestar-2.0.0b3/litestar/openapi/datastructures.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 from litestar.enums import MediaType
 
 if TYPE_CHECKING:
-    from litestar.types import DataclassProtocol, TypedDictClass
+    from litestar.types import DataContainerType
 
-    try:
-        from pydantic import BaseModel
-    except ImportError:
-        BaseModel = Any  # type: ignore
 
 __all__ = ("ResponseSpec",)
 
 
 @dataclass
 class ResponseSpec:
     """Container type of additional responses."""
 
-    data_container: type[BaseModel] | type[DataclassProtocol] | TypedDictClass
+    data_container: DataContainerType
     """A model that describes the content of the response."""
     generate_examples: bool = field(default=True)
     """Generate examples for the response content."""
     description: str = field(default="Additional response")
     """A description of the response."""
     media_type: MediaType = field(default=MediaType.JSON)
     """Response media type."""
```

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/__init__.py` & `litestar-2.0.0b3/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/base.py` & `litestar-2.0.0b3/litestar/openapi/spec/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,31 +11,27 @@
     if key.endswith("_in"):
         return "in"
     if key.startswith("schema_"):
         return key.split("_")[1]
     if "_" in key:
         components = key.split("_")
         return components[0] + "".join(component.title() for component in components[1:])
-    if key == "ref":
-        return "$ref"
-    return key
+    return "$ref" if key == "ref" else key
 
 
 def _normalize_value(value: Any) -> Any:
     if isinstance(value, BaseSchemaObject):
         return value.to_schema()
     if is_dataclass(value):
         return {_normalize_value(k): _normalize_value(v) for k, v in asdict(value).items() if v is not None}
     if isinstance(value, dict):
         return {_normalize_value(k): _normalize_value(v) for k, v in value.items() if v is not None}
     if isinstance(value, list):
         return [_normalize_value(v) for v in value]
-    if isinstance(value, Enum):
-        return value.value
-    return value
+    return value.value if isinstance(value, Enum) else value
 
 
 @dataclass
 class BaseSchemaObject:
     """Base class for schema spec objects"""
 
     def to_schema(self) -> dict[str, Any]:
```

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/callback.py` & `litestar-2.0.0b3/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/components.py` & `litestar-2.0.0b3/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/contact.py` & `litestar-2.0.0b3/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/discriminator.py` & `litestar-2.0.0b3/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/encoding.py` & `litestar-2.0.0b3/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/enums.py` & `litestar-2.0.0b3/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/example.py` & `litestar-2.0.0b3/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/external_documentation.py` & `litestar-2.0.0b3/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/header.py` & `litestar-2.0.0b3/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/info.py` & `litestar-2.0.0b3/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/license.py` & `litestar-2.0.0b3/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/link.py` & `litestar-2.0.0b3/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/media_type.py` & `litestar-2.0.0b3/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/oauth_flow.py` & `litestar-2.0.0b3/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/oauth_flows.py` & `litestar-2.0.0b3/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/open_api.py` & `litestar-2.0.0b3/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/operation.py` & `litestar-2.0.0b3/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/parameter.py` & `litestar-2.0.0b3/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/path_item.py` & `litestar-2.0.0b3/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/paths.py` & `litestar-2.0.0b3/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/reference.py` & `litestar-2.0.0b3/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/request_body.py` & `litestar-2.0.0b3/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/response.py` & `litestar-2.0.0b3/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/responses.py` & `litestar-2.0.0b3/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/schema.py` & `litestar-2.0.0b3/litestar/openapi/spec/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from litestar.openapi.spec.discriminator import Discriminator
     from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
     from litestar.openapi.spec.external_documentation import ExternalDocumentation
     from litestar.openapi.spec.reference import Reference
     from litestar.openapi.spec.xml import XML
     from litestar.types import DataclassProtocol
 
-__all__ = ("Schema",)
+__all__ = ("Schema", "SchemaDataContainer")
 
 
 def _recursive_hash(value: Hashable | Sequence | Mapping | DataclassProtocol | type[DataclassProtocol]) -> int:
     if isinstance(value, Mapping):
         hash_value = 0
         for k, v in value.items():
             if k != "examples":
@@ -30,17 +30,15 @@
         for field in fields(value):
             if field.name != "examples":
                 hash_value += hash(field.name)
                 hash_value += _recursive_hash(getattr(value, field.name, None))
         return hash_value
     if is_non_string_sequence(value):
         return sum(_recursive_hash(v) for v in value)
-    if isinstance(value, Hashable):
-        return hash(value)
-    return 0
+    return hash(value) if isinstance(value, Hashable) else 0
 
 
 @dataclass
 class Schema(BaseSchemaObject):
     """The Schema Object allows the definition of input and output data types. These types can be objects, but also
     primitives and arrays. This object is a superset of the
     `JSON Schema Specification Draft 2020-12 <https://tools.ietf.org/html/draft-bhutton-json-schema-00>`_.
```

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/security_requirement.py` & `litestar-2.0.0b3/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/security_scheme.py` & `litestar-2.0.0b3/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/server.py` & `litestar-2.0.0b3/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/server_variable.py` & `litestar-2.0.0b3/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/tag.py` & `litestar-2.0.0b3/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/openapi/spec/xml.py` & `litestar-2.0.0b3/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/pagination.py` & `litestar-2.0.0b3/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/params.py` & `litestar-2.0.0b3/litestar/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, field
-from typing import TYPE_CHECKING, Any, Hashable
+from typing import TYPE_CHECKING, Any, Hashable, Sequence
 
 from litestar.enums import RequestEncodingType
 from litestar.types import Empty
 
 __all__ = (
     "Body",
     "BodyKwarg",
@@ -102,14 +102,18 @@
 
     Equivalent to pattern in the OpenAPI specification.
     """
     lower_case: bool | None = field(default=None)
     """Constrict a string value to be lower case."""
     upper_case: bool | None = field(default=None)
     """Constrict a string value to be upper case."""
+    format: str | None = field(default=None)
+    """Specify the format to which a string value should be converted."""
+    enum: Sequence[Any] | None = field(default=None)
+    """A sequence of valid values."""
 
     @property
     def is_constrained(self) -> bool:
         """Return True if any of the constraints are set."""
         return any(
             attr if attr and attr is not Empty else False  # type: ignore[comparison-overlap]
             for attr in (
@@ -130,15 +134,15 @@
         )
 
 
 @dataclass(frozen=True)
 class ParameterKwarg(KwargDefinition):
     """Data container representing a parameter."""
 
-    value_type: Any = field(default=Empty)
+    annotation: Any = field(default=Empty)
     """The field value - `Empty` by default."""
     header: str | None = field(default=None)
     """The header parameter key - required for header parameters."""
     cookie: str | None = field(default=None)
     """The cookie parameter key - required for cookie parameters."""
     query: str | None = field(default=None)
     """The query parameter key for this parameter."""
@@ -154,15 +158,15 @@
         Returns:
             A hash
         """
         return sum(hash(v) for v in asdict(self) if isinstance(v, Hashable))
 
 
 def Parameter(
-    value_type: Any = Empty,
+    annotation: Any = Empty,
     *,
     const: bool | None = None,
     content_encoding: str | None = None,
     cookie: str | None = None,
     default: Any = Empty,
     description: str | None = None,
     examples: list[Example] | None = None,
@@ -181,15 +185,15 @@
     query: str | None = None,
     required: bool | None = None,
     title: str | None = None,
 ) -> Any:
     """Create an extended parameter kwarg definition.
 
     Args:
-        value_type: `Empty` by default.
+        annotation: `Empty` by default.
         const: A boolean flag dictating whether this parameter is a constant. If True, the value passed to the parameter
             must equal its default value. This also causes the OpenAPI const field
             to be populated with the default value.
         content_encoding: The content encoding of the value.
             Applicable on to string values. See OpenAPI 3.1 for details.
         cookie: The cookie parameter key - required for cookie parameters.
         default: A default value. If const is true, this value is required.
@@ -219,15 +223,15 @@
             Equivalent to pattern in the OpenAPI specification.
         query: The query parameter key for this parameter.
         required: A boolean flag dictating whether this parameter is required.
             If set to False, None values will be allowed. Defaults to True.
         title: String value used in the title section of the OpenAPI schema for the given parameter.
     """
     return ParameterKwarg(
-        value_type=value_type,
+        annotation=annotation,
         header=header,
         cookie=cookie,
         query=query,
         examples=examples,
         external_docs=external_docs,
         content_encoding=content_encoding,
         required=required,
```

### Comparing `litestar-2.0.0b2/litestar/partial.py` & `litestar-2.0.0b3/litestar/partial.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,37 +5,35 @@
     TYPE_CHECKING,
     Any,
     Generic,
     Optional,
     Type,
     TypeVar,
     Union,
-    get_type_hints,
 )
 
 import msgspec
-from typing_extensions import TypeAlias, TypedDict
+from typing_extensions import TypeAlias, TypedDict, get_type_hints
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types.builtin_types import NoneType
+from litestar.utils import warn_deprecation
 from litestar.utils.predicates import (
     is_attrs_class,
     is_class_var,
     is_dataclass_class,
     is_pydantic_model_class,
     is_struct_class,
     is_typed_dict,
 )
 
 if TYPE_CHECKING:
     import attrs
     import pydantic
 
-__all__ = ("Partial",)
-
 try:
     # python 3.9 changed these variable
     from typing import _UnionGenericAlias as GenericAlias  # type: ignore
 except ImportError:  # pragma: no cover
     from typing import _GenericAlias as GenericAlias  # type: ignore
 
 if TYPE_CHECKING:
@@ -51,20 +49,20 @@
 def _create_partial_type_name(item: SupportedTypes) -> str:
     return f"Partial{item.__name__}"
 
 
 def _extract_type_hints(item: Any) -> tuple[tuple[str, Any], ...]:
     return tuple(
         (field_name, field_type)
-        for field_name, field_type in get_type_hints(item).items()
+        for field_name, field_type in get_type_hints(item, include_extras=True).items()
         if not is_class_var(field_type)
     )
 
 
-class Partial(Generic[T]):
+class _Partial(Generic[T]):
     """Partial is a special typing helper that takes a generic T, and
     returns to static type checkers a version of this T in which all fields -
     and nested fields - are optional.
     """
 
     _models: dict[SupportedTypes, SupportedTypes] = {}
 
@@ -101,36 +99,34 @@
         """Receives a pydantic model class and creates an all optional subclass of it.
 
         Args:
             item: A pydantic model class.
         """
         import pydantic
 
-        field_definitions: dict[str, tuple[Any, None]] = {}
-        for field_name, field_type in _extract_type_hints(item):
-            if not isinstance(field_type, GenericAlias) or NoneType not in field_type.__args__:
-                field_definitions[field_name] = (Optional[field_type], None)
-            else:
-                field_definitions[field_name] = (field_type, None)
-
+        field_definitions: dict[str, tuple[Any, None]] = {
+            field_name: (Optional[field_type], None)
+            if not isinstance(field_type, GenericAlias) or NoneType not in field_type.__args__
+            else (field_type, None)
+            for field_name, field_type in _extract_type_hints(item)
+        }
         cls._models[item] = pydantic.create_model(
             _create_partial_type_name(item), __base__=item, **field_definitions  # pyright: ignore
         )  # type: ignore
 
     @classmethod
     def _create_partial_attrs_model(cls, item: type[attrs.AttrsInstance]) -> None:
         import attrs
 
-        field_definitions: dict[str, Any] = {}
-        for field_name, field_type in _extract_type_hints(item):
-            if not isinstance(field_type, GenericAlias) or NoneType not in field_type.__args__:
-                field_definitions[field_name] = Optional[field_type]
-            else:
-                field_definitions[field_name] = field_type
-
+        field_definitions: dict[str, Any] = {
+            field_name: Optional[field_type]
+            if not isinstance(field_type, GenericAlias) or NoneType not in field_type.__args__
+            else field_type
+            for field_name, field_type in _extract_type_hints(item)
+        }
         cls._models[item] = attrs.define(
             type(
                 _create_partial_type_name(item),
                 (item,),
                 {"__annotations__": field_definitions, **{k: None for k in field_definitions}},
             )
         )
@@ -157,20 +153,20 @@
     @classmethod
     def _create_partial_typeddict(cls, item: TypedDictClass) -> None:
         """Receives a typeddict class and creates a new type with all attributes ``Optional``.
 
         Args:
             item: A :class:`TypedDict <typing.TypeDict>` class.
         """
-        field_definitions: dict[str, Any] = {}
-        for field_name, field_type in _extract_type_hints(item):
-            if not isinstance(field_type, GenericAlias) or NoneType not in field_type.__args__:
-                field_definitions[field_name] = Optional[field_type]
-            else:
-                field_definitions[field_name] = field_type
+        field_definitions: dict[str, Any] = {
+            field_name: Optional[field_type]
+            if not isinstance(field_type, GenericAlias) or NoneType not in field_type.__args__
+            else field_type
+            for field_name, field_type in _extract_type_hints(item)
+        }
         cls._models[item] = TypedDict(_create_partial_type_name(item), field_definitions, total=False)  # type: ignore
 
     @classmethod
     def _create_partial_struct(cls, item: type[msgspec.Struct]) -> None:
         """Receives a :class:`Struct <msgspec.Struct> class and creates a new type with all attributes ``Optional``.
 
         Args:
@@ -183,7 +179,22 @@
             else:
                 field_definitions.append((field_name, field_type, None))
         cls._models[item] = msgspec.defstruct(
             name=_create_partial_type_name(item),
             fields=field_definitions,
             bases=(item,),
         )
+
+
+def __getattr__(attr_name: str) -> object:
+    if "Partial" in attr_name:
+        warn_deprecation(
+            deprecated_name="litestar.partial.Partial",
+            version="2.0b3",
+            kind="class",
+            removal_in="2.0",
+            info="the 'Partial' class is deprecated, please use a partial DTO instead",
+        )
+
+        globals()[attr_name] = _Partial
+        return _Partial
+    raise AttributeError(f"module {__name__!r} has no attribute {attr_name!r}")
```

### Comparing `litestar-2.0.0b2/litestar/plugins.py` & `litestar-2.0.0b3/litestar/plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Protocol, TypedDict, TypeVar, Union, runtime_checkable
-
-from pydantic import BaseModel
-
-from litestar.types.protocols import DataclassProtocol
+from typing import TYPE_CHECKING, Any, Protocol, TypeVar, Union, runtime_checkable
 
 if TYPE_CHECKING:
-    from typing_extensions import TypeGuard
-
+    from litestar._openapi.schema_generation import SchemaCreator
     from litestar.config.app import AppConfig
     from litestar.dto.interface import DTOInterface
+    from litestar.dto.types import ForType
     from litestar.openapi.spec import Schema
-    from litestar.typing import ParsedType
+    from litestar.typing import FieldDefinition
+
 
 __all__ = ("SerializationPluginProtocol", "InitPluginProtocol", "OpenAPISchemaPluginProtocol", "PluginProtocol")
 
-ModelT = TypeVar("ModelT")
-DataContainerT = TypeVar("DataContainerT", bound=Union[BaseModel, DataclassProtocol, TypedDict])  # type: ignore[valid-type]
+
+T = TypeVar("T")
 
 
 @runtime_checkable
 class InitPluginProtocol(Protocol):
     """Protocol used to define plugins that affect the application's init process."""
 
     __slots__ = ()
@@ -61,60 +58,62 @@
 
 @runtime_checkable
 class SerializationPluginProtocol(Protocol):
     """Protocol used to define a serialization plugin for DTOs."""
 
     __slots__ = ()
 
-    def supports_type(self, parsed_type: ParsedType) -> bool:
+    def supports_type(self, field_definition: FieldDefinition) -> bool:
         """Given a value of indeterminate type, determine if this value is supported by the plugin.
 
         Args:
-            parsed_type: A parsed type.
+            field_definition: A parsed type.
 
         Returns:
             Whether the type is supported by the plugin.
         """
         raise NotImplementedError()
 
-    def create_dto_for_type(self, parsed_type: ParsedType) -> type[DTOInterface]:
+    def create_dto_for_type(self, field_definition: FieldDefinition) -> type[DTOInterface]:
         """Given a parsed type, create a DTO class.
 
         Args:
-            parsed_type: A parsed type.
+            field_definition: A parsed type.
 
         Returns:
             A DTO class.
         """
         raise NotImplementedError()
 
 
 @runtime_checkable
-class OpenAPISchemaPluginProtocol(Protocol[ModelT]):
+class OpenAPISchemaPluginProtocol(Protocol):
     """Plugin to extend the support of OpenAPI schema generation for non-library types."""
 
     __slots__ = ()
 
     @staticmethod
-    def is_plugin_supported_type(value: Any) -> TypeGuard[ModelT]:
+    def is_plugin_supported_type(value: Any) -> bool:
         """Given a value of indeterminate type, determine if this value is supported by the plugin.
 
         Args:
             value: An arbitrary value.
 
         Returns:
             A typeguard dictating whether the value is supported by the plugin.
         """
         raise NotImplementedError()
 
-    def to_openapi_schema(self, model_class: type[ModelT]) -> Schema:
-        """Given a model class, transform it into an OpenAPI schema class.
+    def to_openapi_schema(self, annotation: Any, schema_creator: SchemaCreator, dto_for: ForType | None) -> Schema:
+        """Given a type annotation, transform it into an OpenAPI schema class.
 
         Args:
-            model_class: A model class.
+            annotation: A type annotation.
+            schema_creator: An instance of the openapi SchemaCreator.
+            dto_for: The type of the DTO if any.
 
         Returns:
             An :class:`OpenAPI <litestar.openapi.spec.schema.Schema>` instance.
         """
         raise NotImplementedError()
```

### Comparing `litestar-2.0.0b2/litestar/response/base.py` & `litestar-2.0.0b3/litestar/response/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,21 +72,20 @@
             headers: The response headers.
             is_head_response: A boolean indicating if the response is a HEAD response.
             media_type: The response media type.
             status_code: The response status code.
         """
         body = body.encode() if isinstance(body, str) else body
         status_code = status_code or HTTP_200_OK
-        cookies = cookies or []
         encoded_headers = encoded_headers or []
         headers = headers or {}
         media_type = get_enum_string_value(media_type or MediaType.JSON)
 
-        status_allows_body = not (
-            status_code in {HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED} or status_code < HTTP_200_OK
+        status_allows_body = (
+            status_code not in {HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED} and status_code >= HTTP_200_OK
         )
 
         if not status_allows_body or is_head_response:
             if body and body != b"null":
                 raise ImproperlyConfiguredException(
                     "response content is not supported for HEAD responses and responses with a status code "
                     "that does not allow content (304, 204, < 200)"
@@ -107,14 +106,15 @@
 
         if "content-length" not in headers and content_length:
             encoded_headers.append((b"content-length", str(content_length).encode("latin-1")))
 
         self.background = background
         self.body = body
         self.content_length = content_length
+        cookies = cookies or []
         self.encoded_headers = encode_headers(headers.items(), cookies, encoded_headers)
         self.encoding = encoding
         self.is_head_response = is_head_response
         self.status_code = status_code
 
     async def after_response(self) -> None:
         """Execute after the response is sent.
```

### Comparing `litestar-2.0.0b2/litestar/response/file.py` & `litestar-2.0.0b3/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/response/redirect.py` & `litestar-2.0.0b3/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/response/streaming.py` & `litestar-2.0.0b3/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/response/template.py` & `litestar-2.0.0b3/litestar/response/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         headers = {**headers, **self.headers} if headers is not None else self.headers
         cookies = self.cookies if cookies is None else filter_cookies(self.cookies, cookies)
 
         media_type = self.media_type or media_type
         if not media_type:
             suffixes = PurePath(self.template_name).suffixes
             for suffix in suffixes:
-                if _type := guess_type("name" + suffix)[0]:
+                if _type := guess_type(f"name{suffix}")[0]:
                     media_type = _type
                     break
             else:
                 media_type = MediaType.TEXT
 
         template = app.template_engine.get_template(self.template_name)
         context = self.create_template_context(request)
```

### Comparing `litestar-2.0.0b2/litestar/router.py` & `litestar-2.0.0b3/litestar/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         ParametersMap,
         ResponseCookies,
         ResponseType,
         RouteHandlerMapItem,
         RouteHandlerType,
         TypeEncodersMap,
     )
-    from litestar.types.composite_types import Dependencies, ResponseHeaders
+    from litestar.types.composite_types import Dependencies, ResponseHeaders, TypeDecodersSequence
     from litestar.types.empty import EmptyType
 
 
 class Router:
     """The Litestar Router class.
 
     A Router instance is used to group controller, routers and route handler functions under a shared path fragment
@@ -69,14 +69,15 @@
         "response_headers",
         "return_dto",
         "routes",
         "security",
         "signature_namespace",
         "tags",
         "type_encoders",
+        "type_decoders",
     )
 
     def __init__(
         self,
         path: str,
         *,
         after_request: AfterRequestHookHandler | None = None,
@@ -96,14 +97,15 @@
         response_headers: ResponseHeaders | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         route_handlers: Sequence[ControllerRouterHandler],
         security: Sequence[SecurityRequirement] | None = None,
         signature_namespace: Mapping[str, Any] | None = None,
         tags: Sequence[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
+        type_decoders: TypeDecodersSequence | None = None,
     ) -> None:
         """Initialize a ``Router``.
 
         Args:
             after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
                 to any route handler. If this function returns a value, the request will not reach the route handler,
                 and instead this value will be used.
@@ -142,14 +144,15 @@
             security: A sequence of dicts that will be added to the schema of all route handlers in the application.
                 See :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>`
                 for details.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             tags: A sequence of string tags that will be appended to the schema of all route handlers under the
                 application.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
+            type_decoders: A sequence of tuples, each composed of a predicate testing for type identity and a msgspec hook for deserialization.
         """
 
         self.after_request = AsyncCallable(after_request) if after_request else None  # type: ignore[arg-type]
         self.after_response = AsyncCallable(after_response) if after_response else None
         self.before_request = AsyncCallable(before_request) if before_request else None
         self.cache_control = cache_control
         self.dto = dto
@@ -168,14 +171,15 @@
         self.return_dto = return_dto
         self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
         self.security = list(security or [])
         self.signature_namespace = signature_namespace or {}
         self.tags = list(tags or [])
         self.registered_route_handler_ids: set[int] = set()
         self.type_encoders = dict(type_encoders) if type_encoders is not None else None
+        self.type_decoders = list(type_decoders) if type_decoders is not None else None
 
         for route_handler in route_handlers or []:
             self.register(value=route_handler)
 
     def register(self, value: ControllerRouterHandler) -> list[BaseRoute]:
         """Register a Controller, Route instance or RouteHandler on the router.
 
@@ -287,15 +291,15 @@
 
     def _validate_registration_value(self, value: ControllerRouterHandler) -> Controller | RouteHandlerType | Router:
         """Ensure values passed to the register method are supported."""
         if is_class_and_subclass(value, Controller):
             return value(owner=self)
 
         # this narrows down to an ABC, but we assume a non-abstract subclass of the ABC superclass
-        if is_class_and_subclass(value, WebsocketListener):  # type: ignore[type-abstract]
+        if is_class_and_subclass(value, WebsocketListener):
             return value(owner=self).to_handler()  # pyright: ignore
 
         if isinstance(value, Router):
             if value.owner:
                 raise ImproperlyConfiguredException(f"Router with path {value.path} has already been registered")
 
             if value is self:
```

### Comparing `litestar-2.0.0b2/litestar/routes/asgi.py` & `litestar-2.0.0b3/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/routes/base.py` & `litestar-2.0.0b3/litestar/routes/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,47 @@
 from abc import ABC, abstractmethod
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable
 from uuid import UUID
 
-from pydantic.datetime_parse import (
-    parse_date,
-    parse_datetime,
-    parse_duration,
-    parse_time,
-)
+import msgspec
 
 from litestar._kwargs import KwargsModel
 from litestar._signature import get_signature_model
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types.internal_types import PathParameterDefinition
 from litestar.utils import join_paths, normalize_path
 
 if TYPE_CHECKING:
     from litestar.enums import ScopeType
     from litestar.handlers.base import BaseRouteHandler
     from litestar.types import Method, Receive, Scope, Send
 
+
+def _parse_datetime(value: str) -> datetime:
+    return msgspec.convert(value, datetime)
+
+
+def _parse_date(value: str) -> date:
+    return msgspec.convert(value, date)
+
+
+def _parse_time(value: str) -> time:
+    return msgspec.convert(value, time)
+
+
+def _parse_timedelta(value: str) -> timedelta:
+    try:
+        return msgspec.convert(value, timedelta)
+    except msgspec.ValidationError:
+        return timedelta(seconds=int(float(value)))
+
+
 param_match_regex = re.compile(r"{(.*?)}")
 
 param_type_map = {
     "str": str,
     "int": int,
     "float": float,
     "uuid": UUID,
@@ -43,18 +58,18 @@
 
 
 parsers_map: dict[Any, Callable[[Any], Any]] = {
     float: float,
     int: int,
     Decimal: Decimal,
     UUID: UUID,
-    date: parse_date,
-    datetime: parse_datetime,
-    time: parse_time,
-    timedelta: parse_duration,
+    date: _parse_date,
+    datetime: _parse_datetime,
+    time: _parse_time,
+    timedelta: _parse_timedelta,
 }
 
 
 class BaseRoute(ABC):
     """Base Route class used by Litestar.
 
     It's an abstract class meant to be extended.
@@ -124,24 +139,23 @@
             dependencies=route_handler.resolve_dependencies(),
             path_parameters=path_parameters,
             layered_parameters=route_handler.resolve_layered_parameters(),
             data_dto=route_handler.resolve_dto(),
         )
 
     @staticmethod
-    def _validate_path_parameter(param: str) -> None:
+    def _validate_path_parameter(param: str, path: str) -> None:
         """Validate that a path parameter adheres to the required format and datatypes.
 
         Raises:
             ImproperlyConfiguredException: If the parameter has an invalid format.
         """
         if len(param.split(":")) != 2:
             raise ImproperlyConfiguredException(
-                "Path parameters should be declared with a type using the following pattern: '{parameter_name:type}', "
-                "e.g. '/my-path/{my_param:int}'"
+                f"Path parameters should be declared with a type using the following pattern: '{{parameter_name:type}}', e.g. '/my-path/{{my_param:int}}' in path: '{path}'"
             )
         param_name, param_type = (p.strip() for p in param.split(":"))
         if not param_name:
             raise ImproperlyConfiguredException("Path parameter names should be of length greater than zero")
         if param_type not in param_type_map:
             raise ImproperlyConfiguredException(
                 f"Path parameters should be declared with an allowed type, i.e. one of {','.join(param_type_map.keys())}"
@@ -160,18 +174,17 @@
         path = normalize_path(path)
 
         parsed_components: list[str | PathParameterDefinition] = []
         path_format_components = []
 
         components = [component for component in path.split("/") if component]
         for component in components:
-            param_match = param_match_regex.fullmatch(component)
-            if param_match:
+            if param_match := param_match_regex.fullmatch(component):
                 param = param_match.group(1)
-                cls._validate_path_parameter(param)
+                cls._validate_path_parameter(param, path)
                 param_name, param_type = (p.strip() for p in param.split(":"))
                 type_class = param_type_map[param_type]
                 parser = parsers_map[type_class] if type_class not in {str, Path} else None
                 parsed_components.append(
                     PathParameterDefinition(name=param_name, type=type_class, full=param, parser=parser)
                 )
                 path_format_components.append("{" + param_name + "}")
```

### Comparing `litestar-2.0.0b2/litestar/routes/http.py` & `litestar-2.0.0b3/litestar/routes/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,39 +176,38 @@
 
         if parameter_model.has_kwargs and route_handler.signature_model:
             kwargs = parameter_model.to_kwargs(connection=request)
 
             if "data" in kwargs:
                 try:
                     kwargs["data"] = await kwargs["data"]
-                except SerializationException as exc:
-                    raise ClientException(str(exc)) from exc
+                except SerializationException as e:
+                    raise ClientException(str(e)) from e
 
             if "body" in kwargs:
                 kwargs["body"] = await kwargs["body"]
 
             if parameter_model.dependency_batches:
                 cleanup_group = await parameter_model.resolve_dependencies(request, kwargs)
 
             parsed_kwargs = route_handler.signature_model.parse_values_from_connection_kwargs(
                 connection=request, **kwargs
             )
 
         if cleanup_group:
             async with cleanup_group:
-                if route_handler.has_sync_callable:
-                    data = route_handler.fn.value(**parsed_kwargs)
-                else:
-                    data = await route_handler.fn.value(**parsed_kwargs)
-
+                data = (
+                    route_handler.fn.value(**parsed_kwargs)
+                    if route_handler.has_sync_callable
+                    else await route_handler.fn.value(**parsed_kwargs)
+                )
+        elif route_handler.has_sync_callable:
+            data = route_handler.fn.value(**parsed_kwargs)
         else:
-            if route_handler.has_sync_callable:
-                data = route_handler.fn.value(**parsed_kwargs)
-            else:
-                data = await route_handler.fn.value(**parsed_kwargs)
+            data = await route_handler.fn.value(**parsed_kwargs)
 
         return data, cleanup_group
 
     @staticmethod
     async def _get_cached_response(request: Request, route_handler: HTTPRouteHandler) -> ASGIApp | None:
         """Retrieve and un-pickle the cached response, if existing.
```

### Comparing `litestar-2.0.0b2/litestar/routes/websocket.py` & `litestar-2.0.0b3/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/security/base.py` & `litestar-2.0.0b3/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/security/session_auth/auth.py` & `litestar-2.0.0b3/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/security/session_auth/middleware.py` & `litestar-2.0.0b3/litestar/security/session_auth/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Awaitable
+from typing import TYPE_CHECKING, Any
 
 from litestar.exceptions import NotAuthorizedException
 from litestar.middleware.authentication import (
     AbstractAuthenticationMiddleware,
     AuthenticationResult,
 )
 from litestar.middleware.exceptions import ExceptionHandlerMiddleware
@@ -75,15 +75,15 @@
 
     def __init__(
         self,
         app: ASGIApp,
         exclude: str | list[str] | None,
         exclude_opt_key: str,
         scopes: Scopes | None,
-        retrieve_user_handler: AsyncCallable[[dict[str, Any], ASGIConnection[Any, Any, Any, Any]], Awaitable[Any]],
+        retrieve_user_handler: AsyncCallable[[dict[str, Any], ASGIConnection[Any, Any, Any, Any]], Any],
     ) -> None:
         """Session based authentication middleware.
 
         Args:
             app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
             exclude: A pattern or list of patterns to skip in the authentication middleware.
             exclude_opt_key: An identifier to use on routes to disable authentication and authorization checks for a particular route.
```

### Comparing `litestar-2.0.0b2/litestar/serialization.py` & `litestar-2.0.0b3/litestar/serialization/msgspec_hooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,284 +1,265 @@
 from __future__ import annotations
 
 from collections import deque
+from datetime import date, datetime, time
 from decimal import Decimal
 from functools import partial
 from ipaddress import (
     IPv4Address,
     IPv4Interface,
     IPv4Network,
     IPv6Address,
     IPv6Interface,
     IPv6Network,
 )
 from pathlib import Path, PurePath
 from re import Pattern
 from typing import TYPE_CHECKING, Any, Callable, Mapping, TypeVar, overload
+from uuid import UUID
 
 import msgspec
-from pydantic import (
-    BaseModel,
-    ByteSize,
-    ConstrainedBytes,
-    ConstrainedDate,
-    NameEmail,
-    SecretField,
-    StrictBool,
-)
-from pydantic.color import Color
-from pydantic.json import decimal_encoder
 
-from litestar.enums import MediaType
 from litestar.exceptions import SerializationException
-from litestar.types import Empty, Serializer
+from litestar.types import Empty, EmptyType, Serializer, TypeDecodersSequence
 
 if TYPE_CHECKING:
     from litestar.types import TypeEncodersMap
 
 __all__ = (
-    "dec_hook",
     "decode_json",
-    "decode_media_type",
     "decode_msgpack",
+    "default_deserializer",
     "default_serializer",
     "encode_json",
     "encode_msgpack",
     "get_serializer",
 )
 
 T = TypeVar("T")
 
-
-def _enc_base_model(model: BaseModel) -> Any:
-    return model.dict()
-
-
-def _enc_byte_size(bytes_: ByteSize) -> int:
-    return bytes_.real
-
-
-def _enc_constrained_bytes(bytes_: ConstrainedBytes) -> str:
-    return bytes_.decode("utf-8")
-
-
-def _enc_constrained_date(date: ConstrainedDate) -> str:
-    return date.isoformat()
-
-
-def _enc_pattern(pattern: Pattern) -> Any:
-    return pattern.pattern
-
-
 DEFAULT_TYPE_ENCODERS: TypeEncodersMap = {
     Path: str,
     PurePath: str,
-    # pydantic specific types
-    BaseModel: _enc_base_model,
-    ByteSize: _enc_byte_size,
-    NameEmail: str,
-    Color: str,
-    SecretField: str,
-    ConstrainedBytes: _enc_constrained_bytes,
-    ConstrainedDate: _enc_constrained_date,
     IPv4Address: str,
     IPv4Interface: str,
     IPv4Network: str,
     IPv6Address: str,
     IPv6Interface: str,
     IPv6Network: str,
-    # pydantic compatibility
+    datetime: lambda val: val.isoformat(),
+    date: lambda val: val.isoformat(),
+    time: lambda val: val.isoformat(),
     deque: list,
-    Decimal: decimal_encoder,
-    StrictBool: int,
-    Pattern: _enc_pattern,
+    Decimal: lambda val: int(val) if val.as_tuple().exponent >= 0 else float(val),
+    Pattern: lambda val: val.pattern,
     # support subclasses of stdlib types, If no previous type matched, these will be
     # the last type in the mro, so we use this to (attempt to) convert a subclass into
     # its base class. # see https://github.com/jcrist/msgspec/issues/248
     # and https://github.com/litestar-org/litestar/issues/1003
     str: str,
     int: int,
     float: float,
     set: set,
     frozenset: frozenset,
+    bytes: bytes,
 }
 
 
 def default_serializer(value: Any, type_encoders: Mapping[Any, Callable[[Any], Any]] | None = None) -> Any:
     """Transform values non-natively supported by ``msgspec``
 
     Args:
         value: A value to serialized
         type_encoders: Mapping of types to callables to transforming types
     Returns:
         A serialized value
     Raises:
         TypeError: if value is not supported
     """
-    if type_encoders is None:
-        type_encoders = DEFAULT_TYPE_ENCODERS
+    type_encoders = {**DEFAULT_TYPE_ENCODERS, **(type_encoders or {})}
+
     for base in value.__class__.__mro__[:-1]:
         try:
             encoder = type_encoders[base]
+            return encoder(value)
         except KeyError:
             continue
-        return encoder(value)
+
     raise TypeError(f"Unsupported type: {type(value)!r}")
 
 
-def dec_hook(type_: Any, value: Any) -> Any:  # pragma: no cover
+def default_deserializer(
+    target_type: Any, value: Any, type_decoders: TypeDecodersSequence | None = None
+) -> Any:  # pragma: no cover
     """Transform values non-natively supported by ``msgspec``
 
     Args:
-        type_: Encountered type
+        target_type: Encountered type
         value: Value to coerce
+        type_decoders: Optional sequence of type decoders
 
     Returns:
         A ``msgspec``-supported type
     """
-    if issubclass(type_, BaseModel):
-        return type_.parse_obj(value)
-    if issubclass(type_, (Path, PurePath)):
-        return type_(value)
+
+    from litestar.datastructures.state import ImmutableState
+
+    if isinstance(value, target_type):
+        return value
+
+    if type_decoders:
+        for predicate, decoder in type_decoders:
+            if predicate(target_type):
+                return decoder(target_type, value)
+
+    if issubclass(target_type, (Path, PurePath, ImmutableState, UUID)):
+        return target_type(value)
+
     raise TypeError(f"Unsupported type: {type(value)!r}")
 
 
 _msgspec_json_encoder = msgspec.json.Encoder(enc_hook=default_serializer)
-_msgspec_json_decoder = msgspec.json.Decoder(dec_hook=dec_hook)
+_msgspec_json_decoder = msgspec.json.Decoder(dec_hook=default_deserializer)
 _msgspec_msgpack_encoder = msgspec.msgpack.Encoder(enc_hook=default_serializer)
-_msgspec_msgpack_decoder = msgspec.msgpack.Decoder(dec_hook=dec_hook)
+_msgspec_msgpack_decoder = msgspec.msgpack.Decoder(dec_hook=default_deserializer)
 
 
-def encode_json(obj: Any, default: Callable[[Any], Any] | None = default_serializer) -> bytes:
+def encode_json(value: Any, serializer: Callable[[Any], Any] | None = None) -> bytes:
     """Encode a value into JSON.
 
     Args:
-        obj: Value to encode
-        default: Optional callable to support non-natively supported types.
+        value: Value to encode
+        serializer: Optional callable to support non-natively supported types.
 
     Returns:
         JSON as bytes
 
     Raises:
         SerializationException: If error encoding ``obj``.
     """
     try:
-        if default is None or default is default_serializer:
-            return _msgspec_json_encoder.encode(obj)
-        return msgspec.json.encode(obj, enc_hook=default)
+        return msgspec.json.encode(value, enc_hook=serializer) if serializer else _msgspec_json_encoder.encode(value)
     except (TypeError, msgspec.EncodeError) as msgspec_error:
         raise SerializationException(str(msgspec_error)) from msgspec_error
 
 
 @overload
-def decode_json(raw: str | bytes) -> Any:
+def decode_json(value: str | bytes) -> Any:
+    ...
+
+
+@overload
+def decode_json(value: str | bytes, type_decoders: TypeDecodersSequence | None) -> Any:
     ...
 
 
 @overload
-def decode_json(raw: str | bytes, type_: type[T]) -> T:
+def decode_json(value: str | bytes, target_type: type[T]) -> T:
     ...
 
 
-def decode_json(raw: str | bytes, type_: Any = Empty) -> Any:
+@overload
+def decode_json(value: str | bytes, target_type: type[T], type_decoders: TypeDecodersSequence | None) -> T:
+    ...
+
+
+def decode_json(  # type: ignore
+    value: str | bytes,
+    target_type: type[T] | EmptyType = Empty,  # pyright: ignore
+    type_decoders: TypeDecodersSequence | None = None,
+) -> Any:
     """Decode a JSON string/bytes into an object.
 
     Args:
-        raw: Value to decode
-        type_: An optional type to decode the data into
+        value: Value to decode
+        target_type: An optional type to decode the data into
+        type_decoders: Optional sequence of type decoders
 
     Returns:
         An object
 
     Raises:
-        SerializationException: If error decoding ``raw``.
+        SerializationException: If error decoding ``value``.
     """
     try:
-        if type_ is Empty:
-            return _msgspec_json_decoder.decode(raw)
-        return msgspec.json.decode(raw, dec_hook=dec_hook, type=type_)
+        if target_type is Empty:
+            return _msgspec_json_decoder.decode(value)
+        return msgspec.json.decode(
+            value, dec_hook=partial(default_deserializer, type_decoders=type_decoders), type=target_type
+        )
     except msgspec.DecodeError as msgspec_error:
         raise SerializationException(str(msgspec_error)) from msgspec_error
 
 
-def encode_msgpack(obj: Any, enc_hook: Callable[[Any], Any] | None = default_serializer) -> bytes:
+def encode_msgpack(value: Any, serializer: Callable[[Any], Any] | None = default_serializer) -> bytes:
     """Encode a value into MessagePack.
 
     Args:
-        obj: Value to encode
-        enc_hook: Optional callable to support non-natively supported types
+        value: Value to encode
+        serializer: Optional callable to support non-natively supported types
 
     Returns:
         MessagePack as bytes
 
     Raises:
         SerializationException: If error encoding ``obj``.
     """
     try:
-        if enc_hook is None or enc_hook is default_serializer:
-            return _msgspec_msgpack_encoder.encode(obj)
-        return msgspec.msgpack.encode(obj, enc_hook=enc_hook)
+        if serializer is None or serializer is default_serializer:
+            return _msgspec_msgpack_encoder.encode(value)
+        return msgspec.msgpack.encode(value, enc_hook=serializer)
     except (TypeError, msgspec.EncodeError) as msgspec_error:
         raise SerializationException(str(msgspec_error)) from msgspec_error
 
 
 @overload
-def decode_msgpack(raw: bytes) -> Any:
+def decode_msgpack(value: bytes) -> Any:
     ...
 
 
 @overload
-def decode_msgpack(raw: bytes, type_: type[T]) -> T:
+def decode_msgpack(value: bytes, type_decoders: TypeDecodersSequence | None) -> Any:
     ...
 
 
-def decode_msgpack(raw: bytes, type_: Any = Empty) -> Any:
-    """Decode a MessagePack string/bytes into an object.
-
-    Args:
-        raw: Value to decode
-        type_: An optional type to decode the data into
+@overload
+def decode_msgpack(value: bytes, target_type: type[T]) -> T:
+    ...
 
-    Returns:
-        An object
 
-    Raises:
-        SerializationException: If error decoding ``raw``.
-    """
-    try:
-        if type_ is Empty:
-            return _msgspec_msgpack_decoder.decode(raw)
-        return msgspec.msgpack.decode(raw, dec_hook=dec_hook, type=type_)
-    except msgspec.DecodeError as msgspec_error:
-        raise SerializationException(str(msgspec_error)) from msgspec_error
+@overload
+def decode_msgpack(value: bytes, target_type: type[T], type_decoders: TypeDecodersSequence | None) -> T:
+    ...
 
 
-def decode_media_type(raw: bytes, media_type: MediaType | str, type_: Any) -> Any:
-    """Decode a raw value into an object.
+def decode_msgpack(value: bytes, target_type: type[T] | EmptyType = Empty, type_decoders: TypeDecodersSequence | None = None) -> Any:  # type: ignore[misc]
+    """Decode a MessagePack string/bytes into an object.
 
     Args:
-        raw: Value to decode
-        media_type: Media type of the value
-        type_: An optional type to decode the data into
+        value: Value to decode
+        target_type: An optional type to decode the data into
+        type_decoders: Optional sequence of type decoders
 
     Returns:
         An object
 
     Raises:
-        SerializationException: If error decoding ``raw`` or ``media_type`` unsupported.
+        SerializationException: If error decoding ``value``.
     """
-    if media_type == MediaType.JSON:
-        return decode_json(raw, type_=type_)
-
-    if media_type == MediaType.MESSAGEPACK:
-        return decode_msgpack(raw, type_=type_)
-
-    raise SerializationException(f"Unsupported media type: '{media_type}'")
+    try:
+        if target_type is Empty:
+            return _msgspec_msgpack_decoder.decode(value)
+        return msgspec.msgpack.decode(
+            value, dec_hook=partial(default_deserializer, type_decoders=type_decoders), type=target_type
+        )
+    except msgspec.DecodeError as msgspec_error:
+        raise SerializationException(str(msgspec_error)) from msgspec_error
 
 
 def get_serializer(type_encoders: TypeEncodersMap | None = None) -> Serializer:
     """Get the serializer for the given type encoders."""
 
     if type_encoders:
-        return partial(default_serializer, type_encoders={**DEFAULT_TYPE_ENCODERS, **type_encoders})
+        return partial(default_serializer, type_encoders=type_encoders)
 
     return default_serializer
```

### Comparing `litestar-2.0.0b2/litestar/static_files/base.py` & `litestar-2.0.0b3/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/static_files/config.py` & `litestar-2.0.0b3/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/status_codes.py` & `litestar-2.0.0b3/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/stores/base.py` & `litestar-2.0.0b3/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/stores/file.py` & `litestar-2.0.0b3/litestar/stores/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             data = await path.read_bytes()
             return StorageObject.from_bytes(data)
         except FileNotFoundError:
             return None
 
     def _write_sync(self, target_file: Path, storage_obj: StorageObject) -> None:
         try:
-            tmp_file_fd, tmp_file_name = mkstemp(dir=self.path, prefix=target_file.name + ".tmp")
+            tmp_file_fd, tmp_file_name = mkstemp(dir=self.path, prefix=f"{target_file.name}.tmp")
             renamed = False
             try:
                 try:
                     os.write(tmp_file_fd, storage_obj.to_bytes())
                 finally:
                     os.close(tmp_file_fd)
```

### Comparing `litestar-2.0.0b2/litestar/stores/memory.py` & `litestar-2.0.0b3/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/stores/redis.py` & `litestar-2.0.0b3/litestar/stores/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,10 +169,8 @@
         return await self._redis.exists(self._make_key(key)) == 1
 
     async def expires_in(self, key: str) -> int | None:
         """Get the time in seconds ``key`` expires in. If no such ``key`` exists or no
         expiry time was set, return ``None``.
         """
         ttl = await self._redis.ttl(self._make_key(key))
-        if ttl == -2:
-            return None
-        return ttl
+        return None if ttl == -2 else ttl
```

### Comparing `litestar-2.0.0b2/litestar/stores/registry.py` & `litestar-2.0.0b3/litestar/stores/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,11 +55,10 @@
 
         Args:
             name: Name of the store
 
         Returns:
             A :class:`Store <.base.Store>`
         """
-        store = self._stores.get(name)
-        if not store:
-            store = self._stores[name] = self._default_factory(name)
-        return store
+        if not self._stores.get(name):
+            self._stores[name] = self._default_factory(name)
+        return self._stores[name]
```

### Comparing `litestar-2.0.0b2/litestar/template/base.py` & `litestar-2.0.0b3/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/template/config.py` & `litestar-2.0.0b3/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/testing/__init__.py` & `litestar-2.0.0b3/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/testing/client/__init__.py` & `litestar-2.0.0b3/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/testing/client/async_client.py` & `litestar-2.0.0b3/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/testing/client/base.py` & `litestar-2.0.0b3/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/testing/client/sync_client.py` & `litestar-2.0.0b3/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/testing/helpers.py` & `litestar-2.0.0b3/litestar/testing/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,14 @@
     static_files_config: OptionalSequence[StaticFilesConfig] | None = None,
     stores: StoreRegistry | dict[str, Store] | None = None,
     tags: Sequence[str] | None = None,
     template_config: TemplateConfig | None = None,
     timeout: float | None = None,
     type_encoders: TypeEncodersMap | None = None,
     websocket_class: type[WebSocket] | None = None,
-    _preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
 ) -> TestClient[Litestar]:
     """Create a Litestar app instance and initializes it.
 
     :class:`TestClient <litestar.testing.TestClient>` with it.
 
     Notes:
         - This function should be called as a context manager to ensure async startup and shutdown are
@@ -277,15 +276,14 @@
         state=state,
         static_files_config=static_files_config,
         stores=stores,
         tags=tags,
         template_config=template_config,
         type_encoders=type_encoders,
         websocket_class=websocket_class,
-        _preferred_validation_backend=_preferred_validation_backend,
     )
 
     return TestClient[Litestar](
         app=app,
         backend=backend,
         backend_options=backend_options,
         base_url=base_url,
@@ -347,15 +345,14 @@
     static_files_config: OptionalSequence[StaticFilesConfig] | None = None,
     stores: StoreRegistry | dict[str, Store] | None = None,
     tags: Sequence[str] | None = None,
     template_config: TemplateConfig | None = None,
     timeout: float | None = None,
     type_encoders: TypeEncodersMap | None = None,
     websocket_class: type[WebSocket] | None = None,
-    _preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
 ) -> AsyncTestClient[Litestar]:
     """Create a Litestar app instance and initializes it.
 
     :class:`TestClient <litestar.testing.TestClient>` with it.
 
     Notes:
         - This function should be called as a context manager to ensure async startup and shutdown are
@@ -521,15 +518,14 @@
         state=state,
         static_files_config=static_files_config,
         stores=stores,
         tags=tags,
         template_config=template_config,
         type_encoders=type_encoders,
         websocket_class=websocket_class,
-        _preferred_validation_backend=_preferred_validation_backend,
     )
 
     return AsyncTestClient[Litestar](
         app=app,
         backend=backend,
         backend_options=backend_options,
         base_url=base_url,
```

### Comparing `litestar-2.0.0b2/litestar/testing/life_span_handler.py` & `litestar-2.0.0b3/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/testing/request_factory.py` & `litestar-2.0.0b3/litestar/testing/request_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from dataclasses import asdict
+from typing import TYPE_CHECKING, Any, cast
 from urllib.parse import urlencode
 
 from httpx._content import encode_json as httpx_encode_json
 from httpx._content import encode_multipart_data, encode_urlencoded_data
-from pydantic import BaseModel
+from msgspec import Struct, to_builtins
 
 from litestar.app import Litestar
 from litestar.connection import Request
 from litestar.enums import HttpMethod, ParamType, RequestEncodingType, ScopeType
 from litestar.handlers.http_handlers import get
 from litestar.serialization import decode_json, encode_json
-from litestar.types import HTTPScope, RouteHandlerType
+from litestar.types import DataContainerType, HTTPScope, RouteHandlerType
 from litestar.types.asgi_types import ASGIVersion
+from litestar.utils import is_attrs_class, is_dataclass_instance, is_pydantic_model_instance
 
 if TYPE_CHECKING:
     from httpx._types import FileTypes
 
     from litestar.datastructures.cookie import Cookie
     from litestar.handlers.http_handlers import HTTPRouteHandler
 
@@ -205,15 +207,15 @@
         path: str,
         headers: dict[str, str] | None = None,
         cookies: list[Cookie] | str | None = None,
         session: dict[str, Any] | None = None,
         user: Any = None,
         auth: Any = None,
         request_media_type: RequestEncodingType = RequestEncodingType.JSON,
-        data: dict[str, Any] | BaseModel | None = None,
+        data: dict[str, Any] | DataContainerType | None = None,  # pyright: ignore
         files: dict[str, FileTypes] | list[tuple[str, FileTypes]] | None = None,
         query_params: dict[str, str | list[str]] | None = None,
         state: dict[str, Any] | None = None,
         path_params: dict[str, str] | None = None,
         http_version: str | None = "1.1",
         route_handler: RouteHandlerType | None = None,
     ) -> Request[Any, Any, Any]:
@@ -225,16 +227,15 @@
             headers: A dictionary of headers.
             cookies: A string representing the cookie header or a list of "Cookie" instances.
                 This value can include multiple cookies.
             session: A dictionary of session data.
             user: A value for `request.scope["user"]`
             auth: A value for `request.scope["auth"]`
             request_media_type: The 'Content-Type' header of the request.
-            data: A value for the request's body. Can be either a pydantic model instance
-                or a string keyed dictionary.
+            data: A value for the request's body. Can be any supported serializable type.
             files: A dictionary of files to be sent with the request.
             query_params: A dictionary of values from which the request's query will be generated.
             state: Arbitrary request state.
             path_params: A string keyed dictionary of path parameter values.
             http_version: HTTP version. Defaults to "1.1".
             route_handler: A route handler instance or method. If not provided a default handler is set.
 
@@ -252,22 +253,33 @@
             path_params=path_params,
             http_version=http_version,
             route_handler=route_handler,
         )
 
         headers = headers or {}
         if data:
-            if isinstance(data, BaseModel):
-                data = data.dict()
+            if isinstance(data, Struct):
+                data = to_builtins(data)
+            elif is_dataclass_instance(data):
+                data = asdict(data)
+            elif is_attrs_class(type(data)):
+                from attr import asdict as attrs_as_dict
+
+                data = attrs_as_dict(data)  # type: ignore[arg-type]
+            elif is_pydantic_model_instance(data):
+                from litestar.contrib.pydantic import _model_dump
+
+                data = _model_dump(data)
+
             if request_media_type == RequestEncodingType.JSON:
                 encoding_headers, stream = httpx_encode_json(data)
             elif request_media_type == RequestEncodingType.MULTI_PART:
-                encoding_headers, stream = encode_multipart_data(data, files=files or [], boundary=None)  # type: ignore[assignment]
+                encoding_headers, stream = encode_multipart_data(cast("dict[str, Any]", data), files=files or [], boundary=None)  # type: ignore[assignment]
             else:
-                encoding_headers, stream = encode_urlencoded_data(decode_json(encode_json(data)))
+                encoding_headers, stream = encode_urlencoded_data(decode_json(value=encode_json(data)))
             headers.update(encoding_headers)
             body = b""
             for chunk in stream:
                 body += chunk
             scope["_body"] = body  # type: ignore[typeddict-unknown-key]
         else:
             scope["_body"] = b""  # type: ignore[typeddict-unknown-key]
@@ -329,15 +341,15 @@
         path: str = "/",
         headers: dict[str, str] | None = None,
         cookies: list[Cookie] | str | None = None,
         session: dict[str, Any] | None = None,
         user: Any = None,
         auth: Any = None,
         request_media_type: RequestEncodingType = RequestEncodingType.JSON,
-        data: dict[str, Any] | BaseModel | None = None,
+        data: dict[str, Any] | DataContainerType | None = None,  # pyright: ignore
         query_params: dict[str, str | list[str]] | None = None,
         state: dict[str, Any] | None = None,
         path_params: dict[str, str] | None = None,
         http_version: str | None = "1.1",
         route_handler: RouteHandlerType | None = None,
     ) -> Request[Any, Any, Any]:
         """Create a POST :class:`Request <litestar.connection.Request>` instance.
@@ -347,16 +359,15 @@
             headers: A dictionary of headers.
             cookies: A string representing the cookie header or a list of "Cookie" instances.
                 This value can include multiple cookies.
             session: A dictionary of session data.
             user: A value for `request.scope["user"]`.
             auth: A value for `request.scope["auth"]`.
             request_media_type: The 'Content-Type' header of the request.
-            data: A value for the request's body. Can be either a pydantic model instance
-                or a string keyed dictionary.
+            data: A value for the request's body. Can be any supported serializable type.
             query_params: A dictionary of values from which the request's query will be generated.
             state: Arbitrary request state.
             path_params: A string keyed dictionary of path parameter values.
             http_version: HTTP version. Defaults to "1.1".
             route_handler: A route handler instance or method. If not provided a default handler is set.
 
         Returns:
@@ -384,15 +395,15 @@
         path: str = "/",
         headers: dict[str, str] | None = None,
         cookies: list[Cookie] | str | None = None,
         session: dict[str, Any] | None = None,
         user: Any = None,
         auth: Any = None,
         request_media_type: RequestEncodingType = RequestEncodingType.JSON,
-        data: dict[str, Any] | BaseModel | None = None,
+        data: dict[str, Any] | DataContainerType | None = None,  # pyright: ignore
         query_params: dict[str, str | list[str]] | None = None,
         state: dict[str, Any] | None = None,
         path_params: dict[str, str] | None = None,
         http_version: str | None = "1.1",
         route_handler: RouteHandlerType | None = None,
     ) -> Request[Any, Any, Any]:
         """Create a PUT :class:`Request <litestar.connection.Request>` instance.
@@ -402,16 +413,15 @@
             headers: A dictionary of headers.
             cookies: A string representing the cookie header or a list of "Cookie" instances.
                 This value can include multiple cookies.
             session: A dictionary of session data.
             user: A value for `request.scope["user"]`.
             auth: A value for `request.scope["auth"]`.
             request_media_type: The 'Content-Type' header of the request.
-            data: A value for the request's body. Can be either a pydantic model instance
-                or a string keyed dictionary.
+            data: A value for the request's body. Can be any supported serializable type.
             query_params: A dictionary of values from which the request's query will be generated.
             state: Arbitrary request state.
             path_params: A string keyed dictionary of path parameter values.
             http_version: HTTP version. Defaults to "1.1".
             route_handler: A route handler instance or method. If not provided a default handler is set.
 
         Returns:
@@ -439,15 +449,15 @@
         path: str = "/",
         headers: dict[str, str] | None = None,
         cookies: list[Cookie] | str | None = None,
         session: dict[str, Any] | None = None,
         user: Any = None,
         auth: Any = None,
         request_media_type: RequestEncodingType = RequestEncodingType.JSON,
-        data: dict[str, Any] | BaseModel | None = None,
+        data: dict[str, Any] | DataContainerType | None = None,  # pyright: ignore
         query_params: dict[str, str | list[str]] | None = None,
         state: dict[str, Any] | None = None,
         path_params: dict[str, str] | None = None,
         http_version: str | None = "1.1",
         route_handler: RouteHandlerType | None = None,
     ) -> Request[Any, Any, Any]:
         """Create a PATCH :class:`Request <litestar.connection.Request>` instance.
@@ -457,16 +467,15 @@
             headers: A dictionary of headers.
             cookies: A string representing the cookie header or a list of "Cookie" instances.
                 This value can include multiple cookies.
             session: A dictionary of session data.
             user: A value for `request.scope["user"]`.
             auth: A value for `request.scope["auth"]`.
             request_media_type: The 'Content-Type' header of the request.
-            data: A value for the request's body. Can be either a pydantic model instance
-                or a string keyed dictionary.
+            data: A value for the request's body. Can be any supported serializable type.
             query_params: A dictionary of values from which the request's query will be generated.
             state: Arbitrary request state.
             path_params: A string keyed dictionary of path parameter values.
             http_version: HTTP version. Defaults to "1.1".
             route_handler: A route handler instance or method. If not provided a default handler is set.
 
         Returns:
```

### Comparing `litestar-2.0.0b2/litestar/testing/transport.py` & `litestar-2.0.0b3/litestar/testing/transport.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/testing/websocket_test_session.py` & `litestar-2.0.0b3/litestar/testing/websocket_test_session.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/types/__init__.py` & `litestar-2.0.0b3/litestar/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,28 +64,29 @@
     ExceptionHandlersMap,
     Middleware,
     ParametersMap,
     PathType,
     ResponseCookies,
     ResponseHeaders,
     Scopes,
+    TypeDecodersSequence,
     TypeEncodersMap,
 )
 from .empty import Empty, EmptyType
 from .file_types import FileInfo, FileSystemProtocol
 from .helper_types import AnyIOBackend, MaybePartial, OptionalSequence, StreamType, SyncOrAsyncUnion
 from .internal_types import (
     ControllerRouterHandler,
     ReservedKwargs,
     ResponseType,
     RouteHandlerMapItem,
     RouteHandlerType,
 )
 from .protocols import DataclassProtocol, Logger
-from .serialization import LitestarEncodableType
+from .serialization import DataContainerType, LitestarEncodableType
 
 __all__ = (
     "ASGIApp",
     "ASGIVersion",
     "AfterExceptionHookHandler",
     "AfterRequestHookHandler",
     "AfterResponseHookHandler",
@@ -94,14 +95,15 @@
     "AnyIOBackend",
     "AsyncAnyCallable",
     "BaseScope",
     "BeforeMessageSendHookHandler",
     "BeforeRequestHookHandler",
     "CacheKeyBuilder",
     "ControllerRouterHandler",
+    "DataContainerType",
     "DataclassProtocol",
     "Dependencies",
     "Empty",
     "EmptyType",
     "ExceptionHandler",
     "ExceptionHandlersMap",
     "FileInfo",
@@ -150,14 +152,15 @@
     "Scope",
     "ScopeSession",
     "Scopes",
     "Send",
     "Serializer",
     "StreamType",
     "SyncOrAsyncUnion",
+    "TypeDecodersSequence",
     "TypeEncodersMap",
     "TypedDictClass",
     "WebSocketAcceptEvent",
     "WebSocketCloseEvent",
     "WebSocketConnectEvent",
     "WebSocketDisconnectEvent",
     "WebSocketReceiveEvent",
```

### Comparing `litestar-2.0.0b2/litestar/types/asgi_types.py` & `litestar-2.0.0b3/litestar/types/asgi_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,19 @@
     Any,
     Awaitable,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
-    Optional,
     Tuple,
     TypedDict,
     Union,
 )
 
-from pydantic import BaseModel
-
-from litestar.types.empty import EmptyType
-
 __all__ = (
     "ASGIApp",
     "ASGIVersion",
     "BaseScope",
     "HeaderScope",
     "HTTPDisconnectEvent",
     "HTTPReceiveMessage",
@@ -92,25 +87,26 @@
     "WebSocketResponseBodyEvent",
     "WebSocketResponseStartEvent",
     "WebSocketScope",
     "WebSocketSendEvent",
     "WebSocketSendMessage",
 )
 
-
 if TYPE_CHECKING:
     from typing_extensions import TypeAlias
 
     from litestar.app import Litestar
     from litestar.enums import ScopeType
+    from litestar.types.empty import EmptyType
 
     from .internal_types import LitestarType, RouteHandlerType
+    from .serialization import DataContainerType
 
 Method: TypeAlias = Literal["GET", "POST", "DELETE", "PATCH", "PUT", "HEAD", "TRACE", "OPTIONS"]
-ScopeSession: TypeAlias = Optional[Union[EmptyType, Dict[str, Any], BaseModel]]
+ScopeSession: TypeAlias = "EmptyType | Dict[str, Any] | DataContainerType | None"
 
 
 class ASGIVersion(TypedDict):
     """ASGI spec version."""
 
     spec_version: str
     version: Literal["3.0"]
```

### Comparing `litestar-2.0.0b2/litestar/types/builtin_types.py` & `litestar-2.0.0b3/litestar/types/builtin_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/types/callable_types.py` & `litestar-2.0.0b3/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/types/composite_types.py` & `litestar-2.0.0b3/litestar/types/composite_types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,55 @@
 from __future__ import annotations
 
-from os import PathLike
-from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterator,
     Literal,
     Mapping,
     MutableMapping,
     Sequence,
-    Set,
     Tuple,
     Type,
     Union,
 )
 
-from litestar.enums import ScopeType
-
-from .callable_types import AnyCallable, ExceptionHandler
-
 __all__ = (
     "Dependencies",
     "ExceptionHandlersMap",
     "Middleware",
     "ParametersMap",
     "PathType",
     "ResponseCookies",
     "ResponseHeaders",
     "Scopes",
     "TypeEncodersMap",
 )
 
 if TYPE_CHECKING:
+    from os import PathLike
+    from pathlib import Path
+
     from typing_extensions import TypeAlias
 
     from litestar.datastructures.cookie import Cookie
     from litestar.datastructures.response_header import ResponseHeader
     from litestar.di import Provide
+    from litestar.enums import ScopeType
     from litestar.middleware.base import DefineMiddleware, MiddlewareProtocol
     from litestar.params import ParameterKwarg
 
     from .asgi_types import ASGIApp
+    from .callable_types import AnyCallable, ExceptionHandler
 
-    Dependencies: TypeAlias = Mapping[str, Union[Provide, AnyCallable]]
-    Middleware: TypeAlias = Union[
-        Callable[..., ASGIApp], DefineMiddleware, Iterator[Tuple[ASGIApp, Dict[str, Any]]], Type[MiddlewareProtocol]
-    ]
-    ParametersMap: TypeAlias = Mapping[str, ParameterKwarg]
-    ResponseCookies: TypeAlias = Union[Sequence[Cookie], Mapping[str, str]]
-    ResponseHeaders: TypeAlias = Union[Sequence[ResponseHeader], Mapping[str, str]]
-else:
-    Dependencies: TypeAlias = Any
-    Middleware: TypeAlias = Any
-    ParametersMap: TypeAlias = Any
-    ResponseCookies: TypeAlias = Any
-    ResponseHeaders: TypeAlias = Any
-
-ExceptionHandlersMap: TypeAlias = MutableMapping[Union[int, Type[Exception]], ExceptionHandler]
-PathType: TypeAlias = Union[Path, PathLike, str]
-Scopes: TypeAlias = Set[Literal[ScopeType.HTTP, ScopeType.WEBSOCKET]]
-TypeEncodersMap: TypeAlias = Mapping[Any, Callable[[Any], Any]]
+Dependencies: TypeAlias = "Mapping[str, Union[Provide, AnyCallable]]"
+ExceptionHandlersMap: TypeAlias = "MutableMapping[Union[int, Type[Exception]], ExceptionHandler]"
+Middleware: TypeAlias = "Union[Callable[..., ASGIApp], DefineMiddleware, Iterator[Tuple[ASGIApp, Dict[str, Any]]], Type[MiddlewareProtocol]]"
+ParametersMap: TypeAlias = "Mapping[str, ParameterKwarg]"
+PathType: TypeAlias = "Union[Path, PathLike, str]"
+ResponseCookies: TypeAlias = "Union[Sequence[Cookie], Mapping[str, str]]"
+ResponseHeaders: TypeAlias = "Union[Sequence[ResponseHeader], Mapping[str, str]]"
+Scopes: TypeAlias = "set[Literal[ScopeType.HTTP, ScopeType.WEBSOCKET]]"
+TypeDecodersSequence: TypeAlias = "Sequence[tuple[Callable[[Any], bool], Callable[[Any, Any], Any]]]"
+TypeEncodersMap: TypeAlias = "Mapping[Any, Callable[[Any], Any]]"
```

### Comparing `litestar-2.0.0b2/litestar/types/file_types.py` & `litestar-2.0.0b3/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/types/helper_types.py` & `litestar-2.0.0b3/litestar/types/helper_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import (
+    TYPE_CHECKING,
     AsyncIterable,
     AsyncIterator,
     Awaitable,
     Iterable,
     Iterator,
     Literal,
     Optional,
     Sequence,
     TypeVar,
     Union,
 )
 
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
+
 T = TypeVar("T")
 
 __all__ = ("OptionalSequence", "SyncOrAsyncUnion", "AnyIOBackend", "StreamType", "MaybePartial")
 
-OptionalSequence = Optional[Sequence[T]]
+OptionalSequence: TypeAlias = Optional[Sequence[T]]
 """Types 'T' as union of Sequence[T] and None."""
 
-SyncOrAsyncUnion = Union[T, Awaitable[T]]
+SyncOrAsyncUnion: TypeAlias = Union[T, Awaitable[T]]
 """Types 'T' as a union of T and awaitable T."""
 
 
-AnyIOBackend = Literal["asyncio", "trio"]
+AnyIOBackend: TypeAlias = Literal["asyncio", "trio"]
 """Anyio backend names."""
 
-StreamType = Union[Iterable[T], Iterator[T], AsyncIterable[T], AsyncIterator[T]]
+StreamType: TypeAlias = Union[Iterable[T], Iterator[T], AsyncIterable[T], AsyncIterator[T]]
 """A stream type."""
 
-MaybePartial = Union[T, partial]
+MaybePartial: TypeAlias = Union[T, partial]
 """A potentially partial callable."""
```

### Comparing `litestar-2.0.0b2/litestar/types/internal_types.py` & `litestar-2.0.0b3/litestar/types/internal_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     Dict,
     Literal,
     NamedTuple,
     Union,
 )
 
 __all__ = (
-    "AnyConnection",
     "ControllerRouterHandler",
     "LitestarType",
     "PathParameterDefinition",
     "PathParameterDefinition",
     "ReservedKwargs",
     "ResponseType",
     "RouteHandlerMapItem",
@@ -23,32 +22,29 @@
 )
 
 
 if TYPE_CHECKING:
     from typing_extensions import TypeAlias
 
     from litestar.app import Litestar
-    from litestar.connection import ASGIConnection
     from litestar.controller import Controller
     from litestar.handlers.asgi_handlers import ASGIRouteHandler
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.handlers.websocket_handlers import WebsocketRouteHandler
     from litestar.response import Response
     from litestar.router import Router
     from litestar.types import Method
 
-    AnyConnection: TypeAlias = ASGIConnection[Any, Any, Any, Any]
     ReservedKwargs: TypeAlias = Literal["request", "socket", "headers", "query", "cookies", "state", "data"]
     LitestarType: TypeAlias = Litestar
     RouteHandlerType: TypeAlias = Union[HTTPRouteHandler, WebsocketRouteHandler, ASGIRouteHandler]
     ResponseType: TypeAlias = type[Response]
     ControllerRouterHandler: TypeAlias = Union[type[Controller], RouteHandlerType, Router, Callable[..., Any]]
     RouteHandlerMapItem: TypeAlias = Dict[Union[Method, Literal["websocket", "asgi"]], RouteHandlerType]
 else:
-    AnyConnection: TypeAlias = Any
     ReservedKwargs: TypeAlias = Any
     LitestarType: TypeAlias = Any
     RouteHandlerType: TypeAlias = Any
     ResponseType: TypeAlias = Any
     ControllerRouterHandler: TypeAlias = Any
     RouteHandlerMapItem: TypeAlias = Any
```

### Comparing `litestar-2.0.0b2/litestar/types/protocols.py` & `litestar-2.0.0b3/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/types/serialization.py` & `litestar-2.0.0b3/litestar/types/serialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from collections import deque
     from collections.abc import Collection
     from datetime import date, datetime, time
     from decimal import Decimal
     from enum import Enum, IntEnum
@@ -18,45 +18,44 @@
     )
     from pathlib import Path, PurePath
     from re import Pattern
     from uuid import UUID
 
     from msgspec import Raw, Struct
     from msgspec.msgpack import Ext
-    from pydantic import (
-        BaseModel,
-        ByteSize,
-        ConstrainedBytes,
-        ConstrainedDate,
-        NameEmail,
-        SecretField,
-        StrictBool,
-    )
-    from pydantic.color import Color
     from typing_extensions import TypeAlias
 
-    from litestar.types import DataclassProtocol
+    from litestar.types import DataclassProtocol, TypedDictClass
+
+    try:
+        from pydantic import BaseModel
+    except ImportError:
+        BaseModel = Any  # type: ignore
+
+    try:
+        from attrs import AttrsInstance
+    except ImportError:
+        AttrsInstance = Any  # type: ignore
 
 __all__ = (
     "LitestarEncodableType",
     "EncodableBuiltinType",
     "EncodableBuiltinCollectionType",
     "EncodableStdLibType",
     "EncodableStdLibIPType",
     "EncodableMsgSpecType",
-    "EncodablePydanticType",
+    "DataContainerType",
 )
 
 EncodableBuiltinType: TypeAlias = "None | bool | int | float | str | bytes | bytearray"
 EncodableBuiltinCollectionType: TypeAlias = "list | tuple | set | frozenset | dict | Collection"
 EncodableStdLibType: TypeAlias = (
     "date | datetime | deque | time | UUID | Decimal | Enum | IntEnum | DataclassProtocol | Path | PurePath | Pattern"
 )
 EncodableStdLibIPType: TypeAlias = (
     "IPv4Address | IPv4Interface | IPv4Network | IPv6Address | IPv6Interface | IPv6Network"
 )
 EncodableMsgSpecType: TypeAlias = "Ext | Raw | Struct"
-EncodablePydanticType: TypeAlias = (
-    "BaseModel | ByteSize | ConstrainedBytes | ConstrainedDate | NameEmail | SecretField | StrictBool | Color"
+LitestarEncodableType: TypeAlias = "EncodableBuiltinType | EncodableBuiltinCollectionType | EncodableStdLibType | EncodableStdLibIPType | EncodableMsgSpecType | BaseModel | AttrsInstance"  # pyright: ignore
+DataContainerType: TypeAlias = (
+    "Struct | BaseModel | AttrsInstance | TypedDictClass | DataclassProtocol"  # pyright: ignore
 )
-
-LitestarEncodableType: TypeAlias = "EncodableBuiltinType | EncodableBuiltinCollectionType | EncodableStdLibType | EncodableStdLibIPType | EncodableMsgSpecType | EncodablePydanticType"
```

### Comparing `litestar-2.0.0b2/litestar/utils/__init__.py` & `litestar-2.0.0b3/litestar/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     is_mapping,
     is_non_string_iterable,
     is_non_string_sequence,
     is_optional_union,
     is_pydantic_constrained_field,
     is_pydantic_model_class,
     is_pydantic_model_instance,
+    is_struct_class,
+    is_sync_or_async_generator,
     is_typed_dict,
+    is_undefined_sentinel,
     is_union,
 )
 from .scope import (
     delete_litestar_scope_state,
     get_litestar_scope_state,
     get_serializer_from_scope,
     set_litestar_scope_state,
@@ -44,31 +47,34 @@
     "encode_headers",
     "find_index",
     "get_enum_string_value",
     "get_litestar_scope_state",
     "get_name",
     "get_origin_or_inner_type",
     "get_serializer_from_scope",
-    "is_any",
     "is_annotated_type",
+    "is_any",
     "is_async_callable",
     "is_attrs_class",
     "is_class_and_subclass",
     "is_class_var",
     "is_dataclass_class",
     "is_dataclass_instance",
     "is_generic",
     "is_mapping",
     "is_non_string_iterable",
     "is_non_string_sequence",
     "is_optional_union",
     "is_pydantic_constrained_field",
     "is_pydantic_model_class",
     "is_pydantic_model_instance",
+    "is_struct_class",
+    "is_sync_or_async_generator",
     "is_typed_dict",
+    "is_undefined_sentinel",
     "is_union",
     "join_paths",
     "make_non_optional_union",
     "normalize_path",
     "set_litestar_scope_state",
     "unique",
     "url_quote",
```

### Comparing `litestar-2.0.0b2/litestar/utils/compat.py` & `litestar-2.0.0b3/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/utils/dataclass.py` & `litestar-2.0.0b3/litestar/utils/dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,32 +79,37 @@
         A tuple of key/value pairs.
     """
     dataclass_fields = extract_dataclass_fields(dt, exclude_none, exclude_empty, include, exclude)
     return tuple((field.name, getattr(dt, field.name)) for field in dataclass_fields)
 
 
 def simple_asdict(
-    obj: DataclassProtocol, exclude_none: bool = False, exclude_empty: bool = False, convert_nested: bool = True
+    obj: DataclassProtocol,
+    exclude_none: bool = False,
+    exclude_empty: bool = False,
+    convert_nested: bool = True,
+    exclude: set[str] | None = None,
 ) -> dict[str, Any]:
     """Convert a dataclass to a dictionary.
 
     This method has important differences to the standard library version:
     - it does not deepcopy values
     - it does not recurse into collections
 
     Args:
         obj: A dataclass instance.
         exclude_none: Whether to exclude None values.
         exclude_empty: Whether to exclude Empty values.
         convert_nested: Whether to recursively convert nested dataclasses.
+        exclude: An iterable of fields to exclude.
 
     Returns:
         A dictionary of key/value pairs.
     """
     ret = {}
-    for field in extract_dataclass_fields(obj, exclude_none, exclude_empty):
+    for field in extract_dataclass_fields(obj, exclude_none, exclude_empty, exclude=exclude):
         value = getattr(obj, field.name)
         if is_dataclass_instance(value) and convert_nested:
             ret[field.name] = simple_asdict(value, exclude_none, exclude_empty)
         else:
             ret[field.name] = getattr(obj, field.name)
     return ret
```

### Comparing `litestar-2.0.0b2/litestar/utils/deprecation.py` & `litestar-2.0.0b3/litestar/utils/deprecation.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,20 @@
         access_type = "Use of"
 
     if pending:
         parts.append(f"{access_type} {kind} awaiting deprecation {deprecated_name!r}")
     else:
         parts.append(f"{access_type} deprecated {kind} {deprecated_name!r}")
 
-    parts.append(f"Deprecated in litestar {version}")
-    parts.append(f"This {kind} will be removed in {removal_in or 'the next major version'}")
-
+    parts.extend(
+        (
+            f"Deprecated in litestar {version}",
+            f"This {kind} will be removed in {removal_in or 'the next major version'}",
+        )
+    )
     if alternative:
         parts.append(f"Use {alternative!r} instead")
 
     if info:
         parts.append(info)
 
     text = ". ".join(parts)
```

### Comparing `litestar-2.0.0b2/litestar/utils/helpers.py` & `litestar-2.0.0b3/litestar/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     Args:
         local_cookies: Cookies returned from the local scope.
         layered_cookies: Cookies returned from the layers.
 
     Returns:
         A unified list of cookies
     """
-    return [cookie for cookie in {*local_cookies, *layered_cookies} if not cookie.documentation_only]  # noqa: PLC0208
+    return [cookie for cookie in {*local_cookies, *layered_cookies} if not cookie.documentation_only]
 
 
 def url_quote(value: str | bytes) -> str:
     """Quote a URL.
 
     Args:
         value: A URL.
```

### Comparing `litestar-2.0.0b2/litestar/utils/path.py` & `litestar-2.0.0b3/litestar/utils/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Args:
         path: Path string
 
     Returns:
         Path string
     """
     path = path.strip("/")
-    path = "/" + path
+    path = f"/{path}"
     return multi_slash_pattern.sub("/", path)
 
 
 def join_paths(paths: Iterable[str]) -> str:
     """Normalize and joins path fragments.
 
     Args:
```

### Comparing `litestar-2.0.0b2/litestar/utils/predicates.py` & `litestar-2.0.0b3/litestar/utils/predicates.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,52 +32,55 @@
     ParamSpec,
     TypeGuard,
     _AnnotatedAlias,
     get_args,
     is_typeddict,
 )
 
+from litestar.constants import UNDEFINED_SENTINELS
 from litestar.types import Empty
 from litestar.types.builtin_types import NoneType, UnionTypes
 from litestar.utils.typing import get_origin_or_inner_type
 
 if TYPE_CHECKING:
     from litestar.types.builtin_types import TypedDictClass
     from litestar.types.callable_types import AnyGenerator
     from litestar.types.protocols import DataclassProtocol
 
-
 try:
     import pydantic
 except ImportError:  # pragma: no cover
     pydantic = Empty  # type: ignore
 
 try:
     import attrs
 except ImportError:  # pragma: no cover
     attrs = Empty  # type: ignore
 
 __all__ = (
-    "is_async_callable",
+    "is_annotated_type",
     "is_any",
+    "is_async_callable",
     "is_attrs_class",
     "is_class_and_subclass",
     "is_class_var",
     "is_dataclass_class",
     "is_dataclass_instance",
     "is_generic",
     "is_mapping",
     "is_non_string_iterable",
     "is_non_string_sequence",
     "is_optional_union",
     "is_pydantic_constrained_field",
     "is_pydantic_model_class",
     "is_pydantic_model_instance",
+    "is_struct_class",
     "is_sync_or_async_generator",
     "is_typed_dict",
+    "is_undefined_sentinel",
     "is_union",
 )
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
@@ -91,15 +94,15 @@
     Returns:
         Bool determining if type of ``value`` is an awaitable.
     """
     while isinstance(value, partial):
         value = value.func  # type: ignore[unreachable]
 
     return iscoroutinefunction(value) or (
-        callable(value) and iscoroutinefunction(value.__call__)  #  type: ignore[operator]
+        callable(value) and iscoroutinefunction(value.__call__)  # type: ignore[operator]
     )
 
 
 def is_dataclass_instance(obj: Any) -> TypeGuard[DataclassProtocol]:
     """Check if an object is a dataclass instance.
 
     Args:
@@ -122,31 +125,31 @@
     """
     try:
         return isclass(annotation) and is_dataclass(annotation)
     except TypeError:  # pragma: no cover
         return False
 
 
-def is_class_and_subclass(annotation: Any, t_type: type[T]) -> TypeGuard[type[T]]:
+def is_class_and_subclass(annotation: Any, type_or_type_tuple: type[T] | tuple[type[T], ...]) -> TypeGuard[type[T]]:
     """Return ``True`` if ``value`` is a ``class`` and is a subtype of ``t_type``.
 
     See https://github.com/litestar-org/litestar/issues/367
 
     Args:
         annotation: The value to check if is class and subclass of ``t_type``.
-        t_type: Type used for :func:`issubclass` check of ``value``
+        type_or_type_tuple: Type used for :func:`issubclass` check of ``value``
 
     Returns:
         bool
     """
     origin = get_origin_or_inner_type(annotation)
     if not origin and not isclass(annotation):
         return False
     try:
-        return issubclass(origin or annotation, t_type)
+        return issubclass(origin or annotation, type_or_type_tuple)
     except TypeError:  # pragma: no cover
         return False
 
 
 def is_generic(annotation: Any) -> bool:
     """Given a type annotation determine if the annotation is a generic class.
 
@@ -315,17 +318,15 @@
 
     Args:
         annotation: A type.
 
     Returns:
         A typeguard determining whether the type is an attrs class.
     """
-    if attrs is not Empty:  # type: ignore[comparison-overlap]
-        return attrs.has(annotation)  # pyright: ignore
-    return False  # pragma: no cover
+    return attrs.has(annotation) if attrs is not Empty else False  # type: ignore[comparison-overlap]
 
 
 def is_pydantic_constrained_field(
     annotation: Any,
 ) -> Any:
     """Check if the given annotation is a constrained pydantic type.
 
@@ -347,15 +348,15 @@
             ConstrainedInt,
             ConstrainedList,
             ConstrainedSet,
             ConstrainedStr,
         )
 
         return any(
-            is_class_and_subclass(annotation, constrained_type)
+            is_class_and_subclass(annotation, constrained_type)  # type: ignore[arg-type]
             for constrained_type in (
                 ConstrainedBytes,
                 ConstrainedDate,
                 ConstrainedDecimal,
                 ConstrainedFloat,
                 ConstrainedFrozenSet,
                 ConstrainedInt,
@@ -411,7 +412,19 @@
     Args:
         annotation: A type annotation
 
     Returns:
         A boolean.
     """
     return isinstance(annotation, _AnnotatedAlias) and getattr(annotation, "__args__", None) is not None
+
+
+def is_undefined_sentinel(value: Any) -> bool:
+    """Check if the given value is the undefined sentinel.
+
+    Args:
+        value: A value to be tested for undefined sentinel.
+
+    Returns:
+        A boolean.
+    """
+    return any(v is value for v in UNDEFINED_SENTINELS)
```

### Comparing `litestar-2.0.0b2/litestar/utils/scope.py` & `litestar-2.0.0b3/litestar/utils/scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         default: Default value to return.
         pop: Boolean flag dictating whether the value should be deleted from the state.
 
     Returns:
         Value mapped to ``key`` in internal connection scope namespace.
     """
     namespace = scope["state"].setdefault(SCOPE_STATE_NAMESPACE, {})
-    return namespace.get(key, default) if not pop else namespace.pop(key, default)
+    return namespace.pop(key, default) if pop else namespace.get(key, default)
 
 
 def set_litestar_scope_state(scope: Scope, key: str, value: Any) -> None:
     """Set an internal value in connection scope state.
 
     Args:
         scope: The connection scope.
@@ -79,10 +79,9 @@
 
 def delete_litestar_scope_state(scope: Scope, key: str) -> None:
     """Delete an internal value from connection scope state.
 
     Args:
         scope: The connection scope.
         key: Key to set under internal namespace in scope state.
-        value: Value for key.
     """
     del scope["state"][SCOPE_STATE_NAMESPACE][key]
```

### Comparing `litestar-2.0.0b2/litestar/utils/sequence.py` & `litestar-2.0.0b3/litestar/utils/sequence.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,23 +4,20 @@
 
 __all__ = ("find_index", "unique", "compact")
 
 
 T = TypeVar("T")
 
 
-def find_index(target_list: list[T], predicate: Callable[[T], bool]) -> int:
+def find_index(target_list: Sequence[T], predicate: Callable[[T], bool]) -> int:
     """Find element in list given a key and value.
 
     List elements can be dicts or classes
     """
-    for i, element in enumerate(target_list):
-        if predicate(element):
-            return i
-    return -1
+    return next((i for i, element in enumerate(target_list) if predicate(element)), -1)
 
 
 def unique(value: Sequence[T]) -> list[T]:
     """Return all unique values in a given sequence or iterator."""
     try:
         return list(set(value))
     except TypeError:
```

### Comparing `litestar-2.0.0b2/litestar/utils/sync.py` & `litestar-2.0.0b3/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/utils/typing.py` & `litestar-2.0.0b3/litestar/utils/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "annotation_is_iterable_of_type",
     "get_instantiable_origin",
     "get_origin_or_inner_type",
     "get_safe_generic_origin",
     "instantiable_type_mapping",
     "make_non_optional_union",
     "unwrap_annotation",
+    "unwrap_union",
 )
 
 
 T = TypeVar("T")
 UnionT = TypeVar("UnionT", bound="Union")
 
 tuple_types_regex = re.compile(
```

### Comparing `litestar-2.0.0b2/litestar/utils/version.py` & `litestar-2.0.0b3/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/litestar/utils/warnings.py` & `litestar-2.0.0b3/litestar/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b2/pyproject.toml` & `litestar-2.0.0b3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "litestar"
-version = "2.0.0beta2"
+version = "2.0.0beta3"
 description = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
 maintainers = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
-    "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
 license = "MIT"
 readme = "docs/PYPI_README.md"
 homepage = "https://litestar.dev/"
@@ -44,14 +43,27 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "Typing :: Typed",
+    "Framework :: AsyncIO",
+    #    Pending trove-classifiers#148
+    #    "Framework :: Litestar",
+    #    "Framework :: Litestar :: 2",
+    "Framework :: Pydantic",
+    "Framework :: Pydantic :: 1",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: System Administrators",
+    "Topic :: Internet",
+    "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["CHANGELOG.rst"]
 packages = [{ include = "litestar" }]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc"
 "Changelog" = "https://github.com/litestar-org/litestar/releases/"
@@ -63,38 +75,34 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 alembic = { version = "*", optional = true }
 annotated-types = { version = "*", optional = true }
 anyio = ">=3"
 attrs = { version = "*", optional = true }
 brotli = { version = "*", optional = true }
-cattrs = { version = "*", optional = true }
 click = { version = "*", optional = true }
 cryptography = { version = "*", optional = true }
-fast-query-parsers = "*"
+fast-query-parsers = ">=1.0.2"
 httpx = ">=0.22"
 importlib-metadata = { version = "*", python = "<3.10" }
 importlib-resources = { version = ">=5.12.0", python = "<3.9" }
 jinja2 = { version = ">=3.1.2", optional = true }
 jsbeautifier = { version = "*", optional = true }
 mako = { version = ">=1.2.4", optional = true }
-msgspec = ">=0.16.0"
+msgspec = ">=0.17.0"
 multidict = ">=6.0.2"
 opentelemetry-instrumentation-asgi = { version = "*", optional = true }
+piccolo = { version = "*", optional = true }
 picologging = { version = "*", optional = true }
 polyfactory = ">=2.3.2"
-prometheus-client = {version = "*", optional = true}
-pydantic = "<2"
-python-dateutil = { version = "*", optional = true }
+prometheus-client = { version = "*", optional = true }
+pydantic = { version = "*", optional = true, extras = ["email"] }
 python-jose = { version = "*", optional = true }
-pytimeparse = { version = "*", optional = true }
 pyyaml = "*"
-redis = { version = ">=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3,!=4.5.5", optional = true, extras = [
-    "hiredis",
-] }
+redis = { version = ">=4.4.4, <4.5.0", optional = true, extras = ["hiredis"] }
 rich = { version = ">=13.0.0", optional = true }
 rich-click = { version = "*", optional = true }
 sqlalchemy = { version = ">=2.0.12", optional = true }
 structlog = { version = "*", optional = true }
 tortoise-orm = { version = ">=0.17.0", optional = true }
 typing-extensions = "*"
 uvicorn = { extras = ["standard"], version = ">=0.22.0", optional = true }
@@ -102,56 +110,53 @@
 [tool.poetry.group.dev.dependencies]
 aiosqlite = "*"
 alembic = "*"
 annotated-types = "*"
 asyncmy = "*"
 asyncpg = "*"
 attrs = "*"
-beanie = "*"
 beautifulsoup4 = "*"
 brotli = "*"
-cattrs = "*"
 click = "*"
 cryptography = "*"
 duckdb-engine = "*"
-fakeredis = { extras = ["lua"], version = "*" }
+fakeredis = { extras = ["lua"], version = "<2.17.0" }
 freezegun = "*"
 fsspec = "*"
 greenlet = "*"
 hypothesis = "*"
 jinja2 = "*"
 jsbeautifier = "*"
 mako = "*"
 mongomock-motor = { version = "*", markers = "sys_platform != 'win32'" }
 opentelemetry-instrumentation-asgi = "*"
 opentelemetry-sdk = "*"
 oracledb = "*"
-piccolo = "*"
 picologging = "*"
 pre-commit = "*"
 prometheus-client = "*"
 psycopg = "*"
+pydantic = "*"
+pydantic-extra-types = "*"
+email_validator = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-lazy-fixture = "*"
 pytest-mock = "*"
 pytest-rerunfailures = "*"
-python-dateutil = "*"
 python-dotenv = "*"
 python-jose = "*"
-pytimeparse = "*"
-redis = "*"
+redis = ">=4.4.4, <4.5.0"
 rich = "*"
 rich-click = "*"
 sqlalchemy = ">=2.0"
 sqlalchemy-spanner = "*"
 starlette = "*"
 structlog = "*"
-tortoise-orm = "*"
 trio = "*"
 uvicorn = "*"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
@@ -161,64 +166,64 @@
 sphinx = ">=5.3.0,<=6"
 sphinx-autobuild = "*"
 sphinx-copybutton = ">=0.5.1"
 sphinx-design = ">=0.3.0,<1"
 sphinxcontrib-mermaid = ">=0.8.1,<1"
 litestar-sphinx-theme = { git = "https://github.com/litestar-org/litestar-sphinx-theme.git" }
 uvicorn = "*"
+sphinx-click = "^4.4.0"
+piccolo = "*"                                                                                 # temporarily moved here because it depends on Pydantic <2 but we need it to generate the docs
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 asyncpg-stubs = "*"
 black = "*"
 blacken-docs = "*"
 mypy = "*"
 pyright = "*"
 ruff = '*'
 slotscheck = "*"
+sourcery = "*"
+types-beautifulsoup4 = "*"
 types-freezegun = "*"
 types-python-jose = "*"
 types-pyyaml = "*"
 types-redis = "*"
-types-beautifulsoup4 = "*"
-types-python-dateutil = "*"
 
 [tool.poetry.extras]
 annotated-types = ["annotated-types"]
-attrs = ["attrs", "cattrs", "python-dateutil", "pytimeparse"]
+attrs = ["attrs"]
+pydantic = ["pydantic"]
 brotli = ["brotli"]
 cli = ["click", "rich", "rich-click", "jsbeautifier", "uvicorn"]
 cryptography = ["cryptography"]
 jinja = ["jinja2"]
 jwt = ["python-jose", "cryptography"]
 opentelemetry = ["opentelemetry-instrumentation-asgi"]
 picologging = ["picologging"]
+prometheus = ["prometheus-client"]
 redis = ["redis"]
 sqlalchemy = ["sqlalchemy", "alembic"]
 standard = ["click", "jinja2", "jsbeautifier", "rich", "uvicorn", "rich-click"]
 structlog = ["structlog"]
 tortoise-orm = ["tortoise-orm"]
-prometheus = ["prometheus-client"]
 
 full = [
     "alembic",
     "attrs",
     "brotli",
-    "cattrs",
     "click",
     "cryptography",
     "jinja2",
     "jsbeautifier",
     "opentelemetry-instrumentation-asgi",
     "prometheus-client",
-    "python-dateutil",
     "python-jose",
-    "pytimeparse",
     "redis",
     "rich",
     "sqlalchemy",
     "structlog",
     "uvicorn",
 ]
 
@@ -244,14 +249,16 @@
 exclude_lines = [
     'pragma: no cover',
     'if TYPE_CHECKING:',
     'except ImportError as e:',
     'except ImportError:',
     '\.\.\.',
     'raise NotImplementedError',
+    'if VERSION.startswith("1"):',
+    'if pydantic.VERSION.startswith("1"):',
 ]
 
 [tool.pytest.ini_options]
 addopts = "--ignore=examples -m='not sqlalchemy_integration'"
 asyncio_mode = "auto"
 filterwarnings = [
     "ignore::trio.TrioDeprecationWarning:anyio._backends._trio*:164",
@@ -272,14 +279,50 @@
     "sqlalchemy_psycopg_sync: SQLAlchemy Postgres (psycopg sync) Tests",
     "sqlalchemy_sqlite: SQLAlchemy SQLite (sqlite) Tests",
     "sqlalchemy_oracledb: SQLAlchemy Oracle (oracledb) Tests",
     "sqlalchemy_spanner: SQLAlchemy Google Cloud Spanner (sqlalchemy-spanner) Tests",
     "sqlalchemy_duckdb: SQLAlchemy Duckdb (duckdb-engine) Tests",
 ]
 
+[tool.mypy]
+plugins = ["pydantic.mypy"]
+
+warn_unused_ignores = true
+warn_redundant_casts = true
+warn_unused_configs = true
+warn_unreachable = true
+warn_return_any = true
+strict = true
+disallow_untyped_decorators = true
+disallow_any_generics = false
+implicit_reexport = false
+show_error_codes = true
+
+[[tool.mypy.overrides]]
+module = ["tests.*.test_sqlalchemy_sync", "tests.*.test_sqlalchemy_async"]
+disable_error_code = "attr-defined"
+
+[[tool.mypy.overrides]]
+module = "tests.unit.test_contrib.test_sqlalchemy.test_dto"
+disable_error_code = ["arg-type", "misc", "valid-type", "var-annotated"]
+
+[[tool.mypy.overrides]]
+module = "tests.*"
+disallow_untyped_decorators = false
+
+[[tool.mypy.overrides]]
+module = ["mako.*", "pytimeparse.*", "brotli.*", "jsbeautifier.*"]
+ignore_missing_imports = true
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+warn_untyped_fields = true
+
 [tool.pyright]
 include = ["litestar", "tests", "examples"]
 exclude = [
     "examples/plugins/sqlalchemy_plugin",
     "litestar/openapi",
     "tests/unit/test_contrib/test_sqlalchemy/test_dto.py",
 ]
@@ -387,40 +430,17 @@
     "RSE",
     "S",
     "S101",
     "SIM",
     "TCH",
     "TRY",
 ]
+"tests/unit/test_contrib/test_sqlalchemy/**/*.*" = ["UP006"]
 "docs/examples/application_hooks/before_send_hook.py" = ["UP006"]
 "docs/examples/contrib/sqlalchemy/plugins/**/*.*" = ["UP006"]
-"docs/examples/tests/**/*.*" = [
-    "A",
-    "ARG",
-    "B",
-    "BLE",
-    "C901",
-    "D",
-    "DTZ",
-    "EM",
-    "FBT",
-    "G",
-    "N",
-    "PGH",
-    "PIE",
-    "PLR",
-    "PLW",
-    "PTH",
-    "RSE",
-    "S",
-    "S101",
-    "SIM",
-    "TCH",
-    "TRY",
-]
 "docs/**/*.*" = ["S", "B", "DTZ", "A", "TCH", "ERA", "D", "RET"]
 "docs/examples/**" = ["T201"]
 "docs/examples/data_transfer_objects**/*.*" = ["UP006"]
 "litestar/exceptions/*.*" = ["N818"]
 "litestar/handlers/**/*.*" = ["N801"]
 "litestar/_openapi/schema_generation/schema.py" = ["C901"]
 "litestar/params.py" = ["N802"]
```

